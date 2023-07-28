# Comparing `tmp/grazier-0.0.5.tar.gz` & `tmp/grazier-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grazier-0.0.5.tar", last modified: Sun Jul  9 20:20:43 2023, max compression
+gzip compressed data, was "grazier-0.0.6.tar", last modified: Fri Jul 28 19:01:24 2023, max compression
```

## Comparing `grazier-0.0.5.tar` & `grazier-0.0.6.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.5/LICENSE
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10582 2023-07-09 20:20:43.581528 grazier-0.0.5/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8160 2023-07-03 19:47:02.000000 grazier-0.0.5/README.md
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      303 2023-06-27 18:28:08.000000 grazier-0.0.5/grazier/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1031 2023-07-03 19:52:15.000000 grazier-0.0.5/grazier/cli.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.5/grazier/engines/__init__.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/chat/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     5675 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3364 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/anthropic_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      828 2023-07-03 18:01:05.000000 grazier-0.0.5/grazier/engines/chat/anthropic_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    11368 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/bard_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      782 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/bard_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier/engines/chat/dolly/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4163 2023-07-03 18:18:59.000000 grazier-0.0.5/grazier/engines/chat/dolly/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1584 2023-07-03 18:01:37.000000 grazier-0.0.5/grazier/engines/chat/dolly/dolly_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     9237 2023-07-03 18:03:53.000000 grazier-0.0.5/grazier/engines/chat/dolly/instruct_pipeline.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    12590 2023-07-03 19:44:12.000000 grazier-0.0.5/grazier/engines/chat/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      817 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3025 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1013 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4967 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/stable_lm_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      823 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/stable_lm_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3501 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      814 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/chat/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/engines/llm/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3016 2023-07-03 19:54:15.000000 grazier-0.0.5/grazier/engines/llm/__init__.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2109 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/ai21_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      631 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/ai21_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1027 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/chat_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8363 2023-07-03 19:53:19.000000 grazier-0.0.5/grazier/engines/llm/huggingface_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      897 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/huggingface_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2610 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/llama_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      806 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/llama_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2164 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/openai_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      834 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/openai_engine_test.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2159 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/vertex_engine.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      571 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/engines/llm/vertex_engine_test.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/utils/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.5/grazier/utils/__init__.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.581528 grazier-0.0.5/grazier/utils/llama/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10917 2023-07-03 18:25:09.000000 grazier-0.0.5/grazier/utils/llama/convert_llama_weights_to_hf.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     7286 2023-07-03 18:26:09.000000 grazier-0.0.5/grazier/utils/llama/weight_diff.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2258 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/utils/python.py
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-07-03 17:52:47.000000 grazier-0.0.5/grazier/utils/pytorch.py
-drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-09 20:20:43.577528 grazier-0.0.5/grazier.egg-info/
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10582 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/PKG-INFO
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1570 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/SOURCES.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/dependency_links.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/entry_points.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      197 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/requires.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-07-09 20:20:43.000000 grazier-0.0.5/grazier.egg-info/top_level.txt
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2865 2023-07-09 20:20:22.000000 grazier-0.0.5/pyproject.toml
--rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-07-09 20:20:43.581528 grazier-0.0.5/setup.cfg
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1181 2023-06-26 20:44:22.000000 grazier-0.0.6/LICENSE
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10753 2023-07-28 19:01:24.328878 grazier-0.0.6/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     8331 2023-07-28 18:39:58.000000 grazier-0.0.6/README.md
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.324879 grazier-0.0.6/grazier/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1051 2023-07-17 16:13:54.000000 grazier-0.0.6/grazier/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2989 2023-07-14 23:03:06.000000 grazier-0.0.6/grazier/cli.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/engines/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:09:44.000000 grazier-0.0.6/grazier/engines/__init__.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/engines/chat/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     6055 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/chat/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3650 2023-07-14 18:04:02.000000 grazier-0.0.6/grazier/engines/chat/anthropic_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      840 2023-07-11 16:08:19.000000 grazier-0.0.6/grazier/engines/chat/anthropic_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1703 2023-07-28 18:41:29.000000 grazier-0.0.6/grazier/engines/chat/bard_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      782 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/chat/bard_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/engines/chat/dolly/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     5045 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/chat/dolly/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1584 2023-07-03 18:01:37.000000 grazier-0.0.6/grazier/engines/chat/dolly/dolly_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     9237 2023-07-03 18:03:53.000000 grazier-0.0.6/grazier/engines/chat/dolly/instruct_pipeline.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    15860 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/chat/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      817 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/chat/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4289 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/chat/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1013 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/chat/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     5337 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/chat/stable_lm_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      823 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/chat/stable_lm_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4055 2023-07-14 18:02:47.000000 grazier-0.0.6/grazier/engines/chat/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      814 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/chat/vertex_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      792 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/default.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/engines/llm/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3414 2023-07-28 18:45:13.000000 grazier-0.0.6/grazier/engines/llm/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2201 2023-07-14 18:05:58.000000 grazier-0.0.6/grazier/engines/llm/ai21_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      631 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/llm/ai21_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1357 2023-07-14 18:07:23.000000 grazier-0.0.6/grazier/engines/llm/chat_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    15092 2023-07-28 18:47:50.000000 grazier-0.0.6/grazier/engines/llm/huggingface_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      951 2023-07-28 19:00:15.000000 grazier-0.0.6/grazier/engines/llm/huggingface_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     4267 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/llm/llama_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      806 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/llm/llama_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3437 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/engines/llm/openai_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      834 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/llm/openai_engine_test.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2692 2023-07-14 18:02:05.000000 grazier-0.0.6/grazier/engines/llm/vertex_engine.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      571 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/engines/llm/vertex_engine_test.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/utils/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        0 2023-06-26 19:11:27.000000 grazier-0.0.6/grazier/utils/__init__.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2291 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/utils/huggingface.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier/utils/llama/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10910 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/utils/llama/convert_llama_weights_to_hf.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     7286 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/utils/llama/weight_diff.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2549 2023-07-14 17:50:33.000000 grazier-0.0.6/grazier/utils/python.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1123 2023-07-03 17:52:47.000000 grazier-0.0.6/grazier/utils/pytorch.py
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     3806 2023-07-14 22:49:25.000000 grazier-0.0.6/grazier/utils/secrets.py
+drwxrwxr-x   0 davidchan  (1000) davidchan  (1000)        0 2023-07-28 19:01:24.328878 grazier-0.0.6/grazier.egg-info/
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)    10753 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/PKG-INFO
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     1651 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/SOURCES.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        1 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/dependency_links.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       45 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/entry_points.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)      254 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/requires.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)        8 2023-07-28 19:01:24.000000 grazier-0.0.6/grazier.egg-info/top_level.txt
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)     2985 2023-07-28 18:59:33.000000 grazier-0.0.6/pyproject.toml
+-rw-rw-r--   0 davidchan  (1000) davidchan  (1000)       38 2023-07-28 19:01:24.328878 grazier-0.0.6/setup.cfg
```

### Comparing `grazier-0.0.5/LICENSE` & `grazier-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/PKG-INFO` & `grazier-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,14 +42,15 @@
 
 From OpenAI:
 - GPT-4 (Base, 32K) (Chat and Completion Engines)
 - GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
