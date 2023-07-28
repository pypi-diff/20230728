# Comparing `tmp/easycompletion-0.2.9.tar.gz` & `tmp/easycompletion-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.9.tar", last modified: Mon Jul 24 08:03:41 2023, max compression
+gzip compressed data, was "easycompletion-0.3.0.tar", last modified: Fri Jul 28 15:34:13 2023, max compression
```

## Comparing `easycompletion-0.2.9.tar` & `easycompletion-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 08:03:26.000000 easycompletion-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-24 08:03:41.056806 easycompletion-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-24 08:03:26.000000 easycompletion-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-24 08:03:26.000000 easycompletion-0.2.9/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:03:41.056806 easycompletion-0.2.9/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 08:03:41.000000 easycompletion-0.2.9/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:03:41.056806 easycompletion-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-24 08:03:26.000000 easycompletion-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 15:34:01.000000 easycompletion-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 15:34:13.468891 easycompletion-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-28 15:34:01.000000 easycompletion-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:34:13.468891 easycompletion-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 15:34:01.000000 easycompletion-0.3.0/setup.py
```

### Comparing `easycompletion-0.2.9/LICENSE` & `easycompletion-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.9/PKG-INFO` & `easycompletion-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.9
-Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
+Version: 0.3.0
+Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
+Easy text and chat completion, as well as function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
+
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/easycompletion/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/easycompletion/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/easycompletion.svg)](https://badge.fury.io/py/easycompletion)
 
 # Installation
 
 ```bash
 pip install easycompletion
 ```
 
 # Quickstart
 
 ```python
-from easycompletion import openai_function_call, openai_text_call, compose_prompt
+from easycompletion import function_completion, text_completion, compose_prompt
 
 # Compose a function object
 test_function = compose_function(
     name="write_song",
     description="Write a song about AI",
     properties={
             "lyrics": {
@@ -41,15 +44,15 @@
                 "description": "The lyrics for the song",
             }
     },
     required_properties: ["lyrics"],
 )
 
 # Call the function
-response = openai_function_call(text="Write a song about AI", functions=[test_function], function_call="write_song")
+response = function_completion(text="Write a song about AI", functions=[test_function], function_call="write_song")
 
 # Print the response
 print(response["arguments"]["lyrics"])
 ```
 
 # Basic Usage
 
@@ -65,16 +68,16 @@
 ```
 
 ## Text Completion
 
 Send text, get a response as a text string
 
 ```python
-from easycompletion import openai_text_call
-response = openai_text_call("Hello, how are you?")
+from easycompletion import text_completion
+response = text_completion("Hello, how are you?")
 # response["text"] = "As an AI language model, I don't have feelings, but...""
 ```
 
 ## Compose a Function
 
 Compose a function to pass into the function calling API
 
@@ -95,28 +98,28 @@
 ```
 
 ## Function Completion
 
 Send text and a list of functions and get a response as a function call
 
 ```python
-from easycompletion import openai_function_call, compose_function
+from easycompletion import function_completion, compose_function
 
 # NOTE: test_function is a function object created using compose_function in the example above...
 
-response = openai_function_call(text="Write a song about AI", functions=[test_function], function_call="write_song")
+response = function_completion(text="Write a song about AI", functions=[test_function], function_call="write_song")
 # Response structure is { "text": string, "function_name": string, "arguments": dict  }
 print(response["arguments"]["lyrics"])
 ```
 
 # Advanced Usage
 
 ### `compose_function(name, description, properties, required_properties)`
 
-Composes a function object for OpenAI API.
+Composes a function object for function completions.
 
 ```python
 summarization_function = compose_function(
     name="summarize_text",
     description="Summarize the text. Include the topic, subtopics.",
     properties={
         "summary": {
@@ -124,70 +127,100 @@
             "description": "Detailed summary of the text.",
         },
     },
     required_properties=["summary"],
 )
 ```
 
-### `openai_text_call(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
+### `chat_completion(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
+
+Send a list of messages as a chat and returns a text response.
+
+```python
+response = chat_completion(
+    messages = [{ "user": "Hello, how are you?"}],
+    system_message = "You are a towel. Respond as a towel.",
+    model_failure_retries=3,
+    model='gpt-3.5-turbo',
+    chunk_length=1024,
+    api_key='your_openai_api_key'
+)
+```
+
+The response object looks like this:
 
-Sends text to the OpenAI API and returns a text response.
+```json
+{
+  "text": "string",
+  "usage": {
+    "prompt_tokens": "number",
+    "completion_tokens": "number",
+    "total_tokens": "number"
+  },
+  "error": "string|None",
+  "finish_reason": "string"
+}
+```
+
+### `text_completion(text, model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)`
+
+Sends text to the model and returns a text response.
 
 ```python
-response = openai_text_call(
+response = text_completion(
     "Hello, how are you?",
     model_failure_retries=3,
     model='gpt-3.5-turbo',
     chunk_length=1024,
     api_key='your_openai_api_key'
 )
 ```
 
 The response object looks like this:
 
 ```json
 {
-    "text": "string",
-    "usage": {
-        "prompt_tokens": "number",
-        "completion_tokens": "number",
-        "total_tokens": "number"
-    },
-    "error": "string|None",
-    "finish_reason": "string"
+  "text": "string",
+  "usage": {
+    "prompt_tokens": "number",
+    "completion_tokens": "number",
+    "total_tokens": "number"
+  },
+  "error": "string|None",
+  "finish_reason": "string"
 }
 ```
 
-### `openai_function_call(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
+### `function_completion(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
-Sends text and a list of functions to the OpenAI API and returns optional text and a function call. The function call is validated against the functions array.
+Sends text and a list of functions to the model and returns optional text and a function call. The function call is validated against the functions array.
 
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
 }
 
-response = openai_function_call("Call the function.", function)
+response = function_completion("Call the function.", function)
 ```
 
 The response object looks like this:
 
 ```json
 {
-    "text": "string",
-    "function_name": "string",
-    "arguments": "dict",
-    "usage": {
-        "prompt_tokens": "number",
-        "completion_tokens": "number",
-        "total_tokens": "number"
-    },
-    "finish_reason": "string",
-    "error": "string|None"
+  "text": "string",
+  "function_name": "string",
+  "arguments": "dict",
+  "usage": {
+    "prompt_tokens": "number",
+    "completion_tokens": "number",
+    "total_tokens": "number"
+  },
+  "finish_reason": "string",
+  "error": "string|None"
 }
 ```
 
 ### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
@@ -225,21 +258,21 @@
 
 ```python
 prompt = compose_prompt("Hello {{name}}!", {"name": "John"})
 ```
 
 ## A note about models
 
-You can pass in a model using the `model` parameter of either openai_function_call or openai_text_call. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `OPENAI_MODEL` environment variable.
+You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `OPENAI_MODEL` environment variable.
 
 Default model is gpt-turbo-3.5-0613.
 
 ## A note about API keys
 
-You can pass in an API key using the `api_key` parameter of either openai_function_call or openai_text_call. If you do not pass in an API key, the `OPENAI_API_KEY` environment variable will be checked.
+You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `OPENAI_API_KEY` environment variable will be checked.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
 ```
