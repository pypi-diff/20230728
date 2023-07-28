# Comparing `tmp/pih_mio-1.48006.tar.gz` & `tmp/pih_mio-1.48007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48006.tar", last modified: Fri Jul 28 12:18:11 2023, max compression
+gzip compressed data, was "pih_mio-1.48007.tar", last modified: Fri Jul 28 12:34:59 2023, max compression
```

## Comparing `pih_mio-1.48006.tar` & `pih_mio-1.48007.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:18:10.737520 pih_mio-1.48006/
-drwxrwxrwx   0        0        0        0 2023-07-28 12:18:11.018764 pih_mio-1.48006/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48006/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-28 12:15:46.000000 pih_mio-1.48006/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48006/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      827 2023-07-28 12:17:34.000000 pih_mio-1.48006/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48006/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48006/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 12:18:11.237510 pih_mio-1.48006/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 12:18:11.159389 pih_mio-1.48006/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 12:18:09.000000 pih_mio-1.48006/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-07-28 12:18:10.000000 pih_mio-1.48006/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:18:09.000000 pih_mio-1.48006/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 12:18:10.000000 pih_mio-1.48006/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 12:18:10.000000 pih_mio-1.48006/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48006/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 12:18:11.237510 pih_mio-1.48006/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.041710 pih_mio-1.48007/
+drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.088067 pih_mio-1.48007/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48007/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-28 12:15:46.000000 pih_mio-1.48007/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48007/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      827 2023-07-28 12:17:34.000000 pih_mio-1.48007/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48007/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48007/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:34:59.562070 pih_mio-1.48007/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 12:34:59.530821 pih_mio-1.48007/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 12:34:58.000000 pih_mio-1.48007/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1626 2023-07-28 12:34:27.000000 pih_mio-1.48007/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:34:59.562070 pih_mio-1.48007/setup.cfg
```

### Comparing `pih_mio-1.48006/MobileHelperCore/api.py` & `pih_mio-1.48007/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48006/MobileHelperCore/service.py` & `pih_mio-1.48007/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48006/MobileHelperCore/service_api.py` & `pih_mio-1.48007/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48006/MobileHelperCore/tools.py` & `pih_mio-1.48007/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48006/pih_mio_setup.py` & `pih_mio-1.48007/pih_mio_setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,16 +24,22 @@
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
+name: str = j((PIH.NAME, PIH.MIO.NAME), "_")
 setup(
-    name=j((PIH.NAME, PIH.MIO.NAME), "_"),
+    name=name,
+    entry_points={
+        "console_scripts": [
+            f"{name}=__main__:main",
+        ]
+    },
     version=PIH.VERSION.MIO.local(),
     description="PIH Mobile Helper library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
```

