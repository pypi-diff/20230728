# Comparing `tmp/vprikol_api_python-1.5.tar.gz` & `tmp/vprikol_api_python-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.5.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.6.tar", max compression
```

## Comparing `vprikol_api_python-1.5.tar` & `vprikol_api_python-1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/README.md
--rw-r--r--   0        0        0      349 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/api.py
--rw-r--r--   0        0        0     5949 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/main.py
--rw-r--r--   0        0        0     3940 2023-07-24 11:54:20.057432 vprikol_api_python-1.5/vprikol_api/model.py
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.5/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/README.md
+-rw-r--r--   0        0        0      349 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/api.py
+-rw-r--r--   0        0        0     5949 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/main.py
+-rw-r--r--   0        0        0     3942 2023-07-28 08:23:46.712772 vprikol_api_python-1.6/vprikol_api/model.py
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.6/PKG-INFO
```

### Comparing `vprikol_api_python-1.5/vprikol_api/api.py` & `vprikol_api_python-1.6/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.5/vprikol_api/main.py` & `vprikol_api_python-1.6/vprikol_api/main.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.5/vprikol_api/model.py` & `vprikol_api_python-1.6/vprikol_api/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class FastApiErrorResponse(BaseModel):
     detail: FastAPIErrorDetail | str
 
 
 class APIErrorResponse(BaseModel):
     status_code: int
     detail: str
-    request_queue: int | None = None
+    queue_position: int | None = None
 
 
 class Response(GenericModel):
     data: DataT | None
     error: APIErrorResponse | FastApiErrorResponse | None
     success: bool = True
 
@@ -67,15 +67,15 @@
     is_closed: bool = Field(alias='isClosed')
     server_label: str = Field(alias='serverLabel')
 
 
 class CreatedFindTaskAPIResponse(BaseModel):
     request_id: str
     request_time: int
-    request_queue: int
+    queue_position: int
 
 
 class PlayerInfoArizonaAPIResponse(BaseModel):
     account_id: int = Field(alias='accountId')
     player_id: int | None = Field(alias='playerId')
     lvl: int
     cash: int
```

