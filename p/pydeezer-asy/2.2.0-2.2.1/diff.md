# Comparing `tmp/pydeezer_asy-2.2.0.tar.gz` & `tmp/pydeezer_asy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-2.2.0.tar", last modified: Thu Jul 27 22:40:57 2023, max compression
+gzip compressed data, was "pydeezer_asy-2.2.1.tar", last modified: Thu Jul 27 22:47:22 2023, max compression
```

## Comparing `pydeezer_asy-2.2.0.tar` & `pydeezer_asy-2.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 22:40:57.296687 pydeezer_asy-2.2.0/
--rw-rw-rw-   0        0        0     1910 2023-07-27 22:40:57.294688 pydeezer_asy-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 22:40:56.747374 pydeezer_asy-2.2.0/deezer_asy/
--rw-rw-rw-   0        0        0    31178 2023-07-27 22:39:56.000000 pydeezer_asy-2.2.0/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.2.0/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 22:40:56.773304 pydeezer_asy-2.2.0/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.0/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.0/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-27 22:40:57.291696 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     1910 2023-07-27 22:40:56.000000 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-27 22:40:56.000000 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 22:40:56.000000 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-27 22:40:56.000000 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 22:40:56.000000 pydeezer_asy-2.2.0/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 22:40:57.296687 pydeezer_asy-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-27 22:40:50.000000 pydeezer_asy-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.361618 pydeezer_asy-2.2.1/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 22:47:22.360625 pydeezer_asy-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1546 2023-07-27 20:49:08.000000 pydeezer_asy-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.280835 pydeezer_asy-2.2.1/deezer_asy/
+-rw-rw-rw-   0        0        0    31178 2023-07-27 22:39:56.000000 pydeezer_asy-2.2.1/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      136 2023-07-27 18:53:44.000000 pydeezer_asy-2.2.1/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.312785 pydeezer_asy-2.2.1/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.1/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.1/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:47:22.359623 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     1910 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-27 22:47:22.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 22:47:21.000000 pydeezer_asy-2.2.1/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 22:47:22.361618 pydeezer_asy-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-07-27 22:47:15.000000 pydeezer_asy-2.2.1/setup.py
```

### Comparing `pydeezer_asy-2.2.0/PKG-INFO` & `pydeezer_asy-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer_asy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-2.2.0/README.md` & `pydeezer_asy-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/deezer_asy/DeezerAsy.py` & `pydeezer_asy-2.2.1/deezer_asy/DeezerAsy.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/deezer_asy/constants/api_methods.py` & `pydeezer_asy-2.2.1/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/deezer_asy/constants/track_formats.py` & `pydeezer_asy-2.2.1/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/deezer_asy/util.py` & `pydeezer_asy-2.2.1/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/pydeezer_asy.egg-info/PKG-INFO` & `pydeezer_asy-2.2.1/pydeezer_asy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer-asy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pydeezer_asy-2.2.0/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-2.2.1/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.0/setup.py` & `pydeezer_asy-2.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='2.2.0',
+    version='2.2.1',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
     install_requires=[
         "aiofiles",
         "cryptography",
         "mutagen",
         "httpx",
+        "httpx[http2]",
         "yarl",
         "asyncio"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
```

