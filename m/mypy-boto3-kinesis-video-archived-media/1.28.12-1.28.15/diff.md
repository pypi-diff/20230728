# Comparing `tmp/mypy-boto3-kinesis-video-archived-media-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesis-video-archived-media-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-archived-media-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12.tar` & `mypy-boto3-kinesis-video-archived-media-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.636468 mypy-boto3-kinesis-video-archived-media-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-07-27 05:34:53.636468 mypy-boto3-kinesis-video-archived-media-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.636468 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.636468 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.636468 mypy-boto3-kinesis-video-archived-media-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-archived-media-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.565341 mypy-boto3-kinesis-video-archived-media-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-07-28 20:43:05.561341 mypy-boto3-kinesis-video-archived-media-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.557340 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.561341 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.565341 mypy-boto3-kinesis-video-archived-media-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 20:29:13.000000 mypy-boto3-kinesis-video-archived-media-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/LICENSE` & `mypy-boto3-kinesis-video-archived-media-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,29 +344,29 @@
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
     TimestampRangeTypeDef,
     FragmentTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
     HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ClipFragmentSelectorTypeDef,
     DASHFragmentSelectorTypeDef,
     FragmentSelectorTypeDef,
+    GetClipOutputTypeDef,
+    GetDASHStreamingSessionURLOutputTypeDef,
+    GetHLSStreamingSessionURLOutputTypeDef,
+    GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
     GetHLSStreamingSessionURLInputRequestTypeDef,
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/README.md` & `mypy-boto3-kinesis-video-archived-media-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,29 +312,29 @@
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
     TimestampRangeTypeDef,
     FragmentTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
     HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ClipFragmentSelectorTypeDef,
     DASHFragmentSelectorTypeDef,
     FragmentSelectorTypeDef,
+    GetClipOutputTypeDef,
+    GetDASHStreamingSessionURLOutputTypeDef,
+    GetHLSStreamingSessionURLOutputTypeDef,
+    GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
     GetHLSStreamingSessionURLInputRequestTypeDef,
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__init__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__init__.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/__main__.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/client.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/client.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/literals.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/literals.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/paginator.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
 
@@ -89,13 +89,13 @@
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/paginator.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
 class ListFragmentsPaginator(Paginator):
@@ -84,13 +84,13 @@
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/type_defs.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,29 @@
 
 
 __all__ = (
     "ClipTimestampRangeTypeDef",
     "DASHTimestampRangeTypeDef",
     "TimestampRangeTypeDef",
     "FragmentTypeDef",
-    "GetClipOutputTypeDef",
-    "GetDASHStreamingSessionURLOutputTypeDef",
-    "GetHLSStreamingSessionURLOutputTypeDef",
-    "GetImagesInputGetImagesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "GetImagesInputRequestTypeDef",
     "ImageTypeDef",
     "GetMediaForFragmentListInputRequestTypeDef",
-    "GetMediaForFragmentListOutputTypeDef",
     "HLSTimestampRangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ClipFragmentSelectorTypeDef",
     "DASHFragmentSelectorTypeDef",
     "FragmentSelectorTypeDef",
+    "GetClipOutputTypeDef",
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    "GetMediaForFragmentListOutputTypeDef",
     "ListFragmentsOutputTypeDef",
+    "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
     "HLSFragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
     "GetHLSStreamingSessionURLInputRequestTypeDef",
@@ -106,69 +106,35 @@
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
         "FragmentLengthInMilliseconds": int,
     },
     total=False,
 )
 
