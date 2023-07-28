# Comparing `tmp/sa-filters-1.2.0.tar.gz` & `tmp/sa-filters-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sa-filters-1.2.0.tar", last modified: Sun Nov  6 10:29:09 2022, max compression
+gzip compressed data, was "dist/sa-filters-1.3.0.tar", last modified: Fri Jul 28 13:58:11 2023, max compression
```

## Comparing `sa-filters-1.2.0.tar` & `sa-filters-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 10:29:09.000000 sa-filters-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-11-06 10:28:59.000000 sa-filters-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-11-06 10:28:59.000000 sa-filters-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-06 10:28:59.000000 sa-filters-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    21690 2022-11-06 10:29:09.000000 sa-filters-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-11-06 10:28:59.000000 sa-filters-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8120 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/loads.py
--rw-r--r--   0 runner    (1001) docker     (121)     6240 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-11-06 10:28:59.000000 sa-filters-1.2.0/sa_filters/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21690 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 10:29:09.000000 sa-filters-1.2.0/sa_filters.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-06 10:29:09.000000 sa-filters-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-11-06 10:28:59.000000 sa-filters-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:58:11.000000 sa-filters-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-28 13:58:04.000000 sa-filters-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-28 13:58:04.000000 sa-filters-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 13:58:04.000000 sa-filters-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-07-28 13:58:11.000000 sa-filters-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-07-28 13:58:04.000000 sa-filters-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:58:11.000000 sa-filters-1.3.0/sa_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-28 13:58:04.000000 sa-filters-1.3.0/sa_filters/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:58:11.000000 sa-filters-1.3.0/sa_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-07-28 13:58:10.000000 sa-filters-1.3.0/sa_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-28 13:58:11.000000 sa-filters-1.3.0/sa_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:58:10.000000 sa-filters-1.3.0/sa_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:58:10.000000 sa-filters-1.3.0/sa_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 13:58:10.000000 sa-filters-1.3.0/sa_filters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:58:10.000000 sa-filters-1.3.0/sa_filters.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:58:11.000000 sa-filters-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-28 13:58:04.000000 sa-filters-1.3.0/setup.py
```

### Comparing `sa-filters-1.2.0/CHANGELOG.rst` & `sa-filters-1.3.0/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Release Notes
 =============
 
 Here you can see the full list of changes between sa-filters
 versions, where semantic versioning is used: *major.minor.patch*.
 
 
+1.3.0
+-----
+
+Released 2023-07-28
+
+* Add support sqlalchemy 2.0
+* Fix CI error 'Failed to initialize container mariadb:latest'
+* Fix CI work with latest tox version
+
 1.2.0
 -----
 
 Released 2022-11-06
 
 * Add the ability to use table name instead of model name
```

### Comparing `sa-filters-1.2.0/LICENSE` & `sa-filters-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sa-filters-1.2.0/PKG-INFO` & `sa-filters-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sa-filters
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library to filter SQLAlchemy queries.
 Home-page: https://github.com/slymit/sa-filters
 Author: Student.com
 Author-email: wearehiring@student.com
 Maintainer: slymit
 Maintainer-email: slymit@gmail.com
 License: Apache License, Version 2.0
 Description: sa-filters
         ==========
         
         
         Filter, sort and paginate SQLAlchemy query objects. Ideal for
         exposing these actions over a REST API.
         
-        This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 support
+        This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 and 2.0 support
         and other improvements.
         
         
         .. image:: https://img.shields.io/pypi/v/sa-filters.svg
             :target: https://pypi.org/project/sa-filters/
         
         .. image:: https://img.shields.io/pypi/pyversions/sa-filters.svg
@@ -532,15 +532,15 @@
         - MySQL
         - PostgreSQL
         
         
         SQLAlchemy support
         ------------------
         
-        The following SQLAlchemy_ versions are supported: ``1.4``.
+        The following SQLAlchemy_ versions are supported: ``1.4``, ``2.0``.
         
         
         Changelog
         ---------
         
         Consult the `CHANGELOG <https://github.com/slymit/sa-filters/blob/master/CHANGELOG.rst>`_
         document for fixes and enhancements of each version.
```

### Comparing `sa-filters-1.2.0/README.rst` & `sa-filters-1.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sa-filters
 ==========
 
 
 Filter, sort and paginate SQLAlchemy query objects. Ideal for
 exposing these actions over a REST API.
 
-This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 support
+This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 and 2.0 support
 and other improvements.
 
 
 .. image:: https://img.shields.io/pypi/v/sa-filters.svg
     :target: https://pypi.org/project/sa-filters/
 
 .. image:: https://img.shields.io/pypi/pyversions/sa-filters.svg
@@ -522,15 +522,15 @@
 - MySQL
 - PostgreSQL
 
 
 SQLAlchemy support
 ------------------
 
