# Comparing `tmp/mypy-boto3-schemas-1.28.12.tar.gz` & `tmp/mypy-boto3-schemas-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-schemas-1.28.12.tar", last modified: Thu Jul 27 11:49:36 2023, max compression
+gzip compressed data, was "mypy-boto3-schemas-1.28.15.tar", last modified: Fri Jul 28 20:43:41 2023, max compression
```

## Comparing `mypy-boto3-schemas-1.28.12.tar` & `mypy-boto3-schemas-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-27 11:46:06.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-27 11:46:05.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:35.000000 mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:36.041267 mypy-boto3-schemas-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 11:46:03.000000 mypy-boto3-schemas-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.829838 mypy-boto3-schemas-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-28 20:43:41.825838 mypy-boto3-schemas-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.817838 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-28 20:38:36.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:41.825838 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:41.000000 mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:41.829838 mypy-boto3-schemas-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:38:35.000000 mypy-boto3-schemas-1.28.15/setup.py
```

### Comparing `mypy-boto3-schemas-1.28.12/LICENSE` & `mypy-boto3-schemas-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/PKG-INFO` & `mypy-boto3-schemas-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.28.12
-Summary: Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Schemas 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-schemas-1.28.12/README.md` & `mypy-boto3-schemas-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__init__.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/__main__.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Schemas 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Schemas 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/client.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/literals.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/paginator.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/type_defs.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.py` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas/waiter.pyi` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/PKG-INFO` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.28.12
-Summary: Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Schemas 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-schemas)](https://pepy.tech/project/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-schemas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-schemas-1.28.12/mypy_boto3_schemas.egg-info/SOURCES.txt` & `mypy-boto3-schemas-1.28.15/mypy_boto3_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.28.12/setup.py` & `mypy-boto3-schemas-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-schemas",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Schemas 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Schemas 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```
