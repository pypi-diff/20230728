# Comparing `tmp/kast_flow_api_python-1.0.6rc2.tar.gz` & `tmp/kast_flow_api_python-1.0.6rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.6rc2.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.6rc3.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.6rc2.tar` & `kast_flow_api_python-1.0.6rc3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-25 13:58:20.243446 kast_flow_api_python-1.0.6rc2/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     9063 2023-07-25 13:58:20.217446 kast_flow_api_python-1.0.6rc2/kast_flow_api/v1.py
--rw-r--r--   0        0        0      537 2023-07-25 13:58:40.250443 kast_flow_api_python-1.0.6rc2/pyproject.toml
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.6rc2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-28 11:42:29.263404 kast_flow_api_python-1.0.6rc3/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0    10177 2023-07-28 11:24:46.573974 kast_flow_api_python-1.0.6rc3/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      537 2023-07-28 11:42:49.525851 kast_flow_api_python-1.0.6rc3/pyproject.toml
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.6rc3/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.6rc2/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.6rc3/kast_flow_api/v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
-from dataclasses import asdict, dataclass, field, fields
+from dataclasses import MISSING, asdict, dataclass, field, fields
 from enum import StrEnum
 from functools import wraps
-from typing import Any, Callable, Protocol, Self, Tuple, Type, TypeVar, cast
+from typing import Any, Callable, Iterable, Protocol, Self, Tuple, Type, TypeVar, cast
 
 from dacite import Config, from_dict
 
 
 class KastSchemaFileName:
     @staticmethod
     def batch(schemaRegistry_path: str, topics: str) -> str:
@@ -24,29 +24,30 @@
     PARQUET = "parquet"
 
     @staticmethod
     def unmarshal(format: str) -> "KastFormat":
         try:
             return KastFormat(format)
         except ValueError as e:
