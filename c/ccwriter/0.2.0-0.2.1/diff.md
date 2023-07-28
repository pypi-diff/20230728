# Comparing `tmp/ccwriter-0.2.0.tar.gz` & `tmp/ccwriter-0.2.1.tar.gz`

## Comparing `ccwriter-0.2.0.tar` & `ccwriter-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.python-version
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.0/requirements.lock
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ccwriter-0.2.0/src/ccwriter/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ccwriter-0.2.0/README.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 ccwriter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 ccwriter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.python-version
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.1/requirements.lock
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ccwriter-0.2.1/src/ccwriter/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ccwriter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ccwriter-0.2.1/README.md
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ccwriter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 ccwriter-0.2.1/PKG-INFO
```

### Comparing `ccwriter-0.2.0/.github/workflows/workflow.yaml` & `ccwriter-0.2.1/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.0/src/ccwriter/__init__.py` & `ccwriter-0.2.1/src/ccwriter/__init__.py`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.0/README.md` & `ccwriter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.0/pyproject.toml` & `ccwriter-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [project]
 name = "ccwriter"
-version = "0.2.0"
+version = "0.2.1"
 description = "Writer for CloudCompare .bin format"
 authors = [
     { name = "Marko Bausch", email = "60338487+mrkbac@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.22",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
+license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
 ]
 
+[project.urls]
+repository = "https://github.com/mkrbac/ccwriter"
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
```

### Comparing `ccwriter-0.2.0/PKG-INFO` & `ccwriter-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: ccwriter
-Version: 0.2.0
+Version: 0.2.1
 Summary: Writer for CloudCompare .bin format
+Project-URL: repository, https://github.com/mkrbac/ccwriter
 Author-email: Marko Bausch <60338487+mrkbac@users.noreply.github.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: numpy>=1.22
```

