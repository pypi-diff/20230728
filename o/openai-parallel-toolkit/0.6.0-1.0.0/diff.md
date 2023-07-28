# Comparing `tmp/openai_parallel_toolkit-0.6.0-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,9 @@
-Zip file size: 18761 bytes, number of entries: 19
--rw-r--r--  2.0 unx      184 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/__init__.py
--rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
--rw-r--r--  2.0 unx      150 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/api/__init__.py
--rw-r--r--  2.0 unx     5216 b- defN 23-Jun-19 07:03 openai_parallel_toolkit/api/api.py
--rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
--rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
--rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
--rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
--rw-r--r--  2.0 unx     4831 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/core/multithread.py
--rw-r--r--  2.0 unx      148 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/utils/__init__.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/utils/logger.py
--rw-r--r--  2.0 unx     4107 b- defN 23-Jun-26 03:26 openai_parallel_toolkit/utils/reader.py
--rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
--rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13483 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1783 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/RECORD
-19 files, 47627 bytes uncompressed, 15763 bytes compressed:  66.9%
+Zip file size: 5560 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-28 11:58 openai_parallel_toolkit/__init__.py
+-rw-r--r--  2.0 unx     2897 b- defN 23-Jul-28 12:53 openai_parallel_toolkit/main.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6002 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      644 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/RECORD
+7 files, 10799 bytes uncompressed, 4396 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -1,58 +1,22 @@
 Filename: openai_parallel_toolkit/__init__.py
 Comment: 
 
-Filename: openai_parallel_toolkit/config.py
+Filename: openai_parallel_toolkit/main.py
 Comment: 
 
-Filename: openai_parallel_toolkit/api/__init__.py
+Filename: openai_parallel_toolkit-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit/api/api.py
+Filename: openai_parallel_toolkit-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit/api/keys.py
+Filename: openai_parallel_toolkit-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit/api/request.py
+Filename: openai_parallel_toolkit-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit/core/__init__.py
-Comment: 
-
-Filename: openai_parallel_toolkit/core/main.py
-Comment: 
-
-Filename: openai_parallel_toolkit/core/multithread.py
-Comment: 
-
-Filename: openai_parallel_toolkit/utils/__init__.py
-Comment: 
-
-Filename: openai_parallel_toolkit/utils/logger.py
-Comment: 
-
-Filename: openai_parallel_toolkit/utils/reader.py
-Comment: 
-
-Filename: openai_parallel_toolkit/utils/token.py
-Comment: 
-
-Filename: openai_parallel_toolkit/utils/tqdm.py
-Comment: 
-
-Filename: openai_parallel_toolkit-0.6.0.dist-info/LICENSE
-Comment: 
-
-Filename: openai_parallel_toolkit-0.6.0.dist-info/METADATA
-Comment: 
-
-Filename: openai_parallel_toolkit-0.6.0.dist-info/WHEEL
-Comment: 
-
-Filename: openai_parallel_toolkit-0.6.0.dist-info/top_level.txt
-Comment: 
-
-Filename: openai_parallel_toolkit-0.6.0.dist-info/RECORD
+Filename: openai_parallel_toolkit-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .api import APIKeyManager, Gpt35Turbo, Gpt35Turbo0613, Gpt35Turbo16K, Gpt4, OpenAIModel, request_openai_api
-from .core import ParallelToolkit, multi_process_one, multi_thread_run
+from .api.model import OpenAIModel, Prompt
+from .main import ParallelToolkit
```

## Comparing `openai_parallel_toolkit-0.6.0.dist-info/LICENSE` & `openai_parallel_toolkit-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

