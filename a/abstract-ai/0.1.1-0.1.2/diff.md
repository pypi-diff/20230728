# Comparing `tmp/abstract_ai-0.1.1.tar.gz` & `tmp/abstract_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_ai-0.1.1.tar", last modified: Fri Jul 28 02:14:28 2023, max compression
+gzip compressed data, was "abstract_ai-0.1.2.tar", last modified: Fri Jul 28 02:42:15 2023, max compression
```

## Comparing `abstract_ai-0.1.1.tar` & `abstract_ai-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1410 2023-07-28 02:14:16.000000 abstract_ai-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/abstract_ai/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.1/src/abstract_ai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4502 2023-05-31 22:02:05.000000 abstract_ai-0.1.1/src/abstract_ai/api_calls.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.1/src/abstract_ai/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.1/src/abstract_ai/main.py
--rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.1/src/abstract_ai/prompts.py
--rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.1/src/abstract_ai/response_handling.py
--rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.1/src/abstract_ai/tokenization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:14:28.880889 abstract_ai-0.1.1/src/abstract_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 02:14:28.000000 abstract_ai-0.1.1/src/abstract_ai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4729 2023-05-31 17:26:44.000000 abstract_ai-0.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-31 01:51:39.000000 abstract_ai-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1410 2023-07-28 02:41:55.000000 abstract_ai-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/src/abstract_ai/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-29 07:24:38.000000 abstract_ai-0.1.2/src/abstract_ai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4511 2023-07-28 02:41:17.000000 abstract_ai-0.1.2/src/abstract_ai/api_calls.py
+-rw-rw-r--   0 root         (0) root         (0)     4103 2023-05-31 09:35:39.000000 abstract_ai-0.1.2/src/abstract_ai/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1286 2023-05-29 07:24:38.000000 abstract_ai-0.1.2/src/abstract_ai/main.py
+-rw-rw-r--   0 root         (0) root         (0)     9647 2023-05-31 17:38:48.000000 abstract_ai-0.1.2/src/abstract_ai/prompts.py
+-rw-rw-r--   0 root         (0) root         (0)     4344 2023-05-31 19:44:53.000000 abstract_ai-0.1.2/src/abstract_ai/response_handling.py
+-rw-rw-r--   0 root         (0) root         (0)     2331 2023-05-31 22:09:37.000000 abstract_ai-0.1.2/src/abstract_ai/tokenization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:42:15.002638 abstract_ai-0.1.2/src/abstract_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-07-28 02:42:14.000000 abstract_ai-0.1.2/src/abstract_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-28 02:42:14.000000 abstract_ai-0.1.2/src/abstract_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:42:14.000000 abstract_ai-0.1.2/src/abstract_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-28 02:42:14.000000 abstract_ai-0.1.2/src/abstract_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-28 02:42:14.000000 abstract_ai-0.1.2/src/abstract_ai.egg-info/top_level.txt
```

### Comparing `abstract_ai-0.1.1/PKG-INFO` & `abstract_ai-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_ai-0.1.1/README.md` & `abstract_ai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/setup.py` & `abstract_ai-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='abstract_ai',
-      version='0.1.1',
+      version='0.1.2',
       author='putkoff',
       author_email='partners@abstractendeavors.com',
       description="abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai',
       classifiers=[
```

### Comparing `abstract_ai-0.1.1/src/abstract_ai/api_calls.py` & `abstract_ai-0.1.2/src/abstract_ai/api_calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,43 +35,48 @@
 def post_request(endpoint:str=default_endpoint(), prompt:(str or dict)=create_prompt(),content_type:str='application/json',api_key:str=get_openai_key()):
         response = requests.post(endpoint, headers=headers(content_type,api_key), json=prompt)
         if response.status_code == 200:
             return response
         else:
             raise Exception(f'Request failed with status code {response.status_code}')
 
-def hard_request(prompt:str=default_prompt(),model:str=default_model(),max_tokens:int=default_tokens(),temperature:float=0.5,top_p:int=1,frequency_penalty:int=0,presence_penalty:int=0):
-    input([prompt,max_tokens,model])
+def hard_request(prompt: str = default_prompt(), model: str = default_model(), max_tokens: int = default_tokens(),
+                 temperature: float = 0.5, top_p: int = 1, frequency_penalty: int = 0, presence_penalty: int = 0):
     """
     Sends a hard request to the OpenAI API using the provided parameters.
 
     Args:
         max_tokens (int): The maximum number of tokens for the completion.
         prompt (str): The prompt for the API request.
 
     Returns:
         dict: The response received from the OpenAI API.
     """
     load_openai_key()
+    message = {
+        "role": "user",
+        "content": prompt
+    }
     response = openai.ChatCompletion.create(
-      model=model,
-      messages=prompt)
+        model=model,
+        messages=[message]
+    )
     return response
 def quick_request(prompt:str=default_prompt(),max_tokens:int=default_tokens(),model=default_model()):
     """
     Sends a quick request to the OpenAI API using the provided parameters and prints the result.
 
     Args:
         prompt (str, optional): The prompt for the API request. Defaults to the default_prompt().
         max_tokens (int, optional): The maximum number of tokens for the completion. Defaults to default_tokens().
 
     Returns:
         None
     """
-    print(hard_request(max_tokens=max_tokens, prompt=prompt,model=model))
+    return hard_request(max_tokens=max_tokens, prompt=prompt,model=model)
 def raw_data(prompt:str=default_prompt(),model=default_model(),js:dict={}, endpoint:str=default_endpoint()):
     """
     Sends a raw data request to the specified endpoint with the provided parameters.
 
     Args:
         prompt (str, optional): The prompt for the API request. Defaults to default_prompt().
         js (dict, optional): The JSON dictionary containing the request data. Defaults to an empty dictionary.
@@ -91,14 +96,11 @@
     responses = []
     for k in range(0,total):
         bef = int(count_tokens(js['prompt']))
         formatted_prompt = f'part {k} of {total}:\n{token_dist["chunks"]["data"][k]}'
         formatted_prompt_length = count_tokens(formatted_prompt)
         js['prompt'] = formatted_prompt
         js['max_tokens'] = int(float(token_dist["completion"]["available"] - (formatted_prompt_length - bef))*.90)
-        #js['max_tokens'] = int(js['max_tokens']) -((int(count_tokens(js['prompt']))-int(pre_max)))
         response = requests.post(endpoint, json=create_prompt(js), headers=headers())
         resp = save_response(js, response)
-        print(resp)
-        responses.append(resp)
+        responses.append(response.json()['choices'][0]['message']['content'])
     return responses
-
```

### Comparing `abstract_ai-0.1.1/src/abstract_ai/endpoints.py` & `abstract_ai-0.1.2/src/abstract_ai/endpoints.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/src/abstract_ai/main.py` & `abstract_ai-0.1.2/src/abstract_ai/main.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/src/abstract_ai/prompts.py` & `abstract_ai-0.1.2/src/abstract_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/src/abstract_ai/response_handling.py` & `abstract_ai-0.1.2/src/abstract_ai/response_handling.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/src/abstract_ai/tokenization.py` & `abstract_ai-0.1.2/src/abstract_ai/tokenization.py`

 * *Files identical despite different names*

### Comparing `abstract_ai-0.1.1/src/abstract_ai.egg-info/PKG-INFO` & `abstract_ai-0.1.2/src/abstract_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: abstract_ai is a Python module that provides a wide range of functionalities aimed at facilitating and enhancing interactions with AI. Developed by putkoff, it comprises several utility modules to help handle API responses, generate requests, manage tokenization, and deal with other related aspects.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_ai
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

