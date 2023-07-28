# Comparing `tmp/HandyLLM-0.2.1.tar.gz` & `tmp/HandyLLM-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.2.1.tar", last modified: Thu Jul 27 13:37:04 2023, max compression
+gzip compressed data, was "HandyLLM-0.3.0.tar", last modified: Fri Jul 28 04:45:25 2023, max compression
```

## Comparing `HandyLLM-0.2.1.tar` & `HandyLLM-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/prompt_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.202968 HandyLLM-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.202968 HandyLLM-0.3.0/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:45:25.000000 HandyLLM-0.3.0/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:45:25.206968 HandyLLM-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-28 04:45:13.000000 HandyLLM-0.3.0/tests/test_stream.py
```

### Comparing `HandyLLM-0.2.1/PKG-INFO` & `HandyLLM-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.2.1
+Version: 0.3.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,17 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-This toolkit uses HTTP API request instead of OpenAI's official python package to support client-side `timeout` control:
+### Timeout control
+
+This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -53,22 +55,28 @@
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10
     )
 print(response['choices'][0]['message']['content'])
 ```
 
+### Authorization
+
 API key and organization will be loaded using the environment variable `OPENAI_API_KEY` and `OPENAI_ORGANIZATION`, or you can set manually:
 
 ```python
 OpenAIAPI.api_key = 'sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
 OpenAIAPI.organization = '......'  # default: None
 ```
 
-Stream response of `chat`/`completions` can be achieved using `steam` parameter:
+Or, you can pass `api_key` and `organization` parameters in each API call.
+
+### Stream response
+
+Stream response of `chat`/`completions`/`finetunes_list_events` can be achieved using `steam` parameter:
 
 ```python
 response = OpenAIAPI.chat(
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10,
     stream=True
@@ -80,18 +88,48 @@
 
 # or you can use this to get the whole response
 # for chunk in response:
 #     if 'content' in chunk['choices'][0]['delta']:
 #         print(chunk['choices'][0]['delta']['content'], end='')
 ```
 
+### Supported APIs
+
+- chat
+- completions
+- edits
+- embeddings
+- models_list
+- models_retrieve
+- moderations
+- images_generations
+- images_edits
+- images_variations
+- audio_transcriptions
+- audtio_translations
+- files_list
+- files_upload
+- files_delete
+- files_retrieve
+- files_retrieve_content
+- finetunes_create
+- finetunes_list
+- finetunes_retrieve
+- finetunes_cancel
+- finetunes_list_events
+- finetunes_delete_model
+
+Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
+
 
 
 ## Prompt
 
+### Prompt Conversion
+
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
 
 ```
 $system$
 You are a helpful assistant.
 
 $user$
@@ -118,15 +156,15 @@
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
 new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
 ```
 
-
+### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
 %output_format%
 Please output a SINGLE JSON object that contains all items from the two input JSON objects.
```

### Comparing `HandyLLM-0.2.1/README.md` & `HandyLLM-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-This toolkit uses HTTP API request instead of OpenAI's official python package to support client-side `timeout` control:
+### Timeout control
+
+This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -40,22 +42,28 @@
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10
     )
 print(response['choices'][0]['message']['content'])
 ```
 
+### Authorization
+
 API key and organization will be loaded using the environment variable `OPENAI_API_KEY` and `OPENAI_ORGANIZATION`, or you can set manually:
 
 ```python
 OpenAIAPI.api_key = 'sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
 OpenAIAPI.organization = '......'  # default: None
 ```
 
-Stream response of `chat`/`completions` can be achieved using `steam` parameter:
+Or, you can pass `api_key` and `organization` parameters in each API call.
+
+### Stream response
+
+Stream response of `chat`/`completions`/`finetunes_list_events` can be achieved using `steam` parameter:
 
 ```python
 response = OpenAIAPI.chat(
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10,
     stream=True
@@ -67,18 +75,48 @@
 
 # or you can use this to get the whole response
 # for chunk in response:
 #     if 'content' in chunk['choices'][0]['delta']:
 #         print(chunk['choices'][0]['delta']['content'], end='')
 ```
 
+### Supported APIs
+
+- chat
+- completions
+- edits
+- embeddings
+- models_list
+- models_retrieve
+- moderations
+- images_generations
+- images_edits
+- images_variations
+- audio_transcriptions
+- audtio_translations
+- files_list
+- files_upload
+- files_delete
+- files_retrieve
+- files_retrieve_content
+- finetunes_create
+- finetunes_list
+- finetunes_retrieve
+- finetunes_cancel
+- finetunes_list_events
+- finetunes_delete_model
+
+Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
+
 
 
 ## Prompt
 
+### Prompt Conversion
+
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
 
 ```
 $system$
 You are a helpful assistant.
 
 $user$
@@ -105,15 +143,15 @@
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
 new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
 ```
 
-
+### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
 %output_format%
 Please output a SINGLE JSON object that contains all items from the two input JSON objects.
```

### Comparing `HandyLLM-0.2.1/pyproject.toml` & `HandyLLM-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.2.1/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.3.0/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.2.1
+Version: 0.3.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,17 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-This toolkit uses HTTP API request instead of OpenAI's official python package to support client-side `timeout` control:
+### Timeout control
+
+This toolkit supports client-side `timeout` control, which OpenAI's official python package does not support yet:
 
 ```python
 from handyllm import OpenAIAPI
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
@@ -53,22 +55,28 @@
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10
     )
 print(response['choices'][0]['message']['content'])
 ```
 
+### Authorization
+
 API key and organization will be loaded using the environment variable `OPENAI_API_KEY` and `OPENAI_ORGANIZATION`, or you can set manually:
 
 ```python
 OpenAIAPI.api_key = 'sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
 OpenAIAPI.organization = '......'  # default: None
 ```
 
-Stream response of `chat`/`completions` can be achieved using `steam` parameter:
+Or, you can pass `api_key` and `organization` parameters in each API call.
+
+### Stream response
+
+Stream response of `chat`/`completions`/`finetunes_list_events` can be achieved using `steam` parameter:
 
 ```python
 response = OpenAIAPI.chat(
     model="gpt-3.5-turbo",
     messages=prompt,
     timeout=10,
     stream=True
@@ -80,18 +88,48 @@
 
 # or you can use this to get the whole response
 # for chunk in response:
 #     if 'content' in chunk['choices'][0]['delta']:
 #         print(chunk['choices'][0]['delta']['content'], end='')
 ```
 
+### Supported APIs
+
+- chat
+- completions
+- edits
+- embeddings
+- models_list
+- models_retrieve
+- moderations
+- images_generations
+- images_edits
+- images_variations
+- audio_transcriptions
+- audtio_translations
+- files_list
+- files_upload
+- files_delete
+- files_retrieve
+- files_retrieve_content
+- finetunes_create
+- finetunes_list
+- finetunes_retrieve
+- finetunes_cancel
+- finetunes_list_events
+- finetunes_delete_model
+
+Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
+
 
 
 ## Prompt
 
+### Prompt Conversion
+
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
 
 ```
 $system$
 You are a helpful assistant.
 
 $user$
@@ -118,15 +156,15 @@
 # chat can be used as the message parameter for OpenAI API
 chat = converter.rawfile2chat('prompt.txt')
 
 # variables wrapped in %s can be replaced at runtime
 new_chat = converter.chat_replace_variables(chat, {r'%misc%': 'Note: do not use any bad word.'})
 ```
 
-
+### Substitute
 
 `PromptConverter` can also substitute placeholder variables like `%output_format%` stored in text files to make multiple prompts modular. A substitute map `substitute.txt` looks like this:
 
 ```
 %output_format%
 Please output a SINGLE JSON object that contains all items from the two input JSON objects.
```

### Comparing `HandyLLM-0.2.1/src/handyllm/endpoint_manager.py` & `HandyLLM-0.3.0/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.1/src/handyllm/prompt_converter.py` & `HandyLLM-0.3.0/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.1/tests/test_api.py` & `HandyLLM-0.3.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.1/tests/test_prompt.py` & `HandyLLM-0.3.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.1/tests/test_stream.py` & `HandyLLM-0.3.0/tests/test_stream.py`

 * *Files identical despite different names*

