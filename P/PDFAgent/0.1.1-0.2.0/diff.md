# Comparing `tmp/PDFAgent-0.1.1.tar.gz` & `tmp/PDFAgent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFAgent-0.1.1.tar", last modified: Fri Jul 28 14:31:07 2023, max compression
+gzip compressed data, was "PDFAgent-0.2.0.tar", last modified: Fri Jul 28 14:40:11 2023, max compression
```

## Comparing `PDFAgent-0.1.1.tar` & `PDFAgent-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.808531 PDFAgent-0.1.1/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.1.1/LICENSE
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.805780 PDFAgent-0.1.1/PDFAgent/
--rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.1.1/PDFAgent/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1967 2023-07-28 14:28:51.000000 PDFAgent-0.1.1/PDFAgent/agent.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.807212 PDFAgent-0.1.1/PDFAgent.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:31:07.808227 PDFAgent-0.1.1/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.1.1/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:31:07.808633 PDFAgent-0.1.1/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:29:24.000000 PDFAgent-0.1.1/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.807516 PDFAgent-0.1.1/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.1.1/tests/test_basic.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.451284 PDFAgent-0.2.0/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.2.0/LICENSE
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.448623 PDFAgent-0.2.0/PDFAgent/
+-rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.2.0/PDFAgent/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2224 2023-07-28 14:40:02.000000 PDFAgent-0.2.0/PDFAgent/agent.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.450031 PDFAgent-0.2.0/PDFAgent.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:40:11.000000 PDFAgent-0.2.0/PDFAgent.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:40:11.450979 PDFAgent-0.2.0/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.2.0/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:40:11.451384 PDFAgent-0.2.0/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:40:07.000000 PDFAgent-0.2.0/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:40:11.450344 PDFAgent-0.2.0/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.2.0/tests/test_basic.py
```

### Comparing `PDFAgent-0.1.1/LICENSE` & `PDFAgent-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PDFAgent-0.1.1/PDFAgent/agent.py` & `PDFAgent-0.2.0/PDFAgent/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 
     def read_pdf(self, url: str):
         """Inserting a PDF via URL.
         """
         result = self.collection.insert_pdf(url)
         print("Inserting PDF... Please wait 30-60 seconds for this to finish indexing.")
         return result
+
+    def view(
+        self,
+        limit: int = 5,
+        offset: int = 0,
+        fields: list = None,
+        where=None,
+        sort: list = None,
+    ):
+        return self.collection.list_objects(limit=limit, offset=offset, where=where, sort=sort)
     
     def ask(self, question: str, conversation_id: str=None):
         """Ask your PDF a question
         """
         return self.collection.generative_qa(
             prompt=question,
             prompt_fields=None,
```

### Comparing `PDFAgent-0.1.1/README.md` & `PDFAgent-0.2.0/README.md`

 * *Files identical despite different names*

