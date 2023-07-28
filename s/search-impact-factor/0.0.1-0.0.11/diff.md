# Comparing `tmp/search_impact_factor-0.0.1.tar.gz` & `tmp/search_impact_factor-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_impact_factor-0.0.1.tar", last modified: Fri Jul 28 01:13:59 2023, max compression
+gzip compressed data, was "search_impact_factor-0.0.11.tar", last modified: Fri Jul 28 02:01:02 2023, max compression
```

## Comparing `search_impact_factor-0.0.1.tar` & `search_impact_factor-0.0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 01:13:59.908499 search_impact_factor-0.0.1/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1074 2023-07-26 18:27:09.000000 search_impact_factor-0.0.1/LICENSE
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       89 2023-07-26 20:45:37.000000 search_impact_factor-0.0.1/MANIFEST.in
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1676 2023-07-28 01:13:59.908345 search_impact_factor-0.0.1/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)      909 2023-07-28 00:58:15.000000 search_impact_factor-0.0.1/README.md
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 01:13:59.907230 search_impact_factor-0.0.1/search_impact_factor/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)  1825415 2023-07-26 20:50:54.000000 search_impact_factor-0.0.1/search_impact_factor/2022_JCR_IF.csv
--rw-r--r--   0 brritanyhuang   (501) staff       (20)  2032307 2023-07-26 21:21:51.000000 search_impact_factor-0.0.1/search_impact_factor/2023_JCR_IF.csv
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2023-07-26 17:50:23.000000 search_impact_factor-0.0.1/search_impact_factor/__init__.py
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1775 2023-07-28 00:54:26.000000 search_impact_factor-0.0.1/search_impact_factor/search_impact_factor.py
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 01:13:59.908177 search_impact_factor-0.0.1/search_impact_factor.egg-info/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1676 2023-07-28 01:13:59.000000 search_impact_factor-0.0.1/search_impact_factor.egg-info/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)      409 2023-07-28 01:13:59.000000 search_impact_factor-0.0.1/search_impact_factor.egg-info/SOURCES.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2023-07-28 01:13:59.000000 search_impact_factor-0.0.1/search_impact_factor.egg-info/dependency_links.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        7 2023-07-28 01:13:59.000000 search_impact_factor-0.0.1/search_impact_factor.egg-info/requires.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       21 2023-07-28 01:13:59.000000 search_impact_factor-0.0.1/search_impact_factor.egg-info/top_level.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2023-07-28 01:13:59.908543 search_impact_factor-0.0.1/setup.cfg
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1049 2023-07-28 01:13:13.000000 search_impact_factor-0.0.1/setup.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 02:01:02.292269 search_impact_factor-0.0.11/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2023-07-28 01:33:01.000000 search_impact_factor-0.0.11/LICENSE
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       89 2023-07-26 20:45:37.000000 search_impact_factor-0.0.11/MANIFEST.in
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1864 2023-07-28 02:01:02.292112 search_impact_factor-0.0.11/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)      958 2023-07-28 01:54:05.000000 search_impact_factor-0.0.11/README.md
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 02:01:02.290774 search_impact_factor-0.0.11/search_impact_factor/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)  1825415 2023-07-26 20:50:54.000000 search_impact_factor-0.0.11/search_impact_factor/2022_JCR_IF.csv
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)  2032307 2023-07-26 21:21:51.000000 search_impact_factor-0.0.11/search_impact_factor/2023_JCR_IF.csv
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2023-07-26 17:50:23.000000 search_impact_factor-0.0.11/search_impact_factor/__init__.py
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1775 2023-07-28 00:54:26.000000 search_impact_factor-0.0.11/search_impact_factor/search_impact_factor.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2023-07-28 02:01:02.291917 search_impact_factor-0.0.11/search_impact_factor.egg-info/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1864 2023-07-28 02:01:01.000000 search_impact_factor-0.0.11/search_impact_factor.egg-info/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)      409 2023-07-28 02:01:02.000000 search_impact_factor-0.0.11/search_impact_factor.egg-info/SOURCES.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2023-07-28 02:01:01.000000 search_impact_factor-0.0.11/search_impact_factor.egg-info/dependency_links.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        7 2023-07-28 02:01:02.000000 search_impact_factor-0.0.11/search_impact_factor.egg-info/requires.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       21 2023-07-28 02:01:02.000000 search_impact_factor-0.0.11/search_impact_factor.egg-info/top_level.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2023-07-28 02:01:02.292324 search_impact_factor-0.0.11/setup.cfg
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1214 2023-07-28 01:54:25.000000 search_impact_factor-0.0.11/setup.py
```

### Comparing `search_impact_factor-0.0.1/LICENSE` & `search_impact_factor-0.0.11/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2023] [YongZhen,Huang]
+Copyright (c) 2023 Yong-Zhen Huang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `search_impact_factor-0.0.1/PKG-INFO` & `search_impact_factor-0.0.11/search_impact_factor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: search_impact_factor
-Version: 0.0.1
+Name: search-impact-factor
+Version: 0.0.11
 Summary: A package to query the impact factor database
+Home-page: https://github.com/Brritany/search_impact_factor
 Author: hyz
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
+Project-URL: Tracker, https://github.com/Brritany/search_impact_factor/issues
 Keywords: python,impact factor,IF
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Topic :: Software Development :: Libraries
@@ -17,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Search Impact Factor
 
-這個 Python 包提供了查詢 2023 年 Impact Factor 的功能
+這個 Python 包提供了查詢 2023, 2022 年 Impact Factor 的功能
 
 ## Use `pip` to install package
 
 ```bash
 pip install search-impact-factor
 ```
 
@@ -55,10 +57,11 @@
 query_result_df = sif.query_if_score(min_score, max_score)
 
 query_result_df.head()
 ```
 
 ### Update log
 
