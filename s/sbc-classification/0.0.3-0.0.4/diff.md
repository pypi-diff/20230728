# Comparing `tmp/sbc-classification-0.0.3.tar.gz` & `tmp/sbc-classification-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbc-classification-0.0.3.tar", last modified: Fri Jul 28 02:32:52 2023, max compression
+gzip compressed data, was "sbc-classification-0.0.4.tar", last modified: Fri Jul 28 03:07:45 2023, max compression
```

## Comparing `sbc-classification-0.0.3.tar` & `sbc-classification-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 02:32:52.911972 sbc-classification-0.0.3/
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     1067 2023-07-27 22:08:52.000000 sbc-classification-0.0.3/LICENSE
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2440 2023-07-28 02:32:52.911452 sbc-classification-0.0.3/PKG-INFO
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2076 2023-07-28 02:23:00.000000 sbc-classification-0.0.3/README.md
-drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 02:32:52.896010 sbc-classification-0.0.3/sbc/
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504        0 2023-07-21 17:58:45.000000 sbc-classification-0.0.3/sbc/__init__.py
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     4390 2023-07-28 00:52:42.000000 sbc-classification-0.0.3/sbc/sbc_class.py
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     3263 2023-07-21 17:58:45.000000 sbc-classification-0.0.3/sbc/util.py
-drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 02:32:52.902444 sbc-classification-0.0.3/sbc_classification.egg-info/
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2440 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/PKG-INFO
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504      362 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/SOURCES.txt
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504        1 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/dependency_links.txt
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504        1 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/not-zip-safe
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504       46 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/requires.txt
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504       10 2023-07-28 02:32:52.000000 sbc-classification-0.0.3/sbc_classification.egg-info/top_level.txt
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504       38 2023-07-28 02:32:52.912121 sbc-classification-0.0.3/setup.cfg
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504      869 2023-07-28 02:32:02.000000 sbc-classification-0.0.3/setup.py
-drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 02:32:52.910487 sbc-classification-0.0.3/tests/
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504        0 2023-07-21 17:58:45.000000 sbc-classification-0.0.3/tests/__init__.py
--rw-r--r--   0 thunguyen6 (1100182655) 1244544504     1060 2023-07-21 17:58:45.000000 sbc-classification-0.0.3/tests/test_SBCclass.py
+drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 03:07:45.442892 sbc-classification-0.0.4/
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     1067 2023-07-27 22:08:52.000000 sbc-classification-0.0.4/LICENSE
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2502 2023-07-28 03:07:45.442382 sbc-classification-0.0.4/PKG-INFO
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2076 2023-07-28 02:23:00.000000 sbc-classification-0.0.4/README.md
+drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 03:07:45.397772 sbc-classification-0.0.4/sbc/
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504        0 2023-07-21 17:58:45.000000 sbc-classification-0.0.4/sbc/__init__.py
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     4390 2023-07-28 00:52:42.000000 sbc-classification-0.0.4/sbc/sbc_class.py
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     3263 2023-07-21 17:58:45.000000 sbc-classification-0.0.4/sbc/util.py
+drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 03:07:45.434450 sbc-classification-0.0.4/sbc_classification.egg-info/
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     2502 2023-07-28 03:07:44.000000 sbc-classification-0.0.4/sbc_classification.egg-info/PKG-INFO
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504      362 2023-07-28 03:07:44.000000 sbc-classification-0.0.4/sbc_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504        1 2023-07-28 03:07:44.000000 sbc-classification-0.0.4/sbc_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504        1 2023-07-28 02:32:52.000000 sbc-classification-0.0.4/sbc_classification.egg-info/not-zip-safe
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504       46 2023-07-28 03:07:44.000000 sbc-classification-0.0.4/sbc_classification.egg-info/requires.txt
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504       10 2023-07-28 03:07:44.000000 sbc-classification-0.0.4/sbc_classification.egg-info/top_level.txt
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504       38 2023-07-28 03:07:45.443016 sbc-classification-0.0.4/setup.cfg
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504      933 2023-07-28 03:06:59.000000 sbc-classification-0.0.4/setup.py
+drwxr-xr-x   0 thunguyen6 (1100182655) 1244544504        0 2023-07-28 03:07:45.441558 sbc-classification-0.0.4/tests/
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504        0 2023-07-21 17:58:45.000000 sbc-classification-0.0.4/tests/__init__.py
+-rw-r--r--   0 thunguyen6 (1100182655) 1244544504     1060 2023-07-21 17:58:45.000000 sbc-classification-0.0.4/tests/test_SBCclass.py
```

### Comparing `sbc-classification-0.0.3/LICENSE` & `sbc-classification-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sbc-classification-0.0.3/PKG-INFO` & `sbc-classification-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sbc-classification
-Version: 0.0.3
+Version: 0.0.4
 Summary: Demand Patterns SBC (Syntetos, Boylan, Croston) method of Categorizations
+Home-page: https://github.com/tqn14/SBC_classification_python
 Author: Thu Nguyen
 Author-email: tqn1472@gmail.com
 License: MIT License
 Keywords: python,demand patterns,sbc classification,croston,idclass,tsintermittent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sbc-classification-0.0.3/README.md` & `sbc-classification-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sbc-classification-0.0.3/sbc/sbc_class.py` & `sbc-classification-0.0.4/sbc/sbc_class.py`

 * *Files identical despite different names*

### Comparing `sbc-classification-0.0.3/sbc/util.py` & `sbc-classification-0.0.4/sbc/util.py`

 * *Files identical despite different names*

### Comparing `sbc-classification-0.0.3/sbc_classification.egg-info/PKG-INFO` & `sbc-classification-0.0.4/sbc_classification.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sbc-classification
-Version: 0.0.3
+Version: 0.0.4
 Summary: Demand Patterns SBC (Syntetos, Boylan, Croston) method of Categorizations
+Home-page: https://github.com/tqn14/SBC_classification_python
 Author: Thu Nguyen
 Author-email: tqn1472@gmail.com
 License: MIT License
 Keywords: python,demand patterns,sbc classification,croston,idclass,tsintermittent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sbc-classification-0.0.3/setup.py` & `sbc-classification-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(name='sbc-classification',
-      version='0.0.3',
+      version='0.0.4',
       description='Demand Patterns SBC (Syntetos, Boylan, Croston) method of Categorizations',
       author='Thu Nguyen',
       author_email='tqn1472@gmail.com',
       license='MIT License',
       long_description_content_type='text/markdown',
       long_description=open('README.md').read(),
+      url="https://github.com/tqn14/SBC_classification_python",
       packages=find_packages(),
       install_requires=[
           'pandas >= 1.5.3',
           'numpy >= 1.24.4',
           'matplotlib >= 3.7.2'
       ],
       test_suite='tests',
```

### Comparing `sbc-classification-0.0.3/tests/test_SBCclass.py` & `sbc-classification-0.0.4/tests/test_SBCclass.py`

 * *Files identical despite different names*