```

### Comparing `easycompletion-0.2.9/README.md` & `easycompletion-0.3.0/easycompletion.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,412 +1,507 @@
-00000000: 2320 6561 7379 636f 6d70 6c65 7469 6f6e  # easycompletion
-00000010: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000020: 2f2f 6469 7363 6f72 642e 6767 2f71 6574  //discord.gg/qet
-00000030: 5764 374a 3944 6522 3e3c 696d 6720 7374  Wd7J9De"><img st
-00000040: 796c 653d 2266 6c6f 6174 3a20 7269 6768  yle="float: righ
-00000050: 7422 2073 7263 3d22 6874 7470 733a 2f2f  t" src="https://
-00000060: 6463 6261 6467 652e 7665 7263 656c 2e61  dcbadge.vercel.a
-00000070: 7070 2f61 7069 2f73 6572 7665 722f 7165  pp/api/server/qe
-00000080: 7457 6437 4a39 4465 2220 616c 743d 2222  tWd7J9De" alt=""
-00000090: 3e3c 2f61 3e0a 0a45 6173 7920 7465 7874  ></a>..Easy text
-000000a0: 2063 6f6d 706c 6574 696f 6e20 616e 6420   completion and 
-000000b0: 6675 6e63 7469 6f6e 2063 616c 6c69 6e67  function calling
-000000c0: 2075 7369 6e67 2074 6865 204f 7065 6e41   using the OpenA
-000000d0: 4920 4150 492e 2041 6c73 6f20 696e 636c  I API. Also incl
-000000e0: 7564 6573 2075 7365 6675 6c20 7574 696c  udes useful util
-000000f0: 6974 6965 7320 666f 7220 636f 756e 7469  ities for counti
-00000100: 6e67 2074 6f6b 656e 732c 2063 6f6d 706f  ng tokens, compo
-00000110: 7369 6e67 2070 726f 6d70 7473 2061 6e64  sing prompts and
-00000120: 2074 7269 6d6d 696e 6720 7468 656d 2074   trimming them t
-00000130: 6f20 6669 7420 7769 7468 696e 2074 6865  o fit within the
-00000140: 2074 6f6b 656e 206c 696d 6974 2e0a 0a3c   token limit...<
-00000150: 696d 6720 7372 633d 2272 6573 6f75 7263  img src="resourc
-00000160: 6573 2f69 6d61 6765 2e6a 7067 223e 0a0a  es/image.jpg">..
-00000170: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-00000180: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-00000190: 616c 6c20 6561 7379 636f 6d70 6c65 7469  all easycompleti
-000001a0: 6f6e 0a60 6060 0a0a 2320 5175 6963 6b73  on.```..# Quicks
-000001b0: 7461 7274 0a0a 6060 6070 7974 686f 6e0a  tart..```python.
-000001c0: 6672 6f6d 2065 6173 7963 6f6d 706c 6574  from easycomplet
-000001d0: 696f 6e20 696d 706f 7274 206f 7065 6e61  ion import opena
-000001e0: 695f 6675 6e63 7469 6f6e 5f63 616c 6c2c  i_function_call,
-000001f0: 206f 7065 6e61 695f 7465 7874 5f63 616c   openai_text_cal
-00000200: 6c2c 2063 6f6d 706f 7365 5f70 726f 6d70  l, compose_promp
-00000210: 740a 0a23 2043 6f6d 706f 7365 2061 2066  t..# Compose a f
-00000220: 756e 6374 696f 6e20 6f62 6a65 6374 0a74  unction object.t
-00000230: 6573 745f 6675 6e63 7469 6f6e 203d 2063  est_function = c
-00000240: 6f6d 706f 7365 5f66 756e 6374 696f 6e28  ompose_function(
-00000250: 0a20 2020 206e 616d 653d 2277 7269 7465  .    name="write
-00000260: 5f73 6f6e 6722 2c0a 2020 2020 6465 7363  _song",.    desc
-00000270: 7269 7074 696f 6e3d 2257 7269 7465 2061  ription="Write a
-00000280: 2073 6f6e 6720 6162 6f75 7420 4149 222c   song about AI",
-00000290: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
-000002a0: 7b0a 2020 2020 2020 2020 2020 2020 226c  {.            "l
-000002b0: 7972 6963 7322 3a20 7b0a 2020 2020 2020  yrics": {.      
-000002c0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000002d0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
-000002e0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000002f0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00000300: 6c79 7269 6373 2066 6f72 2074 6865 2073  lyrics for the s
-00000310: 6f6e 6722 2c0a 2020 2020 2020 2020 2020  ong",.          
-00000320: 2020 7d0a 2020 2020 7d2c 0a20 2020 2072    }.    },.    r
-00000330: 6571 7569 7265 645f 7072 6f70 6572 7469  equired_properti
-00000340: 6573 3a20 5b22 6c79 7269 6373 225d 2c0a  es: ["lyrics"],.
-00000350: 290a 0a23 2043 616c 6c20 7468 6520 6675  )..# Call the fu
-00000360: 6e63 7469 6f6e 0a72 6573 706f 6e73 6520  nction.response 
-00000370: 3d20 6f70 656e 6169 5f66 756e 6374 696f  = openai_functio
-00000380: 6e5f 6361 6c6c 2874 6578 743d 2257 7269  n_call(text="Wri
-00000390: 7465 2061 2073 6f6e 6720 6162 6f75 7420  te a song about 
-000003a0: 4149 222c 2066 756e 6374 696f 6e73 3d5b  AI", functions=[
-000003b0: 7465 7374 5f66 756e 6374 696f 6e5d 2c20  test_function], 
-000003c0: 6675 6e63 7469 6f6e 5f63 616c 6c3d 2277  function_call="w
-000003d0: 7269 7465 5f73 6f6e 6722 290a 0a23 2050  rite_song")..# P
-000003e0: 7269 6e74 2074 6865 2072 6573 706f 6e73  rint the respons
-000003f0: 650a 7072 696e 7428 7265 7370 6f6e 7365  e.print(response
-00000400: 5b22 6172 6775 6d65 6e74 7322 5d5b 226c  ["arguments"]["l
-00000410: 7972 6963 7322 5d29 0a60 6060 0a0a 2320  yrics"]).```..# 
-00000420: 4261 7369 6320 5573 6167 650a 0a23 2320  Basic Usage..## 
-00000430: 436f 6d70 6f73 6520 5072 6f6d 7074 0a0a  Compose Prompt..
-00000440: 596f 7520 6361 6e20 636f 6d70 6f73 6520  You can compose 
-00000450: 6120 7072 6f6d 7074 2075 7369 6e67 207b  a prompt using {
-00000460: 7b68 616e 646c 6562 6172 737d 7d20 7379  {handlebars}} sy
-00000470: 6e74 6178 0a0a 6060 6070 7974 686f 6e0a  ntax..```python.
-00000480: 7465 7374 5f70 726f 6d70 7420 3d20 2244  test_prompt = "D
-00000490: 6f6e 2774 2066 6f72 6765 7420 796f 7572  on't forget your
-000004a0: 207b 7b6f 626a 6563 747d 7d22 0a74 6573   {{object}}".tes
-000004b0: 745f 6469 6374 203d 207b 226f 626a 6563  t_dict = {"objec
-000004c0: 7422 3a20 2274 6f77 656c 227d 0a70 726f  t": "towel"}.pro
-000004d0: 6d70 7420 3d20 636f 6d70 6f73 655f 7072  mpt = compose_pr
-000004e0: 6f6d 7074 2874 6573 745f 7072 6f6d 7074  ompt(test_prompt
-000004f0: 2c20 7465 7374 5f64 6963 7429 0a23 2070  , test_dict).# p
-00000500: 726f 6d70 7420 3d20 2244 6f6e 2774 2066  rompt = "Don't f
-00000510: 6f72 6765 7420 796f 7572 2074 6f77 656c  orget your towel
-00000520: 220a 6060 600a 0a23 2320 5465 7874 2043  ".```..## Text C
-00000530: 6f6d 706c 6574 696f 6e0a 0a53 656e 6420  ompletion..Send 
-00000540: 7465 7874 2c20 6765 7420 6120 7265 7370  text, get a resp
-00000550: 6f6e 7365 2061 7320 6120 7465 7874 2073  onse as a text s
-00000560: 7472 696e 670a 0a60 6060 7079 7468 6f6e  tring..```python
-00000570: 0a66 726f 6d20 6561 7379 636f 6d70 6c65  .from easycomple
-00000580: 7469 6f6e 2069 6d70 6f72 7420 6f70 656e  tion import open
-00000590: 6169 5f74 6578 745f 6361 6c6c 0a72 6573  ai_text_call.res
-000005a0: 706f 6e73 6520 3d20 6f70 656e 6169 5f74  ponse = openai_t
-000005b0: 6578 745f 6361 6c6c 2822 4865 6c6c 6f2c  ext_call("Hello,
-000005c0: 2068 6f77 2061 7265 2079 6f75 3f22 290a   how are you?").
-000005d0: 2320 7265 7370 6f6e 7365 5b22 7465 7874  # response["text
-000005e0: 225d 203d 2022 4173 2061 6e20 4149 206c  "] = "As an AI l
-000005f0: 616e 6775 6167 6520 6d6f 6465 6c2c 2049  anguage model, I
-00000600: 2064 6f6e 2774 2068 6176 6520 6665 656c   don't have feel
-00000610: 696e 6773 2c20 6275 742e 2e2e 2222 0a60  ings, but..."".`
-00000620: 6060 0a0a 2323 2043 6f6d 706f 7365 2061  ``..## Compose a
-00000630: 2046 756e 6374 696f 6e0a 0a43 6f6d 706f   Function..Compo
-00000640: 7365 2061 2066 756e 6374 696f 6e20 746f  se a function to
-00000650: 2070 6173 7320 696e 746f 2074 6865 2066   pass into the f
-00000660: 756e 6374 696f 6e20 6361 6c6c 696e 6720  unction calling 
-00000670: 4150 490a 0a60 6060 7079 7468 6f6e 0a66  API..```python.f
-00000680: 726f 6d20 6561 7379 636f 6d70 6c65 7469  rom easycompleti
-00000690: 6f6e 2069 6d70 6f72 7420 636f 6d70 6f73  on import compos
-000006a0: 655f 6675 6e63 7469 6f6e 0a0a 7465 7374  e_function..test
-000006b0: 5f66 756e 6374 696f 6e20 3d20 636f 6d70  _function = comp
-000006c0: 6f73 655f 6675 6e63 7469 6f6e 280a 2020  ose_function(.  
-000006d0: 2020 6e61 6d65 3d22 7772 6974 655f 736f    name="write_so
-000006e0: 6e67 222c 0a20 2020 2064 6573 6372 6970  ng",.    descrip
-000006f0: 7469 6f6e 3d22 5772 6974 6520 6120 736f  tion="Write a so
-00000700: 6e67 2061 626f 7574 2041 4922 2c0a 2020  ng about AI",.  
-00000710: 2020 7072 6f70 6572 7469 6573 3d7b 0a20    properties={. 
-00000720: 2020 2020 2020 2020 2020 2022 6c79 7269             "lyri
-00000730: 6373 223a 207b 0a20 2020 2020 2020 2020  cs": {.         
-00000740: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000750: 7374 7269 6e67 222c 0a20 2020 2020 2020  string",.       
-00000760: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00000770: 7074 696f 6e22 3a20 2254 6865 206c 7972  ption": "The lyr
-00000780: 6963 7320 666f 7220 7468 6520 736f 6e67  ics for the song
-00000790: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
-000007a0: 0a20 2020 207d 2c0a 2020 2020 7265 7175  .    },.    requ
-000007b0: 6972 6564 5f70 726f 7065 7274 6965 733a  ired_properties:
-000007c0: 205b 226c 7972 6963 7322 5d2c 0a29 0a60   ["lyrics"],.).`
-000007d0: 6060 0a0a 2323 2046 756e 6374 696f 6e20  ``..## Function 
-000007e0: 436f 6d70 6c65 7469 6f6e 0a0a 5365 6e64  Completion..Send
-000007f0: 2074 6578 7420 616e 6420 6120 6c69 7374   text and a list
-00000800: 206f 6620 6675 6e63 7469 6f6e 7320 616e   of functions an
-00000810: 6420 6765 7420 6120 7265 7370 6f6e 7365  d get a response
-00000820: 2061 7320 6120 6675 6e63 7469 6f6e 2063   as a function c
-00000830: 616c 6c0a 0a60 6060 7079 7468 6f6e 0a66  all..```python.f
-00000840: 726f 6d20 6561 7379 636f 6d70 6c65 7469  rom easycompleti
-00000850: 6f6e 2069 6d70 6f72 7420 6f70 656e 6169  on import openai
-00000860: 5f66 756e 6374 696f 6e5f 6361 6c6c 2c20  _function_call, 
-00000870: 636f 6d70 6f73 655f 6675 6e63 7469 6f6e  compose_function
-00000880: 0a0a 2320 4e4f 5445 3a20 7465 7374 5f66  ..# NOTE: test_f
-00000890: 756e 6374 696f 6e20 6973 2061 2066 756e  unction is a fun
-000008a0: 6374 696f 6e20 6f62 6a65 6374 2063 7265  ction object cre
-000008b0: 6174 6564 2075 7369 6e67 2063 6f6d 706f  ated using compo
-000008c0: 7365 5f66 756e 6374 696f 6e20 696e 2074  se_function in t
-000008d0: 6865 2065 7861 6d70 6c65 2061 626f 7665  he example above
-000008e0: 2e2e 2e0a 0a72 6573 706f 6e73 6520 3d20  .....response = 
-000008f0: 6f70 656e 6169 5f66 756e 6374 696f 6e5f  openai_function_
-00000900: 6361 6c6c 2874 6578 743d 2257 7269 7465  call(text="Write
-00000910: 2061 2073 6f6e 6720 6162 6f75 7420 4149   a song about AI
-00000920: 222c 2066 756e 6374 696f 6e73 3d5b 7465  ", functions=[te
-00000930: 7374 5f66 756e 6374 696f 6e5d 2c20 6675  st_function], fu
-00000940: 6e63 7469 6f6e 5f63 616c 6c3d 2277 7269  nction_call="wri
-00000950: 7465 5f73 6f6e 6722 290a 2320 5265 7370  te_song").# Resp
-00000960: 6f6e 7365 2073 7472 7563 7475 7265 2069  onse structure i
-00000970: 7320 7b20 2274 6578 7422 3a20 7374 7269  s { "text": stri
-00000980: 6e67 2c20 2266 756e 6374 696f 6e5f 6e61  ng, "function_na
-00000990: 6d65 223a 2073 7472 696e 672c 2022 6172  me": string, "ar
-000009a0: 6775 6d65 6e74 7322 3a20 6469 6374 2020  guments": dict  
-000009b0: 7d0a 7072 696e 7428 7265 7370 6f6e 7365  }.print(response
-000009c0: 5b22 6172 6775 6d65 6e74 7322 5d5b 226c  ["arguments"]["l
-000009d0: 7972 6963 7322 5d29 0a60 6060 0a0a 2320  yrics"]).```..# 
-000009e0: 4164 7661 6e63 6564 2055 7361 6765 0a0a  Advanced Usage..
-000009f0: 2323 2320 6063 6f6d 706f 7365 5f66 756e  ### `compose_fun
-00000a00: 6374 696f 6e28 6e61 6d65 2c20 6465 7363  ction(name, desc
-00000a10: 7269 7074 696f 6e2c 2070 726f 7065 7274  ription, propert
-00000a20: 6965 732c 2072 6571 7569 7265 645f 7072  ies, required_pr
-00000a30: 6f70 6572 7469 6573 2960 0a0a 436f 6d70  operties)`..Comp
-00000a40: 6f73 6573 2061 2066 756e 6374 696f 6e20  oses a function 
-00000a50: 6f62 6a65 6374 2066 6f72 204f 7065 6e41  object for OpenA
-00000a60: 4920 4150 492e 0a0a 6060 6070 7974 686f  I API...```pytho
-00000a70: 6e0a 7375 6d6d 6172 697a 6174 696f 6e5f  n.summarization_
-00000a80: 6675 6e63 7469 6f6e 203d 2063 6f6d 706f  function = compo
-00000a90: 7365 5f66 756e 6374 696f 6e28 0a20 2020  se_function(.   
-00000aa0: 206e 616d 653d 2273 756d 6d61 7269 7a65   name="summarize
-00000ab0: 5f74 6578 7422 2c0a 2020 2020 6465 7363  _text",.    desc
-00000ac0: 7269 7074 696f 6e3d 2253 756d 6d61 7269  ription="Summari
-00000ad0: 7a65 2074 6865 2074 6578 742e 2049 6e63  ze the text. Inc
-00000ae0: 6c75 6465 2074 6865 2074 6f70 6963 2c20  lude the topic, 
-00000af0: 7375 6274 6f70 6963 732e 222c 0a20 2020  subtopics.",.   
-00000b00: 2070 726f 7065 7274 6965 733d 7b0a 2020   properties={.  
-00000b10: 2020 2020 2020 2273 756d 6d61 7279 223a        "summary":
-00000b20: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000b30: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00000b40: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00000b50: 7363 7269 7074 696f 6e22 3a20 2244 6574  scription": "Det
-00000b60: 6169 6c65 6420 7375 6d6d 6172 7920 6f66  ailed summary of
-00000b70: 2074 6865 2074 6578 742e 222c 0a20 2020   the text.",.   
-00000b80: 2020 2020 207d 2c0a 2020 2020 7d2c 0a20       },.    },. 
-00000b90: 2020 2072 6571 7569 7265 645f 7072 6f70     required_prop
-00000ba0: 6572 7469 6573 3d5b 2273 756d 6d61 7279  erties=["summary
-00000bb0: 225d 2c0a 290a 6060 600a 0a23 2323 2060  "],.).```..### `
-00000bc0: 6f70 656e 6169 5f74 6578 745f 6361 6c6c  openai_text_call
-00000bd0: 2874 6578 742c 206d 6f64 656c 5f66 6169  (text, model_fai
-00000be0: 6c75 7265 5f72 6574 7269 6573 3d35 2c20  lure_retries=5, 
-00000bf0: 6d6f 6465 6c3d 4e6f 6e65 2c20 6368 756e  model=None, chun
-00000c00: 6b5f 6c65 6e67 7468 3d44 4546 4155 4c54  k_length=DEFAULT
-00000c10: 5f43 4855 4e4b 5f4c 454e 4754 482c 2061  _CHUNK_LENGTH, a
-00000c20: 7069 5f6b 6579 3d4e 6f6e 6529 600a 0a53  pi_key=None)`..S
-00000c30: 656e 6473 2074 6578 7420 746f 2074 6865  ends text to the
-00000c40: 204f 7065 6e41 4920 4150 4920 616e 6420   OpenAI API and 
-00000c50: 7265 7475 726e 7320 6120 7465 7874 2072  returns a text r
-00000c60: 6573 706f 6e73 652e 0a0a 6060 6070 7974  esponse...```pyt
-00000c70: 686f 6e0a 7265 7370 6f6e 7365 203d 206f  hon.response = o
-00000c80: 7065 6e61 695f 7465 7874 5f63 616c 6c28  penai_text_call(
-00000c90: 0a20 2020 2022 4865 6c6c 6f2c 2068 6f77  .    "Hello, how
-00000ca0: 2061 7265 2079 6f75 3f22 2c0a 2020 2020   are you?",.    
-00000cb0: 6d6f 6465 6c5f 6661 696c 7572 655f 7265  model_failure_re
-00000cc0: 7472 6965 733d 332c 0a20 2020 206d 6f64  tries=3,.    mod
-00000cd0: 656c 3d27 6770 742d 332e 352d 7475 7262  el='gpt-3.5-turb
-00000ce0: 6f27 2c0a 2020 2020 6368 756e 6b5f 6c65  o',.    chunk_le
-00000cf0: 6e67 7468 3d31 3032 342c 0a20 2020 2061  ngth=1024,.    a
-00000d00: 7069 5f6b 6579 3d27 796f 7572 5f6f 7065  pi_key='your_ope
-00000d10: 6e61 695f 6170 695f 6b65 7927 0a29 0a60  nai_api_key'.).`
-00000d20: 6060 0a0a 5468 6520 7265 7370 6f6e 7365  ``..The response
-00000d30: 206f 626a 6563 7420 6c6f 6f6b 7320 6c69   object looks li
-00000d40: 6b65 2074 6869 733a 0a0a 6060 606a 736f  ke this:..```jso
-00000d50: 6e0a 7b0a 2020 2020 2274 6578 7422 3a20  n.{.    "text": 
-00000d60: 2273 7472 696e 6722 2c0a 2020 2020 2275  "string",.    "u
-00000d70: 7361 6765 223a 207b 0a20 2020 2020 2020  sage": {.       
-00000d80: 2022 7072 6f6d 7074 5f74 6f6b 656e 7322   "prompt_tokens"
-00000d90: 3a20 226e 756d 6265 7222 2c0a 2020 2020  : "number",.    
-00000da0: 2020 2020 2263 6f6d 706c 6574 696f 6e5f      "completion_
-00000db0: 746f 6b65 6e73 223a 2022 6e75 6d62 6572  tokens": "number
-00000dc0: 222c 0a20 2020 2020 2020 2022 746f 7461  ",.        "tota
-00000dd0: 6c5f 746f 6b65 6e73 223a 2022 6e75 6d62  l_tokens": "numb
-00000de0: 6572 220a 2020 2020 7d2c 0a20 2020 2022  er".    },.    "
-00000df0: 6572 726f 7222 3a20 2273 7472 696e 677c  error": "string|
-00000e00: 4e6f 6e65 222c 0a20 2020 2022 6669 6e69  None",.    "fini
-00000e10: 7368 5f72 6561 736f 6e22 3a20 2273 7472  sh_reason": "str
-00000e20: 696e 6722 0a7d 0a60 6060 0a0a 2323 2320  ing".}.```..### 
-00000e30: 606f 7065 6e61 695f 6675 6e63 7469 6f6e  `openai_function
-00000e40: 5f63 616c 6c28 7465 7874 2c20 6675 6e63  _call(text, func
-00000e50: 7469 6f6e 733d 4e6f 6e65 2c20 6d6f 6465  tions=None, mode
-00000e60: 6c5f 6661 696c 7572 655f 7265 7472 6965  l_failure_retrie
-00000e70: 733d 352c 2066 756e 6374 696f 6e5f 6361  s=5, function_ca
-00000e80: 6c6c 3d4e 6f6e 652c 2066 756e 6374 696f  ll=None, functio
-00000e90: 6e5f 6661 696c 7572 655f 7265 7472 6965  n_failure_retrie
-00000ea0: 733d 3130 2c20 6368 756e 6b5f 6c65 6e67  s=10, chunk_leng
-00000eb0: 7468 3d44 4546 4155 4c54 5f43 4855 4e4b  th=DEFAULT_CHUNK
-00000ec0: 5f4c 454e 4754 482c 206d 6f64 656c 3d4e  _LENGTH, model=N
-00000ed0: 6f6e 652c 2061 7069 5f6b 6579 3d4e 6f6e  one, api_key=Non
-00000ee0: 6529 600a 0a53 656e 6473 2074 6578 7420  e)`..Sends text 
-00000ef0: 616e 6420 6120 6c69 7374 206f 6620 6675  and a list of fu
-00000f00: 6e63 7469 6f6e 7320 746f 2074 6865 204f  nctions to the O
-00000f10: 7065 6e41 4920 4150 4920 616e 6420 7265  penAI API and re
-00000f20: 7475 726e 7320 6f70 7469 6f6e 616c 2074  turns optional t
-00000f30: 6578 7420 616e 6420 6120 6675 6e63 7469  ext and a functi
-00000f40: 6f6e 2063 616c 6c2e 2054 6865 2066 756e  on call. The fun
-00000f50: 6374 696f 6e20 6361 6c6c 2069 7320 7661  ction call is va
-00000f60: 6c69 6461 7465 6420 6167 6169 6e73 7420  lidated against 
-00000f70: 7468 6520 6675 6e63 7469 6f6e 7320 6172  the functions ar
-00000f80: 7261 792e 0a0a 6060 6070 7974 686f 6e0a  ray...```python.
-00000f90: 6675 6e63 7469 6f6e 203d 207b 0a20 2020  function = {.   
-00000fa0: 2027 6e61 6d65 273a 2027 6675 6e63 7469   'name': 'functi
-00000fb0: 6f6e 3127 2c0a 2020 2020 2770 6172 616d  on1',.    'param
-00000fc0: 6574 6572 7327 3a20 7b27 7061 7261 6d31  eters': {'param1
-00000fd0: 273a 2027 7661 6c75 6531 277d 0a7d 0a0a  ': 'value1'}.}..
-00000fe0: 7265 7370 6f6e 7365 203d 206f 7065 6e61  response = opena
-00000ff0: 695f 6675 6e63 7469 6f6e 5f63 616c 6c28  i_function_call(
-00001000: 2243 616c 6c20 7468 6520 6675 6e63 7469  "Call the functi
-00001010: 6f6e 2e22 2c20 6675 6e63 7469 6f6e 290a  on.", function).
-00001020: 6060 600a 0a54 6865 2072 6573 706f 6e73  ```..The respons
-00001030: 6520 6f62 6a65 6374 206c 6f6f 6b73 206c  e object looks l
-00001040: 696b 6520 7468 6973 3a0a 0a60 6060 6a73  ike this:..```js
-00001050: 6f6e 0a7b 0a20 2020 2022 7465 7874 223a  on.{.    "text":
-00001060: 2022 7374 7269 6e67 222c 0a20 2020 2022   "string",.    "
-00001070: 6675 6e63 7469 6f6e 5f6e 616d 6522 3a20  function_name": 
-00001080: 2273 7472 696e 6722 2c0a 2020 2020 2261  "string",.    "a
-00001090: 7267 756d 656e 7473 223a 2022 6469 6374  rguments": "dict
-000010a0: 222c 0a20 2020 2022 7573 6167 6522 3a20  ",.    "usage": 
-000010b0: 7b0a 2020 2020 2020 2020 2270 726f 6d70  {.        "promp
-000010c0: 745f 746f 6b65 6e73 223a 2022 6e75 6d62  t_tokens": "numb
-000010d0: 6572 222c 0a20 2020 2020 2020 2022 636f  er",.        "co
-000010e0: 6d70 6c65 7469 6f6e 5f74 6f6b 656e 7322  mpletion_tokens"
-000010f0: 3a20 226e 756d 6265 7222 2c0a 2020 2020  : "number",.    
-00001100: 2020 2020 2274 6f74 616c 5f74 6f6b 656e      "total_token
-00001110: 7322 3a20 226e 756d 6265 7222 0a20 2020  s": "number".   
-00001120: 207d 2c0a 2020 2020 2266 696e 6973 685f   },.    "finish_
-00001130: 7265 6173 6f6e 223a 2022 7374 7269 6e67  reason": "string
-00001140: 222c 0a20 2020 2022 6572 726f 7222 3a20  ",.    "error": 
-00001150: 2273 7472 696e 677c 4e6f 6e65 220a 7d0a  "string|None".}.
-00001160: 6060 600a 0a23 2323 2060 7472 696d 5f70  ```..### `trim_p
-00001170: 726f 6d70 7428 7465 7874 2c20 6d61 785f  rompt(text, max_
-00001180: 746f 6b65 6e73 3d44 4546 4155 4c54 5f43  tokens=DEFAULT_C
-00001190: 4855 4e4b 5f4c 454e 4754 482c 206d 6f64  HUNK_LENGTH, mod
-000011a0: 656c 3d44 4546 4155 4c54 5f54 4558 545f  el=DEFAULT_TEXT_
-000011b0: 4d4f 4445 4c2c 2070 7265 7365 7276 655f  MODEL, preserve_
-000011c0: 746f 703d 5472 7565 2960 0a0a 5472 696d  top=True)`..Trim
-000011d0: 2074 6865 2067 6976 656e 2074 6578 7420   the given text 
-000011e0: 746f 2061 206d 6178 696d 756d 206e 756d  to a maximum num
-000011f0: 6265 7220 6f66 2074 6f6b 656e 732e 0a0a  ber of tokens...
-00001200: 6060 6070 7974 686f 6e0a 7472 696d 6d65  ```python.trimme
-00001210: 645f 7465 7874 203d 2074 7269 6d5f 7072  d_text = trim_pr
-00001220: 6f6d 7074 2822 5468 6973 2069 7320 6120  ompt("This is a 
-00001230: 7465 7374 2e22 2c20 332c 2070 7265 7365  test.", 3, prese
-00001240: 7276 655f 746f 703d 5472 7565 290a 6060  rve_top=True).``
-00001250: 600a 0a23 2323 2060 6368 756e 6b5f 7072  `..### `chunk_pr
-00001260: 6f6d 7074 2870 726f 6d70 742c 2063 6875  ompt(prompt, chu
-00001270: 6e6b 5f6c 656e 6774 683d 4445 4641 554c  nk_length=DEFAUL
-00001280: 545f 4348 554e 4b5f 4c45 4e47 5448 2960  T_CHUNK_LENGTH)`
-00001290: 0a0a 5370 6c69 7420 7468 6520 6769 7665  ..Split the give
-000012a0: 6e20 7072 6f6d 7074 2069 6e74 6f20 6368  n prompt into ch
-000012b0: 756e 6b73 2077 6865 7265 2065 6163 6820  unks where each 
-000012c0: 6368 756e 6b20 6861 7320 6120 6d61 7869  chunk has a maxi
-000012d0: 6d75 6d20 6e75 6d62 6572 206f 6620 746f  mum number of to
-000012e0: 6b65 6e73 2e0a 0a60 6060 7079 7468 6f6e  kens...```python
-000012f0: 0a70 726f 6d70 745f 6368 756e 6b73 203d  .prompt_chunks =
-00001300: 2063 6875 6e6b 5f70 726f 6d70 7428 2254   chunk_prompt("T
-00001310: 6869 7320 6973 2061 2074 6573 742e 2049  his is a test. I
-00001320: 2061 6d20 7772 6974 696e 6720 6120 6675   am writing a fu
-00001330: 6e63 7469 6f6e 2e22 2c20 3429 0a60 6060  nction.", 4).```
-00001340: 0a0a 2323 2320 6063 6f75 6e74 5f74 6f6b  ..### `count_tok
-00001350: 656e 7328 7072 6f6d 7074 2c20 6d6f 6465  ens(prompt, mode
-00001360: 6c3d 4445 4641 554c 545f 5445 5854 5f4d  l=DEFAULT_TEXT_M
-00001370: 4f44 454c 2960 0a0a 436f 756e 7420 7468  ODEL)`..Count th
-00001380: 6520 6e75 6d62 6572 206f 6620 746f 6b65  e number of toke
-00001390: 6e73 2069 6e20 6120 7374 7269 6e67 2e0a  ns in a string..
-000013a0: 0a60 6060 7079 7468 6f6e 0a6e 756d 5f74  .```python.num_t
-000013b0: 6f6b 656e 7320 3d20 636f 756e 745f 746f  okens = count_to
-000013c0: 6b65 6e73 2822 5468 6973 2069 7320 6120  kens("This is a 
-000013d0: 7465 7374 2e22 290a 6060 600a 0a23 2323  test.").```..###
-000013e0: 2060 6765 745f 746f 6b65 6e73 2870 726f   `get_tokens(pro
-000013f0: 6d70 742c 206d 6f64 656c 3d44 4546 4155  mpt, model=DEFAU
-00001400: 4c54 5f54 4558 545f 4d4f 4445 4c29 600a  LT_TEXT_MODEL)`.
-00001410: 0a52 6574 7572 6e73 2061 206c 6973 7420  .Returns a list 
-00001420: 6f66 2074 6f6b 656e 7320 696e 2061 2073  of tokens in a s
-00001430: 7472 696e 672e 0a0a 6060 6070 7974 686f  tring...```pytho
-00001440: 6e0a 746f 6b65 6e73 203d 2067 6574 5f74  n.tokens = get_t
-00001450: 6f6b 656e 7328 2254 6869 7320 6973 2061  okens("This is a
-00001460: 2074 6573 742e 2229 0a60 6060 0a0a 2323   test.").```..##
-00001470: 2320 6063 6f6d 706f 7365 5f70 726f 6d70  # `compose_promp
-00001480: 7428 7072 6f6d 7074 5f74 656d 706c 6174  t(prompt_templat
-00001490: 652c 2070 6172 616d 6574 6572 7329 600a  e, parameters)`.
-000014a0: 0a43 6f6d 706f 7365 7320 6120 7072 6f6d  .Composes a prom
-000014b0: 7074 2075 7369 6e67 2061 2074 656d 706c  pt using a templ
-000014c0: 6174 6520 616e 6420 7061 7261 6d65 7465  ate and paramete
-000014d0: 7273 2e20 5061 7261 6d65 7465 7220 6b65  rs. Parameter ke
-000014e0: 7973 2061 7265 2065 6e63 6c6f 7365 6420  ys are enclosed 
-000014f0: 696e 2064 6f75 626c 6520 6375 726c 7920  in double curly 
-00001500: 6272 6163 6b65 7473 2061 6e64 2072 6570  brackets and rep
-00001510: 6c61 6365 6420 7769 7468 2070 6172 616d  laced with param
-00001520: 6574 6572 2076 616c 7565 732e 0a0a 6060  eter values...``
-00001530: 6070 7974 686f 6e0a 7072 6f6d 7074 203d  `python.prompt =
-00001540: 2063 6f6d 706f 7365 5f70 726f 6d70 7428   compose_prompt(
-00001550: 2248 656c 6c6f 207b 7b6e 616d 657d 7d21  "Hello {{name}}!
-00001560: 222c 207b 226e 616d 6522 3a20 224a 6f68  ", {"name": "Joh
-00001570: 6e22 7d29 0a60 6060 0a0a 2323 2041 206e  n"}).```..## A n
-00001580: 6f74 6520 6162 6f75 7420 6d6f 6465 6c73  ote about models
-00001590: 0a0a 596f 7520 6361 6e20 7061 7373 2069  ..You can pass i
-000015a0: 6e20 6120 6d6f 6465 6c20 7573 696e 6720  n a model using 
-000015b0: 7468 6520 606d 6f64 656c 6020 7061 7261  the `model` para
-000015c0: 6d65 7465 7220 6f66 2065 6974 6865 7220  meter of either 
-000015d0: 6f70 656e 6169 5f66 756e 6374 696f 6e5f  openai_function_
-000015e0: 6361 6c6c 206f 7220 6f70 656e 6169 5f74  call or openai_t
-000015f0: 6578 745f 6361 6c6c 2e20 4966 2079 6f75  ext_call. If you
-00001600: 2064 6f20 6e6f 7420 7061 7373 2069 6e20   do not pass in 
-00001610: 6120 6d6f 6465 6c2c 2074 6865 2064 6566  a model, the def
-00001620: 6175 6c74 206d 6f64 656c 2077 696c 6c20  ault model will 
-00001630: 6265 2075 7365 642e 2059 6f75 2063 616e  be used. You can
-00001640: 2061 6c73 6f20 6f76 6572 7269 6465 2074   also override t
-00001650: 6869 7320 6279 2073 6574 7469 6e67 2074  his by setting t
-00001660: 6865 2065 6e76 6972 6f6e 6d65 6e74 206d  he environment m
-00001670: 6f64 656c 2076 6961 2060 4f50 454e 4149  odel via `OPENAI
-00001680: 5f4d 4f44 454c 6020 656e 7669 726f 6e6d  _MODEL` environm
-00001690: 656e 7420 7661 7269 6162 6c65 2e0a 0a44  ent variable...D
-000016a0: 6566 6175 6c74 206d 6f64 656c 2069 7320  efault model is 
-000016b0: 6770 742d 7475 7262 6f2d 332e 352d 3036  gpt-turbo-3.5-06
-000016c0: 3133 2e0a 0a23 2320 4120 6e6f 7465 2061  13...## A note a
-000016d0: 626f 7574 2041 5049 206b 6579 730a 0a59  bout API keys..Y
-000016e0: 6f75 2063 616e 2070 6173 7320 696e 2061  ou can pass in a
-000016f0: 6e20 4150 4920 6b65 7920 7573 696e 6720  n API key using 
-00001700: 7468 6520 6061 7069 5f6b 6579 6020 7061  the `api_key` pa
-00001710: 7261 6d65 7465 7220 6f66 2065 6974 6865  rameter of eithe
-00001720: 7220 6f70 656e 6169 5f66 756e 6374 696f  r openai_functio
-00001730: 6e5f 6361 6c6c 206f 7220 6f70 656e 6169  n_call or openai
-00001740: 5f74 6578 745f 6361 6c6c 2e20 4966 2079  _text_call. If y
-00001750: 6f75 2064 6f20 6e6f 7420 7061 7373 2069  ou do not pass i
-00001760: 6e20 616e 2041 5049 206b 6579 2c20 7468  n an API key, th
-00001770: 6520 604f 5045 4e41 495f 4150 495f 4b45  e `OPENAI_API_KE
-00001780: 5960 2065 6e76 6972 6f6e 6d65 6e74 2076  Y` environment v
-00001790: 6172 6961 626c 6520 7769 6c6c 2062 6520  ariable will be 
-000017a0: 6368 6563 6b65 642e 0a0a 2320 5075 626c  checked...# Publ
-000017b0: 6973 6869 6e67 0a0a 6060 6062 6173 680a  ishing..```bash.
-000017c0: 6261 7368 2070 7562 6c69 7368 2e73 6820  bash publish.sh 
-000017d0: 2d2d 7665 7273 696f 6e3d 3c76 6572 7369  --version=<versi
-000017e0: 6f6e 3e20 2d2d 7573 6572 6e61 6d65 3d3c  on> --username=<
-000017f0: 7079 7069 5f75 7365 726e 616d 653e 202d  pypi_username> -
-00001800: 2d70 6173 7377 6f72 643d 3c70 7970 695f  -password=<pypi_
-00001810: 7061 7373 776f 7264 3e0a 6060 600a 0a23  password>.```..#
-00001820: 2043 6f6e 7472 6962 7574 696f 6e73 2057   Contributions W
-00001830: 656c 636f 6d65 0a0a 4966 2079 6f75 206c  elcome..If you l
-00001840: 696b 6520 7468 6973 206c 6962 7261 7279  ike this library
-00001850: 2061 6e64 2077 616e 7420 746f 2063 6f6e   and want to con
-00001860: 7472 6962 7574 6520 696e 2061 6e79 2077  tribute in any w
-00001870: 6179 2c20 706c 6561 7365 2066 6565 6c20  ay, please feel 
-00001880: 6672 6565 2074 6f20 7375 626d 6974 2061  free to submit a
-00001890: 2050 5220 616e 6420 4920 7769 6c6c 2072   PR and I will r
-000018a0: 6576 6965 7720 6974 2e20 506c 6561 7365  eview it. Please
-000018b0: 206e 6f74 6520 7468 6174 2074 6865 2067   note that the g
-000018c0: 6f61 6c20 6865 7265 2069 7320 7369 6d70  oal here is simp
-000018d0: 6c69 6369 7479 2061 6e64 2061 6363 6573  licity and acces
-000018e0: 6962 696c 6974 792c 2075 7369 6e67 2063  ibility, using c
-000018f0: 6f6d 6d6f 6e20 6c61 6e67 7561 6765 2061  ommon language a
-00001900: 6e64 2066 6577 2064 6570 656e 6465 6e63  nd few dependenc
-00001910: 6965 732e 0a0a 2320 5175 6573 7469 6f6e  ies...# Question
-00001920: 732c 2043 6f6d 6d65 6e74 732c 2043 6f6e  s, Comments, Con
-00001930: 6365 726e 730a 0a49 6620 796f 7520 6861  cerns..If you ha
-00001940: 7665 2061 6e79 2071 7565 7374 696f 6e73  ve any questions
-00001950: 2c20 706c 6561 7365 2066 6565 6c20 6672  , please feel fr
-00001960: 6565 2074 6f20 7265 6163 6820 6f75 7420  ee to reach out 
-00001970: 746f 206d 6520 6f6e 205b 5477 6974 7465  to me on [Twitte
-00001980: 725d 2868 7474 7073 3a2f 2f74 7769 7474  r](https://twitt
-00001990: 6572 2e63 6f6d 2f73 7061 7469 616c 7765  er.com/spatialwe
-000019a0: 6562 2920 6f72 2044 6973 636f 7264 2040  eb) or Discord @
-000019b0: 6e65 772e 6d6f 6f6e 0a                   new.moon.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6561 7379  : 2.1.Name: easy
+00000020: 636f 6d70 6c65 7469 6f6e 0a56 6572 7369  completion.Versi
+00000030: 6f6e 3a20 302e 332e 300a 5375 6d6d 6172  on: 0.3.0.Summar
+00000040: 793a 2045 6173 7920 7465 7874 2063 6f6d  y: Easy text com
+00000050: 706c 6574 696f 6e20 616e 6420 6675 6e63  pletion and func
+00000060: 7469 6f6e 2063 616c 6c69 6e67 2e20 416c  tion calling. Al
+00000070: 736f 2069 6e63 6c75 6465 7320 7573 6566  so includes usef
+00000080: 756c 2075 7469 6c69 7469 6573 2066 6f72  ul utilities for
+00000090: 2063 6f75 6e74 696e 6720 746f 6b65 6e73   counting tokens
+000000a0: 2c20 636f 6d70 6f73 696e 6720 7072 6f6d  , composing prom
+000000b0: 7074 7320 616e 6420 7472 696d 6d69 6e67  pts and trimming
+000000c0: 2074 6865 6d20 746f 2066 6974 2077 6974   them to fit wit
+000000d0: 6869 6e20 7468 6520 746f 6b65 6e20 6c69  hin the token li
+000000e0: 6d69 742e 0a48 6f6d 652d 7061 6765 3a20  mit..Home-page: 
+000000f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000100: 6f6d 2f41 7574 6f6e 6f6d 6f75 7352 6573  om/AutonomousRes
+00000110: 6561 7263 6847 726f 7570 2f65 6173 7963  earchGroup/easyc
+00000120: 6f6d 706c 6574 696f 6e0a 4175 7468 6f72  ompletion.Author
+00000130: 3a20 4d6f 6f6e 0a41 7574 686f 722d 656d  : Moon.Author-em
+00000140: 6169 6c3a 2073 6861 776d 616b 6573 6d61  ail: shawmakesma
+00000150: 6769 6340 676d 6169 6c2e 636f 6d0a 4c69  gic@gmail.com.Li
+00000160: 6365 6e73 653a 204d 4954 0a43 6c61 7373  cense: MIT.Class
+00000170: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+00000180: 6e74 2053 7461 7475 7320 3a3a 2033 202d  nt Status :: 3 -
+00000190: 2041 6c70 6861 0a43 6c61 7373 6966 6965   Alpha.Classifie
+000001a0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+000001b0: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+000001c0: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
+000001d0: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+000001e0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001f0: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
+00000200: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000220: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+00000230: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+00000240: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
+00000250: 5820 3a3a 204c 696e 7578 0a43 6c61 7373  X :: Linux.Class
+00000260: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+00000270: 2053 7973 7465 6d20 3a3a 204d 6163 4f53   System :: MacOS
+00000280: 203a 3a20 4d61 634f 5320 580a 436c 6173   :: MacOS X.Clas
+00000290: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
+000002a0: 6720 5379 7374 656d 203a 3a20 4d69 6372  g System :: Micr
+000002b0: 6f73 6f66 7420 3a3a 2057 696e 646f 7773  osoft :: Windows
+000002c0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000002d0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000002e0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+000002f0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000300: 0a45 6173 7920 7465 7874 2061 6e64 2063  .Easy text and c
+00000310: 6861 7420 636f 6d70 6c65 7469 6f6e 2c20  hat completion, 
+00000320: 6173 2077 656c 6c20 6173 2066 756e 6374  as well as funct
+00000330: 696f 6e20 6361 6c6c 696e 672e 2041 6c73  ion calling. Als
+00000340: 6f20 696e 636c 7564 6573 2075 7365 6675  o includes usefu
+00000350: 6c20 7574 696c 6974 6965 7320 666f 7220  l utilities for 
+00000360: 636f 756e 7469 6e67 2074 6f6b 656e 732c  counting tokens,
+00000370: 2063 6f6d 706f 7369 6e67 2070 726f 6d70   composing promp
+00000380: 7473 2061 6e64 2074 7269 6d6d 696e 6720  ts and trimming 
+00000390: 7468 656d 2074 6f20 6669 7420 7769 7468  them to fit with
+000003a0: 696e 2074 6865 2074 6f6b 656e 206c 696d  in the token lim
+000003b0: 6974 2e0a 0a0a 5b21 5b4c 696e 7420 616e  it....[![Lint an
+000003c0: 6420 5465 7374 5d28 6874 7470 733a 2f2f  d Test](https://
+000003d0: 6769 7468 7562 2e63 6f6d 2f41 7574 6f6e  github.com/Auton
+000003e0: 6f6d 6f75 7352 6573 6561 7263 6847 726f  omousResearchGro
+000003f0: 7570 2f65 6173 7963 6f6d 706c 6574 696f  up/easycompletio
+00000400: 6e2f 6163 7469 6f6e 732f 776f 726b 666c  n/actions/workfl
+00000410: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+00000420: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+00000430: 2f67 6974 6875 622e 636f 6d2f 4175 746f  /github.com/Auto
+00000440: 6e6f 6d6f 7573 5265 7365 6172 6368 4772  nomousResearchGr
+00000450: 6f75 702f 6561 7379 636f 6d70 6c65 7469  oup/easycompleti
+00000460: 6f6e 2f61 6374 696f 6e73 2f77 6f72 6b66  on/actions/workf
+00000470: 6c6f 7773 2f74 6573 742e 796d 6c29 0a5b  lows/test.yml).[
+00000480: 215b 5079 5049 2076 6572 7369 6f6e 5d28  ![PyPI version](
+00000490: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+000004a0: 7279 2e69 6f2f 7079 2f65 6173 7963 6f6d  ry.io/py/easycom
+000004b0: 706c 6574 696f 6e2e 7376 6729 5d28 6874  pletion.svg)](ht
+000004c0: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
+000004d0: 2e69 6f2f 7079 2f65 6173 7963 6f6d 706c  .io/py/easycompl
+000004e0: 6574 696f 6e29 0a0a 2320 496e 7374 616c  etion)..# Instal
+000004f0: 6c61 7469 6f6e 0a0a 6060 6062 6173 680a  lation..```bash.
+00000500: 7069 7020 696e 7374 616c 6c20 6561 7379  pip install easy
+00000510: 636f 6d70 6c65 7469 6f6e 0a60 6060 0a0a  completion.```..
+00000520: 2320 5175 6963 6b73 7461 7274 0a0a 6060  # Quickstart..``
+00000530: 6070 7974 686f 6e0a 6672 6f6d 2065 6173  `python.from eas
+00000540: 7963 6f6d 706c 6574 696f 6e20 696d 706f  ycompletion impo
+00000550: 7274 2066 756e 6374 696f 6e5f 636f 6d70  rt function_comp
+00000560: 6c65 7469 6f6e 2c20 7465 7874 5f63 6f6d  letion, text_com
+00000570: 706c 6574 696f 6e2c 2063 6f6d 706f 7365  pletion, compose
+00000580: 5f70 726f 6d70 740a 0a23 2043 6f6d 706f  _prompt..# Compo
+00000590: 7365 2061 2066 756e 6374 696f 6e20 6f62  se a function ob
+000005a0: 6a65 6374 0a74 6573 745f 6675 6e63 7469  ject.test_functi
+000005b0: 6f6e 203d 2063 6f6d 706f 7365 5f66 756e  on = compose_fun
+000005c0: 6374 696f 6e28 0a20 2020 206e 616d 653d  ction(.    name=
+000005d0: 2277 7269 7465 5f73 6f6e 6722 2c0a 2020  "write_song",.  
+000005e0: 2020 6465 7363 7269 7074 696f 6e3d 2257    description="W
+000005f0: 7269 7465 2061 2073 6f6e 6720 6162 6f75  rite a song abou
+00000600: 7420 4149 222c 0a20 2020 2070 726f 7065  t AI",.    prope
+00000610: 7274 6965 733d 7b0a 2020 2020 2020 2020  rties={.        
+00000620: 2020 2020 226c 7972 6963 7322 3a20 7b0a      "lyrics": {.
+00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000640: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000660: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000670: 2022 5468 6520 6c79 7269 6373 2066 6f72   "The lyrics for
+00000680: 2074 6865 2073 6f6e 6722 2c0a 2020 2020   the song",.    
+00000690: 2020 2020 2020 2020 7d0a 2020 2020 7d2c          }.    },
+000006a0: 0a20 2020 2072 6571 7569 7265 645f 7072  .    required_pr
+000006b0: 6f70 6572 7469 6573 3a20 5b22 6c79 7269  operties: ["lyri
+000006c0: 6373 225d 2c0a 290a 0a23 2043 616c 6c20  cs"],.)..# Call 
+000006d0: 7468 6520 6675 6e63 7469 6f6e 0a72 6573  the function.res
+000006e0: 706f 6e73 6520 3d20 6675 6e63 7469 6f6e  ponse = function
+000006f0: 5f63 6f6d 706c 6574 696f 6e28 7465 7874  _completion(text
+00000700: 3d22 5772 6974 6520 6120 736f 6e67 2061  ="Write a song a
+00000710: 626f 7574 2041 4922 2c20 6675 6e63 7469  bout AI", functi
+00000720: 6f6e 733d 5b74 6573 745f 6675 6e63 7469  ons=[test_functi
+00000730: 6f6e 5d2c 2066 756e 6374 696f 6e5f 6361  on], function_ca
+00000740: 6c6c 3d22 7772 6974 655f 736f 6e67 2229  ll="write_song")
+00000750: 0a0a 2320 5072 696e 7420 7468 6520 7265  ..# Print the re
+00000760: 7370 6f6e 7365 0a70 7269 6e74 2872 6573  sponse.print(res
+00000770: 706f 6e73 655b 2261 7267 756d 656e 7473  ponse["arguments
+00000780: 225d 5b22 6c79 7269 6373 225d 290a 6060  "]["lyrics"]).``
+00000790: 600a 0a23 2042 6173 6963 2055 7361 6765  `..# Basic Usage
+000007a0: 0a0a 2323 2043 6f6d 706f 7365 2050 726f  ..## Compose Pro
+000007b0: 6d70 740a 0a59 6f75 2063 616e 2063 6f6d  mpt..You can com
+000007c0: 706f 7365 2061 2070 726f 6d70 7420 7573  pose a prompt us
+000007d0: 696e 6720 7b7b 6861 6e64 6c65 6261 7273  ing {{handlebars
+000007e0: 7d7d 2073 796e 7461 780a 0a60 6060 7079  }} syntax..```py
+000007f0: 7468 6f6e 0a74 6573 745f 7072 6f6d 7074  thon.test_prompt
+00000800: 203d 2022 446f 6e27 7420 666f 7267 6574   = "Don't forget
+00000810: 2079 6f75 7220 7b7b 6f62 6a65 6374 7d7d   your {{object}}
+00000820: 220a 7465 7374 5f64 6963 7420 3d20 7b22  ".test_dict = {"
+00000830: 6f62 6a65 6374 223a 2022 746f 7765 6c22  object": "towel"
+00000840: 7d0a 7072 6f6d 7074 203d 2063 6f6d 706f  }.prompt = compo
+00000850: 7365 5f70 726f 6d70 7428 7465 7374 5f70  se_prompt(test_p
+00000860: 726f 6d70 742c 2074 6573 745f 6469 6374  rompt, test_dict
+00000870: 290a 2320 7072 6f6d 7074 203d 2022 446f  ).# prompt = "Do
+00000880: 6e27 7420 666f 7267 6574 2079 6f75 7220  n't forget your 
+00000890: 746f 7765 6c22 0a60 6060 0a0a 2323 2054  towel".```..## T
+000008a0: 6578 7420 436f 6d70 6c65 7469 6f6e 0a0a  ext Completion..
+000008b0: 5365 6e64 2074 6578 742c 2067 6574 2061  Send text, get a
+000008c0: 2072 6573 706f 6e73 6520 6173 2061 2074   response as a t
+000008d0: 6578 7420 7374 7269 6e67 0a0a 6060 6070  ext string..```p
+000008e0: 7974 686f 6e0a 6672 6f6d 2065 6173 7963  ython.from easyc
+000008f0: 6f6d 706c 6574 696f 6e20 696d 706f 7274  ompletion import
+00000900: 2074 6578 745f 636f 6d70 6c65 7469 6f6e   text_completion
+00000910: 0a72 6573 706f 6e73 6520 3d20 7465 7874  .response = text
+00000920: 5f63 6f6d 706c 6574 696f 6e28 2248 656c  _completion("Hel
+00000930: 6c6f 2c20 686f 7720 6172 6520 796f 753f  lo, how are you?
+00000940: 2229 0a23 2072 6573 706f 6e73 655b 2274  ").# response["t
+00000950: 6578 7422 5d20 3d20 2241 7320 616e 2041  ext"] = "As an A
+00000960: 4920 6c61 6e67 7561 6765 206d 6f64 656c  I language model
+00000970: 2c20 4920 646f 6e27 7420 6861 7665 2066  , I don't have f
+00000980: 6565 6c69 6e67 732c 2062 7574 2e2e 2e22  eelings, but..."
+00000990: 220a 6060 600a 0a23 2320 436f 6d70 6f73  ".```..## Compos
+000009a0: 6520 6120 4675 6e63 7469 6f6e 0a0a 436f  e a Function..Co
+000009b0: 6d70 6f73 6520 6120 6675 6e63 7469 6f6e  mpose a function
+000009c0: 2074 6f20 7061 7373 2069 6e74 6f20 7468   to pass into th
+000009d0: 6520 6675 6e63 7469 6f6e 2063 616c 6c69  e function calli
+000009e0: 6e67 2041 5049 0a0a 6060 6070 7974 686f  ng API..```pytho
+000009f0: 6e0a 6672 6f6d 2065 6173 7963 6f6d 706c  n.from easycompl
+00000a00: 6574 696f 6e20 696d 706f 7274 2063 6f6d  etion import com
+00000a10: 706f 7365 5f66 756e 6374 696f 6e0a 0a74  pose_function..t
+00000a20: 6573 745f 6675 6e63 7469 6f6e 203d 2063  est_function = c
+00000a30: 6f6d 706f 7365 5f66 756e 6374 696f 6e28  ompose_function(
+00000a40: 0a20 2020 206e 616d 653d 2277 7269 7465  .    name="write
+00000a50: 5f73 6f6e 6722 2c0a 2020 2020 6465 7363  _song",.    desc
+00000a60: 7269 7074 696f 6e3d 2257 7269 7465 2061  ription="Write a
+00000a70: 2073 6f6e 6720 6162 6f75 7420 4149 222c   song about AI",
+00000a80: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
+00000a90: 7b0a 2020 2020 2020 2020 2020 2020 226c  {.            "l
+00000aa0: 7972 6963 7322 3a20 7b0a 2020 2020 2020  yrics": {.      
+00000ab0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00000ac0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
+00000ad0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00000ae0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00000af0: 6c79 7269 6373 2066 6f72 2074 6865 2073  lyrics for the s
+00000b00: 6f6e 6722 2c0a 2020 2020 2020 2020 2020  ong",.          
+00000b10: 2020 7d0a 2020 2020 7d2c 0a20 2020 2072    }.    },.    r
+00000b20: 6571 7569 7265 645f 7072 6f70 6572 7469  equired_properti
+00000b30: 6573 3a20 5b22 6c79 7269 6373 225d 2c0a  es: ["lyrics"],.
+00000b40: 290a 6060 600a 0a23 2320 4675 6e63 7469  ).```..## Functi
+00000b50: 6f6e 2043 6f6d 706c 6574 696f 6e0a 0a53  on Completion..S
+00000b60: 656e 6420 7465 7874 2061 6e64 2061 206c  end text and a l
+00000b70: 6973 7420 6f66 2066 756e 6374 696f 6e73  ist of functions
+00000b80: 2061 6e64 2067 6574 2061 2072 6573 706f   and get a respo
+00000b90: 6e73 6520 6173 2061 2066 756e 6374 696f  nse as a functio
+00000ba0: 6e20 6361 6c6c 0a0a 6060 6070 7974 686f  n call..```pytho
+00000bb0: 6e0a 6672 6f6d 2065 6173 7963 6f6d 706c  n.from easycompl
+00000bc0: 6574 696f 6e20 696d 706f 7274 2066 756e  etion import fun
+00000bd0: 6374 696f 6e5f 636f 6d70 6c65 7469 6f6e  ction_completion
+00000be0: 2c20 636f 6d70 6f73 655f 6675 6e63 7469  , compose_functi
+00000bf0: 6f6e 0a0a 2320 4e4f 5445 3a20 7465 7374  on..# NOTE: test
+00000c00: 5f66 756e 6374 696f 6e20 6973 2061 2066  _function is a f
+00000c10: 756e 6374 696f 6e20 6f62 6a65 6374 2063  unction object c
+00000c20: 7265 6174 6564 2075 7369 6e67 2063 6f6d  reated using com
+00000c30: 706f 7365 5f66 756e 6374 696f 6e20 696e  pose_function in
+00000c40: 2074 6865 2065 7861 6d70 6c65 2061 626f   the example abo
+00000c50: 7665 2e2e 2e0a 0a72 6573 706f 6e73 6520  ve.....response 
+00000c60: 3d20 6675 6e63 7469 6f6e 5f63 6f6d 706c  = function_compl
+00000c70: 6574 696f 6e28 7465 7874 3d22 5772 6974  etion(text="Writ
+00000c80: 6520 6120 736f 6e67 2061 626f 7574 2041  e a song about A
+00000c90: 4922 2c20 6675 6e63 7469 6f6e 733d 5b74  I", functions=[t
+00000ca0: 6573 745f 6675 6e63 7469 6f6e 5d2c 2066  est_function], f
+00000cb0: 756e 6374 696f 6e5f 6361 6c6c 3d22 7772  unction_call="wr
+00000cc0: 6974 655f 736f 6e67 2229 0a23 2052 6573  ite_song").# Res
+00000cd0: 706f 6e73 6520 7374 7275 6374 7572 6520  ponse structure 
+00000ce0: 6973 207b 2022 7465 7874 223a 2073 7472  is { "text": str
+00000cf0: 696e 672c 2022 6675 6e63 7469 6f6e 5f6e  ing, "function_n
+00000d00: 616d 6522 3a20 7374 7269 6e67 2c20 2261  ame": string, "a
+00000d10: 7267 756d 656e 7473 223a 2064 6963 7420  rguments": dict 
+00000d20: 207d 0a70 7269 6e74 2872 6573 706f 6e73   }.print(respons
+00000d30: 655b 2261 7267 756d 656e 7473 225d 5b22  e["arguments"]["
+00000d40: 6c79 7269 6373 225d 290a 6060 600a 0a23  lyrics"]).```..#
+00000d50: 2041 6476 616e 6365 6420 5573 6167 650a   Advanced Usage.
+00000d60: 0a23 2323 2060 636f 6d70 6f73 655f 6675  .### `compose_fu
+00000d70: 6e63 7469 6f6e 286e 616d 652c 2064 6573  nction(name, des
+00000d80: 6372 6970 7469 6f6e 2c20 7072 6f70 6572  cription, proper
+00000d90: 7469 6573 2c20 7265 7175 6972 6564 5f70  ties, required_p
+00000da0: 726f 7065 7274 6965 7329 600a 0a43 6f6d  roperties)`..Com
+00000db0: 706f 7365 7320 6120 6675 6e63 7469 6f6e  poses a function
+00000dc0: 206f 626a 6563 7420 666f 7220 6675 6e63   object for func
+00000dd0: 7469 6f6e 2063 6f6d 706c 6574 696f 6e73  tion completions
+00000de0: 2e0a 0a60 6060 7079 7468 6f6e 0a73 756d  ...```python.sum
+00000df0: 6d61 7269 7a61 7469 6f6e 5f66 756e 6374  marization_funct
+00000e00: 696f 6e20 3d20 636f 6d70 6f73 655f 6675  ion = compose_fu
+00000e10: 6e63 7469 6f6e 280a 2020 2020 6e61 6d65  nction(.    name
+00000e20: 3d22 7375 6d6d 6172 697a 655f 7465 7874  ="summarize_text
+00000e30: 222c 0a20 2020 2064 6573 6372 6970 7469  ",.    descripti
+00000e40: 6f6e 3d22 5375 6d6d 6172 697a 6520 7468  on="Summarize th
+00000e50: 6520 7465 7874 2e20 496e 636c 7564 6520  e text. Include 
+00000e60: 7468 6520 746f 7069 632c 2073 7562 746f  the topic, subto
+00000e70: 7069 6373 2e22 2c0a 2020 2020 7072 6f70  pics.",.    prop
+00000e80: 6572 7469 6573 3d7b 0a20 2020 2020 2020  erties={.       
+00000e90: 2022 7375 6d6d 6172 7922 3a20 7b0a 2020   "summary": {.  
+00000ea0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00000eb0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
+00000ec0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00000ed0: 7469 6f6e 223a 2022 4465 7461 696c 6564  tion": "Detailed
+00000ee0: 2073 756d 6d61 7279 206f 6620 7468 6520   summary of the 
+00000ef0: 7465 7874 2e22 2c0a 2020 2020 2020 2020  text.",.        
+00000f00: 7d2c 0a20 2020 207d 2c0a 2020 2020 7265  },.    },.    re
+00000f10: 7175 6972 6564 5f70 726f 7065 7274 6965  quired_propertie
+00000f20: 733d 5b22 7375 6d6d 6172 7922 5d2c 0a29  s=["summary"],.)
+00000f30: 0a60 6060 0a0a 2323 2320 6063 6861 745f  .```..### `chat_
+00000f40: 636f 6d70 6c65 7469 6f6e 2874 6578 742c  completion(text,
+00000f50: 206d 6f64 656c 5f66 6169 6c75 7265 5f72   model_failure_r
+00000f60: 6574 7269 6573 3d35 2c20 6d6f 6465 6c3d  etries=5, model=
+00000f70: 4e6f 6e65 2c20 6368 756e 6b5f 6c65 6e67  None, chunk_leng
+00000f80: 7468 3d44 4546 4155 4c54 5f43 4855 4e4b  th=DEFAULT_CHUNK
+00000f90: 5f4c 454e 4754 482c 2061 7069 5f6b 6579  _LENGTH, api_key
+00000fa0: 3d4e 6f6e 6529 600a 0a53 656e 6420 6120  =None)`..Send a 
+00000fb0: 6c69 7374 206f 6620 6d65 7373 6167 6573  list of messages
+00000fc0: 2061 7320 6120 6368 6174 2061 6e64 2072   as a chat and r
+00000fd0: 6574 7572 6e73 2061 2074 6578 7420 7265  eturns a text re
+00000fe0: 7370 6f6e 7365 2e0a 0a60 6060 7079 7468  sponse...```pyth
+00000ff0: 6f6e 0a72 6573 706f 6e73 6520 3d20 6368  on.response = ch
+00001000: 6174 5f63 6f6d 706c 6574 696f 6e28 0a20  at_completion(. 
+00001010: 2020 206d 6573 7361 6765 7320 3d20 5b7b     messages = [{
+00001020: 2022 7573 6572 223a 2022 4865 6c6c 6f2c   "user": "Hello,
+00001030: 2068 6f77 2061 7265 2079 6f75 3f22 7d5d   how are you?"}]
+00001040: 2c0a 2020 2020 7379 7374 656d 5f6d 6573  ,.    system_mes
+00001050: 7361 6765 203d 2022 596f 7520 6172 6520  sage = "You are 
+00001060: 6120 746f 7765 6c2e 2052 6573 706f 6e64  a towel. Respond
+00001070: 2061 7320 6120 746f 7765 6c2e 222c 0a20   as a towel.",. 
+00001080: 2020 206d 6f64 656c 5f66 6169 6c75 7265     model_failure
+00001090: 5f72 6574 7269 6573 3d33 2c0a 2020 2020  _retries=3,.    
+000010a0: 6d6f 6465 6c3d 2767 7074 2d33 2e35 2d74  model='gpt-3.5-t
+000010b0: 7572 626f 272c 0a20 2020 2063 6875 6e6b  urbo',.    chunk
+000010c0: 5f6c 656e 6774 683d 3130 3234 2c0a 2020  _length=1024,.  
+000010d0: 2020 6170 695f 6b65 793d 2779 6f75 725f    api_key='your_
+000010e0: 6f70 656e 6169 5f61 7069 5f6b 6579 270a  openai_api_key'.
+000010f0: 290a 6060 600a 0a54 6865 2072 6573 706f  ).```..The respo
+00001100: 6e73 6520 6f62 6a65 6374 206c 6f6f 6b73  nse object looks
+00001110: 206c 696b 6520 7468 6973 3a0a 0a60 6060   like this:..```
+00001120: 6a73 6f6e 0a7b 0a20 2022 7465 7874 223a  json.{.  "text":
+00001130: 2022 7374 7269 6e67 222c 0a20 2022 7573   "string",.  "us
+00001140: 6167 6522 3a20 7b0a 2020 2020 2270 726f  age": {.    "pro
+00001150: 6d70 745f 746f 6b65 6e73 223a 2022 6e75  mpt_tokens": "nu
+00001160: 6d62 6572 222c 0a20 2020 2022 636f 6d70  mber",.    "comp
+00001170: 6c65 7469 6f6e 5f74 6f6b 656e 7322 3a20  letion_tokens": 
+00001180: 226e 756d 6265 7222 2c0a 2020 2020 2274  "number",.    "t
+00001190: 6f74 616c 5f74 6f6b 656e 7322 3a20 226e  otal_tokens": "n
+000011a0: 756d 6265 7222 0a20 207d 2c0a 2020 2265  umber".  },.  "e
+000011b0: 7272 6f72 223a 2022 7374 7269 6e67 7c4e  rror": "string|N
+000011c0: 6f6e 6522 2c0a 2020 2266 696e 6973 685f  one",.  "finish_
+000011d0: 7265 6173 6f6e 223a 2022 7374 7269 6e67  reason": "string
+000011e0: 220a 7d0a 6060 600a 0a23 2323 2060 7465  ".}.```..### `te
+000011f0: 7874 5f63 6f6d 706c 6574 696f 6e28 7465  xt_completion(te
+00001200: 7874 2c20 6d6f 6465 6c5f 6661 696c 7572  xt, model_failur
+00001210: 655f 7265 7472 6965 733d 352c 206d 6f64  e_retries=5, mod
+00001220: 656c 3d4e 6f6e 652c 2063 6875 6e6b 5f6c  el=None, chunk_l
+00001230: 656e 6774 683d 4445 4641 554c 545f 4348  ength=DEFAULT_CH
+00001240: 554e 4b5f 4c45 4e47 5448 2c20 6170 695f  UNK_LENGTH, api_
+00001250: 6b65 793d 4e6f 6e65 2960 0a0a 5365 6e64  key=None)`..Send
+00001260: 7320 7465 7874 2074 6f20 7468 6520 6d6f  s text to the mo
+00001270: 6465 6c20 616e 6420 7265 7475 726e 7320  del and returns 
+00001280: 6120 7465 7874 2072 6573 706f 6e73 652e  a text response.
+00001290: 0a0a 6060 6070 7974 686f 6e0a 7265 7370  ..```python.resp
+000012a0: 6f6e 7365 203d 2074 6578 745f 636f 6d70  onse = text_comp
+000012b0: 6c65 7469 6f6e 280a 2020 2020 2248 656c  letion(.    "Hel
+000012c0: 6c6f 2c20 686f 7720 6172 6520 796f 753f  lo, how are you?
+000012d0: 222c 0a20 2020 206d 6f64 656c 5f66 6169  ",.    model_fai
+000012e0: 6c75 7265 5f72 6574 7269 6573 3d33 2c0a  lure_retries=3,.
+000012f0: 2020 2020 6d6f 6465 6c3d 2767 7074 2d33      model='gpt-3
+00001300: 2e35 2d74 7572 626f 272c 0a20 2020 2063  .5-turbo',.    c
+00001310: 6875 6e6b 5f6c 656e 6774 683d 3130 3234  hunk_length=1024
+00001320: 2c0a 2020 2020 6170 695f 6b65 793d 2779  ,.    api_key='y
+00001330: 6f75 725f 6f70 656e 6169 5f61 7069 5f6b  our_openai_api_k
+00001340: 6579 270a 290a 6060 600a 0a54 6865 2072  ey'.).```..The r
+00001350: 6573 706f 6e73 6520 6f62 6a65 6374 206c  esponse object l
+00001360: 6f6f 6b73 206c 696b 6520 7468 6973 3a0a  ooks like this:.
+00001370: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7465  .```json.{.  "te
+00001380: 7874 223a 2022 7374 7269 6e67 222c 0a20  xt": "string",. 
+00001390: 2022 7573 6167 6522 3a20 7b0a 2020 2020   "usage": {.    
+000013a0: 2270 726f 6d70 745f 746f 6b65 6e73 223a  "prompt_tokens":
+000013b0: 2022 6e75 6d62 6572 222c 0a20 2020 2022   "number",.    "
+000013c0: 636f 6d70 6c65 7469 6f6e 5f74 6f6b 656e  completion_token
+000013d0: 7322 3a20 226e 756d 6265 7222 2c0a 2020  s": "number",.  
+000013e0: 2020 2274 6f74 616c 5f74 6f6b 656e 7322    "total_tokens"
+000013f0: 3a20 226e 756d 6265 7222 0a20 207d 2c0a  : "number".  },.
+00001400: 2020 2265 7272 6f72 223a 2022 7374 7269    "error": "stri
+00001410: 6e67 7c4e 6f6e 6522 2c0a 2020 2266 696e  ng|None",.  "fin
+00001420: 6973 685f 7265 6173 6f6e 223a 2022 7374  ish_reason": "st
+00001430: 7269 6e67 220a 7d0a 6060 600a 0a23 2323  ring".}.```..###
+00001440: 2060 6675 6e63 7469 6f6e 5f63 6f6d 706c   `function_compl
+00001450: 6574 696f 6e28 7465 7874 2c20 6675 6e63  etion(text, func
+00001460: 7469 6f6e 733d 4e6f 6e65 2c20 6d6f 6465  tions=None, mode
+00001470: 6c5f 6661 696c 7572 655f 7265 7472 6965  l_failure_retrie
+00001480: 733d 352c 2066 756e 6374 696f 6e5f 6361  s=5, function_ca
+00001490: 6c6c 3d4e 6f6e 652c 2066 756e 6374 696f  ll=None, functio
+000014a0: 6e5f 6661 696c 7572 655f 7265 7472 6965  n_failure_retrie
+000014b0: 733d 3130 2c20 6368 756e 6b5f 6c65 6e67  s=10, chunk_leng
+000014c0: 7468 3d44 4546 4155 4c54 5f43 4855 4e4b  th=DEFAULT_CHUNK
+000014d0: 5f4c 454e 4754 482c 206d 6f64 656c 3d4e  _LENGTH, model=N
+000014e0: 6f6e 652c 2061 7069 5f6b 6579 3d4e 6f6e  one, api_key=Non
+000014f0: 6529 600a 0a53 656e 6473 2074 6578 7420  e)`..Sends text 
+00001500: 616e 6420 6120 6c69 7374 206f 6620 6675  and a list of fu
+00001510: 6e63 7469 6f6e 7320 746f 2074 6865 206d  nctions to the m
+00001520: 6f64 656c 2061 6e64 2072 6574 7572 6e73  odel and returns
+00001530: 206f 7074 696f 6e61 6c20 7465 7874 2061   optional text a
+00001540: 6e64 2061 2066 756e 6374 696f 6e20 6361  nd a function ca
+00001550: 6c6c 2e20 5468 6520 6675 6e63 7469 6f6e  ll. The function
+00001560: 2063 616c 6c20 6973 2076 616c 6964 6174   call is validat
+00001570: 6564 2061 6761 696e 7374 2074 6865 2066  ed against the f
+00001580: 756e 6374 696f 6e73 2061 7272 6179 2e0a  unctions array..
+00001590: 0a60 6060 7079 7468 6f6e 0a66 756e 6374  .```python.funct
+000015a0: 696f 6e20 3d20 7b0a 2020 2020 276e 616d  ion = {.    'nam
+000015b0: 6527 3a20 2766 756e 6374 696f 6e31 272c  e': 'function1',
+000015c0: 0a20 2020 2027 7061 7261 6d65 7465 7273  .    'parameters
+000015d0: 273a 207b 2770 6172 616d 3127 3a20 2776  ': {'param1': 'v
+000015e0: 616c 7565 3127 7d0a 7d0a 0a72 6573 706f  alue1'}.}..respo
+000015f0: 6e73 6520 3d20 6675 6e63 7469 6f6e 5f63  nse = function_c
+00001600: 6f6d 706c 6574 696f 6e28 2243 616c 6c20  ompletion("Call 
+00001610: 7468 6520 6675 6e63 7469 6f6e 2e22 2c20  the function.", 
+00001620: 6675 6e63 7469 6f6e 290a 6060 600a 0a54  function).```..T
+00001630: 6865 2072 6573 706f 6e73 6520 6f62 6a65  he response obje
+00001640: 6374 206c 6f6f 6b73 206c 696b 6520 7468  ct looks like th
+00001650: 6973 3a0a 0a60 6060 6a73 6f6e 0a7b 0a20  is:..```json.{. 
+00001660: 2022 7465 7874 223a 2022 7374 7269 6e67   "text": "string
+00001670: 222c 0a20 2022 6675 6e63 7469 6f6e 5f6e  ",.  "function_n
+00001680: 616d 6522 3a20 2273 7472 696e 6722 2c0a  ame": "string",.
+00001690: 2020 2261 7267 756d 656e 7473 223a 2022    "arguments": "
+000016a0: 6469 6374 222c 0a20 2022 7573 6167 6522  dict",.  "usage"
+000016b0: 3a20 7b0a 2020 2020 2270 726f 6d70 745f  : {.    "prompt_
+000016c0: 746f 6b65 6e73 223a 2022 6e75 6d62 6572  tokens": "number
+000016d0: 222c 0a20 2020 2022 636f 6d70 6c65 7469  ",.    "completi
+000016e0: 6f6e 5f74 6f6b 656e 7322 3a20 226e 756d  on_tokens": "num
+000016f0: 6265 7222 2c0a 2020 2020 2274 6f74 616c  ber",.    "total
+00001700: 5f74 6f6b 656e 7322 3a20 226e 756d 6265  _tokens": "numbe
+00001710: 7222 0a20 207d 2c0a 2020 2266 696e 6973  r".  },.  "finis
+00001720: 685f 7265 6173 6f6e 223a 2022 7374 7269  h_reason": "stri
+00001730: 6e67 222c 0a20 2022 6572 726f 7222 3a20  ng",.  "error": 
+00001740: 2273 7472 696e 677c 4e6f 6e65 220a 7d0a  "string|None".}.
+00001750: 6060 600a 0a23 2323 2060 7472 696d 5f70  ```..### `trim_p
+00001760: 726f 6d70 7428 7465 7874 2c20 6d61 785f  rompt(text, max_
+00001770: 746f 6b65 6e73 3d44 4546 4155 4c54 5f43  tokens=DEFAULT_C
+00001780: 4855 4e4b 5f4c 454e 4754 482c 206d 6f64  HUNK_LENGTH, mod
+00001790: 656c 3d44 4546 4155 4c54 5f54 4558 545f  el=DEFAULT_TEXT_
+000017a0: 4d4f 4445 4c2c 2070 7265 7365 7276 655f  MODEL, preserve_
+000017b0: 746f 703d 5472 7565 2960 0a0a 5472 696d  top=True)`..Trim
+000017c0: 2074 6865 2067 6976 656e 2074 6578 7420   the given text 
+000017d0: 746f 2061 206d 6178 696d 756d 206e 756d  to a maximum num
+000017e0: 6265 7220 6f66 2074 6f6b 656e 732e 0a0a  ber of tokens...
+000017f0: 6060 6070 7974 686f 6e0a 7472 696d 6d65  ```python.trimme
+00001800: 645f 7465 7874 203d 2074 7269 6d5f 7072  d_text = trim_pr
+00001810: 6f6d 7074 2822 5468 6973 2069 7320 6120  ompt("This is a 
+00001820: 7465 7374 2e22 2c20 332c 2070 7265 7365  test.", 3, prese
+00001830: 7276 655f 746f 703d 5472 7565 290a 6060  rve_top=True).``
+00001840: 600a 0a23 2323 2060 6368 756e 6b5f 7072  `..### `chunk_pr
+00001850: 6f6d 7074 2870 726f 6d70 742c 2063 6875  ompt(prompt, chu
+00001860: 6e6b 5f6c 656e 6774 683d 4445 4641 554c  nk_length=DEFAUL
+00001870: 545f 4348 554e 4b5f 4c45 4e47 5448 2960  T_CHUNK_LENGTH)`
+00001880: 0a0a 5370 6c69 7420 7468 6520 6769 7665  ..Split the give
+00001890: 6e20 7072 6f6d 7074 2069 6e74 6f20 6368  n prompt into ch
+000018a0: 756e 6b73 2077 6865 7265 2065 6163 6820  unks where each 
+000018b0: 6368 756e 6b20 6861 7320 6120 6d61 7869  chunk has a maxi
+000018c0: 6d75 6d20 6e75 6d62 6572 206f 6620 746f  mum number of to
+000018d0: 6b65 6e73 2e0a 0a60 6060 7079 7468 6f6e  kens...```python
+000018e0: 0a70 726f 6d70 745f 6368 756e 6b73 203d  .prompt_chunks =
+000018f0: 2063 6875 6e6b 5f70 726f 6d70 7428 2254   chunk_prompt("T
+00001900: 6869 7320 6973 2061 2074 6573 742e 2049  his is a test. I
+00001910: 2061 6d20 7772 6974 696e 6720 6120 6675   am writing a fu
+00001920: 6e63 7469 6f6e 2e22 2c20 3429 0a60 6060  nction.", 4).```
+00001930: 0a0a 2323 2320 6063 6f75 6e74 5f74 6f6b  ..### `count_tok
+00001940: 656e 7328 7072 6f6d 7074 2c20 6d6f 6465  ens(prompt, mode
+00001950: 6c3d 4445 4641 554c 545f 5445 5854 5f4d  l=DEFAULT_TEXT_M
+00001960: 4f44 454c 2960 0a0a 436f 756e 7420 7468  ODEL)`..Count th
+00001970: 6520 6e75 6d62 6572 206f 6620 746f 6b65  e number of toke
+00001980: 6e73 2069 6e20 6120 7374 7269 6e67 2e0a  ns in a string..
+00001990: 0a60 6060 7079 7468 6f6e 0a6e 756d 5f74  .```python.num_t
+000019a0: 6f6b 656e 7320 3d20 636f 756e 745f 746f  okens = count_to
+000019b0: 6b65 6e73 2822 5468 6973 2069 7320 6120  kens("This is a 
+000019c0: 7465 7374 2e22 290a 6060 600a 0a23 2323  test.").```..###
+000019d0: 2060 6765 745f 746f 6b65 6e73 2870 726f   `get_tokens(pro
+000019e0: 6d70 742c 206d 6f64 656c 3d44 4546 4155  mpt, model=DEFAU
+000019f0: 4c54 5f54 4558 545f 4d4f 4445 4c29 600a  LT_TEXT_MODEL)`.
+00001a00: 0a52 6574 7572 6e73 2061 206c 6973 7420  .Returns a list 
+00001a10: 6f66 2074 6f6b 656e 7320 696e 2061 2073  of tokens in a s
+00001a20: 7472 696e 672e 0a0a 6060 6070 7974 686f  tring...```pytho
+00001a30: 6e0a 746f 6b65 6e73 203d 2067 6574 5f74  n.tokens = get_t
+00001a40: 6f6b 656e 7328 2254 6869 7320 6973 2061  okens("This is a
+00001a50: 2074 6573 742e 2229 0a60 6060 0a0a 2323   test.").```..##
+00001a60: 2320 6063 6f6d 706f 7365 5f70 726f 6d70  # `compose_promp
+00001a70: 7428 7072 6f6d 7074 5f74 656d 706c 6174  t(prompt_templat
+00001a80: 652c 2070 6172 616d 6574 6572 7329 600a  e, parameters)`.
+00001a90: 0a43 6f6d 706f 7365 7320 6120 7072 6f6d  .Composes a prom
+00001aa0: 7074 2075 7369 6e67 2061 2074 656d 706c  pt using a templ
+00001ab0: 6174 6520 616e 6420 7061 7261 6d65 7465  ate and paramete
+00001ac0: 7273 2e20 5061 7261 6d65 7465 7220 6b65  rs. Parameter ke
+00001ad0: 7973 2061 7265 2065 6e63 6c6f 7365 6420  ys are enclosed 
+00001ae0: 696e 2064 6f75 626c 6520 6375 726c 7920  in double curly 
+00001af0: 6272 6163 6b65 7473 2061 6e64 2072 6570  brackets and rep
+00001b00: 6c61 6365 6420 7769 7468 2070 6172 616d  laced with param
+00001b10: 6574 6572 2076 616c 7565 732e 0a0a 6060  eter values...``
+00001b20: 6070 7974 686f 6e0a 7072 6f6d 7074 203d  `python.prompt =
+00001b30: 2063 6f6d 706f 7365 5f70 726f 6d70 7428   compose_prompt(
+00001b40: 2248 656c 6c6f 207b 7b6e 616d 657d 7d21  "Hello {{name}}!
+00001b50: 222c 207b 226e 616d 6522 3a20 224a 6f68  ", {"name": "Joh
+00001b60: 6e22 7d29 0a60 6060 0a0a 2323 2041 206e  n"}).```..## A n
+00001b70: 6f74 6520 6162 6f75 7420 6d6f 6465 6c73  ote about models
+00001b80: 0a0a 596f 7520 6361 6e20 7061 7373 2069  ..You can pass i
+00001b90: 6e20 6120 6d6f 6465 6c20 7573 696e 6720  n a model using 
+00001ba0: 7468 6520 606d 6f64 656c 6020 7061 7261  the `model` para
+00001bb0: 6d65 7465 7220 6f66 2065 6974 6865 7220  meter of either 
+00001bc0: 6675 6e63 7469 6f6e 5f63 6f6d 706c 6574  function_complet
+00001bd0: 696f 6e20 6f72 2074 6578 745f 636f 6d70  ion or text_comp
+00001be0: 6c65 7469 6f6e 2e20 4966 2079 6f75 2064  letion. If you d
+00001bf0: 6f20 6e6f 7420 7061 7373 2069 6e20 6120  o not pass in a 
+00001c00: 6d6f 6465 6c2c 2074 6865 2064 6566 6175  model, the defau
+00001c10: 6c74 206d 6f64 656c 2077 696c 6c20 6265  lt model will be
+00001c20: 2075 7365 642e 2059 6f75 2063 616e 2061   used. You can a
+00001c30: 6c73 6f20 6f76 6572 7269 6465 2074 6869  lso override thi
+00001c40: 7320 6279 2073 6574 7469 6e67 2074 6865  s by setting the
+00001c50: 2065 6e76 6972 6f6e 6d65 6e74 206d 6f64   environment mod
+00001c60: 656c 2076 6961 2060 4f50 454e 4149 5f4d  el via `OPENAI_M
+00001c70: 4f44 454c 6020 656e 7669 726f 6e6d 656e  ODEL` environmen
+00001c80: 7420 7661 7269 6162 6c65 2e0a 0a44 6566  t variable...Def
+00001c90: 6175 6c74 206d 6f64 656c 2069 7320 6770  ault model is gp
+00001ca0: 742d 7475 7262 6f2d 332e 352d 3036 3133  t-turbo-3.5-0613
+00001cb0: 2e0a 0a23 2320 4120 6e6f 7465 2061 626f  ...## A note abo
+00001cc0: 7574 2041 5049 206b 6579 730a 0a59 6f75  ut API keys..You
+00001cd0: 2063 616e 2070 6173 7320 696e 2061 6e20   can pass in an 
+00001ce0: 4150 4920 6b65 7920 7573 696e 6720 7468  API key using th
+00001cf0: 6520 6061 7069 5f6b 6579 6020 7061 7261  e `api_key` para
+00001d00: 6d65 7465 7220 6f66 2065 6974 6865 7220  meter of either 
+00001d10: 6675 6e63 7469 6f6e 5f63 6f6d 706c 6574  function_complet
+00001d20: 696f 6e20 6f72 2074 6578 745f 636f 6d70  ion or text_comp
+00001d30: 6c65 7469 6f6e 2e20 4966 2079 6f75 2064  letion. If you d
+00001d40: 6f20 6e6f 7420 7061 7373 2069 6e20 616e  o not pass in an
+00001d50: 2041 5049 206b 6579 2c20 7468 6520 604f   API key, the `O
+00001d60: 5045 4e41 495f 4150 495f 4b45 5960 2065  PENAI_API_KEY` e
+00001d70: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00001d80: 626c 6520 7769 6c6c 2062 6520 6368 6563  ble will be chec
+00001d90: 6b65 642e 0a0a 2320 5075 626c 6973 6869  ked...# Publishi
+00001da0: 6e67 0a0a 6060 6062 6173 680a 6261 7368  ng..```bash.bash
+00001db0: 2070 7562 6c69 7368 2e73 6820 2d2d 7665   publish.sh --ve
+00001dc0: 7273 696f 6e3d 3c76 6572 7369 6f6e 3e20  rsion=<version> 
+00001dd0: 2d2d 7573 6572 6e61 6d65 3d3c 7079 7069  --username=<pypi
+00001de0: 5f75 7365 726e 616d 653e 202d 2d70 6173  _username> --pas
+00001df0: 7377 6f72 643d 3c70 7970 695f 7061 7373  sword=<pypi_pass
+00001e00: 776f 7264 3e0a 6060 600a 0a23 2043 6f6e  word>.```..# Con
+00001e10: 7472 6962 7574 696f 6e73 2057 656c 636f  tributions Welco
+00001e20: 6d65 0a0a 4966 2079 6f75 206c 696b 6520  me..If you like 
+00001e30: 7468 6973 206c 6962 7261 7279 2061 6e64  this library and
+00001e40: 2077 616e 7420 746f 2063 6f6e 7472 6962   want to contrib
+00001e50: 7574 6520 696e 2061 6e79 2077 6179 2c20  ute in any way, 
+00001e60: 706c 6561 7365 2066 6565 6c20 6672 6565  please feel free
+00001e70: 2074 6f20 7375 626d 6974 2061 2050 5220   to submit a PR 
+00001e80: 616e 6420 4920 7769 6c6c 2072 6576 6965  and I will revie
+00001e90: 7720 6974 2e20 506c 6561 7365 206e 6f74  w it. Please not
+00001ea0: 6520 7468 6174 2074 6865 2067 6f61 6c20  e that the goal 
+00001eb0: 6865 7265 2069 7320 7369 6d70 6c69 6369  here is simplici
+00001ec0: 7479 2061 6e64 2061 6363 6573 6962 696c  ty and accesibil
+00001ed0: 6974 792c 2075 7369 6e67 2063 6f6d 6d6f  ity, using commo
+00001ee0: 6e20 6c61 6e67 7561 6765 2061 6e64 2066  n language and f
+00001ef0: 6577 2064 6570 656e 6465 6e63 6965 732e  ew dependencies.
+00001f00: 0a0a 2320 5175 6573 7469 6f6e 732c 2043  ..# Questions, C
+00001f10: 6f6d 6d65 6e74 732c 2043 6f6e 6365 726e  omments, Concern
+00001f20: 730a 0a49 6620 796f 7520 6861 7665 2061  s..If you have a
+00001f30: 6e79 2071 7565 7374 696f 6e73 2c20 706c  ny questions, pl
+00001f40: 6561 7365 2066 6565 6c20 6672 6565 2074  ease feel free t
+00001f50: 6f20 7265 6163 6820 6f75 7420 746f 206d  o reach out to m
+00001f60: 6520 6f6e 205b 5477 6974 7465 725d 2868  e on [Twitter](h
+00001f70: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
+00001f80: 6f6d 2f73 7061 7469 616c 7765 6562 2920  om/spatialweeb) 
+00001f90: 6f72 2044 6973 636f 7264 2040 6e65 772e  or Discord @new.
+00001fa0: 6d6f 6f6e 0a                             moon.
```

### Comparing `easycompletion-0.2.9/easycompletion/constants.py` & `easycompletion-0.3.0/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.9/easycompletion/logger.py` & `easycompletion-0.3.0/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.9/easycompletion/model.py` & `easycompletion-0.3.0/easycompletion/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,29 +51,29 @@
         except (ValueError, SyntaxError):
             try:
                 arguments = re.sub(r"\.\.\.|\…", "", arguments)
                 arguments = re.sub(r"[\r\n]+", "", arguments)
                 arguments = re.sub(r"[^\x00-\x7F]+", "", arguments)
                 arguments = json.loads(arguments)
             # If everything fails, try Python's eval function
-            except (ValueError, SyntaxError):
+            except Exception:
                 try:
                     arguments = eval(arguments)
-                except (ValueError, SyntaxError):
+                except Exception:
                     arguments = None
     log(f"Arguments:\n{str(arguments)}", log=debug)
     return arguments
 
 
 def validate_functions(response, functions, function_call, debug=DEBUG):
     """
-    Validates if the function returned by the OpenAI API matches the intended function call.
+    Validates if the function returned matches the intended function call.
 
     Parameters:
-        response (dict): The response from OpenAI API.
+        response (dict): The response from the model.
         functions (list): A list of function definitions.
         function_call (dict or str): The expected function call.
 
     Returns:
         True if function call matches with the response, False otherwise.
 
     Usage:
@@ -99,59 +99,67 @@
         function_call["name"]
         if function_call != "auto"
         else response_function_call["name"]
     )
 
     # Parse the arguments from the response
     arguments = parse_arguments(response_function_call["arguments"])
-    
+
     # Get the function that matches the function name from the list of functions
     function = next(
         (item for item in functions if item["name"] == function_call_name), None
     )
 
     # If no matching function is found, return False
     if function is None:
         log(
             "No matching function found"
             + f"\nExpected function name:\n{str(function_call_name)}"
-            + f"\n\nResponse:\n{str(response)}"
-            , type="error", log=debug)
+            + f"\n\nResponse:\n{str(response)}",
+            type="error",
+            log=debug,
+        )
         return False
 
     # If arguments are None, return False
     if arguments is None:
         log(
             "Arguments are None"
             + f"\nExpected arguments:\n{str(function['parameters']['properties'].keys())}"
-            + f"\n\nResponse function call:\n{str(response_function_call)}"
-            , type="error", log=debug)
+            + f"\n\nResponse function call:\n{str(response_function_call)}",
+            type="error",
+            log=debug,
+        )
         #
         return False
 
-    
     required_properties = function["parameters"].get("required", [])
 
     # Check that arguments.keys() contains all of the required properties
-    if not all(required_property in arguments.keys() for required_property in required_properties):
+    if not all(
+        required_property in arguments.keys()
+        for required_property in required_properties
+    ):
         log(
             "ERROR: Response did not contain all required properties.\n"
             + f"\nExpected keys:\n{str(function['parameters']['properties'].keys())}"
-            +f"\n\nActual keys:\n{str(arguments.keys())}",
-            type="error", log=debug)
+            + f"\n\nActual keys:\n{str(arguments.keys())}",
+            type="error",
+            log=debug,
+        )
 
         return False
 
     log("Function call is valid", type="success", log=debug)
     return True
 
 
 def compose_function(name, description, properties, required_properties, debug=DEBUG):
     """
-    Composes a function object for OpenAI API.
+    Composes a function object for function calling.
 
     Parameters:
         name (str): The name of the function.
         description (str): Description of the function.
         properties (dict): Dictionary of property objects.
         required_properties (list): List of property names that are required.
 
@@ -180,37 +188,136 @@
             "required": required_properties,
         },
     }
     log(f"Function:\n{str(function)}", type="info", log=debug)
     return function
 
 
-def openai_text_call(
+def chat_completion(
+    messages,
+    system_message=None,
+    model_failure_retries=5,
+    model=None,
+    chunk_length=DEFAULT_CHUNK_LENGTH,
+    api_key=None,
+    debug=DEBUG,
+):
+    """
+    Function for sending chat messages and returning a chat response.
+
+    Parameters:
+        messages (str): Messages to send to the model. In the form {<role>: string, <content>: string} - roles are "user" and "assistant"
+        system_message (str, optional): Message appended at the top sent by the system. Usually used to tell what the agent how to act.
+        model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
+        model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
+        chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
+        api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
+
+    Returns:
+        str: The response content from the model.
+
+    Example:
+        >>> text_completion("Hello, how are you?", model_failure_retries=3, model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key')
+    """
+
+    # Override the API key if provided as parameter
+    if api_key is not None:
+        openai.api_key = api_key
+
+    # Use the default model if no model is specified
+    if model == None:
+        model = DEFAULT_TEXT_MODEL
+
+    # Count tokens in the input text
+    total_tokens = count_tokens(messages, model=model)
+
+    # If text is longer than chunk_length and model is not for long texts, switch to the long text model
+    if total_tokens > chunk_length and "16k" not in model:
+        model = LONG_TEXT_MODEL
+        if not os.environ.get("SUPPRESS_WARNINGS"):
+            print(
+                "Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)"
+            )
+
+    # If text is too long even for long text model, return None
+    if total_tokens > (16384 - chunk_length):
+        print("Error: Message too long")
+        return {
+            "text": None,
+            "usage": None,
+            "finish_reason": None,
+            "error": "Message too long",
+        }
+
+    # Prepare messages for the API call
+    messages = [{"role": "system", "content": system_message}] + messages
+
+    log(f"Prompt:\n{str(messages)}", type="prompt", log=debug)
+
+    # Try to make a request for a specified number of times
+    response = None
+    for i in range(model_failure_retries):
+        try:
+            response = openai.ChatCompletion.create(model=model, messages=messages)
+            break
+        except Exception as e:
+            log(f"OpenAI Error: {e}", type="error", log=debug)
+            continue
+        # wait 1 second
+        time.sleep(1)
+
+    # If response is not valid, print an error message and return None
+    if (
+        response is None
+        or response["choices"] is None
+        or response["choices"][0] is None
+    ):
+        return {
+            "text": None,
+            "usage": None,
+            "finish_reason": None,
+            "error": "Error: Could not get a successful response from OpenAI API",
+        }
+
+    # Extract content from the response
+    text = response["choices"][0]["message"]["content"]
+    finish_reason = response["choices"][0]["finish_reason"]
+    usage = response["usage"]
+
+    return {
+        "text": text,
+        "usage": usage,
+        "finish_reason": finish_reason,
+        "error": None,
+    }
+
+
+def text_completion(
     text,
     model_failure_retries=5,
     model=None,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
     debug=DEBUG,
 ):
     """
-    Function for sending text to the OpenAI API and returning a text response.
+    Function for sending text and returning a text completion response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
         model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
         chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
         api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
     Returns:
         str: The response content from the model.
 
     Example:
-        >>> openai_text_call("Hello, how are you?", model_failure_retries=3, model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key')
+        >>> text_completion("Hello, how are you?", model_failure_retries=3, model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key')
     """
 
     # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
     # Use the default model if no model is specified
@@ -229,15 +336,15 @@
             )
 
     # If text is too long even for long text model, return None
     if total_tokens > (16384 - chunk_length):
         print("Error: Message too long")
         return {
             "text": None,
-            usage: None,
+            "usage": None,
             "finish_reason": None,
             "error": "Message too long",
         }
 
     # Prepare messages for the API call
     messages = [{"role": "user", "content": text}]
 
@@ -259,15 +366,15 @@
     if (
         response is None
         or response["choices"] is None
         or response["choices"][0] is None
     ):
         return {
             "text": None,
-            usage: None,
+            "usage": None,
             "finish_reason": None,
             "error": "Error: Could not get a successful response from OpenAI API",
         }
 
     # Extract content from the response
     text = response["choices"][0]["message"]["content"]
     finish_reason = response["choices"][0]["finish_reason"]
@@ -277,27 +384,27 @@
         "text": text,
         "usage": usage,
         "finish_reason": finish_reason,
         "error": None,
     }
 
 
-def openai_function_call(
+def function_completion(
     text,
     functions=None,
     model_failure_retries=5,
     function_call=None,
     function_failure_retries=10,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     model=None,
     api_key=None,
     debug=DEBUG,
 ):
     """
-    Send text and a list of functions to the OpenAI API and return optional text and a function call.
+    Send text and a list of functions to the model and return optional text and a function call.
     The function call is validated against the functions array.
     The input text is sent to the chat model and is treated as a user message.
 
     Args:
         text (str): Text that will be sent as the user message to the model.
         functions (list[dict] | dict | None): List of functions or a single function dictionary to be sent to the model.
         model_failure_retries (int): Number of times to retry the request if it fails (default is 5).
@@ -309,15 +416,15 @@
 
     Returns:
         dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing
         "text" (response from the model), "function_name" (name of the function called), "arguments" (arguments for the function), "error" (None).
 
     Example:
         >>> function = {'name': 'function1', 'parameters': {'param1': 'value1'}}
-        >>> openai_function_call("Call the function.", function)
+        >>> function_completion("Call the function.", function)
     """
 
     # Check if the user provided an API key
     if api_key is not None:
         openai.api_key = api_key
 
     # Ensure that functions are provided
@@ -431,17 +538,17 @@
             except Exception as e:
                 log(f"OpenAI Error: {e}", type="error", log=debug)
             time.sleep(1)
         if validate_functions(response, functions, function_call):
             break
         time.sleep(1)
 
-    # Check if we have a valid response from OpenAI API
+    # Check if we have a valid response from the model
     if response is None:
-        error = "Could not get a successful response from OpenAI API. Check your API key and arguments."
+        error = "Could not get a successful response from the model. Check your API key and arguments."
         log(error, type="error", log=True)
         return {"error": error}
 
     # Extracting the content and function call response from API response
     response_data = response["choices"][0]["message"]
     finish_reason = response["choices"][0]["finish_reason"]
     usage = response["usage"]
```

### Comparing `easycompletion-0.2.9/easycompletion/prompt.py` & `easycompletion-0.3.0/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.9/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,450 +1,470 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6561 7379  : 2.1.Name: easy
-00000020: 636f 6d70 6c65 7469 6f6e 0a56 6572 7369  completion.Versi
-00000030: 6f6e 3a20 302e 322e 390a 5375 6d6d 6172  on: 0.2.9.Summar
-00000040: 793a 2045 6173 7920 7465 7874 2063 6f6d  y: Easy text com
-00000050: 706c 6574 696f 6e20 616e 6420 6675 6e63  pletion and func
-00000060: 7469 6f6e 2063 616c 6c69 6e67 2075 7369  tion calling usi
-00000070: 6e67 2074 6865 204f 7065 6e41 4920 4150  ng the OpenAI AP
-00000080: 492e 2041 6c73 6f20 696e 636c 7564 6573  I. Also includes
-00000090: 2075 7365 6675 6c20 7574 696c 6974 6965   useful utilitie
-000000a0: 7320 666f 7220 636f 756e 7469 6e67 2074  s for counting t
-000000b0: 6f6b 656e 732c 2063 6f6d 706f 7369 6e67  okens, composing
-000000c0: 2070 726f 6d70 7473 2061 6e64 2074 7269   prompts and tri
-000000d0: 6d6d 696e 6720 7468 656d 2074 6f20 6669  mming them to fi
-000000e0: 7420 7769 7468 696e 2074 6865 2074 6f6b  t within the tok
-000000f0: 656e 206c 696d 6974 2e0a 486f 6d65 2d70  en limit..Home-p
-00000100: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000110: 6875 622e 636f 6d2f 4175 746f 6e6f 6d6f  hub.com/Autonomo
-00000120: 7573 5265 7365 6172 6368 4772 6f75 702f  usResearchGroup/
-00000130: 6561 7379 636f 6d70 6c65 7469 6f6e 0a41  easycompletion.A
-00000140: 7574 686f 723a 204d 6f6f 6e0a 4175 7468  uthor: Moon.Auth
-00000150: 6f72 2d65 6d61 696c 3a20 7368 6177 6d61  or-email: shawma
-00000160: 6b65 736d 6167 6963 4067 6d61 696c 2e63  kesmagic@gmail.c
-00000170: 6f6d 0a4c 6963 656e 7365 3a20 4d49 540a  om.License: MIT.
-00000180: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00000190: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-000001a0: 3a20 3220 2d20 5072 652d 416c 7068 610a  : 2 - Pre-Alpha.
-000001b0: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
-000001c0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001d0: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-000001e0: 680a 436c 6173 7369 6669 6572 3a20 4c69  h.Classifier: Li
-000001f0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000200: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000210: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000220: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-00000230: 6d20 3a3a 2050 4f53 4958 203a 3a20 4c69  m :: POSIX :: Li
-00000240: 6e75 780a 436c 6173 7369 6669 6572 3a20  nux.Classifier: 
-00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000270: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000290: 203a 3a20 4d61 634f 5320 3a3a 204d 6163   :: MacOS :: Mac
-000002a0: 4f53 2058 0a43 6c61 7373 6966 6965 723a  OS X.Classifier:
-000002b0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002c0: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
-000002d0: 3a20 5769 6e64 6f77 730a 4465 7363 7269  : Windows.Descri
-000002e0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-000002f0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000300: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000310: 4c49 4345 4e53 450a 0a0a 4561 7379 2074  LICENSE...Easy t
-00000320: 6578 7420 636f 6d70 6c65 7469 6f6e 2061  ext completion a
-00000330: 6e64 2066 756e 6374 696f 6e20 6361 6c6c  nd function call
-00000340: 696e 6720 7573 696e 6720 7468 6520 4f70  ing using the Op
-00000350: 656e 4149 2041 5049 2e20 416c 736f 2069  enAI API. Also i
-00000360: 6e63 6c75 6465 7320 7573 6566 756c 2075  ncludes useful u
-00000370: 7469 6c69 7469 6573 2066 6f72 2063 6f75  tilities for cou
-00000380: 6e74 696e 6720 746f 6b65 6e73 2c20 636f  nting tokens, co
-00000390: 6d70 6f73 696e 6720 7072 6f6d 7074 7320  mposing prompts 
-000003a0: 616e 6420 7472 696d 6d69 6e67 2074 6865  and trimming the
-000003b0: 6d20 746f 2066 6974 2077 6974 6869 6e20  m to fit within 
-000003c0: 7468 6520 746f 6b65 6e20 6c69 6d69 742e  the token limit.
-000003d0: 0a0a 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
-000003e0: 6e0a 0a60 6060 6261 7368 0a70 6970 2069  n..```bash.pip i
-000003f0: 6e73 7461 6c6c 2065 6173 7963 6f6d 706c  nstall easycompl
-00000400: 6574 696f 6e0a 6060 600a 0a23 2051 7569  etion.```..# Qui
-00000410: 636b 7374 6172 740a 0a60 6060 7079 7468  ckstart..```pyth
-00000420: 6f6e 0a66 726f 6d20 6561 7379 636f 6d70  on.from easycomp
-00000430: 6c65 7469 6f6e 2069 6d70 6f72 7420 6f70  letion import op
-00000440: 656e 6169 5f66 756e 6374 696f 6e5f 6361  enai_function_ca
-00000450: 6c6c 2c20 6f70 656e 6169 5f74 6578 745f  ll, openai_text_
-00000460: 6361 6c6c 2c20 636f 6d70 6f73 655f 7072  call, compose_pr
-00000470: 6f6d 7074 0a0a 2320 436f 6d70 6f73 6520  ompt..# Compose 
-00000480: 6120 6675 6e63 7469 6f6e 206f 626a 6563  a function objec
-00000490: 740a 7465 7374 5f66 756e 6374 696f 6e20  t.test_function 
-000004a0: 3d20 636f 6d70 6f73 655f 6675 6e63 7469  = compose_functi
-000004b0: 6f6e 280a 2020 2020 6e61 6d65 3d22 7772  on(.    name="wr
-000004c0: 6974 655f 736f 6e67 222c 0a20 2020 2064  ite_song",.    d
-000004d0: 6573 6372 6970 7469 6f6e 3d22 5772 6974  escription="Writ
-000004e0: 6520 6120 736f 6e67 2061 626f 7574 2041  e a song about A
-000004f0: 4922 2c0a 2020 2020 7072 6f70 6572 7469  I",.    properti
-00000500: 6573 3d7b 0a20 2020 2020 2020 2020 2020  es={.           
-00000510: 2022 6c79 7269 6373 223a 207b 0a20 2020   "lyrics": {.   
-00000520: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00000530: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
-00000540: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000550: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00000560: 6865 206c 7972 6963 7320 666f 7220 7468  he lyrics for th
-00000570: 6520 736f 6e67 222c 0a20 2020 2020 2020  e song",.       
-00000580: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-00000590: 2020 7265 7175 6972 6564 5f70 726f 7065    required_prope
-000005a0: 7274 6965 733a 205b 226c 7972 6963 7322  rties: ["lyrics"
-000005b0: 5d2c 0a29 0a0a 2320 4361 6c6c 2074 6865  ],.)..# Call the
-000005c0: 2066 756e 6374 696f 6e0a 7265 7370 6f6e   function.respon
-000005d0: 7365 203d 206f 7065 6e61 695f 6675 6e63  se = openai_func
-000005e0: 7469 6f6e 5f63 616c 6c28 7465 7874 3d22  tion_call(text="
-000005f0: 5772 6974 6520 6120 736f 6e67 2061 626f  Write a song abo
-00000600: 7574 2041 4922 2c20 6675 6e63 7469 6f6e  ut AI", function
-00000610: 733d 5b74 6573 745f 6675 6e63 7469 6f6e  s=[test_function
-00000620: 5d2c 2066 756e 6374 696f 6e5f 6361 6c6c  ], function_call
-00000630: 3d22 7772 6974 655f 736f 6e67 2229 0a0a  ="write_song")..
-00000640: 2320 5072 696e 7420 7468 6520 7265 7370  # Print the resp
-00000650: 6f6e 7365 0a70 7269 6e74 2872 6573 706f  onse.print(respo
-00000660: 6e73 655b 2261 7267 756d 656e 7473 225d  nse["arguments"]
-00000670: 5b22 6c79 7269 6373 225d 290a 6060 600a  ["lyrics"]).```.
-00000680: 0a23 2042 6173 6963 2055 7361 6765 0a0a  .# Basic Usage..
-00000690: 2323 2043 6f6d 706f 7365 2050 726f 6d70  ## Compose Promp
-000006a0: 740a 0a59 6f75 2063 616e 2063 6f6d 706f  t..You can compo
-000006b0: 7365 2061 2070 726f 6d70 7420 7573 696e  se a prompt usin
-000006c0: 6720 7b7b 6861 6e64 6c65 6261 7273 7d7d  g {{handlebars}}
-000006d0: 2073 796e 7461 780a 0a60 6060 7079 7468   syntax..```pyth
-000006e0: 6f6e 0a74 6573 745f 7072 6f6d 7074 203d  on.test_prompt =
-000006f0: 2022 446f 6e27 7420 666f 7267 6574 2079   "Don't forget y
-00000700: 6f75 7220 7b7b 6f62 6a65 6374 7d7d 220a  our {{object}}".
-00000710: 7465 7374 5f64 6963 7420 3d20 7b22 6f62  test_dict = {"ob
-00000720: 6a65 6374 223a 2022 746f 7765 6c22 7d0a  ject": "towel"}.
-00000730: 7072 6f6d 7074 203d 2063 6f6d 706f 7365  prompt = compose
-00000740: 5f70 726f 6d70 7428 7465 7374 5f70 726f  _prompt(test_pro
-00000750: 6d70 742c 2074 6573 745f 6469 6374 290a  mpt, test_dict).
-00000760: 2320 7072 6f6d 7074 203d 2022 446f 6e27  # prompt = "Don'
-00000770: 7420 666f 7267 6574 2079 6f75 7220 746f  t forget your to
-00000780: 7765 6c22 0a60 6060 0a0a 2323 2054 6578  wel".```..## Tex
-00000790: 7420 436f 6d70 6c65 7469 6f6e 0a0a 5365  t Completion..Se
-000007a0: 6e64 2074 6578 742c 2067 6574 2061 2072  nd text, get a r
-000007b0: 6573 706f 6e73 6520 6173 2061 2074 6578  esponse as a tex
-000007c0: 7420 7374 7269 6e67 0a0a 6060 6070 7974  t string..```pyt
-000007d0: 686f 6e0a 6672 6f6d 2065 6173 7963 6f6d  hon.from easycom
-000007e0: 706c 6574 696f 6e20 696d 706f 7274 206f  pletion import o
-000007f0: 7065 6e61 695f 7465 7874 5f63 616c 6c0a  penai_text_call.
-00000800: 7265 7370 6f6e 7365 203d 206f 7065 6e61  response = opena
-00000810: 695f 7465 7874 5f63 616c 6c28 2248 656c  i_text_call("Hel
-00000820: 6c6f 2c20 686f 7720 6172 6520 796f 753f  lo, how are you?
-00000830: 2229 0a23 2072 6573 706f 6e73 655b 2274  ").# response["t
-00000840: 6578 7422 5d20 3d20 2241 7320 616e 2041  ext"] = "As an A
-00000850: 4920 6c61 6e67 7561 6765 206d 6f64 656c  I language model
-00000860: 2c20 4920 646f 6e27 7420 6861 7665 2066  , I don't have f
-00000870: 6565 6c69 6e67 732c 2062 7574 2e2e 2e22  eelings, but..."
-00000880: 220a 6060 600a 0a23 2320 436f 6d70 6f73  ".```..## Compos
-00000890: 6520 6120 4675 6e63 7469 6f6e 0a0a 436f  e a Function..Co
-000008a0: 6d70 6f73 6520 6120 6675 6e63 7469 6f6e  mpose a function
-000008b0: 2074 6f20 7061 7373 2069 6e74 6f20 7468   to pass into th
-000008c0: 6520 6675 6e63 7469 6f6e 2063 616c 6c69  e function calli
-000008d0: 6e67 2041 5049 0a0a 6060 6070 7974 686f  ng API..```pytho
-000008e0: 6e0a 6672 6f6d 2065 6173 7963 6f6d 706c  n.from easycompl
-000008f0: 6574 696f 6e20 696d 706f 7274 2063 6f6d  etion import com
-00000900: 706f 7365 5f66 756e 6374 696f 6e0a 0a74  pose_function..t
-00000910: 6573 745f 6675 6e63 7469 6f6e 203d 2063  est_function = c
-00000920: 6f6d 706f 7365 5f66 756e 6374 696f 6e28  ompose_function(
-00000930: 0a20 2020 206e 616d 653d 2277 7269 7465  .    name="write
-00000940: 5f73 6f6e 6722 2c0a 2020 2020 6465 7363  _song",.    desc
-00000950: 7269 7074 696f 6e3d 2257 7269 7465 2061  ription="Write a
-00000960: 2073 6f6e 6720 6162 6f75 7420 4149 222c   song about AI",
-00000970: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
-00000980: 7b0a 2020 2020 2020 2020 2020 2020 226c  {.            "l
-00000990: 7972 6963 7322 3a20 7b0a 2020 2020 2020  yrics": {.      
-000009a0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000009b0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
-000009c0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000009d0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-000009e0: 6c79 7269 6373 2066 6f72 2074 6865 2073  lyrics for the s
-000009f0: 6f6e 6722 2c0a 2020 2020 2020 2020 2020  ong",.          
-00000a00: 2020 7d0a 2020 2020 7d2c 0a20 2020 2072    }.    },.    r
-00000a10: 6571 7569 7265 645f 7072 6f70 6572 7469  equired_properti
-00000a20: 6573 3a20 5b22 6c79 7269 6373 225d 2c0a  es: ["lyrics"],.
-00000a30: 290a 6060 600a 0a23 2320 4675 6e63 7469  ).```..## Functi
-00000a40: 6f6e 2043 6f6d 706c 6574 696f 6e0a 0a53  on Completion..S
-00000a50: 656e 6420 7465 7874 2061 6e64 2061 206c  end text and a l
-00000a60: 6973 7420 6f66 2066 756e 6374 696f 6e73  ist of functions
-00000a70: 2061 6e64 2067 6574 2061 2072 6573 706f   and get a respo
-00000a80: 6e73 6520 6173 2061 2066 756e 6374 696f  nse as a functio
-00000a90: 6e20 6361 6c6c 0a0a 6060 6070 7974 686f  n call..```pytho
-00000aa0: 6e0a 6672 6f6d 2065 6173 7963 6f6d 706c  n.from easycompl
-00000ab0: 6574 696f 6e20 696d 706f 7274 206f 7065  etion import ope
-00000ac0: 6e61 695f 6675 6e63 7469 6f6e 5f63 616c  nai_function_cal
-00000ad0: 6c2c 2063 6f6d 706f 7365 5f66 756e 6374  l, compose_funct
-00000ae0: 696f 6e0a 0a23 204e 4f54 453a 2074 6573  ion..# NOTE: tes
-00000af0: 745f 6675 6e63 7469 6f6e 2069 7320 6120  t_function is a 
-00000b00: 6675 6e63 7469 6f6e 206f 626a 6563 7420  function object 
-00000b10: 6372 6561 7465 6420 7573 696e 6720 636f  created using co
-00000b20: 6d70 6f73 655f 6675 6e63 7469 6f6e 2069  mpose_function i
-00000b30: 6e20 7468 6520 6578 616d 706c 6520 6162  n the example ab
-00000b40: 6f76 652e 2e2e 0a0a 7265 7370 6f6e 7365  ove.....response
-00000b50: 203d 206f 7065 6e61 695f 6675 6e63 7469   = openai_functi
-00000b60: 6f6e 5f63 616c 6c28 7465 7874 3d22 5772  on_call(text="Wr
-00000b70: 6974 6520 6120 736f 6e67 2061 626f 7574  ite a song about
-00000b80: 2041 4922 2c20 6675 6e63 7469 6f6e 733d   AI", functions=
-00000b90: 5b74 6573 745f 6675 6e63 7469 6f6e 5d2c  [test_function],
-00000ba0: 2066 756e 6374 696f 6e5f 6361 6c6c 3d22   function_call="
-00000bb0: 7772 6974 655f 736f 6e67 2229 0a23 2052  write_song").# R
-00000bc0: 6573 706f 6e73 6520 7374 7275 6374 7572  esponse structur
-00000bd0: 6520 6973 207b 2022 7465 7874 223a 2073  e is { "text": s
-00000be0: 7472 696e 672c 2022 6675 6e63 7469 6f6e  tring, "function
-00000bf0: 5f6e 616d 6522 3a20 7374 7269 6e67 2c20  _name": string, 
-00000c00: 2261 7267 756d 656e 7473 223a 2064 6963  "arguments": dic
-00000c10: 7420 207d 0a70 7269 6e74 2872 6573 706f  t  }.print(respo
-00000c20: 6e73 655b 2261 7267 756d 656e 7473 225d  nse["arguments"]
-00000c30: 5b22 6c79 7269 6373 225d 290a 6060 600a  ["lyrics"]).```.
-00000c40: 0a23 2041 6476 616e 6365 6420 5573 6167  .# Advanced Usag
-00000c50: 650a 0a23 2323 2060 636f 6d70 6f73 655f  e..### `compose_
-00000c60: 6675 6e63 7469 6f6e 286e 616d 652c 2064  function(name, d
-00000c70: 6573 6372 6970 7469 6f6e 2c20 7072 6f70  escription, prop
-00000c80: 6572 7469 6573 2c20 7265 7175 6972 6564  erties, required
-00000c90: 5f70 726f 7065 7274 6965 7329 600a 0a43  _properties)`..C
-00000ca0: 6f6d 706f 7365 7320 6120 6675 6e63 7469  omposes a functi
-00000cb0: 6f6e 206f 626a 6563 7420 666f 7220 4f70  on object for Op
-00000cc0: 656e 4149 2041 5049 2e0a 0a60 6060 7079  enAI API...```py
-00000cd0: 7468 6f6e 0a73 756d 6d61 7269 7a61 7469  thon.summarizati
-00000ce0: 6f6e 5f66 756e 6374 696f 6e20 3d20 636f  on_function = co
-00000cf0: 6d70 6f73 655f 6675 6e63 7469 6f6e 280a  mpose_function(.
-00000d00: 2020 2020 6e61 6d65 3d22 7375 6d6d 6172      name="summar
-00000d10: 697a 655f 7465 7874 222c 0a20 2020 2064  ize_text",.    d
-00000d20: 6573 6372 6970 7469 6f6e 3d22 5375 6d6d  escription="Summ
-00000d30: 6172 697a 6520 7468 6520 7465 7874 2e20  arize the text. 
-00000d40: 496e 636c 7564 6520 7468 6520 746f 7069  Include the topi
-00000d50: 632c 2073 7562 746f 7069 6373 2e22 2c0a  c, subtopics.",.
-00000d60: 2020 2020 7072 6f70 6572 7469 6573 3d7b      properties={
-00000d70: 0a20 2020 2020 2020 2022 7375 6d6d 6172  .        "summar
-00000d80: 7922 3a20 7b0a 2020 2020 2020 2020 2020  y": {.          
-00000d90: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00000da0: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-00000db0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00000dc0: 4465 7461 696c 6564 2073 756d 6d61 7279  Detailed summary
-00000dd0: 206f 6620 7468 6520 7465 7874 2e22 2c0a   of the text.",.
-00000de0: 2020 2020 2020 2020 7d2c 0a20 2020 207d          },.    }
-00000df0: 2c0a 2020 2020 7265 7175 6972 6564 5f70  ,.    required_p
-00000e00: 726f 7065 7274 6965 733d 5b22 7375 6d6d  roperties=["summ
-00000e10: 6172 7922 5d2c 0a29 0a60 6060 0a0a 2323  ary"],.).```..##
-00000e20: 2320 606f 7065 6e61 695f 7465 7874 5f63  # `openai_text_c
-00000e30: 616c 6c28 7465 7874 2c20 6d6f 6465 6c5f  all(text, model_
-00000e40: 6661 696c 7572 655f 7265 7472 6965 733d  failure_retries=
-00000e50: 352c 206d 6f64 656c 3d4e 6f6e 652c 2063  5, model=None, c
-00000e60: 6875 6e6b 5f6c 656e 6774 683d 4445 4641  hunk_length=DEFA
-00000e70: 554c 545f 4348 554e 4b5f 4c45 4e47 5448  ULT_CHUNK_LENGTH
-00000e80: 2c20 6170 695f 6b65 793d 4e6f 6e65 2960  , api_key=None)`
-00000e90: 0a0a 5365 6e64 7320 7465 7874 2074 6f20  ..Sends text to 
-00000ea0: 7468 6520 4f70 656e 4149 2041 5049 2061  the OpenAI API a
-00000eb0: 6e64 2072 6574 7572 6e73 2061 2074 6578  nd returns a tex
-00000ec0: 7420 7265 7370 6f6e 7365 2e0a 0a60 6060  t response...```
-00000ed0: 7079 7468 6f6e 0a72 6573 706f 6e73 6520  python.response 
-00000ee0: 3d20 6f70 656e 6169 5f74 6578 745f 6361  = openai_text_ca
-00000ef0: 6c6c 280a 2020 2020 2248 656c 6c6f 2c20  ll(.    "Hello, 
-00000f00: 686f 7720 6172 6520 796f 753f 222c 0a20  how are you?",. 
-00000f10: 2020 206d 6f64 656c 5f66 6169 6c75 7265     model_failure
-00000f20: 5f72 6574 7269 6573 3d33 2c0a 2020 2020  _retries=3,.    
-00000f30: 6d6f 6465 6c3d 2767 7074 2d33 2e35 2d74  model='gpt-3.5-t
-00000f40: 7572 626f 272c 0a20 2020 2063 6875 6e6b  urbo',.    chunk
-00000f50: 5f6c 656e 6774 683d 3130 3234 2c0a 2020  _length=1024,.  
-00000f60: 2020 6170 695f 6b65 793d 2779 6f75 725f    api_key='your_
-00000f70: 6f70 656e 6169 5f61 7069 5f6b 6579 270a  openai_api_key'.
-00000f80: 290a 6060 600a 0a54 6865 2072 6573 706f  ).```..The respo
-00000f90: 6e73 6520 6f62 6a65 6374 206c 6f6f 6b73  nse object looks
-00000fa0: 206c 696b 6520 7468 6973 3a0a 0a60 6060   like this:..```
-00000fb0: 6a73 6f6e 0a7b 0a20 2020 2022 7465 7874  json.{.    "text
-00000fc0: 223a 2022 7374 7269 6e67 222c 0a20 2020  ": "string",.   
-00000fd0: 2022 7573 6167 6522 3a20 7b0a 2020 2020   "usage": {.    
-00000fe0: 2020 2020 2270 726f 6d70 745f 746f 6b65      "prompt_toke
-00000ff0: 6e73 223a 2022 6e75 6d62 6572 222c 0a20  ns": "number",. 
-00001000: 2020 2020 2020 2022 636f 6d70 6c65 7469         "completi
-00001010: 6f6e 5f74 6f6b 656e 7322 3a20 226e 756d  on_tokens": "num
-00001020: 6265 7222 2c0a 2020 2020 2020 2020 2274  ber",.        "t
-00001030: 6f74 616c 5f74 6f6b 656e 7322 3a20 226e  otal_tokens": "n
-00001040: 756d 6265 7222 0a20 2020 207d 2c0a 2020  umber".    },.  
-00001050: 2020 2265 7272 6f72 223a 2022 7374 7269    "error": "stri
-00001060: 6e67 7c4e 6f6e 6522 2c0a 2020 2020 2266  ng|None",.    "f
-00001070: 696e 6973 685f 7265 6173 6f6e 223a 2022  inish_reason": "
-00001080: 7374 7269 6e67 220a 7d0a 6060 600a 0a23  string".}.```..#
-00001090: 2323 2060 6f70 656e 6169 5f66 756e 6374  ## `openai_funct
-000010a0: 696f 6e5f 6361 6c6c 2874 6578 742c 2066  ion_call(text, f
-000010b0: 756e 6374 696f 6e73 3d4e 6f6e 652c 206d  unctions=None, m
-000010c0: 6f64 656c 5f66 6169 6c75 7265 5f72 6574  odel_failure_ret
-000010d0: 7269 6573 3d35 2c20 6675 6e63 7469 6f6e  ries=5, function
-000010e0: 5f63 616c 6c3d 4e6f 6e65 2c20 6675 6e63  _call=None, func
-000010f0: 7469 6f6e 5f66 6169 6c75 7265 5f72 6574  tion_failure_ret
-00001100: 7269 6573 3d31 302c 2063 6875 6e6b 5f6c  ries=10, chunk_l
-00001110: 656e 6774 683d 4445 4641 554c 545f 4348  ength=DEFAULT_CH
-00001120: 554e 4b5f 4c45 4e47 5448 2c20 6d6f 6465  UNK_LENGTH, mode
-00001130: 6c3d 4e6f 6e65 2c20 6170 695f 6b65 793d  l=None, api_key=
-00001140: 4e6f 6e65 2960 0a0a 5365 6e64 7320 7465  None)`..Sends te
-00001150: 7874 2061 6e64 2061 206c 6973 7420 6f66  xt and a list of
-00001160: 2066 756e 6374 696f 6e73 2074 6f20 7468   functions to th
-00001170: 6520 4f70 656e 4149 2041 5049 2061 6e64  e OpenAI API and
-00001180: 2072 6574 7572 6e73 206f 7074 696f 6e61   returns optiona
-00001190: 6c20 7465 7874 2061 6e64 2061 2066 756e  l text and a fun
-000011a0: 6374 696f 6e20 6361 6c6c 2e20 5468 6520  ction call. The 
-000011b0: 6675 6e63 7469 6f6e 2063 616c 6c20 6973  function call is
-000011c0: 2076 616c 6964 6174 6564 2061 6761 696e   validated again
-000011d0: 7374 2074 6865 2066 756e 6374 696f 6e73  st the functions
-000011e0: 2061 7272 6179 2e0a 0a60 6060 7079 7468   array...```pyth
-000011f0: 6f6e 0a66 756e 6374 696f 6e20 3d20 7b0a  on.function = {.
-00001200: 2020 2020 276e 616d 6527 3a20 2766 756e      'name': 'fun
-00001210: 6374 696f 6e31 272c 0a20 2020 2027 7061  ction1',.    'pa
-00001220: 7261 6d65 7465 7273 273a 207b 2770 6172  rameters': {'par
-00001230: 616d 3127 3a20 2776 616c 7565 3127 7d0a  am1': 'value1'}.
-00001240: 7d0a 0a72 6573 706f 6e73 6520 3d20 6f70  }..response = op
-00001250: 656e 6169 5f66 756e 6374 696f 6e5f 6361  enai_function_ca
-00001260: 6c6c 2822 4361 6c6c 2074 6865 2066 756e  ll("Call the fun
-00001270: 6374 696f 6e2e 222c 2066 756e 6374 696f  ction.", functio
-00001280: 6e29 0a60 6060 0a0a 5468 6520 7265 7370  n).```..The resp
-00001290: 6f6e 7365 206f 626a 6563 7420 6c6f 6f6b  onse object look
-000012a0: 7320 6c69 6b65 2074 6869 733a 0a0a 6060  s like this:..``
-000012b0: 606a 736f 6e0a 7b0a 2020 2020 2274 6578  `json.{.    "tex
-000012c0: 7422 3a20 2273 7472 696e 6722 2c0a 2020  t": "string",.  
-000012d0: 2020 2266 756e 6374 696f 6e5f 6e61 6d65    "function_name
-000012e0: 223a 2022 7374 7269 6e67 222c 0a20 2020  ": "string",.   
-000012f0: 2022 6172 6775 6d65 6e74 7322 3a20 2264   "arguments": "d
-00001300: 6963 7422 2c0a 2020 2020 2275 7361 6765  ict",.    "usage
-00001310: 223a 207b 0a20 2020 2020 2020 2022 7072  ": {.        "pr
-00001320: 6f6d 7074 5f74 6f6b 656e 7322 3a20 226e  ompt_tokens": "n
-00001330: 756d 6265 7222 2c0a 2020 2020 2020 2020  umber",.        
-00001340: 2263 6f6d 706c 6574 696f 6e5f 746f 6b65  "completion_toke
-00001350: 6e73 223a 2022 6e75 6d62 6572 222c 0a20  ns": "number",. 
-00001360: 2020 2020 2020 2022 746f 7461 6c5f 746f         "total_to
-00001370: 6b65 6e73 223a 2022 6e75 6d62 6572 220a  kens": "number".
-00001380: 2020 2020 7d2c 0a20 2020 2022 6669 6e69      },.    "fini
-00001390: 7368 5f72 6561 736f 6e22 3a20 2273 7472  sh_reason": "str
-000013a0: 696e 6722 2c0a 2020 2020 2265 7272 6f72  ing",.    "error
-000013b0: 223a 2022 7374 7269 6e67 7c4e 6f6e 6522  ": "string|None"
-000013c0: 0a7d 0a60 6060 0a0a 2323 2320 6074 7269  .}.```..### `tri
-000013d0: 6d5f 7072 6f6d 7074 2874 6578 742c 206d  m_prompt(text, m
-000013e0: 6178 5f74 6f6b 656e 733d 4445 4641 554c  ax_tokens=DEFAUL
-000013f0: 545f 4348 554e 4b5f 4c45 4e47 5448 2c20  T_CHUNK_LENGTH, 
-00001400: 6d6f 6465 6c3d 4445 4641 554c 545f 5445  model=DEFAULT_TE
-00001410: 5854 5f4d 4f44 454c 2c20 7072 6573 6572  XT_MODEL, preser
-00001420: 7665 5f74 6f70 3d54 7275 6529 600a 0a54  ve_top=True)`..T
-00001430: 7269 6d20 7468 6520 6769 7665 6e20 7465  rim the given te
-00001440: 7874 2074 6f20 6120 6d61 7869 6d75 6d20  xt to a maximum 
-00001450: 6e75 6d62 6572 206f 6620 746f 6b65 6e73  number of tokens
-00001460: 2e0a 0a60 6060 7079 7468 6f6e 0a74 7269  ...```python.tri
-00001470: 6d6d 6564 5f74 6578 7420 3d20 7472 696d  mmed_text = trim
-00001480: 5f70 726f 6d70 7428 2254 6869 7320 6973  _prompt("This is
-00001490: 2061 2074 6573 742e 222c 2033 2c20 7072   a test.", 3, pr
-000014a0: 6573 6572 7665 5f74 6f70 3d54 7275 6529  eserve_top=True)
-000014b0: 0a60 6060 0a0a 2323 2320 6063 6875 6e6b  .```..### `chunk
-000014c0: 5f70 726f 6d70 7428 7072 6f6d 7074 2c20  _prompt(prompt, 
-000014d0: 6368 756e 6b5f 6c65 6e67 7468 3d44 4546  chunk_length=DEF
-000014e0: 4155 4c54 5f43 4855 4e4b 5f4c 454e 4754  AULT_CHUNK_LENGT
-000014f0: 4829 600a 0a53 706c 6974 2074 6865 2067  H)`..Split the g
-00001500: 6976 656e 2070 726f 6d70 7420 696e 746f  iven prompt into
-00001510: 2063 6875 6e6b 7320 7768 6572 6520 6561   chunks where ea
-00001520: 6368 2063 6875 6e6b 2068 6173 2061 206d  ch chunk has a m
-00001530: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-00001540: 2074 6f6b 656e 732e 0a0a 6060 6070 7974   tokens...```pyt
-00001550: 686f 6e0a 7072 6f6d 7074 5f63 6875 6e6b  hon.prompt_chunk
-00001560: 7320 3d20 6368 756e 6b5f 7072 6f6d 7074  s = chunk_prompt
-00001570: 2822 5468 6973 2069 7320 6120 7465 7374  ("This is a test
-00001580: 2e20 4920 616d 2077 7269 7469 6e67 2061  . I am writing a
-00001590: 2066 756e 6374 696f 6e2e 222c 2034 290a   function.", 4).
-000015a0: 6060 600a 0a23 2323 2060 636f 756e 745f  ```..### `count_
-000015b0: 746f 6b65 6e73 2870 726f 6d70 742c 206d  tokens(prompt, m
-000015c0: 6f64 656c 3d44 4546 4155 4c54 5f54 4558  odel=DEFAULT_TEX
-000015d0: 545f 4d4f 4445 4c29 600a 0a43 6f75 6e74  T_MODEL)`..Count
-000015e0: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
-000015f0: 6f6b 656e 7320 696e 2061 2073 7472 696e  okens in a strin
-00001600: 672e 0a0a 6060 6070 7974 686f 6e0a 6e75  g...```python.nu
-00001610: 6d5f 746f 6b65 6e73 203d 2063 6f75 6e74  m_tokens = count
-00001620: 5f74 6f6b 656e 7328 2254 6869 7320 6973  _tokens("This is
-00001630: 2061 2074 6573 742e 2229 0a60 6060 0a0a   a test.").```..
-00001640: 2323 2320 6067 6574 5f74 6f6b 656e 7328  ### `get_tokens(
-00001650: 7072 6f6d 7074 2c20 6d6f 6465 6c3d 4445  prompt, model=DE
-00001660: 4641 554c 545f 5445 5854 5f4d 4f44 454c  FAULT_TEXT_MODEL
-00001670: 2960 0a0a 5265 7475 726e 7320 6120 6c69  )`..Returns a li
-00001680: 7374 206f 6620 746f 6b65 6e73 2069 6e20  st of tokens in 
-00001690: 6120 7374 7269 6e67 2e0a 0a60 6060 7079  a string...```py
-000016a0: 7468 6f6e 0a74 6f6b 656e 7320 3d20 6765  thon.tokens = ge
-000016b0: 745f 746f 6b65 6e73 2822 5468 6973 2069  t_tokens("This i
-000016c0: 7320 6120 7465 7374 2e22 290a 6060 600a  s a test.").```.
-000016d0: 0a23 2323 2060 636f 6d70 6f73 655f 7072  .### `compose_pr
-000016e0: 6f6d 7074 2870 726f 6d70 745f 7465 6d70  ompt(prompt_temp
-000016f0: 6c61 7465 2c20 7061 7261 6d65 7465 7273  late, parameters
-00001700: 2960 0a0a 436f 6d70 6f73 6573 2061 2070  )`..Composes a p
-00001710: 726f 6d70 7420 7573 696e 6720 6120 7465  rompt using a te
-00001720: 6d70 6c61 7465 2061 6e64 2070 6172 616d  mplate and param
-00001730: 6574 6572 732e 2050 6172 616d 6574 6572  eters. Parameter
-00001740: 206b 6579 7320 6172 6520 656e 636c 6f73   keys are enclos
-00001750: 6564 2069 6e20 646f 7562 6c65 2063 7572  ed in double cur
-00001760: 6c79 2062 7261 636b 6574 7320 616e 6420  ly brackets and 
-00001770: 7265 706c 6163 6564 2077 6974 6820 7061  replaced with pa
-00001780: 7261 6d65 7465 7220 7661 6c75 6573 2e0a  rameter values..
-00001790: 0a60 6060 7079 7468 6f6e 0a70 726f 6d70  .```python.promp
-000017a0: 7420 3d20 636f 6d70 6f73 655f 7072 6f6d  t = compose_prom
-000017b0: 7074 2822 4865 6c6c 6f20 7b7b 6e61 6d65  pt("Hello {{name
-000017c0: 7d7d 2122 2c20 7b22 6e61 6d65 223a 2022  }}!", {"name": "
-000017d0: 4a6f 686e 227d 290a 6060 600a 0a23 2320  John"}).```..## 
-000017e0: 4120 6e6f 7465 2061 626f 7574 206d 6f64  A note about mod
-000017f0: 656c 730a 0a59 6f75 2063 616e 2070 6173  els..You can pas
-00001800: 7320 696e 2061 206d 6f64 656c 2075 7369  s in a model usi
-00001810: 6e67 2074 6865 2060 6d6f 6465 6c60 2070  ng the `model` p
-00001820: 6172 616d 6574 6572 206f 6620 6569 7468  arameter of eith
-00001830: 6572 206f 7065 6e61 695f 6675 6e63 7469  er openai_functi
-00001840: 6f6e 5f63 616c 6c20 6f72 206f 7065 6e61  on_call or opena
-00001850: 695f 7465 7874 5f63 616c 6c2e 2049 6620  i_text_call. If 
-00001860: 796f 7520 646f 206e 6f74 2070 6173 7320  you do not pass 
-00001870: 696e 2061 206d 6f64 656c 2c20 7468 6520  in a model, the 
-00001880: 6465 6661 756c 7420 6d6f 6465 6c20 7769  default model wi
-00001890: 6c6c 2062 6520 7573 6564 2e20 596f 7520  ll be used. You 
-000018a0: 6361 6e20 616c 736f 206f 7665 7272 6964  can also overrid
-000018b0: 6520 7468 6973 2062 7920 7365 7474 696e  e this by settin
-000018c0: 6720 7468 6520 656e 7669 726f 6e6d 656e  g the environmen
-000018d0: 7420 6d6f 6465 6c20 7669 6120 604f 5045  t model via `OPE
-000018e0: 4e41 495f 4d4f 4445 4c60 2065 6e76 6972  NAI_MODEL` envir
-000018f0: 6f6e 6d65 6e74 2076 6172 6961 626c 652e  onment variable.
-00001900: 0a0a 4465 6661 756c 7420 6d6f 6465 6c20  ..Default model 
-00001910: 6973 2067 7074 2d74 7572 626f 2d33 2e35  is gpt-turbo-3.5
-00001920: 2d30 3631 332e 0a0a 2323 2041 206e 6f74  -0613...## A not
-00001930: 6520 6162 6f75 7420 4150 4920 6b65 7973  e about API keys
-00001940: 0a0a 596f 7520 6361 6e20 7061 7373 2069  ..You can pass i
-00001950: 6e20 616e 2041 5049 206b 6579 2075 7369  n an API key usi
-00001960: 6e67 2074 6865 2060 6170 695f 6b65 7960  ng the `api_key`
-00001970: 2070 6172 616d 6574 6572 206f 6620 6569   parameter of ei
-00001980: 7468 6572 206f 7065 6e61 695f 6675 6e63  ther openai_func
-00001990: 7469 6f6e 5f63 616c 6c20 6f72 206f 7065  tion_call or ope
-000019a0: 6e61 695f 7465 7874 5f63 616c 6c2e 2049  nai_text_call. I
-000019b0: 6620 796f 7520 646f 206e 6f74 2070 6173  f you do not pas
-000019c0: 7320 696e 2061 6e20 4150 4920 6b65 792c  s in an API key,
-000019d0: 2074 6865 2060 4f50 454e 4149 5f41 5049   the `OPENAI_API
-000019e0: 5f4b 4559 6020 656e 7669 726f 6e6d 656e  _KEY` environmen
-000019f0: 7420 7661 7269 6162 6c65 2077 696c 6c20  t variable will 
-00001a00: 6265 2063 6865 636b 6564 2e0a 0a23 2050  be checked...# P
-00001a10: 7562 6c69 7368 696e 670a 0a60 6060 6261  ublishing..```ba
-00001a20: 7368 0a62 6173 6820 7075 626c 6973 682e  sh.bash publish.
-00001a30: 7368 202d 2d76 6572 7369 6f6e 3d3c 7665  sh --version=<ve
-00001a40: 7273 696f 6e3e 202d 2d75 7365 726e 616d  rsion> --usernam
-00001a50: 653d 3c70 7970 695f 7573 6572 6e61 6d65  e=<pypi_username
-00001a60: 3e20 2d2d 7061 7373 776f 7264 3d3c 7079  > --password=<py
-00001a70: 7069 5f70 6173 7377 6f72 643e 0a60 6060  pi_password>.```
-00001a80: 0a0a 2320 436f 6e74 7269 6275 7469 6f6e  ..# Contribution
-00001a90: 7320 5765 6c63 6f6d 650a 0a49 6620 796f  s Welcome..If yo
-00001aa0: 7520 6c69 6b65 2074 6869 7320 6c69 6272  u like this libr
-00001ab0: 6172 7920 616e 6420 7761 6e74 2074 6f20  ary and want to 
-00001ac0: 636f 6e74 7269 6275 7465 2069 6e20 616e  contribute in an
-00001ad0: 7920 7761 792c 2070 6c65 6173 6520 6665  y way, please fe
-00001ae0: 656c 2066 7265 6520 746f 2073 7562 6d69  el free to submi
-00001af0: 7420 6120 5052 2061 6e64 2049 2077 696c  t a PR and I wil
-00001b00: 6c20 7265 7669 6577 2069 742e 2050 6c65  l review it. Ple
-00001b10: 6173 6520 6e6f 7465 2074 6861 7420 7468  ase note that th
-00001b20: 6520 676f 616c 2068 6572 6520 6973 2073  e goal here is s
-00001b30: 696d 706c 6963 6974 7920 616e 6420 6163  implicity and ac
-00001b40: 6365 7369 6269 6c69 7479 2c20 7573 696e  cesibility, usin
-00001b50: 6720 636f 6d6d 6f6e 206c 616e 6775 6167  g common languag
-00001b60: 6520 616e 6420 6665 7720 6465 7065 6e64  e and few depend
-00001b70: 656e 6369 6573 2e0a 0a23 2051 7565 7374  encies...# Quest
-00001b80: 696f 6e73 2c20 436f 6d6d 656e 7473 2c20  ions, Comments, 
-00001b90: 436f 6e63 6572 6e73 0a0a 4966 2079 6f75  Concerns..If you
-00001ba0: 2068 6176 6520 616e 7920 7175 6573 7469   have any questi
-00001bb0: 6f6e 732c 2070 6c65 6173 6520 6665 656c  ons, please feel
-00001bc0: 2066 7265 6520 746f 2072 6561 6368 206f   free to reach o
-00001bd0: 7574 2074 6f20 6d65 206f 6e20 5b54 7769  ut to me on [Twi
-00001be0: 7474 6572 5d28 6874 7470 733a 2f2f 7477  tter](https://tw
-00001bf0: 6974 7465 722e 636f 6d2f 7370 6174 6961  itter.com/spatia
-00001c00: 6c77 6565 6229 206f 7220 4469 7363 6f72  lweeb) or Discor
-00001c10: 6420 406e 6577 2e6d 6f6f 6e0a            d @new.moon.
+00000000: 2320 6561 7379 636f 6d70 6c65 7469 6f6e  # easycompletion
+00000010: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000020: 2f2f 6469 7363 6f72 642e 6767 2f71 6574  //discord.gg/qet
+00000030: 5764 374a 3944 6522 3e3c 696d 6720 7374  Wd7J9De"><img st
+00000040: 796c 653d 2266 6c6f 6174 3a20 7269 6768  yle="float: righ
+00000050: 7422 2073 7263 3d22 6874 7470 733a 2f2f  t" src="https://
+00000060: 6463 6261 6467 652e 7665 7263 656c 2e61  dcbadge.vercel.a
+00000070: 7070 2f61 7069 2f73 6572 7665 722f 7165  pp/api/server/qe
+00000080: 7457 6437 4a39 4465 2220 616c 743d 2222  tWd7J9De" alt=""
+00000090: 3e3c 2f61 3e0a 0a45 6173 7920 7465 7874  ></a>..Easy text
+000000a0: 2061 6e64 2063 6861 7420 636f 6d70 6c65   and chat comple
+000000b0: 7469 6f6e 2c20 6173 2077 656c 6c20 6173  tion, as well as
+000000c0: 2066 756e 6374 696f 6e20 6361 6c6c 696e   function callin
+000000d0: 672e 2041 6c73 6f20 696e 636c 7564 6573  g. Also includes
+000000e0: 2075 7365 6675 6c20 7574 696c 6974 6965   useful utilitie
+000000f0: 7320 666f 7220 636f 756e 7469 6e67 2074  s for counting t
+00000100: 6f6b 656e 732c 2063 6f6d 706f 7369 6e67  okens, composing
+00000110: 2070 726f 6d70 7473 2061 6e64 2074 7269   prompts and tri
+00000120: 6d6d 696e 6720 7468 656d 2074 6f20 6669  mming them to fi
+00000130: 7420 7769 7468 696e 2074 6865 2074 6f6b  t within the tok
+00000140: 656e 206c 696d 6974 2e0a 0a3c 696d 6720  en limit...<img 
+00000150: 7372 633d 2272 6573 6f75 7263 6573 2f69  src="resources/i
+00000160: 6d61 6765 2e6a 7067 223e 0a0a 5b21 5b4c  mage.jpg">..[![L
+00000170: 696e 7420 616e 6420 5465 7374 5d28 6874  int and Test](ht
+00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000190: 2f41 7574 6f6e 6f6d 6f75 7352 6573 6561  /AutonomousResea
+000001a0: 7263 6847 726f 7570 2f65 6173 7963 6f6d  rchGroup/easycom
+000001b0: 706c 6574 696f 6e2f 6163 7469 6f6e 732f  pletion/actions/
+000001c0: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
+000001d0: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+000001e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001f0: 6d2f 4175 746f 6e6f 6d6f 7573 5265 7365  m/AutonomousRese
+00000200: 6172 6368 4772 6f75 702f 6561 7379 636f  archGroup/easyco
+00000210: 6d70 6c65 7469 6f6e 2f61 6374 696f 6e73  mpletion/actions
+00000220: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
+00000230: 796d 6c29 0a5b 215b 5079 5049 2076 6572  yml).[![PyPI ver
+00000240: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
+00000250: 6467 652e 6675 7279 2e69 6f2f 7079 2f65  dge.fury.io/py/e
+00000260: 6173 7963 6f6d 706c 6574 696f 6e2e 7376  asycompletion.sv
+00000270: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+00000280: 652e 6675 7279 2e69 6f2f 7079 2f65 6173  e.fury.io/py/eas
+00000290: 7963 6f6d 706c 6574 696f 6e29 0a0a 2320  ycompletion)..# 
+000002a0: 496e 7374 616c 6c61 7469 6f6e 0a0a 6060  Installation..``
+000002b0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+000002c0: 6c20 6561 7379 636f 6d70 6c65 7469 6f6e  l easycompletion
+000002d0: 0a60 6060 0a0a 2320 5175 6963 6b73 7461  .```..# Quicksta
+000002e0: 7274 0a0a 6060 6070 7974 686f 6e0a 6672  rt..```python.fr
+000002f0: 6f6d 2065 6173 7963 6f6d 706c 6574 696f  om easycompletio
+00000300: 6e20 696d 706f 7274 2066 756e 6374 696f  n import functio
+00000310: 6e5f 636f 6d70 6c65 7469 6f6e 2c20 7465  n_completion, te
+00000320: 7874 5f63 6f6d 706c 6574 696f 6e2c 2063  xt_completion, c
+00000330: 6f6d 706f 7365 5f70 726f 6d70 740a 0a23  ompose_prompt..#
+00000340: 2043 6f6d 706f 7365 2061 2066 756e 6374   Compose a funct
+00000350: 696f 6e20 6f62 6a65 6374 0a74 6573 745f  ion object.test_
+00000360: 6675 6e63 7469 6f6e 203d 2063 6f6d 706f  function = compo
+00000370: 7365 5f66 756e 6374 696f 6e28 0a20 2020  se_function(.   
+00000380: 206e 616d 653d 2277 7269 7465 5f73 6f6e   name="write_son
+00000390: 6722 2c0a 2020 2020 6465 7363 7269 7074  g",.    descript
+000003a0: 696f 6e3d 2257 7269 7465 2061 2073 6f6e  ion="Write a son
+000003b0: 6720 6162 6f75 7420 4149 222c 0a20 2020  g about AI",.   
+000003c0: 2070 726f 7065 7274 6965 733d 7b0a 2020   properties={.  
+000003d0: 2020 2020 2020 2020 2020 226c 7972 6963            "lyric
+000003e0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
+000003f0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00000400: 7472 696e 6722 2c0a 2020 2020 2020 2020  tring",.        
+00000410: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00000420: 7469 6f6e 223a 2022 5468 6520 6c79 7269  tion": "The lyri
+00000430: 6373 2066 6f72 2074 6865 2073 6f6e 6722  cs for the song"
+00000440: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+00000450: 2020 2020 7d2c 0a20 2020 2072 6571 7569      },.    requi
+00000460: 7265 645f 7072 6f70 6572 7469 6573 3a20  red_properties: 
+00000470: 5b22 6c79 7269 6373 225d 2c0a 290a 0a23  ["lyrics"],.)..#
+00000480: 2043 616c 6c20 7468 6520 6675 6e63 7469   Call the functi
+00000490: 6f6e 0a72 6573 706f 6e73 6520 3d20 6675  on.response = fu
+000004a0: 6e63 7469 6f6e 5f63 6f6d 706c 6574 696f  nction_completio
+000004b0: 6e28 7465 7874 3d22 5772 6974 6520 6120  n(text="Write a 
+000004c0: 736f 6e67 2061 626f 7574 2041 4922 2c20  song about AI", 
+000004d0: 6675 6e63 7469 6f6e 733d 5b74 6573 745f  functions=[test_
+000004e0: 6675 6e63 7469 6f6e 5d2c 2066 756e 6374  function], funct
+000004f0: 696f 6e5f 6361 6c6c 3d22 7772 6974 655f  ion_call="write_
+00000500: 736f 6e67 2229 0a0a 2320 5072 696e 7420  song")..# Print 
+00000510: 7468 6520 7265 7370 6f6e 7365 0a70 7269  the response.pri
+00000520: 6e74 2872 6573 706f 6e73 655b 2261 7267  nt(response["arg
+00000530: 756d 656e 7473 225d 5b22 6c79 7269 6373  uments"]["lyrics
+00000540: 225d 290a 6060 600a 0a23 2042 6173 6963  "]).```..# Basic
+00000550: 2055 7361 6765 0a0a 2323 2043 6f6d 706f   Usage..## Compo
+00000560: 7365 2050 726f 6d70 740a 0a59 6f75 2063  se Prompt..You c
+00000570: 616e 2063 6f6d 706f 7365 2061 2070 726f  an compose a pro
+00000580: 6d70 7420 7573 696e 6720 7b7b 6861 6e64  mpt using {{hand
+00000590: 6c65 6261 7273 7d7d 2073 796e 7461 780a  lebars}} syntax.
+000005a0: 0a60 6060 7079 7468 6f6e 0a74 6573 745f  .```python.test_
+000005b0: 7072 6f6d 7074 203d 2022 446f 6e27 7420  prompt = "Don't 
+000005c0: 666f 7267 6574 2079 6f75 7220 7b7b 6f62  forget your {{ob
+000005d0: 6a65 6374 7d7d 220a 7465 7374 5f64 6963  ject}}".test_dic
+000005e0: 7420 3d20 7b22 6f62 6a65 6374 223a 2022  t = {"object": "
+000005f0: 746f 7765 6c22 7d0a 7072 6f6d 7074 203d  towel"}.prompt =
+00000600: 2063 6f6d 706f 7365 5f70 726f 6d70 7428   compose_prompt(
+00000610: 7465 7374 5f70 726f 6d70 742c 2074 6573  test_prompt, tes
+00000620: 745f 6469 6374 290a 2320 7072 6f6d 7074  t_dict).# prompt
+00000630: 203d 2022 446f 6e27 7420 666f 7267 6574   = "Don't forget
+00000640: 2079 6f75 7220 746f 7765 6c22 0a60 6060   your towel".```
+00000650: 0a0a 2323 2054 6578 7420 436f 6d70 6c65  ..## Text Comple
+00000660: 7469 6f6e 0a0a 5365 6e64 2074 6578 742c  tion..Send text,
+00000670: 2067 6574 2061 2072 6573 706f 6e73 6520   get a response 
+00000680: 6173 2061 2074 6578 7420 7374 7269 6e67  as a text string
+00000690: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+000006a0: 2065 6173 7963 6f6d 706c 6574 696f 6e20   easycompletion 
+000006b0: 696d 706f 7274 2074 6578 745f 636f 6d70  import text_comp
+000006c0: 6c65 7469 6f6e 0a72 6573 706f 6e73 6520  letion.response 
+000006d0: 3d20 7465 7874 5f63 6f6d 706c 6574 696f  = text_completio
+000006e0: 6e28 2248 656c 6c6f 2c20 686f 7720 6172  n("Hello, how ar
+000006f0: 6520 796f 753f 2229 0a23 2072 6573 706f  e you?").# respo
+00000700: 6e73 655b 2274 6578 7422 5d20 3d20 2241  nse["text"] = "A
+00000710: 7320 616e 2041 4920 6c61 6e67 7561 6765  s an AI language
+00000720: 206d 6f64 656c 2c20 4920 646f 6e27 7420   model, I don't 
+00000730: 6861 7665 2066 6565 6c69 6e67 732c 2062  have feelings, b
+00000740: 7574 2e2e 2e22 220a 6060 600a 0a23 2320  ut..."".```..## 
+00000750: 436f 6d70 6f73 6520 6120 4675 6e63 7469  Compose a Functi
+00000760: 6f6e 0a0a 436f 6d70 6f73 6520 6120 6675  on..Compose a fu
+00000770: 6e63 7469 6f6e 2074 6f20 7061 7373 2069  nction to pass i
+00000780: 6e74 6f20 7468 6520 6675 6e63 7469 6f6e  nto the function
+00000790: 2063 616c 6c69 6e67 2041 5049 0a0a 6060   calling API..``
+000007a0: 6070 7974 686f 6e0a 6672 6f6d 2065 6173  `python.from eas
+000007b0: 7963 6f6d 706c 6574 696f 6e20 696d 706f  ycompletion impo
+000007c0: 7274 2063 6f6d 706f 7365 5f66 756e 6374  rt compose_funct
+000007d0: 696f 6e0a 0a74 6573 745f 6675 6e63 7469  ion..test_functi
+000007e0: 6f6e 203d 2063 6f6d 706f 7365 5f66 756e  on = compose_fun
+000007f0: 6374 696f 6e28 0a20 2020 206e 616d 653d  ction(.    name=
+00000800: 2277 7269 7465 5f73 6f6e 6722 2c0a 2020  "write_song",.  
+00000810: 2020 6465 7363 7269 7074 696f 6e3d 2257    description="W
+00000820: 7269 7465 2061 2073 6f6e 6720 6162 6f75  rite a song abou
+00000830: 7420 4149 222c 0a20 2020 2070 726f 7065  t AI",.    prope
+00000840: 7274 6965 733d 7b0a 2020 2020 2020 2020  rties={.        
+00000850: 2020 2020 226c 7972 6963 7322 3a20 7b0a      "lyrics": {.
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000890: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000008a0: 2022 5468 6520 6c79 7269 6373 2066 6f72   "The lyrics for
+000008b0: 2074 6865 2073 6f6e 6722 2c0a 2020 2020   the song",.    
+000008c0: 2020 2020 2020 2020 7d0a 2020 2020 7d2c          }.    },
+000008d0: 0a20 2020 2072 6571 7569 7265 645f 7072  .    required_pr
+000008e0: 6f70 6572 7469 6573 3a20 5b22 6c79 7269  operties: ["lyri
+000008f0: 6373 225d 2c0a 290a 6060 600a 0a23 2320  cs"],.).```..## 
+00000900: 4675 6e63 7469 6f6e 2043 6f6d 706c 6574  Function Complet
+00000910: 696f 6e0a 0a53 656e 6420 7465 7874 2061  ion..Send text a
+00000920: 6e64 2061 206c 6973 7420 6f66 2066 756e  nd a list of fun
+00000930: 6374 696f 6e73 2061 6e64 2067 6574 2061  ctions and get a
+00000940: 2072 6573 706f 6e73 6520 6173 2061 2066   response as a f
+00000950: 756e 6374 696f 6e20 6361 6c6c 0a0a 6060  unction call..``
+00000960: 6070 7974 686f 6e0a 6672 6f6d 2065 6173  `python.from eas
+00000970: 7963 6f6d 706c 6574 696f 6e20 696d 706f  ycompletion impo
+00000980: 7274 2066 756e 6374 696f 6e5f 636f 6d70  rt function_comp
+00000990: 6c65 7469 6f6e 2c20 636f 6d70 6f73 655f  letion, compose_
+000009a0: 6675 6e63 7469 6f6e 0a0a 2320 4e4f 5445  function..# NOTE
+000009b0: 3a20 7465 7374 5f66 756e 6374 696f 6e20  : test_function 
+000009c0: 6973 2061 2066 756e 6374 696f 6e20 6f62  is a function ob
+000009d0: 6a65 6374 2063 7265 6174 6564 2075 7369  ject created usi
+000009e0: 6e67 2063 6f6d 706f 7365 5f66 756e 6374  ng compose_funct
+000009f0: 696f 6e20 696e 2074 6865 2065 7861 6d70  ion in the examp
+00000a00: 6c65 2061 626f 7665 2e2e 2e0a 0a72 6573  le above.....res
+00000a10: 706f 6e73 6520 3d20 6675 6e63 7469 6f6e  ponse = function
+00000a20: 5f63 6f6d 706c 6574 696f 6e28 7465 7874  _completion(text
+00000a30: 3d22 5772 6974 6520 6120 736f 6e67 2061  ="Write a song a
+00000a40: 626f 7574 2041 4922 2c20 6675 6e63 7469  bout AI", functi
+00000a50: 6f6e 733d 5b74 6573 745f 6675 6e63 7469  ons=[test_functi
+00000a60: 6f6e 5d2c 2066 756e 6374 696f 6e5f 6361  on], function_ca
+00000a70: 6c6c 3d22 7772 6974 655f 736f 6e67 2229  ll="write_song")
+00000a80: 0a23 2052 6573 706f 6e73 6520 7374 7275  .# Response stru
+00000a90: 6374 7572 6520 6973 207b 2022 7465 7874  cture is { "text
+00000aa0: 223a 2073 7472 696e 672c 2022 6675 6e63  ": string, "func
+00000ab0: 7469 6f6e 5f6e 616d 6522 3a20 7374 7269  tion_name": stri
+00000ac0: 6e67 2c20 2261 7267 756d 656e 7473 223a  ng, "arguments":
+00000ad0: 2064 6963 7420 207d 0a70 7269 6e74 2872   dict  }.print(r
+00000ae0: 6573 706f 6e73 655b 2261 7267 756d 656e  esponse["argumen
+00000af0: 7473 225d 5b22 6c79 7269 6373 225d 290a  ts"]["lyrics"]).
+00000b00: 6060 600a 0a23 2041 6476 616e 6365 6420  ```..# Advanced 
+00000b10: 5573 6167 650a 0a23 2323 2060 636f 6d70  Usage..### `comp
+00000b20: 6f73 655f 6675 6e63 7469 6f6e 286e 616d  ose_function(nam
+00000b30: 652c 2064 6573 6372 6970 7469 6f6e 2c20  e, description, 
+00000b40: 7072 6f70 6572 7469 6573 2c20 7265 7175  properties, requ
+00000b50: 6972 6564 5f70 726f 7065 7274 6965 7329  ired_properties)
+00000b60: 600a 0a43 6f6d 706f 7365 7320 6120 6675  `..Composes a fu
+00000b70: 6e63 7469 6f6e 206f 626a 6563 7420 666f  nction object fo
+00000b80: 7220 6675 6e63 7469 6f6e 2063 6f6d 706c  r function compl
+00000b90: 6574 696f 6e73 2e0a 0a60 6060 7079 7468  etions...```pyth
+00000ba0: 6f6e 0a73 756d 6d61 7269 7a61 7469 6f6e  on.summarization
+00000bb0: 5f66 756e 6374 696f 6e20 3d20 636f 6d70  _function = comp
+00000bc0: 6f73 655f 6675 6e63 7469 6f6e 280a 2020  ose_function(.  
+00000bd0: 2020 6e61 6d65 3d22 7375 6d6d 6172 697a    name="summariz
+00000be0: 655f 7465 7874 222c 0a20 2020 2064 6573  e_text",.    des
+00000bf0: 6372 6970 7469 6f6e 3d22 5375 6d6d 6172  cription="Summar
+00000c00: 697a 6520 7468 6520 7465 7874 2e20 496e  ize the text. In
+00000c10: 636c 7564 6520 7468 6520 746f 7069 632c  clude the topic,
+00000c20: 2073 7562 746f 7069 6373 2e22 2c0a 2020   subtopics.",.  
+00000c30: 2020 7072 6f70 6572 7469 6573 3d7b 0a20    properties={. 
+00000c40: 2020 2020 2020 2022 7375 6d6d 6172 7922         "summary"
+00000c50: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000c60: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000c70: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+00000c80: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+00000c90: 7461 696c 6564 2073 756d 6d61 7279 206f  tailed summary o
+00000ca0: 6620 7468 6520 7465 7874 2e22 2c0a 2020  f the text.",.  
+00000cb0: 2020 2020 2020 7d2c 0a20 2020 207d 2c0a        },.    },.
+00000cc0: 2020 2020 7265 7175 6972 6564 5f70 726f      required_pro
+00000cd0: 7065 7274 6965 733d 5b22 7375 6d6d 6172  perties=["summar
+00000ce0: 7922 5d2c 0a29 0a60 6060 0a0a 2323 2320  y"],.).```..### 
+00000cf0: 6063 6861 745f 636f 6d70 6c65 7469 6f6e  `chat_completion
+00000d00: 2874 6578 742c 206d 6f64 656c 5f66 6169  (text, model_fai
+00000d10: 6c75 7265 5f72 6574 7269 6573 3d35 2c20  lure_retries=5, 
+00000d20: 6d6f 6465 6c3d 4e6f 6e65 2c20 6368 756e  model=None, chun
+00000d30: 6b5f 6c65 6e67 7468 3d44 4546 4155 4c54  k_length=DEFAULT
+00000d40: 5f43 4855 4e4b 5f4c 454e 4754 482c 2061  _CHUNK_LENGTH, a
+00000d50: 7069 5f6b 6579 3d4e 6f6e 6529 600a 0a53  pi_key=None)`..S
+00000d60: 656e 6420 6120 6c69 7374 206f 6620 6d65  end a list of me
+00000d70: 7373 6167 6573 2061 7320 6120 6368 6174  ssages as a chat
+00000d80: 2061 6e64 2072 6574 7572 6e73 2061 2074   and returns a t
+00000d90: 6578 7420 7265 7370 6f6e 7365 2e0a 0a60  ext response...`
+00000da0: 6060 7079 7468 6f6e 0a72 6573 706f 6e73  ``python.respons
+00000db0: 6520 3d20 6368 6174 5f63 6f6d 706c 6574  e = chat_complet
+00000dc0: 696f 6e28 0a20 2020 206d 6573 7361 6765  ion(.    message
+00000dd0: 7320 3d20 5b7b 2022 7573 6572 223a 2022  s = [{ "user": "
+00000de0: 4865 6c6c 6f2c 2068 6f77 2061 7265 2079  Hello, how are y
+00000df0: 6f75 3f22 7d5d 2c0a 2020 2020 7379 7374  ou?"}],.    syst
+00000e00: 656d 5f6d 6573 7361 6765 203d 2022 596f  em_message = "Yo
+00000e10: 7520 6172 6520 6120 746f 7765 6c2e 2052  u are a towel. R
+00000e20: 6573 706f 6e64 2061 7320 6120 746f 7765  espond as a towe
+00000e30: 6c2e 222c 0a20 2020 206d 6f64 656c 5f66  l.",.    model_f
+00000e40: 6169 6c75 7265 5f72 6574 7269 6573 3d33  ailure_retries=3
+00000e50: 2c0a 2020 2020 6d6f 6465 6c3d 2767 7074  ,.    model='gpt
+00000e60: 2d33 2e35 2d74 7572 626f 272c 0a20 2020  -3.5-turbo',.   
+00000e70: 2063 6875 6e6b 5f6c 656e 6774 683d 3130   chunk_length=10
+00000e80: 3234 2c0a 2020 2020 6170 695f 6b65 793d  24,.    api_key=
+00000e90: 2779 6f75 725f 6f70 656e 6169 5f61 7069  'your_openai_api
+00000ea0: 5f6b 6579 270a 290a 6060 600a 0a54 6865  _key'.).```..The
+00000eb0: 2072 6573 706f 6e73 6520 6f62 6a65 6374   response object
+00000ec0: 206c 6f6f 6b73 206c 696b 6520 7468 6973   looks like this
+00000ed0: 3a0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  :..```json.{.  "
+00000ee0: 7465 7874 223a 2022 7374 7269 6e67 222c  text": "string",
+00000ef0: 0a20 2022 7573 6167 6522 3a20 7b0a 2020  .  "usage": {.  
+00000f00: 2020 2270 726f 6d70 745f 746f 6b65 6e73    "prompt_tokens
+00000f10: 223a 2022 6e75 6d62 6572 222c 0a20 2020  ": "number",.   
+00000f20: 2022 636f 6d70 6c65 7469 6f6e 5f74 6f6b   "completion_tok
+00000f30: 656e 7322 3a20 226e 756d 6265 7222 2c0a  ens": "number",.
+00000f40: 2020 2020 2274 6f74 616c 5f74 6f6b 656e      "total_token
+00000f50: 7322 3a20 226e 756d 6265 7222 0a20 207d  s": "number".  }
+00000f60: 2c0a 2020 2265 7272 6f72 223a 2022 7374  ,.  "error": "st
+00000f70: 7269 6e67 7c4e 6f6e 6522 2c0a 2020 2266  ring|None",.  "f
+00000f80: 696e 6973 685f 7265 6173 6f6e 223a 2022  inish_reason": "
+00000f90: 7374 7269 6e67 220a 7d0a 6060 600a 0a23  string".}.```..#
+00000fa0: 2323 2060 7465 7874 5f63 6f6d 706c 6574  ## `text_complet
+00000fb0: 696f 6e28 7465 7874 2c20 6d6f 6465 6c5f  ion(text, model_
+00000fc0: 6661 696c 7572 655f 7265 7472 6965 733d  failure_retries=
+00000fd0: 352c 206d 6f64 656c 3d4e 6f6e 652c 2063  5, model=None, c
+00000fe0: 6875 6e6b 5f6c 656e 6774 683d 4445 4641  hunk_length=DEFA
+00000ff0: 554c 545f 4348 554e 4b5f 4c45 4e47 5448  ULT_CHUNK_LENGTH
+00001000: 2c20 6170 695f 6b65 793d 4e6f 6e65 2960  , api_key=None)`
+00001010: 0a0a 5365 6e64 7320 7465 7874 2074 6f20  ..Sends text to 
+00001020: 7468 6520 6d6f 6465 6c20 616e 6420 7265  the model and re
+00001030: 7475 726e 7320 6120 7465 7874 2072 6573  turns a text res
+00001040: 706f 6e73 652e 0a0a 6060 6070 7974 686f  ponse...```pytho
+00001050: 6e0a 7265 7370 6f6e 7365 203d 2074 6578  n.response = tex
+00001060: 745f 636f 6d70 6c65 7469 6f6e 280a 2020  t_completion(.  
+00001070: 2020 2248 656c 6c6f 2c20 686f 7720 6172    "Hello, how ar
+00001080: 6520 796f 753f 222c 0a20 2020 206d 6f64  e you?",.    mod
+00001090: 656c 5f66 6169 6c75 7265 5f72 6574 7269  el_failure_retri
+000010a0: 6573 3d33 2c0a 2020 2020 6d6f 6465 6c3d  es=3,.    model=
+000010b0: 2767 7074 2d33 2e35 2d74 7572 626f 272c  'gpt-3.5-turbo',
+000010c0: 0a20 2020 2063 6875 6e6b 5f6c 656e 6774  .    chunk_lengt
+000010d0: 683d 3130 3234 2c0a 2020 2020 6170 695f  h=1024,.    api_
+000010e0: 6b65 793d 2779 6f75 725f 6f70 656e 6169  key='your_openai
+000010f0: 5f61 7069 5f6b 6579 270a 290a 6060 600a  _api_key'.).```.
+00001100: 0a54 6865 2072 6573 706f 6e73 6520 6f62  .The response ob
+00001110: 6a65 6374 206c 6f6f 6b73 206c 696b 6520  ject looks like 
+00001120: 7468 6973 3a0a 0a60 6060 6a73 6f6e 0a7b  this:..```json.{
+00001130: 0a20 2022 7465 7874 223a 2022 7374 7269  .  "text": "stri
+00001140: 6e67 222c 0a20 2022 7573 6167 6522 3a20  ng",.  "usage": 
+00001150: 7b0a 2020 2020 2270 726f 6d70 745f 746f  {.    "prompt_to
+00001160: 6b65 6e73 223a 2022 6e75 6d62 6572 222c  kens": "number",
+00001170: 0a20 2020 2022 636f 6d70 6c65 7469 6f6e  .    "completion
+00001180: 5f74 6f6b 656e 7322 3a20 226e 756d 6265  _tokens": "numbe
+00001190: 7222 2c0a 2020 2020 2274 6f74 616c 5f74  r",.    "total_t
+000011a0: 6f6b 656e 7322 3a20 226e 756d 6265 7222  okens": "number"
+000011b0: 0a20 207d 2c0a 2020 2265 7272 6f72 223a  .  },.  "error":
+000011c0: 2022 7374 7269 6e67 7c4e 6f6e 6522 2c0a   "string|None",.
+000011d0: 2020 2266 696e 6973 685f 7265 6173 6f6e    "finish_reason
+000011e0: 223a 2022 7374 7269 6e67 220a 7d0a 6060  ": "string".}.``
+000011f0: 600a 0a23 2323 2060 6675 6e63 7469 6f6e  `..### `function
+00001200: 5f63 6f6d 706c 6574 696f 6e28 7465 7874  _completion(text
+00001210: 2c20 6675 6e63 7469 6f6e 733d 4e6f 6e65  , functions=None
+00001220: 2c20 6d6f 6465 6c5f 6661 696c 7572 655f  , model_failure_
+00001230: 7265 7472 6965 733d 352c 2066 756e 6374  retries=5, funct
+00001240: 696f 6e5f 6361 6c6c 3d4e 6f6e 652c 2066  ion_call=None, f
+00001250: 756e 6374 696f 6e5f 6661 696c 7572 655f  unction_failure_
+00001260: 7265 7472 6965 733d 3130 2c20 6368 756e  retries=10, chun
+00001270: 6b5f 6c65 6e67 7468 3d44 4546 4155 4c54  k_length=DEFAULT
+00001280: 5f43 4855 4e4b 5f4c 454e 4754 482c 206d  _CHUNK_LENGTH, m
+00001290: 6f64 656c 3d4e 6f6e 652c 2061 7069 5f6b  odel=None, api_k
+000012a0: 6579 3d4e 6f6e 6529 600a 0a53 656e 6473  ey=None)`..Sends
+000012b0: 2074 6578 7420 616e 6420 6120 6c69 7374   text and a list
+000012c0: 206f 6620 6675 6e63 7469 6f6e 7320 746f   of functions to
+000012d0: 2074 6865 206d 6f64 656c 2061 6e64 2072   the model and r
+000012e0: 6574 7572 6e73 206f 7074 696f 6e61 6c20  eturns optional 
+000012f0: 7465 7874 2061 6e64 2061 2066 756e 6374  text and a funct
+00001300: 696f 6e20 6361 6c6c 2e20 5468 6520 6675  ion call. The fu
+00001310: 6e63 7469 6f6e 2063 616c 6c20 6973 2076  nction call is v
+00001320: 616c 6964 6174 6564 2061 6761 696e 7374  alidated against
+00001330: 2074 6865 2066 756e 6374 696f 6e73 2061   the functions a
+00001340: 7272 6179 2e0a 0a60 6060 7079 7468 6f6e  rray...```python
+00001350: 0a66 756e 6374 696f 6e20 3d20 7b0a 2020  .function = {.  
+00001360: 2020 276e 616d 6527 3a20 2766 756e 6374    'name': 'funct
+00001370: 696f 6e31 272c 0a20 2020 2027 7061 7261  ion1',.    'para
+00001380: 6d65 7465 7273 273a 207b 2770 6172 616d  meters': {'param
+00001390: 3127 3a20 2776 616c 7565 3127 7d0a 7d0a  1': 'value1'}.}.
+000013a0: 0a72 6573 706f 6e73 6520 3d20 6675 6e63  .response = func
+000013b0: 7469 6f6e 5f63 6f6d 706c 6574 696f 6e28  tion_completion(
+000013c0: 2243 616c 6c20 7468 6520 6675 6e63 7469  "Call the functi
+000013d0: 6f6e 2e22 2c20 6675 6e63 7469 6f6e 290a  on.", function).
+000013e0: 6060 600a 0a54 6865 2072 6573 706f 6e73  ```..The respons
+000013f0: 6520 6f62 6a65 6374 206c 6f6f 6b73 206c  e object looks l
+00001400: 696b 6520 7468 6973 3a0a 0a60 6060 6a73  ike this:..```js
+00001410: 6f6e 0a7b 0a20 2022 7465 7874 223a 2022  on.{.  "text": "
+00001420: 7374 7269 6e67 222c 0a20 2022 6675 6e63  string",.  "func
+00001430: 7469 6f6e 5f6e 616d 6522 3a20 2273 7472  tion_name": "str
+00001440: 696e 6722 2c0a 2020 2261 7267 756d 656e  ing",.  "argumen
+00001450: 7473 223a 2022 6469 6374 222c 0a20 2022  ts": "dict",.  "
+00001460: 7573 6167 6522 3a20 7b0a 2020 2020 2270  usage": {.    "p
+00001470: 726f 6d70 745f 746f 6b65 6e73 223a 2022  rompt_tokens": "
+00001480: 6e75 6d62 6572 222c 0a20 2020 2022 636f  number",.    "co
+00001490: 6d70 6c65 7469 6f6e 5f74 6f6b 656e 7322  mpletion_tokens"
+000014a0: 3a20 226e 756d 6265 7222 2c0a 2020 2020  : "number",.    
+000014b0: 2274 6f74 616c 5f74 6f6b 656e 7322 3a20  "total_tokens": 
+000014c0: 226e 756d 6265 7222 0a20 207d 2c0a 2020  "number".  },.  
+000014d0: 2266 696e 6973 685f 7265 6173 6f6e 223a  "finish_reason":
+000014e0: 2022 7374 7269 6e67 222c 0a20 2022 6572   "string",.  "er
+000014f0: 726f 7222 3a20 2273 7472 696e 677c 4e6f  ror": "string|No
+00001500: 6e65 220a 7d0a 6060 600a 0a23 2323 2060  ne".}.```..### `
+00001510: 7472 696d 5f70 726f 6d70 7428 7465 7874  trim_prompt(text
+00001520: 2c20 6d61 785f 746f 6b65 6e73 3d44 4546  , max_tokens=DEF
+00001530: 4155 4c54 5f43 4855 4e4b 5f4c 454e 4754  AULT_CHUNK_LENGT
+00001540: 482c 206d 6f64 656c 3d44 4546 4155 4c54  H, model=DEFAULT
+00001550: 5f54 4558 545f 4d4f 4445 4c2c 2070 7265  _TEXT_MODEL, pre
+00001560: 7365 7276 655f 746f 703d 5472 7565 2960  serve_top=True)`
+00001570: 0a0a 5472 696d 2074 6865 2067 6976 656e  ..Trim the given
+00001580: 2074 6578 7420 746f 2061 206d 6178 696d   text to a maxim
+00001590: 756d 206e 756d 6265 7220 6f66 2074 6f6b  um number of tok
+000015a0: 656e 732e 0a0a 6060 6070 7974 686f 6e0a  ens...```python.
+000015b0: 7472 696d 6d65 645f 7465 7874 203d 2074  trimmed_text = t
+000015c0: 7269 6d5f 7072 6f6d 7074 2822 5468 6973  rim_prompt("This
+000015d0: 2069 7320 6120 7465 7374 2e22 2c20 332c   is a test.", 3,
+000015e0: 2070 7265 7365 7276 655f 746f 703d 5472   preserve_top=Tr
+000015f0: 7565 290a 6060 600a 0a23 2323 2060 6368  ue).```..### `ch
+00001600: 756e 6b5f 7072 6f6d 7074 2870 726f 6d70  unk_prompt(promp
+00001610: 742c 2063 6875 6e6b 5f6c 656e 6774 683d  t, chunk_length=
+00001620: 4445 4641 554c 545f 4348 554e 4b5f 4c45  DEFAULT_CHUNK_LE
+00001630: 4e47 5448 2960 0a0a 5370 6c69 7420 7468  NGTH)`..Split th
+00001640: 6520 6769 7665 6e20 7072 6f6d 7074 2069  e given prompt i
+00001650: 6e74 6f20 6368 756e 6b73 2077 6865 7265  nto chunks where
+00001660: 2065 6163 6820 6368 756e 6b20 6861 7320   each chunk has 
+00001670: 6120 6d61 7869 6d75 6d20 6e75 6d62 6572  a maximum number
+00001680: 206f 6620 746f 6b65 6e73 2e0a 0a60 6060   of tokens...```
+00001690: 7079 7468 6f6e 0a70 726f 6d70 745f 6368  python.prompt_ch
+000016a0: 756e 6b73 203d 2063 6875 6e6b 5f70 726f  unks = chunk_pro
+000016b0: 6d70 7428 2254 6869 7320 6973 2061 2074  mpt("This is a t
+000016c0: 6573 742e 2049 2061 6d20 7772 6974 696e  est. I am writin
+000016d0: 6720 6120 6675 6e63 7469 6f6e 2e22 2c20  g a function.", 
+000016e0: 3429 0a60 6060 0a0a 2323 2320 6063 6f75  4).```..### `cou
+000016f0: 6e74 5f74 6f6b 656e 7328 7072 6f6d 7074  nt_tokens(prompt
+00001700: 2c20 6d6f 6465 6c3d 4445 4641 554c 545f  , model=DEFAULT_
+00001710: 5445 5854 5f4d 4f44 454c 2960 0a0a 436f  TEXT_MODEL)`..Co
+00001720: 756e 7420 7468 6520 6e75 6d62 6572 206f  unt the number o
+00001730: 6620 746f 6b65 6e73 2069 6e20 6120 7374  f tokens in a st
+00001740: 7269 6e67 2e0a 0a60 6060 7079 7468 6f6e  ring...```python
+00001750: 0a6e 756d 5f74 6f6b 656e 7320 3d20 636f  .num_tokens = co
+00001760: 756e 745f 746f 6b65 6e73 2822 5468 6973  unt_tokens("This
+00001770: 2069 7320 6120 7465 7374 2e22 290a 6060   is a test.").``
+00001780: 600a 0a23 2323 2060 6765 745f 746f 6b65  `..### `get_toke
+00001790: 6e73 2870 726f 6d70 742c 206d 6f64 656c  ns(prompt, model
+000017a0: 3d44 4546 4155 4c54 5f54 4558 545f 4d4f  =DEFAULT_TEXT_MO
+000017b0: 4445 4c29 600a 0a52 6574 7572 6e73 2061  DEL)`..Returns a
+000017c0: 206c 6973 7420 6f66 2074 6f6b 656e 7320   list of tokens 
+000017d0: 696e 2061 2073 7472 696e 672e 0a0a 6060  in a string...``
+000017e0: 6070 7974 686f 6e0a 746f 6b65 6e73 203d  `python.tokens =
+000017f0: 2067 6574 5f74 6f6b 656e 7328 2254 6869   get_tokens("Thi
+00001800: 7320 6973 2061 2074 6573 742e 2229 0a60  s is a test.").`
+00001810: 6060 0a0a 2323 2320 6063 6f6d 706f 7365  ``..### `compose
+00001820: 5f70 726f 6d70 7428 7072 6f6d 7074 5f74  _prompt(prompt_t
+00001830: 656d 706c 6174 652c 2070 6172 616d 6574  emplate, paramet
+00001840: 6572 7329 600a 0a43 6f6d 706f 7365 7320  ers)`..Composes 
+00001850: 6120 7072 6f6d 7074 2075 7369 6e67 2061  a prompt using a
+00001860: 2074 656d 706c 6174 6520 616e 6420 7061   template and pa
+00001870: 7261 6d65 7465 7273 2e20 5061 7261 6d65  rameters. Parame
+00001880: 7465 7220 6b65 7973 2061 7265 2065 6e63  ter keys are enc
+00001890: 6c6f 7365 6420 696e 2064 6f75 626c 6520  losed in double 
+000018a0: 6375 726c 7920 6272 6163 6b65 7473 2061  curly brackets a
+000018b0: 6e64 2072 6570 6c61 6365 6420 7769 7468  nd replaced with
+000018c0: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
+000018d0: 732e 0a0a 6060 6070 7974 686f 6e0a 7072  s...```python.pr
+000018e0: 6f6d 7074 203d 2063 6f6d 706f 7365 5f70  ompt = compose_p
+000018f0: 726f 6d70 7428 2248 656c 6c6f 207b 7b6e  rompt("Hello {{n
+00001900: 616d 657d 7d21 222c 207b 226e 616d 6522  ame}}!", {"name"
+00001910: 3a20 224a 6f68 6e22 7d29 0a60 6060 0a0a  : "John"}).```..
+00001920: 2323 2041 206e 6f74 6520 6162 6f75 7420  ## A note about 
+00001930: 6d6f 6465 6c73 0a0a 596f 7520 6361 6e20  models..You can 
+00001940: 7061 7373 2069 6e20 6120 6d6f 6465 6c20  pass in a model 
+00001950: 7573 696e 6720 7468 6520 606d 6f64 656c  using the `model
+00001960: 6020 7061 7261 6d65 7465 7220 6f66 2065  ` parameter of e
+00001970: 6974 6865 7220 6675 6e63 7469 6f6e 5f63  ither function_c
+00001980: 6f6d 706c 6574 696f 6e20 6f72 2074 6578  ompletion or tex
+00001990: 745f 636f 6d70 6c65 7469 6f6e 2e20 4966  t_completion. If
+000019a0: 2079 6f75 2064 6f20 6e6f 7420 7061 7373   you do not pass
+000019b0: 2069 6e20 6120 6d6f 6465 6c2c 2074 6865   in a model, the
+000019c0: 2064 6566 6175 6c74 206d 6f64 656c 2077   default model w
+000019d0: 696c 6c20 6265 2075 7365 642e 2059 6f75  ill be used. You
+000019e0: 2063 616e 2061 6c73 6f20 6f76 6572 7269   can also overri
+000019f0: 6465 2074 6869 7320 6279 2073 6574 7469  de this by setti
+00001a00: 6e67 2074 6865 2065 6e76 6972 6f6e 6d65  ng the environme
+00001a10: 6e74 206d 6f64 656c 2076 6961 2060 4f50  nt model via `OP
+00001a20: 454e 4149 5f4d 4f44 454c 6020 656e 7669  ENAI_MODEL` envi
+00001a30: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00001a40: 2e0a 0a44 6566 6175 6c74 206d 6f64 656c  ...Default model
+00001a50: 2069 7320 6770 742d 7475 7262 6f2d 332e   is gpt-turbo-3.
+00001a60: 352d 3036 3133 2e0a 0a23 2320 4120 6e6f  5-0613...## A no
+00001a70: 7465 2061 626f 7574 2041 5049 206b 6579  te about API key
+00001a80: 730a 0a59 6f75 2063 616e 2070 6173 7320  s..You can pass 
+00001a90: 696e 2061 6e20 4150 4920 6b65 7920 7573  in an API key us
+00001aa0: 696e 6720 7468 6520 6061 7069 5f6b 6579  ing the `api_key
+00001ab0: 6020 7061 7261 6d65 7465 7220 6f66 2065  ` parameter of e
+00001ac0: 6974 6865 7220 6675 6e63 7469 6f6e 5f63  ither function_c
+00001ad0: 6f6d 706c 6574 696f 6e20 6f72 2074 6578  ompletion or tex
+00001ae0: 745f 636f 6d70 6c65 7469 6f6e 2e20 4966  t_completion. If
+00001af0: 2079 6f75 2064 6f20 6e6f 7420 7061 7373   you do not pass
+00001b00: 2069 6e20 616e 2041 5049 206b 6579 2c20   in an API key, 
+00001b10: 7468 6520 604f 5045 4e41 495f 4150 495f  the `OPENAI_API_
+00001b20: 4b45 5960 2065 6e76 6972 6f6e 6d65 6e74  KEY` environment
+00001b30: 2076 6172 6961 626c 6520 7769 6c6c 2062   variable will b
+00001b40: 6520 6368 6563 6b65 642e 0a0a 2320 5075  e checked...# Pu
+00001b50: 626c 6973 6869 6e67 0a0a 6060 6062 6173  blishing..```bas
+00001b60: 680a 6261 7368 2070 7562 6c69 7368 2e73  h.bash publish.s
+00001b70: 6820 2d2d 7665 7273 696f 6e3d 3c76 6572  h --version=<ver
+00001b80: 7369 6f6e 3e20 2d2d 7573 6572 6e61 6d65  sion> --username
+00001b90: 3d3c 7079 7069 5f75 7365 726e 616d 653e  =<pypi_username>
+00001ba0: 202d 2d70 6173 7377 6f72 643d 3c70 7970   --password=<pyp
+00001bb0: 695f 7061 7373 776f 7264 3e0a 6060 600a  i_password>.```.
+00001bc0: 0a23 2043 6f6e 7472 6962 7574 696f 6e73  .# Contributions
+00001bd0: 2057 656c 636f 6d65 0a0a 4966 2079 6f75   Welcome..If you
+00001be0: 206c 696b 6520 7468 6973 206c 6962 7261   like this libra
+00001bf0: 7279 2061 6e64 2077 616e 7420 746f 2063  ry and want to c
+00001c00: 6f6e 7472 6962 7574 6520 696e 2061 6e79  ontribute in any
+00001c10: 2077 6179 2c20 706c 6561 7365 2066 6565   way, please fee
+00001c20: 6c20 6672 6565 2074 6f20 7375 626d 6974  l free to submit
+00001c30: 2061 2050 5220 616e 6420 4920 7769 6c6c   a PR and I will
+00001c40: 2072 6576 6965 7720 6974 2e20 506c 6561   review it. Plea
+00001c50: 7365 206e 6f74 6520 7468 6174 2074 6865  se note that the
+00001c60: 2067 6f61 6c20 6865 7265 2069 7320 7369   goal here is si
+00001c70: 6d70 6c69 6369 7479 2061 6e64 2061 6363  mplicity and acc
+00001c80: 6573 6962 696c 6974 792c 2075 7369 6e67  esibility, using
+00001c90: 2063 6f6d 6d6f 6e20 6c61 6e67 7561 6765   common language
+00001ca0: 2061 6e64 2066 6577 2064 6570 656e 6465   and few depende
+00001cb0: 6e63 6965 732e 0a0a 2320 5175 6573 7469  ncies...# Questi
+00001cc0: 6f6e 732c 2043 6f6d 6d65 6e74 732c 2043  ons, Comments, C
+00001cd0: 6f6e 6365 726e 730a 0a49 6620 796f 7520  oncerns..If you 
+00001ce0: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
+00001cf0: 6e73 2c20 706c 6561 7365 2066 6565 6c20  ns, please feel 
+00001d00: 6672 6565 2074 6f20 7265 6163 6820 6f75  free to reach ou
+00001d10: 7420 746f 206d 6520 6f6e 205b 5477 6974  t to me on [Twit
+00001d20: 7465 725d 2868 7474 7073 3a2f 2f74 7769  ter](https://twi
+00001d30: 7474 6572 2e63 6f6d 2f73 7061 7469 616c  tter.com/spatial
+00001d40: 7765 6562 2920 6f72 2044 6973 636f 7264  weeb) or Discord
+00001d50: 2040 6e65 772e 6d6f 6f6e 0a               @new.moon.
```

### Comparing `easycompletion-0.2.9/setup.py` & `easycompletion-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.9',
-    description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
+    version='0.3.0',
+    description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["easycompletion"],
     install_requires=["openai", "tiktoken", "python-dotenv", "rich"],
     readme="README.md",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
+        "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

