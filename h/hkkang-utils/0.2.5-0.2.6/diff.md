# Comparing `tmp/hkkang_utils-0.2.5.tar.gz` & `tmp/hkkang_utils-0.2.6.tar.gz`

## Comparing `hkkang_utils-0.2.5.tar` & `hkkang_utils-0.2.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/docs/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/docs/source/conf.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/docs/source/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_string.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_testing.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_tensor/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_tensor/test_tensor.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/tests/test_tensor/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/README.md
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hkkang_utils-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_string.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_testing.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_tensor/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_tensor/test_tensor.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/tests/test_tensor/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hkkang_utils-0.2.6/PKG-INFO
```

### Comparing `hkkang_utils-0.2.5/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.2.6/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/.github/workflows/unittest.yml` & `hkkang_utils-0.2.6/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/docs/Makefile` & `hkkang_utils-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/docs/make.bat` & `hkkang_utils-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/docs/source/conf.py` & `hkkang_utils-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/__init__.py` & `hkkang_utils-0.2.6/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.2.6/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/file.py` & `hkkang_utils-0.2.6/src/hkkang_utils/file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/list.py` & `hkkang_utils-0.2.6/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/metrics.py` & `hkkang_utils-0.2.6/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/misc.py` & `hkkang_utils-0.2.6/src/hkkang_utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import os
+import sys
 from typing import Any, Callable, Dict, Iterable, List
 
 import dotenv
 
 
 def infinite_iterator(iterator: Iterable) -> Any:
     """Infinite iterator
@@ -76,7 +77,12 @@
     possible_paths = python_paths + [working_dir_path, caller_file_path]
 
     # Find and load dotenv
     for path in possible_paths:
         dotenv.load_dotenv(dotenv_path=os.path.join(path, ".env"))
         if "SLACK_ACCESS_TOKEN" in os.environ:
             break
+
+
+def is_debugger_active() -> bool:
+    """Return if the debugger is currently active"""
+    return hasattr(sys, "gettrace") and sys.gettrace() is not None
```

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/ml.py` & `hkkang_utils-0.2.6/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/pattern.py` & `hkkang_utils-0.2.6/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/pg.py` & `hkkang_utils-0.2.6/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/slack.py` & `hkkang_utils-0.2.6/src/hkkang_utils/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,17 @@
     :type success_msg: str, optional
     :param error_msg: Message to send when error raise with the given code block, defaults to None
     :type error_msg: str, optional
     :param token: slack access token, defaults to DEFAULT_ACCESS_TOKEN
     :type token: str, optional
     :rtype: None
     """
+    if misc_utils.is_debugger_active():
+        disable = True
+
     if disable:
         yield None
         return None
 
     slack_messenger = SlackMessenger(channel=channel, token=token)
     try:
         yield slack_messenger
```

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/sql.py` & `hkkang_utils-0.2.6/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/string.py` & `hkkang_utils-0.2.6/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/tensor.py` & `hkkang_utils-0.2.6/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/src/hkkang_utils/time.py` & `hkkang_utils-0.2.6/src/hkkang_utils/time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_concurrent.py` & `hkkang_utils-0.2.6/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_file.py` & `hkkang_utils-0.2.6/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_io.py` & `hkkang_utils-0.2.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_list.py` & `hkkang_utils-0.2.6/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_metrics.py` & `hkkang_utils-0.2.6/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_misc.py` & `hkkang_utils-0.2.6/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_pattern.py` & `hkkang_utils-0.2.6/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_string.py` & `hkkang_utils-0.2.6/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_testing.py` & `hkkang_utils-0.2.6/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_time.py` & `hkkang_utils-0.2.6/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_tensor/test_tensor.py` & `hkkang_utils-0.2.6/tests/test_tensor/test_tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/tests/test_tensor/utils.py` & `hkkang_utils-0.2.6/tests/test_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/.gitignore` & `hkkang_utils-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/LICENSE` & `hkkang_utils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.2.5/pyproject.toml` & `hkkang_utils-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.2.5"
+version = "0.2.6"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.2.5/PKG-INFO` & `hkkang_utils-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.2.5
+Version: 0.2.6
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