+- Claude 2 (Base) (Chat and Completion Engines)
 - Claude (Base, 100K) (Chat and Completion Engines)
 - Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
@@ -58,14 +59,15 @@
 - GPT-J (6B) (Completion Engine)
 - Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
 - Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
 - MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
+- Llama 2 (7B, 13B, 70B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
 - Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
 - Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
@@ -91,40 +93,39 @@
 
 Each of the LLMs may need additional setup, which you can find in the engine setup section below.
 
 
 
 ## Usage
 
-For completion engines, you can use the `LLMEngine` class:
+For completion engines, it's as simple as:
 ```python
-from grazier import LLMEngine
+import grazier
 
-LLMEngine.list_models()
+grazier.list_models()
 ['gptj-6B', 'gpt2', 'gpt2-med', 'gpt2-lg', 'gpt2-xl', 'distilgpt2', 'gptneo-125M', 'gptneo-1.3B', 'gptneo-2.7B', 'stablelm-3B', 'stablelm-7B', 'opt-125M', 'opt-350M', 'opt-1.3b', 'opt-2.7b', 'opt-6.7b', 'opt-13b', 'opt-30b', 'opt-66b', 'llama-7B', 'llama-13B', 'llama-30B', 'llama-65B', 'gpt3-davinci3', 'gpt3-davinci2', 'gpt3-curie', 'gpt3-babbage', 'gpt3-ada', 'palm']
-gpt2 = LLMEngine.from_string("gpt2")
+gpt2 = grazier.get("gpt2")
 completion = gpt2("I enjoy walking with my cute dog, but sometimes he gets scared and")
 print(completion)
 ```
 
-For chat engines, you can use the `LLMChat` class:
+For chat engines, all you need to do is add the `chat` parameter:
 ```python
-from grazier import LLMChat, Conversation, Speaker
+from grazier import Conversation, Speaker, get, list_models
 
 conversation = Conversation()
 conversation.add_turn("You are a funny person.", speaker=Speaker.SYSTEM)
 conversation.add_turn("Hi, how are you?", speaker=Speaker.USER)
 conversation.add_turn("I am doing well, how about you?", speaker=Speaker.AI)
 conversation.add_turn("What are you planning to do today?", speaker=Speaker.USER)
 
-LLMChat.list_models()
+list_models(chat=True)
 ['claude', 'claude-100k', 'claude-instant', 'claude-instant-100k', 'bard', 'koala-7b', 'koala-13b-v1', 'koala-13b-v2', 'vicuna-7b', 'vicuna-13b', 'alpaca-13b', 'chat-gpt', 'gpt4', 'gpt4-32k', 'stablelm-3b', 'stablelm-7b', 'palm']
-gpt4 = LLMChat.from_string("gpt4")
+gpt4 = get("gpt4", chat=True)
 next_turn = gpt4(conversation)
-
 print(next_turn)
 ```
 
 
 ## Individual Engine Setup
 
 Each engine may require some specific details to be passed in. For example, OpenAI engines require an API key. These
@@ -170,19 +171,21 @@
 ```
 or on the command line:
 ```bash
 export GOOGLE_APPLICATION_CREDENTIALS=<path to your JSON file>
 ```
 
 ### Bard
-For the Bard engine, you will need to get your Bard SESSION_ID.  Get the value of this variable by first going to
-https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab, then "Cookies",
-then copy the value of the "__Secure-1PSID" cookie. You can then set the environment variable:
+For the Bard engine, you will need to get your Bard __Secure-1PSID and __Secure-1PSIDTS tokens.  Get the value of this
+variable by first going to https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab,
+then "Cookies", then copy the value of the "__Secure-1PSID" and "__Secure-1PSIDTS" cookies. You can then set the
+environment variables:
 ```bash
-GOOGLE_BARD_SESSION_ID=<your session id>
+BARD__Secure_1PSID=<your session id>
+BARD__Secure_1PSIDTS=<your session id timestamp>
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
```

### Comparing `grazier-0.0.5/README.md` & `grazier-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 From OpenAI:
 - GPT-4 (Base, 32K) (Chat and Completion Engines)
 - GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
+- Claude 2 (Base) (Chat and Completion Engines)
 - Claude (Base, 100K) (Chat and Completion Engines)
 - Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
@@ -22,14 +23,15 @@
 - GPT-J (6B) (Completion Engine)
 - Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
 - Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
 - MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
+- Llama 2 (7B, 13B, 70B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
 - Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
 - Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
@@ -55,40 +57,39 @@
 
 Each of the LLMs may need additional setup, which you can find in the engine setup section below.
 
 
 
 ## Usage
 
-For completion engines, you can use the `LLMEngine` class:
+For completion engines, it's as simple as:
 ```python
-from grazier import LLMEngine
+import grazier
 
-LLMEngine.list_models()
+grazier.list_models()
 ['gptj-6B', 'gpt2', 'gpt2-med', 'gpt2-lg', 'gpt2-xl', 'distilgpt2', 'gptneo-125M', 'gptneo-1.3B', 'gptneo-2.7B', 'stablelm-3B', 'stablelm-7B', 'opt-125M', 'opt-350M', 'opt-1.3b', 'opt-2.7b', 'opt-6.7b', 'opt-13b', 'opt-30b', 'opt-66b', 'llama-7B', 'llama-13B', 'llama-30B', 'llama-65B', 'gpt3-davinci3', 'gpt3-davinci2', 'gpt3-curie', 'gpt3-babbage', 'gpt3-ada', 'palm']
-gpt2 = LLMEngine.from_string("gpt2")
+gpt2 = grazier.get("gpt2")
 completion = gpt2("I enjoy walking with my cute dog, but sometimes he gets scared and")
 print(completion)
 ```
 
-For chat engines, you can use the `LLMChat` class:
+For chat engines, all you need to do is add the `chat` parameter:
 ```python
-from grazier import LLMChat, Conversation, Speaker
+from grazier import Conversation, Speaker, get, list_models
 
 conversation = Conversation()
 conversation.add_turn("You are a funny person.", speaker=Speaker.SYSTEM)
 conversation.add_turn("Hi, how are you?", speaker=Speaker.USER)
 conversation.add_turn("I am doing well, how about you?", speaker=Speaker.AI)
 conversation.add_turn("What are you planning to do today?", speaker=Speaker.USER)
 
-LLMChat.list_models()
+list_models(chat=True)
 ['claude', 'claude-100k', 'claude-instant', 'claude-instant-100k', 'bard', 'koala-7b', 'koala-13b-v1', 'koala-13b-v2', 'vicuna-7b', 'vicuna-13b', 'alpaca-13b', 'chat-gpt', 'gpt4', 'gpt4-32k', 'stablelm-3b', 'stablelm-7b', 'palm']
-gpt4 = LLMChat.from_string("gpt4")
+gpt4 = get("gpt4", chat=True)
 next_turn = gpt4(conversation)
-
 print(next_turn)
 ```
 
 
 ## Individual Engine Setup
 
 Each engine may require some specific details to be passed in. For example, OpenAI engines require an API key. These
@@ -134,19 +135,21 @@
 ```
 or on the command line:
 ```bash
 export GOOGLE_APPLICATION_CREDENTIALS=<path to your JSON file>
 ```
 
 ### Bard
-For the Bard engine, you will need to get your Bard SESSION_ID.  Get the value of this variable by first going to
-https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab, then "Cookies",
-then copy the value of the "__Secure-1PSID" cookie. You can then set the environment variable:
+For the Bard engine, you will need to get your Bard __Secure-1PSID and __Secure-1PSIDTS tokens.  Get the value of this
+variable by first going to https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab,
+then "Cookies", then copy the value of the "__Secure-1PSID" and "__Secure-1PSIDTS" cookies. You can then set the
+environment variables:
 ```bash
-GOOGLE_BARD_SESSION_ID=<your session id>
+BARD__Secure_1PSID=<your session id>
+BARD__Secure_1PSIDTS=<your session id timestamp>
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
```

### Comparing `grazier-0.0.5/grazier/engines/chat/__init__.py` & `grazier-0.0.6/grazier/engines/chat/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
+from grazier.engines.default import Engine
 from grazier.engines.llm import register_chat_engine
 from grazier.utils.pytorch import select_device
 
 
 class Speaker(Enum):
     USER = "user"
     AI = "ai"
@@ -71,21 +72,15 @@
             self.turns.append(other)
         else:
             assert isinstance(other, Conversation)
             self.turns.extend(other.turns)
         return self
 
 
-class LLMChat(ABC):
-    @property
-    @abstractmethod
-    def name(self) -> Tuple[str, str]:
-        """Returns a tuple of (Pretty Name, CLI name) of the language model."""
-        raise NotImplementedError()
-
+class LLMChat(Engine):
     def __init__(self, device: Optional[str] = None) -> None:
         self.device = select_device(device)
 
     def __call__(
         self, prompt: Union[Conversation, ConversationTurn, str], n_completions: int = 1, **kwargs: Any
     ) -> List[ConversationTurn]:
         conversation = None
@@ -106,25 +101,34 @@
         raise NotImplementedError()
 
     def __repr__(
         self,
     ) -> str:
         return f"{self.__class__.__name__}({self.name[0]})"
 
-    @classmethod
-    def configure(cls, *args, **kwargs):
-        raise NotImplementedError("This engine does not support automated configuration.")
-
     @staticmethod
     def from_string(typestr: str, **kwargs: Any) -> "LLMChat":
         typestr = typestr.lower()
         if typestr in LM_CHAT_ENGINES:
-            return LM_CHAT_ENGINES[typestr](**kwargs)  # type: ignore
+            if not LM_CHAT_ENGINES[typestr].is_configured() and LM_CHAT_ENGINES[typestr].requires_configuration():
+                raise ValueError(
+                    f"Language model type: {typestr} requires configuration. Please run `grazier configure {typestr}` first."
+                )
+            else:
+                return LM_CHAT_ENGINES[typestr](**kwargs)  # type: ignore
         elif typestr in LM_CHAT_ENGINES_CLI:
-            return LM_CHAT_ENGINES_CLI[typestr](**kwargs)  # type: ignore
+            if (
+                not LM_CHAT_ENGINES_CLI[typestr].is_configured()
+                and LM_CHAT_ENGINES_CLI[typestr].requires_configuration()
+            ):
+                raise ValueError(
+                    f"Language model type: {typestr} requires configuration. Please run `grazier configure {typestr}` first."
+                )
+            else:
+                return LM_CHAT_ENGINES_CLI[typestr](**kwargs)  # type: ignore
 
         raise ValueError(f"Invalid language model type: {typestr}. Valid types are: {list(LM_CHAT_ENGINES_CLI.keys())}")
 
     @staticmethod
     def list_models() -> List[str]:
         return list(LM_CHAT_ENGINES_CLI.keys())
```

### Comparing `grazier-0.0.5/grazier/engines/chat/anthropic_engine.py` & `grazier-0.0.6/grazier/engines/chat/anthropic_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,18 @@
         samples = []
         for _ in range(n_completions):
             resp = self._completion(prompt, temperature=temperature)
             samples.append(resp["completion"])
 
         return [ConversationTurn(text=s.strip(), speaker=Speaker.AI) for s in samples]
 
+    @staticmethod
+    def is_configured() -> bool:
+        return os.getenv("ANTHROPIC_API_KEY", None) is not None
+
 
 @register_engine
 @singleton
 class Claude(AnthropicLMEngine):
     name = ("Claude", "claude")
 
     def __init__(self) -> None:
@@ -93,7 +97,16 @@
 @register_engine
 @singleton
 class ClaudeInstant100K(AnthropicLMEngine):
     name = ("Claude Instant 100K", "claude-instant-100k")
 
     def __init__(self) -> None:
         super().__init__("claude-instant-1-100k")
+
+
+@register_engine
+@singleton
+class Claude2(AnthropicLMEngine):
+    name = ("Claude 2", "claude-2")
+
+    def __init__(self) -> None:
+        super().__init__("claude-2")
```

### Comparing `grazier-0.0.5/grazier/engines/chat/anthropic_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/bard_engine_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["claude-instant"])
-def test_anthropic_chat_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["bard"])
+def test_bard_llm_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
-    conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
-    conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
+    conversation.add_turn(
+        "You are an intelligent AI named Jason. Your name, followed by a colon with the number 42 is:",
+        speaker=Speaker.USER,
+    )
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
         assert r.text.strip() != ""
         if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.5/grazier/engines/chat/bard_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/anthropic_engine_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import logging
 
 import pytest
 
 from grazier.engines.chat import Conversation, LLMChat, Speaker
 
 
