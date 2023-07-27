# Comparing `tmp/llm-claude-0.2.0.tar.gz` & `tmp/llm-claude-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-claude-0.2.0.tar", last modified: Sun Jul 23 10:40:43 2023, max compression
+gzip compressed data, was "llm-claude-0.3.0.tar", last modified: Thu Jul 27 22:09:17 2023, max compression
```

## Comparing `llm-claude-0.2.0.tar` & `llm-claude-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-23 10:40:29.000000 llm-claude-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-23 10:40:43.660306 llm-claude-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-23 10:40:29.000000 llm-claude-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.656306 llm-claude-0.2.0/llm_claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/llm_claude/vendored_anthropic/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46863 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_base_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/llm_claude/vendored_anthropic/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/resources/completions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/llm_claude/vendored_anthropic/types/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/types/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-23 10:40:29.000000 llm-claude-0.2.0/llm_claude/vendored_anthropic/types/completion_create_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.656306 llm-claude-0.2.0/llm_claude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-23 10:40:43.000000 llm-claude-0.2.0/llm_claude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-23 10:40:29.000000 llm-claude-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 10:40:43.660306 llm-claude-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:40:43.660306 llm-claude-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-23 10:40:29.000000 llm-claude-0.2.0/tests/test_llm_claude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 22:09:03.000000 llm-claude-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 22:09:17.751294 llm-claude-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-27 22:09:03.000000 llm-claude-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46863 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/completions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-27 22:09:03.000000 llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion_create_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.747294 llm-claude-0.3.0/llm_claude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 22:09:17.000000 llm-claude-0.3.0/llm_claude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 22:09:03.000000 llm-claude-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:09:17.751294 llm-claude-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:09:17.751294 llm-claude-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-27 22:09:03.000000 llm-claude-0.3.0/tests/test_llm_claude.py
```

### Comparing `llm-claude-0.2.0/LICENSE` & `llm-claude-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/PKG-INFO` & `llm-claude-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-claude
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM plugin for Anthropic's Claude
 Author: Tom Viner
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tomviner/llm-claude
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -39,29 +39,43 @@
 Enter key: <paste key here>
 ```
 
 ## Usage
 
 This plugin adds models called `claude` and `claude-instant`.
 
-Anthropic [describe them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
+Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
-
-> **Claude Instant**: low-latency, high throughput
-> **Claude**: superior performance on tasks that require complex reasoning
+> - **Claude Instant**: low-latency, high throughput
+> - **Claude**: superior performance on tasks that require complex reasoning
 
 You can execute them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
+```
 
+```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
 ```
 
+## Options
+
+- `max_tokens_to_sample`, default 10_000: The maximum number of tokens to generate before stopping
+
+Use like this:
+```bash
+llm -m claude -o max_tokens_to_sample 20 "Sing me the alphabet"
+ Here is the alphabet song:
+
+A B C D E F G
+H I J
+```
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
     cd llm-claude
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `llm-claude-0.2.0/README.md` & `llm-claude-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,29 +26,43 @@
 Enter key: <paste key here>
 ```
 
 ## Usage
 
 This plugin adds models called `claude` and `claude-instant`.
 
