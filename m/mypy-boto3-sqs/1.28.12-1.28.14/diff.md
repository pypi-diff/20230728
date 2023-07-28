# Comparing `tmp/mypy-boto3-sqs-1.28.12.tar.gz` & `tmp/mypy-boto3-sqs-1.28.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.28.14.tar", last modified: Fri Jul 28 01:48:35 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.28.12.tar` & `mypy-boto3-sqs-1.28.14.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.593320 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-27 11:47:14.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-27 11:47:14.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-07-27 11:47:15.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-27 11:47:15.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:35.397926 mypy-boto3-sqs-1.28.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-28 01:48:35.397926 mypy-boto3-sqs-1.28.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:35.397926 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18052 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19031 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18992 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-28 01:48:25.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:48:35.397926 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 01:48:35.000000 mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:48:35.397926 mypy-boto3-sqs-1.28.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 01:48:24.000000 mypy-boto3-sqs-1.28.14/setup.py
```

### Comparing `mypy-boto3-sqs-1.28.12/LICENSE` & `mypy-boto3-sqs-1.28.14/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/PKG-INFO` & `mypy-boto3-sqs-1.28.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.12
-Summary: Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.14
+Summary: Type annotations for boto3.SQS 1.28.14 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.14](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sqs-1.28.12/README.md` & `mypy-boto3-sqs-1.28.14/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.14](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        "Type annotations for boto3.SQS 1.28.14\nVersion:         1.28.14\nBuilder version:"
         " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.14")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queues)
         """
 
     def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#purge_queue)
         """
 
     def receive_message(
         self,
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,16 @@
         Returns a list of your queues in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queues)
         """
     def purge_queue(self, *, QueueUrl: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.purge_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#purge_queue)
         """
     def receive_message(
         self,
         *,
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queueload-method)
         """
 
     def purge(self) -> None:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.purge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuepurge-method)
         """
 
     def receive_messages(
         self,
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,16 @@
         Queue resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.load)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queueload-method)
         """
     def purge(self) -> None:
         """
-        Deletes the messages in a queue specified by the `QueueURL` parameter.
+        Deletes available messages in a queue (including in-flight messages) specified
+        by the `QueueURL` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.purge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuepurge-method)
         """
     def receive_messages(
         self,
         *,
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.12
-Summary: Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.14
+Summary: Type annotations for boto3.SQS 1.28.14 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.14](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.28.14/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.12/setup.py` & `mypy-boto3-sqs-1.28.14/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.28.12",
+    version="1.28.14",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SQS 1.28.14 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