-GetClipOutputTypeDef = TypedDict(
-    "GetClipOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetDASHStreamingSessionURLOutputTypeDef",
-    {
-        "DASHStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HLSStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
-    {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetImagesInputGetImagesPaginateTypeDef(
-    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
-):
-    pass
-
-
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
         "SamplingInterval": int,
@@ -225,53 +191,23 @@
 class GetMediaForFragmentListInputRequestTypeDef(
     _RequiredGetMediaForFragmentListInputRequestTypeDef,
     _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
 
-GetMediaForFragmentListOutputTypeDef = TypedDict(
-    "GetMediaForFragmentListOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HLSTimestampRangeTypeDef = TypedDict(
     "HLSTimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ClipFragmentSelectorTypeDef = TypedDict(
     "ClipFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": ClipFragmentSelectorTypeType,
         "TimestampRange": ClipTimestampRangeTypeDef,
     },
 )
@@ -289,29 +225,93 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
+GetClipOutputTypeDef = TypedDict(
+    "GetClipOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    {
+        "DASHStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    {
+        "HLSStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMediaForFragmentListOutputTypeDef = TypedDict(
+    "GetMediaForFragmentListOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFragmentsOutputTypeDef = TypedDict(
     "ListFragmentsOutputTypeDef",
     {
         "Fragments": List[FragmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": Union[datetime, str],
+        "EndTimestamp": Union[datetime, str],
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetImagesInputGetImagesPaginateTypeDef(
+    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+):
+    pass
+
+
 GetImagesOutputTypeDef = TypedDict(
     "GetImagesOutputTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
@@ -359,15 +359,15 @@
 
 ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "FragmentSelector": FragmentSelectorTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFragmentsInputRequestTypeDef = TypedDict(
     "ListFragmentsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media/type_defs.pyi` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -44,29 +44,29 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ClipTimestampRangeTypeDef",
     "DASHTimestampRangeTypeDef",
     "TimestampRangeTypeDef",
     "FragmentTypeDef",
-    "GetClipOutputTypeDef",
-    "GetDASHStreamingSessionURLOutputTypeDef",
-    "GetHLSStreamingSessionURLOutputTypeDef",
-    "GetImagesInputGetImagesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "GetImagesInputRequestTypeDef",
     "ImageTypeDef",
     "GetMediaForFragmentListInputRequestTypeDef",
-    "GetMediaForFragmentListOutputTypeDef",
     "HLSTimestampRangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ClipFragmentSelectorTypeDef",
     "DASHFragmentSelectorTypeDef",
     "FragmentSelectorTypeDef",
+    "GetClipOutputTypeDef",
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    "GetMediaForFragmentListOutputTypeDef",
     "ListFragmentsOutputTypeDef",
+    "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
     "HLSFragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
     "GetHLSStreamingSessionURLInputRequestTypeDef",
@@ -105,67 +105,35 @@
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
         "FragmentLengthInMilliseconds": int,
     },
     total=False,
 )
 
-GetClipOutputTypeDef = TypedDict(
-    "GetClipOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetDASHStreamingSessionURLOutputTypeDef",
-    {
-        "DASHStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HLSStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
-    {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
-    },
-)
-_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetImagesInputGetImagesPaginateTypeDef(
-    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
-):
-    pass
-
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
         "SamplingInterval": int,
@@ -218,53 +186,23 @@
 
 class GetMediaForFragmentListInputRequestTypeDef(
     _RequiredGetMediaForFragmentListInputRequestTypeDef,
     _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
-GetMediaForFragmentListOutputTypeDef = TypedDict(
-    "GetMediaForFragmentListOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HLSTimestampRangeTypeDef = TypedDict(
     "HLSTimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ClipFragmentSelectorTypeDef = TypedDict(
     "ClipFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": ClipFragmentSelectorTypeType,
         "TimestampRange": ClipTimestampRangeTypeDef,
     },
 )
@@ -282,29 +220,91 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
+GetClipOutputTypeDef = TypedDict(
+    "GetClipOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    {
+        "DASHStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    {
+        "HLSStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMediaForFragmentListOutputTypeDef = TypedDict(
+    "GetMediaForFragmentListOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFragmentsOutputTypeDef = TypedDict(
     "ListFragmentsOutputTypeDef",
     {
         "Fragments": List[FragmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": Union[datetime, str],
+        "EndTimestamp": Union[datetime, str],
+        "SamplingInterval": int,
+        "Format": FormatType,
     },
 )
+_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetImagesInputGetImagesPaginateTypeDef(
+    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+):
+    pass
 
 GetImagesOutputTypeDef = TypedDict(
     "GetImagesOutputTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
@@ -350,15 +350,15 @@
 
 ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "FragmentSelector": FragmentSelectorTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFragmentsInputRequestTypeDef = TypedDict(
     "ListFragmentsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-archived-media
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-archived-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoArchivedMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
+[boto3.KinesisVideoArchivedMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [mypy-boto3-kinesis-video-archived-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_archived_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,29 +344,29 @@
 
 ```python
 from mypy_boto3_kinesis_video_archived_media.type_defs import (
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
     TimestampRangeTypeDef,
     FragmentTypeDef,
-    GetClipOutputTypeDef,
-    GetDASHStreamingSessionURLOutputTypeDef,
-    GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     GetImagesInputRequestTypeDef,
     ImageTypeDef,
     GetMediaForFragmentListInputRequestTypeDef,
-    GetMediaForFragmentListOutputTypeDef,
     HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ClipFragmentSelectorTypeDef,
     DASHFragmentSelectorTypeDef,
     FragmentSelectorTypeDef,
+    GetClipOutputTypeDef,
+    GetDASHStreamingSessionURLOutputTypeDef,
+    GetHLSStreamingSessionURLOutputTypeDef,
+    GetMediaForFragmentListOutputTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
     GetHLSStreamingSessionURLInputRequestTypeDef,
```

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-archived-media-1.28.15/mypy_boto3_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-archived-media-1.28.12/setup.py` & `mypy-boto3-kinesis-video-archived-media-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-archived-media",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KinesisVideoArchivedMedia 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

