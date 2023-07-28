# Comparing `tmp/vpype_rerun-0.1.0.tar.gz` & `tmp/vpype_rerun-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpype_rerun-0.1.0.tar", max compression
+gzip compressed data, was "vpype_rerun-0.1.0a0.tar", max compression
```

## Comparing `vpype_rerun-0.1.0.tar` & `vpype_rerun-0.1.0a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-07-28 20:26:39.955464 vpype_rerun-0.1.0/LICENSE
--rw-r--r--   0        0        0     1182 2023-07-28 20:26:39.955464 vpype_rerun-0.1.0/README.md
--rw-r--r--   0        0        0      851 2023-07-28 20:26:39.959464 vpype_rerun-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 20:26:39.959464 vpype_rerun-0.1.0/vpype_rerun/__init__.py
--rw-r--r--   0        0        0      766 2023-07-28 20:26:39.959464 vpype_rerun-0.1.0/vpype_rerun/rerun.py
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 vpype_rerun-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-28 19:20:22.841254 vpype_rerun-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1225 2023-07-28 19:20:22.845750 vpype_rerun-0.1.0a0/README.md
+-rw-r--r--   0        0        0      853 2023-07-28 19:38:19.175001 vpype_rerun-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 19:20:22.849465 vpype_rerun-0.1.0a0/vpype_rerun/__init__.py
+-rw-r--r--   0        0        0      734 2023-07-28 19:42:22.278603 vpype_rerun-0.1.0a0/vpype_rerun/rerun.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 vpype_rerun-0.1.0a0/PKG-INFO
```

### Comparing `vpype_rerun-0.1.0/LICENSE` & `vpype_rerun-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `vpype_rerun-0.1.0/pyproject.toml` & `vpype_rerun-0.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vpype-rerun"
-version = "0.1.0"
+version = "0.1.0a0"
 description = "Rerun viewer integration for vpype"
 authors = ["Antoine Beyeler <abeyeler@ab-ware.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `vpype_rerun-0.1.0/vpype_rerun/rerun.py` & `vpype_rerun-0.1.0a0/vpype_rerun/rerun.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import random
-
 import vpype as vp
 import vpype_cli
 import rerun as rr
 
 
 @vpype_cli.cli.command(group="Plugins")
 @vpype_cli.global_processor
 def rerun(document: vp.Document) -> vp.Document:
     """Rerun test"""
 
-    rr.init(f"vpype_{random.random()}", spawn=True)
+    rr.init("my data", spawn=True)
 
     for lid, layer in document.layers.items():
         pen_width = layer.property("vp_pen_width") or document.property("vp_pen_width") or 1.0
         color = layer.property("vp_color") or document.property("vp_color") or vp.Color("blue")
 
         rr.log_line_strips_2d(
             f"{lid}_layer",
```

### Comparing `vpype_rerun-0.1.0/PKG-INFO` & `vpype_rerun-0.1.0a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpype-rerun
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Rerun viewer integration for vpype
 License: MIT
 Author: Antoine Beyeler
 Author-email: abeyeler@ab-ware.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
@@ -17,53 +17,77 @@
 Requires-Dist: click (>=8.1.6)
 Requires-Dist: rerun-sdk (>=0.8.0)
 Requires-Dist: vpype[all] (>=1.13)
 Description-Content-Type: text/markdown
 
 # vpype-rerun
 
-This plug-in integrates the [Rerun viewer](https://github.com/rerun-io/rerun) in [*vpype*](https://github.com/abey79/vpype).
+[`vpype`](https://github.com/abey79/vpype) plug-in to [_to be completed_]
 
-## Example
 
-```
-vpype random -n 500 -a 20cm 20cm rerun
-```
-
-<img width="1106" alt="image" src="https://github.com/abey79/vpype-rerun/assets/49431240/4bcadf27-3058-4c16-aaab-5ba5fe3e9252">
+## Examples
 
-
-## Why?
-
-This plug-in makes it easy to log large quantities of [2D line strips](https://www.rerun.io/docs/reference/data_types/linestrip2d) to the Rerun viewer, which is useful for stress-testing, etc.
+_to be completed_
 
 
 ## Installation
 
 See the [installation instructions](https://vpype.readthedocs.io/en/latest/install.html) for information on how
-to install `vpype` (TL;DR: `pipx install "vpype[all]"`).
+to install `vpype`.
 
 If *vpype* was installed using pipx, use the following command:
 
 ```bash
 $ pipx inject vpype vpype-rerun
 ```
 
 If *vpype* was installed using pip in a virtual environment, activate the virtual environment and use the following command:
 
 ```bash
 $ pip install vpype-rerun
 ```
 
+Check that your install is successful:
+
+```
+$ vpype rerun --help
+[...]
+```
+
 ## Documentation
 
 The complete plug-in documentation is available directly in the CLI help:
 
 ```bash
 $ vpype rerun --help
 ```
 
 
+## Development setup
+
+Here is how to clone the project for development:
+
+```bash
+$ git clone https://github.com/abey79/vpype-rerun.git
+$ cd vpype-rerun
+```
+
+Create a virtual environment:
+
+```bash
+$ python3 -m venv venv
+$ source venv/bin/activate
+$ pip install --upgrade pip
+```
+
+Install `vpype-rerun` and its dependencies (including `vpype`):
+
+```bash
+$ pip install -e .
+$ pip install -r dev-dependencies.txt
+```
+
+
 ## License
 
 See the [LICENSE](LICENSE) file for details.
```

