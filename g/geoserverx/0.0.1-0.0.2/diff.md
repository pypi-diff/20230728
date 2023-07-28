# Comparing `tmp/geoserverx-0.0.1.tar.gz` & `tmp/geoserverx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoserverx-0.0.1.tar", max compression
+gzip compressed data, was "geoserverx-0.0.2.tar", max compression
```

## Comparing `geoserverx-0.0.1.tar` & `geoserverx-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-05-26 12:19:10.430540 geoserverx-0.0.1/LICENSE
--rw-r--r--   0        0        0      614 2023-05-26 12:19:10.438540 geoserverx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/_async/__init__.py
--rw-r--r--   0        0        0    10154 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/_async/gsx.py
--rw-r--r--   0        0        0        0 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/_sync/__init__.py
--rw-r--r--   0        0        0     9201 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/_sync/gsx.py
--rw-r--r--   0        0        0    11769 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/cli/cli.py
--rw-r--r--   0        0        0        0 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/__init__.py
--rw-r--r--   0        0        0      799 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/coverages_store.py
--rw-r--r--   0        0        0     1386 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/data_store.py
--rw-r--r--   0        0        0      187 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/gs_response.py
--rw-r--r--   0        0        0      493 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/style.py
--rw-r--r--   0        0        0      728 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/models/workspace.py
--rw-r--r--   0        0        0        0 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/__init__.py
--rw-r--r--   0        0        0      682 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/auth.py
--rw-r--r--   0        0        0      705 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/enums.py
--rw-r--r--   0        0        0      193 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/errors.py
--rw-r--r--   0        0        0      180 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/http_client.py
--rw-r--r--   0        0        0      358 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/logger.py
--rw-r--r--   0        0        0     3220 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/services/async_datastore.py
--rw-r--r--   0        0        0     3288 2023-05-26 12:19:10.438540 geoserverx-0.0.1/src/geoserverx/utils/services/datastore.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 geoserverx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 12:52:31.863898 geoserverx-0.0.2/LICENSE
+-rw-r--r--   0        0        0      614 2023-07-28 12:52:31.867898 geoserverx-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/_async/__init__.py
+-rw-r--r--   0        0        0    11581 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/_async/gsx.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/_sync/__init__.py
+-rw-r--r--   0        0        0    10642 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/_sync/gsx.py
+-rw-r--r--   0        0        0    13549 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/__init__.py
+-rw-r--r--   0        0        0      799 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/coverages_store.py
+-rw-r--r--   0        0        0     1386 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/data_store.py
+-rw-r--r--   0        0        0      187 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/gs_response.py
+-rw-r--r--   0        0        0     1193 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/layers.py
+-rw-r--r--   0        0        0      493 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/style.py
+-rw-r--r--   0        0        0      728 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/models/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/__init__.py
+-rw-r--r--   0        0        0      682 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/auth.py
+-rw-r--r--   0        0        0      882 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/enums.py
+-rw-r--r--   0        0        0      193 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/errors.py
+-rw-r--r--   0        0        0      180 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/http_client.py
+-rw-r--r--   0        0        0      358 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/logger.py
+-rw-r--r--   0        0        0     3220 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/services/async_datastore.py
+-rw-r--r--   0        0        0     3288 2023-07-28 12:52:31.867898 geoserverx-0.0.2/src/geoserverx/utils/services/datastore.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 geoserverx-0.0.2/PKG-INFO
```

### Comparing `geoserverx-0.0.1/LICENSE` & `geoserverx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/pyproject.toml` & `geoserverx-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoserverx"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["krishnaglodha <krishnaglodha@gmail.com>"]
 
 [tool.poetry.scripts]
 gsx = "geoserverx.cli.cli:app"
 
 [tool.poetry.dependencies]
```

### Comparing `geoserverx-0.0.1/src/geoserverx/_async/gsx.py` & `geoserverx-0.0.2/src/geoserverx/_async/gsx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Union
+from typing import Union, Optional
 from geoserverx.utils.logger import std_out_logger
 from geoserverx.utils.enums import GSResponseEnum
 from geoserverx.models.gs_response import GSResponse
 from geoserverx.utils.errors import GeoServerXError
 from geoserverx.models.style import StyleModel, AllStylesModel
 import asyncio
 from geoserverx.utils.http_client import AsyncClient
@@ -17,14 +17,15 @@
 from geoserverx.models.data_store import (
     DataStoreModel,
     DataStoresModel,
     CreateDataStoreModel,
     CreateStoreItem,
     MainCreateDataStoreModel,
 )
