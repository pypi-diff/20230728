# Comparing `tmp/xinference-0.0.6.tar.gz` & `tmp/xinference-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.6.tar", last modified: Mon Jul 24 07:06:26 2023, max compression
+gzip compressed data, was "xinference-0.1.0.tar", last modified: Fri Jul 28 13:13:48 2023, max compression
```

## Comparing `xinference-0.0.6.tar` & `xinference-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-24 07:06:18.000000 xinference-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-24 07:06:18.000000 xinference-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-24 07:06:26.973025 xinference-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-24 07:06:18.000000 xinference-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 07:06:18.000000 xinference-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-24 07:06:26.973025 xinference-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-24 07:06:18.000000 xinference-0.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-24 07:06:18.000000 xinference-0.0.6/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20685 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/locale/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/llama2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/orca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.973025 xinference-0.0.6/xinference/model/llm/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/pytorch/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-24 07:06:18.000000 xinference-0.0.6/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:06:26.969025 xinference-0.0.6/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 07:06:26.000000 xinference-0.0.6/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 13:13:39.000000 xinference-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 13:13:39.000000 xinference-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-28 13:13:48.451522 xinference-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 13:13:39.000000 xinference-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-28 13:13:39.000000 xinference-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-28 13:13:48.455522 xinference-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-28 13:13:39.000000 xinference-0.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-28 13:13:39.000000 xinference-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.455522 xinference-0.1.0/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 13:13:48.455522 xinference-0.1.0/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/ggml/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/ggml/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/llm_family.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/llm_family.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference/model/llm/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/pytorch/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/model/llm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-28 13:13:39.000000 xinference-0.1.0/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:13:48.451522 xinference-0.1.0/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 13:13:48.000000 xinference-0.1.0/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.6/LICENSE` & `xinference-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/PKG-INFO` & `xinference-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.6
+Version: 0.1.0
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: ggml
+Provides-Extra: pytorch
 Provides-Extra: doc
 License-File: LICENSE
 
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
@@ -41,16 +43,14 @@
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-![demo](assets/demo.gif)
-
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
 
 ## Key Features
 🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
@@ -73,22 +73,43 @@
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
+
+### Installation
 ```bash
-$ pip install "xinference[all]"
+$ pip install "xinference"
+```
+`xinference` installs basic packages for serving models. 
+
+#### Installation with GGML
+To serve ggml models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[ggml]"
 ```
-`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
+If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
+#### Installation with PyTorch
+To serve PyTorch models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[pytorch]"
+```
+
+#### Installation with all dependencies
+If you want to serve all the supported models, install all the dependencies:
+```bash
+$ pip install "xinference[all]"
+```
+
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
 #### Local
 To start a local instance of Xinference, run the following command:
 ```bash
@@ -118,15 +139,15 @@
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
 You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
-![web UI](assets/xinference-downloading.png)
+![web UI](assets/demo.gif)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
 commands:
 
 - Launch a model (a model UID will be returned): `xinference launch`
 - List running models: `xinference list`
@@ -182,37 +203,81 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
+### ggmlv3 models
+
 | Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
 |---------------|------------------|----------|---------|--------------------|-----------------------------------------|
 | llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
-| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13, 70          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
+### pytorch models
+
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization             |
+|---------------|------------------|----------|---------|--------------------|--------------------------|
+| baichuan      | Foundation Model | en, zh   | pytorch | 7, 13              | '4-bit', '8-bit', 'none' |
+| baichuan-chat | SFT Model        | en, zh   | pytorch | 13                 | '4-bit', '8-bit', 'none' |
+| vicuna-v1.3   | SFT Model        | en       | pytorch | 7, 13, 33          | '4-bit', '8-bit', 'none' |
+
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
 - If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
