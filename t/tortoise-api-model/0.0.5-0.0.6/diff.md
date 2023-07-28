# Comparing `tmp/tortoise_api_model-0.0.5.tar.gz` & `tmp/tortoise_api_model-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.0.5.tar", last modified: Fri Jul 28 08:03:02 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.0.6.tar", last modified: Fri Jul 28 19:29:09 2023, max compression
```

## Comparing `tortoise_api_model-0.0.5.tar` & `tortoise_api_model-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:03:02.395378 tortoise_api_model-0.0.5/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 08:03:02.395019 tortoise_api_model-0.0.5/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 08:03:02.395475 tortoise_api_model-0.0.5/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-28 08:02:17.000000 tortoise_api_model-0.0.5/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:03:02.392893 tortoise_api_model-0.0.5/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       50 2023-07-25 15:09:00.000000 tortoise_api_model-0.0.5/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)      973 2023-07-27 16:35:52.000000 tortoise_api_model-0.0.5/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:03:02.394523 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 08:03:02.000000 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-28 08:03:02.000000 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 08:03:02.000000 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 08:03:02.000000 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-28 08:03:02.000000 tortoise_api_model-0.0.5/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.697956 tortoise_api_model-0.0.6/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 19:29:09.697739 tortoise_api_model-0.0.6/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 19:29:09.698016 tortoise_api_model-0.0.6/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-28 18:12:45.000000 tortoise_api_model-0.0.6/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.696027 tortoise_api_model-0.0.6/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)       50 2023-07-25 15:09:00.000000 tortoise_api_model-0.0.6/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)      921 2023-07-28 18:00:16.000000 tortoise_api_model-0.0.6/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:29:09.697471 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-28 19:29:09.000000 tortoise_api_model-0.0.6/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.0.5/setup.py` & `tortoise_api_model-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

### Comparing `tortoise_api_model-0.0.5/tortoise_api_model/model.py` & `tortoise_api_model-0.0.6/tortoise_api_model/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from asyncpg import Point, Polygon
+from asyncpg import Point, Polygon, Range
 from tortoise import Model as BaseModel
 from tortoise.fields import Field
+from tortoise.fields.base import VALUE
 
 
 class Model(BaseModel):
     # id: int = IntField(pk=True)
     _name: str = 'name'
     def repr(self):
         if self._name in self._meta.db_fields:
             return getattr(self, self._name)
         return self.__repr__()
 
 
 # Custom Fields
-class PointField(Field[Point]):
-    SQL_TYPE = "POINT"
-    field_type = Point
-
+class SeqField(Field[VALUE]):
     def to_python_value(self, value):
-        if value is not None and not isinstance(value, Point):
-            value = Point(*value)  # pylint: disable=E1102
+        if value is not None and not isinstance(value, self.field_type):
+            value = self.field_type(*value)
         self.validate(value)
         return value
 
-class PolygonField(Field[Polygon]):
+class RangeField(SeqField[Range]):
+    SQL_TYPE = "int4range"
+    field_type = Range
+
+class PointField(SeqField[Point]):
+    SQL_TYPE = "POINT"
+    field_type = Point
+
+class PolygonField(SeqField[Polygon]):
     SQL_TYPE = "POLYGON"
     field_type = Polygon
     base_field = PointField
-
-    def to_python_value(self, value):
-        if value is not None and not isinstance(value, Polygon):
-            value = Polygon(*value)  # pylint: disable=E1102
-        self.validate(value)
-        return value
```

