# Comparing `tmp/happyaccidentsapi-0.0.1.tar.gz` & `tmp/happyaccidentsapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyaccidentsapi-0.0.1.tar", max compression
+gzip compressed data, was "happyaccidentsapi-0.0.2.tar", max compression
```

## Comparing `happyaccidentsapi-0.0.1.tar` & `happyaccidentsapi-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.1/LICENSE
--rw-r--r--   0        0        0     1831 2023-07-28 17:01:49.246542 happyaccidentsapi-0.0.1/PYPI.md
--rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.1/happyaccidentsapi/__init__.py
--rw-r--r--   0        0        0     8051 2023-07-28 15:44:14.084288 happyaccidentsapi-0.0.1/happyaccidentsapi/_happyaccidentsapi.py
--rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.1/happyaccidentsapi/_token.py
--rw-r--r--   0        0        0     2847 2023-07-28 13:23:32.859138 happyaccidentsapi-0.0.1/happyaccidentsapi/enums.py
--rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.1/happyaccidentsapi/errors.py
--rw-r--r--   0        0        0    12581 2023-07-28 16:15:56.041644 happyaccidentsapi-0.0.1/happyaccidentsapi/models.py
--rw-r--r--   0        0        0     1117 2023-07-28 17:05:56.665202 happyaccidentsapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1831 2023-07-28 17:01:49.246542 happyaccidentsapi-0.0.2/PYPI.md
+-rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.2/happyaccidentsapi/__init__.py
+-rw-r--r--   0        0        0     8071 2023-07-28 17:39:42.259527 happyaccidentsapi-0.0.2/happyaccidentsapi/_happyaccidentsapi.py
+-rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.2/happyaccidentsapi/_token.py
+-rw-r--r--   0        0        0     2847 2023-07-28 13:23:32.859138 happyaccidentsapi-0.0.2/happyaccidentsapi/enums.py
+-rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.2/happyaccidentsapi/errors.py
+-rw-r--r--   0        0        0    12912 2023-07-28 17:39:45.639578 happyaccidentsapi-0.0.2/happyaccidentsapi/models.py
+-rw-r--r--   0        0        0     1118 2023-07-28 17:39:54.293041 happyaccidentsapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.2/PKG-INFO
```

### Comparing `happyaccidentsapi-0.0.1/LICENSE` & `happyaccidentsapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.1/PYPI.md` & `happyaccidentsapi-0.0.2/PYPI.md`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.1/happyaccidentsapi/_happyaccidentsapi.py` & `happyaccidentsapi-0.0.2/happyaccidentsapi/_happyaccidentsapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
                 },
             )
             data = await self._proceed_response(response)
             return ApiPaginatedListResponseInferenceHistoricalResult.model_validate(
                 data
             )
 
+    @token_required
     async def fetch_community_inferences(
         self,
         current_page: int = 0,
         page_size: int = 10,
         favorites_only: bool = True,
         nsfw: bool = False,
         query: str = "",
```

### Comparing `happyaccidentsapi-0.0.1/happyaccidentsapi/_token.py` & `happyaccidentsapi-0.0.2/happyaccidentsapi/_token.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.1/happyaccidentsapi/enums.py` & `happyaccidentsapi-0.0.2/happyaccidentsapi/enums.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.1/happyaccidentsapi/errors.py` & `happyaccidentsapi-0.0.2/happyaccidentsapi/errors.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.1/happyaccidentsapi/models.py` & `happyaccidentsapi-0.0.2/happyaccidentsapi/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,113 +4,113 @@
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import aiofiles
 from aiohttp import ClientSession
-from pydantic import BaseModel, Field, HttpUrl
+from pydantic import AnyUrl, BaseModel, Field, HttpUrl
 
 from .enums import *
 from .errors import handle_error
 
 
 class ModelCreator(BaseModel):
     username: str
-    image: HttpUrl
+    image: Optional[AnyUrl]
 
 
 class ModelFileMetadata(BaseModel):
-    format: str
-    fp: Union[str, None] = None
-    size: Union[str, None] = None
+    format: Optional[str] = None
+    fp: Optional[str] = None
+    size: Optional[str] = None
 
 
 class ModelImage(BaseModel):
-    url: HttpUrl
+    url: AnyUrl
     nsfw: Union[bool, str]
     width: int
     height: int
-    generationProcess: Union[str, None]
+    generationProcess: Optional[str] = None
 
 
 class ModelFile(BaseModel):
     name: str
     id: int
     sizeKb: float
     type: str
-    pickleScanResult: str
-    pickleScanMessage: str
-    virusScanResult: str
-    scannedAt: datetime
-    downloadUrl: HttpUrl
-    format: Union[str, None]
-    metadata: ModelFileMetadata
+    pickleScanResult: Optional[str] = None
+    pickleScanMessage: Optional[str] = None
+    virusScanResult: Optional[str] = None
+    scannedAt: Union[datetime, str, None] = ""
+    downloadUrl: Optional[AnyUrl] = None
+    format: Optional[str] = None
+    metadata: Optional[ModelFileMetadata] = None
 
 
 class ModelVersion(BaseModel):
     id: int
     modelId: int
     name: str
     baseModel: CivitAiBaseModelType  # noqa: 405
