# Comparing `tmp/jinaai-0.2.3.tar.gz` & `tmp/jinaai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.2.3.tar", last modified: Tue Jul 25 05:27:10 2023, max compression
+gzip compressed data, was "jinaai-0.2.4.tar", last modified: Fri Jul 28 04:29:40 2023, max compression
```

## Comparing `jinaai-0.2.3.tar` & `jinaai-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.968061 jinaai-0.2.3/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.3/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-25 05:27:10.967885 jinaai-0.2.3/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14446 2023-07-25 04:59:05.000000 jinaai-0.2.3/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.965507 jinaai-0.2.3/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     3273 2023-07-25 04:10:03.000000 jinaai-0.2.3/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.967712 jinaai-0.2.3/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1639 2023-07-25 03:49:04.000000 jinaai-0.2.3/jinaai/clients/BestBannerClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.3/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1856 2023-07-02 05:36:25.000000 jinaai-0.2.3/jinaai/clients/JinaChatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2094 2023-07-02 05:51:36.000000 jinaai-0.2.3/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.3/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2020 2023-07-25 04:30:23.000000 jinaai-0.2.3/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.3/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.3/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-25 05:27:10.966243 jinaai-0.2.3/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      437 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/requires.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-25 05:27:10.000000 jinaai-0.2.3/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-25 05:27:10.968104 jinaai-0.2.3/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-25 05:25:41.000000 jinaai-0.2.3/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.627063 jinaai-0.2.4/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.4/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-28 04:29:40.626874 jinaai-0.2.4/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14446 2023-07-25 06:20:32.000000 jinaai-0.2.4/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.624660 jinaai-0.2.4/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     3411 2023-07-28 04:12:19.000000 jinaai-0.2.4/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.626705 jinaai-0.2.4/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1670 2023-07-28 03:49:43.000000 jinaai-0.2.4/jinaai/clients/BestBannerClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1261 2023-07-28 04:07:41.000000 jinaai-0.2.4/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1986 2023-07-28 04:17:10.000000 jinaai-0.2.4/jinaai/clients/JinaChatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2125 2023-07-28 03:50:10.000000 jinaai-0.2.4/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1965 2023-07-28 03:51:28.000000 jinaai-0.2.4/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2051 2023-07-28 03:51:56.000000 jinaai-0.2.4/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.4/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.4/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.625311 jinaai-0.2.4/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      437 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/requires.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-28 04:29:40.627107 jinaai-0.2.4/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-28 04:29:30.000000 jinaai-0.2.4/setup.py
```

### Comparing `jinaai-0.2.3/LICENSE` & `jinaai-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.3/PKG-INFO` & `jinaai-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.3
+Version: 0.2.4
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jinaai-0.2.3/README.md` & `jinaai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.3/jinaai/__init__.py` & `jinaai-0.2.4/jinaai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,18 @@
     def generate(self, input, options=None):
         if isinstance(input, list):
             data = self.CCClient.from_array(input, options)
         elif isinstance(input, str):
             data = self.CCClient.from_string(input, options)
         else:
             data = input
-        return self.CCClient.generate(data, options)
+        if options is not None and options.get('stream', False):
+            return self.CCClient.stream(data, options)
+        else:
+            return self.CCClient.generate(data, options)
 
     def imagine(self, input, options=None):
         if isinstance(input, list):
             data = self.BBClient.from_array(input, options)
         elif isinstance(input, str):
             data = self.BBClient.from_string(input, options)
         else:
```

### Comparing `jinaai-0.2.3/jinaai/clients/BestBannerClient.py` & `jinaai-0.2.4/jinaai/clients/BestBannerClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .HTTPClient import HTTPClient
 
 class BestBannerClient(HTTPClient):
-    def __init__(self, headers=None):
+    def __init__(self, headers=None, options=None):
         baseUrl = 'https://api.bestbanner.jina.ai/v1'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
-        super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
+        super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
             'data': [
                 {
                     'text': i,
                     **(options or {})
```

### Comparing `jinaai-0.2.3/jinaai/clients/JinaChatClient.py` & `jinaai-0.2.4/jinaai/clients/JinaChatClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 
 class JinaChatClient(HTTPClient):
-    def __init__(self, headers=None):
+    def __init__(self, headers=None, options=None):
         baseUrl = 'https://api.chat.jina.ai/v1/chat'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
-        super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
+        super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
             'messages': [
                 {
                     'content': i,
                     **(((is_url(i) or is_base64(i)) and { 'image': i }) or {}),
@@ -48,7 +48,10 @@
 
     def generate(self, data, options = None):
         raw_output = self.post('/completions', data)
         simplified_output = self.to_simplified_output(raw_output)
         if options and 'raw' in options:
             simplified_output['raw'] = raw_output
         return simplified_output
+
+    def stream(self, data, options = None):
+        return self.post('/completions', data, False)
```

### Comparing `jinaai-0.2.3/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.2.4/jinaai/clients/PromptPerfectClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 class PromptPerfectClient(HTTPClient):
-    def __init__(self, headers=None):
+    def __init__(self, headers=None, options=None):
         baseUrl = 'https://api.promptperfect.jina.ai'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
-        super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
+        super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
             'data': [
                 {
                     **(((not is_url(i) and not is_base64(i)) and { 'prompt': i }) or {}),
                     **(((is_url(i) or is_base64(i)) and { 'imagePrompt': i }) or {}),
```

### Comparing `jinaai-0.2.3/jinaai/clients/RationaleClient.py` & `jinaai-0.2.4/jinaai/clients/RationaleClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 MAXLEN = 300
 
 class RationaleClient(HTTPClient):
-    def __init__(self, headers=None):
+    def __init__(self, headers=None, options=None):
         baseUrl = 'https://us-central1-rationale-ai.cloudfunctions.net'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
-        super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
+        super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
             'data': [
                 {
                     'decision': i[:MAXLEN],
                     **(options or {})
```

### Comparing `jinaai-0.2.3/jinaai/clients/SceneXClient.py` & `jinaai-0.2.4/jinaai/clients/SceneXClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 def autoFillFeatures(options=None):
     features = options.get('features', []) if options else []
     if options and 'question' in options and 'question_answer' not in features:
         features.append('question_answer')
     return features
 
 class SceneXClient(HTTPClient):
-    def __init__(self, headers=None):
+    def __init__(self, headers=None, options=None):
         baseUrl = 'https://api.scenex.jina.ai/v1'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
-        super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
+        super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
             'data': [
                 {
                     'image': i,
                     'features': autoFillFeatures(options),
```

### Comparing `jinaai-0.2.3/jinaai/utils.py` & `jinaai-0.2.4/jinaai/utils.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.3/jinaai.egg-info/PKG-INFO` & `jinaai-0.2.4/jinaai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.3
+Version: 0.2.4
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

