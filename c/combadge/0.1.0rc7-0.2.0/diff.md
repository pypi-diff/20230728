# Comparing `tmp/combadge-0.1.0rc7.tar.gz` & `tmp/combadge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-0.1.0rc7.tar", max compression
+gzip compressed data, was "combadge-0.2.0.tar", max compression
```

## Comparing `combadge-0.1.0rc7.tar` & `combadge-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11350 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/LICENSE
--rw-r--r--   0        0        0     2682 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/README.md
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/backend.py
--rw-r--r--   0        0        0     3358 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/binder.py
--rw-r--r--   0        0        0     2982 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/interfaces.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/method.py
--rw-r--r--   0        0        0      890 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     1997 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/request.py
--rw-r--r--   0        0        0     6312 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/response.py
--rw-r--r--   0        0        0     1830 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/service.py
--rw-r--r--   0        0        0     2354 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/signature.py
--rw-r--r--   0        0        0      343 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/typevars.py
--rw-r--r--   0        0        0      203 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/core/warnings.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/py.typed
--rw-r--r--   0        0        0       50 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/__init__.py
--rw-r--r--   0        0        0     1470 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/abc.py
--rw-r--r--   0        0        0      807 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/aliases.py
--rw-r--r--   0        0        0      264 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/headers.py
--rw-r--r--   0        0        0     7338 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/markers.py
--rw-r--r--   0        0        0      398 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/http/request.py
--rw-r--r--   0        0        0      124 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     3349 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0     1536 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     3207 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      348 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/async_.py
--rw-r--r--   0        0        0      308 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/contextlib.py
--rw-r--r--   0        0        0      338 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/shared/sync.py
--rw-r--r--   0        0        0       39 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      256 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     2198 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      212 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/request.py
--rw-r--r--   0        0        0      870 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/soap/response.py
--rw-r--r--   0        0        0      131 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     3450 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     3059 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     3296 2023-05-24 13:25:11.808665 combadge-0.1.0rc7/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3394 2023-05-24 13:25:27.060479 combadge-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 combadge-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-07-28 12:33:31.003912 combadge-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2682 2023-07-28 12:33:31.003912 combadge-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/backend.py
+-rw-r--r--   0        0        0     3358 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/binder.py
+-rw-r--r--   0        0        0     2982 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0     2562 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      890 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     1997 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/request.py
+-rw-r--r--   0        0        0     6312 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/response.py
+-rw-r--r--   0        0        0     1830 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/service.py
+-rw-r--r--   0        0        0     2354 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/signature.py
+-rw-r--r--   0        0        0      343 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/typevars.py
+-rw-r--r--   0        0        0      203 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/core/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/py.typed
+-rw-r--r--   0        0        0       50 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0     1470 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/abc.py
+-rw-r--r--   0        0        0      807 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/aliases.py
+-rw-r--r--   0        0        0      264 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/headers.py
+-rw-r--r--   0        0        0     7338 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/markers.py
+-rw-r--r--   0        0        0      398 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/http/request.py
+-rw-r--r--   0        0        0      124 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     3349 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0     1536 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     3207 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/async_.py
+-rw-r--r--   0        0        0      308 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/contextlib.py
+-rw-r--r--   0        0        0      338 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/shared/sync.py
+-rw-r--r--   0        0        0       39 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     2198 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      212 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/request.py
+-rw-r--r--   0        0        0      870 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      131 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     5884 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     3400 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     5070 2023-07-28 12:33:31.003912 combadge-0.2.0/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3404 2023-07-28 12:33:45.331809 combadge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 combadge-0.2.0/PKG-INFO
```

### Comparing `combadge-0.1.0rc7/LICENSE` & `combadge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/README.md` & `combadge-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/backend.py` & `combadge-0.2.0/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/binder.py` & `combadge-0.2.0/combadge/core/binder.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/interfaces.py` & `combadge-0.2.0/combadge/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/markers/method.py` & `combadge-0.2.0/combadge/core/markers/method.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/markers/parameter.py` & `combadge-0.2.0/combadge/core/markers/parameter.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/request.py` & `combadge-0.2.0/combadge/core/request.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/response.py` & `combadge-0.2.0/combadge/core/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/service.py` & `combadge-0.2.0/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/core/signature.py` & `combadge-0.2.0/combadge/core/signature.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/http/abc.py` & `combadge-0.2.0/combadge/support/http/abc.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/http/aliases.py` & `combadge-0.2.0/combadge/support/http/aliases.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/http/markers.py` & `combadge-0.2.0/combadge/support/http/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/httpx/backends/async_.py` & `combadge-0.2.0/combadge/support/httpx/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/httpx/backends/base.py` & `combadge-0.2.0/combadge/support/httpx/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/httpx/backends/sync.py` & `combadge-0.2.0/combadge/support/httpx/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/soap/markers.py` & `combadge-0.2.0/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/soap/response.py` & `combadge-0.2.0/combadge/support/soap/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc7/combadge/support/zeep/backends/async_.py` & `combadge-0.2.0/combadge/support/zeep/backends/sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,133 @@
 from __future__ import annotations
 
