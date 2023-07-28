# Comparing `tmp/mypy-boto3-serverlessrepo-1.28.12.tar.gz` & `tmp/mypy-boto3-serverlessrepo-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.15.tar", last modified: Fri Jul 28 20:43:43 2023, max compression
```

## Comparing `mypy-boto3-serverlessrepo-1.28.12.tar` & `mypy-boto3-serverlessrepo-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.409289 mypy-boto3-serverlessrepo-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-27 11:49:38.405289 mypy-boto3-serverlessrepo-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.401289 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19897 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.405289 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.409289 mypy-boto3-serverlessrepo-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.025854 mypy-boto3-serverlessrepo-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-07-28 20:39:06.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19897 2023-07-28 20:39:06.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.021854 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:42.000000 mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:43.025854 mypy-boto3-serverlessrepo-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 20:39:05.000000 mypy-boto3-serverlessrepo-1.28.15/setup.py
```

### Comparing `mypy-boto3-serverlessrepo-1.28.12/LICENSE` & `mypy-boto3-serverlessrepo-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.12
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.12/README.md` & `mypy-boto3-serverlessrepo-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.pyi` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__main__.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.pyi` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.pyi` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.pyi` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.py` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.pyi` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.12
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt` & `mypy-boto3-serverlessrepo-1.28.15/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.12/setup.py` & `mypy-boto3-serverlessrepo-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-serverlessrepo",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

