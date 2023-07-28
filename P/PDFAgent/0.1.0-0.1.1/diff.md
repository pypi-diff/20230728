# Comparing `tmp/PDFAgent-0.1.0.tar.gz` & `tmp/PDFAgent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFAgent-0.1.0.tar", last modified: Mon Jul 24 04:39:40 2023, max compression
+gzip compressed data, was "PDFAgent-0.1.1.tar", last modified: Fri Jul 28 14:31:07 2023, max compression
```

## Comparing `PDFAgent-0.1.0.tar` & `PDFAgent-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 04:39:40.046007 PDFAgent-0.1.0/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.1.0/LICENSE
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 04:39:40.042868 PDFAgent-0.1.0/PDFAgent/
--rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.1.0/PDFAgent/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1626 2023-07-24 04:24:28.000000 PDFAgent-0.1.0/PDFAgent/agent.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 04:39:40.044678 PDFAgent-0.1.0/PDFAgent.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-24 04:39:39.000000 PDFAgent-0.1.0/PDFAgent.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-24 04:39:39.000000 PDFAgent-0.1.0/PDFAgent.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-24 04:39:39.000000 PDFAgent-0.1.0/PDFAgent.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-24 04:39:39.000000 PDFAgent-0.1.0/PDFAgent.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-24 04:39:39.000000 PDFAgent-0.1.0/PDFAgent.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-24 04:39:40.045682 PDFAgent-0.1.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     2281 2023-07-24 04:37:29.000000 PDFAgent-0.1.0/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-24 04:39:40.046130 PDFAgent-0.1.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-24 04:39:37.000000 PDFAgent-0.1.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-24 04:39:40.044958 PDFAgent-0.1.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.1.0/tests/test_basic.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.808531 PDFAgent-0.1.1/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-07-24 02:34:20.000000 PDFAgent-0.1.1/LICENSE
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.805780 PDFAgent-0.1.1/PDFAgent/
+-rw-r--r--   0 jackywong   (501) staff       (20)       56 2023-07-24 03:43:47.000000 PDFAgent-0.1.1/PDFAgent/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1967 2023-07-28 14:28:51.000000 PDFAgent-0.1.1/PDFAgent/agent.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.807212 PDFAgent-0.1.1/PDFAgent.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      244 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-28 14:31:07.000000 PDFAgent-0.1.1/PDFAgent.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)      206 2023-07-28 14:31:07.808227 PDFAgent-0.1.1/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     2316 2023-07-28 14:24:33.000000 PDFAgent-0.1.1/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-28 14:31:07.808633 PDFAgent-0.1.1/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      328 2023-07-28 14:29:24.000000 PDFAgent-0.1.1/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-28 14:31:07.807516 PDFAgent-0.1.1/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)       46 2023-07-24 04:27:34.000000 PDFAgent-0.1.1/tests/test_basic.py
```

### Comparing `PDFAgent-0.1.0/LICENSE` & `PDFAgent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PDFAgent-0.1.0/PDFAgent/agent.py` & `PDFAgent-0.1.1/PDFAgent/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         ):
         self.api_key = api_key
         self.base_url = base_url if base_url else "https://app.twilix.io/api/v1"
         self.client: Client = Client(api_key)
         self.name = name
         self.collection = self.client.Collection(name)
 
-    def insert_pdf(self, url: str):
+    def read_pdf(self, url: str):
         """Inserting a PDF via URL.
         """
         result = self.collection.insert_pdf(url)
         print("Inserting PDF... Please wait 30-60 seconds for this to finish indexing.")
         return result
     
     def ask(self, question: str, conversation_id: str=None):
@@ -27,21 +27,33 @@
         """
         return self.collection.generative_qa(
             prompt=question,
             prompt_fields=None,
             conversation_id=conversation_id
         )
 
-    def template(self, prompt: str, conversation_id: str=None):
+    def template(
+        self, 
+        prompt: str, 
+        conversation_id: str=None,
+        limit: int=5, 
+        minimum_rerank_score: float=0.05,
+        include_moderation: bool=False, 
+    ):
         """Use a template to analyze how your PDF
         """
         return self.collection.template(
             prompt=prompt,
             prompt_fields=["autoGen_content"],
-            conversation_id=conversation_id
+            fields=["autoGen_content"],
+            conversation_id=conversation_id,
+            limit=limit,
+            include_rerank=True,
+            minimum_rerank_score=minimum_rerank_score,
+            include_moderation=include_moderation
         )
 
     def copilot(self, prompt: str, conversation_id: str=None):
         """The endpoint for advanced analysis
         """
         return self.collection.copilot(
             prompt=prompt,
```

### Comparing `PDFAgent-0.1.0/README.md` & `PDFAgent-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # PDFAgent
 
 A production-ready PDF agent for reading, analysing and conversing with your PDF built for business-critical use cases on retrieval-augmented generation.
 
 Got questions/need support? Join our discord here: https://discord.gg/a3K9c8GRGt
 
+![Code Example](assets/examplecode.png)
+
 # Features
 
 ✅ Production-ready PDFReaderAgent - built with Rest API (see docs.twilix.io for more information)  
 ✅ Built-in observability (via Twilix dashboard)  
 ✅ Built-in easily swappable read/write API keys (so no one can over-write your data)  
 ✅ Production-ready insertion and retrieval pipelines built in (via Twilix)  
 ✅ Multi-line citations, managed vector store, production-ready conversation memory handling.
@@ -28,21 +30,21 @@
 from PDFAgent import PDFAgent
 agent = PDFAgent(
     name="AgentExample",
     api_key="XXX"
 )
 ```
 
-### Inserting a PDF 
+### Reading a PDF 
 
-You can insert a PDF in just 1 line of code - under the hood, we take care of OCR, preprocessing,
+You can read a PDF in just 1 line of code - under the hood, we take care of OCR, preprocessing,
 vectorising, splitting and storage.
 
 ```python
-agent.insert_pdf(
+agent.read_pdf(
     "https://www.w3.org/WAI/WCAG21/working-examples/pdf-table/table.pdf"
 )
 ```
 
 Once it's inserted, we recommend giving it 30 to 60 seconds to properly index.
 
 If you have a local, PDF, we recommend uploading and inserting via
```