-`0.0.1` first edition
+`0.0.11` Add GitHub link, re-do README.md
+`0.0.1`  First edition
```

### Comparing `search_impact_factor-0.0.1/README.md` & `search_impact_factor-0.0.11/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Search Impact Factor
 
-這個 Python 包提供了查詢 2023 年 Impact Factor 的功能
+這個 Python 包提供了查詢 2023, 2022 年 Impact Factor 的功能
 
 ## Use `pip` to install package
 
 ```bash
 pip install search-impact-factor
 ```
 
@@ -34,8 +34,9 @@
 query_result_df = sif.query_if_score(min_score, max_score)
 
 query_result_df.head()
 ```
 
 ### Update log
 
-`0.0.1` first edition
+`0.0.11` Add GitHub link, re-do README.md
+`0.0.1`  First edition
```

### Comparing `search_impact_factor-0.0.1/search_impact_factor/2022_JCR_IF.csv` & `search_impact_factor-0.0.11/search_impact_factor/2022_JCR_IF.csv`

 * *Files identical despite different names*

### Comparing `search_impact_factor-0.0.1/search_impact_factor/2023_JCR_IF.csv` & `search_impact_factor-0.0.11/search_impact_factor/2023_JCR_IF.csv`

 * *Files identical despite different names*

### Comparing `search_impact_factor-0.0.1/search_impact_factor/search_impact_factor.py` & `search_impact_factor-0.0.11/search_impact_factor/search_impact_factor.py`

 * *Files identical despite different names*

### Comparing `search_impact_factor-0.0.1/search_impact_factor.egg-info/PKG-INFO` & `search_impact_factor-0.0.11/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: search-impact-factor
-Version: 0.0.1
+Name: search_impact_factor
+Version: 0.0.11
 Summary: A package to query the impact factor database
+Home-page: https://github.com/Brritany/search_impact_factor
 Author: hyz
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
+Project-URL: Tracker, https://github.com/Brritany/search_impact_factor/issues
 Keywords: python,impact factor,IF
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Topic :: Software Development :: Libraries
@@ -17,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Search Impact Factor
 
-這個 Python 包提供了查詢 2023 年 Impact Factor 的功能
+這個 Python 包提供了查詢 2023, 2022 年 Impact Factor 的功能
 
 ## Use `pip` to install package
 
 ```bash
 pip install search-impact-factor
 ```
 
@@ -55,10 +57,11 @@
 query_result_df = sif.query_if_score(min_score, max_score)
 
 query_result_df.head()
 ```
 
 ### Update log
 
-`0.0.1` first edition
+`0.0.11` Add GitHub link, re-do README.md
+`0.0.1`  First edition
```

### Comparing `search_impact_factor-0.0.1/setup.py` & `search_impact_factor-0.0.11/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="search_impact_factor",
-    version="0.0.1",
+    version="0.0.11",
     description="A package to query the impact factor database",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    url='https://github.com/Brritany/search_impact_factor',
+    project_urls={
+        'Tracker': 'https://github.com/Brritany/search_impact_factor/issues',
+    },
     author="hyz",
     author_email="m946111005@tmu.edu.tw",
     packages=find_packages(),
     keywords=['python', 'impact factor', 'IF'],
     install_requires=[
         "pandas",
     ],
```