-@pytest.mark.parametrize("engine", ["bard"])
-def test_bard_llm_engine(engine: str) -> None:
+@pytest.mark.parametrize("engine", ["claude-instant", "claude-2"])
+def test_anthropic_chat_engine(engine: str) -> None:
     # Construct a conversation
     conversation = Conversation()
-    conversation.add_turn(
-        "You are an intelligent AI named Jason. Your name, followed by a colon with the number 42 is:",
-        speaker=Speaker.USER,
-    )
+    conversation.add_turn("You are an intelligent AI named Jason.", speaker=Speaker.SYSTEM)
+    conversation.add_turn("Your name, followed by a colon with the number 42 is:", speaker=Speaker.USER)
 
     _engine = LLMChat.from_string(engine)
     responses = _engine(conversation)
     for r in responses:
         assert r.text.strip() != ""
         if "Jason" not in r.text:
             logging.warning(f'Name "Jason" not found in response "{r.text}"')
```

### Comparing `grazier-0.0.5/grazier/engines/chat/dolly/__init__.py` & `grazier-0.0.6/grazier/engines/chat/dolly/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Any, List, Optional
 
 from transformers import AutoModelForCausalLM, AutoTokenizer, TFAutoModelForCausalLM
 from transformers.pipelines import PIPELINE_REGISTRY, pipeline
 
 from grazier.engines.chat import Conversation, ConversationTurn, LLMChat, Speaker, register_engine
