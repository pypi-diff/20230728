# Comparing `tmp/PDFAgent-0.2.0.tar.gz` & `tmp/PDFAgent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFAgent-0.2.0.tar", last modified: Fri Jul 28 14:40:11 2023, max compression
+gzip compressed data, was "PDFAgent-0.2.1.tar", last modified: Fri Jul 28 14:45:53 2023, max compression
```

## Comparing `PDFAgent-0.2.0.tar` & `PDFAgent-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.451284 PDFAgent-0.2.0/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.2.0/LICENSE
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.448623 PDFAgent-0.2.0/PDFAgent/
--rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.2.0/PDFAgent/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2224 2023-07-28 14:40:02.000000 PDFAgent-0.2.0/PDFAgent/agent.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.450031 PDFAgent-0.2.0/PDFAgent.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:40:11.450979 PDFAgent-0.2.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.2.0/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:40:11.451384 PDFAgent-0.2.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:40:07.000000 PDFAgent-0.2.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.450344 PDFAgent-0.2.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.2.0/tests/test_basic.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:45:53.461197 PDFAgent-0.2.1/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.2.1/LICENSE
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:45:53.457962 PDFAgent-0.2.1/PDFAgent/
+-rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.2.1/PDFAgent/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2203 2023-07-28 14:45:03.000000 PDFAgent-0.2.1/PDFAgent/agent.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:45:53.459988 PDFAgent-0.2.1/PDFAgent.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:45:53.000000 PDFAgent-0.2.1/PDFAgent.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:45:53.000000 PDFAgent-0.2.1/PDFAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:45:53.000000 PDFAgent-0.2.1/PDFAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:45:53.000000 PDFAgent-0.2.1/PDFAgent.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:45:53.000000 PDFAgent-0.2.1/PDFAgent.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:45:53.460892 PDFAgent-0.2.1/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.2.1/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:45:53.461305 PDFAgent-0.2.1/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:45:50.000000 PDFAgent-0.2.1/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:45:53.460288 PDFAgent-0.2.1/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.2.1/tests/test_basic.py
```

### Comparing `PDFAgent-0.2.0/LICENSE` & `PDFAgent-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PDFAgent-0.2.0/PDFAgent/agent.py` & `PDFAgent-0.2.1/PDFAgent/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,27 +42,27 @@
         )
 
     def template(
         self, 
         prompt: str, 
         conversation_id: str=None,
         limit: int=5, 
-        minimum_rerank_score: float=0.05,
+        minimum_score: float=0.01,
         include_moderation: bool=False, 
     ):
         """Use a template to analyze how your PDF
         """
         return self.collection.template(
             prompt=prompt,
             prompt_fields=["autoGen_content"],
             fields=["autoGen_content"],
             conversation_id=conversation_id,
             limit=limit,
             include_rerank=True,
-            minimum_rerank_score=minimum_rerank_score,
+            minimum_score=minimum_score,
             include_moderation=include_moderation
         )
 
     def copilot(self, prompt: str, conversation_id: str=None):
         """The endpoint for advanced analysis
         """
         return self.collection.copilot(
```

### Comparing `PDFAgent-0.2.0/README.md` & `PDFAgent-0.2.1/README.md`

 * *Files identical despite different names*

