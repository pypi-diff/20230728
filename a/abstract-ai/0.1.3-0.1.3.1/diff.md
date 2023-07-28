# Comparing `tmp/abstract_ai-0.1.3.tar.gz` & `tmp/abstract_ai-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.1.3.tar", last modified: Fri Jul 28 02:51:44 2023, max compression
+gzip compressed data, was "abstract_ai-0.1.3.1.tar", last modified: Fri Jul 28 03:45:07 2023, max compression
```

## Comparing `abstract_ai-0.1.3.tar` & `abstract_ai-0.1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:51:44.097929 abstract_ai-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:51:44.097929 abstract_ai-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.3/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 02:51:44.101929 abstract_ai-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1410 2023-07-28 02:51:27.000000 abstract_ai-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:51:44.097929 abstract_ai-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:51:44.097929 abstract_ai-0.1.3/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.3/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4588 2023-07-28 02:50:46.000000 abstract_ai-0.1.3/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.3/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.3/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.3/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.3/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.3/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:51:44.097929 abstract_ai-0.1.3/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:51:44.000000 abstract_ai-0.1.3/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 02:51:44.000000 abstract_ai-0.1.3/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:51:44.000000 abstract_ai-0.1.3/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 02:51:44.000000 abstract_ai-0.1.3/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 02:51:44.000000 abstract_ai-0.1.3/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.3.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1412 2023-07-28 03:44:09.000000 abstract_ai-0.1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.3.1/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4589 2023-07-28 03:44:36.000000 abstract_ai-0.1.3.1/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.3.1/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.3.1/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.3.1/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.3.1/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.3.1/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:45:07.881232 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-07-28 03:45:07.000000 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 03:45:07.000000 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:45:07.000000 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 03:45:07.000000 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 03:45:07.000000 abstract_ai-0.1.3.1/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.1.3/PKG-INFO` & `abstract_ai-0.1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.1.3/README.md` & `abstract_ai-0.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/setup.py` & `abstract_ai-0.1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.1.3',
+      version='0.1.3.1',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.1.3/src/abstract_ai/api_calls.py` & `abstract_ai-0.1.3.1/src/abstract_ai/api_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 import openai
 from abstract_security.envy_it import get_env_value
 from .response_handling import save_response
 from .tokenization import count_tokens,calculate_token_distribution
 from .prompts import default_prompt,create_prompt
 from .endpoints import default_model,default_endpoint,default_tokens
+
 def get_openai_key(key:str='OPENAI_API_KEY'):
     """
     Retrieves the OpenAI API key from the environment variables.
 
     Args:
         path (str): The path to the environment file. Defaults to '/home/hmmm/envy_all.env'.
         st (str): The name of the environment variable containing the API key. Defaults to 'OPENAI_API_KEY'.
```

### Comparing `abstract_ai-0.1.3/src/abstract_ai/endpoints.py` & `abstract_ai-0.1.3.1/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/src/abstract_ai/main.py` & `abstract_ai-0.1.3.1/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/src/abstract_ai/prompts.py` & `abstract_ai-0.1.3.1/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/src/abstract_ai/response_handling.py` & `abstract_ai-0.1.3.1/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/src/abstract_ai/tokenization.py` & `abstract_ai-0.1.3.1/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.3/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.1.3.1/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

