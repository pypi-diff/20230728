# Comparing `tmp/html_content_extractor-0.0.1.tar.gz` & `tmp/html_content_extractor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_content_extractor-0.0.1.tar", last modified: Fri Jul 28 02:08:45 2023, max compression
+gzip compressed data, was "html_content_extractor-0.0.2.tar", last modified: Fri Jul 28 19:04:58 2023, max compression
```

## Comparing `html_content_extractor-0.0.1.tar` & `html_content_extractor-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 02:08:45.913220 html_content_extractor-0.0.1/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    11357 2023-07-28 01:26:01.000000 html_content_extractor-0.0.1/LICENSE
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    14182 2023-07-28 02:08:45.913220 html_content_extractor-0.0.1/PKG-INFO
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      619 2023-07-28 01:32:36.000000 html_content_extractor-0.0.1/README.md
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 02:08:45.913220 html_content_extractor-0.0.1/html_content_extractor/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       39 2023-07-28 01:33:04.000000 html_content_extractor-0.0.1/html_content_extractor/__init__.py
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       62 2023-07-28 01:33:19.000000 html_content_extractor-0.0.1/html_content_extractor/extractor.py
-drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 02:08:45.913220 html_content_extractor-0.0.1/html_content_extractor.egg-info/
--rw-rw-r--   0 kevins    (1000) kevins    (1000)    14182 2023-07-28 02:08:45.000000 html_content_extractor-0.0.1/html_content_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      332 2023-07-28 02:08:45.000000 html_content_extractor-0.0.1/html_content_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)        1 2023-07-28 02:08:45.000000 html_content_extractor-0.0.1/html_content_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       43 2023-07-28 02:08:45.000000 html_content_extractor-0.0.1/html_content_extractor.egg-info/requires.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       23 2023-07-28 02:08:45.000000 html_content_extractor-0.0.1/html_content_extractor.egg-info/top_level.txt
--rw-rw-r--   0 kevins    (1000) kevins    (1000)      760 2023-07-28 01:57:11.000000 html_content_extractor-0.0.1/pyproject.toml
--rw-rw-r--   0 kevins    (1000) kevins    (1000)       38 2023-07-28 02:08:45.913220 html_content_extractor-0.0.1/setup.cfg
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.132373 html_content_extractor-0.0.2/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    11357 2023-07-28 01:26:01.000000 html_content_extractor-0.0.2/LICENSE
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    14480 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/PKG-INFO
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      806 2023-07-28 02:45:22.000000 html_content_extractor-0.0.2/README.md
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/html_content_extractor/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       39 2023-07-28 01:33:04.000000 html_content_extractor-0.0.2/html_content_extractor/__init__.py
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)     2358 2023-07-28 02:50:58.000000 html_content_extractor-0.0.2/html_content_extractor/extractor.py
+drwxrwxr-x   0 kevins    (1000) kevins    (1000)        0 2023-07-28 19:04:58.128373 html_content_extractor-0.0.2/html_content_extractor.egg-info/
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)    14480 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      332 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)        1 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       43 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/requires.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       23 2023-07-28 19:04:58.000000 html_content_extractor-0.0.2/html_content_extractor.egg-info/top_level.txt
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)      858 2023-07-28 03:18:05.000000 html_content_extractor-0.0.2/pyproject.toml
+-rw-rw-r--   0 kevins    (1000) kevins    (1000)       38 2023-07-28 19:04:58.132373 html_content_extractor-0.0.2/setup.cfg
```

### Comparing `html_content_extractor-0.0.1/LICENSE` & `html_content_extractor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `html_content_extractor-0.0.1/PKG-INFO` & `html_content_extractor-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_content_extractor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to extract the main content from HTML documents
 Author-email: Kevin Sparks <pip@just-digital.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,31 +203,33 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/just-digital/html-content-extractor
 Project-URL: Bug Tracker, https://github.com/just-digital/html-content-extractor/issues
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # html-content-extractor
 
 This Python package provides a function to extract the "main content" from HTML documents.
 
 ## Installation
 
 You can install this package via pip:
 
 ```sh
-pip install html-content-extractor
+$ pip install html-content-extractor
 
 ```
 
 ## Usage
 
 ```python
 from html_content_extractor import extract_content
@@ -237,7 +239,21 @@
 >>> print(content)
 "An HTML Page\n\nThis is some HTML content."
 
 >>> markdown = extract_content(html, format='markdown')
 >>> print(content)
 "# An HTML Page\n\nThis is some HTML content."
 ```
+
+## Build
+
+```sh
+$ python3 -m pip install --upgrade build
+$ python3 -m build
+```
+
+# Publish to PyPI
+
+```sh
+$ python3 -m pip install --upgrade twine
+$ python3 -m twine upload dist/*
+```
```

### Comparing `html_content_extractor-0.0.1/html_content_extractor.egg-info/PKG-INFO` & `html_content_extractor-0.0.2/html_content_extractor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-content-extractor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package to extract the main content from HTML documents
 Author-email: Kevin Sparks <pip@just-digital.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -203,31 +203,33 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/just-digital/html-content-extractor
 Project-URL: Bug Tracker, https://github.com/just-digital/html-content-extractor/issues
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # html-content-extractor
 
 This Python package provides a function to extract the "main content" from HTML documents.
 
 ## Installation
 
 You can install this package via pip:
 
 ```sh
-pip install html-content-extractor
+$ pip install html-content-extractor
 
 ```
 
 ## Usage
 
 ```python
 from html_content_extractor import extract_content
@@ -237,7 +239,21 @@
 >>> print(content)
 "An HTML Page\n\nThis is some HTML content."
 
 >>> markdown = extract_content(html, format='markdown')
 >>> print(content)
 "# An HTML Page\n\nThis is some HTML content."
 ```
+
+## Build
+
+```sh
+$ python3 -m pip install --upgrade build
+$ python3 -m build
+```
+
+# Publish to PyPI
+
+```sh
+$ python3 -m pip install --upgrade twine
+$ python3 -m twine upload dist/*
+```
```

### Comparing `html_content_extractor-0.0.1/pyproject.toml` & `html_content_extractor-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "html_content_extractor"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kevin Sparks", email="pip@just-digital.net" },
 ]
 description = "A Python package to extract the main content from HTML documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
+    "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
+    "Topic :: Text Processing :: Markup :: HTML"
 ]
 license.file = "LICENSE"
 dependencies = [
   "beautifulsoup4>=4.12.2",
   "markdownify==0.11.6"
 ]
 
-
 [project.urls]
 "Homepage" = "https://github.com/just-digital/html-content-extractor"
 "Bug Tracker" = "https://github.com/just-digital/html-content-extractor/issues"
-
```

