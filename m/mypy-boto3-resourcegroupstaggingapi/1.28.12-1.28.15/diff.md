# Comparing `tmp/mypy-boto3-resourcegroupstaggingapi-1.28.12.tar.gz` & `tmp/mypy-boto3-resourcegroupstaggingapi-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-resourcegroupstaggingapi-1.28.15.tar", last modified: Fri Jul 28 20:43:34 2023, max compression
```

## Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12.tar` & `mypy-boto3-resourcegroupstaggingapi-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.325214 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-27 11:44:42.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-27 11:44:41.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 11:49:30.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.329213 mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 11:44:40.000000 mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.849742 mypy-boto3-resourcegroupstaggingapi-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-28 20:43:34.849742 mypy-boto3-resourcegroupstaggingapi-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.845742 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-28 20:37:01.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-28 20:37:01.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-28 20:37:01.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-28 20:37:01.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-28 20:37:01.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.849742 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 20:43:34.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:34.849742 mypy-boto3-resourcegroupstaggingapi-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-28 20:37:00.000000 mypy-boto3-resourcegroupstaggingapi-1.28.15/setup.py
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/LICENSE` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/README.md` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__init__.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/__main__.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/client.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/literals.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/paginator.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resourcegroupstaggingapi
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resourcegroupstaggingapi)](https://pepy.tech/project/mypy-boto3-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroupsTaggingAPI 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
+[boto3.ResourceGroupsTaggingAPI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [mypy-boto3-resourcegroupstaggingapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resourcegroupstaggingapi/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/mypy_boto3_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resourcegroupstaggingapi-1.28.12/setup.py` & `mypy-boto3-resourcegroupstaggingapi-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resourcegroupstaggingapi",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ResourceGroupsTaggingAPI 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

