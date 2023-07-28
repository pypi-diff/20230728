# Comparing `tmp/mkdocs_multirepo_plugin-0.6.1.tar.gz` & `tmp/mkdocs_multirepo_plugin-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_multirepo_plugin-0.6.1.tar", max compression
+gzip compressed data, was "mkdocs_multirepo_plugin-0.6.2.tar", max compression
```

## Comparing `mkdocs_multirepo_plugin-0.6.1.tar` & `mkdocs_multirepo_plugin-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-03-29 13:10:54.752523 mkdocs_multirepo_plugin-0.6.1/LICENSE
--rw-r--r--   0        0        0    13420 2023-03-29 13:10:54.752523 mkdocs_multirepo_plugin-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/__init__.py
--rw-r--r--   0        0        0    14329 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/plugin.py
--rw-r--r--   0        0        0       37 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/scripts/mv_docs_up.sh
--rwxr-xr-x   0        0        0      633 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/scripts/sparse_clone.sh
--rw-r--r--   0        0        0      910 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/scripts/sparse_clone_old.sh
--rw-r--r--   0        0        0    18212 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/structure.py
--rw-r--r--   0        0        0     4063 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/util.py
--rw-r--r--   0        0        0     1785 2023-03-29 13:10:54.756523 mkdocs_multirepo_plugin-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    15073 1970-01-01 00:00:00.000000 mkdocs_multirepo_plugin-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 12:41:31.099058 mkdocs_multirepo_plugin-0.6.2/LICENSE
+-rw-r--r--   0        0        0    13406 2023-07-28 12:41:31.099058 mkdocs_multirepo_plugin-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/__init__.py
+-rw-r--r--   0        0        0    14329 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/plugin.py
+-rw-r--r--   0        0        0       37 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/scripts/mv_docs_up.sh
+-rwxr-xr-x   0        0        0      633 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/scripts/sparse_clone.sh
+-rw-r--r--   0        0        0      910 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/scripts/sparse_clone_old.sh
+-rw-r--r--   0        0        0    18212 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/structure.py
+-rw-r--r--   0        0        0     4063 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/util.py
+-rw-r--r--   0        0        0     1815 2023-07-28 12:41:31.107058 mkdocs_multirepo_plugin-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    15092 1970-01-01 00:00:00.000000 mkdocs_multirepo_plugin-0.6.2/PKG-INFO
```

### Comparing `mkdocs_multirepo_plugin-0.6.1/LICENSE` & `mkdocs_multirepo_plugin-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/README.md` & `mkdocs_multirepo_plugin-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-:warning: One person maintains this plugin in their spare time for free. :warning:
-
 If you like this plugin and want me to continue maintaining it in my free time, please buy me a [beer 🍺](https://www.buymeacoffee.com/jdoiro) or sponser this plugin!
 
 # mkdocs-multirepo-plugin
 
 [![](https://github.com/jdoiro3/mkdocs-multirepo-plugin/workflows/Tests/badge.svg)](https://github.com/jdoiro3/mkdocs-multirepo-plugin/actions)
 [![](https://github.com/jdoiro3/mkdocs-multirepo-plugin/workflows/Build%2C%20Test%20%26%20Deploy/badge.svg)](https://github.com/jdoiro3/mkdocs-multirepo-plugin/actions)
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-multirepo-plugin)](https://pypi.org/project/mkdocs-multirepo-plugin/)
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![Project Status: Inactive – The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows.](https://www.repostatus.org/badges/latest/inactive.svg)](https://www.repostatus.org/#inactive)
 ![](https://img.shields.io/badge/lifecycle-beta-509bf5.svg)
 <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/mkdocs-multirepo-plugin?style=plastic">
 
 Build documentation in multiple repos into one site.
 
 ## Features
 
@@ -43,15 +41,15 @@
 pip install mkdocs-multirepo-plugin
 ```
 
 Next, add the plugin to your `mkdocs.yml`
 
 ```yaml
 plugins:
-  - multirepo
+  - multirepo:
       # (optional) tells multirepo to cleanup the temporary directory after site is built.
       cleanup: true
       # if set the docs directory will not be removed when importing docs.
       # When using this with a nav section in an imported repo you must keep the
       # docs directory in the path (e.g., docs/path/to/file.md).
       keep_docs_dir: true
 ```
```

### Comparing `mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/plugin.py` & `mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/scripts/sparse_clone.sh` & `mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/scripts/sparse_clone.sh`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/scripts/sparse_clone_old.sh` & `mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/scripts/sparse_clone_old.sh`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/structure.py` & `mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/structure.py`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/mkdocs_multirepo_plugin/util.py` & `mkdocs_multirepo_plugin-0.6.2/mkdocs_multirepo_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs_multirepo_plugin-0.6.1/pyproject.toml` & `mkdocs_multirepo_plugin-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-multirepo-plugin"
-version = "0.6.1"
+version = "0.6.2"
 description = "Build documentation in multiple repos into one site."
 authors = ["jdoiro3 <josephdoiron1234@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/mkdocs-multirepo-plugin/"
 repository = "https://github.com/jdoiro3/mkdocs-multirepo-plugin"
 keywords = ["mkdocs", "docs", "documentation"]
@@ -21,15 +21,15 @@
 [tool.poetry.scripts]
 sparse_clone = { reference = 'mkdocs_multirepo_plugin/scripts/sparse_clone.sh', type = "file" }
 sparse_clone_old = { reference = 'mkdocs_multirepo_plugin/scripts/sparse_clone_old.sh', type = "file" }
 mv_docs_up = { reference = 'mkdocs_multirepo_plugin/scripts/mv_docs_up.sh', type = "file" }
 
 [tool.poetry.dependencies]
 mkdocs = {version = ">=1.0.4", python = ">=3.6"}
-asyncio = "*"
+asyncio = {version = "*", python = "<=3.8"}
 python-slugify = {version = "*", python = ">=2.7,<2.8 || >=3.6.0"}
 dacite = {version = "^1.8.0", python = ">=3.6"}
 typing-inspect = {version = "^0.8.0", python = ">=3.6"}
 
 [tool.poetry.dev-dependencies]
 aiofiles = {version = "*", python = ">=3.6,<4.0"}
 flake8 = {version = "*", python = ">=3.6.1"}
```

### Comparing `mkdocs_multirepo_plugin-0.6.1/PKG-INFO` & `mkdocs_multirepo_plugin-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-multirepo-plugin
-Version: 0.6.1
+Version: 0.6.2
 Summary: Build documentation in multiple repos into one site.
 Home-page: https://pypi.org/project/mkdocs-multirepo-plugin/
 License: MIT
 Keywords: mkdocs,docs,documentation
 Author: jdoiro3
 Author-email: josephdoiron1234@yahoo.com
 Classifier: Development Status :: 3 - Alpha
@@ -22,32 +22,30 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
-Requires-Dist: asyncio
+Requires-Dist: asyncio ; python_full_version <= "3.8.0"
 Requires-Dist: dacite (>=1.8.0,<2.0.0) ; python_version >= "3.6"
 Requires-Dist: mkdocs (>=1.0.4) ; python_version >= "3.6"
 Requires-Dist: python-slugify ; python_version >= "2.7" and python_version < "2.8" or python_full_version >= "3.6.0"
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0) ; python_version >= "3.6"
 Project-URL: Repository, https://github.com/jdoiro3/mkdocs-multirepo-plugin
 Description-Content-Type: text/markdown
 
-:warning: One person maintains this plugin in their spare time for free. :warning:
-
 If you like this plugin and want me to continue maintaining it in my free time, please buy me a [beer 🍺](https://www.buymeacoffee.com/jdoiro) or sponser this plugin!
 
 # mkdocs-multirepo-plugin
 
 [![](https://github.com/jdoiro3/mkdocs-multirepo-plugin/workflows/Tests/badge.svg)](https://github.com/jdoiro3/mkdocs-multirepo-plugin/actions)
 [![](https://github.com/jdoiro3/mkdocs-multirepo-plugin/workflows/Build%2C%20Test%20%26%20Deploy/badge.svg)](https://github.com/jdoiro3/mkdocs-multirepo-plugin/actions)
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-multirepo-plugin)](https://pypi.org/project/mkdocs-multirepo-plugin/)
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![Project Status: Inactive – The project has reached a stable, usable state but is no longer being actively developed; support/maintenance will be provided as time allows.](https://www.repostatus.org/badges/latest/inactive.svg)](https://www.repostatus.org/#inactive)
 ![](https://img.shields.io/badge/lifecycle-beta-509bf5.svg)
 <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/mkdocs-multirepo-plugin?style=plastic">
 
 Build documentation in multiple repos into one site.
 
 ## Features
 
@@ -79,15 +77,15 @@
 pip install mkdocs-multirepo-plugin
 ```
 
 Next, add the plugin to your `mkdocs.yml`
 
 ```yaml
 plugins:
-  - multirepo
+  - multirepo:
       # (optional) tells multirepo to cleanup the temporary directory after site is built.
       cleanup: true
       # if set the docs directory will not be removed when importing docs.
       # When using this with a nav section in an imported repo you must keep the
       # docs directory in the path (e.g., docs/path/to/file.md).
       keep_docs_dir: true
 ```
```