-Anthropic [describe them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
+Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
-
-> **Claude Instant**: low-latency, high throughput
-> **Claude**: superior performance on tasks that require complex reasoning
+> - **Claude Instant**: low-latency, high throughput
+> - **Claude**: superior performance on tasks that require complex reasoning
 
 You can execute them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
+```
 
+```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
 ```
 
+## Options
+
+- `max_tokens_to_sample`, default 10_000: The maximum number of tokens to generate before stopping
+
+Use like this:
+```bash
+llm -m claude -o max_tokens_to_sample 20 "Sing me the alphabet"
+ Here is the alphabet song:
+
+A B C D E F G
+H I J
+```
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
     cd llm-claude
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `llm-claude-0.2.0/llm_claude/__init__.py` & `llm-claude-0.3.0/llm_claude/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from typing import Optional
+
 import click
-import httpx
 import llm
+from pydantic import Field, field_validator
 
 from .vendored_anthropic import AI_PROMPT, HUMAN_PROMPT, Anthropic
 
 
 @llm.hookimpl
 def register_models(register):
     # https://docs.anthropic.com/claude/reference/selecting-a-model
@@ -16,14 +18,26 @@
 
 
 class Claude(llm.Model):
     needs_key = "claude"
     key_env_var = "ANTHROPIC_API_KEY"
     can_stream = True
 
+    class Options(llm.Options):
+        max_tokens_to_sample: Optional[int] = Field(
+            description="The maximum number of tokens to generate before stopping",
+            default=10_000,
+        )
+
+        @field_validator("max_tokens_to_sample")
+        def validate_length(cls, max_tokens_to_sample):
+            if not (0 < max_tokens_to_sample <= 1_000_000):
+                raise ValueError("max_tokens_to_sample must be in range 1-1,000,000")
+            return max_tokens_to_sample
+
     def __init__(self, model_id):
         self.model_id = model_id
 
     def generate_prompt_messages(self, prompt, conversation):
         if conversation:
             for response in conversation.responses:
                 yield self.build_prompt(response.prompt.prompt, response.text())
@@ -36,15 +50,15 @@
     def execute(self, prompt, stream, response, conversation):
         anthropic = Anthropic(api_key=self.get_key())
 
         prompt_str = "".join(self.generate_prompt_messages(prompt.prompt, conversation))
 
         completion = anthropic.completions.create(
             model=self.model_id,
-            max_tokens_to_sample=300,
+            max_tokens_to_sample=prompt.options.max_tokens_to_sample,
             prompt=prompt_str,
             stream=stream,
         )
         if stream:
             for comp in completion:
                 yield comp.completion
         else:
```

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/__init__.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_base_client.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_client.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_base_exceptions.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_client.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_client.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_exceptions.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_models.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_qs.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_resource.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_streaming.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_tokenizers.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_types.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/__init__.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/_transform.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/_utils/_utils.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/resources/completions.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/resources/completions.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/types/completion.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude/vendored_anthropic/types/completion_create_params.py` & `llm-claude-0.3.0/llm_claude/vendored_anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/llm_claude.egg-info/PKG-INFO` & `llm-claude-0.3.0/llm_claude.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-claude
-Version: 0.2.0
+Version: 0.3.0
 Summary: LLM plugin for Anthropic's Claude
 Author: Tom Viner
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tomviner/llm-claude
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -39,29 +39,43 @@
 Enter key: <paste key here>
 ```
 
 ## Usage
 
 This plugin adds models called `claude` and `claude-instant`.
 
-Anthropic [describe them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
+Anthropic [describes them as](https://docs.anthropic.com/claude/reference/selecting-a-model):
 
 > two families of models, both of which support 100,000 token context windows:
-
-> **Claude Instant**: low-latency, high throughput
-> **Claude**: superior performance on tasks that require complex reasoning
+> - **Claude Instant**: low-latency, high throughput
+> - **Claude**: superior performance on tasks that require complex reasoning
 
 You can execute them like this:
 
 ```bash
 llm -m claude-instant "Ten great names for a new space station"
+```
 
+```bash
 llm -m claude "Compare and contrast the leadership styles of Abraham Lincoln and Boris Johnson."
 ```
 
+## Options
+
+- `max_tokens_to_sample`, default 10_000: The maximum number of tokens to generate before stopping
+
+Use like this:
+```bash
+llm -m claude -o max_tokens_to_sample 20 "Sing me the alphabet"
+ Here is the alphabet song:
+
+A B C D E F G
+H I J
+```
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 
     cd llm-claude
     python3 -m venv venv
     source venv/bin/activate
```

### Comparing `llm-claude-0.2.0/llm_claude.egg-info/SOURCES.txt` & `llm-claude-0.3.0/llm_claude.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-claude-0.2.0/pyproject.toml` & `llm-claude-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-claude"
-version = "0.2.0"
+version = "0.3.0"
 
 description = "LLM plugin for Anthropic's Claude"
 readme = "README.md"
 authors = [{name = "Tom Viner"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

