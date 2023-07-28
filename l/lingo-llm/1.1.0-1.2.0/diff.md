# Comparing `tmp/lingo-llm-1.1.0.tar.gz` & `tmp/lingo-llm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingo-llm-1.1.0.tar", last modified: Fri Jul 28 13:07:58 2023, max compression
+gzip compressed data, was "lingo-llm-1.2.0.tar", last modified: Fri Jul 28 13:09:25 2023, max compression
```

## Comparing `lingo-llm-1.1.0.tar` & `lingo-llm-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.603478 lingo-llm-1.1.0/
--rw-rw-rw-   0        0        0    11558 2023-07-28 11:54:47.000000 lingo-llm-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      228 2023-07-28 13:07:58.602474 lingo-llm-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.570605 lingo-llm-1.1.0/lingo/
--rw-rw-rw-   0        0        0     4698 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/__init__.py
--rw-rw-rw-   0        0        0      290 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/__main__.py
--rw-rw-rw-   0        0        0    25947 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/argments.py
--rw-rw-rw-   0        0        0     1648 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/dataset.py
--rw-rw-rw-   0        0        0     3008 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/deepspeed_file.py
--rw-rw-rw-   0        0        0     7983 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/inference.py
--rw-rw-rw-   0        0        0     2999 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/initialize.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.571605 lingo-llm-1.1.0/lingo/kernels/
--rw-rw-rw-   0        0        0     3092 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/kernels/__init__.py
--rw-rw-rw-   0        0        0    30080 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/lomo.py
--rw-rw-rw-   0        0        0    13985 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/lora.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.585599 lingo-llm-1.1.0/lingo/models/
--rw-rw-rw-   0        0        0    17109 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/GLM130B_model.py
--rw-rw-rw-   0        0        0     5831 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/GPT2_model.py
--rw-rw-rw-   0        0        0     6814 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/GPTNeo_model.py
--rw-rw-rw-   0        0        0    10234 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/LLAMA_model.py
--rw-rw-rw-   0        0        0     8290 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/LLAMAv2_model.py
--rw-rw-rw-   0        0        0    17780 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/__init__.py
--rw-rw-rw-   0        0        0    17431 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/basemodel.py
--rw-rw-rw-   0        0        0    16024 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/model_io.py
--rw-rw-rw-   0        0        0    31589 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/models/transformers_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.589602 lingo-llm-1.1.0/lingo/quantization/
--rw-rw-rw-   0        0        0     5522 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/quantization/__init__.py
--rw-rw-rw-   0        0        0     1321 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/quantization/functional.py
--rw-rw-rw-   0        0        0     9662 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/quantization/layers.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.593611 lingo-llm-1.1.0/lingo/scaled_rope/
--rw-rw-rw-   0        0        0        0 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/scaled_rope/__init__.py
--rw-rw-rw-   0        0        0      562 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/scaled_rope/configuration_llama.py
--rw-rw-rw-   0        0        0    59267 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/scaled_rope/modelling_llama.py
--rw-rw-rw-   0        0        0      114 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/setting.py
--rw-rw-rw-   0        0        0    28630 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/trainer.py
--rw-rw-rw-   0        0        0    26409 2023-07-28 11:45:21.000000 lingo-llm-1.1.0/lingo/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:07:58.601469 lingo-llm-1.1.0/lingo_llm.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-28 13:07:58.000000 lingo-llm-1.1.0/lingo_llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2023-07-28 13:07:58.000000 lingo-llm-1.1.0/lingo_llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:07:58.000000 lingo-llm-1.1.0/lingo_llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-07-28 13:07:58.000000 lingo-llm-1.1.0/lingo_llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 13:07:58.000000 lingo-llm-1.1.0/lingo_llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 13:07:58.603478 lingo-llm-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1235 2023-07-28 13:07:43.000000 lingo-llm-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.463147 lingo-llm-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-28 11:54:47.000000 lingo-llm-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-07-28 13:09:25.463147 lingo-llm-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.431506 lingo-llm-1.2.0/lingo/
+-rw-rw-rw-   0        0        0     4698 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/__init__.py
+-rw-rw-rw-   0        0        0      290 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/__main__.py
+-rw-rw-rw-   0        0        0    25947 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/argments.py
+-rw-rw-rw-   0        0        0     1648 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/dataset.py
+-rw-rw-rw-   0        0        0     3008 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/deepspeed_file.py
+-rw-rw-rw-   0        0        0     7983 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/inference.py
+-rw-rw-rw-   0        0        0     2999 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/initialize.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.433012 lingo-llm-1.2.0/lingo/kernels/
+-rw-rw-rw-   0        0        0     3092 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/kernels/__init__.py
+-rw-rw-rw-   0        0        0    30080 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/lomo.py
+-rw-rw-rw-   0        0        0    13985 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/lora.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.445432 lingo-llm-1.2.0/lingo/models/
+-rw-rw-rw-   0        0        0    17109 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/GLM130B_model.py
+-rw-rw-rw-   0        0        0     5831 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/GPT2_model.py
+-rw-rw-rw-   0        0        0     6814 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/GPTNeo_model.py
+-rw-rw-rw-   0        0        0    10234 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/LLAMA_model.py
+-rw-rw-rw-   0        0        0     8290 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/LLAMAv2_model.py
+-rw-rw-rw-   0        0        0    17780 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/__init__.py
+-rw-rw-rw-   0        0        0    17431 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/basemodel.py
+-rw-rw-rw-   0        0        0    16024 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/model_io.py
+-rw-rw-rw-   0        0        0    31589 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/models/transformers_model.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.450719 lingo-llm-1.2.0/lingo/quantization/
+-rw-rw-rw-   0        0        0     5522 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/quantization/__init__.py
+-rw-rw-rw-   0        0        0     1321 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/quantization/functional.py
+-rw-rw-rw-   0        0        0     9662 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/quantization/layers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.454733 lingo-llm-1.2.0/lingo/scaled_rope/
+-rw-rw-rw-   0        0        0        0 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/scaled_rope/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/scaled_rope/configuration_llama.py
+-rw-rw-rw-   0        0        0    59267 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/scaled_rope/modelling_llama.py
+-rw-rw-rw-   0        0        0      114 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/setting.py
+-rw-rw-rw-   0        0        0    28630 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/trainer.py
+-rw-rw-rw-   0        0        0    26409 2023-07-28 11:45:21.000000 lingo-llm-1.2.0/lingo/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:09:25.460492 lingo-llm-1.2.0/lingo_llm.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-28 13:09:25.000000 lingo-llm-1.2.0/lingo_llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2023-07-28 13:09:25.000000 lingo-llm-1.2.0/lingo_llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:09:25.000000 lingo-llm-1.2.0/lingo_llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-07-28 13:09:25.000000 lingo-llm-1.2.0/lingo_llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 13:09:25.000000 lingo-llm-1.2.0/lingo_llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:09:25.464237 lingo-llm-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2023-07-28 13:09:11.000000 lingo-llm-1.2.0/setup.py
```

### Comparing `lingo-llm-1.1.0/LICENSE` & `lingo-llm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/__init__.py` & `lingo-llm-1.2.0/lingo/__init__.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/argments.py` & `lingo-llm-1.2.0/lingo/argments.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/dataset.py` & `lingo-llm-1.2.0/lingo/dataset.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/deepspeed_file.py` & `lingo-llm-1.2.0/lingo/deepspeed_file.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/inference.py` & `lingo-llm-1.2.0/lingo/inference.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/initialize.py` & `lingo-llm-1.2.0/lingo/initialize.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/kernels/__init__.py` & `lingo-llm-1.2.0/lingo/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/lomo.py` & `lingo-llm-1.2.0/lingo/lomo.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/lora.py` & `lingo-llm-1.2.0/lingo/lora.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/GLM130B_model.py` & `lingo-llm-1.2.0/lingo/models/GLM130B_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/GPT2_model.py` & `lingo-llm-1.2.0/lingo/models/GPT2_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/GPTNeo_model.py` & `lingo-llm-1.2.0/lingo/models/GPTNeo_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/LLAMA_model.py` & `lingo-llm-1.2.0/lingo/models/LLAMA_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/LLAMAv2_model.py` & `lingo-llm-1.2.0/lingo/models/LLAMAv2_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/__init__.py` & `lingo-llm-1.2.0/lingo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/basemodel.py` & `lingo-llm-1.2.0/lingo/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/model_io.py` & `lingo-llm-1.2.0/lingo/models/model_io.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/models/transformers_model.py` & `lingo-llm-1.2.0/lingo/models/transformers_model.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/quantization/__init__.py` & `lingo-llm-1.2.0/lingo/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/quantization/functional.py` & `lingo-llm-1.2.0/lingo/quantization/functional.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/quantization/layers.py` & `lingo-llm-1.2.0/lingo/quantization/layers.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/scaled_rope/configuration_llama.py` & `lingo-llm-1.2.0/lingo/scaled_rope/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/scaled_rope/modelling_llama.py` & `lingo-llm-1.2.0/lingo/scaled_rope/modelling_llama.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/trainer.py` & `lingo-llm-1.2.0/lingo/trainer.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo/utils.py` & `lingo-llm-1.2.0/lingo/utils.py`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/lingo_llm.egg-info/SOURCES.txt` & `lingo-llm-1.2.0/lingo_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lingo-llm-1.1.0/setup.py` & `lingo-llm-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 """Install script."""
 
 import setuptools
 
 setuptools.setup(
     name="lingo-llm",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/WENGSYX/Lingo",
     author="Yixuan Weng",
     author_email="wengsyx@gmail.com",
     description="Lingo: Make the LLM Better for Everyone",
     packages=setuptools.find_packages(),
     install_requires=[
         "transformers>=4.30.2",
```

