# Comparing `tmp/maxsmart-0.1.8.tar.gz` & `tmp/maxsmart-0.1.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxsmart-0.1.8.tar", last modified: Tue Jul 25 06:32:33 2023, max compression
+gzip compressed data, was "maxsmart-0.1.9b0.tar", last modified: Fri Jul 28 16:40:42 2023, max compression
```

## Comparing `maxsmart-0.1.8.tar` & `maxsmart-0.1.9b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.8/LICENSE
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-07-25 06:32:33.608309 maxsmart-0.1.8/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     7581 2023-06-22 20:20:51.000000 maxsmart-0.1.8/README.md
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/maxsmart/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.8/maxsmart/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5134 2023-07-25 06:30:30.000000 maxsmart-0.1.8/maxsmart/maxsmart.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/maxsmart.egg-info/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/SOURCES.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/dependency_links.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/requires.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/top_level.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-07-25 06:32:33.608309 maxsmart-0.1.8/setup.cfg
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-07-25 06:19:57.000000 maxsmart-0.1.8/setup.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/tests/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.8/tests/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.8/tests/test_maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-28 16:40:42.376590 maxsmart-0.1.9b0/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.9b0/LICENSE
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      848 2023-07-28 16:40:42.373257 maxsmart-0.1.9b0/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     7581 2023-06-22 20:20:51.000000 maxsmart-0.1.9b0/README.md
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-28 16:40:42.373257 maxsmart-0.1.9b0/maxsmart/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.9b0/maxsmart/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5135 2023-07-28 16:39:06.000000 maxsmart-0.1.9b0/maxsmart/maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-28 16:40:42.373257 maxsmart-0.1.9b0/maxsmart.egg-info/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      848 2023-07-28 16:40:42.000000 maxsmart-0.1.9b0/maxsmart.egg-info/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-07-28 16:40:42.000000 maxsmart-0.1.9b0/maxsmart.egg-info/SOURCES.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-07-28 16:40:42.000000 maxsmart-0.1.9b0/maxsmart.egg-info/dependency_links.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-07-28 16:40:42.000000 maxsmart-0.1.9b0/maxsmart.egg-info/requires.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-07-28 16:40:42.000000 maxsmart-0.1.9b0/maxsmart.egg-info/top_level.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-07-28 16:40:42.376590 maxsmart-0.1.9b0/setup.cfg
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1015 2023-07-28 16:40:21.000000 maxsmart-0.1.9b0/setup.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-28 16:40:42.373257 maxsmart-0.1.9b0/tests/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.9b0/tests/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.9b0/tests/test_maxsmart.py
```

### Comparing `maxsmart-0.1.8/LICENSE` & `maxsmart-0.1.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.8/PKG-INFO` & `maxsmart-0.1.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.8
+Version: 0.1.9b0
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.8/README.md` & `maxsmart-0.1.9b0/README.md`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.8/maxsmart/maxsmart.py` & `maxsmart-0.1.9b0/maxsmart/maxsmart.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                         }
 
                         maxsmart_devices.append(maxsmart_device)
 
                 except socket.timeout:
                     break
 
-        MaxSmartDiscovery._validate_firmware_versions(maxsmart_devices)
+#        MaxSmartDiscovery._validate_firmware_versions(maxsmart_devices)
 
         return maxsmart_devices
 
     @staticmethod
     def _validate_firmware_versions(devices):
         for device in devices:
             firmware_version = device.get('ver')
```

### Comparing `maxsmart-0.1.8/maxsmart.egg-info/PKG-INFO` & `maxsmart-0.1.9b0/maxsmart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.8
+Version: 0.1.9b0
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.8/setup.py` & `maxsmart-0.1.9b0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='maxsmart',
-    version='0.1.8',
+    version='0.1.9b',
     author='Akim Sissaoui',
     author_email='superkikim@sissaoui.com',
     description='A Python module for operating network connected power strips',
     long_description='''A Python module for operating network connected power strips.
                         It provides functionality to turn on/off sockets, check their state, and retrieve power consumption data.''',
     url='https://github.com/superkikim/maxsmart',
     packages=find_packages(),
```

### Comparing `maxsmart-0.1.8/tests/test_maxsmart.py` & `maxsmart-0.1.9b0/tests/test_maxsmart.py`

 * *Files identical despite different names*