-from contextlib import AbstractAsyncContextManager
+from contextlib import AbstractContextManager, nullcontext
+from os import PathLike, fspath
 from types import TracebackType
-from typing import Any, Callable
+from typing import Any, Callable, Collection
 
 from pydantic import BaseModel
 from typing_extensions import Self
+from zeep import Client, Plugin, Transport
 from zeep.exceptions import Fault
-from zeep.proxy import AsyncOperationProxy, AsyncServiceProxy
+from zeep.proxy import OperationProxy, ServiceProxy
+from zeep.wsse import UsernameToken
 
 from combadge.core.backend import ServiceContainer
 from combadge.core.binder import BaseBoundService
 from combadge.core.interfaces import CallServiceMethod
 from combadge.core.request import build_request
 from combadge.core.signature import Signature
 from combadge.core.typevars import ResponseT
-from combadge.support.shared.async_ import SupportsRequestWith
-from combadge.support.shared.contextlib import asyncnullcontext
+from combadge.support.shared.sync import SupportsRequestWith
 from combadge.support.soap.request import Request
 from combadge.support.soap.response import SoapFaultT
-from combadge.support.zeep.backends.base import BaseZeepBackend
+from combadge.support.zeep.backends.base import BaseZeepBackend, ByBindingName, ByServiceName
 
 
-class ZeepBackend(
-    BaseZeepBackend[AsyncServiceProxy, AsyncOperationProxy],
-    SupportsRequestWith[Request],
-    ServiceContainer,
-):
-    """Asynchronous Zeep service."""
+class ZeepBackend(BaseZeepBackend[ServiceProxy, OperationProxy], SupportsRequestWith[Request], ServiceContainer):
+    """Synchronous Zeep service."""
 
     __slots__ = ("_service", "_request_with", "_service_cache")
 
+    @classmethod
+    def with_params(
+        cls,
+        wsdl_path: PathLike,
+        *,
+        service: ByBindingName | ByServiceName | None = None,
+        plugins: Collection[Plugin] | None = None,
+        load_timeout: float | None = None,
+        operation_timeout: float | None = None,
+        wsse: UsernameToken | None = None,
+        verify_ssl: bool | PathLike = True,
+        cert_file: PathLike | None = None,
+        key_file: PathLike | None = None,
+    ) -> ZeepBackend:
+        """
+        Instantiate the backend using a set of the most common parameters.
+
+        Using the `__init__()` may become quite wordy, so this method simplifies typical use cases.
+        """
+        client = Client(
+            fspath(wsdl_path),
+            wsse=wsse,
+            transport=Transport(timeout=load_timeout, operation_timeout=operation_timeout),
+            plugins=plugins,
+        )
+        client.transport.session.verify = verify_ssl if isinstance(verify_ssl, bool) else fspath(verify_ssl)
+        client.transport.session.cert = (
+            fspath(cert_file) if cert_file is not None else None,
+            fspath(key_file) if key_file is not None else None,
+        )
+        if service is None:
+            service_proxy = client.service
+        elif isinstance(service, ByServiceName):
+            service_proxy = client.bind(service.service_name, service.port_name)
+        elif isinstance(service, ByBindingName):
+            service_proxy = client.create_service(service.binding_name, service.address)
+        else:
+            raise TypeError(type(service))
+        return cls(service_proxy)
+
     def __init__(
         self,
-        service: AsyncServiceProxy,
+        service: ServiceProxy,
         *,
-        request_with: Callable[[Any], AbstractAsyncContextManager] = asyncnullcontext,
+        request_with: Callable[[Any], AbstractContextManager] = nullcontext,
     ) -> None:
         """
         Instantiate the backend.
 
         Args:
             service: [service proxy object](https://docs.python-zeep.org/en/master/client.html#the-serviceproxy-object)
             request_with: an optional context manager getter to wrap each request into
         """
         BaseZeepBackend.__init__(self, service)
         SupportsRequestWith.__init__(self, request_with)
         ServiceContainer.__init__(self)
 
-    async def __call__(
+    def __call__(
         self,
         request: Request,
         response_type: type[ResponseT],
         fault_type: type[SoapFaultT],
-    ) -> BaseModel:
+    ) -> ResponseT | SoapFaultT:
         """
         Call the specified service method.
 
         Args:
             request: prepared request
             response_type: non-fault response model type
             fault_type: SOAP fault model type
         """
         operation = self._get_operation(request.operation_name)
         try:
-            response = await operation(**request.body.dict(by_alias=True))
+            response = operation(**request.body.dict(by_alias=True))
         except Fault as e:
             return self._parse_soap_fault(e, fault_type)
         return self._parse_response(response, response_type)
 
     @classmethod
     def bind_method(cls, signature: Signature) -> CallServiceMethod[ZeepBackend]:  # noqa: D102
         response_type, fault_type = cls._split_response_type(signature.return_type)
 