-The following SQLAlchemy_ versions are supported: ``1.4``.
+The following SQLAlchemy_ versions are supported: ``1.4``, ``2.0``.
 
 
 Changelog
 ---------
 
 Consult the `CHANGELOG <https://github.com/slymit/sa-filters/blob/master/CHANGELOG.rst>`_
 document for fixes and enhancements of each version.
```

### Comparing `sa-filters-1.2.0/sa_filters/filters.py` & `sa-filters-1.3.0/sa_filters/filters.py`

 * *Files identical despite different names*

### Comparing `sa-filters-1.2.0/sa_filters/loads.py` & `sa-filters-1.3.0/sa_filters/loads.py`

 * *Files identical despite different names*

### Comparing `sa-filters-1.2.0/sa_filters/models.py` & `sa-filters-1.3.0/sa_filters/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.inspection import inspect
 from sqlalchemy.orm import mapperlib, Query
 from sqlalchemy.sql.util import find_tables
 from sqlalchemy import Table
-from sqlalchemy.util import symbol
+from sqlalchemy.ext.hybrid import hybrid_property, hybrid_method
 import types
 
 from .exceptions import BadQuery, FieldNotFound, BadSpec
 
 
 class Field(object):
 
@@ -35,28 +35,20 @@
         inspect_mapper = inspect(self.model)
         columns = inspect_mapper.columns
         orm_descriptors = inspect_mapper.all_orm_descriptors
 
         column_names = columns.keys()
         hybrid_names = [
             key for key, item in orm_descriptors.items()
-            if _is_hybrid_property(item) or _is_hybrid_method(item)
+            if type(item) in [hybrid_property, hybrid_method]
         ]
 
         return set(column_names) | set(hybrid_names)
 
 
-def _is_hybrid_property(orm_descriptor):
-    return orm_descriptor.extension_type == symbol('HYBRID_PROPERTY')
-
-
-def _is_hybrid_method(orm_descriptor):
-    return orm_descriptor.extension_type == symbol('HYBRID_METHOD')
-
-
 def get_model_from_table(table):  # pragma: nocover
     """Resolve model class from table object"""
 
     for registry in mapperlib._all_registries():
         for mapper in registry.mappers:
             if table in mapper.tables:
                 return mapper.class_
```

### Comparing `sa-filters-1.2.0/sa_filters/pagination.py` & `sa-filters-1.3.0/sa_filters/pagination.py`

 * *Files identical despite different names*

### Comparing `sa-filters-1.2.0/sa_filters/sorting.py` & `sa-filters-1.3.0/sa_filters/sorting.py`

 * *Files identical despite different names*

### Comparing `sa-filters-1.2.0/sa_filters.egg-info/PKG-INFO` & `sa-filters-1.3.0/sa_filters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sa-filters
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library to filter SQLAlchemy queries.
 Home-page: https://github.com/slymit/sa-filters
 Author: Student.com
 Author-email: wearehiring@student.com
 Maintainer: slymit
 Maintainer-email: slymit@gmail.com
 License: Apache License, Version 2.0
 Description: sa-filters
         ==========
         
         
         Filter, sort and paginate SQLAlchemy query objects. Ideal for
         exposing these actions over a REST API.
         
-        This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 support
+        This project is fork of sqlalchemy-filters_ with sqlalchemy 1.4 and 2.0 support
         and other improvements.
         
         
         .. image:: https://img.shields.io/pypi/v/sa-filters.svg
             :target: https://pypi.org/project/sa-filters/
         
         .. image:: https://img.shields.io/pypi/pyversions/sa-filters.svg
@@ -532,15 +532,15 @@
         - MySQL
         - PostgreSQL
         
         
         SQLAlchemy support
         ------------------
         
-        The following SQLAlchemy_ versions are supported: ``1.4``.
+        The following SQLAlchemy_ versions are supported: ``1.4``, ``2.0``.
         
         
         Changelog
         ---------
         
         Consult the `CHANGELOG <https://github.com/slymit/sa-filters/blob/master/CHANGELOG.rst>`_
         document for fixes and enhancements of each version.
```

### Comparing `sa-filters-1.2.0/setup.py` & `sa-filters-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'README.rst'), 'r', 'utf-8') as handle:
     readme = handle.read()
 
 setup(
     name='sa-filters',
-    version='1.2.0',
+    version='1.3.0',
     description='A library to filter SQLAlchemy queries.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Student.com',
     author_email='wearehiring@student.com',
     maintainer='slymit',
     maintainer_email='slymit@gmail.com',
     url='https://github.com/slymit/sa-filters',
     packages=find_packages(exclude=['test', 'test.*']),
     install_requires=['sqlalchemy>=1.4.0'],
     extras_require={
         'dev': [
             'pytest>=6.2.5',
+            'packaging>=23.1',
             'coverage~=5.0.4',
-            'sqlalchemy-utils~=0.37.2',
+            'sqlalchemy-utils~=0.41.1',
             'flake8',
             'restructuredtext-lint',
             'Pygments',
         ],
         'mysql': ['mysql-connector-python-rf==2.2.2'],
         'postgresql': ['psycopg2==2.8.4'],
     },
```

