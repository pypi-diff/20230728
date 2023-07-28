# Comparing `tmp/vprikol_api_python-1.6.tar.gz` & `tmp/vprikol_api_python-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.6.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.7.tar", max compression
```

## Comparing `vprikol_api_python-1.6.tar` & `vprikol_api_python-1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/README.md
--rw-r--r--   0        0        0      349 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/pyproject.toml
--rw-r--r--   0        0        0       51 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/api.py
--rw-r--r--   0        0        0     5949 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/main.py
--rw-r--r--   0        0        0     3942 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/model.py
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.6/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/README.md
+-rw-r--r--   0        0        0      349 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/vprikol_api/api.py
+-rw-r--r--   0        0        0     5956 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/vprikol_api/main.py
+-rw-r--r--   0        0        0     3916 2023-07-28 08:29:20.754295 vprikol_api_python-1.7/vprikol_api/model.py
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.7/PKG-INFO
```

### Comparing `vprikol_api_python-1.6/vprikol_api/api.py` & `vprikol_api_python-1.7/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.6/vprikol_api/main.py` & `vprikol_api_python-1.7/vprikol_api/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,23 +62,23 @@
             result = await get(url=f'{self.base_url}find/getTaskResult', headers=self.headers,
                                params={'request_id': task.request_id})
 
             if not result.success and result.error.error_code and result.error.error_code == 425:
                 await asyncio.sleep(1)
                 continue
 
-            if result.error and result.error.error_code == 422:
+            if result.error and result.error.status_code == 422:
                 return PlayerInfoNotFound(**result.error.dict())
 
             try:
                 return PlayerInfoArizonaAPIResponse(**result.data)
             except ValidationError:
                 return PlayerInfoArizonaAPIResponse(**result.data)
 
-    async def get_server_status(self, server_id: int | None = None) -> ServerStatusAPIResponse:
+    async def get_server_status(self, server_id: int | None = None) -> list[ServerStatusAPIResponse]:
         if server_id:
             params = {'server': server_id}
         else:
             params = None
 
         result = await get(url=f'{self.base_url}status', headers=self.headers,
                            params=params)
```

### Comparing `vprikol_api_python-1.6/vprikol_api/model.py` & `vprikol_api_python-1.7/vprikol_api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Literal, Generic, TypeVar
+from typing import TypeVar
 
 from pydantic import BaseModel, Field
 from pydantic.generics import GenericModel
 
 DataT = TypeVar('DataT')
 
 
@@ -13,15 +13,15 @@
 
 
 class FastApiErrorResponse(BaseModel):
     detail: FastAPIErrorDetail | str
 
 
 class APIErrorResponse(BaseModel):
-    status_code: int
+    error_code: int
     detail: str
     queue_position: int | None = None
 
 
 class Response(GenericModel):
     data: DataT | None
     error: APIErrorResponse | FastApiErrorResponse | None
```

