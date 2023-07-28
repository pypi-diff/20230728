# Comparing `tmp/cjptools-0.1.1.tar.gz` & `tmp/cjptools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjptools-0.1.1.tar", last modified: Fri Jul 28 07:08:42 2023, max compression
+gzip compressed data, was "cjptools-0.1.2.tar", last modified: Fri Jul 28 07:17:48 2023, max compression
```

## Comparing `cjptools-0.1.1.tar` & `cjptools-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 07:08:42.709087 cjptools-0.1.1/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      276 2023-07-28 07:08:42.709087 cjptools-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 07:08:42.687143 cjptools-0.1.1/cjptools/
--rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.1/cjptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:08:42.697090 cjptools-0.1.1/cjptools/printModules/
--rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.1/cjptools/printModules/__init__.py
--rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.1/cjptools/printModules/absPrinter.py
--rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.1/cjptools/printModules/printerCompose.py
--rw-rw-rw-   0        0        0      626 2022-10-13 16:20:01.000000 cjptools-0.1.1/cjptools/printModules/printers.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:08:42.707063 cjptools-0.1.1/cjptools/utils/
--rw-rw-rw-   0        0        0      167 2023-07-28 07:06:53.000000 cjptools-0.1.1/cjptools/utils/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.1/cjptools/utils/check.py
--rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.1/cjptools/utils/gpu_mem_track.py
--rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.1/cjptools/utils/modelsize_estimate.py
--rw-rw-rw-   0        0        0      505 2023-07-28 07:06:40.000000 cjptools-0.1.1/cjptools/utils/path.py
--rw-rw-rw-   0        0        0      768 2023-07-28 03:39:36.000000 cjptools-0.1.1/cjptools/utils/rnd.py
--rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.1/cjptools/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:08:42.692103 cjptools-0.1.1/cjptools.egg-info/
--rw-rw-rw-   0        0        0      276 2023-07-28 07:08:42.000000 cjptools-0.1.1/cjptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-07-28 07:08:42.000000 cjptools-0.1.1/cjptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 07:08:42.000000 cjptools-0.1.1/cjptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 07:08:42.000000 cjptools-0.1.1/cjptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 07:08:42.709087 cjptools-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-07-28 07:06:40.000000 cjptools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.330849 cjptools-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-07-28 07:17:48.330849 cjptools-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.309327 cjptools-0.1.2/cjptools/
+-rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.2/cjptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.319329 cjptools-0.1.2/cjptools/printModules/
+-rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/absPrinter.py
+-rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/printerCompose.py
+-rw-rw-rw-   0        0        0      626 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/printers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.329794 cjptools-0.1.2/cjptools/utils/
+-rw-rw-rw-   0        0        0      167 2023-07-28 07:06:53.000000 cjptools-0.1.2/cjptools/utils/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.2/cjptools/utils/check.py
+-rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.2/cjptools/utils/gpu_mem_track.py
+-rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.2/cjptools/utils/modelsize_estimate.py
+-rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.2/cjptools/utils/path.py
+-rw-rw-rw-   0        0        0      768 2023-07-28 03:39:36.000000 cjptools-0.1.2/cjptools/utils/rnd.py
+-rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.2/cjptools/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.314342 cjptools-0.1.2/cjptools.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 07:17:48.331823 cjptools-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-07-28 07:17:44.000000 cjptools-0.1.2/setup.py
```

### Comparing `cjptools-0.1.1/LICENSE` & `cjptools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.1/cjptools/printModules/printers.py` & `cjptools-0.1.2/cjptools/printModules/printers.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.1/cjptools/utils/gpu_mem_track.py` & `cjptools-0.1.2/cjptools/utils/gpu_mem_track.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.1/cjptools/utils/modelsize_estimate.py` & `cjptools-0.1.2/cjptools/utils/modelsize_estimate.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.1/cjptools/utils/rnd.py` & `cjptools-0.1.2/cjptools/utils/rnd.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.1/setup.py` & `cjptools-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="cjptools",
-    version="0.1.1",
+    version="0.1.2",
     keywords=("database", "localServer"),
     description="My Personal Toolkit",
     long_description="My Personal Toolkit",
     license="MIT Licence",
     author="Cai Jianping",
     author_email="jpingcai@163.com",
```

