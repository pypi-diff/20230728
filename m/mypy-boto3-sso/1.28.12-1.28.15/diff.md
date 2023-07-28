# Comparing `tmp/mypy-boto3-sso-1.28.12.tar.gz` & `tmp/mypy-boto3-sso-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-1.28.15.tar", last modified: Fri Jul 28 20:43:50 2023, max compression
```

## Comparing `mypy-boto3-sso-1.28.12.tar` & `mypy-boto3-sso-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.041343 mypy-boto3-sso-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/mypy_boto3_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-27 11:47:36.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.033343 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:43.000000 mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.041343 mypy-boto3-sso-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:35.000000 mypy-boto3-sso-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.277954 mypy-boto3-sso-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-28 20:43:50.277954 mypy-boto3-sso-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.277954 mypy-boto3-sso-1.28.15/mypy_boto3_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:50.277954 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:50.000000 mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:50.277954 mypy-boto3-sso-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:40:12.000000 mypy-boto3-sso-1.28.15/setup.py
```

### Comparing `mypy-boto3-sso-1.28.12/LICENSE` & `mypy-boto3-sso-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/PKG-INFO` & `mypy-boto3-sso-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso
-Version: 1.28.12
-Summary: Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSO 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-1.28.12/README.md` & `mypy-boto3-sso-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__init__.pyi` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/__main__.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSO 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SSO 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/client.pyi` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/literals.pyi` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/paginator.pyi` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.py` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso/type_defs.pyi` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/PKG-INFO` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso
-Version: 1.28.12
-Summary: Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSO 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso)](https://pepy.tech/project/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-sso-1.28.12/mypy_boto3_sso.egg-info/SOURCES.txt` & `mypy-boto3-sso-1.28.15/mypy_boto3_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.28.12/setup.py` & `mypy-boto3-sso-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSO 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SSO 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```
