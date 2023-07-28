# Comparing `tmp/pytest-analyzer-1.0.7.tar.gz` & `tmp/pytest-analyzer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-analyzer-1.0.7.tar", last modified: Fri Jul 28 17:10:19 2023, max compression
+gzip compressed data, was "pytest-analyzer-1.0.8.tar", last modified: Fri Jul 28 17:21:25 2023, max compression
```

## Comparing `pytest-analyzer-1.0.7.tar` & `pytest-analyzer-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:10:19.958346 pytest-analyzer-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-04 18:48:32.000000 pytest-analyzer-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3528 2023-07-28 17:10:19.958346 pytest-analyzer-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2848 2023-07-28 14:05:19.000000 pytest-analyzer-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 17:10:19.946060 pytest-analyzer-1.0.7/analyzer/
--rw-rw-rw-   0        0        0        0 2023-07-28 12:45:20.000000 pytest-analyzer-1.0.7/analyzer/__init__.py
--rw-rw-rw-   0        0        0     6868 2023-07-28 17:08:49.000000 pytest-analyzer-1.0.7/analyzer/analyzer.py
--rw-rw-rw-   0        0        0      702 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.7/analyzer/code_collector.py
--rw-rw-rw-   0        0        0     5536 2023-07-28 13:59:23.000000 pytest-analyzer-1.0.7/analyzer/connector.py
--rw-rw-rw-   0        0        0     3149 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.7/analyzer/decorator_updater.py
--rw-rw-rw-   0        0        0     1750 2023-07-28 09:36:45.000000 pytest-analyzer-1.0.7/analyzer/testItem.py
--rw-rw-rw-   0        0        0      731 2023-07-28 10:25:11.000000 pytest-analyzer-1.0.7/analyzer/testRunConfig.py
--rw-rw-rw-   0        0        0     1360 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.7/analyzer/testomat_item.py
--rw-rw-rw-   0        0        0      869 2023-07-28 17:09:32.000000 pytest-analyzer-1.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-28 17:10:19.953831 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/
--rw-rw-rw-   0        0        0     3528 2023-07-28 17:10:19.000000 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-07-28 17:10:19.000000 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:10:19.000000 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-28 17:10:19.000000 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 17:10:19.000000 pytest-analyzer-1.0.7/pytest_analyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:10:19.959343 pytest-analyzer-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 17:10:19.956338 pytest-analyzer-1.0.7/tests/
--rw-rw-rw-   0        0        0      320 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.7/tests/test_class_root.py
--rw-rw-rw-   0        0        0      546 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.7/tests/test_root.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-04 18:48:32.000000 pytest-analyzer-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3528 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2848 2023-07-28 14:05:19.000000 pytest-analyzer-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.331925 pytest-analyzer-1.0.8/analyzer/
+-rw-rw-rw-   0        0        0        0 2023-07-28 12:45:20.000000 pytest-analyzer-1.0.8/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     6868 2023-07-28 17:08:49.000000 pytest-analyzer-1.0.8/analyzer/analyzer.py
+-rw-rw-rw-   0        0        0      702 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/code_collector.py
+-rw-rw-rw-   0        0        0     5536 2023-07-28 13:59:23.000000 pytest-analyzer-1.0.8/analyzer/connector.py
+-rw-rw-rw-   0        0        0     3149 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/decorator_updater.py
+-rw-rw-rw-   0        0        0     1750 2023-07-28 09:36:45.000000 pytest-analyzer-1.0.8/analyzer/testItem.py
+-rw-rw-rw-   0        0        0      731 2023-07-28 10:25:11.000000 pytest-analyzer-1.0.8/analyzer/testRunConfig.py
+-rw-rw-rw-   0        0        0     1360 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/testomat_item.py
+-rw-rw-rw-   0        0        0      957 2023-07-28 17:19:40.000000 pytest-analyzer-1.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.335924 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/
+-rw-rw-rw-   0        0        0     3528 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.337924 pytest-analyzer-1.0.8/tests/
+-rw-rw-rw-   0        0        0      320 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.8/tests/test_class_root.py
+-rw-rw-rw-   0        0        0      546 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.8/tests/test_root.py
```

### Comparing `pytest-analyzer-1.0.7/LICENSE` & `pytest-analyzer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/PKG-INFO` & `pytest-analyzer-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-analyzer
-Version: 1.0.7
+Version: 1.0.8
 Summary: this plugin allows to analyze tests in pytest project, collect test metadata and sync it with testomat.io TCM system
 Author: Oleksii Ostapov
 Project-URL: Author's Blog, https://qamania.org
 Project-URL: Homepage, https://github.com/Ypurek/pytest-analyzer
 Project-URL: Bug Tracker, https://github.com/Ypurek/pytest-analyzer/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytest-analyzer-1.0.7/README.md` & `pytest-analyzer-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/analyzer.py` & `pytest-analyzer-1.0.8/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/code_collector.py` & `pytest-analyzer-1.0.8/analyzer/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/connector.py` & `pytest-analyzer-1.0.8/analyzer/connector.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/decorator_updater.py` & `pytest-analyzer-1.0.8/analyzer/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/testItem.py` & `pytest-analyzer-1.0.8/analyzer/testItem.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/testRunConfig.py` & `pytest-analyzer-1.0.8/analyzer/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/analyzer/testomat_item.py` & `pytest-analyzer-1.0.8/analyzer/testomat_item.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.7/pyproject.toml` & `pytest-analyzer-1.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [build-system]
 requires = ["setuptools>=65.5.1", "requests>=2.29.0", "autopep8>=2.0.2", "pytest>=7.3.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-analyzer"
-version = "1.0.7"
+version = "1.0.8"
+
+dependencies = [
+  "requests>=2.29.0",
+  "autopep8>=2.0.2",
+  "pytest>=7.3.1",]
+
 authors = [
   { name="Oleksii Ostapov" },
 ]
 description = "this plugin allows to analyze tests in pytest project, collect test metadata and sync it with testomat.io TCM system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pytest-analyzer-1.0.7/pytest_analyzer.egg-info/PKG-INFO` & `pytest-analyzer-1.0.8/pytest_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-analyzer
-Version: 1.0.7
+Version: 1.0.8
 Summary: this plugin allows to analyze tests in pytest project, collect test metadata and sync it with testomat.io TCM system
 Author: Oleksii Ostapov
 Project-URL: Author's Blog, https://qamania.org
 Project-URL: Homepage, https://github.com/Ypurek/pytest-analyzer
 Project-URL: Bug Tracker, https://github.com/Ypurek/pytest-analyzer/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytest-analyzer-1.0.7/tests/test_root.py` & `pytest-analyzer-1.0.8/tests/test_root.py`

 * *Files identical despite different names*

