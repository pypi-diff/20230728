# Comparing `tmp/latitude_cli-0.0.1.tar.gz` & `tmp/latitude_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latitude_cli-0.0.1.tar", max compression
+gzip compressed data, was "latitude_cli-0.0.5.tar", max compression
```

## Comparing `latitude_cli-0.0.1.tar` & `latitude_cli-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      771 2023-07-24 20:54:29.020966 latitude_cli-0.0.1/README.md
--rw-r--r--   0        0        0      854 2023-07-24 20:54:29.020966 latitude_cli-0.0.1/latitude_cli/cli.py
--rw-r--r--   0        0        0     1377 2023-07-24 20:54:29.020966 latitude_cli-0.0.1/latitude_cli/libs/version.py
--rw-r--r--   0        0        0      757 2023-07-24 20:54:29.020966 latitude_cli-0.0.1/latitude_cli/modules/serverless.py
--rw-r--r--   0        0        0      659 2023-07-24 20:54:29.020966 latitude_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 latitude_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      771 2023-07-28 13:41:22.475726 latitude_cli-0.0.5/README.md
+-rw-r--r--   0        0        0      797 2023-07-28 13:41:22.475726 latitude_cli-0.0.5/latitude_cli/cli.py
+-rw-r--r--   0        0        0     1377 2023-07-28 13:41:22.475726 latitude_cli-0.0.5/latitude_cli/libs/version.py
+-rw-r--r--   0        0        0      757 2023-07-28 13:41:22.475726 latitude_cli-0.0.5/latitude_cli/modules/serverless.py
+-rw-r--r--   0        0        0      659 2023-07-28 13:41:22.475726 latitude_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 latitude_cli-0.0.5/PKG-INFO
```

### Comparing `latitude_cli-0.0.1/README.md` & `latitude_cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `latitude_cli-0.0.1/latitude_cli/cli.py` & `latitude_cli-0.0.5/latitude_cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 import latitude_cli.modules.serverless
 import typer
-from latitude_cli.libs.version import getLatestPyPiVersion
 from latitude_cli.libs.version import getVerison
 
 
 app = typer.Typer()
 app.add_typer(
     latitude_cli.modules.serverless,
     name="sls",
@@ -34,9 +33,9 @@
 
 ) -> None:
     return
 
 
 def run() -> None:
     """Run commands."""
-    getLatestPyPiVersion()
+    # getLatestPyPiVersion()
     app()
```

### Comparing `latitude_cli-0.0.1/latitude_cli/libs/version.py` & `latitude_cli-0.0.5/latitude_cli/libs/version.py`

 * *Files identical despite different names*

### Comparing `latitude_cli-0.0.1/latitude_cli/modules/serverless.py` & `latitude_cli-0.0.5/latitude_cli/modules/serverless.py`

 * *Files identical despite different names*

### Comparing `latitude_cli-0.0.1/pyproject.toml` & `latitude_cli-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latitude-cli"
-version = "0.0.1"
+version = "0.0.5"
 description = "CLI for managing some general dev tasks"
 readme = "README.md"
 documentation = ""
 repository = "https://github.com/hloughrey/latitude-cli"
 authors = ["Hugh Loughrey <hugh.loughrey@gmail.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `latitude_cli-0.0.1/PKG-INFO` & `latitude_cli-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latitude-cli
-Version: 0.0.1
+Version: 0.0.5
 Summary: CLI for managing some general dev tasks
 Home-page: https://github.com/hloughrey/latitude-cli
 Author: Hugh Loughrey
 Author-email: hugh.loughrey@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

