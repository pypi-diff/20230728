# Comparing `tmp/kodexa-6.3.35668071917.tar.gz` & `tmp/kodexa-6.3.35690079772.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35668071917.tar", max compression
+gzip compressed data, was "kodexa-6.3.35690079772.tar", max compression
```

## Comparing `kodexa-6.3.35668071917.tar` & `kodexa-6.3.35690079772.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-07-26 11:16:16.245479 kodexa-6.3.35668071917/LICENSE
--rw-r--r--   0        0        0     2804 2023-07-26 11:16:16.245479 kodexa-6.3.35668071917/README.md
--rw-r--r--   0        0        0      847 2023-07-26 11:16:16.249479 kodexa-6.3.35668071917/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-07-26 11:16:16.249479 kodexa-6.3.35668071917/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/model/model.py
--rw-r--r--   0        0        0   118200 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/model/objects.py
--rw-r--r--   0        0        0    38816 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111395 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/platform/client.py
--rw-r--r--   0        0        0    28288 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 11:16:16.253479 kodexa-6.3.35668071917/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-07-26 11:16:29.757362 kodexa-6.3.35668071917/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35668071917/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 08:49:53.181417 kodexa-6.3.35690079772/LICENSE
+-rw-r--r--   0        0        0     2804 2023-07-28 08:49:53.181417 kodexa-6.3.35690079772/README.md
+-rw-r--r--   0        0        0      847 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/model/model.py
+-rw-r--r--   0        0        0   118280 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38816 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111395 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28288 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:49:53.189417 kodexa-6.3.35690079772/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-07-28 08:50:29.233533 kodexa-6.3.35690079772/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35690079772/PKG-INFO
```

### Comparing `kodexa-6.3.35668071917/LICENSE` & `kodexa-6.3.35690079772/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/README.md` & `kodexa-6.3.35690079772/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/__init__.py` & `kodexa-6.3.35690079772/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/assistant/assistant.py` & `kodexa-6.3.35690079772/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/connectors/connectors.py` & `kodexa-6.3.35690079772/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/model/__init__.py` & `kodexa-6.3.35690079772/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/model/base.py` & `kodexa-6.3.35690079772/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/model/model.py` & `kodexa-6.3.35690079772/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/model/objects.py` & `kodexa-6.3.35690079772/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
     slug: Optional[str] = None
     name: Optional[str] = None
     description: Optional[str] = None
     widgets: Optional[List[DashboardWidget]] = None
     template_ref: Optional[str] = Field(None, alias='templateRef')
     ref: Optional[str] = None
-
+    single_widget: Optional[DashboardWidget] = Field(None, alias='singleWidget')
 
 class StoreType(Enum):
     document = 'DOCUMENT'
     table = 'TABLE'
     dictionary = 'DICTIONARY'
     model = 'MODEL'
```

### Comparing `kodexa-6.3.35668071917/kodexa/model/persistence.py` & `kodexa-6.3.35690079772/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35690079772/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/platform/client.py` & `kodexa-6.3.35690079772/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/platform/kodexa.py` & `kodexa-6.3.35690079772/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/ast.py` & `kodexa-6.3.35690079772/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/core.py` & `kodexa-6.3.35690079772/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/lexrules.py` & `kodexa-6.3.35690079772/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/lextab.py` & `kodexa-6.3.35690079772/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/parserules.py` & `kodexa-6.3.35690079772/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/selectors/parsetab.py` & `kodexa-6.3.35690079772/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/spatial/azure_models.py` & `kodexa-6.3.35690079772/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35690079772/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35690079772/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/steps/common.py` & `kodexa-6.3.35690079772/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/testing/test_components.py` & `kodexa-6.3.35690079772/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/kodexa/testing/test_utils.py` & `kodexa-6.3.35690079772/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35668071917/pyproject.toml` & `kodexa-6.3.35690079772/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35668071917"
+version = "6.3.35690079772"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35668071917/PKG-INFO` & `kodexa-6.3.35690079772/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35668071917
+Version: 6.3.35690079772
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

