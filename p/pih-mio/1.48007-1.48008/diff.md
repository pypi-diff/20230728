# Comparing `tmp/pih_mio-1.48007.tar.gz` & `tmp/pih-mio-1.48008.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48007.tar", last modified: Fri Jul 28 12:34:59 2023, max compression
+gzip compressed data, was "pih-mio-1.48008.tar", last modified: Fri Jul 28 12:43:48 2023, max compression
```

## Comparing `pih_mio-1.48007.tar` & `pih-mio-1.48008.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.041710 pih_mio-1.48007/
-drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.088067 pih_mio-1.48007/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48007/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-28 12:15:46.000000 pih_mio-1.48007/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48007/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      827 2023-07-28 12:17:34.000000 pih_mio-1.48007/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48007/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48007/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 12:34:59.562070 pih_mio-1.48007/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.530821 pih_mio-1.48007/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1626 2023-07-28 12:34:27.000000 pih_mio-1.48007/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 12:34:59.562070 pih_mio-1.48007/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 12:43:47.637864 pih-mio-1.48008/
+drwxrwxrwx   0        0        0        0 2023-07-28 12:43:47.684736 pih-mio-1.48008/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48008/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-07-28 12:42:54.000000 pih-mio-1.48008/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48008/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48008/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih-mio-1.48008/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48008/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:43:48.190597 pih-mio-1.48008/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 12:43:48.143725 pih-mio-1.48008/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48008/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:43:48.190597 pih-mio-1.48008/setup.cfg
```

### Comparing `pih_mio-1.48007/MobileHelperCore/api.py` & `pih-mio-1.48008/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48007/MobileHelperCore/service_api.py` & `pih-mio-1.48008/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48007/MobileHelperCore/tools.py` & `pih-mio-1.48008/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48007/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48008/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48007/pih_mio_setup.py` & `pih-mio-1.48008/pih_mio_setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,20 +24,20 @@
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
-name: str = j((PIH.NAME, PIH.MIO.NAME), "_")
+name: str = j((PIH.NAME, PIH.MIO.NAME), "-")
 setup(
     name=name,
     entry_points={
         "console_scripts": [
-            f"{name}=__main__:main",
+            f"{name}=MobileHelperCore.__main__:start",
         ]
     },
     version=PIH.VERSION.MIO.local(),
     description="PIH Mobile Helper library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
```

