# Comparing `tmp/readmedocs_fetcher_haystack-0.0.1.tar.gz` & `tmp/readmedocs_fetcher_haystack-0.0.2.tar.gz`

## Comparing `readmedocs_fetcher_haystack-0.0.1.tar` & `readmedocs_fetcher_haystack-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/examples/readmedocs_indexing.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/src/readmedocs_fetcher_haystack/__about__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/src/readmedocs_fetcher_haystack/__init__.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/src/readmedocs_fetcher_haystack/readmedocs_fetcher.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/README.md
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/examples/readmedocs_indexing.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/src/readmedocs_fetcher_haystack/__about__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/src/readmedocs_fetcher_haystack/__init__.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/src/readmedocs_fetcher_haystack/readmedocs_fetcher.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/README.md
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 readmedocs_fetcher_haystack-0.0.2/PKG-INFO
```

### Comparing `readmedocs_fetcher_haystack-0.0.1/examples/readmedocs_indexing.py` & `readmedocs_fetcher_haystack-0.0.2/examples/readmedocs_indexing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from readmedocs_fetcher_haystack.readmedocs_fetcher import ReadmeDocsFetcher
+from readmedocs_fetcher_haystack import ReadmeDocsFetcher
 import os
 from dotenv import load_dotenv
 from haystack import Pipeline
 from haystack.nodes import MarkdownConverter, PreProcessor
 from haystack.document_stores import InMemoryDocumentStore
 load_dotenv()
 README_API_KEY = os.getenv('README_API_KEY')
 
 converter = MarkdownConverter(remove_code_snippets=False)
-readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter)
+readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter, base_url="https://docs.haystack.deepset.ai")
 
 preprocessor = PreProcessor()
 doc_store = InMemoryDocumentStore()
+doc_store.delete_documents()
 
 pipe = Pipeline()
 pipe.add_node(component=readme_fetcher, name="ReadmeFetcher", inputs=["File"])
 pipe.add_node(component=preprocessor, name="Preprocessor", inputs=["ReadmeFetcher"])
 pipe.add_node(component=doc_store, name="DocumentStore", inputs=["Preprocessor"])
-pipe.run(params={"ReadmeFetcher":{"slug": "nodes_overview"}})
-
-print(doc_store.get_document_count())
+pipe.run(params={"ReadmeFetcher":{"slugs": ["nodes_overview"]}})
```

### Comparing `readmedocs_fetcher_haystack-0.0.1/src/readmedocs_fetcher_haystack/readmedocs_fetcher.py` & `readmedocs_fetcher_haystack-0.0.2/src/readmedocs_fetcher_haystack/readmedocs_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,51 +20,55 @@
         def readme_token(self):
             if not self.api_key:
                 raise Exception("Please provide a Readem API Key")
             api_key = f"{self.api_key}"
             return base64.b64encode(api_key.encode("utf-8")).decode("utf-8")
         
     
-    def __init__(self, api_key: str, markdown_converter: Optional[MarkdownConverter] = None):
+    def __init__(self, api_key: str, base_url: Optional[str] = None, markdown_converter: Optional[MarkdownConverter] = None):
         self.api_key = api_key
         self.auth = self.ReadmeAuth(api_key=self.api_key)
+        self.base_url = base_url
         if markdown_converter is None:
             self.markdown_converter = MarkdownConverter()
         else:
             self.markdown_converter = markdown_converter
     
-    def run(self, slug: Optional[str]= None, version: Optional[str] = None):
-        documents = self.fetch_docs(slug=slug, version=version)
+    def run(self, slugs: Optional[List[str]] = None, version: Optional[str] = None):
+        documents = self.fetch_docs(base_url = self.base_url, slugs=slugs, version=version)
         outputs = {"documents": documents}
         return outputs, "output_1"
     
-    def fetch_docs(self, slug: Optional[str]= None, version: Optional[str] = None) -> List[Document]:
+    def fetch_docs(self, base_url: Optional[str] = None, slugs: Optional[List[str]]= None, version: Optional[str] = None) -> List[Document]:
         if version is None:
             version = self.get_stable_version()
         categories = self.get_categories_slugs(version)
         available_slugs = []
         for c in categories:
             available_slugs.extend(self.get_category_docs_slugs(c, version))
         docs = []
-        if slug != None:
-            if slug not in available_slugs:
+        if slugs != None:
+            if not all(item in available_slugs for item in slugs):
                 raise Exception("Please provide a document slug that exists in your readme docs")
             else:
