# Comparing `tmp/mypy-boto3-connect-contact-lens-1.28.12.tar.gz` & `tmp/mypy-boto3-connect-contact-lens-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-contact-lens-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-contact-lens-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-connect-contact-lens-1.28.12.tar` & `mypy-boto3-connect-contact-lens-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.328543 mypy-boto3-connect-contact-lens-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-27 05:34:31.328543 mypy-boto3-connect-contact-lens-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.328543 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.328543 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:31.000000 mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.328543 mypy-boto3-connect-contact-lens-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-27 05:19:46.000000 mypy-boto3-connect-contact-lens-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.520910 mypy-boto3-connect-contact-lens-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-28 20:42:34.520910 mypy-boto3-connect-contact-lens-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.520910 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:16.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.520910 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:42:34.000000 mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.520910 mypy-boto3-connect-contact-lens-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-28 20:22:15.000000 mypy-boto3-connect-contact-lens-1.28.15/setup.py
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/LICENSE` & `mypy-boto3-connect-contact-lens-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/PKG-INFO` & `mypy-boto3-connect-contact-lens-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect-contact-lens
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectContactLens 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectContactLens 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect-contact-lens.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect-contact-lens)](https://pepy.tech/project/mypy-boto3-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectContactLens 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[boto3.ConnectContactLens 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
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
 [mypy-boto3-connect-contact-lens docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/README.md` & `mypy-boto3-connect-contact-lens-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect-contact-lens.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect-contact-lens)](https://pepy.tech/project/mypy-boto3-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectContactLens 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[boto3.ConnectContactLens 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
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
 [mypy-boto3-connect-contact-lens docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/__main__.py` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectContactLens 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConnectContactLens 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens\nOther"
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

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/client.py` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/client.pyi` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/literals.py` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/literals.pyi` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/type_defs.py` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,10 +143,10 @@
 )
 
 ListRealtimeContactAnalysisSegmentsResponseTypeDef = TypedDict(
     "ListRealtimeContactAnalysisSegmentsResponseTypeDef",
     {
         "Segments": List[RealtimeContactAnalysisSegmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens/type_defs.pyi` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -138,10 +138,10 @@
 )
 
 ListRealtimeContactAnalysisSegmentsResponseTypeDef = TypedDict(
     "ListRealtimeContactAnalysisSegmentsResponseTypeDef",
     {
         "Segments": List[RealtimeContactAnalysisSegmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/PKG-INFO` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect-contact-lens
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectContactLens 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectContactLens 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect-contact-lens.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect-contact-lens)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connect-contact-lens)](https://pepy.tech/project/mypy-boto3-connect-contact-lens)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectContactLens 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
+[boto3.ConnectContactLens 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens)
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
 [mypy-boto3-connect-contact-lens docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect_contact_lens/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/mypy_boto3_connect_contact_lens.egg-info/SOURCES.txt` & `mypy-boto3-connect-contact-lens-1.28.15/mypy_boto3_connect_contact_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-contact-lens-1.28.12/setup.py` & `mypy-boto3-connect-contact-lens-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect-contact-lens",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_connect_contact_lens"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectContactLens 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ConnectContactLens 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

