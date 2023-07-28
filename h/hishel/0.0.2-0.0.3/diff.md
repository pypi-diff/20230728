# Comparing `tmp/hishel-0.0.2.tar.gz` & `tmp/hishel-0.0.3.tar.gz`

## Comparing `hishel-0.0.2.tar` & `hishel-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 hishel-0.0.2/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/__about__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/__init__.py
--rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_headers.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_synchronization.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/py.typed
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_client.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_pool.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_transports.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_client.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.2/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.2/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 hishel-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hishel-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 hishel-0.0.3/README.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/__about__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/__init__.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 hishel-0.0.3/PKG-INFO
```

### Comparing `hishel-0.0.2/README.md` & `hishel-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -39,66 +39,68 @@
 import hishel
 
 with hishel.CacheClient() as client:
     client.get("https://www.github.com")
     client.get("https://www.github.com")  # takes from the cache (very fast!)
 ```
 
-If the response is cacheable according to **RFC 9111**, hishel will save it for later use, so the user only needs to change the **client and the rest of the staff will be done automatically.**
+or in asynchronous context
 
-Hishel also works well with httpcore, and you can **make your httpcore connection pools cacheable with a single line of code.**
-
-Your existing code
-``` python
-from httpcore import ConnectionPool
-
-pool = ConnectionPool()
+```python
+import hishel
 
-...
+async with hishel.AsyncCacheClient() as client:
+    await client.get("https://www.github.com")
+    await client.get("https://www.github.com")  # takes from the cache
 ```
 
-Adding HTTP caching to your program will make it much faster and more efficient.
-``` python
-import hishel
-from httpcore import ConnectionPool
+## HTTPX and HTTP Core
 
-pool = ConnectionPool()
-pool = hishel.CacheConnectionPool(pool=pool)
-...
-```
+`Hishel` also supports the transports of `HTTPX` and the connection pools of `HTTP Core`.
 
-As you can see, it is **extremely simple to integrate**. 
+`Hishel` respects existing **transports** and **connection pools** and can therefore work **on top of them**, making hishel a very **compatible and flexible library**.
 
-Because `Hishel` respects your custom transports and connection pools, it requires the real **ConnectionPool** and the real **HTTPTransport** to work on top of it.
 
 **Transports** example:
 
 ``` python
 import httpx
 import hishel
 
 transport = httpx.HTTPTransport()
 cache_transport = hishel.CacheTransport(transport=transport)
 
-req = httpx.Request("GET",
-                    "https://google.com")
+req = httpx.Request("GET", "https://www.github.com")
 
 cache_transport.handle_request(req)
-cache_transport.handle_request(req)
+cache_transport.handle_request(req)  # takes from the cache
 ```
 
-## How and where are the responses saved?
+**Connection Pool** example:
 
-Hishel supports a variety of backends for storing responses, but the **filesystem is the default**.
 
-You can also use another backend, such as **redis**, to store your responses, or even **write your own** if necessary.
+```python
+import httpcore
+import hishel
+
+pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
+
+pool.request("GET", "https://www.github.com")
+pool.request("GET", "https://www.github.com")  # takes from the cache
+
+```
+
+## How and where are the responses saved?
+
+The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a variety of built-in storage options, but the default storage is a [filesystem storage](TODO). You can switch the storage to another one that `Hishel` offers or, if necessary, write your own; for more information, see the storage documentation.
 
 
 ## Contributing
 
-Hishel is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
+`Hishel` is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
+
+You can open the pull request by following these instructions if you want to improve `Hishel`. 💓
 
-The most common strategy for contributing `Hishel` appears to be:
+- Fork the project.
+- Make change.
+- Open the pull request.
 
