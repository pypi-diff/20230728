# Comparing `tmp/abstract_ai-0.1.0.tar.gz` & `tmp/abstract_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.1.0.tar", last modified: Fri Jul 28 02:13:07 2023, max compression
+gzip compressed data, was "abstract_ai-0.1.1.tar", last modified: Fri Jul 28 02:14:28 2023, max compression
```

## Comparing `abstract_ai-0.1.0.tar` & `abstract_ai-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5546 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.0/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1409 2023-07-28 02:12:54.000000 abstract_ai-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.0/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4502 2023-05-31 22:02:05.000000 abstract_ai-0.1.0/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.0/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.0/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.0/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.0/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.0/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:13:07.072801 abstract_ai-0.1.0/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5546 2023-07-28 02:13:07.000000 abstract_ai-0.1.0/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 02:13:07.000000 abstract_ai-0.1.0/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:13:07.000000 abstract_ai-0.1.0/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 02:13:07.000000 abstract_ai-0.1.0/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 02:13:07.000000 abstract_ai-0.1.0/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-07-28 02:14:16.000000 abstract_ai-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.1/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4502 2023-05-31 22:02:05.000000 abstract_ai-0.1.1/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.1/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.1/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.1/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.1/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.1/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.1.0/PKG-INFO` & `abstract_ai-0.1.1/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: abstract_ai
-Version: 0.1.0
+Name: abstract-ai
+Version: 0.1.1
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
-Home-page: https://github.io/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_ai-0.1.0/README.md` & `abstract_ai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/setup.py` & `abstract_ai-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.1.0',
+      version='0.1.1',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
-      url='https://github.io/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
+      url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
```

### Comparing `abstract_ai-0.1.0/src/abstract_ai/api_calls.py` & `abstract_ai-0.1.1/src/abstract_ai/api_calls.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai/endpoints.py` & `abstract_ai-0.1.1/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai/main.py` & `abstract_ai-0.1.1/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai/prompts.py` & `abstract_ai-0.1.1/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai/response_handling.py` & `abstract_ai-0.1.1/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai/tokenization.py` & `abstract_ai-0.1.1/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.0/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: abstract-ai
-Version: 0.1.0
+Name: abstract_ai
+Version: 0.1.1
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
-Home-page: https://github.io/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

