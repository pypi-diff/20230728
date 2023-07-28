# Comparing `tmp/typer_tinydb-0.1.4.tar.gz` & `tmp/typer_tinydb-0.1.4.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_tinydb-0.1.4.tar", max compression
+gzip compressed data, was "typer_tinydb-0.1.4.post0.tar", max compression
```

## Comparing `typer_tinydb-0.1.4.tar` & `typer_tinydb-0.1.4.post0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:13:33.735228 typer_tinydb-0.1.4/LICENSE
--rw-r--r--   0        0        0     2659 2023-04-30 23:13:33.739228 typer_tinydb-0.1.4/README.md
--rw-r--r--   0        0        0      906 2023-04-30 23:23:51.902066 typer_tinydb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      446 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/__init__.py
--rw-r--r--   0        0        0      172 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/__main__.py
--rw-r--r--   0        0        0      896 2023-04-30 23:23:22.950306 typer_tinydb-0.1.4/typer_tinydb/static/config.json
--rw-r--r--   0        0        0    11362 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tdb.py
--rw-r--r--   0        0        0       21 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tests/__init__.py
--rw-r--r--   0        0        0     4812 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/tests/test_upsert.py
--rw-r--r--   0        0        0    14287 2023-04-30 23:13:33.743228 typer_tinydb-0.1.4/typer_tinydb/utils.py
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 typer_tinydb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-28 01:04:57.952144 typer_tinydb-0.1.4.post0/LICENSE
+-rw-r--r--   0        0        0     4084 2023-07-28 01:04:57.952144 typer_tinydb-0.1.4.post0/README.md
+-rw-r--r--   0        0        0     1021 2023-07-28 01:07:56.269829 typer_tinydb-0.1.4.post0/pyproject.toml
+-rw-r--r--   0        0        0      446 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/__main__.py
+-rw-r--r--   0        0        0      896 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/static/config.json
+-rw-r--r--   0        0        0    11362 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/tdb.py
+-rw-r--r--   0        0        0       21 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/tests/__init__.py
+-rw-r--r--   0        0        0     4812 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/tests/test_upsert.py
+-rw-r--r--   0        0        0    14287 2023-07-28 01:04:57.958143 typer_tinydb-0.1.4.post0/typer_tinydb/utils.py
+-rw-r--r--   0        0        0     4784 1970-01-01 00:00:00.000000 typer_tinydb-0.1.4.post0/PKG-INFO
```

### Comparing `typer_tinydb-0.1.4/LICENSE` & `typer_tinydb-0.1.4.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.4/README.md` & `typer_tinydb-0.1.4.post0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 [![PyPI version](https://badge.fury.io/py/typer-tinydb.svg)](https://badge.fury.io/py/typer-tinydb) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/arnos-stuff/typer-tinydb/master/LICENSE)
 [![codecov](https://codecov.io/gh/arnos-stuff/typer-tinydb/branch/master/graph/badge.svg?token=7MP5WBU8GI)](https://codecov.io/gh/arnos-stuff/typer-tinydb)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/arnos-stuff/typer-tinydb/tree/master.svg?style=shield "CircleCI Build Status")](https://dl.circleci.com/status-badge/redirect/gh/arnos-stuff/typer-tinydb/tree/master)
+[![PyPI dls](https://img.shields.io/pypi/dm/typer-tinydb?color=teal&logo=python&logoColor=green)](https://pypi.org/project/typer-tinydb/)
+
 
 # A Typer config file get/set boilerplate
 
 # Using the boilerplate
 
 ## Aliases and subcommands
 
@@ -50,27 +52,56 @@
 
 With the same configuration as above, your new app can now run the commands:
 
 ```bash
 super-app cfg list # list config key:value pairs
 super-app cfg get some-key # get the values linked to the key 'some-key'
 super-app cfg set some-key '20-hS407zuqYKQ8tPP2r5' # store some hash or token into your settings file
-super-app cfg set some-key '20-hS407zuqYKQ8tPP2r5'
+super-app cfg set -k user23 'supersecretpassword' # it's going to get obfuscated so looking at the JSON doesn't help
 ```
 
 You can obviously use `super-app config get` and others, or any name you attribute to it.
 
 ## Using it within python modules
 
 The CLI key-values are stored in a tinydb instance that is available by just importing the table named `globals`:
 
 ```python
 from typer_tinydb import db, globals, where
 ```
 
+### Insert / Upsert
+
+To insert a new value, the easiest is to use the `upsert_param`.
+
+```python
+def upsert_param(param:str, value:Any, obfuscate: bool = False):
+    ...
+```
+
+This function is used to upsert a parameter (`param`) and its corresponding value (`value`) to the global database.
+The function takes in 3 parameters: `param`, `value`, and `obfuscate`. 
+
+* The `param` parameter is a string that contains the parameter name. 
+* The `value` parameter can take in any type of value, and it contains the value to be upserted to the database.
+* The `obfuscate` parameter is a boolean value that determines if the parameter and its corresponding value will be obfuscated before being stored in the database.
+
+The function uses the usual `Query()` and `db.search(..)` from [tinydb](https://tinydb.readthedocs.io).
+
+The function upserts the `param` and `value` to the database, and also stores the `timestamp`, `machine`, and a boolean to indicate wether parameters are obfuscated.
+
+### Get Keys / Values
+
+There are two pre-made functions: `getKey` and `getValue`. The key difference is as follows:
+
+* `getKey` returns **all the values associated with key `key`**
+* `getValue` arbitrarily returns the first encountered value.
+
+# The underlying database
+
 You can create any table using the database object `db`, please [check out the tinydb docs !](https://tinydb.readthedocs.io/)
 
 To get the key just use `where` :
 
 ```python
 returns = globals.search(where('param') == param)
 ```
@@ -87,8 +118,8 @@
     "machine": socket.gethostname(),
     },
     Param.param == param
 )
 ```
 # Commands
 
-Go check out the [documentation page 🚀](https://arnos-stuff.github.io/typer-tinydb)
+Go check out the [commands page 🚀](commands.md)
```

### Comparing `typer_tinydb-0.1.4/pyproject.toml` & `typer_tinydb-0.1.4.post0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [tool.poetry]
 name = "typer-tinydb"
-version = "0.1.4"
+version = "0.1.4-post0"
 description = "A Python Typer CLI subcommand boilerplate to manage config files using tinydb"
 authors = ["arnos-stuff <bcda0276@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_tinydb"}]
 homepage = "https://arnos-stuff.github.io/typer-tinydb/"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-typer = {extras = ["all"], version = "^0.7.0"}
+python = ">=3.8.1,<4.0"
+typer = [
+	{extras = ["all"], version = "^0.7.0", python = "< 3.10"},
+	{extras = ["all"], version = ">=0.9.0", python = ">= 3.10"}
+	]
+	
 tinydb = "^4.7.1"
 
 
 [tool.poetry.scripts]
 typer-tinydb-config = 'typer_tinydb.db:app'
 tcfg = 'typer_tinydb.tdb:cfg'
 
@@ -22,14 +26,15 @@
 mkdocs-dracula-theme = "^1.0.4"
 mkdocs-material = "^9.1.7"
 pillow = "^9.5.0"
 cairosvg = "^2.7.0"
 mike = "^1.1.2"
 shtab = "^1.6.1"
 mkdocs-glightbox = "^0.3.3"
+flake8 = "^6.0.0"
 pytest = "^7.3.1"
 codecov = "^2.1.13"
 pytest-cov = "^4.0.0"
 mkgendocs = "^0.9.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `typer_tinydb-0.1.4/typer_tinydb/static/config.json` & `typer_tinydb-0.1.4.post0/typer_tinydb/static/config.json`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.4/typer_tinydb/tdb.py` & `typer_tinydb-0.1.4.post0/typer_tinydb/tdb.py`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.4/typer_tinydb/tests/test_upsert.py` & `typer_tinydb-0.1.4.post0/typer_tinydb/tests/test_upsert.py`

 * *Files identical despite different names*

### Comparing `typer_tinydb-0.1.4/typer_tinydb/utils.py` & `typer_tinydb-0.1.4.post0/typer_tinydb/utils.py`

 * *Files identical despite different names*

