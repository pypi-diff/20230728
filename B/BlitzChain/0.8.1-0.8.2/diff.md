# Comparing `tmp/BlitzChain-0.8.1.tar.gz` & `tmp/BlitzChain-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.8.1.tar", last modified: Mon Jul 24 03:47:04 2023, max compression
+gzip compressed data, was "BlitzChain-0.8.2.tar", last modified: Fri Jul 28 14:38:29 2023, max compression
```

## Comparing `BlitzChain-0.8.1.tar` & `BlitzChain-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.986428 BlitzChain-0.8.1/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.983977 BlitzChain-0.8.1/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-24 03:47:04.000000 BlitzChain-0.8.1/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.8.1/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-24 03:47:04.986291 BlitzChain-0.8.1/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3436 2023-07-09 13:29:34.000000 BlitzChain-0.8.1/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.984835 BlitzChain-0.8.1/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-24 03:46:21.000000 BlitzChain-0.8.1/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)    10275 2023-07-24 03:46:09.000000 BlitzChain-0.8.1/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2079 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      794 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.985234 BlitzChain-0.8.1/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-07-09 14:53:24.000000 BlitzChain-0.8.1/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      435 2023-07-20 07:06:24.000000 BlitzChain-0.8.1/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-24 03:47:04.986472 BlitzChain-0.8.1/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      481 2023-07-24 03:30:52.000000 BlitzChain-0.8.1/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 03:47:04.986045 BlitzChain-0.8.1/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      722 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      615 2023-07-23 13:02:56.000000 BlitzChain-0.8.1/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:38:29.718236 BlitzChain-0.8.2/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:38:29.713088 BlitzChain-0.8.2/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-28 14:38:29.000000 BlitzChain-0.8.2/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-28 14:38:29.000000 BlitzChain-0.8.2/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:38:29.000000 BlitzChain-0.8.2/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:38:29.000000 BlitzChain-0.8.2/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-28 14:38:29.000000 BlitzChain-0.8.2/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.8.2/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-28 14:38:29.717944 BlitzChain-0.8.2/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3436 2023-07-09 13:29:34.000000 BlitzChain-0.8.2/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:38:29.715022 BlitzChain-0.8.2/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-28 14:38:07.000000 BlitzChain-0.8.2/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)    10182 2023-07-28 14:37:58.000000 BlitzChain-0.8.2/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2079 2023-07-23 13:02:56.000000 BlitzChain-0.8.2/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      794 2023-07-23 13:02:56.000000 BlitzChain-0.8.2/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:38:29.715814 BlitzChain-0.8.2/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-07-09 14:53:24.000000 BlitzChain-0.8.2/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      435 2023-07-20 07:06:24.000000 BlitzChain-0.8.2/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:38:29.718335 BlitzChain-0.8.2/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      481 2023-07-24 03:30:52.000000 BlitzChain-0.8.2/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:38:29.717453 BlitzChain-0.8.2/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-07-23 13:02:56.000000 BlitzChain-0.8.2/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      722 2023-07-23 13:02:56.000000 BlitzChain-0.8.2/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      615 2023-07-23 13:02:56.000000 BlitzChain-0.8.2/tests/test_qa.py
```

### Comparing `BlitzChain-0.8.1/LICENSE` & `BlitzChain-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.1/README.md` & `BlitzChain-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.1/blitzchain/api.py` & `BlitzChain-0.8.2/blitzchain/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,27 +282,26 @@
         token = encoding.decode()
         link = "https://ask.twilix.io/custom?token=" + token
         print(link)
     
     def template(
         self, prompt: str, prompt_fields: list=None,
         limit: int=5, fields: list=None,
-        include_rerank: bool=False, minimum_rerank_score: float=0.05,
+        minimum_score: float=0.05,
         include_moderation: bool=False, conversation_id: str=None
     ):
         url = self.base_url + "collection/template"
         print(url)
         data = {
             "collection": self.collection_name,
             "prompt": prompt,
             "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
-            "includeRerank": include_rerank,
-            "minimumRerankScore": minimum_rerank_score,
+            "minimumScore": minimum_score,
             "includeModeration": include_moderation,
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
```

### Comparing `BlitzChain-0.8.1/blitzchain/splitter.py` & `BlitzChain-0.8.2/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.1/blitzchain/utils.py` & `BlitzChain-0.8.2/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.1/tests/test_pdf.py` & `BlitzChain-0.8.2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.8.1/tests/test_qa.py` & `BlitzChain-0.8.2/tests/test_qa.py`

 * *Files identical despite different names*

