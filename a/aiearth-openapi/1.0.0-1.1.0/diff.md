# Comparing `tmp/aiearth-openapi-1.0.0.tar.gz` & `tmp/aiearth-openapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiearth-openapi-1.0.0.tar", last modified: Thu Jun  8 06:22:34 2023, max compression
+gzip compressed data, was "aiearth-openapi-1.1.0.tar", last modified: Fri Jul 28 04:09:51 2023, max compression
```

## Comparing `aiearth-openapi-1.0.0.tar` & `aiearth-openapi-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:22:34.875435 aiearth-openapi-1.0.0/
--rw-r--r--   0 songci     (502) staff       (20)      340 2023-06-08 06:22:34.874961 aiearth-openapi-1.0.0/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)       15 2023-05-26 05:48:12.000000 aiearth-openapi-1.0.0/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:22:34.867302 aiearth-openapi-1.0.0/aiearth/
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:22:34.870463 aiearth-openapi-1.0.0/aiearth/openapi/
--rw-r--r--   0 songci     (502) staff       (20)      546 2023-06-06 06:56:50.000000 aiearth-openapi-1.0.0/aiearth/openapi/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     3377 2023-05-29 11:40:11.000000 aiearth-openapi-1.0.0/aiearth/openapi/enums.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:22:34.871025 aiearth-openapi-1.0.0/aiearth/openapi/models/
--rw-r--r--   0 songci     (502) staff       (20)       56 2023-05-26 07:59:47.000000 aiearth-openapi-1.0.0/aiearth/openapi/models/__init__.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:22:34.874318 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      340 2023-06-08 06:22:34.000000 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      300 2023-06-08 06:22:34.000000 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-06-08 06:22:34.000000 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)       43 2023-06-08 06:22:34.000000 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        8 2023-06-08 06:22:34.000000 aiearth-openapi-1.0.0/aiearth_openapi.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-06-08 06:22:34.875567 aiearth-openapi-1.0.0/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)     1078 2023-06-06 06:54:36.000000 aiearth-openapi-1.0.0/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 04:09:51.968430 aiearth-openapi-1.1.0/
+-rw-r--r--   0 songci     (502) staff       (20)      340 2023-07-28 04:09:51.968031 aiearth-openapi-1.1.0/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)       15 2023-05-26 05:48:12.000000 aiearth-openapi-1.1.0/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 04:09:51.959262 aiearth-openapi-1.1.0/aiearth/
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 04:09:51.963857 aiearth-openapi-1.1.0/aiearth/openapi/
+-rw-r--r--   0 songci     (502) staff       (20)      717 2023-07-20 07:25:22.000000 aiearth-openapi-1.1.0/aiearth/openapi/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2212 2023-07-20 06:41:00.000000 aiearth-openapi-1.1.0/aiearth/openapi/client.py
+-rw-r--r--   0 songci     (502) staff       (20)     3465 2023-07-19 11:51:54.000000 aiearth-openapi-1.1.0/aiearth/openapi/enums.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 04:09:51.964433 aiearth-openapi-1.1.0/aiearth/openapi/models/
+-rw-r--r--   0 songci     (502) staff       (20)     8461 2023-07-20 06:41:00.000000 aiearth-openapi-1.1.0/aiearth/openapi/models/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)      532 2023-07-19 11:38:42.000000 aiearth-openapi-1.1.0/aiearth/openapi/oss.py
+-rw-r--r--   0 songci     (502) staff       (20)    13013 2023-07-27 03:04:38.000000 aiearth-openapi-1.1.0/aiearth/openapi/publisher.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 04:09:51.967522 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      340 2023-07-28 04:09:51.000000 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      378 2023-07-28 04:09:51.000000 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-28 04:09:51.000000 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)       43 2023-07-28 04:09:51.000000 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        8 2023-07-28 04:09:51.000000 aiearth-openapi-1.1.0/aiearth_openapi.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-28 04:09:51.968546 aiearth-openapi-1.1.0/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1078 2023-06-06 06:54:36.000000 aiearth-openapi-1.1.0/setup.py
```

### Comparing `aiearth-openapi-1.0.0/aiearth/openapi/__init__.py` & `aiearth-openapi-1.1.0/aiearth/openapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from alibabacloud_tea_openapi.models import Config
 from alibabacloud_aiearth_engine20220609.client import Client
 from aiearth.core.client.endpoints import Endpoints
 
 __ENDPOINT__ = Endpoints.OPENAPI_ENDPOINT
 __REGION_ID__ = Endpoints.OPENAPI_REGION_ID
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
+
+from aiearth.openapi.publisher import ExtClient
+
 
 def build_client(access_key_id, access_key_secret, endpoint=__ENDPOINT__):
     config = Config(
         access_key_id=access_key_id,
         access_key_secret=access_key_secret,
         region_id=__REGION_ID__,
         endpoint=endpoint
     )
 
-    return Client(config)
+    from aiearth import core
+    core.Authenticate(access_key_id=access_key_id, access_key_secret=access_key_secret)
+
+    return ExtClient(config)
```

### Comparing `aiearth-openapi-1.0.0/aiearth/openapi/enums.py` & `aiearth-openapi-1.1.0/aiearth/openapi/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,18 @@
     """
     RPB = "rpb"
     RPC = "rpc"
     TFW = "tfw"
     IGE = "ige"
 
 
+class VectorType(Enum):
+    SHAPE = "shape"
+
+
 class MapServiceProjectionType(Enum):
     """
     地图服务投影类型
     """
     # 经纬度投影
     LONGLAT = "longlat"
     # 墨卡托投影
@@ -122,22 +126,26 @@
 
 
 class DataType(Enum):
     """
     数据类型
     """
     # 栅格
-    RATSER = "raster"
+    RASTER = "raster"
     # 矢量
     VECTOR = "vector"
     # 地图服务
     MAP_SERVICE = "map_service"
+    # 数据集
+    DATASET = "dataset"
+
 
 class DownloadStatus(Enum):
     INITED = "inited"
     PROCESSING = "processing"
     FINISHED = "finished"
     FAILED = "failed"
 
+
 class JobOutDataType(Enum):
     RASTER = 0
     VECTOR = 1
```

### Comparing `aiearth-openapi-1.0.0/setup.py` & `aiearth-openapi-1.1.0/setup.py`

 * *Files identical despite different names*

