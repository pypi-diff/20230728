# Comparing `tmp/combadge-0.2.0.tar.gz` & `tmp/combadge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-0.2.0.tar", max compression
+gzip compressed data, was "combadge-0.2.1.tar", max compression
```

## Comparing `combadge-0.2.0.tar` & `combadge-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11350 2023-07-28 12:33:31.003912 combadge-0.2.0/LICENSE
--rw-r--r--   0        0        0     2682 2023-07-28 12:33:31.003912 combadge-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/backend.py
--rw-r--r--   0        0        0     3358 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/binder.py
--rw-r--r--   0        0        0     2982 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/interfaces.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0     2562 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/method.py
--rw-r--r--   0        0        0      890 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     1997 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/request.py
--rw-r--r--   0        0        0     6312 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/response.py
--rw-r--r--   0        0        0     1830 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/service.py
--rw-r--r--   0        0        0     2354 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/signature.py
--rw-r--r--   0        0        0      343 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/typevars.py
--rw-r--r--   0        0        0      203 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/warnings.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/py.typed
--rw-r--r--   0        0        0       50 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/__init__.py
--rw-r--r--   0        0        0     1470 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/abc.py
--rw-r--r--   0        0        0      807 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/aliases.py
--rw-r--r--   0        0        0      264 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/headers.py
--rw-r--r--   0        0        0     7338 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/markers.py
--rw-r--r--   0        0        0      398 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/request.py
--rw-r--r--   0        0        0      124 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     3349 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0     1536 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     3207 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      348 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/async_.py
--rw-r--r--   0        0        0      308 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/contextlib.py
--rw-r--r--   0        0        0      338 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/sync.py
--rw-r--r--   0        0        0       39 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      256 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     2198 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      212 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/request.py
--rw-r--r--   0        0        0      870 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/response.py
--rw-r--r--   0        0        0      131 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     5884 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     3400 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     5070 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3404 2023-07-28 12:33:45.331809 combadge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 combadge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-07-28 13:22:48.448433 combadge-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2682 2023-07-28 13:22:48.448433 combadge-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/backend.py
+-rw-r--r--   0        0        0     3358 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/binder.py
+-rw-r--r--   0        0        0     2982 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0     2562 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      890 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     1997 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/request.py
+-rw-r--r--   0        0        0     6215 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/response.py
+-rw-r--r--   0        0        0     1830 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/service.py
+-rw-r--r--   0        0        0     2354 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/signature.py
+-rw-r--r--   0        0        0      343 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/typevars.py
+-rw-r--r--   0        0        0      203 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/core/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/py.typed
+-rw-r--r--   0        0        0       50 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0     1470 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/abc.py
+-rw-r--r--   0        0        0      807 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/aliases.py
+-rw-r--r--   0        0        0      264 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/headers.py
+-rw-r--r--   0        0        0     7338 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/markers.py
+-rw-r--r--   0        0        0      398 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/http/request.py
+-rw-r--r--   0        0        0      124 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     3349 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0     1536 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     3207 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/shared/async_.py
+-rw-r--r--   0        0        0      308 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/shared/contextlib.py
+-rw-r--r--   0        0        0      338 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/shared/sync.py
+-rw-r--r--   0        0        0       39 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     2198 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      212 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/soap/request.py
+-rw-r--r--   0        0        0      870 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      131 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     5884 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     3400 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     5070 2023-07-28 13:22:48.448433 combadge-0.2.1/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3443 2023-07-28 13:23:02.632375 combadge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 combadge-0.2.1/PKG-INFO
```

### Comparing `combadge-0.2.0/LICENSE` & `combadge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/README.md` & `combadge-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/backend.py` & `combadge-0.2.1/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/binder.py` & `combadge-0.2.1/combadge/core/binder.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/interfaces.py` & `combadge-0.2.1/combadge/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/markers/method.py` & `combadge-0.2.1/combadge/core/markers/method.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/markers/parameter.py` & `combadge-0.2.1/combadge/core/markers/parameter.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/request.py` & `combadge-0.2.1/combadge/core/request.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/response.py` & `combadge-0.2.1/combadge/core/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Generic response models."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Generic, Iterable, NoReturn
+from typing import Any, ClassVar, Generic, Iterable, NoReturn, Type
 
 from pydantic import BaseModel
-from typing_extensions import Self, TypeAlias
+from typing_extensions import Self
 
 from combadge.core.typevars import ResponseT
 
 
 class BaseResponse(ABC, BaseModel):
     """
     Base model representing any possible service response.
@@ -90,56 +90,60 @@
         """
 
     def unwrap(self) -> Self:
         """Return itself since there's no error."""
         return self
 
 