-- Fork the project
-- Make change
-- Open the pull request
```

#### html2text {}

```diff
@@ -22,30 +22,30 @@
 parts of RFC 9111 **should be ignored and which should not**, for example, you
 can explicitly disable stale responses for your safety or enable re-validation
 for each response before using it. - ð Very fast: When **IO is not
 required**, your requests are even faster. ## QuickStart Install `Hishel` using
 pip: ``` shell $ pip install hishel ``` Let's begin with an example of a httpx
 client. ```python import hishel with hishel.CacheClient() as client: client.get
 ("https://www.github.com") client.get("https://www.github.com") # takes from
-the cache (very fast!) ``` If the response is cacheable according to **RFC
-9111**, hishel will save it for later use, so the user only needs to change the
-**client and the rest of the staff will be done automatically.** Hishel also
-works well with httpcore, and you can **make your httpcore connection pools
-cacheable with a single line of code.** Your existing code ``` python from
-httpcore import ConnectionPool pool = ConnectionPool() ... ``` Adding HTTP
-caching to your program will make it much faster and more efficient. ``` python
-import hishel from httpcore import ConnectionPool pool = ConnectionPool() pool
-= hishel.CacheConnectionPool(pool=pool) ... ``` As you can see, it is
-**extremely simple to integrate**. Because `Hishel` respects your custom
-transports and connection pools, it requires the real **ConnectionPool** and
-the real **HTTPTransport** to work on top of it. **Transports** example: ```
-python import httpx import hishel transport = httpx.HTTPTransport()
-cache_transport = hishel.CacheTransport(transport=transport) req =
-httpx.Request("GET", "https://google.com") cache_transport.handle_request(req)
-cache_transport.handle_request(req) ``` ## How and where are the responses
-saved? Hishel supports a variety of backends for storing responses, but the
-**filesystem is the default**. You can also use another backend, such as
-**redis**, to store your responses, or even **write your own** if necessary. ##
-Contributing Hishel is a powerful tool, but it is also a new project with
-potential flaws, so we welcome contributions! The most common strategy for
-contributing `Hishel` appears to be: - Fork the project - Make change - Open
-the pull request
+the cache (very fast!) ``` or in asynchronous context ```python import hishel
+async with hishel.AsyncCacheClient() as client: await client.get("https://
+www.github.com") await client.get("https://www.github.com") # takes from the
+cache ``` ## HTTPX and HTTP Core `Hishel` also supports the transports of
+`HTTPX` and the connection pools of `HTTP Core`. `Hishel` respects existing
+**transports** and **connection pools** and can therefore work **on top of
+them**, making hishel a very **compatible and flexible library**.
+**Transports** example: ``` python import httpx import hishel transport =
+httpx.HTTPTransport() cache_transport = hishel.CacheTransport
+(transport=transport) req = httpx.Request("GET", "https://www.github.com")
+cache_transport.handle_request(req) cache_transport.handle_request(req) # takes
+from the cache ``` **Connection Pool** example: ```python import httpcore
+import hishel pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
+pool.request("GET", "https://www.github.com") pool.request("GET", "https://
+www.github.com") # takes from the cache ``` ## How and where are the responses
+saved? The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a
+variety of built-in storage options, but the default storage is a [filesystem
+storage](TODO). You can switch the storage to another one that `Hishel` offers
+or, if necessary, write your own; for more information, see the storage
+documentation. ## Contributing `Hishel` is a powerful tool, but it is also a
+new project with potential flaws, so we welcome contributions! You can open the
+pull request by following these instructions if you want to improve `Hishel`.
+ð - Fork the project. - Make change. - Open the pull request.
```

### Comparing `hishel-0.0.2/hishel/_files.py` & `hishel-0.0.3/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.2/hishel/_headers.py` & `hishel-0.0.3/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.2/hishel/_serializers.py` & `hishel-0.0.3/hishel/_serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import yaml
 from httpcore import Response
 
 HEADERS_ENCODING = "iso-8859-1"
 KNOWN_RESPONSE_EXTENSIONS = ("http_version", "reason_phrase")
 
+__all__ = ("PickleSerializer", "JSONSerializer", "YamlSerializer", "BaseSerializer")
+
 
 class BaseSerializer:
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         raise NotImplementedError()
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
         raise NotImplementedError()
@@ -41,15 +43,15 @@
         return tp.cast(Response, pickle.loads(data))
 
     @property
     def is_binary(self) -> bool:  # pragma: no cover
         return True
 
 
-class DictSerializer(BaseSerializer):
+class JSONSerializer(BaseSerializer):
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         response_dict = {
             "status": response.status,
             "headers": [
                 (key.decode(HEADERS_ENCODING), value.decode(HEADERS_ENCODING))
                 for key, value in response.headers
             ],
```

### Comparing `hishel-0.0.2/hishel/_synchronization.py` & `hishel-0.0.3/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.2/hishel/_utils.py` & `hishel-0.0.3/hishel/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import time
 import typing as tp
 from email.utils import parsedate_tz
 from hashlib import blake2b
 
 import anyio
 import httpcore
-from httpcore import URL
 
-from ._headers import Vary
+HEADERS_ENCODING = "iso-8859-1"
 
 
 class BaseClock:
     def now(self) -> int:
         raise NotImplementedError()
 
 
@@ -30,63 +29,51 @@
 
     if isinstance(url, httpcore.URL):
         port = f":{url.port}" if url.port is not None else ""
         return f'{url.scheme.decode("ascii")}://{url.host.decode("ascii")}{port}{url.target.decode("ascii")}'
     assert False, "Invalid type for `normalized_url`"  # pragma: no cover
 
 
-def generate_key(
-    method: bytes, url: URL, headers: tp.List[tp.Tuple[bytes, bytes]]
-) -> str:
-    # TODO: sort vary headers
-    vary_values = [
-        val.decode("ascii") for val in extract_header_values(headers, b"vary")
-    ]
-    vary = Vary.from_value(vary_values=vary_values)
-    vary_headers_suffix = b""
-    for vary_value in vary._values:
-        vary_headers_suffix += vary_value.encode("ascii") + b"="
-        vary_headers_suffix += b", ".join(
-            extract_header_values(headers, vary_value.encode("ascii"))
-        )
-
-    encoded_url = normalized_url(url).encode("ascii")
+def generate_key(request: httpcore.Request) -> str:
+    encoded_url = normalized_url(request.url).encode("ascii")
 
     key_parts = [
-        method,
+        request.method,
         encoded_url,
-        vary_headers_suffix,
     ]
 
     key = blake2b(digest_size=16)
     for part in key_parts:
         key.update(part)
     return key.hexdigest()
 
 
 def extract_header_values(
-    headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes, single: bool = False
+    headers: tp.List[tp.Tuple[bytes, bytes]],
+    header_key: tp.Union[bytes, str],
+    single: bool = False,
 ) -> tp.List[bytes]:
+    if isinstance(header_key, str):
+        header_key = header_key.encode(HEADERS_ENCODING)
     extracted_headers = []
-
     for key, value in headers:
         if key.lower() == header_key.lower():
             extracted_headers.append(value)
             if single:
                 break
     return extracted_headers
 
 
 def extract_header_values_decoded(
     headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes, single: bool = False
 ) -> tp.List[str]:
     values = extract_header_values(
         headers=headers, header_key=header_key, single=single
     )
-    return [value.decode() for value in values]
+    return [value.decode(HEADERS_ENCODING) for value in values]
 
 
 def header_presents(
     headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes
 ) -> bool:
     return bool(extract_header_values(headers, header_key, single=True))
```

### Comparing `hishel-0.0.2/hishel/_async/_client.py` & `hishel-0.0.3/hishel/_async/_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from hishel._async._transports import AsyncCacheTransport
 
 __all__ = ("AsyncCacheClient",)
 
 
 class AsyncCacheClient(httpx.AsyncClient):
     def __init__(self, *args: tp.Any, **kwargs: tp.Any):
-        self._storage = kwargs.get("cache_storage", None)
-        self._controller = kwargs.get("cache_controller", None)
+        self._storage = kwargs.pop("storage") if "storage" in kwargs else None
+        self._controller = kwargs.pop("controller") if "controller" in kwargs else None
         super().__init__(*args, **kwargs)
 
     def _init_transport(self, *args, **kwargs) -> AsyncCacheTransport:  # type: ignore
         _transport = super()._init_transport(*args, **kwargs)
         return AsyncCacheTransport(
             transport=_transport,
             storage=self._storage,
-            cache_controller=self._controller,
+            controller=self._controller,
         )
 
     def _init_proxy_transport(self, *args, **kwargs) -> AsyncCacheTransport:  # type: ignore
         _transport = super()._init_proxy_transport(*args, **kwargs)  # pragma: no cover
         return AsyncCacheTransport(  # pragma: no cover
             transport=_transport,
             storage=self._storage,
-            cache_controller=self._controller,
+            controller=self._controller,
         )
```

### Comparing `hishel-0.0.2/hishel/_async/_pool.py` & `hishel-0.0.3/hishel/_async/_pool.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,76 @@
-import logging
 import types
 import typing as tp
 
 from httpcore._async.interfaces import AsyncRequestInterface
 from httpcore._models import Request, Response
 
 from .._controller import Controller
-from .._serializers import DictSerializer
-from .._utils import generate_key, normalized_url
+from .._serializers import JSONSerializer
+from .._utils import generate_key
 from ._storages import AsyncBaseStorage, AsyncFileStorage
 
-logger = logging.getLogger("hishel.pool")
-
 T = tp.TypeVar("T")
 
 __all__ = ("AsyncCacheConnectionPool",)
 
 
 class AsyncCacheConnectionPool(AsyncRequestInterface):
     def __init__(
         self,
         pool: AsyncRequestInterface,
         storage: tp.Optional[AsyncBaseStorage] = None,
-        cache_controller: tp.Optional[Controller] = None,
+        controller: tp.Optional[Controller] = None,
     ) -> None:
         self._pool = pool
-
-        if storage is not None:  # pragma: no cover
-            self._storage = storage
-        else:
-            self._storage = AsyncFileStorage(serializer=DictSerializer())
-
-        if cache_controller is not None:  # pragma: no cover
-            self._controller = cache_controller
-        else:
-            self._controller = Controller()
+        self._storage = (
+            storage
+            if storage is not None
+            else AsyncFileStorage(serializer=JSONSerializer())
+        )
+        self._controller = controller if controller is not None else Controller()
 
     async def handle_async_request(self, request: Request) -> Response:
-        key = generate_key(request.method, request.url, request.headers)
+        key = generate_key(request)
         stored_resposne = await self._storage.retreive(key)
 
-        url = normalized_url(request.url)
-
         if stored_resposne:
-            await stored_resposne.aread()
-            logger.debug(f"The cached response for the `{url}` url was found.")
+            # Try using the stored response if it was discovered.
+
             res = self._controller.construct_response_from_cache(
                 request=request, response=stored_resposne
             )
 
             if isinstance(res, Response):
-                logger.debug(f"For the `{url}` url, the cached response was used.")
+                # Simply use the response if the controller determines it is ready for use.
+                res.extensions["from_cache"] = True  # type: ignore[index]
                 return res
-            elif isinstance(res, Request):  # pragma: no cover
-                logger.debug(
-                    f"Validating the response associated with the `{url}` url."
-                )
+
+            if isinstance(res, Request):
+                # Re-validating the response.
+
                 response = await self._pool.handle_async_request(res)
-                await response.aread()
-                updated_response = self._controller.handle_validation_response(
+
+                # Merge headers with the stale response.
+                full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
-                await self._storage.store(key, updated_response)
-                return updated_response
 
-            assert (
-                False
-            ), "invalid return value for `construct_response_from_cache`"  # pragma: no cover
-        logger.debug(f"A cached response to the url `{url}` was not found.")
+                await full_response.aread()
+                await self._storage.store(key, full_response)
+                full_response.extensions["from_cache"] = response.status == 304  # type: ignore[index]
+                return full_response
+
         response = await self._pool.handle_async_request(request)
-        await response.aread()
 
         if self._controller.is_cachable(request=request, response=response):
+            await response.aread()
             await self._storage.store(key, response)
-        else:  # pragma: no cover
-            logger.debug(f"The response to the `{url}` url is not cacheable.")
 
+        response.extensions["from_cache"] = False  # type: ignore[index]
         return response
 
     async def aclose(self) -> None:
         await self._storage.aclose()
 
     async def __aenter__(self: T) -> T:
         return self
```

### Comparing `hishel-0.0.2/hishel/_async/_storages.py` & `hishel-0.0.3/hishel/_async/_storages.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 import redis.asyncio as redis
 from httpcore import Response
 
 from hishel._serializers import BaseSerializer
 
 from .._files import AsyncFileManager
-from .._serializers import DictSerializer
+from .._serializers import JSONSerializer
 from .._synchronization import AsyncLock
 
 logger = logging.getLogger("hishel.storages")
 
 __all__ = ("AsyncFileStorage", "AsyncRedisStorage")
 
 
 class AsyncBaseStorage:
     def __init__(self, serializer: tp.Optional[BaseSerializer] = None) -> None:
         if serializer:  # pragma: no cover
             self._serializer = serializer
         else:
-            self._serializer = DictSerializer()
+            self._serializer = JSONSerializer()
 
     async def store(self, key: str, response: Response) -> None:
         raise NotImplementedError()
 
     async def retreive(self, key: str) -> tp.Optional[Response]:
         raise NotImplementedError()
```

### Comparing `hishel-0.0.2/hishel/_sync/_client.py` & `hishel-0.0.3/hishel/_sync/_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from hishel._sync._transports import CacheTransport
 
 __all__ = ("CacheClient",)
 
 
 class CacheClient(httpx.Client):
     def __init__(self, *args: tp.Any, **kwargs: tp.Any):
-        self._storage = kwargs.get("cache_storage", None)
-        self._controller = kwargs.get("cache_controller", None)
+        self._storage = kwargs.pop("storage") if "storage" in kwargs else None
+        self._controller = kwargs.pop("controller") if "controller" in kwargs else None
         super().__init__(*args, **kwargs)
 
     def _init_transport(self, *args, **kwargs) -> CacheTransport:  # type: ignore
         _transport = super()._init_transport(*args, **kwargs)
         return CacheTransport(
             transport=_transport,
             storage=self._storage,
-            cache_controller=self._controller,
+            controller=self._controller,
         )
 
     def _init_proxy_transport(self, *args, **kwargs) -> CacheTransport:  # type: ignore
         _transport = super()._init_proxy_transport(*args, **kwargs)  # pragma: no cover
         return CacheTransport(  # pragma: no cover
             transport=_transport,
             storage=self._storage,
-            cache_controller=self._controller,
+            controller=self._controller,
         )
```

### Comparing `hishel-0.0.2/hishel/_sync/_pool.py` & `hishel-0.0.3/hishel/_sync/_pool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,76 @@
-import logging
 import types
 import typing as tp
 
 from httpcore._sync.interfaces import RequestInterface
 from httpcore._models import Request, Response
 
 from .._controller import Controller
-from .._serializers import DictSerializer
-from .._utils import generate_key, normalized_url
+from .._serializers import JSONSerializer
+from .._utils import generate_key
 from ._storages import BaseStorage, FileStorage
 
-logger = logging.getLogger("hishel.pool")
-
 T = tp.TypeVar("T")
 
 __all__ = ("CacheConnectionPool",)
 
 
 class CacheConnectionPool(RequestInterface):
     def __init__(
         self,
         pool: RequestInterface,
         storage: tp.Optional[BaseStorage] = None,
-        cache_controller: tp.Optional[Controller] = None,
+        controller: tp.Optional[Controller] = None,
     ) -> None:
         self._pool = pool
-
-        if storage is not None:  # pragma: no cover
-            self._storage = storage
-        else:
-            self._storage = FileStorage(serializer=DictSerializer())
-
-        if cache_controller is not None:  # pragma: no cover
-            self._controller = cache_controller
-        else:
-            self._controller = Controller()
+        self._storage = (
+            storage
+            if storage is not None
+            else FileStorage(serializer=JSONSerializer())
+        )
+        self._controller = controller if controller is not None else Controller()
 
     def handle_request(self, request: Request) -> Response:
-        key = generate_key(request.method, request.url, request.headers)
+        key = generate_key(request)
         stored_resposne = self._storage.retreive(key)
 
-        url = normalized_url(request.url)
-
         if stored_resposne:
-            stored_resposne.read()
-            logger.debug(f"The cached response for the `{url}` url was found.")
+            # Try using the stored response if it was discovered.
+
             res = self._controller.construct_response_from_cache(
                 request=request, response=stored_resposne
             )
 
             if isinstance(res, Response):
-                logger.debug(f"For the `{url}` url, the cached response was used.")
+                # Simply use the response if the controller determines it is ready for use.
+                res.extensions["from_cache"] = True  # type: ignore[index]
                 return res
-            elif isinstance(res, Request):  # pragma: no cover
-                logger.debug(
-                    f"Validating the response associated with the `{url}` url."
-                )
+
+            if isinstance(res, Request):
+                # Re-validating the response.
+
                 response = self._pool.handle_request(res)
-                response.read()
-                updated_response = self._controller.handle_validation_response(
+
+                # Merge headers with the stale response.
+                full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
-                self._storage.store(key, updated_response)
-                return updated_response
 
-            assert (
-                False
-            ), "invalid return value for `construct_response_from_cache`"  # pragma: no cover
-        logger.debug(f"A cached response to the url `{url}` was not found.")
+                full_response.read()
+                self._storage.store(key, full_response)
+                full_response.extensions["from_cache"] = response.status == 304  # type: ignore[index]
+                return full_response
+
         response = self._pool.handle_request(request)
-        response.read()
 
         if self._controller.is_cachable(request=request, response=response):
+            response.read()
             self._storage.store(key, response)
-        else:  # pragma: no cover
-            logger.debug(f"The response to the `{url}` url is not cacheable.")
 
+        response.extensions["from_cache"] = False  # type: ignore[index]
         return response
 
     def close(self) -> None:
         self._storage.close()
 
     def __enter__(self: T) -> T:
         return self
```

### Comparing `hishel-0.0.2/hishel/_sync/_storages.py` & `hishel-0.0.3/hishel/_sync/_storages.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 import redis
 from httpcore import Response
 
 from hishel._serializers import BaseSerializer
 
 from .._files import FileManager
-from .._serializers import DictSerializer
+from .._serializers import JSONSerializer
 from .._synchronization import Lock
 
 logger = logging.getLogger("hishel.storages")
 
 __all__ = ("FileStorage", "RedisStorage")
 
 
 class BaseStorage:
     def __init__(self, serializer: tp.Optional[BaseSerializer] = None) -> None:
         if serializer:  # pragma: no cover
             self._serializer = serializer
         else:
-            self._serializer = DictSerializer()
+            self._serializer = JSONSerializer()
 
     def store(self, key: str, response: Response) -> None:
         raise NotImplementedError()
 
     def retreive(self, key: str) -> tp.Optional[Response]:
         raise NotImplementedError()
```

### Comparing `hishel-0.0.2/LICENSE` & `hishel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.2/pyproject.toml` & `hishel-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.2/PKG-INFO` & `hishel-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -70,73 +70,81 @@
 import hishel
 
 with hishel.CacheClient() as client:
     client.get("https://www.github.com")
     client.get("https://www.github.com")  # takes from the cache (very fast!)
 ```
 
-If the response is cacheable according to **RFC 9111**, hishel will save it for later use, so the user only needs to change the **client and the rest of the staff will be done automatically.**
+or in asynchronous context
 
-Hishel also works well with httpcore, and you can **make your httpcore connection pools cacheable with a single line of code.**
-
-Your existing code
-``` python
-from httpcore import ConnectionPool
-
-pool = ConnectionPool()
+```python
+import hishel
 
-...
+async with hishel.AsyncCacheClient() as client:
+    await client.get("https://www.github.com")
+    await client.get("https://www.github.com")  # takes from the cache
 ```
 
-Adding HTTP caching to your program will make it much faster and more efficient.
-``` python
-import hishel
-from httpcore import ConnectionPool
+## HTTPX and HTTP Core
 
-pool = ConnectionPool()
-pool = hishel.CacheConnectionPool(pool=pool)
-...
-```
+`Hishel` also supports the transports of `HTTPX` and the connection pools of `HTTP Core`.
 
-As you can see, it is **extremely simple to integrate**. 
+`Hishel` respects existing **transports** and **connection pools** and can therefore work **on top of them**, making hishel a very **compatible and flexible library**.
 
-Because `Hishel` respects your custom transports and connection pools, it requires the real **ConnectionPool** and the real **HTTPTransport** to work on top of it.
 
 **Transports** example:
 
 ``` python
 import httpx
 import hishel
 
 transport = httpx.HTTPTransport()
 cache_transport = hishel.CacheTransport(transport=transport)
 
-req = httpx.Request("GET",
-                    "https://google.com")
+req = httpx.Request("GET", "https://www.github.com")
 
 cache_transport.handle_request(req)
-cache_transport.handle_request(req)
+cache_transport.handle_request(req)  # takes from the cache
 ```
 
-## How and where are the responses saved?
+**Connection Pool** example:
+
 
-Hishel supports a variety of backends for storing responses, but the **filesystem is the default**.
+```python
+import httpcore
+import hishel
+
+pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
 
-You can also use another backend, such as **redis**, to store your responses, or even **write your own** if necessary.
+pool.request("GET", "https://www.github.com")
+pool.request("GET", "https://www.github.com")  # takes from the cache
+
+```
+
+## How and where are the responses saved?
+
+The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a variety of built-in storage options, but the default storage is a [filesystem storage](TODO). You can switch the storage to another one that `Hishel` offers or, if necessary, write your own; for more information, see the storage documentation.
 
 
 ## Contributing
 
-Hishel is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
+`Hishel` is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
+
+You can open the pull request by following these instructions if you want to improve `Hishel`. 💓
+
+- Fork the project.
+- Make change.
+- Open the pull request.
+
+# Changelog
 
-The most common strategy for contributing `Hishel` appears to be:
+## 0.0.3 (7/28/2023)
 
-- Fork the project
-- Make change
-- Open the pull request# Changelog
+- Add `from_cache` response extension.
+- Add `typing_extensions` into the requirements.
 
 ## 0.0.2 (7/25/2023)
 
 - Add [redis](https://redis.io/) support.
 - Make backends thread and task safe.
 - Add black as a new linter.
 - Add an expire time for cached responses.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.2 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.3 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -39,32 +39,34 @@
 parts of RFC 9111 **should be ignored and which should not**, for example, you
 can explicitly disable stale responses for your safety or enable re-validation
 for each response before using it. - ð Very fast: When **IO is not
 required**, your requests are even faster. ## QuickStart Install `Hishel` using
 pip: ``` shell $ pip install hishel ``` Let's begin with an example of a httpx
 client. ```python import hishel with hishel.CacheClient() as client: client.get
 ("https://www.github.com") client.get("https://www.github.com") # takes from
-the cache (very fast!) ``` If the response is cacheable according to **RFC
-9111**, hishel will save it for later use, so the user only needs to change the
-**client and the rest of the staff will be done automatically.** Hishel also
-works well with httpcore, and you can **make your httpcore connection pools
-cacheable with a single line of code.** Your existing code ``` python from
-httpcore import ConnectionPool pool = ConnectionPool() ... ``` Adding HTTP
-caching to your program will make it much faster and more efficient. ``` python
-import hishel from httpcore import ConnectionPool pool = ConnectionPool() pool
-= hishel.CacheConnectionPool(pool=pool) ... ``` As you can see, it is
-**extremely simple to integrate**. Because `Hishel` respects your custom
-transports and connection pools, it requires the real **ConnectionPool** and
-the real **HTTPTransport** to work on top of it. **Transports** example: ```
-python import httpx import hishel transport = httpx.HTTPTransport()
-cache_transport = hishel.CacheTransport(transport=transport) req =
-httpx.Request("GET", "https://google.com") cache_transport.handle_request(req)
-cache_transport.handle_request(req) ``` ## How and where are the responses
-saved? Hishel supports a variety of backends for storing responses, but the
-**filesystem is the default**. You can also use another backend, such as
-**redis**, to store your responses, or even **write your own** if necessary. ##
-Contributing Hishel is a powerful tool, but it is also a new project with
-potential flaws, so we welcome contributions! The most common strategy for
-contributing `Hishel` appears to be: - Fork the project - Make change - Open
-the pull request# Changelog ## 0.0.2 (7/25/2023) - Add [redis](https://
-redis.io/) support. - Make backends thread and task safe. - Add black as a new
-linter. - Add an expire time for cached responses.
+the cache (very fast!) ``` or in asynchronous context ```python import hishel
+async with hishel.AsyncCacheClient() as client: await client.get("https://
+www.github.com") await client.get("https://www.github.com") # takes from the
+cache ``` ## HTTPX and HTTP Core `Hishel` also supports the transports of
+`HTTPX` and the connection pools of `HTTP Core`. `Hishel` respects existing
+**transports** and **connection pools** and can therefore work **on top of
+them**, making hishel a very **compatible and flexible library**.
+**Transports** example: ``` python import httpx import hishel transport =
+httpx.HTTPTransport() cache_transport = hishel.CacheTransport
+(transport=transport) req = httpx.Request("GET", "https://www.github.com")
+cache_transport.handle_request(req) cache_transport.handle_request(req) # takes
+from the cache ``` **Connection Pool** example: ```python import httpcore
+import hishel pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
+pool.request("GET", "https://www.github.com") pool.request("GET", "https://
+www.github.com") # takes from the cache ``` ## How and where are the responses
+saved? The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a
+variety of built-in storage options, but the default storage is a [filesystem
+storage](TODO). You can switch the storage to another one that `Hishel` offers
+or, if necessary, write your own; for more information, see the storage
+documentation. ## Contributing `Hishel` is a powerful tool, but it is also a
+new project with potential flaws, so we welcome contributions! You can open the
+pull request by following these instructions if you want to improve `Hishel`.
+ð - Fork the project. - Make change. - Open the pull request. # Changelog ##
+0.0.3 (7/28/2023) - Add `from_cache` response extension. - Add
+`typing_extensions` into the requirements. ## 0.0.2 (7/25/2023) - Add [redis]
+(https://redis.io/) support. - Make backends thread and task safe. - Add black
+as a new linter. - Add an expire time for cached responses.
```