-    description: Union[str, None]
+    description: Optional[str] = None
     trainedWords: List[str]
-    createdAt: datetime
+    createdAt: Optional[datetime] = None
     files: List[ModelFile]
     images: List[ModelImage]
 
 
 class ModelStats(BaseModel):
-    downloadCount: int
-    favoriteCount: int
-    commentCount: int
-    ratingCount: int
-    rating: float
+    downloadCount: Optional[int] = None
+    favoriteCount: Optional[int] = None
+    commentCount: Optional[int] = None
+    ratingCount: Optional[int] = None
+    rating: Optional[float] = None
 
 
 class MetadataItemVersion(BaseModel):
     name: str
     id: str
-    createdAt: datetime
+    createdAt: Optional[datetime] = None
     modelMetadataItemId: str
     externalId: Union[int, str]
     baseModel: CivitAiBaseModelType  # noqa: 405
     description: str
-    downloadUrl: HttpUrl
+    downloadUrl: AnyUrl
     images: List[ModelImage]
     files: List[ModelFile]
 
 
 class MetadataItem(BaseModel):
     id: str
     name: str
-    activeVersionId: Union[str, None] = None
+    activeVersionId: Optional[str] = None
     activeVersion: Union[MetadataItemVersion, None] = None
-    author: Union[str, None]
-    authorAvatarUrl: Union[HttpUrl, None] = None
+    author: Optional[str] = None
+    authorAvatarUrl: Optional[AnyUrl] = None
     externalId: Union[int, str]
     type: CivitAiModelType  # noqa: 405
     allowCommercialUse: str
     allowNoCredit: bool
     nsfw: bool
-    description: Union[str, None]
+    description: Optional[str] = None
     requestingUserId: str
-    createdAt: datetime
+    createdAt: Optional[datetime] = None
     ratings: ModelStats
     downloadStatus: DownloadStatus  # noqa
     tags: List[str]
     trainedWords: List[str]
-    thumbnailImageUrl: HttpUrl
-    thumbnailImageNsfw: bool
+    thumbnailImageUrl: Optional[AnyUrl] = None
+    thumbnailImageNsfw: Optional[bool] = None
     versionMetadataItems: List[MetadataItemVersion]
-    volumePath: Union[str, None]
-    modelCheckpointFilename: Union[str, None]
-    modelProvider: Union[str, None]
-    configYaml: Union[str, None]
-    datetimeDeleted: Union[datetime, None]
+    volumePath: Optional[str] = None
+    modelCheckpointFilename: Optional[str] = None
+    modelProvider: Optional[str] = None
+    configYaml: Optional[str] = None
+    datetimeDeleted: Optional[datetime] = None
 
 
 class MetadataItems(BaseModel):
     items: List[MetadataItem]
     paginationMetadata: RangePaginationMetadata
 
     def first(self):
@@ -134,15 +134,15 @@
 
 
 class ModelsMetadata(BaseModel):
     totalItems: int
     currentPage: int
     pageSize: int
     totalPages: int
-    nextPage: Union[HttpUrl, None] = None
+    nextPage: Optional[AnyUrl] = None
 
 
 class Models(BaseModel):
     items: List[Model]
     metadata: ModelsMetadata
 
     def first(self):
```

### Comparing `happyaccidentsapi-0.0.1/pyproject.toml` & `happyaccidentsapi-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "happyaccidentsapi"
-version = "0.0.1"
+version = "0.0.2"
 description = "API Wrapper for HappyAccidents"
 authors = ["hoopengo <hoopengo@yandex.ru>"]
 readme = ["PYPI.md"]
 license = "Apache-2.0"
 repository = "https://github.com/hoopengo/happyaccidentsapi"
 keywords = ["api", "happyaccidents", "ai"]
 classifiers = [
@@ -19,16 +19,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "2.0.0"
-aiohttp = { extras = ["speedups"], version = "^3.8.5" }
+pydantic = "^2.0.0"
+aiohttp = { extras = ["speedups"], version = "^3.8.4" }
 aiofiles = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 
 [build-system]
```

### Comparing `happyaccidentsapi-0.0.1/PKG-INFO` & `happyaccidentsapi-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyaccidentsapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: API Wrapper for HappyAccidents
 Home-page: https://github.com/hoopengo/happyaccidentsapi
 License: Apache-2.0
 Keywords: api,happyaccidents,ai
 Author: hoopengo
 Author-email: hoopengo@yandex.ru
 Requires-Python: >=3.8,<4.0
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0)
-Requires-Dist: pydantic (==2.0.0)
+Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/hoopengo/happyaccidentsapi
 Description-Content-Type: text/markdown
 
 <img alt="banner" src="https://raw.githubusercontent.com/hoopengo/hoopengo/master/images/HappyAccidentsAPI/banner-light.svg" style="max-width: 100%;">
 
 ## HappyAccidentsAPI
```

