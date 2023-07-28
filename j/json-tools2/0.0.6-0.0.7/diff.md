# Comparing `tmp/json-tools2-0.0.6.tar.gz` & `tmp/json-tools2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-tools2-0.0.6.tar", last modified: Tue Nov  2 20:49:36 2021, max compression
+gzip compressed data, was "json-tools2-0.0.7.tar", last modified: Fri Jul 28 09:36:51 2023, max compression
```

## Comparing `json-tools2-0.0.6.tar` & `json-tools2-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-11-02 20:49:36.000000 json-tools2-0.0.6/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2021-11-02 20:48:13.000000 json-tools2-0.0.6/setup.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       21 2021-10-05 22:07:19.000000 json-tools2-0.0.6/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2021-11-02 20:49:36.000000 json-tools2-0.0.6/setup.cfg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 20:48:05.000000 json-tools2-0.0.6/src/json_tools2/spark.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4525 2021-11-02 20:48:05.000000 json-tools2-0.0.6/src/json_tools2/schema.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.6/src/json_tools2/util.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       94 2021-11-02 20:48:05.000000 json-tools2-0.0.6/src/json_tools2/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.6/src/json_tools2/flat_json.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      374 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/top_level.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      406 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2021-11-02 20:49:36.000000 json-tools2-0.0.6/src/json_tools2.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      406 2021-11-02 20:49:36.000000 json-tools2-0.0.6/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.6/MANIFEST.in
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2021-11-02 20:49:36.000000 json-tools2-0.0.6/test/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3039 2021-10-05 22:07:19.000000 json-tools2-0.0.6/test/test_main.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.598134 json-tools2-0.0.7/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1067 2021-10-05 22:07:19.000000 json-tools2-0.0.7/LICENSE
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.7/MANIFEST.in
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3003 2023-07-28 09:36:51.598134 json-tools2-0.0.7/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2634 2023-07-28 09:29:32.000000 json-tools2-0.0.7/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-28 09:36:51.598134 json-tools2-0.0.7/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2023-07-28 09:29:41.000000 json-tools2-0.0.7/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.594134 json-tools2-0.0.7/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.594134 json-tools2-0.0.7/src/json_tools2/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       93 2023-07-28 07:36:36.000000 json-tools2-0.0.7/src/json_tools2/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.7/src/json_tools2/flat_json.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8295 2023-07-28 08:53:42.000000 json-tools2-0.0.7/src/json_tools2/schema.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 22:26:53.000000 json-tools2-0.0.7/src/json_tools2/spark.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.7/src/json_tools2/util.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.598134 json-tools2-0.0.7/src/json_tools2.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3003 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      364 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `json-tools2-0.0.6/setup.py` & `json-tools2-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="json-tools2",
-    version="0.0.6",
+    version="0.0.7",
     description="JSON Tools Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/json_tools2",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `json-tools2-0.0.6/src/json_tools2/spark.py` & `json-tools2-0.0.7/src/json_tools2/spark.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.6/src/json_tools2/util.py` & `json-tools2-0.0.7/src/json_tools2/util.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.6/src/json_tools2/flat_json.py` & `json-tools2-0.0.7/src/json_tools2/flat_json.py`

 * *Files identical despite different names*