-            raise KastFunctionInvalidArgumentsException(
+            raise KastFunctionInvalidArgumentsError(
                 message=[
                     ["KastFormat", f"shoud be one of {list(map(str, KastFormat))}"],
                 ],
                 errors=e,
             )
 
 
 T = TypeVar("T")
 
 
 def kast_unmarshal(clazz: T) -> T:
-    """Type ignore is necessary due to typechecker not supporting alias of dataclass
-    see: https://github.com/python/mypy/issues/9875
-    """
+    """decorator to unmarshal class as KastNode"""
+    # Type ignore is necessary due to typechecker not supporting alias of dataclass
+    # see: https://github.com/python/mypy/issues/9875
+    #
     return dataclass(clazz, frozen=True, slots=True, kw_only=True, eq=True)  # type: ignore
 
 
 class KastDataFrame(Protocol):
     @property
     def parents_id(self: Self) -> list[str]:
         ...
@@ -56,53 +57,63 @@
         ...
 
     @property
     def schema(self: Self) -> Any:
         ...
 
     @property
+    def avro_schema(self: Self) -> str:
+        ...
+
+    @property
     def engine(self: Self) -> Any:
         ...
 
     @classmethod
     def read(
         cls: Type[Self], id: str, format: str, path: str, schema: str, **kwargs: Any
     ) -> "KastDataFrame":
         ...
 
     @classmethod
-    def fromDataFrame(
+    def from_dataframe(
         cls: Type[Self], df: Any, id: str, parents: list[str] = []
     ) -> "KastDataFrame":
         ...
 
     @classmethod
-    def createDataFrame(
+    def create_dataframe(
         cls: Type[Self], df: Any, id: str, schema: str
     ) -> "KastDataFrame":
         ...
 
     def write(self: Self, format: str, topics: str, mode: str, **kwargs: Any) -> None:
         ...
 
     @classmethod
-    def emptyDataFrame(cls: Type[Self], id: str) -> "KastDataFrame":
+    def empty_dataframe(cls: Type[Self], id: str) -> "KastDataFrame":
         ...
 
-    def createOrReplaceTempView(self: Self, name: str = "") -> "KastDataFrame":
+    def create_or_replace_tempview(self: Self, name: str = "") -> "KastDataFrame":
         ...
 
     def map(self: Self, fn: Any, schema: str | dict[str, Any]) -> "KastDataFrame":
         ...
 
     def show(
-        self: Self, id: list[str] = [], truncate: bool = False, vertical: bool = False
+        self: Self,
+        lines: int = 20,
+        truncate: bool = False,
+        vertical: bool = False,
     ) -> None:
         ...
 
+    def show_schema(self: Self, engine_schema: bool = False) -> None:
+        ...
+
     def sql(self: Self, query: str) -> "KastDataFrame":
         ...
 
     def table_sql(self: Self, query: str) -> None:
         ...
 
     def checkpoint(self: Self) -> "KastDataFrame":
@@ -125,29 +136,58 @@
     return cast(SideOut, dict[SideOutKey, SideOutValue])
 
 
 def make_outs() -> KastOuts:
     return field(default_factory=lambda: cast(KastOuts, tuple()))
 
 
+KAST_MISSING = MISSING
+
+
+def kast_field(
+    *,
+    default=KAST_MISSING,
+    default_factory=KAST_MISSING,
+    init=True,
+    repr=True,
+    hash=None,
+    compare=True,
+    metadata=None,
+    kw_only=KAST_MISSING,
+):
+    """Kast-flow version of dataclass's `field()` (just using real `field()` for now
+    but making this interface will allow to change implementation without the
+    need to change imports in udf and custom nodes )"""
+    return field(
+        default=default,
+        default_factory=default_factory,
+        init=init,
+        repr=repr,
+        hash=hash,
+        compare=compare,
+        metadata=metadata,
+        kw_only=kw_only,
+    )
+
+
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastTable:
     sql: str
     type: str = "table"
 
 
 class KastTool(Protocol):
-    def newKastDataFrame(
+    def new_kast_dataframe(
         self: Self,
         df: Any,
         schema: str = "",
     ) -> KastDataFrame:
         ...
 
-    def emptyKastDataFrame(self: Self) -> KastDataFrame:
+    def empty_kast_dataframe(self: Self) -> KastDataFrame:
         ...
 
 
 @dataclass(frozen=True, slots=True, kw_only=True, eq=True)
 class KastFunction(Protocol):
     id: str
     registerSchema: bool = False
@@ -183,17 +223,15 @@
     sideOut: SideOut = field(default_factory=make_side_out)
     out: KastOuts = make_outs()
     settings: dict[str, Any] = field(default_factory=dict)
     internal: Internal = field(default_factory=make_internal)
 
     def clazz_settings_name(self: Self) -> str:
         names: list[str] = self.type.split("-")
-        if len(names) == 2:
-            return f"{names[0].capitalize()}{names[1].capitalize()}"
-        return f"{names[0].capitalize()}"
+        return "".join([word.capitalize() for word in names])
 
 
 class KastNode(PredefinedAttributesMixin):
     def __init__(self: Self, **kwargs: Any) -> None:
         return super().__init__(**kwargs)
 
     @property
@@ -212,23 +250,23 @@
                     data_class=clazz,
                     data=asdict(compute),
                     config=Config(check_types=True),
                 )
             except AttributeError:
                 continue
             except Exception as e:
-                raise KastFunctionInvalidArgumentsException(
+                raise KastFunctionInvalidArgumentsError(
                     message=[
                         ["Origin", str(e)],
                         ["Function", mod],
                         ["ID", self.id],
                     ],
                     errors=e,
                 )
-        raise KastNodeNotFoundException(
+        raise KastNodeNotFoundError(
             message=[
                 ["Origin", f"{target} is an unknown function implementation"],
                 ["ID", self.id],
             ],
             errors=None,
         )
 
@@ -274,52 +312,62 @@
 class KastManifest:
     __nodes: KastNodeList
 
     def __init__(self: Self, nodes: KastNodeList) -> None:
         self.__nodes = nodes
 
     def deser(self: Self, *add_modules: str) -> KastNodeList:
-        nodesRaw: list[KastNode] = []
+        nodes_raw: list[KastNode] = []
         for node in self.__nodes:
             node_dict: dict[str, Any] = cast(dict[str, Any], node)
-            nodesRaw.append(
+            nodes_raw.append(
                 KastNode.from_dict(
                     modules={__name__, *add_modules},
                     **node_dict,
                 )
             )
-        return cast(KastNodeList, nodesRaw)
+        return cast(KastNodeList, nodes_raw)
 
 
-class KastBaseException(Exception):
-    """base exception for errors requiring better feedback"""
+class KastBaseError(Exception):
+    """base error for errors requiring better feedback"""
 
-    def __init__(self: Self, message: list[list[str]] = [], errors: Any = None) -> None:
+    def __init__(
+        self: Self,
+        errors: Any = None,
+        message: list[list[str]] = [],
+        message_maxcolwidths: Iterable[int | None] = None,
+        before: str = "",
+        after: str = "",
+    ) -> None:
         super().__init__(message)
-        self._message = message
         self.errors = errors
+        self._message = message
+        self._before = before
+        self._after = after
+        self._message_maxcolwidths = message_maxcolwidths
 
     def __str__(self: Self) -> str:
         from tabulate import tabulate
 
-        return f"\n\n{tabulate(tabular_data=self._message, tablefmt='grid')}"
+        return f"\n\n{self._before}\n{tabulate(tabular_data=self._message, tablefmt='grid', maxcolwidths=self._message_maxcolwidths)}\n{self._after}\n"
 
 
-class KastNodeNotFoundException(KastBaseException):
-    "When node is missing from the dag, this exception is raised"
+class KastNodeNotFoundError(KastBaseError):
+    "When node is missing from the dag, this error is raised"
 
 
-class KastUnsupportedDAGOperation(KastBaseException):
-    "when unsupported operation happens on the graph dag pub/sub, this exception is raised"
+class KastUnsupportedDAGOperationError(KastBaseError):
+    "when unsupported operation happens on the graph dag pub/sub, this error is raised"
 
 
-class KastFunctionInvalidArgumentsException(KastBaseException):
-    """when required, unknown or invalid arguments are passed as input to a function,
-    this exception is raised"""
+class KastFunctionInvalidArgumentsError(KastBaseError):
+    """when required, unknown or invalid arguments are passed as arguments to a function,
+    this error is raised"""
 
 
-class KastConfigDeserializationException(KastBaseException):
-    "When invalid configuration file is passed, this exception is raised"
+class KastConfigDeserializationError(KastBaseError):
+    "When invalid configuration file is passed, this error is raised"
 
 
-class KastInvalidDataFrameBackend(KastBaseException):
-    "When invalid backend is requested, this exception is raised"
+class KastInvalidDataFrameBackendError(KastBaseError):
+    "When invalid backend is requested, this error is raised"
```

### Comparing `kast_flow_api_python-1.0.6rc2/pyproject.toml` & `kast_flow_api_python-1.0.6rc3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.6-preview2"
+version = "1.0.6-preview3"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

