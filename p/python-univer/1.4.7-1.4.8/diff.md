# Comparing `tmp/python-univer-1.4.7.tar.gz` & `tmp/python-univer-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-univer-1.4.7.tar", last modified: Tue Jul 25 23:51:25 2023, max compression
+gzip compressed data, was "python-univer-1.4.8.tar", last modified: Fri Jul 28 06:37:53 2023, max compression
```

## Comparing `python-univer-1.4.7.tar` & `python-univer-1.4.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-25 23:51:25.849998 python-univer-1.4.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.7/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.846664 python-univer-1.4.7/python_univer.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      732 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-25 23:51:25.849998 python-univer-1.4.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      891 2023-07-25 23:51:12.000000 python-univer-1.4.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/config.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/models/
--rw-r--r--   0 user      (1000) user      (1001)      225 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)     9276 2023-07-25 23:49:51.000000 python-univer-1.4.7/univer_db/models/base.py
--rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/dormitories.py
--rw-r--r--   0 user      (1000) user      (1001)     1888 2023-07-25 23:43:54.000000 python-univer-1.4.7/univer_db/models/geo.py
--rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/grades.py
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/groups.py
--rw-r--r--   0 user      (1000) user      (1001)    35417 2023-07-25 23:50:41.000000 python-univer-1.4.7/univer_db/models/models.py
--rw-r--r--   0 user      (1000) user      (1001)     9229 2023-07-25 23:49:39.000000 python-univer-1.4.7/univer_db/models/orders.py
--rw-r--r--   0 user      (1000) user      (1001)    25491 2023-07-25 23:48:54.000000 python-univer-1.4.7/univer_db/models/roles.py
--rw-r--r--   0 user      (1000) user      (1001)     4194 2023-07-25 23:48:54.000000 python-univer-1.4.7/univer_db/models/schedule.py
--rw-r--r--   0 user      (1000) user      (1001)     3573 2023-07-25 23:48:09.000000 python-univer-1.4.7/univer_db/models/sheets.py
--rw-r--r--   0 user      (1000) user      (1001)     5071 2023-07-25 23:46:52.000000 python-univer-1.4.7/univer_db/models/structures.py
--rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/tests/
--rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/geo.py
--rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/models.py
--rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/roles.py
--rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/structures.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.146666 python-univer-1.4.8/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-28 06:37:53.146666 python-univer-1.4.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.8/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.116666 python-univer-1.4.8/python_univer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)     1231 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      765 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-28 06:37:52.000000 python-univer-1.4.8/python_univer.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-28 06:37:53.146666 python-univer-1.4.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      827 2023-07-28 06:37:05.000000 python-univer-1.4.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.119999 python-univer-1.4.8/univer_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/config.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.143333 python-univer-1.4.8/univer_db/models/
+-rw-r--r--   0 user      (1000) user      (1001)      253 2023-07-28 06:36:00.000000 python-univer-1.4.8/univer_db/models/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)     9276 2023-07-25 23:49:51.000000 python-univer-1.4.8/univer_db/models/base.py
+-rw-r--r--   0 user      (1000) user      (1001)     4523 2023-07-28 06:35:35.000000 python-univer-1.4.8/univer_db/models/certificates.py
+-rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/dormitories.py
+-rw-r--r--   0 user      (1000) user      (1001)     1888 2023-07-25 23:43:54.000000 python-univer-1.4.8/univer_db/models/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/grades.py
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/models/groups.py
+-rw-r--r--   0 user      (1000) user      (1001)    35417 2023-07-25 23:50:41.000000 python-univer-1.4.8/univer_db/models/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     9229 2023-07-25 23:49:39.000000 python-univer-1.4.8/univer_db/models/orders.py
+-rw-r--r--   0 user      (1000) user      (1001)    25491 2023-07-25 23:48:54.000000 python-univer-1.4.8/univer_db/models/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)     4194 2023-07-25 23:48:54.000000 python-univer-1.4.8/univer_db/models/schedule.py
+-rw-r--r--   0 user      (1000) user      (1001)     3573 2023-07-25 23:48:09.000000 python-univer-1.4.8/univer_db/models/sheets.py
+-rw-r--r--   0 user      (1000) user      (1001)     5071 2023-07-25 23:46:52.000000 python-univer-1.4.8/univer_db/models/structures.py
+-rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-28 06:37:53.143333 python-univer-1.4.8/univer_db/tests/
+-rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.8/univer_db/tests/structures.py
```

### Comparing `python-univer-1.4.7/PKG-INFO` & `python-univer-1.4.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.7
-Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
+Version: 1.4.8
+Summary: Данная библиотека содержит SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `python-univer-1.4.7/README.md` & `python-univer-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/python_univer.egg-info/PKG-INFO` & `python-univer-1.4.8/python_univer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.7
-Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
+Version: 1.4.8
+Summary: Данная библиотека содержит SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `python-univer-1.4.7/python_univer.egg-info/SOURCES.txt` & `python-univer-1.4.8/python_univer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 python_univer.egg-info/requires.txt
 python_univer.egg-info/top_level.txt
 univer_db/__init__.py
 univer_db/config.py
 univer_db/orm.py
 univer_db/models/__init__.py
 univer_db/models/base.py
+univer_db/models/certificates.py
 univer_db/models/dormitories.py
 univer_db/models/geo.py
 univer_db/models/grades.py
 univer_db/models/groups.py
 univer_db/models/models.py
 univer_db/models/orders.py
 univer_db/models/roles.py
```

### Comparing `python-univer-1.4.7/setup.py` & `python-univer-1.4.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-"""
-Модуль установки библиотеки
-"""
-
 import setuptools
 
 with open('README.md', 'r', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-univer",
-    version="1.4.7",
+    version="1.4.8",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
-    description="Данная библиотека содержить SqlAlchemy ORM для системы Univer",
+    description="Данная библиотека содержит SqlAlchemy ORM для системы Univer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_univer",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
```

### Comparing `python-univer-1.4.7/univer_db/models/base.py` & `python-univer-1.4.8/univer_db/models/base.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/dormitories.py` & `python-univer-1.4.8/univer_db/models/dormitories.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/geo.py` & `python-univer-1.4.8/univer_db/models/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/grades.py` & `python-univer-1.4.8/univer_db/models/grades.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/models.py` & `python-univer-1.4.8/univer_db/models/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/orders.py` & `python-univer-1.4.8/univer_db/models/orders.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/roles.py` & `python-univer-1.4.8/univer_db/models/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/schedule.py` & `python-univer-1.4.8/univer_db/models/schedule.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/sheets.py` & `python-univer-1.4.8/univer_db/models/sheets.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/models/structures.py` & `python-univer-1.4.8/univer_db/models/structures.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/orm.py` & `python-univer-1.4.8/univer_db/orm.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/tests/geo.py` & `python-univer-1.4.8/univer_db/tests/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/tests/models.py` & `python-univer-1.4.8/univer_db/tests/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/tests/roles.py` & `python-univer-1.4.8/univer_db/tests/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.7/univer_db/tests/structures.py` & `python-univer-1.4.8/univer_db/tests/structures.py`

 * *Files identical despite different names*

