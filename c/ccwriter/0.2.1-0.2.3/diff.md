# Comparing `tmp/ccwriter-0.2.1.tar.gz` & `tmp/ccwriter-0.2.3.tar.gz`

## Comparing `ccwriter-0.2.1.tar` & `ccwriter-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.python-version
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.1/requirements.lock
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ccwriter-0.2.1/src/ccwriter/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.2.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ccwriter-0.2.1/LICENSE
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ccwriter-0.2.1/README.md
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 ccwriter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 ccwriter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccwriter-0.2.3/.python-version
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.3/requirements-dev.lock
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ccwriter-0.2.3/requirements.lock
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ccwriter-0.2.3/.github/workflows/bump.yaml
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ccwriter-0.2.3/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ccwriter-0.2.3/src/ccwriter/__about__.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ccwriter-0.2.3/src/ccwriter/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ccwriter-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 ccwriter-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 ccwriter-0.2.3/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 ccwriter-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 ccwriter-0.2.3/PKG-INFO
```

### Comparing `ccwriter-0.2.1/.github/workflows/workflow.yaml` & `ccwriter-0.2.3/.github/workflows/workflow.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -8,29 +8,31 @@
         description: 'Jobs'
         required: true
         default: 'lint'
         type: choice
         options:
           - lint
           - build
+  release:
+    types: [published]
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - uses: chartboost/ruff-action@v1
 
   build:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v') || inputs.job == 'build'
+    if: github.event_name == 'release' || github.event.inputs.job == 'build'
     needs: lint
 
     runs-on: ubuntu-latest
-    # Specifying a GitHub environment is optional, but strongly encouraged
+
     environment: release
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
       contents: read
 
     steps:
```

### Comparing `ccwriter-0.2.1/src/ccwriter/__init__.py` & `ccwriter-0.2.3/src/ccwriter/__init__.py`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.1/LICENSE` & `ccwriter-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.1/README.md` & `ccwriter-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ccwriter-0.2.1/pyproject.toml` & `ccwriter-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "ccwriter"
-version = "0.2.1"
 description = "Writer for CloudCompare .bin format"
 authors = [
     { name = "Marko Bausch", email = "60338487+mrkbac@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.22",
 ]
@@ -19,27 +18,32 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 
+dynamic = ["version"]
+
 [project.urls]
-repository = "https://github.com/mkrbac/ccwriter"
+Source = "https://github.com/mkrbac/ccwriter"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "autopep8>=2.0.2",
 ]
 
+[tool.hatch.version]
+path = "src/ccwriter/__about__.py"
+
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.autopep8]
 aggressive = 3
 recursive = true
 max_line_length = 100
```

### Comparing `ccwriter-0.2.1/PKG-INFO` & `ccwriter-0.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ccwriter
-Version: 0.2.1
+Version: 0.2.3
 Summary: Writer for CloudCompare .bin format
-Project-URL: repository, https://github.com/mkrbac/ccwriter
+Project-URL: Source, https://github.com/mkrbac/ccwriter
 Author-email: Marko Bausch <60338487+mrkbac@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

