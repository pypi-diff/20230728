# Comparing `tmp/nbautoexport-0.5.1.tar.gz` & `tmp/nbautoexport-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbautoexport-0.5.1.tar", last modified: Tue Jul 18 18:17:44 2023, max compression
+gzip compressed data, was "nbautoexport-0.5.2.tar", last modified: Fri Jul 28 21:10:17 2023, max compression
```

## Comparing `nbautoexport-0.5.1.tar` & `nbautoexport-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1055 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/LICENSE
--rw-r--r--   0        0        0     7080 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/README.md
--rw-r--r--   0        0        0      159 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/__init__.py
--rw-r--r--   0        0        0       83 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/__main__.py
--rw-r--r--   0        0        0     4602 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/clean.py
--rw-r--r--   0        0        0     5219 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/export.py
--rw-r--r--   0        0        0     4837 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/jupyter_config.py
--rw-r--r--   0        0        0    13661 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/nbautoexport.py
--rw-r--r--   0        0        0     2249 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/sentinel.py
--rw-r--r--   0        0        0     3583 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/nbautoexport/utils.py
--rw-r--r--   0        0        0     2097 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       42 2023-07-18 18:17:02.665674 nbautoexport-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0    18553 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/assets/the_notebook.ipynb
--rw-r--r--   0        0        0      731 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     1404 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_clean.py
--rw-r--r--   0        0        0     2953 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli.py
--rw-r--r--   0        0        0     9795 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_clean.py
--rw-r--r--   0        0        0     5248 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_configure.py
--rw-r--r--   0        0        0     9757 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_export.py
--rw-r--r--   0        0        0     2191 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_cli_install.py
--rw-r--r--   0        0        0     5633 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_export.py
--rw-r--r--   0        0        0    11730 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_jupyter_config.py
--rw-r--r--   0        0        0     4809 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_post_save.py
--rw-r--r--   0        0        0      836 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_sentinel.py
--rw-r--r--   0        0        0     4299 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/test_utils.py
--rw-r--r--   0        0        0      628 2023-07-18 18:17:02.669674 nbautoexport-0.5.1/tests/utils.py
--rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 nbautoexport-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-28 21:09:26.843706 nbautoexport-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7080 2023-07-28 21:09:26.843706 nbautoexport-0.5.2/README.md
+-rw-r--r--   0        0        0      159 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/__main__.py
+-rw-r--r--   0        0        0     4602 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/clean.py
+-rw-r--r--   0        0        0     5225 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/export.py
+-rw-r--r--   0        0        0     4837 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/jupyter_config.py
+-rw-r--r--   0        0        0    13661 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/nbautoexport.py
+-rw-r--r--   0        0        0     2249 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/sentinel.py
+-rw-r--r--   0        0        0     3583 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/nbautoexport/utils.py
+-rw-r--r--   0        0        0     2097 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0    18553 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/assets/the_notebook.ipynb
+-rw-r--r--   0        0        0      731 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     1404 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_clean.py
+-rw-r--r--   0        0        0     2953 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_cli.py
+-rw-r--r--   0        0        0     9795 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_cli_clean.py
+-rw-r--r--   0        0        0     5248 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_cli_configure.py
+-rw-r--r--   0        0        0     9757 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_cli_export.py
+-rw-r--r--   0        0        0     2191 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_cli_install.py
+-rw-r--r--   0        0        0     5633 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_export.py
+-rw-r--r--   0        0        0    11736 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_jupyter_config.py
+-rw-r--r--   0        0        0     4815 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_post_save.py
+-rw-r--r--   0        0        0      836 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_sentinel.py
+-rw-r--r--   0        0        0     4299 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/test_utils.py
+-rw-r--r--   0        0        0      628 2023-07-28 21:09:26.847707 nbautoexport-0.5.2/tests/utils.py
+-rw-r--r--   0        0        0     8293 1970-01-01 00:00:00.000000 nbautoexport-0.5.2/PKG-INFO
```

### Comparing `nbautoexport-0.5.1/LICENSE` & `nbautoexport-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/README.md` & `nbautoexport-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/nbautoexport/clean.py` & `nbautoexport-0.5.2/nbautoexport/clean.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/nbautoexport/export.py` & `nbautoexport-0.5.2/nbautoexport/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import re
 
 from nbconvert.nbconvertapp import NbConvertApp
 from nbconvert.postprocessors.base import PostProcessorBase
