# Comparing `tmp/http_cat_utils-0.1.tar.gz` & `tmp/http_cat_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_cat_utils-0.1.tar", last modified: Fri Jul 28 15:06:44 2023, max compression
+gzip compressed data, was "http_cat_utils-0.2.tar", last modified: Fri Jul 28 15:43:08 2023, max compression
```

## Comparing `http_cat_utils-0.1.tar` & `http_cat_utils-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 15:06:44.439677 http_cat_utils-0.1/
--rw-rw-rw-   0        0        0     1086 2023-07-28 14:19:37.000000 http_cat_utils-0.1/LICENSE
--rw-rw-rw-   0        0        0      836 2023-07-28 15:06:44.438676 http_cat_utils-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2023-07-28 14:53:54.000000 http_cat_utils-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 15:06:44.429677 http_cat_utils-0.1/http_cat/
--rw-rw-rw-   0        0        0     1568 2023-07-28 14:13:31.000000 http_cat_utils-0.1/http_cat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:06:44.437677 http_cat_utils-0.1/http_cat_utils.egg-info/
--rw-rw-rw-   0        0        0      836 2023-07-28 15:06:44.000000 http_cat_utils-0.1/http_cat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-28 15:06:44.000000 http_cat_utils-0.1/http_cat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 15:06:44.000000 http_cat_utils-0.1/http_cat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 15:06:44.000000 http_cat_utils-0.1/http_cat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 15:06:44.000000 http_cat_utils-0.1/http_cat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 15:06:44.439677 http_cat_utils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-07-28 15:06:20.000000 http_cat_utils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:43:08.096945 http_cat_utils-0.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-28 14:19:37.000000 http_cat_utils-0.2/LICENSE
+-rw-rw-rw-   0        0        0     2398 2023-07-28 15:43:08.096945 http_cat_utils-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2023-07-28 14:53:54.000000 http_cat_utils-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 15:43:08.088945 http_cat_utils-0.2/http_cat/
+-rw-rw-rw-   0        0        0     1568 2023-07-28 14:13:31.000000 http_cat_utils-0.2/http_cat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:43:08.095945 http_cat_utils-0.2/http_cat_utils.egg-info/
+-rw-rw-rw-   0        0        0     2398 2023-07-28 15:43:07.000000 http_cat_utils-0.2/http_cat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-28 15:43:07.000000 http_cat_utils-0.2/http_cat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 15:43:07.000000 http_cat_utils-0.2/http_cat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 15:43:07.000000 http_cat_utils-0.2/http_cat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 15:43:07.000000 http_cat_utils-0.2/http_cat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 15:43:08.097945 http_cat_utils-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-07-28 15:40:55.000000 http_cat_utils-0.2/setup.py
```

### Comparing `http_cat_utils-0.1/LICENSE` & `http_cat_utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `http_cat_utils-0.1/README.md` & `http_cat_utils-0.2/README.md`

 * *Files identical despite different names*

### Comparing `http_cat_utils-0.1/http_cat/__init__.py` & `http_cat_utils-0.2/http_cat/__init__.py`

 * *Files identical despite different names*

### Comparing `http_cat_utils-0.1/setup.py` & `http_cat_utils-0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from setuptools import setup
 
+# 从README.md文件中读取长描述
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
 setup(
     name="http_cat_utils",
-    version="0.1",
+    version="0.2",
     author="cacaview",
     author_email="cacaview@foxmail.com",
     description="A simple httpcat call function returns image data when called",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     license="MIT",
     packages=["http_cat"],
     install_requires=["requests"],
     url="https://github.com/cacaview/http_cat",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

