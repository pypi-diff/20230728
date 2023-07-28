# Comparing `tmp/efpy-0.1.4.tar.gz` & `tmp/efpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.4.tar", last modified: Wed Jul 26 14:11:53 2023, max compression
+gzip compressed data, was "efpy-0.1.5.tar", last modified: Fri Jul 28 04:11:34 2023, max compression
```

## Comparing `efpy-0.1.4.tar` & `efpy-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/
--rw-rw-rw-   0        0        0      255 2023-07-26 14:11:53.704205 efpy-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/efpy/
--rw-rw-rw-   0        0        0     1106 2023-07-26 14:10:32.000000 efpy-0.1.4/efpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.4/efpy/env.py
--rw-rw-rw-   0        0        0     2723 2023-07-26 13:58:57.000000 efpy-0.1.4/efpy/expHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:11:53.704205 efpy-0.1.4/efpy.egg-info/
--rw-rw-rw-   0        0        0      255 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 14:11:53.000000 efpy-0.1.4/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:11:53.704205 efpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-26 14:11:45.000000 efpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:11:34.498997 efpy-0.1.5/
+-rw-rw-rw-   0        0        0      255 2023-07-28 04:11:34.498008 efpy-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 04:11:34.488166 efpy-0.1.5/efpy/
+-rw-rw-rw-   0        0        0     1106 2023-07-26 14:10:32.000000 efpy-0.1.5/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.5/efpy/env.py
+-rw-rw-rw-   0        0        0     3021 2023-07-28 04:11:00.000000 efpy-0.1.5/efpy/expHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:11:34.496979 efpy-0.1.5/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-07-28 04:11:34.000000 efpy-0.1.5/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-28 04:11:34.000000 efpy-0.1.5/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:11:34.000000 efpy-0.1.5/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 04:11:34.000000 efpy-0.1.5/efpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 04:11:34.000000 efpy-0.1.5/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:11:34.498997 efpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-28 04:11:19.000000 efpy-0.1.5/setup.py
```

### Comparing `efpy-0.1.4/efpy/__init__.py` & `efpy-0.1.5/efpy/__init__.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.4/efpy/env.py` & `efpy-0.1.5/efpy/env.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.4/efpy/expHelper.py` & `efpy-0.1.5/efpy/expHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,18 +72,25 @@
         return None;
     dyConfig = dyConfig[activeDynamicYamlId]
     dictConv(dyConfig, varSettings)
     dictConv(theConfig, dyConfig)
     return theConfig, dyConfig
 
 
+def loadSettingFromYamlSimple(backgroundYamlFile, varSettings={}):
+    with open(backgroundYamlFile, 'r', encoding='utf-8') as c:
+        defConfigs = list(yaml.load_all(c, Loader=yaml.FullLoader))
+        theConfig = defConfigs[0]
+    dictConv(theConfig, varSettings)
+    return theConfig
+
+
 def removeNoneSetting(param):
     rmKeys = []
     for key1 in param:
         val = param[key1]
         if val is None:
             rmKeys.append(key1)
         elif isinstance(val, dict):
             removeNoneSetting(val);
     for key1 in rmKeys:
         del param[key1]
-
```

### Comparing `efpy-0.1.4/setup.py` & `efpy-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "efpy",
-    version = "0.1.4",
+    version = "0.1.5",
     keywords = ("experience","environment"),
     description = "experience",
     long_description = "experience",
     license = "MIT Licence",
 
     url = "https://github.com/imcjp/efpy",
     author = "Cai Jianping",
```

