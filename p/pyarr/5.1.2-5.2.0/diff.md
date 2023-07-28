# Comparing `tmp/pyarr-5.1.2.tar.gz` & `tmp/pyarr-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarr-5.1.2.tar", max compression
+gzip compressed data, was "pyarr-5.2.0.tar", max compression
```

## Comparing `pyarr-5.1.2.tar` & `pyarr-5.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1056 2023-07-26 15:00:27.061761 pyarr-5.1.2/LICENSE
--rw-r--r--   0        0        0     6525 2023-07-26 15:00:27.061761 pyarr-5.1.2/README.md
--rw-r--r--   0        0        0      249 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/__init__.py
--rw-r--r--   0        0        0    32046 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/base.py
--rw-r--r--   0        0        0      182 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/const.py
--rw-r--r--   0        0        0     1081 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/exceptions.py
--rw-r--r--   0        0        0    28396 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/lidarr.py
--rw-r--r--   0        0        0        0 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/__init__.py
--rw-r--r--   0        0        0     2592 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/common.py
--rw-r--r--   0        0        0     1828 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/lidarr.py
--rw-r--r--   0        0        0     1964 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/radarr.py
--rw-r--r--   0        0        0     1867 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/readarr.py
--rw-r--r--   0        0        0     2165 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/models/sonarr.py
--rw-r--r--   0        0        0        0 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/py.typed
--rw-r--r--   0        0        0    21169 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/radarr.py
--rw-r--r--   0        0        0    31608 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/readarr.py
--rw-r--r--   0        0        0     8346 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/request_handler.py
--rw-r--r--   0        0        0    26239 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/sonarr.py
--rw-r--r--   0        0        0      300 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyarr/types.py
--rw-r--r--   0        0        0     3092 2023-07-26 15:00:27.061761 pyarr-5.1.2/pyproject.toml
--rw-r--r--   0        0        0     7629 1970-01-01 00:00:00.000000 pyarr-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-28 14:51:24.475690 pyarr-5.2.0/LICENSE
+-rw-r--r--   0        0        0     6525 2023-07-28 14:51:24.475690 pyarr-5.2.0/README.md
+-rw-r--r--   0        0        0      249 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/__init__.py
+-rw-r--r--   0        0        0    32046 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/base.py
+-rw-r--r--   0        0        0      182 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/const.py
+-rw-r--r--   0        0        0     1081 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/lib/__init__.py
+-rw-r--r--   0        0        0     1925 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/lib/alias_decorator.py
+-rw-r--r--   0        0        0    28396 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/lidarr.py
+-rw-r--r--   0        0        0        0 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/common.py
+-rw-r--r--   0        0        0     1828 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/lidarr.py
+-rw-r--r--   0        0        0     1964 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/radarr.py
+-rw-r--r--   0        0        0     1867 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/readarr.py
+-rw-r--r--   0        0        0     2165 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/models/sonarr.py
+-rw-r--r--   0        0        0        0 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/py.typed
+-rw-r--r--   0        0        0    22955 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/radarr.py
+-rw-r--r--   0        0        0    31608 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/readarr.py
+-rw-r--r--   0        0        0     8346 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/request_handler.py
+-rw-r--r--   0        0        0    26427 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/sonarr.py
+-rw-r--r--   0        0        0      300 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyarr/types.py
+-rw-r--r--   0        0        0     3092 2023-07-28 14:51:24.479690 pyarr-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7629 1970-01-01 00:00:00.000000 pyarr-5.2.0/PKG-INFO
```

### Comparing `pyarr-5.1.2/LICENSE` & `pyarr-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/README.md` & `pyarr-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/base.py` & `pyarr-5.2.0/pyarr/base.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/exceptions.py` & `pyarr-5.2.0/pyarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/lidarr.py` & `pyarr-5.2.0/pyarr/lidarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/models/common.py` & `pyarr-5.2.0/pyarr/models/common.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/models/lidarr.py` & `pyarr-5.2.0/pyarr/models/lidarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/models/radarr.py` & `pyarr-5.2.0/pyarr/models/radarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/models/readarr.py` & `pyarr-5.2.0/pyarr/models/readarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/models/sonarr.py` & `pyarr-5.2.0/pyarr/models/sonarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/radarr.py` & `pyarr-5.2.0/pyarr/radarr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import Any, Optional, Union
 from warnings import warn
 
 from requests import Response
 
 from pyarr.const import DEPRECATION_WARNING
 from pyarr.types import JsonArray, JsonObject
