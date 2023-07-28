# Comparing `tmp/tipg-0.3.0.tar.gz` & `tmp/tipg-0.3.1.tar.gz`

## Comparing `tipg-0.3.0.tar` & `tipg-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/__init__.py
--rw-r--r--   0        0        0    32496 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/collections.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/database.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/errors.py
--rw-r--r--   0        0        0    73592 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/logger.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/main.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/middleware.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/model.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/enums.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/resources/response.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/collection.html
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/collections.html
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/header.html
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/item.html
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/items.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/landing.html
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/map.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tileset.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.3.0/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.3.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.3.0/LICENSE
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.3.0/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tipg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 tipg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/__init__.py
+-rw-r--r--   0        0        0    32496 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/collections.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/database.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/errors.py
+-rw-r--r--   0        0        0    73823 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/logger.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/main.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/middleware.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/model.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/enums.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/response.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/collections.html
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/header.html
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/item.html
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/items.html
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/landing.html
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/map.html
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.3.1/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tipg-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 tipg-0.3.1/PKG-INFO
```

### Comparing `tipg-0.3.0/tipg/collections.py` & `tipg-0.3.1/tipg/collections.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/database.py` & `tipg-0.3.1/tipg/database.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/dependencies.py` & `tipg-0.3.1/tipg/dependencies.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/errors.py` & `tipg-0.3.1/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/factory.py` & `tipg-0.3.1/tipg/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from tipg import model
 from tipg.collections import Catalog, Collection
 from tipg.dependencies import (
     CatalogParams,
     CollectionParams,
     ItemsOutputType,
     OutputType,
+    QueryablesOutputType,
     TileParams,
     bbox_query,
     datetime_query,
     filter_query,
     function_parameters_query,
     ids_query,
     properties_filter_query,
@@ -702,15 +703,17 @@
                     }
                 },
             },
         )
         def queryables(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
-            output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
+            output_type: Annotated[
+                Optional[MediaType], Depends(QueryablesOutputType)
+            ] = None,
         ):
             """Queryables for a feature collection.
 
             ref: http://docs.ogc.org/DRAFTS/19-079r1.html#filter-queryables
             """
             qs = "?" + str(request.query_params) if request.query_params else ""
 
@@ -1356,15 +1359,22 @@
             return data
 
         @self.router.get(
             "/collections/{collectionId}/tiles",
             response_model=model.TileSetList,
             response_class=ORJSONResponse,
             response_model_exclude_none=True,
-            responses={200: {"content": {MediaType.json.value: {}}}},
+            responses={
+                200: {
+                    "content": {
+                        MediaType.json.value: {},
+                        MediaType.html.value: {},
+                    }
+                }
+            },
             summary="Retrieve a list of available vector tilesets for the specified collection.",
             operation_id=".collection.vector.getTileSetsList",
         )
         async def collection_tileset_list(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
```

### Comparing `tipg-0.3.0/tipg/main.py` & `tipg-0.3.1/tipg/main.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/middleware.py` & `tipg-0.3.1/tipg/middleware.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/model.py` & `tipg-0.3.1/tipg/model.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/settings.py` & `tipg-0.3.1/tipg/settings.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/filter/evaluate.py` & `tipg-0.3.1/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/filter/filters.py` & `tipg-0.3.1/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/resources/enums.py` & `tipg-0.3.1/tipg/resources/enums.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/resources/response.py` & `tipg-0.3.1/tipg/resources/response.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/sql/dbcatalog.sql` & `tipg-0.3.1/tipg/sql/dbcatalog.sql`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/collection.html` & `tipg-0.3.1/tipg/templates/collection.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/collections.html` & `tipg-0.3.1/tipg/templates/collections.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/conformance.html` & `tipg-0.3.1/tipg/templates/conformance.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/header.html` & `tipg-0.3.1/tipg/templates/header.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/item.html` & `tipg-0.3.1/tipg/templates/item.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/items.html` & `tipg-0.3.1/tipg/templates/items.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/landing.html` & `tipg-0.3.1/tipg/templates/landing.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/map.html` & `tipg-0.3.1/tipg/templates/map.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/queryables.html` & `tipg-0.3.1/tipg/templates/queryables.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/tilematrixset.html` & `tipg-0.3.1/tipg/templates/tilematrixset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/tilematrixsets.html` & `tipg-0.3.1/tipg/templates/tilematrixsets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/tileset.html` & `tipg-0.3.1/tipg/templates/tileset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/tipg/templates/tilesets.html` & `tipg-0.3.1/tipg/templates/tilesets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/.gitignore` & `tipg-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/LICENSE` & `tipg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/README.md` & `tipg-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/pyproject.toml` & `tipg-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tipg-0.3.0/PKG-INFO` & `tipg-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipg
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tipg Version: 0.3.0 Summary: Simple and Fast
+Metadata-Version: 2.1 Name: tipg Version: 0.3.1 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
```