+class BaseError(Generic[ResponseT], Exception):
+    """Base exception class for all errors derived from `ErrorResponse`."""
+
+    def __init__(self, response: ResponseT) -> None:
+        """
+        Instantiate the error.
+
+        Args:
+            response: original response that caused the exception
+        """
+        super().__init__(response)
+
+    @property
+    def response(self) -> ResponseT:
+        """Get the response that caused the exception."""
+        return self.args[0]
+
+
 class ErrorResponse(BaseResponse, ABC):
     """
     Parent model for error responses.
 
     Users should not use it directly, but inherit their response models from it.
     """
 
-    class Error(Generic[ResponseT], Exception):
-        """
-        Dynamically derived exception class.
-
-        For each model inherited from `ErrorResponse` Combadge generates an exception
-        class, which is accessible through the `<ModelClass>.Error` attribute.
-
-        Examples:
-            >>> class InvalidInput(ErrorResponse):
-            >>>     code: Literal["INVALID_INPUT"]
-            >>>
-            >>> try:
-            >>>     service.call(...)
-            >>> except InvalidInput.Error:
-            >>>     ...
-
-        Note: Why dynamically constructed class?
-            The problem with `pydantic` is that you can't inherit from `BaseModel` and `Exception`
-            at the same time. Thus, Combadge dynamically constructs a derived exception class,
-            which is available via the class attribute and raised by `raise_for_result()` and `unwrap()`.
-        """
-
-        def __init__(self, response: ResponseT) -> None:
-            """
-            Instantiate the error.
+    Error: ClassVar[Type[BaseError]] = BaseError
+    """
+    Dynamically derived exception class.
 
-            Args:
-                response: original response that caused the exception
-            """
-            super().__init__(response)
+    For each model inherited from `ErrorResponse` Combadge generates an exception
+    class, which is accessible through the `<ModelClass>.Error` attribute.
 
-        @property
-        def response(self) -> ResponseT:
-            """Get the response that caused the exception."""
-            return self.args[0]
+    Examples:
+        >>> class InvalidInput(ErrorResponse):
+        >>>     code: Literal["INVALID_INPUT"]
+        >>>
+        >>> try:
+        >>>     service.call(...)
+        >>> except InvalidInput.Error:
+        >>>     ...
+
+    Note: Why dynamically constructed class?
+        The problem with `pydantic` is that you can't inherit from `BaseModel` and `Exception`
+        at the same time. Thus, Combadge dynamically constructs a derived exception class,
+        which is available via the class attribute and raised by `raise_for_result()` and `unwrap()`.
+    """
 
     def __init_subclass__(cls, exception_bases: Iterable[type[BaseException]] = (), **kwargs: Any) -> None:
         """
         Build the derived exception class.
 
         Args:
             exception_bases: additional bases for the derived exception class
@@ -179,11 +183,7 @@
         if not exception:
             raise self.Error(self)
         raise exception from self.Error(self)
 
     def unwrap(self) -> NoReturn:
         """Raise the derived exception."""
         raise self.Error(self)
-
-
-BaseError: TypeAlias = ErrorResponse.Error
-"""Base exception class for all errors derived from `ErrorResponse`."""
```

### Comparing `combadge-0.2.0/combadge/core/service.py` & `combadge-0.2.1/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/core/signature.py` & `combadge-0.2.1/combadge/core/signature.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/http/abc.py` & `combadge-0.2.1/combadge/support/http/abc.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/http/aliases.py` & `combadge-0.2.1/combadge/support/http/aliases.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/http/markers.py` & `combadge-0.2.1/combadge/support/http/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/httpx/backends/async_.py` & `combadge-0.2.1/combadge/support/httpx/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/httpx/backends/base.py` & `combadge-0.2.1/combadge/support/httpx/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/httpx/backends/sync.py` & `combadge-0.2.1/combadge/support/httpx/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/soap/markers.py` & `combadge-0.2.1/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/soap/response.py` & `combadge-0.2.1/combadge/support/soap/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/zeep/backends/async_.py` & `combadge-0.2.1/combadge/support/zeep/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/zeep/backends/base.py` & `combadge-0.2.1/combadge/support/zeep/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/combadge/support/zeep/backends/sync.py` & `combadge-0.2.1/combadge/support/zeep/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.2.0/pyproject.toml` & `combadge-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "0.2.0"
+version = "0.2.1"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -76,19 +76,21 @@
     "D104",
     "D105",
     "D202",
     "D203",
     "D212",  # alternative of D213
     "D406",
     "D407",
+    "D413",
     "PT001",
     "PT011",
     "PT013",
     "RET505",
     "TRY003",
+    "UP006", # Python 3.9+
 ]
 unfixable = ["B"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["D101", "D102", "D106"]
 
 [tool.ruff.flake8-quotes]
@@ -128,19 +130,19 @@
 zeep = ["zeep"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
-mypy = "^1.0.0"
+mypy = "^1.4.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 types-requests = "^2.28.11.8"
-ruff = "^0.0.263"
+ruff = "^0.0.280"
 pytest-recording = "^0.12.1"
 pytest-asyncio = "^0.20.3"
 urllib3 = "^1.26.16"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `combadge-0.2.0/PKG-INFO` & `combadge-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
```

