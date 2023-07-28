# Comparing `tmp/openrpc-7.0.1.tar.gz` & `tmp/openrpc-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrpc-7.0.1.tar", max compression
+gzip compressed data, was "openrpc-7.0.2.tar", max compression
```

## Comparing `openrpc-7.0.1.tar` & `openrpc-7.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-07-28 16:42:50.380538 openrpc-7.0.1/LICENSE
--rw-r--r--   0        0        0     3257 2023-07-28 16:42:50.380538 openrpc-7.0.1/README.md
--rw-r--r--   0        0        0     1045 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/__init__.py
--rw-r--r--   0        0        0      183 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/_depends.py
--rw-r--r--   0        0        0        0 2023-07-28 16:42:50.406537 openrpc-7.0.1/openrpc/_discover/__init__.py
--rw-r--r--   0        0        0     4266 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/_discover/_methods.py
--rw-r--r--   0        0        0     6112 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/_discover/_schemas.py
--rw-r--r--   0        0        0     1289 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/_discover/discover.py
--rw-r--r--   0        0        0     7862 2023-07-28 16:42:50.380538 openrpc-7.0.1/openrpc/_method_processor.py
--rw-r--r--   0        0        0     6105 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_method_registrar.py
--rw-r--r--   0        0        0     9417 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_objects.py
--rw-r--r--   0        0        0     7616 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_request_processor.py
--rw-r--r--   0        0        0      280 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_router.py
--rw-r--r--   0        0        0     1168 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_rpcmethod.py
--rw-r--r--   0        0        0     9267 2023-07-28 16:42:50.381538 openrpc-7.0.1/openrpc/_server.py
--rw-r--r--   0        0        0        0 2023-07-28 16:42:50.406537 openrpc-7.0.1/openrpc/py.typed
--rw-r--r--   0        0        0     1479 2023-07-28 16:42:50.381538 openrpc-7.0.1/pyproject.toml
--rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 openrpc-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-28 19:04:29.147665 openrpc-7.0.2/LICENSE
+-rw-r--r--   0        0        0     3255 2023-07-28 19:04:29.147665 openrpc-7.0.2/README.md
+-rw-r--r--   0        0        0     1045 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_depends.py
+-rw-r--r--   0        0        0        0 2023-07-28 19:04:29.171665 openrpc-7.0.2/openrpc/_discover/__init__.py
+-rw-r--r--   0        0        0     4266 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_discover/_methods.py
+-rw-r--r--   0        0        0     6112 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_discover/_schemas.py
+-rw-r--r--   0        0        0     1289 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_discover/discover.py
+-rw-r--r--   0        0        0     7862 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_method_processor.py
+-rw-r--r--   0        0        0     6235 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_method_registrar.py
+-rw-r--r--   0        0        0     9417 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_objects.py
+-rw-r--r--   0        0        0     7616 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_request_processor.py
+-rw-r--r--   0        0        0      280 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_router.py
+-rw-r--r--   0        0        0     1168 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_rpcmethod.py
+-rw-r--r--   0        0        0     9267 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_server.py
+-rw-r--r--   0        0        0        0 2023-07-28 19:04:29.172665 openrpc-7.0.2/openrpc/py.typed
+-rw-r--r--   0        0        0     1477 2023-07-28 19:04:29.148665 openrpc-7.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 openrpc-7.0.2/PKG-INFO
```

### Comparing `openrpc-7.0.1/LICENSE` & `openrpc-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/README.md` & `openrpc-7.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align=center>
   <h1>OpenRPC</h1>
-  <h3>OpenRPC provides classes to rapidly develop an
-  <a href="https://open-rpc.org">OpenRPC</a> server.</h3>
+  <h3>Transport agnostic framework for developing
+  <a href="https://open-rpc.org">OpenRPC</a> servers.</h3>
   <img src="https://img.shields.io/badge/License-MIT-blue.svg"
    height="20"
    alt="License: MIT">
   <img src="https://img.shields.io/badge/code%20style-black-000000.svg"
    height="20"
    alt="Code style: black">
   <img src="https://img.shields.io/pypi/v/openrpc.svg"
