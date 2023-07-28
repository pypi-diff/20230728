# Comparing `tmp/PDFAgent-0.2.2.tar.gz` & `tmp/PDFAgent-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFAgent-0.2.2.tar", last modified: Fri Jul 28 14:49:51 2023, max compression
+gzip compressed data, was "PDFAgent-0.2.3.tar", last modified: Fri Jul 28 14:52:02 2023, max compression
```

## Comparing `PDFAgent-0.2.2.tar` & `PDFAgent-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:49:51.331398 PDFAgent-0.2.2/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.2.2/LICENSE
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:49:51.328698 PDFAgent-0.2.2/PDFAgent/
--rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-28 14:48:36.000000 PDFAgent-0.2.2/PDFAgent/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2203 2023-07-28 14:48:40.000000 PDFAgent-0.2.2/PDFAgent/agent.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:49:51.330276 PDFAgent-0.2.2/PDFAgent.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:49:51.000000 PDFAgent-0.2.2/PDFAgent.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:49:51.000000 PDFAgent-0.2.2/PDFAgent.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:49:51.000000 PDFAgent-0.2.2/PDFAgent.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:49:51.000000 PDFAgent-0.2.2/PDFAgent.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:49:51.000000 PDFAgent-0.2.2/PDFAgent.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:49:51.331118 PDFAgent-0.2.2/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.2.2/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:49:51.331490 PDFAgent-0.2.2/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:49:37.000000 PDFAgent-0.2.2/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:49:51.330555 PDFAgent-0.2.2/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.2.2/tests/test_basic.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:52:02.913425 PDFAgent-0.2.3/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.2.3/LICENSE
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:52:02.910943 PDFAgent-0.2.3/PDFAgent/
+-rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-28 14:51:48.000000 PDFAgent-0.2.3/PDFAgent/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2170 2023-07-28 14:51:44.000000 PDFAgent-0.2.3/PDFAgent/agent.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:52:02.912289 PDFAgent-0.2.3/PDFAgent.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:52:02.000000 PDFAgent-0.2.3/PDFAgent.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:52:02.000000 PDFAgent-0.2.3/PDFAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:52:02.000000 PDFAgent-0.2.3/PDFAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:52:02.000000 PDFAgent-0.2.3/PDFAgent.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:52:02.000000 PDFAgent-0.2.3/PDFAgent.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:52:02.913145 PDFAgent-0.2.3/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.2.3/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:52:02.913523 PDFAgent-0.2.3/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:51:52.000000 PDFAgent-0.2.3/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:52:02.912552 PDFAgent-0.2.3/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.2.3/tests/test_basic.py
```

### Comparing `PDFAgent-0.2.2/LICENSE` & `PDFAgent-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PDFAgent-0.2.2/PDFAgent/agent.py` & `PDFAgent-0.2.3/PDFAgent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         """
         return self.collection.template(
             prompt=prompt,
             prompt_fields=["autoGen_content"],
             fields=["autoGen_content"],
             conversation_id=conversation_id,
             limit=limit,
-            include_rerank=True,
             minimum_score=minimum_score,
             include_moderation=include_moderation
         )
 
     def copilot(self, prompt: str, conversation_id: str=None):
         """The endpoint for advanced analysis
         """
```

### Comparing `PDFAgent-0.2.2/README.md` & `PDFAgent-0.2.3/README.md`

 * *Files identical despite different names*