+from geoserverx.models.layers import LayersModel, LayerModel
 from geoserverx.models.coverages_store import CoveragesStoreModel, CoveragesStoresModel
 from geoserverx.models.gs_response import GSResponse
 from geoserverx.utils.services.async_datastore import (
     AddDataStoreProtocol,
     CreateFileStore,
     ShapefileStore,
     GPKGfileStore,
@@ -81,14 +82,16 @@
             resp = GSResponseEnum._503.value
         elif r == 404:
             resp = GSResponseEnum._404.value
         elif r == 403:
             resp = GSResponseEnum._403.value
         elif r == 201:
             resp = GSResponseEnum._201.value
+        elif r == 200:
+            resp = GSResponseEnum._200.value
         elif r == 409:
             resp = GSResponseEnum._409.value
         return GSResponse.parse_obj(resp)
 
     # Get all workspaces
     async def get_all_workspaces(self) -> Union[WorkspacesModel, GSResponse]:
         Client = self.http_client
@@ -274,7 +277,41 @@
         elif service_type == "gpkg":
             service = GPKGfileStore(
                 service=service, logger=std_out_logger("GeoPackage"), file=file
             )
         else:
             raise ValueError(f"Service type {service_type} not supported")
         await service.addFile(self.http_client, workspace, store)
+
+    # Get all layers
+    async def get_all_layers(
+        self, workspace: Optional[str] = None
+    ) -> Union[LayersModel, GSResponse]:
+        Client = self.http_client
+        if workspace:
+            responses = await Client.get(f"/workspaces/{workspace}/layers")
+        else:
+            responses = await Client.get(f"layers")
+        if responses.status_code == 200:
+            return LayersModel.parse_obj(responses.json())
+        else:
+            results = self.response_recognise(responses.status_code)
+            return results
+
+    # Get specific layer
+    async def get_layer(
+        self, workspace: str, layer: str
+    ) -> Union[LayerModel, GSResponse]:
+        Client = self.http_client
+        responses = await Client.get(f"layers/{workspace}:{layer}")
+        if responses.status_code == 200:
+            return LayerModel.parse_obj(responses.json())
+        else:
+            results = self.response_recognise(responses.status_code)
+            return results
+
+    # Delete specific layer
+    async def delete_layer(self, workspace: str, layer: str) -> GSResponse:
+        Client = self.http_client
+        responses = await Client.delete(f"layers/{workspace}:{layer}")
+        results = self.response_recognise(responses.status_code)
+        return results
```

### Comparing `geoserverx-0.0.1/src/geoserverx/_sync/gsx.py` & `geoserverx-0.0.2/src/geoserverx/_sync/gsx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Union
+from typing import Union, Optional
 from geoserverx.utils.logger import std_out_logger
 import logging
 
 from geoserverx.utils.errors import GeoServerXError
 from geoserverx.utils.enums import GSResponseEnum, HTTPXErrorEnum
 
 from geoserverx.models.style import StyleModel, AllStylesModel
@@ -16,14 +16,16 @@
 from geoserverx.models.data_store import (
     DataStoreModel,
     DataStoresModel,
     CreateDataStoreModel,
     CreateStoreItem,
     MainCreateDataStoreModel,
 )
+
+from geoserverx.models.layers import LayersModel, LayerModel
 from geoserverx.models.coverages_store import CoveragesStoreModel, CoveragesStoresModel
 
 from geoserverx.models.gs_response import GSResponse, HttpxError
 from geoserverx.utils.services.datastore import (
     AddDataStoreProtocol,
     CreateFileStore,
     ShapefileStore,
@@ -85,14 +87,16 @@
             resp = GSResponseEnum._404.value
         elif r == 403:
             resp = GSResponseEnum._403.value
         elif r == 201:
             resp = GSResponseEnum._201.value
         elif r == 409:
             resp = GSResponseEnum._409.value
+        elif r == 200:
+            resp = GSResponseEnum._200.value
         return GSResponse.parse_obj(resp)
 
     def exception_handler(func):
         def inner_function(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except httpx.ConnectError as exc:
@@ -257,7 +261,42 @@
         responses = Client.post(
             f"workspaces/{workspace}/datastores/",
             data=payload.json(),
             headers=self.head,
         )
         results = self.response_recognise(responses.status_code)
         return results
+
+    # Get all layers
+    @exception_handler
+    def get_all_layers(
+        self, workspace: Optional[str] = None
+    ) -> Union[LayersModel, GSResponse]:
+        Client = self.http_client
+        if workspace:
+            responses = Client.get(f"/workspaces/{workspace}/layers")
+        else:
+            responses = Client.get(f"layers")
+        if responses.status_code == 200:
+            return LayersModel.parse_obj(responses.json())
+        else:
+            results = self.response_recognise(responses.status_code)
+            return results
+
+    # Get specific layer
+    @exception_handler
+    def get_layer(self, workspace: str, layer: str) -> Union[LayerModel, GSResponse]:
+        Client = self.http_client
+        responses = Client.get(f"layers/{workspace}:{layer}")
+        if responses.status_code == 200:
+            return LayerModel.parse_obj(responses.json())
+        else:
+            results = self.response_recognise(responses.status_code)
+            return results
+
+    # Delete specific layer
+    @exception_handler
+    def delete_layer(self, workspace: str, layer: str) -> GSResponse:
+        Client = self.http_client
+        responses = Client.delete(f"layers/{workspace}:{layer}")
+        results = self.response_recognise(responses.status_code)
+        return results
```

### Comparing `geoserverx-0.0.1/src/geoserverx/cli/cli.py` & `geoserverx-0.0.2/src/geoserverx/cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -334,7 +334,60 @@
         )
         if result.code == 201:
             typer.secho(result, fg=typer.colors.GREEN)
         else:
             typer.secho(result, fg=typer.colors.RED)
     else:
         typer.echo("Async support will be shortly")
+
+
+# get all layers
+@SyncGeoServerX.exception_handler
+@app.command(help="Get all layers in the Geoserver")
+def layers(
+    request: requestEnum = requestEnum._sync,
+    url: str = typer.Option(
+        "http://127.0.0.1:8080/geoserver/rest/", help="Geoserver REST URL"
+    ),
+    workspace: str = typer.Option(None, help="Workspace name"),
+    password: str = typer.Option("geoserver", help="Geoserver Password"),
+    username: str = typer.Option("admin", help="Geoserver username"),
+):
+    """
+    Get all layers in the Geoserver
+    """
+    if request.value == "sync":
+        client = SyncGeoServerX(username, password, url)
+        result = client.get_all_layers(workspace).json()
+        if "code" in result:
+            typer.secho(result, fg=typer.colors.RED)
+        else:
+            print(result)
+    else:
+        typer.echo("Async support will be shortly")
+
+
+# get layer
+@SyncGeoServerX.exception_handler
+@app.command(help="Get layer in the Geoserver")
+def layer(
+    request: requestEnum = requestEnum._sync,
+    workspace: str = typer.Option(..., help="Workspace name"),
+    layer: str = typer.Option(..., help="Layer name"),
+    url: str = typer.Option(
+        "http://127.0.0.1:8080/geoserver/rest/", help="Geoserver REST URL"
+    ),
+    password: str = typer.Option("geoserver", help="Geoserver Password"),
+    username: str = typer.Option("admin", help="Geoserver username"),
+):
+    """
+    Get workspace in the Geoserver
+    """
+    if request.value == "sync":
+        client = SyncGeoServerX(username, password, url)
+        result = client.get_layer(workspace, layer).json()
+        if "code" in result:
+            typer.secho(result, fg=typer.colors.RED)
+        else:
+            print(result)
+    else:
+        typer.echo("Async support will be shortly")
```

### Comparing `geoserverx-0.0.1/src/geoserverx/models/coverages_store.py` & `geoserverx-0.0.2/src/geoserverx/models/coverages_store.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/src/geoserverx/models/data_store.py` & `geoserverx-0.0.2/src/geoserverx/models/data_store.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/src/geoserverx/models/workspace.py` & `geoserverx-0.0.2/src/geoserverx/models/workspace.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/src/geoserverx/utils/auth.py` & `geoserverx-0.0.2/src/geoserverx/utils/auth.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/src/geoserverx/utils/services/async_datastore.py` & `geoserverx-0.0.2/src/geoserverx/utils/services/async_datastore.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/src/geoserverx/utils/services/datastore.py` & `geoserverx-0.0.2/src/geoserverx/utils/services/datastore.py`

 * *Files identical despite different names*

### Comparing `geoserverx-0.0.1/PKG-INFO` & `geoserverx-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoserverx
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: krishnaglodha
 Author-email: krishnaglodha@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

