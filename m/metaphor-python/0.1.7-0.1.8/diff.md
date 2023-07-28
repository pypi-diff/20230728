# Comparing `tmp/metaphor-python-0.1.7.tar.gz` & `tmp/metaphor-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.7.tar", last modified: Tue Jul 25 20:49:50 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.8.tar", last modified: Fri Jul 28 03:10:18 2023, max compression
```

## Comparing `metaphor-python-0.1.7.tar` & `metaphor-python-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.103162 metaphor-python-0.1.7/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 20:49:50.103012 metaphor-python-0.1.7/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.7/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.102177 metaphor-python-0.1.7/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      113 2023-07-25 20:46:42.000000 metaphor-python-0.1.7/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     4865 2023-07-25 20:46:59.000000 metaphor-python-0.1.7/metaphor_python/api.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 20:49:50.102831 metaphor-python-0.1.7/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 20:49:50.000000 metaphor-python-0.1.7/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 20:49:50.103203 metaphor-python-0.1.7/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 20:49:38.000000 metaphor-python-0.1.7/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.530148 metaphor-python-0.1.8/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:10:18.530006 metaphor-python-0.1.8/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     1136 2023-07-28 03:06:33.000000 metaphor-python-0.1.8/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.529193 metaphor-python-0.1.8/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      113 2023-07-25 20:46:42.000000 metaphor-python-0.1.8/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     4875 2023-07-28 03:10:04.000000 metaphor-python-0.1.8/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.529816 metaphor-python-0.1.8/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-28 03:10:18.530185 metaphor-python-0.1.8/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-28 03:09:42.000000 metaphor-python-0.1.8/setup.py
```

### Comparing `metaphor-python-0.1.7/PKG-INFO` & `metaphor-python-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.7/README.md` & `metaphor-python-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,47 +16,39 @@
 ```python
 from metaphor_python import Metaphor
 
 client = Metaphor(api_key="your-api-key")
 ```
 
 ## Search Request
-You can perform a search by creating a SearchRequest object and passing it to the search method:
-
 ```python
-from metaphor_python import SearchRequest
 
-request = SearchRequest(query="Here is a reaully interesting AI company:", num_results=5)
-response = client.search(request)
+response = client.search("funny article about tech culture",
+    num_results=5,
+    includeDomains: ["nytimes.com", "wsj.com"],
+    startPublishedDate: "2023-06-12"
+)
 
 for result in response.results:
     print(result.title, result.url)
 ```
 
 ## Find Similar
-To find documents similar to a given URL, you can use the FindSimilarRequest object:
 
 ```python
-from metaphor_python import FindSimilarRequest
-
-request = FindSimilarRequest(url="https://example.com/article", num_results=5)
-response = client.find_similar(request)
+response = client.find_similar("https://waitbutwhy.com/2014/05/fermi-paradox.html", num_results=5)
 
 for result in response.results:
     print(result.title, result.url)
 ```
 
 ## Retrieve Document Contents
-To retrieve the contents of documents, use the GetContentsRequest object:
-
-from metaphor_python import GetContentsRequest
-
 ```python
-request = GetContentsRequest(ids=["doc1", "doc2"])
-response = client.get_contents(request)
+ids = ["8U71IlQ5DUTdsZFherhhYA", "X3wd0PbJmAvhu_DQjDKA7A"]
+response = client.get_contents(ids)
 
 for content in response.contents:
     print(content.title, content.url)
 ```
 
 # Contribution
 Contributions to metaphor-python are very welcome! Feel free to submit pull requests or raise issues.
```

### Comparing `metaphor-python-0.1.7/metaphor_python/api.py` & `metaphor-python-0.1.8/metaphor_python/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if not isinstance(value, VALID_FIND_SIMILAR_OPTIONS[key]):
             raise ValueError(f"Invalid type for option '{key}': Expected {VALID_FIND_SIMILAR_OPTIONS[key]}, got {type(value)}")
 
 @dataclass
 class Result:
     title: str
     url: str
-    score: float
+    score: Optional[float]
     id: str
     published_date: Optional[str] = None
     author: Optional[str] = None
     extract: Optional[str] = None # beta field. returned when findSimilar_and_get_contents is called
 
     def __init__(self, title, url, score, id, published_date=None, author=None, **kwargs):
         self.title = title
```

### Comparing `metaphor-python-0.1.7/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.8/metaphor_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.7/setup.py` & `metaphor-python-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metaphor-python',
-    version='0.1.7',
+    version='0.1.8',
     description='A Python package for the Metaphor API.',
     author='Metaphor',
     author_email='hello@metaphor.systems',
     url='https://github.com/metaphorsystems/metaphor-python',
     packages=find_packages(),
     install_requires=[
         'requests',
```

