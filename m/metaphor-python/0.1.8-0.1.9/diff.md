# Comparing `tmp/metaphor-python-0.1.8.tar.gz` & `tmp/metaphor-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.8.tar", last modified: Fri Jul 28 03:10:18 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.9.tar", last modified: Fri Jul 28 03:12:56 2023, max compression
```

## Comparing `metaphor-python-0.1.8.tar` & `metaphor-python-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.530148 metaphor-python-0.1.8/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:10:18.530006 metaphor-python-0.1.8/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)     1136 2023-07-28 03:06:33.000000 metaphor-python-0.1.8/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.529193 metaphor-python-0.1.8/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      113 2023-07-25 20:46:42.000000 metaphor-python-0.1.8/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     4875 2023-07-28 03:10:04.000000 metaphor-python-0.1.8/metaphor_python/api.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:10:18.529816 metaphor-python-0.1.8/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-28 03:10:18.000000 metaphor-python-0.1.8/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-28 03:10:18.530185 metaphor-python-0.1.8/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-28 03:09:42.000000 metaphor-python-0.1.8/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:12:56.279785 metaphor-python-0.1.9/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:12:56.279638 metaphor-python-0.1.9/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     1136 2023-07-28 03:06:33.000000 metaphor-python-0.1.9/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:12:56.278629 metaphor-python-0.1.9/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      113 2023-07-25 20:46:42.000000 metaphor-python-0.1.9/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     4882 2023-07-28 03:12:33.000000 metaphor-python-0.1.9/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-28 03:12:56.279457 metaphor-python-0.1.9/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-28 03:12:56.000000 metaphor-python-0.1.9/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-28 03:12:56.000000 metaphor-python-0.1.9/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-28 03:12:56.000000 metaphor-python-0.1.9/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-28 03:12:56.000000 metaphor-python-0.1.9/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-28 03:12:56.000000 metaphor-python-0.1.9/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-28 03:12:56.279828 metaphor-python-0.1.9/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-28 03:12:47.000000 metaphor-python-0.1.9/setup.py
```

### Comparing `metaphor-python-0.1.8/PKG-INFO` & `metaphor-python-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.8/README.md` & `metaphor-python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `metaphor-python-0.1.8/metaphor_python/api.py` & `metaphor-python-0.1.9/metaphor_python/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         if not isinstance(value, VALID_FIND_SIMILAR_OPTIONS[key]):
             raise ValueError(f"Invalid type for option '{key}': Expected {VALID_FIND_SIMILAR_OPTIONS[key]}, got {type(value)}")
 
 @dataclass
 class Result:
     title: str
     url: str
-    score: Optional[float]
     id: str
+    score: Optional[float] = None
     published_date: Optional[str] = None
     author: Optional[str] = None
     extract: Optional[str] = None # beta field. returned when findSimilar_and_get_contents is called
 
     def __init__(self, title, url, score, id, published_date=None, author=None, **kwargs):
         self.title = title
         self.url = url
```

### Comparing `metaphor-python-0.1.8/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.9/metaphor_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.8/setup.py` & `metaphor-python-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metaphor-python',
-    version='0.1.8',
+    version='0.1.9',
     description='A Python package for the Metaphor API.',
     author='Metaphor',
     author_email='hello@metaphor.systems',
     url='https://github.com/metaphorsystems/metaphor-python',
     packages=find_packages(),
     install_requires=[
         'requests',
```