@@ -630,7 +631,60 @@
         Args:
             data (JsonObject): Data containing changes
 
         Returns:
             JsonObject: Dictionary of updated record
         """
         return self._put("manualimport", self.ver_uri, data=data)
+
+    ## RELEASE
+
+    # GET /release
+    def get_release(self, id_: Optional[int] = None) -> JsonArray:
+        """Query indexers for latest releases.
+
+        Args:
+            id_ (int): Database id for movie to check
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        return self._get("release", self.ver_uri, {"movieId": id_} if id_ else None)
+
+    # POST /release
+    def post_release(self, guid: str, indexer_id: int) -> JsonObject:
+        """Adds a previously searched release to the download client, if the release is
+         still in Radarr's search cache (30 minute cache). If the release is not found
+         in the cache Radarr will return a 404.
+
+        Args:
+            guid (str): Recently searched result guid
+            indexer_id (int): Database id of indexer to use
+
+        Returns:
+            JsonObject: Dictionary with download release details
+        """
+        data = {"guid": guid, "indexerId": indexer_id}
+        return self._post("release", self.ver_uri, data=data)
+
+    # POST /release/push
+    def post_release_push(
+        self, title: str, download_url: str, protocol: str, publish_date: datetime
+    ) -> Any:
+        """If the title is wanted, Radarr will grab it.
+
+        Args:
+            title (str): Release name
+            download_url (str): .torrent file URL
+            protocol (str): "Usenet" or "Torrent
+            publish_date (datetime): ISO8601 date
+
+        Returns:
+            JSON: Array
+        """
+        data = {
+            "title": title,
+            "downloadUrl": download_url,
+            "protocol": protocol,
+            "publishDate": publish_date.isoformat(),
+        }
+        return self._post("release/push", self.ver_uri, data=data)
```

### Comparing `pyarr-5.1.2/pyarr/readarr.py` & `pyarr-5.2.0/pyarr/readarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/request_handler.py` & `pyarr-5.2.0/pyarr/request_handler.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.1.2/pyarr/sonarr.py` & `pyarr-5.2.0/pyarr/sonarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 from requests import Response
 
 from pyarr.const import DEPRECATION_WARNING
 from pyarr.exceptions import PyarrMissingArgument
 from pyarr.types import JsonArray, JsonObject
 
 from .base import BaseArrAPI
+from .lib.alias_decorator import alias, aliased
 from .models.common import PyarrHistorySortKey, PyarrSortDirection
 from .models.sonarr import SonarrCommands, SonarrSortKey
 
 
+@aliased
 class SonarrAPI(BaseArrAPI):
     """API wrapper for Sonarr endpoints."""
 
     def __init__(self, host_url: str, api_key: str, ver_uri: str = "/v3"):
         """Initialize the Sonarr API.
 
         Args:
@@ -394,27 +396,29 @@
             stacklevel=2,
         )
         return self._get("parse", self.ver_uri, {"path": file_path})
 
     ## RELEASE
 
     # GET /release
-    def get_releases(self, id_: Optional[int] = None) -> JsonArray:
+    @alias("get_releases", deprecated_version="6.0.0")
+    def get_release(self, id_: Optional[int] = None) -> JsonArray:
         """Query indexers for latest releases.
 
         Args:
             id_ (int): Database id for episode to check
 
         Returns:
             JsonArray: List of dictionaries with items
         """
         return self._get("release", self.ver_uri, {"episodeId": id_} if id_ else None)
 
     # POST /release
-    def download_release(self, guid: str, indexer_id: int) -> JsonObject:
+    @alias("download_release", "6.0.0")
+    def post_release(self, guid: str, indexer_id: int) -> JsonObject:
         """Adds a previously searched release to the download client, if the release is
          still in Sonarr's search cache (30 minute cache). If the release is not found
          in the cache Sonarr will return a 404.
 
         Args:
             guid (str): Recently searched result guid
             indexer_id (int): Database id of indexer to use
@@ -423,15 +427,16 @@
             JsonObject: Dictionary with download release details
         """
         data = {"guid": guid, "indexerId": indexer_id}
         return self._post("release", self.ver_uri, data=data)
 
     # POST /release/push
     # TODO: find response
-    def push_release(
+    @alias("push_release", "6.0.0")
+    def post_release_push(
         self, title: str, download_url: str, protocol: str, publish_date: datetime
     ) -> Any:
         """If the title is wanted, Sonarr will grab it.
 
         Args:
             title (str): Release name
             download_url (str): .torrent file URL
```

### Comparing `pyarr-5.1.2/pyproject.toml` & `pyarr-5.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyarr"
-version = "5.1.2"
+version = "5.2.0"
 description = "Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python"
 authors = ["Steven Marks <marksie1988@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sonarr", "radarr", "readarr", "lidarr", "api", "wrapper", "plex"]
 homepage = "https://github.com/totaldebug/pyarr"
 repository = "https://github.com/totaldebug/pyarr"
```

### Comparing `pyarr-5.1.2/PKG-INFO` & `pyarr-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarr
-Version: 5.1.2
+Version: 5.2.0
 Summary: Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python
 Home-page: https://github.com/totaldebug/pyarr
 License: MIT
 Keywords: sonarr,radarr,readarr,lidarr,api,wrapper,plex
 Author: Steven Marks
 Author-email: marksie1988@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyarr Version: 5.1.2 Summary: Synchronous Sonarr,
+Metadata-Version: 2.1 Name: pyarr Version: 5.2.0 Summary: Synchronous Sonarr,
 Radarr, Lidarr and Readarr API's for Python Home-page: https://github.com/
 totaldebug/pyarr License: MIT Keywords:
 sonarr,radarr,readarr,lidarr,api,wrapper,plex Author: Steven Marks Author-
 email: marksie1988@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