+from grazier.utils.huggingface import check_huggingface_model_files_are_local
 from grazier.utils.python import singleton
 
 from .instruct_pipeline import InstructionTextGenerationPipeline
 
 PIPELINE_REGISTRY.register_pipeline(
     task="dolly-instruct",
     pipeline_class=InstructionTextGenerationPipeline,
@@ -72,66 +73,90 @@
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="databricks/dolly-v2-3b",
             device=device,
         )
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("databricks/dolly-v2-3b")
+
 
 @register_engine
 @singleton
 class DollyV27B(DollyEngine):
     name = ("Dolly v2 7B", "dolly-v2-7b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="databricks/dolly-v2-7b",
             device=device,
         )
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("databricks/dolly-v2-7b")
+
 
 @register_engine
 @singleton
 class DollyV212B(DollyEngine):
     name = ("Dolly v2 12B", "dolly-v2-12b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="databricks/dolly-v2-12b",
             device=device,
         )
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("databricks/dolly-v2-12b")
+
 
 @register_engine
 @singleton
 class DollyV16B(DollyEngine):
     name = ("Dolly v1 6B", "dolly-v1-6b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="databricks/dolly-v1-6b",
             device=device,
         )
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("databricks/dolly-v1-6b")
+
 
 @register_engine
 @singleton
 class MPT7BInstruct(DollyEngine):
     name = ("MPT 7B Instruct", "mpt-7b-instruct")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="mosaicml/mpt-7b-instruct",
             device=device,
         )
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("mosaicml/mpt-7b-instruct")
+
 
 @register_engine
 @singleton
 class MPT30BInstruct(DollyEngine):
     name = ("MPT 30B Instruct", "mpt-30b-instruct")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__(
             model="mosaicml/mpt-30b-instruct",
             device=device,
         )
+
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("mosaicml/mpt-30b-instruct")
```

### Comparing `grazier-0.0.5/grazier/engines/chat/dolly/dolly_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/dolly/dolly_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/chat/dolly/instruct_pipeline.py` & `grazier-0.0.6/grazier/engines/chat/dolly/instruct_pipeline.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/chat/llama_engine.py` & `grazier-0.0.6/grazier/engines/chat/llama_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import logging
 import os
 from typing import Any, List, Optional, Tuple
 
 from transformers import LlamaForCausalLM, LlamaTokenizer
 
 from grazier.engines.chat import Conversation, ConversationTurn, LLMChat, Speaker, register_engine
@@ -59,14 +60,44 @@
         # outputs = self._extract_last_turn(outputs_filtered, last_prompt_is_user)
 
         return [
             ConversationTurn(text=o, speaker=Speaker.AI if last_prompt_is_user else Speaker.USER)
             for o in outputs_filtered
         ]
 
+    @staticmethod
+    def _is_configured(weight_root: Optional[str], model: str) -> bool:
+        # Check to see if the weights are available in the weight_root
+        if weight_root is None:
+            return False
+        if not os.path.exists(os.path.join(weight_root, model)):
+            return False
+
+        # Check to see if the files are available:
+        files = [
+            "config.json",
+            "pytorch_model.bin.index.json",
+            "tokenizer_config.json",
+            "generation_config.json",
+            "special_tokens_map.json",
+            "tokenizer.model",
+        ]
+
+        # Check to see if at least one model shard is available
+        # pytorch_model-{n_layers + 1}-of-{n_layers + 1}.bin
+        shards = list(glob.glob(os.path.join(weight_root, model, "pytorch_model-*.bin")))
+        if len(shards) == 0:
+            return False
+
+        for file in files:
+            if not os.path.exists(os.path.join(weight_root, model, file)):
+                return False
+
+        return True
+
 
 class KoalaLMEngine(LlamaLMEngine):
     def _build_prompt_from_conversation(self, conversation: Conversation) -> Tuple[str, bool]:
         # Step 1: Build the prompt from the conversation
         prompt = "BEGINNING OF CONVERSATION: "
         for turn in conversation.turns:
             if turn.speaker in (Speaker.USER, Speaker.SYSTEM):
