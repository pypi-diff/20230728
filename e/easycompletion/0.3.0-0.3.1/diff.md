# Comparing `tmp/easycompletion-0.3.0.tar.gz` & `tmp/easycompletion-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.3.0.tar", last modified: Fri Jul 28 15:34:13 2023, max compression
+gzip compressed data, was "easycompletion-0.3.1.tar", last modified: Fri Jul 28 16:29:13 2023, max compression
```

## Comparing `easycompletion-0.3.0.tar` & `easycompletion-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 15:34:01.000000 easycompletion-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 15:34:13.468891 easycompletion-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-28 15:34:01.000000 easycompletion-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-28 15:34:01.000000 easycompletion-0.3.0/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:34:13.468891 easycompletion-0.3.0/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 15:34:13.000000 easycompletion-0.3.0/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:34:13.468891 easycompletion-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 15:34:01.000000 easycompletion-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:29:13.062634 easycompletion-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 16:29:01.000000 easycompletion-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 16:29:13.062634 easycompletion-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-28 16:29:01.000000 easycompletion-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:29:13.062634 easycompletion-0.3.1/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 16:29:01.000000 easycompletion-0.3.1/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 16:29:01.000000 easycompletion-0.3.1/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 16:29:01.000000 easycompletion-0.3.1/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-28 16:29:01.000000 easycompletion-0.3.1/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-28 16:29:01.000000 easycompletion-0.3.1/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:29:13.062634 easycompletion-0.3.1/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 16:29:13.000000 easycompletion-0.3.1/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 16:29:13.000000 easycompletion-0.3.1/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:29:13.000000 easycompletion-0.3.1/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:29:13.000000 easycompletion-0.3.1/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 16:29:13.000000 easycompletion-0.3.1/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:29:13.062634 easycompletion-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 16:29:01.000000 easycompletion-0.3.1/setup.py
```

### Comparing `easycompletion-0.3.0/LICENSE` & `easycompletion-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/PKG-INFO` & `easycompletion-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.0/README.md` & `easycompletion-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/easycompletion/__init__.py` & `easycompletion-0.3.1/easycompletion/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .model import (
     function_completion,
     text_completion,
     compose_function,
 )
 
 openai_function_call = function_completion
-openai_text_completion = text_completion
+openai_text_call = text_completion
 
 from .prompt import (
     compose_prompt,
     trim_prompt,
     chunk_prompt,
     count_tokens,
     get_tokens,
```

### Comparing `easycompletion-0.3.0/easycompletion/constants.py` & `easycompletion-0.3.1/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/easycompletion/logger.py` & `easycompletion-0.3.1/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/easycompletion/model.py` & `easycompletion-0.3.1/easycompletion/model.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/easycompletion/prompt.py` & `easycompletion-0.3.1/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.0/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.3.1/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.0/setup.py` & `easycompletion-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.3.0',
+    version='0.3.1',
     description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