-        async def bound_method(self: BaseBoundService[ZeepBackend], *args: Any, **kwargs: Any) -> BaseModel:
+        def bound_method(self: BaseBoundService[ZeepBackend], *args: Any, **kwargs: Any) -> BaseModel:
             request = build_request(Request, signature, self, args, kwargs)
-            async with self.backend._request_with(request):
-                return await self.backend(request, response_type, fault_type)
+            with self.backend._request_with(request):
+                return self.backend(request, response_type, fault_type)
 
         return bound_method  # type: ignore[return-value]
 
     binder = bind_method  # type: ignore[assignment]
 
-    async def __aenter__(self) -> Self:
-        self._service = await self._service.__aenter__()
+    def __enter__(self) -> Self:
+        self._service = self._service.__enter__()
         return self
 
-    async def __aexit__(
+    def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         traceback: TracebackType | None,
     ) -> Any:
-        return await self._service.__aexit__(exc_type, exc_value, traceback)
+        return self._service.__exit__(exc_type, exc_value, traceback)
```

### Comparing `combadge-0.1.0rc7/combadge/support/zeep/backends/base.py` & `combadge-0.2.0/combadge/support/zeep/backends/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 from abc import ABC
-from typing import Any, Generic, Tuple, Type, TypeVar, Union
+from dataclasses import dataclass
+from typing import Any, Generic, TypeVar, Union
 
 from pydantic import BaseModel, parse_obj_as
 from typing_extensions import get_args as get_type_args
 from typing_extensions import get_origin as get_type_origin
 from zeep.exceptions import Fault
 from zeep.helpers import serialize_object
 from zeep.proxy import OperationProxy, ServiceProxy
@@ -29,15 +32,15 @@
     """Base class for the sync and async backends. Not intended for a direct use."""
 
     def __init__(self, service: _ServiceProxyT) -> None:
         """Instantiate the backend."""
         self._service = service
 
     @staticmethod
-    def _split_response_type(response_type: Type[Any]) -> Tuple[Type[BaseModel], Type[BaseSoapFault]]:
+    def _split_response_type(response_type: type[Any]) -> tuple[type[BaseModel], type[BaseSoapFault]]:
         """
         Split the response type into non-faults and faults.
 
         SOAP faults are handled separately, so we need to extract them from the annotated
         response type.
         """
 
@@ -66,15 +69,31 @@
         """Get an operation by its name."""
         try:
             return self._service[name]
         except AttributeError as e:
             raise RuntimeError(f"available operations are: {dir(self._service)}") from e
 
     @staticmethod
-    def _parse_response(value: CompoundValue, response_type: Type[ResponseT]) -> ResponseT:
+    def _parse_response(value: CompoundValue, response_type: type[ResponseT]) -> ResponseT:
         """Parse the response value using the generic response types."""
         return parse_obj_as(response_type, serialize_object(value, dict))
 
     @staticmethod
-    def _parse_soap_fault(exception: Fault, fault_type: Type[SoapFaultT]) -> SoapFaultT:
+    def _parse_soap_fault(exception: Fault, fault_type: type[SoapFaultT]) -> SoapFaultT:
         """Parse the SOAP fault."""
         return parse_obj_as(fault_type, exception.__dict__)
+
+
+@dataclass
+class ByBindingName:
+    """Create service by binding name and address."""
+
+    binding_name: str
+    address: str
+
+
+@dataclass
+class ByServiceName:
+    """Create service by service and port names."""
+
+    service_name: str | None = None
+    port_name: str | None = None
```

### Comparing `combadge-0.1.0rc7/pyproject.toml` & `combadge-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "0.1.0rc7"
+version = "0.2.0"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -117,15 +117,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 typing-extensions = "^4.4.0"
 pydantic = "^1.10.4"
 get-annotations = { version = "^0.1.2", python = "<3.10" }
 zeep = {version = "^4.2.1", optional = true}
-httpx = {version = "^0.23.3", optional = true}
+httpx = {version = ">=0.23.3, <1.0.0", optional = true}
 
 [tool.poetry.extras]
 httpx = ["httpx"]
 zeep = ["zeep"]
 
 [tool.poetry.group.dev]
 optional = true
@@ -154,9 +154,9 @@
 black = "^22.12.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 pattern = "default-unprefixed"
 style = "pep440"
-strict = false # TODO
+strict = true
 latest-tag = true
```

### Comparing `combadge-0.1.0rc7/PKG-INFO` & `combadge-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,15 +24,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Provides-Extra: httpx
 Provides-Extra: zeep
 Requires-Dist: get-annotations (>=0.1.2,<0.2.0) ; python_version < "3.10"
-Requires-Dist: httpx (>=0.23.3,<0.24.0) ; extra == "httpx"
+Requires-Dist: httpx (>=0.23.3,<1.0.0) ; extra == "httpx"
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: zeep (>=4.2.1,<5.0.0) ; extra == "zeep"
 Project-URL: Repository, https://github.com/kpn/combadge
 Description-Content-Type: text/markdown
 
 # Combadge
```

