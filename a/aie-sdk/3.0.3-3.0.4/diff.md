# Comparing `tmp/aie-sdk-3.0.3.tar.gz` & `tmp/aie-sdk-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-3.0.3.tar", last modified: Thu Jul 13 08:32:40 2023, max compression
+gzip compressed data, was "aie-sdk-3.0.4.tar", last modified: Fri Jul 28 05:53:26 2023, max compression
```

## Comparing `aie-sdk-3.0.3.tar` & `aie-sdk-3.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.605948 aie-sdk-3.0.3/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 08:32:40.605464 aie-sdk-3.0.3/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.3/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.600265 aie-sdk-3.0.3/aie/
--rw-r--r--   0 songci     (502) staff       (20)      249 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)       31 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/auth.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.600883 aie-sdk-3.0.3/aie/client/
--rw-r--r--   0 songci     (502) staff       (20)       35 2023-07-13 03:57:55.000000 aie-sdk-3.0.3/aie/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)       30 2023-07-13 04:09:28.000000 aie-sdk-3.0.3/aie/env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.601462 aie-sdk-3.0.3/aie/error/
--rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 03:58:55.000000 aie-sdk-3.0.3/aie/error/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 04:09:38.000000 aie-sdk-3.0.3/aie/g_var.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-13 08:32:40.604627 aie-sdk-3.0.3/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      454 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      269 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)      248 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-07-13 08:32:40.000000 aie-sdk-3.0.3/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-13 08:32:40.606085 aie-sdk-3.0.3/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.3/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 05:53:26.920631 aie-sdk-3.0.4/
+-rw-r--r--   0 songci     (502) staff       (20)      475 2023-07-28 05:53:26.920164 aie-sdk-3.0.4/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.4/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 05:53:26.915485 aie-sdk-3.0.4/aie/
+-rw-r--r--   0 songci     (502) staff       (20)      249 2023-07-28 05:52:13.000000 aie-sdk-3.0.4/aie/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       31 2023-07-13 04:09:28.000000 aie-sdk-3.0.4/aie/auth.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 05:53:26.915982 aie-sdk-3.0.4/aie/client/
+-rw-r--r--   0 songci     (502) staff       (20)       35 2023-07-13 03:57:55.000000 aie-sdk-3.0.4/aie/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       30 2023-07-13 04:09:28.000000 aie-sdk-3.0.4/aie/env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 05:53:26.916461 aie-sdk-3.0.4/aie/error/
+-rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 03:58:55.000000 aie-sdk-3.0.4/aie/error/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)       32 2023-07-13 04:09:38.000000 aie-sdk-3.0.4/aie/g_var.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 05:53:26.919560 aie-sdk-3.0.4/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      475 2023-07-28 05:53:26.000000 aie-sdk-3.0.4/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      269 2023-07-28 05:53:26.000000 aie-sdk-3.0.4/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-28 05:53:26.000000 aie-sdk-3.0.4/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)      304 2023-07-28 05:53:26.000000 aie-sdk-3.0.4/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-07-28 05:53:26.000000 aie-sdk-3.0.4/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-28 05:53:26.920807 aie-sdk-3.0.4/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1178 2023-07-28 05:49:32.000000 aie-sdk-3.0.4/setup.py
```

### Comparing `aie-sdk-3.0.3/setup.py` & `aie-sdk-3.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 # print("packages:", packages)
 setup(
     name="aie-sdk",
     version=__version__,
     description="AIEarth Engine Python SDK",
     url="https://engine-aiearth.aliyun.com/",
     packages=packages,
-    python_requires=">=3.5.0",
+    python_requires=">=3.8.0",
     install_requires=requirements,
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     extras_require={
-        "engine": ["aiearth-core", "aie-ipyleaflet", "aiearth-engine", "notebook<7"],
-        "openapi": ["aiearth-openapi>=1.0.0", "alibabacloud-aiearth-engine20220609>=1.0.5"]
+        "engine": ["aiearth-core", "aie-ipyleaflet", "aiearth-engine", "notebook<7", "aie-sdk>=3.0.3"],
+        "openapi": ["aiearth-openapi>=1.1.0", "alibabacloud-aiearth-engine20220609>=1.0.6"],
+        "data": ["aiearth-core>=1.0.1", "aiearth-data"]
     }
 )
```