-                docs = [slug]
+                docs = slugs
         else:
             docs = available_slugs
 
         bodies = {d: self.get_doc_markdown(d, version) for d in docs}
         documents = []
         with tempfile.TemporaryDirectory() as temp_dir:
             for slug, body in bodies.items():
                 temp_file_path = os.path.join(temp_dir, f"{slug}.md")
                 with open(temp_file_path, 'w') as temp_file:
                     temp_file.write(body)
-                documents.extend(self.markdown_converter.convert(file_path=temp_file_path, meta={"version": version, "name": slug}))
+                meta = {"version": version, "name": slug}
+                if base_url is not None:
+                    meta["url"] = base_url + f"/docs/{slug}"
+                documents.extend(self.markdown_converter.convert(file_path=temp_file_path, meta=meta))
         return documents
     
     def run_batch(self, query: str, version: Optional[str]):
        pass
 
     def get_categories_slugs(self, version: str) -> List[str]:
         """
```

### Comparing `readmedocs_fetcher_haystack-0.0.1/.gitignore` & `readmedocs_fetcher_haystack-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `readmedocs_fetcher_haystack-0.0.1/LICENSE.txt` & `readmedocs_fetcher_haystack-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `readmedocs_fetcher_haystack-0.0.1/README.md` & `readmedocs_fetcher_haystack-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,58 +9,62 @@
 ```bash
 pip install readmedocs-fetcher-haystack
 ```
 
 ## Usage in Haystack
 
 1. To initialize a `ReadmeDocsFetcher` you have to provide an `api_key` paramter. This is your ReadMe Docs API Key.
-2. There are 3 optional parameters to initialize the `ReadmeDocsFetcher`
-    - `slug`: To fetch a single defined page from your documentation. E.g. if you have want to fetch 'https://docs.haystack.deepset.ai/docs/installation' the slug would be `installation`. If not set, all of the available pages will be fetched.
+2. There are also 4 optional parameters to initialize the `ReadmeDocsFetcher`
+    - `slugs`: To fetch a list of specific pages from your documentation. E.g. if you have want to fetch 'https://docs.haystack.deepset.ai/docs/installation' the slug would be `installation`. If not set, all of the available pages will be fetched.
+    - `base_url`: Optionally provide this to add the full url of a documentation page to the `meta` of the created document. For example `base_url='https://docs.haystack.deepset.ai'"`
     - `version`: If not set, the latest stable version of tour docs will be fethed. 
     - `markdown_converter`: When documents are fetched from ReadMe, temporary `.md` files are created and we use a [`MakrdownConverter`](https://docs.haystack.deepset.ai/reference/file-converters-api#markdownconverter) to create a list of haystack `Documents`. If not provided at initialization, the a `MarkdownConverter` with the default parameters is used.
 
 ### Standalone
 ```python
 import os
 from dotenv import load_dotenv
 from haystack.nodes import MarkdownConverter
+from readmedocs_fetcher_haystack import ReadmeDocsFetcher
 
 load_dotenv()
 README_API_KEY = os.getenv('README_API_KEY')
 
 converter = MarkdownConverter(remove_code_snippets=False)
-readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter)
+readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter, base_url="https://docs.haystack.deepset.ai")
 readme_fetcher.fetch_docs()
 ```
 
 To fetch a single doc from a specific version:
 ```python
-readme_fetcher.fetch_docs(slug="nodes_overview", version="v1.18")
+readme_fetcher.fetch_docs(slugs=["nodes_overview"], version="v1.18")
 ```
 ### In a Pipeline
 
 ```python
 import os
 from dotenv import load_dotenv
 from haystack import Pipeline
 from haystack.nodes import MarkdownConverter, PreProcessor
 from haystack.document_stores import InMemoryDocumentStore
+from readmedocs_fetcher_haystack import ReadmeDocsFetcher
+
 load_dotenv()
 README_API_KEY = os.getenv('README_API_KEY')
 
 converter = MarkdownConverter(remove_code_snippets=False)
-readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter)
+readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter, base_url="https://docs.haystack.deepset.ai")
 
 preprocessor = PreProcessor()
 doc_store = InMemoryDocumentStore()
 
 pipe = Pipeline()
 pipe.add_node(component=readme_fetcher, name="ReadmeFetcher", inputs=["File"])
 pipe.add_node(component=preprocessor, name="Preprocessor", inputs=["ReadmeFetcher"])
 pipe.add_node(component=doc_store, name="DocumentStore", inputs=["Preprocessor"])
 pipe.run()
 ```
 
 To fetch a single documentation page:
 ```python
-pipe.run(params={"ReadmeFetcher":{"slug": "nodes_overview"}})
+pipe.run(params={"ReadmeFetcher":{"slugs": ["nodes_overview"]}})
 ```
```

### Comparing `readmedocs_fetcher_haystack-0.0.1/pyproject.toml` & `readmedocs_fetcher_haystack-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readmedocs_fetcher_haystack-0.0.1/PKG-INFO` & `readmedocs_fetcher_haystack-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmedocs-fetcher-haystack
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/readmedocs-fetcher-haystack#readme
 Project-URL: Issues, https://github.com/unknown/readmedocs-fetcher-haystack/issues
 Project-URL: Source, https://github.com/unknown/readmedocs-fetcher-haystack
 Author-email: Tuana Celik <tuana.celik@deepset.ai>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -31,58 +31,62 @@
 ```bash
 pip install readmedocs-fetcher-haystack
 ```
 
 ## Usage in Haystack
 
 1. To initialize a `ReadmeDocsFetcher` you have to provide an `api_key` paramter. This is your ReadMe Docs API Key.
-2. There are 3 optional parameters to initialize the `ReadmeDocsFetcher`
-    - `slug`: To fetch a single defined page from your documentation. E.g. if you have want to fetch 'https://docs.haystack.deepset.ai/docs/installation' the slug would be `installation`. If not set, all of the available pages will be fetched.
+2. There are also 4 optional parameters to initialize the `ReadmeDocsFetcher`
+    - `slugs`: To fetch a list of specific pages from your documentation. E.g. if you have want to fetch 'https://docs.haystack.deepset.ai/docs/installation' the slug would be `installation`. If not set, all of the available pages will be fetched.
+    - `base_url`: Optionally provide this to add the full url of a documentation page to the `meta` of the created document. For example `base_url='https://docs.haystack.deepset.ai'"`
     - `version`: If not set, the latest stable version of tour docs will be fethed. 
     - `markdown_converter`: When documents are fetched from ReadMe, temporary `.md` files are created and we use a [`MakrdownConverter`](https://docs.haystack.deepset.ai/reference/file-converters-api#markdownconverter) to create a list of haystack `Documents`. If not provided at initialization, the a `MarkdownConverter` with the default parameters is used.
 
 ### Standalone
 ```python
 import os
 from dotenv import load_dotenv
 from haystack.nodes import MarkdownConverter
+from readmedocs_fetcher_haystack import ReadmeDocsFetcher
 
 load_dotenv()
 README_API_KEY = os.getenv('README_API_KEY')
 
 converter = MarkdownConverter(remove_code_snippets=False)
-readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter)
+readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter, base_url="https://docs.haystack.deepset.ai")
 readme_fetcher.fetch_docs()
 ```
 
 To fetch a single doc from a specific version:
 ```python
-readme_fetcher.fetch_docs(slug="nodes_overview", version="v1.18")
+readme_fetcher.fetch_docs(slugs=["nodes_overview"], version="v1.18")
 ```
 ### In a Pipeline
 
 ```python
 import os
 from dotenv import load_dotenv
 from haystack import Pipeline
 from haystack.nodes import MarkdownConverter, PreProcessor
 from haystack.document_stores import InMemoryDocumentStore
+from readmedocs_fetcher_haystack import ReadmeDocsFetcher
+
 load_dotenv()
 README_API_KEY = os.getenv('README_API_KEY')
 
 converter = MarkdownConverter(remove_code_snippets=False)
-readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter)
+readme_fetcher = ReadmeDocsFetcher(api_key=README_API_KEY, markdown_converter=converter, base_url="https://docs.haystack.deepset.ai")
 
 preprocessor = PreProcessor()
 doc_store = InMemoryDocumentStore()
 
 pipe = Pipeline()
 pipe.add_node(component=readme_fetcher, name="ReadmeFetcher", inputs=["File"])
 pipe.add_node(component=preprocessor, name="Preprocessor", inputs=["ReadmeFetcher"])
 pipe.add_node(component=doc_store, name="DocumentStore", inputs=["Preprocessor"])
 pipe.run()
 ```
 
 To fetch a single documentation page:
 ```python
-pipe.run(params={"ReadmeFetcher":{"slug": "nodes_overview"}})
+pipe.run(params={"ReadmeFetcher":{"slugs": ["nodes_overview"]}})
 ```
```

