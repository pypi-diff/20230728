# Comparing `tmp/mypy-boto3-textract-1.28.12.tar.gz` & `tmp/mypy-boto3-textract-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-textract-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-textract-1.28.15.tar", last modified: Fri Jul 28 20:43:52 2023, max compression
```

## Comparing `mypy-boto3-textract-1.28.12.tar` & `mypy-boto3-textract-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.401432 mypy-boto3-textract-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-27 11:49:46.397432 mypy-boto3-textract-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.385431 mypy-boto3-textract-1.28.12/mypy_boto3_textract/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-07-27 11:47:57.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23288 2023-07-27 11:47:57.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.397432 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.401432 mypy-boto3-textract-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.345982 mypy-boto3-textract-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-28 20:43:52.337982 mypy-boto3-textract-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.337982 mypy-boto3-textract-1.28.15/mypy_boto3_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-07-28 20:40:36.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23288 2023-07-28 20:40:36.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.337982 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:52.000000 mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:52.345982 mypy-boto3-textract-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:40:35.000000 mypy-boto3-textract-1.28.15/setup.py
```

### Comparing `mypy-boto3-textract-1.28.12/LICENSE` & `mypy-boto3-textract-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/PKG-INFO` & `mypy-boto3-textract-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.28.12
-Summary: Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Textract 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-textract-1.28.12/README.md` & `mypy-boto3-textract-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/__main__.py` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Textract 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Textract 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
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

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.py` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.pyi` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.py` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.pyi` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.py` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.pyi` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/PKG-INFO` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.28.12
-Summary: Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Textract 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/SOURCES.txt` & `mypy-boto3-textract-1.28.15/mypy_boto3_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.12/setup.py` & `mypy-boto3-textract-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-textract",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Textract 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