+- `llama-2-chat` 70B ggmlv3 model only supports q4_0 quantization currently.
+
+
+## Pytorch Model Best Practices
+
+Pytorch has been integrated recently, and the usage scenarios are described below:
+
+### supported models
+- Foundation Model：baichuan（7B、13B）。
+- SFT Model：baichuan-chat（13B）、vicuna-v1.3（7B、13B、33B）。
+
+### supported devices
+- CUDA: On Linux and Windows systems, `cuda` device is used by default.
+- MPS: On Mac M1/M2 devices, `mps` device is used by default.
+- CPU: It is not recommended to use a `cpu` device, as it takes up a lot of memory and the inference speed is very slow.
+
+### quantization methods
+- `none`: indicates that no quantization is used.
+- `8-bit`: use 8-bit quantization.
+- `4-bit`: use 4-bit quantization. Note: 4-bit quantization is only supported on Linux systems and CUDA devices.
+
+### other instructions
+- On MacOS system, baichuan-chat model is not supported, and baichuan model cannot use 8-bit quantization.
+
+### use cases
+
+The table below shows memory usage and supported devices of some models.
+
+| Name          | Size (B) | OS    | No quantization (MB) | Quantization 8-bit (MB) | Quantization 4-bit (MB) |
+|---------------|----------|-------|----------------------|-------------------------|-------------------------|
+| baichuan-chat | 13       | linux | not currently tested | 13275                   | 7263                    |
+| baichuan-chat | 13       | macos | not supported        | not supported           | not supported           |
+| vicuna-v1.3   | 7        | linux | 12884                | 6708                    | 3620                    |
+| vicuna-v1.3   | 7        | macos | 12916                | 565                     | not supported           |
+| baichuan      | 7        | linux | 13480                | 7304                    | 4216                    |
+| baichuan      | 7        | macos | 13480                | not supported           | not supported           |
+
+
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
-### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
-within Xinference.
-
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.6 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.1.0 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
-Extra: doc License-File: LICENSE
+Extra: ggml Provides-Extra: pytorch Provides-Extra: doc License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
@@ -25,15 +25,15 @@
                (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
-full potential of cutting-edge AI models. ![demo](assets/demo.gif)
+full potential of cutting-edge AI models.
                         ð_Join_our_Slack_community!
 ## Key Features ð **Model Serving Made Easy**: Simplify the process of
 serving large language, speech recognition, and multimodal models. You can set
 up and deploy your models for experimentation and production with a single
 command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
 built-in models using a single command. Inference provides access to state-of-
 the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
@@ -45,82 +45,112 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
-installs all the necessary packages for serving models. If you want to achieve
+conflicts. ### Installation ```bash $ pip install "xinference" ``` `xinference`
+installs basic packages for serving models. #### Installation with GGML To
+serve ggml models, you need to install the following extra dependencies:
+```bash $ pip install "xinference[ggml]" ``` If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
-`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
-a single command or deploy it in a distributed cluster. #### Local To start a
-local instance of Xinference, run the following command: ```bash $ xinference
-``` #### Distributed To deploy Xinference in a cluster, you need to start a
-Xinference supervisor on one server and Xinference workers on the other
-servers. Follow the steps below: **Starting the Supervisor**: On the server
-where you want to run the Xinference supervisor, run the following command:
-```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+`chatglm` and `chatglm2`. #### Installation with PyTorch To serve PyTorch
+models, you need to install the following extra dependencies: ```bash $ pip
+install "xinference[pytorch]" ``` #### Installation with all dependencies If
+you want to serve all the supported models, install all the dependencies:
+```bash $ pip install "xinference[all]" ``` ### Deployment You can deploy
+Xinference locally with a single command or deploy it in a distributed cluster.
+#### Local To start a local instance of Xinference, run the following command:
+```bash $ xinference ``` #### Distributed To deploy Xinference in a cluster,
+you need to start a Xinference supervisor on one server and Xinference workers
+on the other servers. Follow the steps below: **Starting the Supervisor**: On
+the server where you want to run the Xinference supervisor, run the following
+command: ```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
 {supervisor_host}` with the actual host of your supervisor server. **Starting
 the Workers**: On each of the other servers where you want to run Xinference
 workers, run the following command: ```bash $ xinference-worker -e "http://$
 {supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
 accessible for model management via CLI or Xinference client. - For local
 deployment, the endpoint will be `http://localhost:9997`. - For cluster
 deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
 {supervisor_host}` is the hostname or IP address of the server where the
 supervisor is running. You can also view a web UI using the Xinference endpoint
 to chat with all the builtin models. You can even **chat with two cutting-edge
 AI models side-by-side to compare their performance**! ![web UI](assets/
-xinference-downloading.png) ### Xinference CLI Xinference provides a command
-line interface (CLI) for model management. Here are some useful commands: -
-Launch a model (a model UID will be returned): `xinference launch` - List
-running models: `xinference list` - List all the builtin models: `xinference
-list --all` - Terminate a model: `xinference terminate --model-uid $
-{model_uid}` ### Xinference Client Xinference also provides a client for
-managing and accessing models programmatically: ```python from
-xinference.client import Client client = Client("http://localhost:9997")
-model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
-(model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
-( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
-```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
-"56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
-1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
-"content": "The largest animal that has been scientifically measured is the
-blue whale, which has a maximum length of around 23 meters (75 feet) for adult
-animals and can weigh up to 150,000 pounds (68,000 kg). However, it is
-important to note that this is just an estimate and that the largest animal
-known to science may be larger still. Some scientists believe that the largest
-animals may not have a clear \"size\" in the same way that humans do, as their
-size can vary depending on the environment and the stage of their life." },
-"finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
-"completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
-for more examples. ## Builtin models To view the builtin models, run the
-following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | |---------------|---------------
----|----------|---------|--------------------|---------------------------------
---------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
-ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+demo.gif) ### Xinference CLI Xinference provides a command line interface (CLI)
+for model management. Here are some useful commands: - Launch a model (a model
+UID will be returned): `xinference launch` - List running models: `xinference
+list` - List all the builtin models: `xinference list --all` - Terminate a
+model: `xinference terminate --model-uid ${model_uid}` ### Xinference Client
+Xinference also provides a client for managing and accessing models
+programmatically: ```python from xinference.client import Client client =
+Client("http://localhost:9997") model_uid = client.launch_model
+(model_name="chatglm2") model = client.get_model(model_uid) chat_history = []
+prompt = "What is the largest animal?" model.chat( prompt, chat_history,
+generate_config={"max_tokens": 1024} ) ``` Result: ```json { "id": "chatcmpl-
+8d76b65a-bad0-42ef-912d-4a0533d90d61", "model": "56f69622-1e73-11ee-a3bd-
+9af9f16816c6", "object": "chat.completion", "created": 1688919187, "choices":
+[ { "index": 0, "message": { "role": "assistant", "content": "The largest
+animal that has been scientifically measured is the blue whale, which has a
+maximum length of around 23 meters (75 feet) for adult animals and can weigh up
+to 150,000 pounds (68,000 kg). However, it is important to note that this is
+just an estimate and that the largest animal known to science may be larger
+still. Some scientists believe that the largest animals may not have a clear
+\"size\" in the same way that humans do, as their size can vary depending on
+the environment and the stage of their life." }, "finish_reason": "None" } ],
+"usage": { "prompt_tokens": -1, "completion_tokens": -1, "total_tokens": -1 } }
+``` See [examples](examples) for more examples. ## Builtin models To view the
+builtin models, run the following command: ```bash $ xinference list --all ```
+### ggmlv3 models | Name | Type | Language | Format | Size (in billions) |
+Quantization | |---------------|------------------|----------|---------|-------
+-------------|-----------------------------------------| | llama-2 | Foundation
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
-'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
-'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
-ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
-Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
-SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-**NOTE**: - Xinference will download models automatically for you, and by
-default the models will be saved under `${USER}/.xinference/cache`. -
-Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
-acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
-Xinference is currently under active development. Here's a roadmap outlining
-our planned developments for the next few weeks: ### PyTorch Support With
-PyTorch integration, users will be able to seamlessly utilize PyTorch models
-from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
-With Xinference, it will be much easier for users to use these libraries and
-build applications with LLMs.
+baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | llama-2-chat | RLHF Model | en | ggmlv3 | 7, 13, 70 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh |
+ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model |
+en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0
+| SFT Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'
+| | wizardlm-v1.1 | SFT Model | en | ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 |
+'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | ### pytorch models | Name | Type |
+Language | Format | Size (in billions) | Quantization | |---------------|------
+------------|----------|---------|--------------------|------------------------
+--| | baichuan | Foundation Model | en, zh | pytorch | 7, 13 | '4-bit', '8-
+bit', 'none' | | baichuan-chat | SFT Model | en, zh | pytorch | 13 | '4-bit',
+'8-bit', 'none' | | vicuna-v1.3 | SFT Model | en | pytorch | 7, 13, 33 | '4-
+bit', '8-bit', 'none' | **NOTE**: - Xinference will download models
+automatically for you, and by default the models will be saved under `$
+{USER}/.xinference/cache`. - Foundation models only provide interface
+`generate`. - RLHF and SFT models provide both `generate` and `chat`. - If you
+want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1
+quantization methods. - `llama-2-chat` 70B ggmlv3 model only supports q4_0
+quantization currently. ## Pytorch Model Best Practices Pytorch has been
+integrated recently, and the usage scenarios are described below: ### supported
+models - Foundation Modelï¼baichuanï¼7Bã13Bï¼ã - SFT Modelï¼baichuan-
+chatï¼13Bï¼ãvicuna-v1.3ï¼7Bã13Bã33Bï¼ã ### supported devices -
+CUDA: On Linux and Windows systems, `cuda` device is used by default. - MPS: On
+Mac M1/M2 devices, `mps` device is used by default. - CPU: It is not
+recommended to use a `cpu` device, as it takes up a lot of memory and the
+inference speed is very slow. ### quantization methods - `none`: indicates that
+no quantization is used. - `8-bit`: use 8-bit quantization. - `4-bit`: use 4-
+bit quantization. Note: 4-bit quantization is only supported on Linux systems
+and CUDA devices. ### other instructions - On MacOS system, baichuan-chat model
+is not supported, and baichuan model cannot use 8-bit quantization. ### use
+cases The table below shows memory usage and supported devices of some models.
+| Name | Size (B) | OS | No quantization (MB) | Quantization 8-bit (MB) |
+Quantization 4-bit (MB) | |---------------|----------|-------|-----------------
+-----|-------------------------|-------------------------| | baichuan-chat | 13
+| linux | not currently tested | 13275 | 7263 | | baichuan-chat | 13 | macos |
+not supported | not supported | not supported | | vicuna-v1.3 | 7 | linux |
+12884 | 6708 | 3620 | | vicuna-v1.3 | 7 | macos | 12916 | 565 | not supported |
+| baichuan | 7 | linux | 13480 | 7304 | 4216 | | baichuan | 7 | macos | 13480 |
+not supported | not supported | ## Roadmap Xinference is currently under active
+development. Here's a roadmap outlining our planned developments for the next
+few weeks: ### Langchain & LlamaIndex integration With Xinference, it will be
+much easier for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.6/README.md` & `xinference-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-![demo](assets/demo.gif)
-
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
 
 ## Key Features
 🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
@@ -48,22 +46,43 @@
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
+
+### Installation
 ```bash
-$ pip install "xinference[all]"
+$ pip install "xinference"
+```
+`xinference` installs basic packages for serving models. 
+
+#### Installation with GGML
+To serve ggml models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[ggml]"
 ```
-`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
+If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
+#### Installation with PyTorch
+To serve PyTorch models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[pytorch]"
+```
+
+#### Installation with all dependencies
+If you want to serve all the supported models, install all the dependencies:
+```bash
+$ pip install "xinference[all]"
+```
+
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
 #### Local
 To start a local instance of Xinference, run the following command:
 ```bash
@@ -93,15 +112,15 @@
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
 You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
-![web UI](assets/xinference-downloading.png)
+![web UI](assets/demo.gif)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
 commands:
 
 - Launch a model (a model UID will be returned): `xinference launch`
 - List running models: `xinference list`
@@ -157,37 +176,81 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
+### ggmlv3 models
+
 | Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
 |---------------|------------------|----------|---------|--------------------|-----------------------------------------|
 | llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
-| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13, 70          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
+### pytorch models
+
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization             |
+|---------------|------------------|----------|---------|--------------------|--------------------------|
+| baichuan      | Foundation Model | en, zh   | pytorch | 7, 13              | '4-bit', '8-bit', 'none' |
+| baichuan-chat | SFT Model        | en, zh   | pytorch | 13                 | '4-bit', '8-bit', 'none' |
+| vicuna-v1.3   | SFT Model        | en       | pytorch | 7, 13, 33          | '4-bit', '8-bit', 'none' |
+
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
 - If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
+- `llama-2-chat` 70B ggmlv3 model only supports q4_0 quantization currently.
+
+
+## Pytorch Model Best Practices
+
+Pytorch has been integrated recently, and the usage scenarios are described below:
+
+### supported models
+- Foundation Model：baichuan（7B、13B）。
+- SFT Model：baichuan-chat（13B）、vicuna-v1.3（7B、13B、33B）。
+
+### supported devices
+- CUDA: On Linux and Windows systems, `cuda` device is used by default.
+- MPS: On Mac M1/M2 devices, `mps` device is used by default.
+- CPU: It is not recommended to use a `cpu` device, as it takes up a lot of memory and the inference speed is very slow.
+
+### quantization methods
+- `none`: indicates that no quantization is used.
+- `8-bit`: use 8-bit quantization.
+- `4-bit`: use 4-bit quantization. Note: 4-bit quantization is only supported on Linux systems and CUDA devices.
+
+### other instructions
+- On MacOS system, baichuan-chat model is not supported, and baichuan model cannot use 8-bit quantization.
+
+### use cases
+
+The table below shows memory usage and supported devices of some models.
+
+| Name          | Size (B) | OS    | No quantization (MB) | Quantization 8-bit (MB) | Quantization 4-bit (MB) |
+|---------------|----------|-------|----------------------|-------------------------|-------------------------|
+| baichuan-chat | 13       | linux | not currently tested | 13275                   | 7263                    |
+| baichuan-chat | 13       | macos | not supported        | not supported           | not supported           |
+| vicuna-v1.3   | 7        | linux | 12884                | 6708                    | 3620                    |
+| vicuna-v1.3   | 7        | macos | 12916                | 565                     | not supported           |
+| baichuan      | 7        | linux | 13480                | 7304                    | 4216                    |
+| baichuan      | 7        | macos | 13480                | not supported           | not supported           |
+
+
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
-### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
-within Xinference.
-
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
                (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
-full potential of cutting-edge AI models. ![demo](assets/demo.gif)
+full potential of cutting-edge AI models.
                         ð_Join_our_Slack_community!
 ## Key Features ð **Model Serving Made Easy**: Simplify the process of
 serving large language, speech recognition, and multimodal models. You can set
 up and deploy your models for experimentation and production with a single
 command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
 built-in models using a single command. Inference provides access to state-of-
 the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
@@ -33,82 +33,112 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
-installs all the necessary packages for serving models. If you want to achieve
+conflicts. ### Installation ```bash $ pip install "xinference" ``` `xinference`
+installs basic packages for serving models. #### Installation with GGML To
+serve ggml models, you need to install the following extra dependencies:
+```bash $ pip install "xinference[ggml]" ``` If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
-`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
-a single command or deploy it in a distributed cluster. #### Local To start a
-local instance of Xinference, run the following command: ```bash $ xinference
-``` #### Distributed To deploy Xinference in a cluster, you need to start a
-Xinference supervisor on one server and Xinference workers on the other
-servers. Follow the steps below: **Starting the Supervisor**: On the server
-where you want to run the Xinference supervisor, run the following command:
-```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+`chatglm` and `chatglm2`. #### Installation with PyTorch To serve PyTorch
+models, you need to install the following extra dependencies: ```bash $ pip
+install "xinference[pytorch]" ``` #### Installation with all dependencies If
+you want to serve all the supported models, install all the dependencies:
+```bash $ pip install "xinference[all]" ``` ### Deployment You can deploy
+Xinference locally with a single command or deploy it in a distributed cluster.
+#### Local To start a local instance of Xinference, run the following command:
+```bash $ xinference ``` #### Distributed To deploy Xinference in a cluster,
+you need to start a Xinference supervisor on one server and Xinference workers
+on the other servers. Follow the steps below: **Starting the Supervisor**: On
+the server where you want to run the Xinference supervisor, run the following
+command: ```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
 {supervisor_host}` with the actual host of your supervisor server. **Starting
 the Workers**: On each of the other servers where you want to run Xinference
 workers, run the following command: ```bash $ xinference-worker -e "http://$
 {supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
 accessible for model management via CLI or Xinference client. - For local
 deployment, the endpoint will be `http://localhost:9997`. - For cluster
 deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
 {supervisor_host}` is the hostname or IP address of the server where the
 supervisor is running. You can also view a web UI using the Xinference endpoint
 to chat with all the builtin models. You can even **chat with two cutting-edge
 AI models side-by-side to compare their performance**! ![web UI](assets/
-xinference-downloading.png) ### Xinference CLI Xinference provides a command
-line interface (CLI) for model management. Here are some useful commands: -
-Launch a model (a model UID will be returned): `xinference launch` - List
-running models: `xinference list` - List all the builtin models: `xinference
-list --all` - Terminate a model: `xinference terminate --model-uid $
-{model_uid}` ### Xinference Client Xinference also provides a client for
-managing and accessing models programmatically: ```python from
-xinference.client import Client client = Client("http://localhost:9997")
-model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
-(model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
-( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
-```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
-"56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
-1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
-"content": "The largest animal that has been scientifically measured is the
-blue whale, which has a maximum length of around 23 meters (75 feet) for adult
-animals and can weigh up to 150,000 pounds (68,000 kg). However, it is
-important to note that this is just an estimate and that the largest animal
-known to science may be larger still. Some scientists believe that the largest
-animals may not have a clear \"size\" in the same way that humans do, as their
-size can vary depending on the environment and the stage of their life." },
-"finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
-"completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
-for more examples. ## Builtin models To view the builtin models, run the
-following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | |---------------|---------------
----|----------|---------|--------------------|---------------------------------
---------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
-ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+demo.gif) ### Xinference CLI Xinference provides a command line interface (CLI)
+for model management. Here are some useful commands: - Launch a model (a model
+UID will be returned): `xinference launch` - List running models: `xinference
+list` - List all the builtin models: `xinference list --all` - Terminate a
+model: `xinference terminate --model-uid ${model_uid}` ### Xinference Client
+Xinference also provides a client for managing and accessing models
+programmatically: ```python from xinference.client import Client client =
+Client("http://localhost:9997") model_uid = client.launch_model
+(model_name="chatglm2") model = client.get_model(model_uid) chat_history = []
+prompt = "What is the largest animal?" model.chat( prompt, chat_history,
+generate_config={"max_tokens": 1024} ) ``` Result: ```json { "id": "chatcmpl-
+8d76b65a-bad0-42ef-912d-4a0533d90d61", "model": "56f69622-1e73-11ee-a3bd-
+9af9f16816c6", "object": "chat.completion", "created": 1688919187, "choices":
+[ { "index": 0, "message": { "role": "assistant", "content": "The largest
+animal that has been scientifically measured is the blue whale, which has a
+maximum length of around 23 meters (75 feet) for adult animals and can weigh up
+to 150,000 pounds (68,000 kg). However, it is important to note that this is
+just an estimate and that the largest animal known to science may be larger
+still. Some scientists believe that the largest animals may not have a clear
+\"size\" in the same way that humans do, as their size can vary depending on
+the environment and the stage of their life." }, "finish_reason": "None" } ],
+"usage": { "prompt_tokens": -1, "completion_tokens": -1, "total_tokens": -1 } }
+``` See [examples](examples) for more examples. ## Builtin models To view the
+builtin models, run the following command: ```bash $ xinference list --all ```
+### ggmlv3 models | Name | Type | Language | Format | Size (in billions) |
+Quantization | |---------------|------------------|----------|---------|-------
+-------------|-----------------------------------------| | llama-2 | Foundation
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
-'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
-'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
-ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
-Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
-SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-**NOTE**: - Xinference will download models automatically for you, and by
-default the models will be saved under `${USER}/.xinference/cache`. -
-Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
-acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
-Xinference is currently under active development. Here's a roadmap outlining
-our planned developments for the next few weeks: ### PyTorch Support With
-PyTorch integration, users will be able to seamlessly utilize PyTorch models
-from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
-With Xinference, it will be much easier for users to use these libraries and
-build applications with LLMs.
+baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | llama-2-chat | RLHF Model | en | ggmlv3 | 7, 13, 70 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh |
+ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model |
+en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0
+| SFT Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'
+| | wizardlm-v1.1 | SFT Model | en | ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 |
+'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | ### pytorch models | Name | Type |
+Language | Format | Size (in billions) | Quantization | |---------------|------
+------------|----------|---------|--------------------|------------------------
+--| | baichuan | Foundation Model | en, zh | pytorch | 7, 13 | '4-bit', '8-
+bit', 'none' | | baichuan-chat | SFT Model | en, zh | pytorch | 13 | '4-bit',
+'8-bit', 'none' | | vicuna-v1.3 | SFT Model | en | pytorch | 7, 13, 33 | '4-
+bit', '8-bit', 'none' | **NOTE**: - Xinference will download models
+automatically for you, and by default the models will be saved under `$
+{USER}/.xinference/cache`. - Foundation models only provide interface
+`generate`. - RLHF and SFT models provide both `generate` and `chat`. - If you
+want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1
+quantization methods. - `llama-2-chat` 70B ggmlv3 model only supports q4_0
+quantization currently. ## Pytorch Model Best Practices Pytorch has been
+integrated recently, and the usage scenarios are described below: ### supported
+models - Foundation Modelï¼baichuanï¼7Bã13Bï¼ã - SFT Modelï¼baichuan-
+chatï¼13Bï¼ãvicuna-v1.3ï¼7Bã13Bã33Bï¼ã ### supported devices -
+CUDA: On Linux and Windows systems, `cuda` device is used by default. - MPS: On
+Mac M1/M2 devices, `mps` device is used by default. - CPU: It is not
+recommended to use a `cpu` device, as it takes up a lot of memory and the
+inference speed is very slow. ### quantization methods - `none`: indicates that
+no quantization is used. - `8-bit`: use 8-bit quantization. - `4-bit`: use 4-
+bit quantization. Note: 4-bit quantization is only supported on Linux systems
+and CUDA devices. ### other instructions - On MacOS system, baichuan-chat model
+is not supported, and baichuan model cannot use 8-bit quantization. ### use
+cases The table below shows memory usage and supported devices of some models.
+| Name | Size (B) | OS | No quantization (MB) | Quantization 8-bit (MB) |
+Quantization 4-bit (MB) | |---------------|----------|-------|-----------------
+-----|-------------------------|-------------------------| | baichuan-chat | 13
+| linux | not currently tested | 13275 | 7263 | | baichuan-chat | 13 | macos |
+not supported | not supported | not supported | | vicuna-v1.3 | 7 | linux |
+12884 | 6708 | 3620 | | vicuna-v1.3 | 7 | macos | 12916 | 565 | not supported |
+| baichuan | 7 | linux | 13480 | 7304 | 4216 | | baichuan | 7 | macos | 13480 |
+not supported | not supported | ## Roadmap Xinference is currently under active
+development. Here's a roadmap outlining our planned developments for the next
+few weeks: ### Langchain & LlamaIndex integration With Xinference, it will be
+much easier for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.6/setup.cfg` & `xinference-0.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 include_package_data = True
 packages = find:
 install_requires = 
 	xoscar
 	xorbits
 	gradio>=3.35.0
 	click
-	tqdm
+	tqdm>=4.27
 	tabulate
 	requests
-	pydantic
+	pydantic<2
 	fastapi
 	uvicorn
 	sse_starlette
+	huggingface-hub>=0.14.1,<1.0
+	typing_extensions
 
 [options.packages.find]
 exclude = 
 	*.conftest*
 	*.tests.*
 	*.tests
 
@@ -55,21 +57,33 @@
 	pydata-sphinx-theme>=0.3.0
 	sphinx-intl>=0.9.9
 	jieba>=0.42.0
 	flake8>=3.8.0
 	black
 all = 
 	chatglm-cpp
-	llama-cpp-python
-	transformers
+	llama-cpp-python>=0.1.77
+	transformers>=4.31.0
 	torch
-	accelerate
+	accelerate>=0.20.3
 	sentencepiece
 	transformers_stream_generator
-	cpm_kernels; platform_system != "Darwin"
+	bitsandbytes
+	protobuf
+ggml = 
+	chatglm-cpp
+	llama-cpp-python>=0.1.77
+pytorch = 
+	transformers>=4.31.0
+	torch
+	accelerate>=0.20.3
+	sentencepiece
+	transformers_stream_generator
+	bitsandbytes
+	protobuf
 doc = 
 	ipython>=6.5.0
 	sphinx>=3.0.0,<5.0.0
 	pydata-sphinx-theme>=0.3.0
 	sphinx-intl>=0.9.9
 
 [options.entry_points]
```

### Comparing `xinference-0.0.6/setup.py` & `xinference-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/versioneer.py` & `xinference-0.1.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/__init__.py` & `xinference-0.1.0/xinference/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 
 from . import _version
 
 __version__ = _version.get_versions()["version"]
 
 
-def install():
+def _install():
     from xoscar.backends.router import Router
 
-    from .model import install as install_model
+    from .model import _install as install_model
 
     default_router = Router.get_instance_or_empty()
     Router.set_instance(default_router)
+
     install_model()
 
 
-install()
-del install
+_install()
+del _install
```

### Comparing `xinference-0.0.6/xinference/client.py` & `xinference-0.1.0/xinference/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
 import json
 import uuid
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union
 
 import requests
 import xoscar as xo
 
 from .core.model import ModelActor
 from .core.service import SupervisorActor
 from .isolation import Isolation
 
 if TYPE_CHECKING:
-    from .model import ModelSpec
-    from .model.llm.chatglm import ChatglmCppGenerateConfig
-    from .model.llm.core import LlamaCppGenerateConfig
+    from .model.llm.ggml.chatglm import ChatglmCppGenerateConfig
+    from .model.llm.ggml.llamacpp import LlamaCppGenerateConfig
     from .model.llm.pytorch.core import PytorchGenerateConfig
     from .types import (
         ChatCompletion,
         ChatCompletionChunk,
         ChatCompletionMessage,
         Completion,
         CompletionChunk,
@@ -130,25 +129,19 @@
         self,
         prompt: str,
         generate_config: Optional[
             Union["LlamaCppGenerateConfig", "PytorchGenerateConfig"]
         ] = None,
     ) -> Union["Completion", Iterator["CompletionChunk"]]:
         url = f"{self._base_url}/v1/completions"
-        if generate_config is None:
-            request_body = {"model": self._model_uid, "prompt": prompt}
-        else:
-            generate_config_dict = {}
+
+        request_body: Dict[str, Any] = {"model": self._model_uid, "prompt": prompt}
+        if generate_config is not None:
             for key, value in generate_config.items():
-                generate_config_dict[str(key)] = str(value)
-            request_body = {
-                "model": self._model_uid,
-                "prompt": prompt,
-                **generate_config_dict,
-            }
+                request_body[key] = value
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate completion, detail: {response.json()['detail']}"
             )
 
@@ -192,25 +185,21 @@
 
         else:
             if system_prompt is not None:
                 chat_history.insert(0, {"role": "system", "content": system_prompt})
 
         chat_history.append({"role": "user", "content": prompt})
 
-        if generate_config is None:
-            request_body = {"model": self._model_uid, "messages": chat_history}
-        else:
-            generate_config_dict = {}
+        request_body: Dict[str, Any] = {
+            "model": self._model_uid,
+            "messages": chat_history,
+        }
+        if generate_config is not None:
             for key, value in generate_config.items():
-                generate_config_dict[str(key)] = str(value)
-            request_body = {
-                "model": self._model_uid,
-                "messages": chat_history,
-                **generate_config_dict,
-            }
+                request_body[key] = value
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate chat completion, detail: {response.json()['detail']}"
             )
 
@@ -231,25 +220,22 @@
         url = f"{self._base_url}/v1/chat/completions"
 
         if chat_history is None:
             chat_history = []
 
         chat_history.append({"role": "user", "content": prompt})
 
-        if generate_config is None:
-            request_body = {"model": self._model_uid, "messages": chat_history}
-        else:
-            generate_config_dict = {}
+        request_body: Dict[str, Any] = {
+            "model": self._model_uid,
+            "messages": chat_history,
+        }
+
+        if generate_config is not None:
             for key, value in generate_config.items():
-                generate_config_dict[str(key)] = str(value)
-            request_body = {
-                "model": self._model_uid,
-                "messages": chat_history,
-                **generate_config_dict,
-            }
+                request_body[key] = value
 
         response = requests.post(url, json=request_body)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to generate chat completion, detail: {response.json()['detail']}"
             )
 
@@ -297,30 +283,32 @@
 
         return model_uid
 
     def terminate_model(self, model_uid: str):
         coro = self._supervisor_ref.terminate_model(model_uid)
         return self._isolation.call(coro)
 
-    def list_models(self) -> List[Tuple[str, "ModelSpec"]]:
+    def list_models(self) -> Dict[str, Dict[str, Any]]:
         coro = self._supervisor_ref.list_models()
         return self._isolation.call(coro)
 
     def get_model(self, model_uid: str) -> "ModelHandle":
-        model_spec: "ModelSpec" = self._isolation.call(
+        desc: Dict[str, Any] = self._isolation.call(
             self._supervisor_ref.describe_model(model_uid)
         )
         model_ref = self._isolation.call(self._supervisor_ref.get_model(model_uid))
 
-        if model_spec.model_name == "chatglm" or model_spec.model_name == "chatglm2":
+        if desc["model_name"] == "chatglm" or desc["model_name"] == "chatglm2":
             return ChatglmCppChatModelHandle(model_ref, self._isolation)
-        elif model_spec.model_name in ["baichuan", "baichuan-base", "llama-2"]:
+        elif "generate" in desc["model_ability"]:
             return GenerateModelHandle(model_ref, self._isolation)
-        else:
+        elif "chat" in desc["model_ability"]:
             return ChatModelHandle(model_ref, self._isolation)
+        else:
+            raise ValueError(f"Unrecognized model ability: {desc['model_ability']}")
 
 
 class RESTfulClient:
     def __init__(self, base_url):
         self.base_url = base_url
 
     @classmethod
@@ -393,18 +381,17 @@
     def get_model(self, model_uid: str) -> RESTfulModelHandle:
         url = f"{self.base_url}/v1/models/{model_uid}"
         response = requests.get(url)
         if response.status_code != 200:
             raise RuntimeError(
                 f"Failed to get the model description, detail: {response.json()['detail']}"
             )
-        model_spec = response.json()
+        desc = response.json()
 
-        if (
-            model_spec["model_name"] == "chatglm"
-            or model_spec["model_name"] == "chatglm2"
-        ):
+        if desc["model_name"] == "chatglm" or desc["model_name"] == "chatglm2":
             return RESTfulChatglmCppChatModelHandle(model_uid, self.base_url)
-        elif model_spec["model_name"] in ["baichuan", "baichuan-base", "llama-2"]:
+        elif "generate" in desc["model_ability"]:
             return RESTfulGenerateModelHandle(model_uid, self.base_url)
-        else:
+        elif "chat" in desc["model_ability"]:
             return RESTfulChatModelHandle(model_uid, self.base_url)
+        else:
+            raise ValueError(f"Unrecognized model ability: {desc['model_ability']}")
```

### Comparing `xinference-0.0.6/xinference/constants.py` & `xinference-0.1.0/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/core/__init__.py` & `xinference-0.1.0/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/core/api.py` & `xinference-0.1.0/xinference/core/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
-from typing import TYPE_CHECKING, List, Optional, Tuple
+from typing import Any, Dict, Optional
 
 import xoscar as xo
 
 from ..isolation import Isolation
 from . import ModelActor
 from .service import SupervisorActor
 
-if TYPE_CHECKING:
-    from ..model import ModelSpec
-
 
 class AsyncSupervisorAPI:
     def __init__(self, supervisor_address: str):
         self._supervisor_address = supervisor_address
         self._supervisor_ref = None
 
     async def _get_supervisor_ref(self) -> xo.ActorRefType["SupervisorActor"]:
@@ -57,22 +54,27 @@
         )
         return model_uid
 
     async def terminate_model(self, model_uid: str):
         supervisor_ref = await self._get_supervisor_ref()
         await supervisor_ref.terminate_model(model_uid)
 
-    async def list_models(self) -> List[Tuple[str, "ModelSpec"]]:
+    async def list_models(self) -> Dict[str, Dict[str, Any]]:
         supervisor_ref = await self._get_supervisor_ref()
         return await supervisor_ref.list_models()
 
     async def get_model(self, model_uid: str) -> xo.ActorRefType["ModelActor"]:
         supervisor_ref = await self._get_supervisor_ref()
         return await supervisor_ref.get_model(model_uid)
 
+    async def is_local_deployment(self) -> bool:
+        # TODO: temporary.
+        supervisor_ref = await self._get_supervisor_ref()
+        return await supervisor_ref.is_local_deployment()
+
 
 class SyncSupervisorAPI:
     def __init__(self, supervisor_address: str):
         self._supervisor_address = supervisor_address
         self._supervisor_ref = None
         self._isolation = Isolation(asyncio.new_event_loop(), threaded=True)
         self._isolation.start()
@@ -110,20 +112,28 @@
     def terminate_model(self, model_uid: str):
         async def _terminate_model():
             supervisor_ref = await self._get_supervisor_ref()
             await supervisor_ref.terminate_model(model_uid)
 
         return self._isolation.call(_terminate_model())
 
-    def list_models(self) -> List[Tuple[str, "ModelSpec"]]:
+    def list_models(self) -> Dict[str, Dict[str, Any]]:
         async def _list_models():
             supervisor_ref = await self._get_supervisor_ref()
             return await supervisor_ref.list_models()
 
         return self._isolation.call(_list_models())
 
     def get_model(self, model_uid: str) -> xo.ActorRefType["ModelActor"]:
         async def _get_model():
             supervisor_ref = await self._get_supervisor_ref()
             return await supervisor_ref.get_model(model_uid)
 
         return self._isolation.call(_get_model())
+
+    def is_local_deployment(self) -> bool:
+        # TODO: temporary.
+        async def _is_local_deployment():
+            supervisor_ref = await self._get_supervisor_ref()
+            return await supervisor_ref.is_local_deployment()
+
+        return self._isolation.call(_is_local_deployment())
```

### Comparing `xinference-0.0.6/xinference/core/gradio.py` & `xinference-0.1.0/xinference/core/gradio.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,31 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import urllib.request
 import uuid
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import gradio as gr
 
 from ..locale.utils import Locale
-from ..model import MODEL_FAMILIES, ModelSpec
+from ..model.llm import LLM_FAMILIES, LLMFamilyV1, match_llm
+from ..model.llm.llm_family import cache
 from .api import SyncSupervisorAPI
 
 if TYPE_CHECKING:
     from ..types import ChatCompletionChunk, ChatCompletionMessage
 
-MODEL_TO_FAMILIES = dict(
+MODEL_TO_FAMILIES: Dict[str, LLMFamilyV1] = dict(
     (model_family.model_name, model_family)
-    for model_family in MODEL_FAMILIES
+    for model_family in LLM_FAMILIES
     if model_family.model_name not in ["baichuan", "baichuan-base", "llama-2"]
 )
 
 
 class GradioApp:
     def __init__(
         self,
@@ -53,15 +52,15 @@
         model_size_in_billions: Optional[int] = None,
         model_format: Optional[str] = None,
         quantization: Optional[str] = None,
     ):
         model_uid = str(uuid.uuid1())
         models = self._api.list_models()
         if len(models) >= self._max_model_num:
-            self._api.terminate_model(models[0][0])
+            self._api.terminate_model(list(models.keys())[0])
         return self._api.launch_model(
             model_uid, model_name, model_size_in_billions, model_format, quantization
         )
 
     async def generate(
         self,
         model: str,
@@ -218,83 +217,122 @@
                     scale=1,
                 )
             create_model = gr.Button(value=self._locale("create"))
 
             def select_model_name(model_name: str):
                 if model_name:
                     model_family = MODEL_TO_FAMILIES[model_name]
-                    formats = [model_family.model_format]
-                    model_sizes_in_billions = [
-                        str(b) for b in model_family.model_sizes_in_billions
-                    ]
-                    quantizations = model_family.quantizations
+                    formats = list(
+                        {spec.model_format for spec in model_family.model_specs}
+                    )
+                    formats.sort()
                     return (
                         gr.Dropdown.update(
-                            choices=formats,
-                            interactive=True,
-                            value=model_family.model_format,
-                        ),
-                        gr.Dropdown.update(
-                            choices=model_sizes_in_billions,
-                            interactive=True,
-                            value=model_sizes_in_billions[0],
+                            choices=formats, interactive=True, value=None
                         ),
+                        gr.Dropdown.update(choices=[], interactive=False, value=None),
+                        gr.Dropdown.update(choices=[], interactive=False, value=None),
+                    )
+                else:
+                    return (
+                        gr.Dropdown.update(),
+                        gr.Dropdown.update(),
+                        gr.Dropdown.update(),
+                    )
+
+            def select_model_format(model_name: str, model_format: str):
+                if model_name:
+                    model_family = MODEL_TO_FAMILIES[model_name]
+                    sizes = list(
+                        {
+                            spec.model_size_in_billions
+                            for spec in model_family.model_specs
+                            if spec.model_format == model_format
+                        }
+                    )
+                    sizes.sort()
+                    return (
                         gr.Dropdown.update(
-                            choices=quantizations,
+                            choices=list(map(lambda s: str(s), sizes)),
                             interactive=True,
-                            value=quantizations[0],
+                            value=None,
                         ),
+                        gr.Dropdown.update(choices=[], interactive=False, value=None),
                     )
                 else:
                     return (
                         gr.Dropdown.update(),
                         gr.Dropdown.update(),
-                        gr.Dropdown.update(),
                     )
 
+            def select_model_size(
+                model_name: str, model_format: str, model_size_in_billions: str
+            ):
+                if model_name:
+                    model_family = MODEL_TO_FAMILIES[model_name]
+                    quantizations = list(
+                        {
+                            quantization
+                            for spec in model_family.model_specs
+                            if spec.model_format == model_format
+                            and str(spec.model_size_in_billions)
+                            == model_size_in_billions
+                            for quantization in spec.quantizations
+                        }
+                    )
+                    quantizations.sort()
+                    return gr.Dropdown.update(
+                        choices=quantizations,
+                        interactive=True,
+                    )
+                else:
+                    return gr.Dropdown.update()
+
             model_name.change(
                 select_model_name,
                 inputs=[model_name],
                 outputs=[model_format, model_size_in_billions, quantization],
             )
+            model_format.change(
+                select_model_format,
+                inputs=[model_name, model_format],
+                outputs=[model_size_in_billions, quantization],
+            )
+            model_size_in_billions.change(
+                select_model_size,
+                inputs=[model_name, model_format, model_size_in_billions],
+                outputs=[quantization],
+            )
 
             components = self._build_chatbot("", "")
             model_text = components[0]
             chat, model_uid = components[1], components[-1]
 
         def select_model(
             _model_name: str,
             _model_format: str,
             _model_size_in_billions: str,
             _quantization: str,
-            progress=gr.Progress(),
+            progress=gr.Progress(track_tqdm=True),
         ):
-            model_family = MODEL_TO_FAMILIES[_model_name]
-            cache_path = model_family.generate_cache_path(
-                int(_model_size_in_billions), _quantization
-            )
-            if not (os.path.exists(cache_path)):
-                if os.path.exists(cache_path):
-                    os.remove(cache_path)
-                url = model_family.url_generator(
-                    int(_model_size_in_billions), _quantization
+            match_result = match_llm(
+                _model_name,
+                _model_format,
+                int(_model_size_in_billions),
+                _quantization,
+                self._api.is_local_deployment(),
+            )
+            if not match_result:
+                raise ValueError(
+                    f"Model not found, name: {_model_name}, format: {_model_format},"
+                    f" size: {_model_size_in_billions}, quantization: {_quantization}"
                 )
-                try:
-                    urllib.request.urlretrieve(
-                        url,
-                        cache_path,
-                        reporthook=lambda block_num, block_size, total_size: progress(
-                            block_num * block_size / total_size,
-                            desc=self._locale("Downloading"),
-                        ),
-                    )
-                except:
-                    if os.path.exists(cache_path):
-                        os.remove(cache_path)
-                    raise gr.Error(self._locale(f"Download failed, please retry."))
+
+            llm_family, llm_spec, _quantization = match_result
+            cache(llm_family, llm_spec, _quantization)
 
             model_uid = self._create_model(
                 _model_name, int(_model_size_in_billions), _model_format, _quantization
             )
             return gr.Chatbot.update(
                 label="-".join(
                     [_model_name, _model_size_in_billions, _model_format, _quantization]
@@ -356,87 +394,15 @@
 
         def update_message(text_in: str):
             return "", text_in
 
         msg.submit(update_message, inputs=[msg], outputs=[msg, model_text])
         gr.ClearButton(components=[chat, msg, model_text])
 
-    def _build_single_with_launched(
-        self, models: List[Tuple[str, ModelSpec]], default_index: int
-    ):
-        uid_to_model_spec: Dict[str, ModelSpec] = dict((m[0], m[1]) for m in models)
-        choices = [
-            "-".join(
-                [
-                    s.model_name,
-                    str(s.model_size_in_billions),
-                    s.model_format,
-                    s.quantization,
-                ]
-            )
-            for s in uid_to_model_spec.values()
-        ]
-        choice_to_uid = dict(zip(choices, uid_to_model_spec.keys()))
-        model_selection = gr.Dropdown(
-            label=self._locale("select model"),
-            choices=choices,
-            value=choices[default_index],
-        )
-        components = self._build_chatbot(
-            models[default_index][0], choices[default_index]
-        )
-        model_text = components[0]
-        model_uid = components[-1]
-        chat = components[1]
-
-        def select_model(model_name):
-            uid = choice_to_uid[model_name]
-            return gr.Chatbot.update(label=model_name), uid
-
-        model_selection.change(
-            select_model, inputs=[model_selection], outputs=[chat, model_uid]
-        )
-        return chat, model_text
-
-    def _build_arena_with_launched(self, models: List[Tuple[str, ModelSpec]]):
-        chat_and_text = []
-        with gr.Row():
-            for i in range(self._gladiator_num):
-                with gr.Column():
-                    chat_and_text.append(self._build_single_with_launched(models, i))
-
-        chats = [c[0] for c in chat_and_text]
-        texts = [c[1] for c in chat_and_text]
-
-        msg = gr.Textbox(label=self._locale("Input"))
-
-        def update_message(text_in: str):
-            return "", text_in, text_in
-
-        msg.submit(update_message, inputs=[msg], outputs=[msg] + texts)
-
-        gr.ClearButton(components=[msg] + chats + texts)
-
     def build(self):
-        if self._use_launched_model:
-            models = self._api.list_models()
-            with gr.Blocks() as blocks:
-                with gr.Tab(self._locale("Chat")):
-                    chat, model_text = self._build_single_with_launched(models, 0)
-                    msg = gr.Textbox(label=self._locale("Input"))
-
-                    def update_message(text_in: str):
-                        return "", text_in
-
-                    msg.submit(update_message, inputs=[msg], outputs=[msg, model_text])
-                    gr.ClearButton(components=[chat, msg, model_text])
-                if len(models) >= 2:
-                    with gr.Tab(self._locale("Arena")):
-                        self._build_arena_with_launched(models)
-        else:
-            with gr.Blocks() as blocks:
-                with gr.Tab(self._locale("Chat")):
-                    self._build_single()
-                with gr.Tab(self._locale("Arena")):
-                    self._build_arena()
+        with gr.Blocks() as blocks:
+            with gr.Tab(self._locale("Chat")):
+                self._build_single()
+            with gr.Tab(self._locale("Arena")):
+                self._build_arena()
         blocks.queue(concurrency_count=40)
         return blocks
```

### Comparing `xinference-0.0.6/xinference/core/model.py` & `xinference-0.1.0/xinference/core/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import inspect
 from typing import TYPE_CHECKING, Any, Generic, Iterator, List, Optional, TypeVar, Union
 
 import xoscar as xo
 
 if TYPE_CHECKING:
-    from ..model.llm.core import Model
+    from ..model.llm.core import LLM
     from ..types import ChatCompletionChunk, CompletionChunk
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -52,15 +52,15 @@
                 raise StopAsyncIteration
             else:
                 raise
 
 
 class ModelActor(xo.Actor):
     @classmethod
-    def gen_uid(cls, model: "Model"):
+    def gen_uid(cls, model: "LLM"):
         return f"{model.__class__}-model-actor"
 
     async def __pre_destroy__(self):
         if self._model.model_spec.model_format == "pytorch":
             try:
                 import gc
 
@@ -73,15 +73,15 @@
 
                 raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
             del self._model
             gc.collect()
             torch.cuda.empty_cache()
 
-    def __init__(self, model: "Model"):
+    def __init__(self, model: "LLM"):
         super().__init__()
         self._model = model
         self._generator: Optional[Iterator] = None
 
     def load(self):
         self._model.load()
```

### Comparing `xinference-0.0.6/xinference/core/resource.py` & `xinference-0.1.0/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/core/restful_api.py` & `xinference-0.1.0/xinference/core/restful_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,30 +279,20 @@
             server.run(self._sockets)
 
         server_thread = threading.Thread(target=_serve, daemon=True)
         server_thread.start()
 
     async def list_models(self) -> Dict[str, Dict[str, Any]]:
         try:
-            models = await self._supervisor_ref.list_models()
+            return await self._supervisor_ref.list_models()
         except Exception as e:
             logger.error(e, exc_info=True)
             raise HTTPException(status_code=500, detail=str(e))
 
-        models_dict = {}
-        for model_uid, model_spec in models:
-            models_dict[model_uid] = {
-                "model_name": model_spec.model_name,
-                "model_format": model_spec.model_format,
-                "model_size_in_billions": model_spec.model_size_in_billions,
-                "quantization": model_spec.quantization,
-            }
-        return models_dict
-
-    async def describe_model(self, model_uid: str):
+    async def describe_model(self, model_uid: str) -> Dict[str, Any]:
         try:
             return await self._supervisor_ref.describe_model(model_uid)
 
         except ValueError as ve:
             logger.error(str(ve), exc_info=True)
             raise HTTPException(status_code=400, detail=str(ve))
```

### Comparing `xinference-0.0.6/xinference/core/service.py` & `xinference-0.1.0/xinference/core/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # limitations under the License.
 
 import asyncio
 import platform
 import time
 from dataclasses import dataclass
 from logging import getLogger
-from typing import Callable, Dict, List, Optional, Set, Tuple
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple
 
 import xoscar as xo
 
 from ..core import ModelActor
-from ..model import ModelSpec
+from ..model.llm import LLMFamilyV1, LLMSpecV1
 from .resource import ResourceStatus, gather_node_info
 
 logger = getLogger(__name__)
 
 
 DEFAULT_NODE_DEAD_TIMEOUT = 30
 DEFAULT_NODE_CHECK_INTERVAL = 1
@@ -127,27 +127,31 @@
         # TODO: not protected.
         self._model_uid_to_worker[model_uid] = worker_ref
 
         raise xo.Return(model_ref)
 
     async def _check_dead_nodes(self):
         while True:
+            dead_nodes = []
             for address, status in self._worker_status.items():
                 if time.time() - status.update_time > DEFAULT_NODE_DEAD_TIMEOUT:
                     dead_models = []
                     for model_uid in self._model_uid_to_worker:
                         if self._model_uid_to_worker[model_uid].address == address:
                             dead_models.append(model_uid)
                     logger.error(
                         "Worker timeout. address: %s, influenced models: %s",
                         address,
                         dead_models,
                     )
-                    self._worker_status.pop(address)
-                    self._worker_address_to_worker.pop(address)
+                    dead_nodes.append(address)
+
+            for address in dead_nodes:
+                self._worker_status.pop(address)
+                self._worker_address_to_worker.pop(address)
             await asyncio.sleep(5)
 
     @log
     async def terminate_model(self, model_uid: str):
         if model_uid not in self._model_uid_to_worker:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
@@ -160,28 +164,35 @@
         if model_uid not in self._model_uid_to_worker:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         worker_ref = self._model_uid_to_worker[model_uid]
         return await worker_ref.get_model(model_uid=model_uid)
 
     @log
-    async def describe_model(self, model_uid: str):
+    async def describe_model(self, model_uid: str) -> Dict[str, Any]:
         if model_uid not in self._model_uid_to_worker:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         worker_ref = self._model_uid_to_worker[model_uid]
         return await worker_ref.describe_model(model_uid=model_uid)
 
     @log
-    async def list_models(self) -> List[Tuple[str, ModelSpec]]:
-        ret = []
+    async def list_models(self) -> Dict[str, Dict[str, Any]]:
+        ret = {}
         for worker in self._worker_address_to_worker.values():
-            ret.extend(await worker.list_models())
+            ret.update(await worker.list_models())
         return ret
 
+    def is_local_deployment(self) -> bool:
+        # TODO: temporary.
+        return (
+            len(self._worker_address_to_worker) == 1
+            and list(self._worker_address_to_worker)[0] == self.address
+        )
+
     @log
     async def add_worker(self, worker_address: str):
         assert worker_address not in self._worker_address_to_worker
 
         worker_ref = await xo.actor_ref(address=worker_address, uid=WorkerActor.uid())
         self._worker_address_to_worker[worker_address] = worker_ref
         logger.info("Worker %s has been added successfully", worker_address)
@@ -196,15 +207,17 @@
 
 class WorkerActor(xo.Actor):
     def __init__(self, supervisor_address: str, subpool_addresses: List[str]):
         super().__init__()
         self._supervisor_address = supervisor_address
         self._supervisor_ref = None
         self._model_uid_to_model: Dict[str, xo.ActorRefType["ModelActor"]] = {}
-        self._model_uid_to_model_spec: Dict[str, ModelSpec] = {}
+        self._model_uid_to_model_spec: Dict[
+            str, Tuple[LLMFamilyV1, LLMSpecV1, str]
+        ] = {}
         self._subpool_address_to_model_uids: Dict[str, Set[str]] = dict(
             [(subpool_address, set()) for subpool_address in subpool_addresses]
         )
         logger.debug(f"Worker actor initialized with subpools: {subpool_addresses}")
 
     @classmethod
     def uid(cls) -> str:
@@ -250,62 +263,83 @@
     def _check_model_is_valid(self, model_name):
         # baichuan-base and baichuan-chat depend on `cpm_kernels` module,
         # but `cpm_kernels` cannot run on Darwin system.
         if platform.system() == "Darwin":
             if model_name in ["baichuan-base", "baichuan-chat"]:
                 raise ValueError(f"{model_name} model can't run on Darwin system.")
 
+    @staticmethod
+    def _to_llm_description(
+        llm_family: LLMFamilyV1, llm_spec: LLMSpecV1, quantization: str
+    ) -> Dict[str, Any]:
+        return {
+            "model_type": "LLM",
+            "model_name": llm_family.model_name,
+            "model_lang": llm_family.model_lang,
+            "model_ability": llm_family.model_ability,
+            "model_description": llm_family.model_description,
+            "model_format": llm_spec.model_format,
+            "model_size_in_billions": llm_spec.model_size_in_billions,
+            "quantization": quantization,
+        }
+
     @log
     async def launch_builtin_model(
         self,
         model_uid: str,
         model_name: str,
         model_size_in_billions: Optional[int],
         model_format: Optional[str],
         quantization: Optional[str],
         **kwargs,
     ) -> xo.ActorRefType["ModelActor"]:
         assert model_uid not in self._model_uid_to_model
         self._check_model_is_valid(model_name)
 
-        from ..model import MODEL_FAMILIES
+        from ..model.llm import match_llm, match_llm_cls
 
-        for model_family in MODEL_FAMILIES:
-            model_spec = model_family.match(
-                model_name=model_name,
-                model_format=model_format,
-                model_size_in_billions=model_size_in_billions,
-                quantization=quantization,
+        assert self._supervisor_ref is not None
+        match_result = match_llm(
+            model_name,
+            model_format,
+            model_size_in_billions,
+            quantization,
+            await self._supervisor_ref.is_local_deployment(),
+        )
+        if not match_result:
+            raise ValueError(
+                f"Model not found, name: {model_name}, format: {model_format},"
+                f" size: {model_size_in_billions}, quantization: {quantization}"
             )
+        llm_family, llm_spec, quantization = match_result
+        assert quantization is not None
 
-            if model_spec is None:
-                continue
+        from ..model.llm.llm_family import cache
 
-            save_path = await asyncio.to_thread(
-                model_family.cache,
-                model_spec.model_size_in_billions,
-                model_spec.quantization,
-            )
+        save_path = await asyncio.to_thread(cache, llm_family, llm_spec, quantization)
 
-            cls = model_family.cls
-            model = cls(model_uid, model_spec, save_path, kwargs)
-            subpool_address = self._choose_subpool()
-            model_ref = await xo.create_actor(
-                ModelActor, address=subpool_address, uid=model_uid, model=model
+        llm_cls = match_llm_cls(llm_family, llm_spec)
+        if not llm_cls:
+            raise ValueError(
+                f"Model not supported, name: {model_name}, format: {model_format},"
+                f" size: {model_size_in_billions}, quantization: {quantization}"
             )
-            await model_ref.load()
-            self._model_uid_to_model[model_uid] = model_ref
-            self._model_uid_to_model_spec[model_uid] = model_spec
-            self._subpool_address_to_model_uids[subpool_address].add(model_uid)
-            return model_ref
-
-        raise ValueError(
-            f"Model not found, name: {model_name}, format: {model_format},"
-            f" size: {model_size_in_billions}, quantization: {quantization}"
+
+        model = llm_cls(
+            model_uid, llm_family, llm_spec, quantization, save_path, kwargs
+        )
+        subpool_address = self._choose_subpool()
+        model_ref = await xo.create_actor(
+            ModelActor, address=subpool_address, uid=model_uid, model=model
         )
+        await model_ref.load()
+        self._model_uid_to_model[model_uid] = model_ref
+        self._model_uid_to_model_spec[model_uid] = (llm_family, llm_spec, quantization)
+        self._subpool_address_to_model_uids[subpool_address].add(model_uid)
+        return model_ref
 
     @log
     async def terminate_model(self, model_uid: str):
         if model_uid not in self._model_uid_to_model:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         model_ref = self._model_uid_to_model[model_uid]
@@ -314,33 +348,34 @@
         del self._model_uid_to_model[model_uid]
         del self._model_uid_to_model_spec[model_uid]
         for subpool_address in self._subpool_address_to_model_uids:
             if model_uid in self._subpool_address_to_model_uids[subpool_address]:
                 self._subpool_address_to_model_uids[subpool_address].remove(model_uid)
 
     @log
-    async def list_models(self) -> List[Tuple[str, ModelSpec]]:
-        ret = []
+    async def list_models(self) -> Dict[str, Dict[str, Any]]:
+        ret = {}
         for k, v in self._model_uid_to_model_spec.items():
-            ret.append((k, v))
+            ret[k] = self._to_llm_description(v[0], v[1], v[2])
         return ret
 
     @log
     async def get_model(self, model_uid: str) -> xo.ActorRefType["ModelActor"]:
         if model_uid not in self._model_uid_to_model:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
         return self._model_uid_to_model[model_uid]
 
     @log
-    async def describe_model(self, model_uid: str) -> ModelSpec:
+    async def describe_model(self, model_uid: str) -> Dict[str, Any]:
         if model_uid not in self._model_uid_to_model:
             raise ValueError(f"Model not found in the model list, uid: {model_uid}")
 
-        return self._model_uid_to_model_spec[model_uid]
+        llm_family, llm_spec, quantization = self._model_uid_to_model_spec[model_uid]
+        return self._to_llm_description(llm_family, llm_spec, quantization)
 
     async def report_status(self):
         status = await asyncio.to_thread(gather_node_info)
         await self._supervisor_ref.report_worker_status(self.address, status)
 
     async def _periodical_report_status(self):
         while True:
```

### Comparing `xinference-0.0.6/xinference/deploy/__init__.py` & `xinference-0.1.0/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/deploy/cmdline.py` & `xinference-0.1.0/xinference/deploy/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,32 +141,30 @@
 )
 @click.option("--all", is_flag=True)
 def model_list(endpoint: str, all: bool):
     import sys
 
     from tabulate import tabulate
 
-    from ..model import MODEL_FAMILIES
+    # TODO: get from the supervisor
+    from ..model.llm import LLM_FAMILIES
 
     table = []
     if all:
-        for model_family in MODEL_FAMILIES:
+        for model_family in LLM_FAMILIES:
             table.append(
                 [
                     model_family.model_name,
-                    model_family.model_format,
-                    model_family.model_sizes_in_billions,
-                    model_family.quantizations,
+                    model_family.model_lang,
+                    model_family.model_ability,
                 ]
             )
 
         print(
-            tabulate(
-                table, headers=["Name", "Format", "Size (in billions)", "Quantization"]
-            ),
+            tabulate(table, headers=["Name", "Language", "Ability"]),
             file=sys.stderr,
         )
     else:
         client = RESTfulClient(base_url=endpoint)
         models = client.list_models()
         for model_uid, model_spec in models.items():
             table.append(
```

### Comparing `xinference-0.0.6/xinference/deploy/local.py` & `xinference-0.1.0/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/deploy/supervisor.py` & `xinference-0.1.0/xinference/deploy/supervisor.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/deploy/test/__init__.py` & `xinference-0.1.0/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/deploy/utils.py` & `xinference-0.1.0/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/deploy/worker.py` & `xinference-0.1.0/xinference/deploy/worker.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/isolation.py` & `xinference-0.1.0/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/locale/__init__.py` & `xinference-0.1.0/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/locale/utils.py` & `xinference-0.1.0/xinference/locale/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/locale/zh_CN.json` & `xinference-0.1.0/xinference/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/model/llm/chatglm.py` & `xinference-0.1.0/xinference/model/llm/ggml/chatglm.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
 import time
 import uuid
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterator, List, Optional, TypedDict, Union
 
-from ...types import ChatCompletion, ChatCompletionChunk, ChatCompletionMessage
-from .core import Model
+from ....types import ChatCompletion, ChatCompletionChunk, ChatCompletionMessage
+from .. import LLMFamilyV1, LLMSpecV1
+from ..core import LLM
 
 if TYPE_CHECKING:
     from chatglm_cpp import Pipeline
 
-    from .. import ModelSpec
 
 logger = logging.getLogger(__name__)
 
 
 class ChatglmCppModelConfig(TypedDict, total=False):
     pass
 
@@ -36,25 +37,26 @@
 class ChatglmCppGenerateConfig(TypedDict, total=False):
     max_tokens: int
     top_p: float
     temperature: float
     stream: bool
 
 
-class ChatglmCppChatModel(Model):
+class ChatglmCppChatModel(LLM):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
         model_config: Optional[ChatglmCppModelConfig] = None,
     ):
-        super().__init__(model_uid, model_spec)
+        super().__init__(model_uid, model_family, model_spec, quantization, model_path)
         self._llm: Optional["Pipeline"] = None
-        self._model_path = model_path
 
         # just a placeholder for now as the chatglm_cpp repo doesn't support model config.
         self._model_config = model_config
 
     @classmethod
     def _sanitize_generate_config(
         cls,
@@ -76,15 +78,37 @@
                 "pip install git+https://github.com/li-plus/chatglm.cpp.git@main\n\n",
                 "Or visit the original git repo if the above command fails:\n",
                 "https://github.com/li-plus/chatglm.cpp",
             ]
 
             raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
-        self._llm = chatglm_cpp.Pipeline(Path(self._model_path))
+        model_file_path = os.path.join(
+            self.model_path,
+            self.model_spec.model_file_name_template.format(
+                quantization=self.quantization
+            ),
+        )
+
+        # handle legacy cache.
+        legacy_model_file_path = os.path.join(self.model_path, "model.bin")
+        if os.path.exists(legacy_model_file_path):
+            model_file_path = legacy_model_file_path
+
+        self._llm = chatglm_cpp.Pipeline(Path(model_file_path))
+
+    @classmethod
+    def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
+        if llm_spec.model_format != "ggmlv3":
+            return False
+        if "chatglm" not in llm_family.model_name:
+            return False
+        if "chat" not in llm_family.model_ability:
+            return False
+        return True
 
     @staticmethod
     def _convert_raw_text_chunks_to_chat(
         tokens: Iterator[str], model_name: str
     ) -> Iterator[ChatCompletionChunk]:
         yield {
             "id": "chat" + f"cmpl-{str(uuid.uuid4())}",
```

### Comparing `xinference-0.0.6/xinference/model/llm/core.py` & `xinference-0.1.0/xinference/model/llm/ggml/llamacpp.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,45 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import abc
 import logging
+import os
 import platform
-from abc import abstractmethod
 from typing import TYPE_CHECKING, Iterator, List, Optional, TypedDict, Union
 
-from ...types import (
+from ....types import (
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionMessage,
     Completion,
     CompletionChunk,
     Embedding,
 )
-from .utils import ChatModelDataProcessorMixin
+from ..core import LLM
+from ..llm_family import LLMFamilyV1, LLMSpecV1
+from ..utils import ChatModelMixin
 
 if TYPE_CHECKING:
     from llama_cpp import LogitsProcessorList, StoppingCriteriaList
 
-    from .. import ModelSpec
-
 logger = logging.getLogger(__name__)
 
-SIZE_TO_GPU_LAYERS = {
-    3: 26,
-    7: 32,
-    13: 40,
-    30: 60,
-    65: 80,
-}
-
 
 class LlamaCppGenerateConfig(TypedDict, total=False):
     suffix: Optional[str]
     max_tokens: int
     temperature: float
     top_p: float
     logprobs: Optional[int]
@@ -79,61 +70,52 @@
     embedding: bool
     n_threads: Optional[int]
     n_batch: int
     last_n_tokens_size: int
     lora_base: Optional[str]
     lora_path: Optional[str]
     low_vram: bool
+    n_gqa: Optional[int]  # (TEMPORARY) must be 8 for llama2 70b
+    rms_norm_eps: Optional[float]  # (TEMPORARY)
     verbose: bool
 
 
-class Model(abc.ABC):
-    def __init__(self, model_uid: str, model_spec: "ModelSpec", *args, **kwargs):
-        self.model_uid = model_uid
-        self.model_spec = model_spec
-
-    @staticmethod
-    def _is_darwin_and_apple_silicon():
-        return platform.system() == "Darwin" and platform.processor() == "arm"
-
-    @staticmethod
-    def _is_linux():
-        return platform.system() == "Linux"
-
-    @abstractmethod
-    def load(self):
-        pass
+SIZE_TO_GPU_LAYERS = {
+    3: 26,
+    7: 32,
+    13: 40,
+    30: 60,
+    65: 80,
+}
 
 
-class LlamaCppModel(Model):
+class LlamaCppModel(LLM):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
         llamacpp_model_config: Optional[LlamaCppModelConfig] = None,
     ):
-        super().__init__(model_uid, model_spec)
+        super().__init__(model_uid, model_family, model_spec, quantization, model_path)
 
         closest_size = min(
             SIZE_TO_GPU_LAYERS.keys(),
             key=lambda x: abs(x - model_spec.model_size_in_billions),
         )
         self._gpu_layers = SIZE_TO_GPU_LAYERS[closest_size]
-        self._model_path = model_path
         self._llamacpp_model_config: LlamaCppModelConfig = self._sanitize_model_config(
             llamacpp_model_config
         )
         self._llm = None
 
     def _can_apply_metal(self):
-        return (
-            self.model_spec.quantization == "q4_0"
-            or self.model_spec.quantization == "q4_1"
-        )
+        return self.quantization in ["q4_0", "q4_1"]
 
     def _can_apply_cublas(self):
         # TODO: figure out the quantizations supported.
         return True
 
     def _sanitize_model_config(
         self, llamacpp_model_config: Optional[LlamaCppModelConfig]
@@ -145,14 +127,21 @@
         else:
             llamacpp_model_config.setdefault("n_ctx", 2048)
 
         llamacpp_model_config.setdefault("embedding", True)
         llamacpp_model_config.setdefault("use_mmap", False)
         llamacpp_model_config.setdefault("use_mlock", True)
 
+        if (
+            "llama-2" in self.model_family.model_name
+            and self.model_spec.model_size_in_billions == 70
+        ):
+            llamacpp_model_config["use_mlock"] = False
+            llamacpp_model_config["n_gqa"] = 8
+
         if self._is_darwin_and_apple_silicon() and self._can_apply_metal():
             llamacpp_model_config.setdefault("n_gpu_layers", 1)
         elif self._is_linux() and self._can_apply_cublas():
             llamacpp_model_config.setdefault("n_gpu_layers", self._gpu_layers)
 
         return llamacpp_model_config
 
@@ -173,20 +162,41 @@
                 "Please make sure 'llama_cpp' is installed. ",
                 "You can install it by visiting the installation section of the git repo:\n",
                 "https://github.com/abetlen/llama-cpp-python#installation-with-openblas--cublas--clblast--metal",
             ]
 
             raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
+        # handle legacy cache.
+        model_path = os.path.join(
+            self.model_path,
+            self.model_spec.model_file_name_template.format(
+                quantization=self.quantization
+            ),
+        )
+        legacy_model_file_path = os.path.join(self.model_path, "model.bin")
+        if os.path.exists(legacy_model_file_path):
+            model_path = legacy_model_file_path
+
         self._llm = Llama(
-            model_path=self._model_path,
+            model_path=model_path,
             verbose=False,
             **self._llamacpp_model_config,
         )
 
+    @classmethod
+    def match(cls, llm_family: LLMFamilyV1, llm_spec: LLMSpecV1) -> bool:
+        if llm_spec.model_format != "ggmlv3":
+            return False
+        if "chatglm" in llm_family.model_name:
+            return False
+        if "generate" not in llm_family.model_ability:
+            return False
+        return True
+
     def generate(
         self, prompt: str, generate_config: Optional[LlamaCppGenerateConfig] = None
     ) -> Union[Completion, Iterator[CompletionChunk]]:
         def generator_wrapper(
             _prompt: str,
             repeat_penalty: float,
             _generate_config: LlamaCppGenerateConfig,
@@ -221,52 +231,66 @@
 
     def create_embedding(self, input: Union[str, List[str]]) -> Embedding:
         assert self._llm is not None
         embedding = self._llm.create_embedding(input)
         return embedding
 
 
-class LlamaCppChatModel(LlamaCppModel, ChatModelDataProcessorMixin):
+class LlamaCppChatModel(LlamaCppModel, ChatModelMixin):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
-        system_prompt: str,
-        sep: str,
-        user_name: str,
-        assistant_name: str,
-        stop: Optional[Union[str, List[str]]] = None,
         llamacpp_model_config: Optional[LlamaCppModelConfig] = None,
     ):
-        super().__init__(model_uid, model_spec, model_path, llamacpp_model_config)
-        self._system_prompt: str = system_prompt
-        self._sep: str = sep
-        self._user_name: str = user_name
-        self._assistant_name: str = assistant_name
-        self._stop = stop
+        super().__init__(
+            model_uid,
+            model_family,
+            model_spec,
+            quantization,
+            model_path,
+            llamacpp_model_config,
+        )
+
+    @classmethod
+    def match(cls, llm_family: LLMFamilyV1, llm_spec: LLMSpecV1) -> bool:
+        if llm_spec.model_format != "ggmlv3":
+            return False
+        if "chatglm" in llm_family.model_name:
+            return False
+        if "chat" not in llm_family.model_ability:
+            return False
+        return True
 
     def _sanitize_generate_config(
         self, generate_config: Optional[LlamaCppGenerateConfig]
     ) -> LlamaCppGenerateConfig:
         generate_config = super()._sanitize_generate_config(generate_config)
-        if self._stop:
-            generate_config["stop"] = self._stop
+        if self.model_family.prompt_style and self.model_family.prompt_style.stop:
+            generate_config["stop"] = self.model_family.prompt_style.stop
         return generate_config
 
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
         chat_history: Optional[List[ChatCompletionMessage]] = None,
         generate_config: Optional[LlamaCppGenerateConfig] = None,
     ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
-        system_prompt = system_prompt or self._system_prompt
+        assert self.model_family.prompt_style is not None
+        prompt_style = self.model_family.prompt_style.copy()
+        if system_prompt:
+            prompt_style.system_prompt = system_prompt
+
         chat_history = chat_history or []
-        full_prompt = self._to_prompt(prompt, system_prompt, chat_history=chat_history)
+        assert prompt_style is not None
+        full_prompt = self.get_prompt(prompt, chat_history, prompt_style)
 
         generate_config = self._sanitize_generate_config(generate_config)
 
         stream = generate_config.get("stream", False)
         if stream:
             it = self.generate(full_prompt, generate_config)
             assert isinstance(it, Iterator)
```

### Comparing `xinference-0.0.6/xinference/model/llm/orca.py` & `xinference-0.1.0/xinference/model/llm/pytorch/vicuna.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,41 +8,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, Optional
+# Copyright 2022-2023 XProbe Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from .core import LlamaCppChatModel, LlamaCppModelConfig
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
-    from .. import ModelSpec
-
+    from .. import LLMFamilyV1, LLMSpecV1
+    from .core import PytorchChatModel, PytorchModelConfig
 
-class OrcaMiniGgml(LlamaCppChatModel):
-    _system_prompt = (
-        "### System:\n You are an AI assistant that follows instruction extremely well. Help as"
-        " much as you can."
-    )
-    _sep = "###"
-    _user_name = "User"
-    _assistant_name = "Response"
 
+class VicunaCensoredPytorch(PytorchChatModel):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
-        llamacpp_model_config: Optional[LlamaCppModelConfig] = None,
+        pytorch_model_config: Optional["PytorchModelConfig"] = None,
     ):
         super().__init__(
             model_uid,
+            model_family,
             model_spec,
             model_path,
-            system_prompt=self._system_prompt,
-            sep=self._sep,
-            user_name=self._user_name,
-            assistant_name=self._assistant_name,
-            llamacpp_model_config=llamacpp_model_config,
+            quantization,
+            pytorch_model_config=pytorch_model_config,
         )
+        self._use_fast_tokenizer = False
+
+    @classmethod
+    def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
+        if llm_spec.model_format != "pytorch":
+            return False
+        if "vicuna" not in llm_family.model_name:
+            return False
+        if "chat" not in llm_family.model_ability:
+            return False
+        return True
```

### Comparing `xinference-0.0.6/xinference/model/llm/pytorch/__init__.py` & `xinference-0.1.0/xinference/model/llm/ggml/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/model/llm/pytorch/core.py` & `xinference-0.1.0/xinference/model/llm/pytorch/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import TYPE_CHECKING, Iterator, List, Optional, TypedDict, Union
+from typing import Iterator, List, Optional, TypedDict, Union
 
 import torch
 
 from ....constants import XINFERENCE_CACHE_DIR
 from ....types import (
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionMessage,
     Completion,
     CompletionChunk,
     Embedding,
 )
-from ..core import Model
-from ..utils import ChatModelDataProcessorMixin
+from ..core import LLM
+from ..llm_family import LLMFamilyV1, LLMSpecV1
+from ..utils import ChatModelMixin
+from .compression import load_compress_model
 from .utils import generate_stream
 
-if TYPE_CHECKING:
-    from ... import ModelSpec
-
 logger = logging.getLogger(__name__)
 
 
 class PytorchGenerateConfig(TypedDict, total=False):
     temperature: float
     repetition_penalty: float
     top_p: float
@@ -52,47 +51,44 @@
 
 class PytorchModelConfig(TypedDict, total=False):
     revision: str
     device: str
     gpus: Optional[str]
     num_gpus: int
     max_gpu_memory: str
-    load_8bit: bool
-    cpu_offloading: bool
     gptq_ckpt: Optional[str]
     gptq_wbits: int
     gptq_groupsize: int
     gptq_act_order: bool
 
 
-class PytorchModel(Model):
+class PytorchModel(LLM):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
         pytorch_model_config: Optional[PytorchModelConfig] = None,
     ):
-        super().__init__(model_uid, model_spec)
+        super().__init__(model_uid, model_family, model_spec, quantization, model_path)
         self._use_fast_tokenizer = True
-        self._model_path = model_path
         self._pytorch_model_config: PytorchModelConfig = self._sanitize_model_config(
             pytorch_model_config
         )
 
     def _sanitize_model_config(
         self, pytorch_model_config: Optional[PytorchModelConfig]
     ) -> PytorchModelConfig:
         if pytorch_model_config is None:
             pytorch_model_config = PytorchModelConfig()
         pytorch_model_config.setdefault("revision", "main")
         pytorch_model_config.setdefault("gpus", None)
         pytorch_model_config.setdefault("num_gpus", 1)
-        pytorch_model_config.setdefault("load_8bit", False)
-        pytorch_model_config.setdefault("cpu_offloading", False)
         pytorch_model_config.setdefault("gptq_ckpt", None)
         pytorch_model_config.setdefault("gptq_wbits", 16)
         pytorch_model_config.setdefault("gptq_groupsize", -1)
         pytorch_model_config.setdefault("gptq_act_order", False)
         if self._is_darwin_and_apple_silicon():
             pytorch_model_config.setdefault("device", "mps")
         else:
@@ -121,60 +117,91 @@
                 "Please make sure 'transformers' is installed. ",
                 "You can install it by `pip install transformers`\n",
             ]
 
             raise ImportError(f"{error_message}\n\n{''.join(installation_guide)}")
 
         tokenizer = AutoTokenizer.from_pretrained(
-            self._model_path,
+            self.model_path,
             use_fast=self._use_fast_tokenizer,
             revision=kwargs["revision"],
             cache_dir=XINFERENCE_CACHE_DIR,
         )
         model = AutoModelForCausalLM.from_pretrained(
-            self._model_path,
+            self.model_path,
             low_cpu_mem_usage=True,
             cache_dir=XINFERENCE_CACHE_DIR,
             **kwargs,
         )
         return model, tokenizer
 
     def load(self):
+        quantization = self.quantization
         num_gpus = self._pytorch_model_config.get("num_gpus", 1)
-        cpu_offloading = self._pytorch_model_config.get("cpu_offloading", False)
         if self._is_darwin_and_apple_silicon():
             device = self._pytorch_model_config.get("device", "mps")
         else:
             device = self._pytorch_model_config.get("device", "cuda")
 
         if device == "cpu":
             kwargs = {"torch_dtype": torch.float32}
         elif device == "cuda":
             kwargs = {"torch_dtype": torch.float16}
-            if cpu_offloading:
-                kwargs["device_map"] = "auto"
         elif device == "mps":
             kwargs = {"torch_dtype": torch.float16}
         else:
             raise ValueError(f"Device {device} is not supported in temporary")
         kwargs["revision"] = self._pytorch_model_config.get("revision", "main")
 
-        self._model, self._tokenizer = self._load_model(kwargs)
+        if quantization != "none":
+            if device == "cuda" and self._is_linux():
+                kwargs["device_map"] = "auto"
+                if quantization == "4-bit":
+                    kwargs["load_in_4bit"] = True
+                elif quantization == "8-bit":
+                    kwargs["load_in_8bit"] = True
+                else:
+                    raise ValueError(
+                        f"Quantization {quantization} is not supported in temporary"
+                    )
+            else:
+                if num_gpus != 1:
+                    raise ValueError(f"Quantization is not supported for multi-gpu")
+                elif quantization != "8-bit":
+                    raise ValueError(
+                        f"Only 8-bit quantization is supported if it is not linux system or cuda device"
+                    )
+                else:
+                    self._model, self._tokenizer = load_compress_model(
+                        model_path=self.model_path,
+                        device=device,
+                        torch_dtype=kwargs["torch_dtype"],
+                        use_fast=self._use_fast_tokenizer,
+                        revision=kwargs["revision"],
+                    )
+                    logger.debug(f"Model Memory: {self._model.get_memory_footprint()}")
+                    return
 
-        quantization = self.model_spec.quantization
-        if quantization == "int4":
-            self._model = self._model.quantize(4)
-        elif quantization == "int8":
-            self._model = self._model.quantize(8)
+        self._model, self._tokenizer = self._load_model(kwargs)
 
         if (
-            device == "cuda" and num_gpus == 1 and not cpu_offloading
+            device == "cuda" and num_gpus == 1 and quantization == "none"
         ) or device == "mps":
             self._model.to(device)
-        print(self._model)
+        logger.debug(f"Model Memory: {self._model.get_memory_footprint()}")
+
+    @classmethod
+    def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
+        if llm_spec.model_format != "pytorch":
+            return False
+        if "baichuan" in llm_family.model_name:
+            return False
+        if "generate" not in llm_family.model_ability:
+            return False
+        return True
 
     def generate(
         self, prompt: str, generate_config: Optional[PytorchGenerateConfig] = None
     ) -> Union[Completion, Iterator[CompletionChunk]]:
         def generator_wrapper(
             prompt: str, device: str, generate_config: PytorchGenerateConfig
         ) -> Iterator[CompletionChunk]:
@@ -214,63 +241,80 @@
         else:
             return generator_wrapper(prompt, device, generate_config)
 
     def create_embedding(self, input: Union[str, List[str]]) -> Embedding:
         raise NotImplementedError
 
 
-class PytorchChatModel(PytorchModel, ChatModelDataProcessorMixin):
+class PytorchChatModel(PytorchModel, ChatModelMixin):
     def __init__(
         self,
         model_uid: str,
-        model_spec: "ModelSpec",
+        model_family: "LLMFamilyV1",
+        model_spec: "LLMSpecV1",
+        quantization: str,
         model_path: str,
-        system_prompt: str,
-        sep: str,
-        user_name: str,
-        assistant_name: str,
-        stop: Optional[Union[str, List[str]]] = None,
-        stop_token_ids: Optional[Union[int, List[int]]] = None,
         pytorch_model_config: Optional[PytorchModelConfig] = None,
     ):
-        super().__init__(model_uid, model_spec, model_path, pytorch_model_config)
-        self._system_prompt: str = system_prompt
-        self._sep: str = sep
-        self._user_name: str = user_name
-        self._assistant_name: str = assistant_name
-        self._stop: Optional[Union[str, List[str]]] = stop
-        self._stop_token_ids: Optional[Union[int, List[int]]] = stop_token_ids
+        super().__init__(
+            model_uid,
+            model_family,
+            model_spec,
+            quantization,
+            model_path,
+            pytorch_model_config,
+        )
 
     def _sanitize_generate_config(
         self,
         pytorch_generate_config: Optional[PytorchGenerateConfig],
     ) -> PytorchGenerateConfig:
         pytorch_generate_config = super()._sanitize_generate_config(
             pytorch_generate_config
         )
-        if "stop" not in pytorch_generate_config and self._stop is not None:
-            pytorch_generate_config["stop"] = self._stop
+        if (
+            "stop" not in pytorch_generate_config
+            and self.model_family.prompt_style
+            and self.model_family.prompt_style.stop
+        ):
+            pytorch_generate_config["stop"] = self.model_family.prompt_style.stop
         if (
             "stop_token_ids" not in pytorch_generate_config
-            and self._stop_token_ids is not None
+            and self.model_family.prompt_style
+            and self.model_family.prompt_style.stop_token_ids
         ):
-            pytorch_generate_config["stop_token_ids"] = self._stop_token_ids
+            pytorch_generate_config[
+                "stop_token_ids"
+            ] = self.model_family.prompt_style.stop_token_ids
 
         return pytorch_generate_config
 
+    @classmethod
+    def match(cls, llm_family: "LLMFamilyV1", llm_spec: "LLMSpecV1") -> bool:
+        if llm_spec.model_format != "pytorch":
+            return False
+        if "baichuan" in llm_family.model_name:
+            return False
+        if "chat" not in llm_family.model_ability:
+            return False
+        return True
+
     def chat(
         self,
         prompt: str,
         system_prompt: Optional[str] = None,
         chat_history: Optional[List[ChatCompletionMessage]] = None,
         generate_config: Optional[PytorchGenerateConfig] = None,
     ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
-        system_prompt = system_prompt or self._system_prompt
+        assert self.model_family.prompt_style is not None
+        prompt_style = self.model_family.prompt_style.copy()
+        if system_prompt:
+            prompt_style.system_prompt = system_prompt
         chat_history = chat_history or []
-        full_prompt = self._to_prompt(prompt, system_prompt, chat_history=chat_history)
+        full_prompt = self.get_prompt(prompt, chat_history, prompt_style)
 
         generate_config = self._sanitize_generate_config(generate_config)
 
         stream = generate_config.get("stream", False)
         if stream:
             it = self.generate(full_prompt, generate_config)
             assert isinstance(it, Iterator)
```

### Comparing `xinference-0.0.6/xinference/model/llm/pytorch/utils.py` & `xinference-0.1.0/xinference/model/llm/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.6/xinference/types.py` & `xinference-0.1.0/xinference/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     created: int
     model: str
     choices: List[CompletionChoice]
     usage: CompletionUsage
 
 
 class ChatCompletionMessage(TypedDict):
-    role: Literal["assistant", "user", "system"]
+    role: str
     content: str
     user: NotRequired[str]
 
 
 class ChatCompletionChoice(TypedDict):
     index: int
     message: ChatCompletionMessage
@@ -90,15 +90,15 @@
     created: int
     model: str
     choices: List[ChatCompletionChoice]
     usage: CompletionUsage
 
 
 class ChatCompletionChunkDelta(TypedDict):
-    role: NotRequired[Literal["assistant"]]
+    role: NotRequired[str]
     content: NotRequired[str]
 
 
 class ChatCompletionChunkChoice(TypedDict):
     index: int
     delta: ChatCompletionChunkDelta
     finish_reason: Optional[str]
```

### Comparing `xinference-0.0.6/xinference.egg-info/PKG-INFO` & `xinference-0.1.0/xinference.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.6
+Version: 0.1.0
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
+Provides-Extra: ggml
+Provides-Extra: pytorch
 Provides-Extra: doc
 License-File: LICENSE
 
 <div align="center">
 <img src="./assets/xorbits-logo.png" width="180px" alt="xorbits" />
 
 # Xorbits Inference: Model Serving Made Easy 🤖
@@ -41,16 +43,14 @@
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
-![demo](assets/demo.gif)
-
 <div align="center">
 <i><a href="https://join.slack.com/t/xorbitsio/shared_invite/zt-1z3zsm9ep-87yI9YZ_B79HLB2ccTq4WA">👉 Join our Slack community!</a></i>
 </div>
 
 
 ## Key Features
 🌟 **Model Serving Made Easy**: Simplify the process of serving large language, speech 
@@ -73,22 +73,43 @@
 
 🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
 with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
+
+### Installation
 ```bash
-$ pip install "xinference[all]"
+$ pip install "xinference"
+```
+`xinference` installs basic packages for serving models. 
+
+#### Installation with GGML
+To serve ggml models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[ggml]"
 ```
-`xinference[all]` installs all the necessary packages for serving models. If you want to achieve acceleration on 
+If you want to achieve acceleration on 
 different hardware, refer to the installation documentation of the corresponding package.
 - [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
 - [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
 
+#### Installation with PyTorch
+To serve PyTorch models, you need to install the following extra dependencies:
+```bash
+$ pip install "xinference[pytorch]"
+```
+
+#### Installation with all dependencies
+If you want to serve all the supported models, install all the dependencies:
+```bash
+$ pip install "xinference[all]"
+```
+
 
 ### Deployment
 You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
 #### Local
 To start a local instance of Xinference, run the following command:
 ```bash
@@ -118,15 +139,15 @@
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
 You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
-![web UI](assets/xinference-downloading.png)
+![web UI](assets/demo.gif)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
 commands:
 
 - Launch a model (a model UID will be returned): `xinference launch`
 - List running models: `xinference list`
@@ -182,37 +203,81 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
+### ggmlv3 models
+
 | Name          | Type             | Language | Format  | Size (in billions) | Quantization                            |
 |---------------|------------------|----------|---------|--------------------|-----------------------------------------|
 | llama-2       | Foundation Model | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | baichuan      | Foundation Model | en, zh   | ggmlv3  | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
-| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
+| llama-2-chat  | RLHF Model       | en       | ggmlv3  | 7, 13, 70          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | chatglm       | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | chatglm2      | SFT Model        | en, zh   | ggmlv3  | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 | wizardlm-v1.0 | SFT Model        | en       | ggmlv3  | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | wizardlm-v1.1 | SFT Model        | en       | ggmlv3  | 13                 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | vicuna-v1.3   | SFT Model        | en       | ggmlv3  | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'  |
 | orca          | SFT Model        | en       | ggmlv3  | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0'  |
 
+### pytorch models
+
+| Name          | Type             | Language | Format  | Size (in billions) | Quantization             |
+|---------------|------------------|----------|---------|--------------------|--------------------------|
+| baichuan      | Foundation Model | en, zh   | pytorch | 7, 13              | '4-bit', '8-bit', 'none' |
+| baichuan-chat | SFT Model        | en, zh   | pytorch | 13                 | '4-bit', '8-bit', 'none' |
+| vicuna-v1.3   | SFT Model        | en       | pytorch | 7, 13, 33          | '4-bit', '8-bit', 'none' |
+
 
 **NOTE**:
 - Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
 - Foundation models only provide interface `generate`.
 - RLHF and SFT models provide both `generate` and `chat`.
 - If you want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1 quantization methods.
+- `llama-2-chat` 70B ggmlv3 model only supports q4_0 quantization currently.
+
+
+## Pytorch Model Best Practices
+
+Pytorch has been integrated recently, and the usage scenarios are described below:
+
+### supported models
+- Foundation Model：baichuan（7B、13B）。
+- SFT Model：baichuan-chat（13B）、vicuna-v1.3（7B、13B、33B）。
+
+### supported devices
+- CUDA: On Linux and Windows systems, `cuda` device is used by default.
+- MPS: On Mac M1/M2 devices, `mps` device is used by default.
+- CPU: It is not recommended to use a `cpu` device, as it takes up a lot of memory and the inference speed is very slow.
+
+### quantization methods
+- `none`: indicates that no quantization is used.
+- `8-bit`: use 8-bit quantization.
+- `4-bit`: use 4-bit quantization. Note: 4-bit quantization is only supported on Linux systems and CUDA devices.
+
+### other instructions
+- On MacOS system, baichuan-chat model is not supported, and baichuan model cannot use 8-bit quantization.
+
+### use cases
+
+The table below shows memory usage and supported devices of some models.
+
+| Name          | Size (B) | OS    | No quantization (MB) | Quantization 8-bit (MB) | Quantization 4-bit (MB) |
+|---------------|----------|-------|----------------------|-------------------------|-------------------------|
+| baichuan-chat | 13       | linux | not currently tested | 13275                   | 7263                    |
+| baichuan-chat | 13       | macos | not supported        | not supported           | not supported           |
+| vicuna-v1.3   | 7        | linux | 12884                | 6708                    | 3620                    |
+| vicuna-v1.3   | 7        | macos | 12916                | 565                     | not supported           |
+| baichuan      | 7        | linux | 13480                | 7304                    | 4216                    |
+| baichuan      | 7        | macos | 13480                | not supported           | not supported           |
+
+
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
-### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
-within Xinference.
-
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: xinference Version: 0.0.6 Summary: Model Serving
+Metadata-Version: 2.1 Name: xinference Version: 0.1.0 Summary: Model Serving
 Made Easy Home-page: https://github.com/xorbitsai/inference Author: Qin Xuye
 Author-email: qinxuye@xprobe.io Maintainer: Qin Xuye Maintainer-email:
 qinxuye@xprobe.io License: Apache License 2.0 Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Topic :: Software Development :: Libraries Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: all Provides-
-Extra: doc License-File: LICENSE
+Extra: ggml Provides-Extra: pytorch Provides-Extra: doc License-File: LICENSE
   [xorbits] # Xorbits Inference: Model Serving Made Easy ð¤ [![PyPI Latest
   Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)]
 (https://pypi.org/project/xinference/) [![License](https://img.shields.io/pypi/
 l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/
   blob/main/LICENSE) [![Build Status](https://img.shields.io/github/actions/
   workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-
   badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/
@@ -25,15 +25,15 @@
                (README_zh_CN.md) | [æ¥æ¬èª](README_ja_JP.md)
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to
 serve language, speech recognition, and multimodal models. With Xorbits
 Inference, you can effortlessly deploy and serve your or state-of-the-art
 built-in models using just a single command. Whether you are a researcher,
 developer, or data scientist, Xorbits Inference empowers you to unleash the
-full potential of cutting-edge AI models. ![demo](assets/demo.gif)
+full potential of cutting-edge AI models.
                         ð_Join_our_Slack_community!
 ## Key Features ð **Model Serving Made Easy**: Simplify the process of
 serving large language, speech recognition, and multimodal models. You can set
 up and deploy your models for experimentation and production with a single
 command. â¡ï¸ **State-of-the-Art Models**: Experiment with cutting-edge
 built-in models using a single command. Inference provides access to state-of-
 the-art open-source models! ð¥ **Heterogeneous Hardware Utilization**: Make
@@ -45,82 +45,112 @@
 WebUI for seamless management and monitoring. ð **Distributed Deployment**:
 Excel in distributed deployment scenarios, allowing the seamless distribution
 of model inference across multiple devices or machines. ð **Built-in
 Integration with Third-Party Libraries**: Xorbits Inference seamlessly
 integrates with popular third-party libraries like LangChain and LlamaIndex.
 (Coming soon) ## Getting Started Xinference can be installed via pip from PyPI.
 It is highly recommended to create a new virtual environment to avoid
-conflicts. ```bash $ pip install "xinference[all]" ``` `xinference[all]`
-installs all the necessary packages for serving models. If you want to achieve
+conflicts. ### Installation ```bash $ pip install "xinference" ``` `xinference`
+installs basic packages for serving models. #### Installation with GGML To
+serve ggml models, you need to install the following extra dependencies:
+```bash $ pip install "xinference[ggml]" ``` If you want to achieve
 acceleration on different hardware, refer to the installation documentation of
 the corresponding package. - [llama-cpp-python](https://github.com/abetlen/
 llama-cpp-python#installation-from-pypi-recommended) is required to run
 `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`. - [chatglm-cpp-python]
 (https://github.com/li-plus/chatglm.cpp#getting-started) is required to run
-`chatglm` and `chatglm2`. ### Deployment You can deploy Xinference locally with
-a single command or deploy it in a distributed cluster. #### Local To start a
-local instance of Xinference, run the following command: ```bash $ xinference
-``` #### Distributed To deploy Xinference in a cluster, you need to start a
-Xinference supervisor on one server and Xinference workers on the other
-servers. Follow the steps below: **Starting the Supervisor**: On the server
-where you want to run the Xinference supervisor, run the following command:
-```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
+`chatglm` and `chatglm2`. #### Installation with PyTorch To serve PyTorch
+models, you need to install the following extra dependencies: ```bash $ pip
+install "xinference[pytorch]" ``` #### Installation with all dependencies If
+you want to serve all the supported models, install all the dependencies:
+```bash $ pip install "xinference[all]" ``` ### Deployment You can deploy
+Xinference locally with a single command or deploy it in a distributed cluster.
+#### Local To start a local instance of Xinference, run the following command:
+```bash $ xinference ``` #### Distributed To deploy Xinference in a cluster,
+you need to start a Xinference supervisor on one server and Xinference workers
+on the other servers. Follow the steps below: **Starting the Supervisor**: On
+the server where you want to run the Xinference supervisor, run the following
+command: ```bash $ xinference-supervisor -H "${supervisor_host}" ``` Replace `$
 {supervisor_host}` with the actual host of your supervisor server. **Starting
 the Workers**: On each of the other servers where you want to run Xinference
 workers, run the following command: ```bash $ xinference-worker -e "http://$
 {supervisor_host}:9997" ``` Once Xinference is running, an endpoint will be
 accessible for model management via CLI or Xinference client. - For local
 deployment, the endpoint will be `http://localhost:9997`. - For cluster
 deployment, the endpoint will be `http://${supervisor_host}:9997`, where `$
 {supervisor_host}` is the hostname or IP address of the server where the
 supervisor is running. You can also view a web UI using the Xinference endpoint
 to chat with all the builtin models. You can even **chat with two cutting-edge
 AI models side-by-side to compare their performance**! ![web UI](assets/
-xinference-downloading.png) ### Xinference CLI Xinference provides a command
-line interface (CLI) for model management. Here are some useful commands: -
-Launch a model (a model UID will be returned): `xinference launch` - List
-running models: `xinference list` - List all the builtin models: `xinference
-list --all` - Terminate a model: `xinference terminate --model-uid $
-{model_uid}` ### Xinference Client Xinference also provides a client for
-managing and accessing models programmatically: ```python from
-xinference.client import Client client = Client("http://localhost:9997")
-model_uid = client.launch_model(model_name="chatglm2") model = client.get_model
-(model_uid) chat_history = [] prompt = "What is the largest animal?" model.chat
-( prompt, chat_history, generate_config={"max_tokens": 1024} ) ``` Result:
-```json { "id": "chatcmpl-8d76b65a-bad0-42ef-912d-4a0533d90d61", "model":
-"56f69622-1e73-11ee-a3bd-9af9f16816c6", "object": "chat.completion", "created":
-1688919187, "choices": [ { "index": 0, "message": { "role": "assistant",
-"content": "The largest animal that has been scientifically measured is the
-blue whale, which has a maximum length of around 23 meters (75 feet) for adult
-animals and can weigh up to 150,000 pounds (68,000 kg). However, it is
-important to note that this is just an estimate and that the largest animal
-known to science may be larger still. Some scientists believe that the largest
-animals may not have a clear \"size\" in the same way that humans do, as their
-size can vary depending on the environment and the stage of their life." },
-"finish_reason": "None" } ], "usage": { "prompt_tokens": -1,
-"completion_tokens": -1, "total_tokens": -1 } } ``` See [examples](examples)
-for more examples. ## Builtin models To view the builtin models, run the
-following command: ```bash $ xinference list --all ``` | Name | Type | Language
-| Format | Size (in billions) | Quantization | |---------------|---------------
----|----------|---------|--------------------|---------------------------------
---------| | llama-2 | Foundation Model | en | ggmlv3 | 7, 13 | 'q2_K',
-'q3_K_L', ... , 'q6_K', 'q8_0' | | baichuan | Foundation Model | en, zh |
-ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | llama-2-chat | RLHF
+demo.gif) ### Xinference CLI Xinference provides a command line interface (CLI)
+for model management. Here are some useful commands: - Launch a model (a model
+UID will be returned): `xinference launch` - List running models: `xinference
+list` - List all the builtin models: `xinference list --all` - Terminate a
+model: `xinference terminate --model-uid ${model_uid}` ### Xinference Client
+Xinference also provides a client for managing and accessing models
+programmatically: ```python from xinference.client import Client client =
+Client("http://localhost:9997") model_uid = client.launch_model
+(model_name="chatglm2") model = client.get_model(model_uid) chat_history = []
+prompt = "What is the largest animal?" model.chat( prompt, chat_history,
+generate_config={"max_tokens": 1024} ) ``` Result: ```json { "id": "chatcmpl-
+8d76b65a-bad0-42ef-912d-4a0533d90d61", "model": "56f69622-1e73-11ee-a3bd-
+9af9f16816c6", "object": "chat.completion", "created": 1688919187, "choices":
+[ { "index": 0, "message": { "role": "assistant", "content": "The largest
+animal that has been scientifically measured is the blue whale, which has a
+maximum length of around 23 meters (75 feet) for adult animals and can weigh up
+to 150,000 pounds (68,000 kg). However, it is important to note that this is
+just an estimate and that the largest animal known to science may be larger
+still. Some scientists believe that the largest animals may not have a clear
+\"size\" in the same way that humans do, as their size can vary depending on
+the environment and the stage of their life." }, "finish_reason": "None" } ],
+"usage": { "prompt_tokens": -1, "completion_tokens": -1, "total_tokens": -1 } }
+``` See [examples](examples) for more examples. ## Builtin models To view the
+builtin models, run the following command: ```bash $ xinference list --all ```
+### ggmlv3 models | Name | Type | Language | Format | Size (in billions) |
+Quantization | |---------------|------------------|----------|---------|-------
+-------------|-----------------------------------------| | llama-2 | Foundation
 Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | |
-chatglm | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1',
-'q8_0' | | chatglm2 | SFT Model | en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0',
-'q5_1', 'q8_0' | | wizardlm-v1.0 | SFT Model | en | ggmlv3 | 7, 13, 33 |
-'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | wizardlm-v1.1 | SFT Model | en |
-ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | vicuna-v1.3 | SFT
-Model | en | ggmlv3 | 7, 13 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | orca |
-SFT Model | en | ggmlv3 | 3, 7, 13 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
-**NOTE**: - Xinference will download models automatically for you, and by
-default the models will be saved under `${USER}/.xinference/cache`. -
-Foundation models only provide interface `generate`. - RLHF and SFT models
-provide both `generate` and `chat`. - If you want to use Apple Metal GPU for
-acceleration, please choose the q4_0 and q4_1 quantization methods. ## Roadmap
-Xinference is currently under active development. Here's a roadmap outlining
-our planned developments for the next few weeks: ### PyTorch Support With
-PyTorch integration, users will be able to seamlessly utilize PyTorch models
-from Hugging Face within Xinference. ### Langchain & LlamaIndex integration
-With Xinference, it will be much easier for users to use these libraries and
-build applications with LLMs.
+baichuan | Foundation Model | en, zh | ggmlv3 | 7 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | llama-2-chat | RLHF Model | en | ggmlv3 | 7, 13, 70 |
+'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' | | chatglm | SFT Model | en, zh |
+ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | chatglm2 | SFT Model |
+en, zh | ggmlv3 | 6 | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | | wizardlm-v1.0
+| SFT Model | en | ggmlv3 | 7, 13, 33 | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0'
+| | wizardlm-v1.1 | SFT Model | en | ggmlv3 | 13 | 'q2_K', 'q3_K_L', ... ,
+'q6_K', 'q8_0' | | vicuna-v1.3 | SFT Model | en | ggmlv3 | 7, 13 | 'q2_K',
+'q3_K_L', ... , 'q6_K', 'q8_0' | | orca | SFT Model | en | ggmlv3 | 3, 7, 13 |
+'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' | ### pytorch models | Name | Type |
+Language | Format | Size (in billions) | Quantization | |---------------|------
+------------|----------|---------|--------------------|------------------------
+--| | baichuan | Foundation Model | en, zh | pytorch | 7, 13 | '4-bit', '8-
+bit', 'none' | | baichuan-chat | SFT Model | en, zh | pytorch | 13 | '4-bit',
+'8-bit', 'none' | | vicuna-v1.3 | SFT Model | en | pytorch | 7, 13, 33 | '4-
+bit', '8-bit', 'none' | **NOTE**: - Xinference will download models
+automatically for you, and by default the models will be saved under `$
+{USER}/.xinference/cache`. - Foundation models only provide interface
+`generate`. - RLHF and SFT models provide both `generate` and `chat`. - If you
+want to use Apple Metal GPU for acceleration, please choose the q4_0 and q4_1
+quantization methods. - `llama-2-chat` 70B ggmlv3 model only supports q4_0
+quantization currently. ## Pytorch Model Best Practices Pytorch has been
+integrated recently, and the usage scenarios are described below: ### supported
+models - Foundation Modelï¼baichuanï¼7Bã13Bï¼ã - SFT Modelï¼baichuan-
+chatï¼13Bï¼ãvicuna-v1.3ï¼7Bã13Bã33Bï¼ã ### supported devices -
+CUDA: On Linux and Windows systems, `cuda` device is used by default. - MPS: On
+Mac M1/M2 devices, `mps` device is used by default. - CPU: It is not
+recommended to use a `cpu` device, as it takes up a lot of memory and the
+inference speed is very slow. ### quantization methods - `none`: indicates that
+no quantization is used. - `8-bit`: use 8-bit quantization. - `4-bit`: use 4-
+bit quantization. Note: 4-bit quantization is only supported on Linux systems
+and CUDA devices. ### other instructions - On MacOS system, baichuan-chat model
+is not supported, and baichuan model cannot use 8-bit quantization. ### use
+cases The table below shows memory usage and supported devices of some models.
+| Name | Size (B) | OS | No quantization (MB) | Quantization 8-bit (MB) |
+Quantization 4-bit (MB) | |---------------|----------|-------|-----------------
+-----|-------------------------|-------------------------| | baichuan-chat | 13
+| linux | not currently tested | 13275 | 7263 | | baichuan-chat | 13 | macos |
+not supported | not supported | not supported | | vicuna-v1.3 | 7 | linux |
+12884 | 6708 | 3620 | | vicuna-v1.3 | 7 | macos | 12916 | 565 | not supported |
+| baichuan | 7 | linux | 13480 | 7304 | 4216 | | baichuan | 7 | macos | 13480 |
+not supported | not supported | ## Roadmap Xinference is currently under active
+development. Here's a roadmap outlining our planned developments for the next
+few weeks: ### Langchain & LlamaIndex integration With Xinference, it will be
+much easier for users to use these libraries and build applications with LLMs.
```

### Comparing `xinference-0.0.6/xinference.egg-info/SOURCES.txt` & `xinference-0.1.0/xinference.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,20 +32,22 @@
 xinference/deploy/utils.py
 xinference/deploy/worker.py
 xinference/deploy/test/__init__.py
 xinference/locale/__init__.py
 xinference/locale/utils.py
 xinference/locale/zh_CN.json
 xinference/model/__init__.py
+xinference/model/core.py
 xinference/model/llm/__init__.py
-xinference/model/llm/chatglm.py
 xinference/model/llm/core.py
-xinference/model/llm/llama2.py
-xinference/model/llm/orca.py
+xinference/model/llm/llm_family.json
+xinference/model/llm/llm_family.py
 xinference/model/llm/utils.py
-xinference/model/llm/vicuna.py
-xinference/model/llm/wizardlm.py
+xinference/model/llm/ggml/__init__.py
+xinference/model/llm/ggml/chatglm.py
+xinference/model/llm/ggml/llamacpp.py
 xinference/model/llm/pytorch/__init__.py
 xinference/model/llm/pytorch/baichuan.py
+xinference/model/llm/pytorch/compression.py
 xinference/model/llm/pytorch/core.py
 xinference/model/llm/pytorch/utils.py
 xinference/model/llm/pytorch/vicuna.py
```