@@ -216,123 +247,179 @@
 @singleton
 class Koala7B(KoalaLMEngine):
     name = ("Koala (7B)", "koala-7B")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("koala_7B", "KOALA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("KOALA_WEIGHTS_ROOT", None), "koala_7B")
+
 
 @register_engine
 @singleton
 class Koala13BV1(KoalaLMEngine):
     name = ("Koala (13B, v1)", "koala-13B-v1")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("koala_13B_v1", "KOALA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("KOALA_WEIGHTS_ROOT", None), "koala_13B_v1")
+
 
 @register_engine
 @singleton
 class Koala13BV2(KoalaLMEngine):
     name = ("Koala (13B, v2)", "koala-13B-v2")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("koala_13B_v2", "KOALA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("KOALA_WEIGHTS_ROOT", None), "koala_13B_v2")
+
 
 @register_engine
 @singleton
 class Vicuna7B(Vicuna11LMEngine):
     name = ("Vicuna (7B)", "vicuna-7B")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("vicuna_7B", "VICUNA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("VICUNA_WEIGHTS_ROOT", None), "vicuna_7B")
+
 
 @register_engine
 @singleton
 class Vicuna13B(Vicuna11LMEngine):
     name = ("Vicuna (13B)", "vicuna-13B")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("vicuna_13B", "VICUNA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("VICUNA_WEIGHTS_ROOT", None), "vicuna_13B")
+
 
 @register_engine
 @singleton
 class Alpaca13B(AlpacaLMEngine):
     name = ("Alpaca (13B)", "alpaca-13B")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("alpaca_13B", "ALPACA_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALPACA_WEIGHTS_ROOT", None), "alpaca_13B")
+
 
 @register_engine
 @singleton
 class Tulu7B(AllenAILlamaLMEngine):
     name = ("Tulu (7B)", "tulu-7b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("tulu-7b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "tulu-7b")
+
 
 @register_engine
 @singleton
 class Tulu13B(AllenAILlamaLMEngine):
     name = ("Tulu (13B)", "tulu-13b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("tulu-13b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "tulu-13b")
+
 
 @register_engine
 @singleton
 class Tulu30B(AllenAILlamaLMEngine):
     name = ("Tulu (30B)", "tulu-30b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("tulu-30b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "tulu-30b")
+
 
 @register_engine
 @singleton
 class Tulu65B(AllenAILlamaLMEngine):
     name = ("Tulu (65B)", "tulu-65b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("tulu-65b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "tulu-65b")
+
 
 @register_engine
 @singleton
 class OIShareGPT7B(AllenAILlamaLMEngine):
     name = ("Open Instruct ShareGPT (7B)", "open-instruct-sharegpt-7b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("open-instruct-sharegpt-7b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "open-instruct-sharegpt-7b")
+
 
 @register_engine
 @singleton
 class OIShareGPT13B(AllenAILlamaLMEngine):
     name = ("Open Instruct ShareGPT (13B)", "open-instruct-sharegpt-13b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("open-instruct-sharegpt-13b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "open-instruct-sharegpt-13b")
+
 
 @register_engine
 @singleton
 class OIShareGPT30B(AllenAILlamaLMEngine):
     name = ("Open Instruct ShareGPT (30B)", "open-instruct-sharegpt-30b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("open-instruct-sharegpt-30b", "ALLENAI_WEIGHTS_ROOT", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "open-instruct-sharegpt-30b")
+
 
 @register_engine
 @singleton
 class OIShareGPT65B(AllenAILlamaLMEngine):
     name = ("Open Instruct ShareGPT (65B)", "open-instruct-sharegpt-65b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("open-instruct-sharegpt-65b", "ALLENAI_WEIGHTS_ROOT", device=device)
+
+    @staticmethod
+    def is_configured() -> bool:
+        return LlamaLMEngine._is_configured(os.environ.get("ALLENAI_WEIGHTS_ROOT", None), "open-instruct-sharegpt-65b")
```

### Comparing `grazier-0.0.5/grazier/engines/chat/llama_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/llama_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/chat/openai_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/openai_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/chat/stable_lm_engine.py` & `grazier-0.0.6/grazier/engines/chat/stable_lm_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Any, List, Optional
 
 import torch
 from transformers import AutoModelForCausalLM, AutoTokenizer, StoppingCriteria, StoppingCriteriaList
 
 from grazier.engines.chat import Conversation, ConversationTurn, LLMChat, Speaker, register_engine
+from grazier.utils.huggingface import check_huggingface_model_files_are_local
 from grazier.utils.python import singleton
 from grazier.utils.pytorch import select_device
 
 
 class StopOnTokens(StoppingCriteria):
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs: Any) -> bool:
         stop_ids = [50278, 50279, 50277, 1, 0]
@@ -111,15 +112,23 @@
 @singleton
 class StableLM3B(StableLMChatEngine):
     name = ("Stable LM (3B)", "stablelm-3b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("stabilityai/stablelm-tuned-alpha-3b", device=device)
 
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("stabilityai/stablelm-tuned-alpha-3b")
+
 
 @register_engine
 @singleton
 class StableLM7B(StableLMChatEngine):
     name = ("Stable LM (7B)", "stablelm-7b")
 
     def __init__(self, device: Optional[str] = None) -> None:
         super().__init__("stabilityai/stablelm-tuned-alpha-7b", device=device)
+
+    @staticmethod
+    def is_configured() -> bool:
+        return check_huggingface_model_files_are_local("stabilityai/stablelm-tuned-alpha-7b")
```

### Comparing `grazier-0.0.5/grazier/engines/chat/stable_lm_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/stable_lm_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/chat/vertex_engine.py` & `grazier-0.0.6/grazier/engines/chat/vertex_engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,14 +74,33 @@
             ConversationTurn(
                 self._rate_limited_model_predict((context, examples, non_system_turns[-1].text), **kwargs),
                 speaker=Speaker.AI,
             )  # type: ignore
             for _ in range(n_completions)
         ]
 
+    @staticmethod
+    def is_configured() -> bool:
+        # Check to see if the Vertex AI SDK is installed, and if so, if the user has configured their credentials.
+        if ChatModel is None or InputOutputTextPair is None:
+            return False
+
+        # Check to see if the user has configured their google cloud credentials.
+        try:
+            from google.auth import default
+        except ImportError:
+            return False
+
+        try:
+            default()
+        except Exception:
+            return False
+
+        return True
+
 
 @register_engine
 @singleton
 class PaLMEngine(VertexLLMEngine):
     name = ("PaLM", "palm")
 
     def __init__(self) -> None:
```

### Comparing `grazier-0.0.5/grazier/engines/chat/vertex_engine_test.py` & `grazier-0.0.6/grazier/engines/chat/vertex_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/llm/__init__.py` & `grazier-0.0.6/grazier/engines/llm/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import logging
-from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar
+from abc import abstractmethod
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
 from huggingface_hub import HfApi, ModelFilter
 
+from grazier.engines.default import Engine
 from grazier.utils.pytorch import select_device
 
 
-class LLMEngine(ABC):
-    @property
-    @abstractmethod
-    def name(self) -> Tuple[str, str]:
-        """Returns a tuple of (Pretty Name, CLI name) of the language model."""
-        raise NotImplementedError()
-
+class LLMEngine(Engine):
     def __init__(self, device: Optional[str] = None) -> None:
         self.device = select_device(device)
+        self.device_specified = device is not None
 
     @property
     def prompt_prefix(self) -> str:
         return ""
 
     @property
     def prompt_suffix(self) -> str:
@@ -34,24 +30,32 @@
         raise NotImplementedError()
 
     def __repr__(
         self,
     ) -> str:
         return f"{self.__class__.__name__}({self.name[0]})"
 
-    @classmethod
-    def configure(cls, *args, **kwargs):
-        raise NotImplementedError("This engine does not support automated configuration.")
-
     @staticmethod
     def from_string(typestr: str, **kwargs: Any) -> "LLMEngine":
+        typestr = typestr.lower()
+
         if typestr in LM_ENGINES:
-            return LM_ENGINES[typestr](**kwargs)  # type: ignore
+            if not LM_ENGINES[typestr].is_configured() and LM_ENGINES[typestr].requires_configuration():
+                raise ValueError(
+                    f"Language model type: {typestr} requires configuration. Please run `grazier configure {typestr}` first."
+                )
+            else:
+                return LM_ENGINES[typestr](**kwargs)  # type: ignore
         elif typestr in LM_ENGINES_CLI:
-            return LM_ENGINES_CLI[typestr](**kwargs)  # type: ignore
+            if not LM_ENGINES_CLI[typestr].is_configured() and LM_ENGINES_CLI[typestr].requires_configuration():
+                raise ValueError(
+                    f"Language model type: {typestr} requires configuration. Please run `grazier configure {typestr}` first."
+                )
+            else:
+                return LM_ENGINES_CLI[typestr](**kwargs)  # type: ignore
 
         logging.info(f"Failed to find local LLM matching {typestr}. Fetching remote LLMs...")
         api = HfApi()
         models = list(api.list_models(filter=ModelFilter(model_name=typestr, task="text-generation")))
         if len(models) > 0:
             return HuggingFaceTextGenerationLMEngine.from_hub_model(typestr)(**kwargs)
```

### Comparing `grazier-0.0.5/grazier/engines/llm/ai21_engine.py` & `grazier-0.0.6/grazier/engines/llm/ai21_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,18 @@
             "stopSequences": ["##"],
         }
 
         response = ai21.Completion.execute(model=self._model, prompt=prompt, **(_default_params | kwargs))
 
         return [c["data"]["text"] for c in response["completions"]]
 
+    @staticmethod
+    def is_configured() -> bool:
+        return ai21.api_key is not None
+
 
 @register_engine
 @singleton
 class J2Light(AI21CompletionLLMEngine):
     name = ("J2 (Light)", "j2-light")
 
     def __init__(self) -> None:
```

### Comparing `grazier-0.0.5/grazier/engines/llm/ai21_engine_test.py` & `grazier-0.0.6/grazier/engines/llm/ai21_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/llm/chat_engine.py` & `grazier-0.0.6/grazier/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-from typing import Any, List, Type
+# isort: skip_file
 
-from grazier.engines.chat import Conversation, Speaker
-from grazier.engines.llm import LLMEngine
-
-
-def wrap_chat_llm_engine(cls) -> Type[LLMEngine]:  # type: ignore
-    """
-    Wrap an LLMChat engine to make it compatible with the LLMEngine interface.
-
-    Args:
-        cls (Type[LLMChat]): The LLMChat engine to wrap.
-
-    Returns:
-        Type[LLMEngine]: The wrapped LLMEngine.
-    """
-
-    class _WrappedEngine(LLMEngine):
-        name = (f"{cls.name[0]} (Chat)", f"{cls.name[1]}")
-
-        def __init__(self, **kwargs: Any) -> None:
-            super().__init__(device="defer")
-            self._engine = cls(**kwargs)
-
-        def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
-            # Build a conversation
-            conversation = Conversation()
-            conversation.add_turn(prompt, speaker=Speaker.USER)
-            return [x.text for x in self._engine.call(conversation, n_completions=n_completions, **kwargs)]
-
-    return _WrappedEngine
+from dotenv import load_dotenv
+from typing import Union, List
+import logging
+
+from rich.logging import RichHandler
+
+__version__ = "0.0.2"
+load_dotenv()
+
+# Configure logging
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(message)s",
+    datefmt="[%X]",
+    handlers=[RichHandler(rich_tracebacks=True)],
+)
+
+# Ignore import sorting, since LLMEngine needs to be imported first
+from grazier.engines.llm import LLMEngine  # noqa: E402
+from grazier.engines.chat import Conversation, LLMChat, Speaker, ConversationTurn  # noqa: F401, E402
+
+
+def get(name: str, chat: bool = False) -> Union[LLMChat, LLMEngine]:
+    """Get an engine by name."""
+    if chat:
+        if name in LLMChat.list_models():
+            return LLMChat.from_string(name)
+        else:
+            raise ValueError(f"Chat engine {name} not found")
+
+    return LLMEngine.from_string(name)
+
+
+def list_models(chat: bool = False) -> List[str]:
+    """List available LLMs."""
+    if chat:
+        return LLMChat.list_models()
+    return LLMEngine.list_models()
```

### Comparing `grazier-0.0.5/grazier/engines/llm/llama_engine_test.py` & `grazier-0.0.6/grazier/engines/llm/llama_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/llm/openai_engine.py` & `grazier-0.0.6/grazier/engines/llm/openai_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-import os
+import logging
 from abc import abstractmethod
 from typing import Any, List
 
 import openai
+from rich.prompt import Prompt
 
 from grazier.engines.llm import LLMEngine, register_engine
 from grazier.utils.python import retry, singleton
+from grazier.utils.secrets import get_secret, set_secret
 
-# Setup openai api keys
-openai.organization = os.getenv("OPENAI_API_ORG", None)
-openai.api_key = os.getenv("OPENAI_API_KEY", None)
+
+def _setup_api_keys():
+    # Setup openai api keys
+    openai.api_key = get_secret("OPENAI_API_KEY", None)
+    openai.organization = get_secret("OPENAI_API_ORG", None)
 
 
 @singleton
 class OpenAI:
     USAGE = 0.0
 
 
@@ -21,22 +25,50 @@
     @property
     @abstractmethod
     def cost_per_token(self) -> float:
         raise NotImplementedError()
 
     def __init__(self, model: str):
         self._model = model
+
+        _setup_api_keys()
+
         super().__init__(device="api")
 
     @retry(no_retry_on=(openai.error.AuthenticationError,))
     def call(self, prompt: str, n_completions: int = 1, **kwargs: Any) -> List[str]:
         cp = openai.Completion.create(model=self._model, prompt=prompt, n=n_completions, **kwargs)  # type: ignore
         OpenAI.USAGE += int(cp.usage.total_tokens) * self.cost_per_token
         return [i.text for i in cp.choices]  # type: ignore
 
+    @staticmethod
+    def is_configured() -> bool:
+        _setup_api_keys()
+        return openai.api_key is not None
+
+    @staticmethod
+    def configure():
+        if OpenAICompletionLLMEngine.is_configured():
+            reconfigure = Prompt.ask("OpenAI API key is already configured. Reconfigure?", choices=["y", "n"])
+            if reconfigure == "n":
+                logging.info("OpenAI API key already configured.")
+                return
+
+        have_openai_key = Prompt.ask("Do you have an OpenAI API key?", choices=["y", "n"])
+        if have_openai_key == "n":
+            Prompt.ask(
+                "Please follow the instructions here [u cyan]https://www.howtogeek.com/885918/how-to-get-an-openai-api-key/[/u cyan] to obtain an API key.\nWhen you have the key, press enter to continue",
+            )
+
+        openai_key = Prompt.ask("Please enter your OpenAI API key (It will be saved to your platform's secrets store)")
+        set_secret("OPENAI_API_KEY", openai_key.strip())
+
+        # Save the openai api key to the secrets store
+        logging.info("OpenAI API successfully configured.")
+
 
 @register_engine
 @singleton
 class GPT3Davinci3(OpenAICompletionLLMEngine):
     cost_per_token = 0.02 / 1000
     name = ("GPT-3 Davinci", "gpt3-davinci3")
```

### Comparing `grazier-0.0.5/grazier/engines/llm/openai_engine_test.py` & `grazier-0.0.6/grazier/engines/llm/openai_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/engines/llm/vertex_engine.py` & `grazier-0.0.6/grazier/engines/llm/vertex_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,33 @@
                 "temperature": kwargs.pop("temperature", 1.0),
             }
             | kwargs
         )
 
         return [self._rate_limited_model_predict(prompt, **kwargs).text for _ in range(n_completions)]  # type: ignore
 
+    @staticmethod
+    def is_configured() -> bool:
+        # Check to see if the Vertex AI SDK is installed, and if so, if the user has configured their credentials.
+        if TextGenerationModel is None:
+            return False
+
+        # Check to see if the user has configured their google cloud credentials.
+        try:
+            from google.auth import default
+        except ImportError:
+            return False
+
+        try:
+            default()
+        except Exception:
+            return False
+
+        return True
+
 
 @register_engine
 @singleton
 class PaLMEngine(VertexLLMEngine):
     name = ("PaLM", "palm")
 
     def __init__(self) -> None:
```

### Comparing `grazier-0.0.5/grazier/engines/llm/vertex_engine_test.py` & `grazier-0.0.6/grazier/engines/llm/vertex_engine_test.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier/utils/llama/convert_llama_weights_to_hf.py` & `grazier-0.0.6/grazier/utils/llama/convert_llama_weights_to_hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 import json
 import math
 import os
 import shutil
 import warnings
 
 import torch
-
 from transformers import LlamaConfig, LlamaForCausalLM, LlamaTokenizer
 
-
 try:
     from transformers import LlamaTokenizerFast
 except ImportError as e:
     warnings.warn(e)
     warnings.warn(
         "The converted tokenizer will be the `slow` tokenizer. To use the fast, update your `tokenizers` library and re-run the tokenizer conversion"
     )
@@ -69,15 +67,15 @@
 
 
 def compute_intermediate_size(n):
     return int(math.ceil(n * 8 / 3) + 255) // 256 * 256
 
 
 def read_json(path):
-    with open(path, "r") as f:
+    with open(path) as f:
         return json.load(f)
 
 
 def write_json(text, path):
     with open(path, "w") as f:
         json.dump(text, f)
```

### Comparing `grazier-0.0.5/grazier/utils/llama/weight_diff.py` & `grazier-0.0.6/grazier/utils/llama/weight_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from typing import Optional, Dict
+from typing import Dict, Optional
 
 import fire
 import torch
 import tqdm
 import transformers
```

### Comparing `grazier-0.0.5/grazier/utils/python.py` & `grazier-0.0.6/grazier/utils/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,10 +68,16 @@
 
     def __call__(self, *args: Any, **kwargs: Any) -> T:
         """Returns a single instance of decorated class"""
         if self._instance is None:
             self._instance = self.__wrapped__(*args, **kwargs)
         return self._instance
 
+    # Pass class methods/attributes through to the wrapped class
+    def __getattr__(self, attr: str) -> Any:
+        if hasattr(self.__wrapped__, attr):
+            return getattr(self.__wrapped__, attr)
+        raise AttributeError(f"{self.__wrapped__.__name__} has no attribute {attr}")
+
 
 def singleton(cls: Type[S]) -> _SingletonWrapper[S]:
     return _SingletonWrapper(cls)
```

### Comparing `grazier-0.0.5/grazier/utils/pytorch.py` & `grazier-0.0.6/grazier/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `grazier-0.0.5/grazier.egg-info/PKG-INFO` & `grazier-0.0.6/grazier.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grazier
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for calling (and calling out to) large language models.
 Author-email: David Chan <davidchan@berkeley.edu>
 License: 
         Copyright 2023, Regents of the University of California
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,14 +42,15 @@
 
 From OpenAI:
 - GPT-4 (Base, 32K) (Chat and Completion Engines)
 - GPT-3.5 (ChatGPT) (Chat and Completion Engines)
 - GPT-3 (Davinci (v2,v3), Ada, Babbage, Curie) (Completion Engine)
 
 From Anthropic:
+- Claude 2 (Base) (Chat and Completion Engines)
 - Claude (Base, 100K) (Chat and Completion Engines)
 - Claude Instant (Base, 100K) (Chat and Completion Engines)
 
 From Google/GCP:
 - PaLM (Chat and Completion Engines)
 
 From Huggingface
@@ -58,14 +59,15 @@
 - GPT-J (6B) (Completion Engine)
 - Falcon (7B, 40B, rw-1B, rw-7B) (Completion Engine)
 - Dolly (v1 - 6B, v2 - 3B, 7B, 12B) (Chat and Completion Engines)
 - MPT (Instruct - 7B, 30B) (Chat and Completion Engines)
 
 From Facebook (via Huggingface)
 - Llama (7B, 13B, 30B, 65B) (Completion Engine)
+- Llama 2 (7B, 13B, 70B) (Completion Engine)
 - OPT (125M, 350M, 1.3B, 2.7B, 6.7B, 13B, 30B, 66B) (Completion Engine)
 
 From Stanford (via Huggingface)
 - Alpaca (7B) (Chat and Completion Engines)
 
 From Berkeley (via Huggingface)
 - Koala (7B, 13B_v1, 13B_v2) (Chat and Completion Engines)
@@ -91,40 +93,39 @@
 
 Each of the LLMs may need additional setup, which you can find in the engine setup section below.
 
 
 
 ## Usage
 
-For completion engines, you can use the `LLMEngine` class:
+For completion engines, it's as simple as:
 ```python
-from grazier import LLMEngine
+import grazier
 
-LLMEngine.list_models()
+grazier.list_models()
 ['gptj-6B', 'gpt2', 'gpt2-med', 'gpt2-lg', 'gpt2-xl', 'distilgpt2', 'gptneo-125M', 'gptneo-1.3B', 'gptneo-2.7B', 'stablelm-3B', 'stablelm-7B', 'opt-125M', 'opt-350M', 'opt-1.3b', 'opt-2.7b', 'opt-6.7b', 'opt-13b', 'opt-30b', 'opt-66b', 'llama-7B', 'llama-13B', 'llama-30B', 'llama-65B', 'gpt3-davinci3', 'gpt3-davinci2', 'gpt3-curie', 'gpt3-babbage', 'gpt3-ada', 'palm']
-gpt2 = LLMEngine.from_string("gpt2")
+gpt2 = grazier.get("gpt2")
 completion = gpt2("I enjoy walking with my cute dog, but sometimes he gets scared and")
 print(completion)
 ```
 
-For chat engines, you can use the `LLMChat` class:
+For chat engines, all you need to do is add the `chat` parameter:
 ```python
-from grazier import LLMChat, Conversation, Speaker
+from grazier import Conversation, Speaker, get, list_models
 
 conversation = Conversation()
 conversation.add_turn("You are a funny person.", speaker=Speaker.SYSTEM)
 conversation.add_turn("Hi, how are you?", speaker=Speaker.USER)
 conversation.add_turn("I am doing well, how about you?", speaker=Speaker.AI)
 conversation.add_turn("What are you planning to do today?", speaker=Speaker.USER)
 
-LLMChat.list_models()
+list_models(chat=True)
 ['claude', 'claude-100k', 'claude-instant', 'claude-instant-100k', 'bard', 'koala-7b', 'koala-13b-v1', 'koala-13b-v2', 'vicuna-7b', 'vicuna-13b', 'alpaca-13b', 'chat-gpt', 'gpt4', 'gpt4-32k', 'stablelm-3b', 'stablelm-7b', 'palm']
-gpt4 = LLMChat.from_string("gpt4")
+gpt4 = get("gpt4", chat=True)
 next_turn = gpt4(conversation)
-
 print(next_turn)
 ```
 
 
 ## Individual Engine Setup
 
 Each engine may require some specific details to be passed in. For example, OpenAI engines require an API key. These
@@ -170,19 +171,21 @@
 ```
 or on the command line:
 ```bash
 export GOOGLE_APPLICATION_CREDENTIALS=<path to your JSON file>
 ```
 
 ### Bard
-For the Bard engine, you will need to get your Bard SESSION_ID.  Get the value of this variable by first going to
-https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab, then "Cookies",
-then copy the value of the "__Secure-1PSID" cookie. You can then set the environment variable:
+For the Bard engine, you will need to get your Bard __Secure-1PSID and __Secure-1PSIDTS tokens.  Get the value of this
+variable by first going to https://bard.google.com/, then log in, press F12 for console, and go to the "Application" tab,
+then "Cookies", then copy the value of the "__Secure-1PSID" and "__Secure-1PSIDTS" cookies. You can then set the
+environment variables:
 ```bash
-GOOGLE_BARD_SESSION_ID=<your session id>
+BARD__Secure_1PSID=<your session id>
+BARD__Secure_1PSIDTS=<your session id timestamp>
 ```
 
 ### Huggingface Engines
 Most of the huggingface engines require no additional setup, however, some of the larger models require a GPU to run
 with any kind of efficiency (and some require multiple GPUs with large amounts of memory). You can find more details
 about the requirements for each model on the [Huggingface model hub](https://huggingface.co/models).
```

### Comparing `grazier-0.0.5/grazier.egg-info/SOURCES.txt` & `grazier-0.0.6/grazier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 grazier.egg-info/PKG-INFO
 grazier.egg-info/SOURCES.txt
 grazier.egg-info/dependency_links.txt
 grazier.egg-info/entry_points.txt
 grazier.egg-info/requires.txt
 grazier.egg-info/top_level.txt
 grazier/engines/__init__.py
+grazier/engines/default.py
 grazier/engines/chat/__init__.py
 grazier/engines/chat/anthropic_engine.py
 grazier/engines/chat/anthropic_engine_test.py
 grazier/engines/chat/bard_engine.py
 grazier/engines/chat/bard_engine_test.py
 grazier/engines/chat/llama_engine.py
 grazier/engines/chat/llama_engine_test.py
@@ -35,11 +36,13 @@
 grazier/engines/llm/llama_engine.py
 grazier/engines/llm/llama_engine_test.py
 grazier/engines/llm/openai_engine.py
 grazier/engines/llm/openai_engine_test.py
 grazier/engines/llm/vertex_engine.py
 grazier/engines/llm/vertex_engine_test.py
 grazier/utils/__init__.py
+grazier/utils/huggingface.py
 grazier/utils/python.py
 grazier/utils/pytorch.py
+grazier/utils/secrets.py
 grazier/utils/llama/convert_llama_weights_to_hf.py
 grazier/utils/llama/weight_diff.py
```

### Comparing `grazier-0.0.5/pyproject.toml` & `grazier-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 [project]
 name = 'grazier'
-version = '0.0.5'
+version = '0.0.6'
 description = 'A tool for calling (and calling out to) large language models.'
 authors = [
     {name='David Chan', email='davidchan@berkeley.edu'}
 ]
 dependencies=[
     # Base dependencies
     "click",
     "rich",
     "python-dotenv",
     "ratelimit",
     "fire", # For weight_diff.py. TODO: Remove this, replace with click
 
+    # For keyring support
+    "keyring",
+    "keyrings.cryptfile",
+
     # LM Engines
+    "requests",
     "openai",
     "anthropic",
     "google-cloud-aiplatform[pipelines]",
     "ai21",
+    "GoogleBard",
 
     # Local LM Engines
     "torch>=1.13.0",
     "transformers>=4.30.2",
+    "bitsandbytes",
     "sentencepiece",
     "accelerate",
     "einops",
-    "xformers"
+    "scipy",
 
 ]
 license = { file = "LICENSE" }
 requires-python=">=3.8.0"
 readme = "README.md"
 keywords = [
   "language-models",
```