-from notebook.services.contents.filemanager import FileContentsManager
+from jupyter_server.services.contents.filemanager import FileContentsManager
 
 from nbautoexport.clean import FORMATS_WITH_IMAGE_DIR
 from nbautoexport.sentinel import (
     ExportFormat,
     NbAutoexportConfig,
     SAVE_PROGRESS_INDICATOR_FILE,
 )
```

### Comparing `nbautoexport-0.5.1/nbautoexport/jupyter_config.py` & `nbautoexport-0.5.2/nbautoexport/jupyter_config.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/nbautoexport/nbautoexport.py` & `nbautoexport-0.5.2/nbautoexport/nbautoexport.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/nbautoexport/sentinel.py` & `nbautoexport-0.5.2/nbautoexport/sentinel.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/nbautoexport/utils.py` & `nbautoexport-0.5.2/nbautoexport/utils.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/pyproject.toml` & `nbautoexport-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "nbformat",
     "notebook",
     "packaging",
     "pydantic",
     "traitlets",
     "typer>=0.3.0",
 ]
-version = "0.5.1"
+version = "0.5.2"
 
 [project.scripts]
 nbautoexport = "nbautoexport.nbautoexport:app"
 
 [project.urls]
 Homepage = "https://github.com/drivendataorg/nbautoexport"
 Repository = "https://github.com/drivendataorg/nbautoexport"
```

### Comparing `nbautoexport-0.5.1/tests/assets/the_notebook.ipynb` & `nbautoexport-0.5.2/tests/assets/the_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/conftest.py` & `nbautoexport-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_clean.py` & `nbautoexport-0.5.2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_cli.py` & `nbautoexport-0.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_cli_clean.py` & `nbautoexport-0.5.2/tests/test_cli_clean.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_cli_configure.py` & `nbautoexport-0.5.2/tests/test_cli_configure.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_cli_export.py` & `nbautoexport-0.5.2/tests/test_cli_export.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_cli_install.py` & `nbautoexport-0.5.2/tests/test_cli_install.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_export.py` & `nbautoexport-0.5.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_jupyter_config.py` & `nbautoexport-0.5.2/tests/test_jupyter_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import builtins
 import logging
 from pkg_resources import parse_version
 from pkg_resources.extern.packaging.version import Version
 import sys
 import textwrap
 
-from notebook.services.contents.filemanager import FileContentsManager
+from jupyter_server.services.contents.filemanager import FileContentsManager
 from traitlets.config.loader import Config
 
 from nbautoexport import __version__
 import nbautoexport as nbautoexport_root
 from nbautoexport import export, jupyter_config
 from tests.utils import caplog_contains
```

### Comparing `nbautoexport-0.5.1/tests/test_post_save.py` & `nbautoexport-0.5.2/tests/test_post_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import shutil
 
 import nbformat
-from notebook.services.contents.filemanager import FileContentsManager
+from jupyter_server.services.contents.filemanager import FileContentsManager
 import pytest
 from traitlets.config import Config
 
 from nbautoexport.jupyter_config import initialize_post_save_hook
 from nbautoexport.sentinel import (
     ExportFormat,
     NbAutoexportConfig,
```

### Comparing `nbautoexport-0.5.1/tests/test_sentinel.py` & `nbautoexport-0.5.2/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/test_utils.py` & `nbautoexport-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/tests/utils.py` & `nbautoexport-0.5.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nbautoexport-0.5.1/PKG-INFO` & `nbautoexport-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbautoexport
-Version: 0.5.1
+Version: 0.5.2
 Summary: Automatically export Jupyter notebooks to various file formats (.py, .html, and more) on save.
 License: MIT
 Keywords: nbautoexport,jupyter,nbconvert
 Author-email: DrivenData <info@drivendata.org>
 Requires-Python: >=3.7
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
```

