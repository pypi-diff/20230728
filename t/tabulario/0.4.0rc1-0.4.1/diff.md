# Comparing `tmp/tabulario-0.4.0rc1.tar.gz` & `tmp/tabulario-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulario-0.4.0rc1.tar", max compression
+gzip compressed data, was "tabulario-0.4.1.tar", max compression
```

## Comparing `tabulario-0.4.0rc1.tar` & `tabulario-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0     7126 2023-06-26 14:48:22.117095 tabulario-0.4.0rc1/README.md
--rw-r--r--   0        0        0     2493 2023-06-26 14:48:35.917175 tabulario-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0      785 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/__init__.py
--rw-r--r--   0        0        0     4229 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/cli.py
--rw-r--r--   0        0        0      871 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/exceptions.py
--rw-r--r--   0        0        0     5018 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/oauth.py
--rw-r--r--   0        0        0     1004 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tab/util.py
--rw-r--r--   0        0        0      836 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/__init__.py
--rw-r--r--   0        0        0     4955 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/loader.py
--rw-r--r--   0        0        0     2111 2023-06-26 14:48:22.121095 tabulario-0.4.0rc1/tabular/tabular.py
--rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 tabulario-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-28 11:47:25.370234 tabulario-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7126 2023-07-28 11:47:25.374234 tabulario-0.4.1/README.md
+-rw-r--r--   0        0        0     2487 2023-07-28 11:47:41.690230 tabulario-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      785 2023-07-28 11:47:25.374234 tabulario-0.4.1/tab/__init__.py
+-rw-r--r--   0        0        0     4229 2023-07-28 11:47:25.374234 tabulario-0.4.1/tab/cli.py
+-rw-r--r--   0        0        0      871 2023-07-28 11:47:25.374234 tabulario-0.4.1/tab/exceptions.py
+-rw-r--r--   0        0        0     5018 2023-07-28 11:47:25.374234 tabulario-0.4.1/tab/oauth.py
+-rw-r--r--   0        0        0     1004 2023-07-28 11:47:25.374234 tabulario-0.4.1/tab/util.py
+-rw-r--r--   0        0        0      836 2023-07-28 11:47:25.374234 tabulario-0.4.1/tabular/__init__.py
+-rw-r--r--   0        0        0     5145 2023-07-28 11:47:25.374234 tabulario-0.4.1/tabular/loader.py
+-rw-r--r--   0        0        0     2111 2023-07-28 11:47:25.374234 tabulario-0.4.1/tabular/tabular.py
+-rw-r--r--   0        0        0     7937 1970-01-01 00:00:00.000000 tabulario-0.4.1/PKG-INFO
```

### Comparing `tabulario-0.4.0rc1/LICENSE` & `tabulario-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/README.md` & `tabulario-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/pyproject.toml` & `tabulario-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "tabulario"
-version = "0.4.0rc1"
+version = "0.4.1"
 readme = "README.md"
 homepage = "https://tabular.io/"
 repository = "https://github.com/tabular-io/"
 description = "Utility library for Tabular.io"
 authors = ["Tabular Technologies, Inc. <fokko@tabular.io>"]
 license = "Apache License 2.0"
 
@@ -40,15 +40,15 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 click = "^8.1.3"
-pyiceberg = "0.4.0rc1"
+pyiceberg = "0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-checkdocs = "^2.9.0"
 pre-commit = "^2.0.0"
 coverage = { version = "^6.5.0", extras = ["toml"] }
 requests-mock = "^1.10.0"
```

### Comparing `tabulario-0.4.0rc1/tab/__init__.py` & `tabulario-0.4.1/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tab/cli.py` & `tabulario-0.4.1/tab/cli.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tab/exceptions.py` & `tabulario-0.4.1/tab/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tab/oauth.py` & `tabulario-0.4.1/tab/oauth.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tab/util.py` & `tabulario-0.4.1/tab/util.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tabular/__init__.py` & `tabulario-0.4.1/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/tabular/loader.py` & `tabulario-0.4.1/tabular/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Dict,
     Literal,
     Optional,
     Union,
 )
 
 from pyiceberg.catalog import Catalog, load_catalog
-from pyiceberg.catalog.rest import Endpoints
+from pyiceberg.catalog.rest import Endpoints, RestCatalog
 from pyiceberg.table import Identifier, Table
 from requests import HTTPError
 
 from tab.exceptions import InvalidInputError
 
 
 def enable_loading(
@@ -67,15 +67,15 @@
         f"{Endpoints.load_table}/loader",
         prefixed=True,
         **catalog._split_identifier_for_path(identifier),  # pylint: disable=[W0212]
     )
     # Remove the redirection for ice controller
     url = url.replace("/ice/", "/")
 
-    response = catalog.session.post(url, json=payload)
+    response = catalog._session.post(url, json=payload)  # pylint: disable=W0212
 
     try:
         response.raise_for_status()
     except HTTPError as exc:
         catalog._handle_non_200_response(exc, {})  # pylint: disable=[W0212]
 
 
@@ -101,25 +101,28 @@
     loader_path += "/" + os.path.basename(file)
     io = table.io
 
     with io.new_input(file).open() as fin, io.new_output(loader_path).create(overwrite=True) as fout:
         shutil.copyfileobj(fin, fout)
 
 
-def _resolve_catalog(identifier: Union[Identifier, str], catalog: Optional[Catalog] = None) -> Catalog:
+def _resolve_catalog(identifier: Union[Identifier, str], catalog: Optional[RestCatalog] = None) -> RestCatalog:
     identifier_tuple: Identifier = Catalog.identifier_to_tuple(identifier)
 
     # Check if the catalog was provided in the identifier
     if len(identifier_tuple) == 3:
         if catalog:
             if catalog.name != identifier_tuple[0]:
                 raise ValueError(f"Catalog identifier '{identifier_tuple[0]}' does not match catalog f'{catalog.name}'")
             return catalog
         else:
-            return load_catalog(identifier_tuple[0])
+            catalog = load_catalog(identifier_tuple[0])
+            if not isinstance(catalog, RestCatalog):
+                raise ValueError("Expected a REST catalog")
+            return catalog
 
     assert len(identifier_tuple) == 2, "Identifier must include database and table"
     return catalog or load_catalog("default")
 
 
 def _normalize_table_identifier(identifier: Union[Identifier, str]) -> Identifier:
     identifier_tuple: Identifier = Catalog.identifier_to_tuple(identifier)
```

### Comparing `tabulario-0.4.0rc1/tabular/tabular.py` & `tabulario-0.4.1/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.4.0rc1/PKG-INFO` & `tabulario-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tabulario
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: Utility library for Tabular.io
 Home-page: https://tabular.io/
 License: Apache-2.0
 Author: Tabular Technologies, Inc.
 Author-email: fokko@tabular.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: pyiceberg (==0.4.0rc1)
+Requires-Dist: pyiceberg (==0.4.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/tabular-io/
 Description-Content-Type: text/markdown
 
 # Tab
 
 This is a helper library to easily fetch and refresh access token from Tabular.
```