```

### Comparing `openrpc-7.0.1/openrpc/__init__.py` & `openrpc-7.0.2/openrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_discover/_methods.py` & `openrpc-7.0.2/openrpc/_discover/_methods.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_discover/_schemas.py` & `openrpc-7.0.2/openrpc/_discover/_schemas.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_discover/discover.py` & `openrpc-7.0.2/openrpc/_discover/discover.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_method_processor.py` & `openrpc-7.0.2/openrpc/_method_processor.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_method_registrar.py` & `openrpc-7.0.2/openrpc/_method_registrar.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class MethodRegistrar:
     """Interface for registering RPC methods."""
 
     def __init__(self) -> None:
         """Initialize a new instance of the MethodRegistrar class."""
         self._rpc_methods: dict[str, RPCMethod] = {}
         self._request_processor = RequestProcessor(debug=False)
+        self._warn = True
 
     @property
     def debug(self) -> bool:
         """Debug logging status."""
         return self._request_processor.debug
 
     @debug.setter
@@ -102,14 +103,15 @@
         """
         tag_objects = (
             [tag if isinstance(tag, TagObject) else TagObject(name=tag) for tag in tags]
             if tags is not None
             else None
         )
         if not args:
+            self._warn = False
             return partial(  # type: ignore
                 self.method,
                 name=name,
                 params=params,
                 result=result,
                 tags=tag_objects,
                 summary=summary,
@@ -118,20 +120,22 @@
                 deprecated=deprecated,
                 servers=servers,
                 errors=errors,
                 links=links,
                 param_structure=param_structure,
                 examples=examples,
             )
-        warnings.warn(
-            "RPCServer `method` decorator must be called in future releases, use"
-            " `method()` instead.",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
+        if self._warn:
+            warnings.warn(
+                "RPCServer `method` decorator must be called in future releases, use"
+                " `method()` instead.",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+        self._warn = True
         func = args[0]
         name = name or func.__name__
         return self._method(
             func,
             MethodMetaData(
                 name=name,
                 params=params,
```

### Comparing `openrpc-7.0.1/openrpc/_objects.py` & `openrpc-7.0.2/openrpc/_objects.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_request_processor.py` & `openrpc-7.0.2/openrpc/_request_processor.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_rpcmethod.py` & `openrpc-7.0.2/openrpc/_rpcmethod.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/openrpc/_server.py` & `openrpc-7.0.2/openrpc/_server.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.1/pyproject.toml` & `openrpc-7.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openrpc"
-version = "7.0.1"
-description = "OpenRPC provides classes to rapidly develop an OpenRPC server."
+version = "7.0.2"
+description = "Transport agnostic framework for developing OpenRPC servers."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/openrpc"
 homepage = "https://gitlab.com/mburkard/openrpc"
 license = "MIT"
 authors = ["Matthew Burkard <matthewjburkard@gmail.com>"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `openrpc-7.0.1/PKG-INFO` & `openrpc-7.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openrpc
-Version: 7.0.1
-Summary: OpenRPC provides classes to rapidly develop an OpenRPC server.
+Version: 7.0.2
+Summary: Transport agnostic framework for developing OpenRPC servers.
 Home-page: https://gitlab.com/mburkard/openrpc
 License: MIT
 Author: Matthew Burkard
 Author-email: matthewjburkard@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,16 @@
 Requires-Dist: jsonrpc2-objects (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://gitlab.com/mburkard/openrpc
 Description-Content-Type: text/markdown
 
 <div align=center>
   <h1>OpenRPC</h1>
-  <h3>OpenRPC provides classes to rapidly develop an
-  <a href="https://open-rpc.org">OpenRPC</a> server.</h3>
+  <h3>Transport agnostic framework for developing
+  <a href="https://open-rpc.org">OpenRPC</a> servers.</h3>
   <img src="https://img.shields.io/badge/License-MIT-blue.svg"
    height="20"
    alt="License: MIT">
   <img src="https://img.shields.io/badge/code%20style-black-000000.svg"
    height="20"
    alt="Code style: black">
   <img src="https://img.shields.io/pypi/v/openrpc.svg"
```

