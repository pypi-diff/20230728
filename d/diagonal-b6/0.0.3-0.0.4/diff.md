# Comparing `tmp/diagonal_b6-0.0.3.tar.gz` & `tmp/diagonal_b6-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagonal_b6-0.0.3.tar", last modified: Thu Jun 29 17:19:38 2023, max compression
+gzip compressed data, was "diagonal_b6-0.0.4.tar", last modified: Fri Jul 28 09:27:35 2023, max compression
```

## Comparing `diagonal_b6-0.0.3.tar` & `diagonal_b6-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       71 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.381563 diagonal_b6-0.0.3/diagonal_b6/
--rw-rw-r--   0 root         (0) root         (0)      233 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54912 2023-06-29 17:19:24.000000 diagonal_b6-0.0.3/diagonal_b6/api_generated.py
--rw-r--r--   0 root         (0) root         (0)     9079 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-29 17:17:43.000000 diagonal_b6-0.0.3/diagonal_b6/api_pb2_grpc.py
--rwxrwxr-x   0 root         (0) root         (0)    27773 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/b6_test.py
--rw-rw-r--   0 root         (0) root         (0)     1466 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/collection.py
--rw-rw-r--   0 root         (0) root         (0)      976 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/connect.py
--rw-rw-r--   0 root         (0) root         (0)     4238 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/expression.py
--rw-rw-r--   0 root         (0) root         (0)     6766 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/features.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/features_pb2.py
--rwxrwxr-x   0 root         (0) root         (0)     8424 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/generate_api.py
--rw-rw-r--   0 root         (0) root         (0)     3927 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/geometry.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/geometry_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2168 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/diagonal_b6.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      803 2023-06-29 17:17:43.000000 diagonal_b6-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:27:35.136276 diagonal_b6-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-07-28 09:27:35.136276 diagonal_b6-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:27:35.136276 diagonal_b6-0.0.4/diagonal_b6/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58525 2023-07-28 09:27:23.000000 diagonal_b6-0.0.4/diagonal_b6/api_generated.py
+-rw-r--r--   0 root         (0) root         (0)     9079 2023-07-28 09:26:48.000000 diagonal_b6-0.0.4/diagonal_b6/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-28 09:26:48.000000 diagonal_b6-0.0.4/diagonal_b6/api_pb2_grpc.py
+-rwxr-xr-x   0 root         (0) root         (0)    29777 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/b6_test.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/connect.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/expression.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/features.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-28 09:26:48.000000 diagonal_b6-0.0.4/diagonal_b6/features_pb2.py
+-rwxr-xr-x   0 root         (0) root         (0)     9056 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/generate_api.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-07-28 09:26:48.000000 diagonal_b6-0.0.4/diagonal_b6/geometry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-27 16:47:51.000000 diagonal_b6-0.0.4/diagonal_b6/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:27:35.136276 diagonal_b6-0.0.4/diagonal_b6.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-07-28 09:27:35.000000 diagonal_b6-0.0.4/diagonal_b6.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-28 09:27:35.000000 diagonal_b6-0.0.4/diagonal_b6.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:27:35.000000 diagonal_b6-0.0.4/diagonal_b6.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-28 09:27:35.000000 diagonal_b6-0.0.4/diagonal_b6.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 09:27:35.000000 diagonal_b6-0.0.4/diagonal_b6.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-28 09:26:48.000000 diagonal_b6-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:27:35.136276 diagonal_b6-0.0.4/setup.cfg
```

### Comparing `diagonal_b6-0.0.3/PKG-INFO` & `diagonal_b6-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagonal_b6
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
 Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/api_generated.py` & `diagonal_b6-0.0.4/diagonal_b6/api_generated.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 # Client library for Diagonal's geospatial analysis engine, b6.
 
 from __future__ import annotations
 
 from typing import Callable
 
 import diagonal_b6.expression
-from diagonal_b6.expression import Call, Symbol, Lambda, Result
+from diagonal_b6.expression import Call, Symbol, Lambda, Result, register_builtin_result
 
-VERSION = '0.0.3+modified'
+VERSION = '0.0.4+modified'
 
 class CollectionTraits:
 
-    def flattern(self) -> CollectionResult:
-        return flattern(self)
-
-    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-        return map(self, a0)
-
-    def count(self) -> IntTraits:
-        return count(self)
-
     def map_parallel(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
         return map_parallel(self, a0)
 
+    def flattern(self) -> CollectionResult:
+        return flattern(self)
+
     def top(self, a0: IntTraits) -> CollectionResult:
         return top(self, a0)
 
+    def filter(self, a0: Callable[[AnyTraits],BoolTraits]) -> CollectionResult:
+        return filter(self, a0)
+
+    def sum_by_key(self) -> CollectionResult:
+        return sum_by_key(self)
+
     def take(self, a0: IntTraits) -> CollectionResult:
         return take(self, a0)
 
     def count_values(self) -> CollectionResult:
         return count_values(self)
 
-    def map_items(self, a0: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
-        return map_items(self, a0)
+    def count(self) -> IntTraits:
+        return count(self)
 
-    def sum_by_key(self) -> CollectionResult:
-        return sum_by_key(self)
+    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+        return map(self, a0)
 
-    def filter(self, a0: Callable[[AnyTraits],BoolTraits]) -> CollectionResult:
-        return filter(self, a0)
+    def map_items(self, a0: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
+        return map_items(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class RenderableTraits:
 
@@ -67,459 +67,541 @@
 
     @classmethod
     def _values(cls):
         return RenderableResult
 
 class GeometryTraits(RenderableTraits):
 
+    def points(self) -> PointCollectionResult:
+        return points(self)
+
     def centroid(self) -> PointTraits:
         return centroid(self)
 
-    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
-        return tile_paths(self, a0)
-
     def intersecting(self) -> QueryTraits:
         return intersecting(self)
 
-    def points(self) -> PointCollectionResult:
-        return points(self)
+    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
+        return tile_paths(self, a0)
 
     @classmethod
     def _collection(cls):
         return AnyGeometryCollectionResult
 
 class GeometryValuesTraits(RenderableValuesTraits):
 
+    def points(self) -> CollectionTraits:
+        return self.map(Lambda(points, [self._values()]))
+
     def centroid(self) -> PointCollectionTraits:
         return self.map(Lambda(centroid, [self._values()]))
 
-    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
-
     def intersecting(self) -> CollectionTraits:
         return self.map(Lambda(intersecting, [self._values()]))
 
-    def points(self) -> CollectionTraits:
-        return self.map(Lambda(points, [self._values()]))
+    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
 
 class AnyGeometryValuesResult(Result, GeometryValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return GeometryResult
 
 class IdentifiableTraits:
 
-    def all_tags(self) -> IntTagCollectionResult:
-        return all_tags(self)
+    def count_tag_value(self, a0: StringTraits) -> CollectionResult:
+        return count_tag_value(self, a0)
+
+    def get(self, a0: StringTraits) -> TagTraits:
+        return get(self, a0)
+
+    def get_int(self, a0: StringTraits) -> IntTraits:
+        return get_int(self, a0)
 
     def remove_tag(self, a0: StringTraits) -> ChangeTraits:
         return remove_tag(self, a0)
 
     def add_tag(self, a0: TagTraits) -> ChangeTraits:
         return add_tag(self, a0)
 
-    def count_tag_value(self, a0: StringTraits) -> CollectionResult:
-        return count_tag_value(self, a0)
-
-    def get_int(self, a0: StringTraits) -> IntTraits:
-        return get_int(self, a0)
-
     def debug_tokens(self) -> IntStringCollectionResult:
         return debug_tokens(self)
 
-    def get_string(self, a0: StringTraits) -> StringTraits:
-        return get_string(self, a0)
+    def all_tags(self) -> IntTagCollectionResult:
+        return all_tags(self)
 
     def get_float(self, a0: StringTraits) -> FloatTraits:
         return get_float(self, a0)
 
-    def get(self, a0: StringTraits) -> TagTraits:
-        return get(self, a0)
+    def get_string(self, a0: StringTraits) -> StringTraits:
+        return get_string(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class IdentifiableValuesTraits:
 
-    def all_tags(self) -> CollectionTraits:
-        return self.map(Lambda(all_tags, [self._values()]))
-
-    def remove_tag(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
-
-    def add_tag(self, a0: TagTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: add_tag(x, a0), [self._values()]))
-
     def count_tag_value(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: count_tag_value(x, a0), [self._values()]))
 
+    def get(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
+
     def get_int(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: get_int(x, a0), [self._values()]))
 
+    def remove_tag(self, a0: StringTraits) -> AnyChangeCollectionTraits:
+        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
+
+    def add_tag(self, a0: TagTraits) -> AnyChangeCollectionTraits:
+        return self.map(Lambda(lambda x: add_tag(x, a0), [self._values()]))
+
     def debug_tokens(self) -> CollectionTraits:
         return self.map(Lambda(debug_tokens, [self._values()]))
 
-    def get_string(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
+    def all_tags(self) -> CollectionTraits:
+        return self.map(Lambda(all_tags, [self._values()]))
 
     def get_float(self, a0: StringTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: get_float(x, a0), [self._values()]))
 
-    def get(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
+    def get_string(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
 
 class AnyIdentifiableValuesResult(Result, IdentifiableValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IdentifiableResult
 
-class FeatureTraits(IdentifiableTraits, RenderableTraits):
-
-    def has_key(self, a0: StringTraits) -> BoolTraits:
-        return has_key(self, a0)
-
-    def connect_to_network(self) -> ChangeTraits:
-        return connect_to_network(self)
-
-    def tile_ids_hex(self) -> FeatureIDStringCollectionResult:
-        return tile_ids_hex(self)
+class FeatureTraits(RenderableTraits, IdentifiableTraits):
 
-    def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureIDIntCollectionResult:
-        return paths_to_reach(self, a0, a1, a2)
+    def point_features(self) -> PointFeatureCollectionResult:
+        return point_features(self)
 
     def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionResult:
         return reachable(self, a0, a1, a2)
 
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
-        return reachable_points(self, a0, a1, a2)
+    def tile_ids(self) -> FeatureIDIntCollectionResult:
+        return tile_ids(self)
 
-    def point_features(self) -> PointFeatureCollectionResult:
-        return point_features(self)
+    def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureIDIntCollectionResult:
+        return paths_to_reach(self, a0, a1, a2)
 
-    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> FloatTraits:
-        return reachable_area(self, a0, a1)
+    def tile_ids_hex(self) -> FeatureIDStringCollectionResult:
+        return tile_ids_hex(self)
 
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureTraits:
         return closest(self, a0, a1, a2)
 
+    def has_key(self, a0: StringTraits) -> BoolTraits:
+        return has_key(self, a0)
+
     def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FloatTraits:
         return closest_distance(self, a0, a1, a2)
 
-    def tile_ids(self) -> FeatureIDIntCollectionResult:
-        return tile_ids(self)
+    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> FloatTraits:
+        return reachable_area(self, a0, a1)
+
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
+        return reachable_points(self, a0, a1, a2)
+
+    def connect_to_network(self) -> ChangeTraits:
+        return connect_to_network(self)
 
     @classmethod
     def _collection(cls):
         return FeatureCollectionResult
 
-class FeatureValuesTraits(IdentifiableValuesTraits, RenderableValuesTraits):
-
-    def has_key(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: has_key(x, a0), [self._values()]))
-
-    def connect_to_network(self) -> CollectionTraits:
-        return self.map(Lambda(connect_to_network, [self._values()]))
-
-    def tile_ids_hex(self) -> CollectionTraits:
-        return self.map(Lambda(tile_ids_hex, [self._values()]))
+class FeatureValuesTraits(RenderableValuesTraits, IdentifiableValuesTraits):
 
-    def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: paths_to_reach(x, a0, a1, a2), [self._values()]))
+    def point_features(self) -> CollectionTraits:
+        return self.map(Lambda(point_features, [self._values()]))
 
     def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: reachable(x, a0, a1, a2), [self._values()]))
 
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
+    def tile_ids(self) -> CollectionTraits:
+        return self.map(Lambda(tile_ids, [self._values()]))
 
-    def point_features(self) -> CollectionTraits:
-        return self.map(Lambda(point_features, [self._values()]))
+    def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: paths_to_reach(x, a0, a1, a2), [self._values()]))
 
-    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: reachable_area(x, a0, a1), [self._values()]))
+    def tile_ids_hex(self) -> CollectionTraits:
+        return self.map(Lambda(tile_ids_hex, [self._values()]))
 
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionTraits:
         return self.map(Lambda(lambda x: closest(x, a0, a1, a2), [self._values()]))
 
+    def has_key(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: has_key(x, a0), [self._values()]))
+
     def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: closest_distance(x, a0, a1, a2), [self._values()]))
 
-    def tile_ids(self) -> CollectionTraits:
-        return self.map(Lambda(tile_ids, [self._values()]))
+    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: reachable_area(x, a0, a1), [self._values()]))
+
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
+
+    def connect_to_network(self) -> AnyChangeCollectionTraits:
+        return self.map(Lambda(connect_to_network, [self._values()]))
 
 class AnyFeatureValuesResult(Result, FeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureResult
 
-class AreaTraits(GeometryTraits):
+class PointTraits(GeometryTraits):
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
-        return snap_area_edges(self, a0, a1)
+    def add_point(self, a0: StringPointCollectionResult) -> StringPointCollectionResult:
+        return add_point(self, a0)
 
-    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
-        return s2_grid(self, a0)
+    def within_cap(self, a0: FloatTraits) -> QueryTraits:
+        return within_cap(self, a0)
 
-    def s2_points(self, a0: IntTraits, a1: IntTraits) -> StringPointCollectionResult:
-        return s2_points(self, a0, a1)
+    def intersecting_cap(self, a0: FloatTraits) -> QueryTraits:
+        return intersecting_cap(self, a0)
+
+    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
+        return cap_polygon(self, a0)
+
+    def sightline(self, a0: FloatTraits) -> AreaTraits:
+        return sightline(self, a0)
+
+    def distance_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_meters(self, a0)
+
+    def rectangle_polygon(self, a0: PointTraits) -> AreaTraits:
+        return rectangle_polygon(self, a0)
+
+    @classmethod
+    def _collection(cls):
+        return PointCollectionResult
+
+class PointValuesTraits(GeometryValuesTraits):
+
+    def add_point(self, a0: StringPointCollectionResult) -> CollectionTraits:
+        return self.map(Lambda(lambda x: add_point(x, a0), [self._values()]))
+
+    def within_cap(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: within_cap(x, a0), [self._values()]))
+
+    def intersecting_cap(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: intersecting_cap(x, a0), [self._values()]))
+
+    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
+
+    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
+
+    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
+
+    def rectangle_polygon(self, a0: PointTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: rectangle_polygon(x, a0), [self._values()]))
+
+class AnyPointValuesResult(Result, PointValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PointResult
+
+class AreaTraits(GeometryTraits):
+
+    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> StringStringCollectionResult:
+        return s2_covering(self, a0, a1)
 
     def within(self) -> QueryTraits:
         return within(self)
 
+    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
+        return s2_grid(self, a0)
+
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
+        return snap_area_edges(self, a0, a1)
+
     def area(self) -> FloatTraits:
         return area(self)
 
-    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> StringStringCollectionResult:
-        return s2_covering(self, a0, a1)
+    def s2_points(self, a0: IntTraits, a1: IntTraits) -> StringPointCollectionResult:
+        return s2_points(self, a0, a1)
 
     @classmethod
     def _collection(cls):
         return AreaCollectionResult
 
 class AreaValuesTraits(GeometryValuesTraits):
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
+    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: s2_covering(x, a0, a1), [self._values()]))
+
+    def within(self) -> CollectionTraits:
+        return self.map(Lambda(within, [self._values()]))
 
     def s2_grid(self, a0: IntTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: s2_grid(x, a0), [self._values()]))
 
-    def s2_points(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: s2_points(x, a0, a1), [self._values()]))
-
-    def within(self) -> CollectionTraits:
-        return self.map(Lambda(within, [self._values()]))
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
 
     def area(self) -> AnyFloatCollectionTraits:
         return self.map(Lambda(area, [self._values()]))
 
-    def s2_covering(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: s2_covering(x, a0, a1), [self._values()]))
+    def s2_points(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: s2_points(x, a0, a1), [self._values()]))
 
 class AnyAreaValuesResult(Result, AreaValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return AreaResult
 
 class NumberTraits:
 
+    def add(self, a0: NumberTraits) -> NumberTraits:
+        return add(self, a0)
+
     def divide(self, a0: NumberTraits) -> NumberTraits:
         return divide(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class NumberValuesTraits:
 
+    def add(self, a0: NumberTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: add(x, a0), [self._values()]))
+
     def divide(self, a0: NumberTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: divide(x, a0), [self._values()]))
 
 class AnyNumberValuesResult(Result, NumberValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return NumberResult
 
-class PointTraits(GeometryTraits):
+class StringTraits:
 
-    def sightline(self, a0: FloatTraits) -> AreaTraits:
-        return sightline(self, a0)
+    def parse_geojson_file(self) -> GeoJSONTraits:
+        return parse_geojson_file(self)
 
-    def intersecting_cap(self, a0: FloatTraits) -> QueryTraits:
-        return intersecting_cap(self, a0)
+    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson_file(self, a0)
 
-    def add_point(self, a0: StringPointCollectionResult) -> StringPointCollectionResult:
-        return add_point(self, a0)
+    def s2_center(self) -> PointTraits:
+        return s2_center(self)
 
-    def within_cap(self, a0: FloatTraits) -> QueryTraits:
-        return within_cap(self, a0)
+    def debug_all_query(self) -> QueryTraits:
+        return debug_all_query(self)
 
-    def rectangle_polygon(self, a0: PointTraits) -> AreaTraits:
-        return rectangle_polygon(self, a0)
+    def tag(self, a0: StringTraits) -> TagTraits:
+        return tag(self, a0)
 
-    def distance_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_meters(self, a0)
+    def keyed(self) -> QueryTraits:
+        return keyed(self)
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
-        return cap_polygon(self, a0)
+    def s2_polygon(self) -> AreaTraits:
+        return s2_polygon(self)
+
+    def parse_geojson(self) -> GeoJSONTraits:
+        return parse_geojson(self)
+
+    def tagged(self, a0: StringTraits) -> QueryTraits:
+        return tagged(self, a0)
+
+    def export_world(self) -> IntTraits:
+        return export_world(self)
 
     @classmethod
     def _collection(cls):
-        return PointCollectionResult
+        return CollectionResult
 
-class PointValuesTraits(GeometryValuesTraits):
+class StringValuesTraits:
 
-    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
+    def parse_geojson_file(self) -> CollectionTraits:
+        return self.map(Lambda(parse_geojson_file, [self._values()]))
 
-    def intersecting_cap(self, a0: FloatTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: intersecting_cap(x, a0), [self._values()]))
+    def import_geojson_file(self, a0: StringTraits) -> AnyChangeCollectionTraits:
+        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
 
-    def add_point(self, a0: StringPointCollectionResult) -> CollectionTraits:
-        return self.map(Lambda(lambda x: add_point(x, a0), [self._values()]))
+    def s2_center(self) -> PointCollectionTraits:
+        return self.map(Lambda(s2_center, [self._values()]))
 
-    def within_cap(self, a0: FloatTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: within_cap(x, a0), [self._values()]))
+    def debug_all_query(self) -> CollectionTraits:
+        return self.map(Lambda(debug_all_query, [self._values()]))
 
-    def rectangle_polygon(self, a0: PointTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: rectangle_polygon(x, a0), [self._values()]))
+    def tag(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tag(x, a0), [self._values()]))
 
-    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
+    def keyed(self) -> CollectionTraits:
+        return self.map(Lambda(keyed, [self._values()]))
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
+    def s2_polygon(self) -> AreaCollectionTraits:
+        return self.map(Lambda(s2_polygon, [self._values()]))
 
-class AnyPointValuesResult(Result, PointValuesTraits, CollectionTraits):
+    def parse_geojson(self) -> CollectionTraits:
+        return self.map(Lambda(parse_geojson, [self._values()]))
+
+    def tagged(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tagged(x, a0), [self._values()]))
+
+    def export_world(self) -> CollectionTraits:
+        return self.map(Lambda(export_world, [self._values()]))
+
+class AnyStringValuesResult(Result, StringValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointResult
+        return StringResult
 
 class PathTraits(GeometryTraits):
 
     def ordered_join(self, a0: PathTraits) -> PathTraits:
         return ordered_join(self, a0)
 
-    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_to_point_meters(self, a0)
+    def join(self, a0: PathTraits) -> PathTraits:
+        return join(self, a0)
 
     def interpolate(self, a0: FloatTraits) -> PointTraits:
         return interpolate(self, a0)
 
     def sample_points(self, a0: FloatTraits) -> StringPointCollectionResult:
         return sample_points(self, a0)
 
-    def join(self, a0: PathTraits) -> PathTraits:
-        return join(self, a0)
+    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_to_point_meters(self, a0)
 
     @classmethod
     def _collection(cls):
         return PathCollectionResult
 
 class PathValuesTraits(GeometryValuesTraits):
 
     def ordered_join(self, a0: PathTraits) -> PathCollectionTraits:
         return self.map(Lambda(lambda x: ordered_join(x, a0), [self._values()]))
 
-    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
+    def join(self, a0: PathTraits) -> PathCollectionTraits:
+        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
 
     def interpolate(self, a0: FloatTraits) -> PointCollectionTraits:
         return self.map(Lambda(lambda x: interpolate(x, a0), [self._values()]))
 
     def sample_points(self, a0: FloatTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: sample_points(x, a0), [self._values()]))
 
-    def join(self, a0: PathTraits) -> PathCollectionTraits:
-        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
+    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
 
 class AnyPathValuesResult(Result, PathValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return PathResult
 
-class StringTraits:
+class FeatureIDTraits(IdentifiableTraits):
 
-    def s2_polygon(self) -> AreaTraits:
-        return s2_polygon(self)
+    def find_feature(self) -> FeatureTraits:
+        return find_feature(self)
 
-    def tagged(self, a0: StringTraits) -> QueryTraits:
-        return tagged(self, a0)
+    def find_path(self) -> PathFeatureTraits:
+        return find_path(self)
 
-    def export_world(self) -> IntTraits:
-        return export_world(self)
+    def find_point(self) -> PointFeatureTraits:
+        return find_point(self)
 
-    def tag(self, a0: StringTraits) -> TagTraits:
-        return tag(self, a0)
+    def find_area(self) -> AreaFeatureTraits:
+        return find_area(self)
 
-    def parse_geojson(self) -> GeoJSONTraits:
-        return parse_geojson(self)
+    def find_relation(self) -> RelationFeatureTraits:
+        return find_relation(self)
 
-    def keyed(self) -> QueryTraits:
-        return keyed(self)
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def s2_center(self) -> PointTraits:
-        return s2_center(self)
+class FeatureIDValuesTraits(IdentifiableValuesTraits):
 
-    def debug_all_query(self) -> QueryTraits:
-        return debug_all_query(self)
+    def find_feature(self) -> FeatureCollectionTraits:
+        return self.map(Lambda(find_feature, [self._values()]))
 
-    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson_file(self, a0)
+    def find_path(self) -> PathFeatureCollectionTraits:
+        return self.map(Lambda(find_path, [self._values()]))
 
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+    def find_point(self) -> PointFeatureCollectionTraits:
+        return self.map(Lambda(find_point, [self._values()]))
 
-class StringValuesTraits:
+    def find_area(self) -> AreaFeatureCollectionTraits:
+        return self.map(Lambda(find_area, [self._values()]))
 
-    def s2_polygon(self) -> AreaCollectionTraits:
-        return self.map(Lambda(s2_polygon, [self._values()]))
+    def find_relation(self) -> RelationFeatureCollectionTraits:
+        return self.map(Lambda(find_relation, [self._values()]))
 
-    def tagged(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tagged(x, a0), [self._values()]))
+class AnyFeatureIDValuesResult(Result, FeatureIDValuesTraits, CollectionTraits):
 
-    def export_world(self) -> CollectionTraits:
-        return self.map(Lambda(export_world, [self._values()]))
+    def __init__(self, node):
+        Result.__init__(self, node)
 
-    def tag(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tag(x, a0), [self._values()]))
+    @classmethod
+    def _values(cls):
+        return FeatureIDResult
 
-    def parse_geojson(self) -> CollectionTraits:
-        return self.map(Lambda(parse_geojson, [self._values()]))
+class IdentifiablePointTraits:
 
-    def keyed(self) -> CollectionTraits:
-        return self.map(Lambda(keyed, [self._values()]))
+    def point_paths(self) -> PathFeatureCollectionResult:
+        return point_paths(self)
 
-    def s2_center(self) -> PointCollectionTraits:
-        return self.map(Lambda(s2_center, [self._values()]))
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def debug_all_query(self) -> CollectionTraits:
-        return self.map(Lambda(debug_all_query, [self._values()]))
+class IdentifiablePointValuesTraits:
 
-    def import_geojson_file(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
+    def point_paths(self) -> CollectionTraits:
+        return self.map(Lambda(point_paths, [self._values()]))
 
-class AnyStringValuesResult(Result, StringValuesTraits, CollectionTraits):
+class AnyIdentifiablePointValuesResult(Result, IdentifiablePointValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return IdentifiablePointResult
 
 class TagTraits:
 
     def int_value(self) -> IntTraits:
         return int_value(self)
 
     def value(self) -> StringTraits:
@@ -548,135 +630,92 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return TagResult
 
-class IdentifiablePointTraits:
-
-    def point_paths(self) -> PathFeatureCollectionResult:
-        return point_paths(self)
-
+class AreaFeatureTraits(FeatureTraits, AreaTraits):
     @classmethod
     def _collection(cls):
-        return CollectionResult
-
-class IdentifiablePointValuesTraits:
+        return AreaFeatureCollectionResult
 
-    def point_paths(self) -> CollectionTraits:
-        return self.map(Lambda(point_paths, [self._values()]))
+class AreaFeatureValuesTraits(FeatureValuesTraits, AreaValuesTraits):
+    pass
 
-class AnyIdentifiablePointValuesResult(Result, IdentifiablePointValuesTraits, CollectionTraits):
+class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return IdentifiablePointResult
-
-class FeatureIDTraits(IdentifiableTraits):
-
-    def find_relation(self) -> RelationFeatureTraits:
-        return find_relation(self)
-
-    def find_point(self) -> PointFeatureTraits:
-        return find_point(self)
-
-    def find_feature(self) -> FeatureTraits:
-        return find_feature(self)
-
-    def find_area(self) -> AreaFeatureTraits:
-        return find_area(self)
-
-    def find_path(self) -> PathFeatureTraits:
-        return find_path(self)
+        return AreaFeatureResult
 
+class PointCollectionTraits(CollectionTraits, PointValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDValuesTraits(IdentifiableValuesTraits):
+class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def find_relation(self) -> RelationFeatureCollectionTraits:
-        return self.map(Lambda(find_relation, [self._values()]))
+class ChangeTraits:
 
-    def find_point(self) -> PointFeatureCollectionTraits:
-        return self.map(Lambda(find_point, [self._values()]))
+    def with_change(self, a0: Callable[[],AnyTraits]) -> AnyTraits:
+        return with_change(self, a0)
 
-    def find_feature(self) -> FeatureCollectionTraits:
-        return self.map(Lambda(find_feature, [self._values()]))
+    @classmethod
+    def _collection(cls):
+        return AnyChangeCollectionResult
 
-    def find_area(self) -> AreaFeatureCollectionTraits:
-        return self.map(Lambda(find_area, [self._values()]))
+class ChangeValuesTraits:
 
-    def find_path(self) -> PathFeatureCollectionTraits:
-        return self.map(Lambda(find_path, [self._values()]))
+    def with_change(self, a0: Callable[[],AnyTraits]) -> CollectionTraits:
+        return self.map(Lambda(lambda x: with_change(x, a0), [self._values()]))
 
-class AnyFeatureIDValuesResult(Result, FeatureIDValuesTraits, CollectionTraits):
+class AnyChangeValuesResult(Result, ChangeValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureIDResult
+        return ChangeResult
 
-class AnyTraits:
+class PointFeatureTraits(FeatureTraits, PointTraits, IdentifiablePointTraits):
 
-    def gt(self, a0: AnyTraits) -> BoolTraits:
-        return gt(self, a0)
-
-    def pair(self, a0: AnyTraits) -> PairTraits:
-        return pair(self, a0)
+    def degree(self) -> IntTraits:
+        return degree(self)
 
-    def collection(self, a0: AnyTraits) -> CollectionResult:
-        return collection(self, a0)
+    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
+        return connect(self, a0)
 
     @classmethod
     def _collection(cls):
-        return CollectionResult
-
-class AnyValuesTraits:
-
-    def gt(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: gt(x, a0), [self._values()]))
-
-    def pair(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
-
-    def collection(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: collection(x, a0), [self._values()]))
+        return PointFeatureCollectionResult
 
-class AnyAnyValuesResult(Result, AnyValuesTraits, CollectionTraits):
+class PointFeatureValuesTraits(FeatureValuesTraits, PointValuesTraits, IdentifiablePointValuesTraits):
 
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-    @classmethod
-    def _values(cls):
-        return AnyResult
-
-class AreaFeatureTraits(AreaTraits, FeatureTraits):
-    @classmethod
-    def _collection(cls):
-        return AreaFeatureCollectionResult
+    def degree(self) -> CollectionTraits:
+        return self.map(Lambda(degree, [self._values()]))
 
-class AreaFeatureValuesTraits(AreaValuesTraits, FeatureValuesTraits):
-    pass
+    def connect(self, a0: PointFeatureTraits) -> AnyChangeCollectionTraits:
+        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
 
-class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
+class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return PointFeatureResult
 
 class FloatTraits(NumberTraits):
 
     def ll(self, a0: FloatTraits) -> PointTraits:
         return ll(self, a0)
 
     @classmethod
@@ -693,37 +732,14 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FloatResult
 
-class PathFeatureTraits(FeatureTraits, PathTraits):
-
-    def length(self) -> FloatTraits:
-        return length(self)
-
-    @classmethod
-    def _collection(cls):
-        return PathFeatureCollectionResult
-
-class PathFeatureValuesTraits(FeatureValuesTraits, PathValuesTraits):
-
-    def length(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(length, [self._values()]))
-
-class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-    @classmethod
-    def _values(cls):
-        return PathFeatureResult
-
 class IntTraits(NumberTraits):
 
     def add_ints(self, a0: IntTraits) -> IntTraits:
         return add_ints(self, a0)
 
     def clamp(self, a0: IntTraits, a1: IntTraits) -> IntTraits:
         return clamp(self, a0, a1)
@@ -751,266 +767,285 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IntResult
 
-class PointCollectionTraits(CollectionTraits, PointValuesTraits):
+class PathFeatureTraits(PathTraits, FeatureTraits):
+
+    def length(self) -> FloatTraits:
+        return length(self)
+
     @classmethod
     def _collection(cls):
-        return CollectionResult
+        return PathFeatureCollectionResult
+
+class PathFeatureValuesTraits(PathValuesTraits, FeatureValuesTraits):
+
+    def length(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(length, [self._values()]))
+
+class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PathFeatureResult
 
 class PathCollectionTraits(CollectionTraits, PathValuesTraits):
 
     def sample_points_along_paths(self, a0: FloatTraits) -> PointCollectionResult:
         return sample_points_along_paths(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+class AnyTraits:
+
+    def collection(self) -> CollectionResult:
+        return collection(self)
+
+    def pair(self, a0: AnyTraits) -> PairTraits:
+        return pair(self, a0)
+
+    def gt(self, a0: AnyTraits) -> BoolTraits:
+        return gt(self, a0)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class RelationFeatureTraits(FeatureTraits, GeometryTraits):
+class AnyValuesTraits:
+
+    def collection(self) -> CollectionTraits:
+        return self.map(Lambda(collection, [self._values()]))
+
+    def pair(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
+
+    def gt(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: gt(x, a0), [self._values()]))
+
+class AnyAnyValuesResult(Result, AnyValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return AnyResult
+
+class RelationFeatureTraits(GeometryTraits, FeatureTraits):
     @classmethod
     def _collection(cls):
         return RelationFeatureCollectionResult
 
-class RelationFeatureValuesTraits(FeatureValuesTraits, GeometryValuesTraits):
+class RelationFeatureValuesTraits(GeometryValuesTraits, FeatureValuesTraits):
     pass
 
 class AnyRelationFeatureValuesResult(Result, RelationFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return RelationFeatureResult
 
-class PointFeatureTraits(PointTraits, IdentifiablePointTraits, FeatureTraits):
-
-    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
-        return connect(self, a0)
+class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def degree(self) -> IntTraits:
-        return degree(self)
+class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
+class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
     @classmethod
     def _collection(cls):
-        return PointFeatureCollectionResult
+        return CollectionResult
 
-class PointFeatureValuesTraits(PointValuesTraits, IdentifiablePointValuesTraits, FeatureValuesTraits):
+class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
 
-    def connect(self, a0: PointFeatureTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
+    def to_geojson_collection(self) -> GeoJSONTraits:
+        return to_geojson_collection(self)
 
-    def degree(self) -> CollectionTraits:
-        return self.map(Lambda(degree, [self._values()]))
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
+class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
 
-    def __init__(self, node):
-        Result.__init__(self, node)
+    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
+        return containing_areas(self, a0)
 
     @classmethod
-    def _values(cls):
-        return PointFeatureResult
+    def _collection(cls):
+        return CollectionResult
 
-class PairTraits:
+class QueryProtoTraits:
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def first(self) -> AnyTraits:
-        return first(self)
+class AnyGeometryCollectionTraits(CollectionTraits, GeometryValuesTraits):
 
-    def second(self) -> AnyTraits:
-        return second(self)
+    def convex_hull(self) -> AreaTraits:
+        return convex_hull(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class QueryTraits:
 
+    def find_relations(self) -> RelationFeatureCollectionResult:
+        return find_relations(self)
+
     def find_paths(self) -> PathFeatureCollectionResult:
         return find_paths(self)
 
-    def find(self) -> FeatureCollectionResult:
-        return find(self)
-
-    def or_(self, a0: QueryTraits) -> QueryTraits:
-        return or_(self, a0)
-
-    def find_points(self) -> PointFeatureCollectionResult:
-        return find_points(self)
-
     def find_areas(self) -> AreaFeatureCollectionResult:
         return find_areas(self)
 
-    def find_relations(self) -> RelationFeatureCollectionResult:
-        return find_relations(self)
+    def find_points(self) -> PointFeatureCollectionResult:
+        return find_points(self)
 
     def and_(self, a0: QueryTraits) -> QueryTraits:
         return and_(self, a0)
 
+    def or_(self, a0: QueryTraits) -> QueryTraits:
+        return or_(self, a0)
+
+    def find(self) -> FeatureCollectionResult:
+        return find(self)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
+class PathFeatureCollectionTraits(PathCollectionTraits, PathFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class GeoJSONTraits:
-
-    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-        return map_geometries(self, a0)
-
-    def geojson_areas(self) -> StringAreaCollectionResult:
-        return geojson_areas(self)
+class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
 
-    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson(self, a0)
+    def remove_tags(self) -> ChangeTraits:
+        return remove_tags(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class RelationFeatureCollectionTraits(CollectionTraits, RelationFeatureValuesTraits):
+class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class BoolTraits:
+class IntFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
-
-    def add_tags(self) -> ChangeTraits:
-        return add_tags(self)
-
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
 
-class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
+        return building_access(self, a0, a1)
 
-class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class AnyFloatCollectionTraits(CollectionTraits, FloatValuesTraits):
 
     def percentiles(self) -> AnyFloatCollectionResult:
         return percentiles(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
+class PairTraits:
 
-    def to_geojson_collection(self) -> GeoJSONTraits:
-        return to_geojson_collection(self)
+    def first(self) -> AnyTraits:
+        return first(self)
 
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+    def second(self) -> AnyTraits:
+        return second(self)
 
-class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+class AnyChangeCollectionTraits(CollectionTraits, ChangeValuesTraits):
+
+    def merge_changes(self) -> ChangeTraits:
+        return merge_changes(self)
 
-class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
 
-    def remove_tags(self) -> ChangeTraits:
-        return remove_tags(self)
+    def add_tags(self) -> ChangeTraits:
+        return add_tags(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class QueryProtoTraits:
+class RelationFeatureCollectionTraits(CollectionTraits, RelationFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class ChangeTraits:
-
-    def with_change(self, a0: Callable[[],AnyTraits]) -> AnyTraits:
-        return with_change(self, a0)
-
+class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class AreaFeatureCollectionTraits(AreaCollectionTraits, AreaFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AnyGeometryCollectionTraits(CollectionTraits, GeometryValuesTraits):
-
-    def convex_hull(self) -> AreaTraits:
-        return convex_hull(self)
-
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+class GeoJSONTraits:
 
-class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
+    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson(self, a0)
 
-class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
+    def geojson_areas(self) -> StringAreaCollectionResult:
+        return geojson_areas(self)
 
-    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
-        return containing_areas(self, a0)
+    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+        return map_geometries(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PathFeatureCollectionTraits(PathCollectionTraits, PathFeatureValuesTraits):
+class BoolTraits:
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
-
-    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
-        return building_access(self, a0, a1)
-
+class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class IntFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
+class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class CollectionResult(Result, CollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
@@ -1031,654 +1066,788 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
 class FeatureResult(Result, FeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
+class PointResult(Result, PointTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
 class AreaResult(Result, AreaTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class NumberResult(Result, NumberTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointResult(Result, PointTraits):
+class StringResult(Result, StringTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class PathResult(Result, PathTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class StringResult(Result, StringTraits):
+class FeatureIDResult(Result, FeatureIDTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class IdentifiablePointResult(Result, IdentifiablePointTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class TagResult(Result, TagTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class IdentifiablePointResult(Result, IdentifiablePointTraits):
+class AreaFeatureResult(Result, AreaFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FeatureIDResult(Result, FeatureIDTraits):
+class PointCollectionResult(Result, PointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AnyResult(Result, AnyTraits):
+    @classmethod
+    def _values(cls):
+        return PointResult
+
+class AreaCollectionResult(Result, AreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaFeatureResult(Result, AreaFeatureTraits):
+    @classmethod
+    def _values(cls):
+        return AreaResult
+
+class ChangeResult(Result, ChangeTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FloatResult(Result, FloatTraits):
+class PointFeatureResult(Result, PointFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathFeatureResult(Result, PathFeatureTraits):
+class FloatResult(Result, FloatTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class IntResult(Result, IntTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointCollectionResult(Result, PointCollectionTraits):
+class PathFeatureResult(Result, PathFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return PointResult
-
 class PathCollectionResult(Result, PathCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return PathResult
 
-class AreaCollectionResult(Result, AreaCollectionTraits):
+class AnyResult(Result, AnyTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return AreaResult
-
 class RelationFeatureResult(Result, RelationFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointFeatureResult(Result, PointFeatureTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-class PairResult(Result, PairTraits):
+class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class QueryResult(Result, QueryTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
+    @classmethod
+    def _values(cls):
+        return AreaResult
 
 class StringPointCollectionResult(Result, StringPointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return PointResult
 
-class GeoJSONResult(Result, GeoJSONTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-class RelationFeatureCollectionResult(Result, RelationFeatureCollectionTraits):
+class IntTagCollectionResult(Result, IntTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RelationFeatureResult
-
-class BoolResult(Result, BoolTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
+        return TagResult
 
-class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
+class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return TagResult
+        return RenderableResult
 
-class IntTagCollectionResult(Result, IntTagCollectionTraits):
+class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return TagResult
+        return PointFeatureResult
 
-class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
+class QueryProtoResult(Result, QueryProtoTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class AnyGeometryCollectionResult(Result, AnyGeometryCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return IntResult
+        return GeometryResult
 
-class AnyFloatCollectionResult(Result, AnyFloatCollectionTraits):
+class QueryResult(Result, QueryTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FloatResult
+        return PathFeatureResult
 
-class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
+class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RenderableResult
+        return StringResult
 
-class IntStringCollectionResult(Result, IntStringCollectionTraits):
+class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return IntResult
 
-class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
+class IntFeatureIDCollectionResult(Result, IntFeatureIDCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureIDResult
 
-class StringStringCollectionResult(Result, StringStringCollectionTraits):
+class FeatureCollectionResult(Result, FeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return FeatureResult
 
-class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
+class AnyFloatCollectionResult(Result, AnyFloatCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return FloatResult
 
-class QueryProtoResult(Result, QueryProtoTraits):
+class PairResult(Result, PairTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class ChangeResult(Result, ChangeTraits):
+class AnyChangeCollectionResult(Result, AnyChangeCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
+    @classmethod
+    def _values(cls):
+        return ChangeResult
+
+class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return TagResult
 
-class AnyGeometryCollectionResult(Result, AnyGeometryCollectionTraits):
+class RelationFeatureCollectionResult(Result, RelationFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return GeometryResult
+        return RelationFeatureResult
 
-class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
+class StringStringCollectionResult(Result, StringStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaResult
+        return StringResult
 
-class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
+class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointFeatureResult
+        return AreaFeatureResult
 
-class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
+class GeoJSONResult(Result, GeoJSONTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return PathFeatureResult
+class BoolResult(Result, BoolTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
 
-class FeatureCollectionResult(Result, FeatureCollectionTraits):
+class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureResult
+        return FeatureIDResult
 
-class IntFeatureIDCollectionResult(Result, IntFeatureIDCollectionTraits):
+class IntStringCollectionResult(Result, IntStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureIDResult
+        return StringResult
 
-class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
+class FunctionAnyAnyResult(Result, Callable[[AnyTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AnyTraits) -> BoolTraits:
+    def __call__(self, a0 : AnyTraits) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionAnyAnyResult(Result, Callable[[AnyTraits],AnyTraits]):
+class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AnyTraits) -> AnyTraits:
+    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
+class FunctionAnyResult(Result, Callable[[],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PathTraits) -> GeometryTraits:
+    def __call__(self, ) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionPairAnyResult(Result, Callable[[PairTraits],AnyTraits]):
+class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PairTraits) -> AnyTraits:
+    def __call__(self, a0 : PathTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionAnyResult(Result, Callable[[],AnyTraits]):
+class FunctionPointGeometryResult(Result, Callable[[PointTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, ) -> AnyTraits:
+    def __call__(self, a0 : PointTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
+class FunctionPairAnyResult(Result, Callable[[PairTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
+    def __call__(self, a0 : PairTraits) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionPointGeometryResult(Result, Callable[[PointTraits],GeometryTraits]):
+class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PointTraits) -> GeometryTraits:
+    def __call__(self, a0 : AnyTraits) -> BoolTraits:
         raise NotImplementedError()
 
 class FunctionGeometryGeometryResult(Result, Callable[[GeometryTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     def __call__(self, a0 : GeometryTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('find-paths'), [a0]))
+def int_value(a0: TagTraits) -> IntTraits:
+    args = [a0]
+    return IntResult(Call(Symbol('int-value'), args))
 
-def convex_hull(a0: AnyGeometryCollectionResult) -> AreaTraits:
-    return AreaResult(Call(Symbol('convex-hull'), [a0]))
+def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
+    args = [a0]
+    return PointFeatureCollectionResult(Call(Symbol('point-features'), args))
 
-def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson-collection'), [a0]))
+def reachable(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureCollectionResult:
+    args = [a0, a1, a2, a3]
+    return FeatureCollectionResult(Call(Symbol('reachable'), args))
 
 def building_access(a0: FeatureCollectionResult, a1: FloatTraits, a2: StringTraits) -> FeatureIDFeatureIDCollectionResult:
-    return FeatureIDFeatureIDCollectionResult(Call(Symbol('building-access'), [a0, a1, a2]))
+    args = [a0, a1, a2]
+    return FeatureIDFeatureIDCollectionResult(Call(Symbol('building-access'), args))
 
-def find(a0: QueryTraits) -> FeatureCollectionResult:
-    return FeatureCollectionResult(Call(Symbol('find'), [a0]))
+def add_point(a0: PointTraits, a1: StringPointCollectionResult) -> StringPointCollectionResult:
+    args = [a0, a1]
+    return StringPointCollectionResult(Call(Symbol('add-point'), args))
 
-def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('or'), [a0, a1]))
+def within_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
+    args = [a0, a1]
+    return QueryResult(Call(Symbol('within-cap'), args))
 
-def s2_polygon(a0: StringTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('s2-polygon'), [a0]))
+def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
+    args = [a0]
+    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), args))
 
-def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
-    return BoolResult(Call(Symbol('gt'), [a0, a1]))
+def type_path() -> QueryProtoTraits:
+    args = []
+    return QueryProtoResult(Call(Symbol('type-path'), args))
 
-def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
-    return PairResult(Call(Symbol('pair'), [a0, a1]))
+def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
+    args = [a0, a1]
+    return CollectionResult(Call(Symbol('count-tag-value'), args))
 
-def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('tagged'), [a0, a1]))
+def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    args = [a0, a1]
+    return PathResult(Call(Symbol('ordered-join'), args))
 
-def centroid(a0: GeometryTraits) -> PointTraits:
-    return PointResult(Call(Symbol('centroid'), [a0]))
+def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
+    args = [a0, a1, a2]
+    return StringStringCollectionResult(Call(Symbol('s2-covering'), args))
 
-def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('sightline'), [a0, a1]))
+def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
+    args = [a0]
+    return GeoJSONResult(Call(Symbol('to-geojson'), args))
 
-def flattern(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('flattern'), [a0]))
+def map_parallel(a0: CollectionResult, a1: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+    args = [a0, a1]
+    return CollectionResult(Call(Symbol('map-parallel'), args))
 
-def has_key(a0: FeatureTraits, a1: StringTraits) -> BoolTraits:
-    return BoolResult(Call(Symbol('has-key'), [a0, a1]))
+def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
+    args = [a0]
+    return AnyFloatCollectionResult(Call(Symbol('percentiles'), args))
 
-def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
-    return IntResult(Call(Symbol('add-ints'), [a0, a1]))
+def value(a0: TagTraits) -> StringTraits:
+    args = [a0]
+    return StringResult(Call(Symbol('value'), args))
 
-def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect-to-network'), [a0]))
+def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
+    args = [a0, a1]
+    return TagResult(Call(Symbol('get'), args))
 
-def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
-    return IntTagCollectionResult(Call(Symbol('all-tags'), [a0]))
+def points(a0: GeometryTraits) -> PointCollectionResult:
+    args = [a0]
+    return PointCollectionResult(Call(Symbol('points'), args))
 
-def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
-    return NumberResult(Call(Symbol('divide'), [a0, a1]))
+def intersecting_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
+    args = [a0, a1]
+    return QueryResult(Call(Symbol('intersecting-cap'), args))
 
-def snap_area_edges(a0: AreaTraits, a1: QueryTraits, a2: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('snap-area-edges'), [a0, a1, a2]))
+def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
+    args = [a0, a1]
+    return IntResult(Call(Symbol('get-int'), args))
 
-def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-grid'), [a0, a1]))
+def parse_geojson_file(a0: StringTraits) -> GeoJSONTraits:
+    args = [a0]
+    return GeoJSONResult(Call(Symbol('parse-geojson-file'), args))
+
+def collection(*a0: AnyTraits) -> CollectionResult:
+    args = []
+    args.extend(a0)
+    return CollectionResult(Call(Symbol('collection'), args))
+
+def merge_changes(a0: AnyChangeCollectionResult) -> ChangeTraits:
+    args = [a0]
+    return ChangeResult(Call(Symbol('merge-changes'), args))
 
-def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
-    return AnyFloatCollectionResult(Call(Symbol('percentiles'), [a0]))
+def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
+    args = [a0]
+    return PathFeatureCollectionResult(Call(Symbol('find-paths'), args))
 
-def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), [a0]))
+def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
+    args = [a0]
+    return PathFeatureCollectionResult(Call(Symbol('point-paths'), args))
 
-def export_world(a0: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('export-world'), [a0]))
+def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
+    args = [a0]
+    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), args))
 
-def int_value(a0: TagTraits) -> IntTraits:
-    return IntResult(Call(Symbol('int-value'), [a0]))
+def import_geojson_file(a0: StringTraits, a1: StringTraits) -> ChangeTraits:
+    args = [a0, a1]
+    return ChangeResult(Call(Symbol('import-geojson-file'), args))
 
-def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('map-geometries'), [a0, a1]))
+def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
+    args = [a0, a1]
+    return ChangeResult(Call(Symbol('remove-tag'), args))
 
-def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
-    return RelationFeatureResult(Call(Symbol('find-relation'), [a0]))
+def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
+    args = [a0]
+    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), args))
 
-def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
-    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), [a0]))
+def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
+    args = [a0, a1]
+    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), args))
 
-def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), [a0]))
+def first(a0: PairTraits) -> AnyTraits:
+    args = [a0]
+    return AnyResult(Call(Symbol('first'), args))
 
-def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tag'), [a0, a1]))
+def flattern(a0: CollectionResult) -> CollectionResult:
+    args = [a0]
+    return CollectionResult(Call(Symbol('flattern'), args))
 
-def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect'), [a0, a1]))
+def second(a0: PairTraits) -> AnyTraits:
+    args = [a0]
+    return AnyResult(Call(Symbol('second'), args))
 
-def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('tile-paths'), [a0, a1]))
+def top(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
+    args = [a0, a1]
+    return CollectionResult(Call(Symbol('top'), args))
 
-def empty_points() -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('empty-points'), []))
+def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
+    args = [a0]
+    return ChangeResult(Call(Symbol('remove-tags'), args))
 
-def geojson_areas(a0: GeoJSONTraits) -> StringAreaCollectionResult:
-    return StringAreaCollectionResult(Call(Symbol('geojson-areas'), [a0]))
+def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
+    args = [a0]
+    return FeatureResult(Call(Symbol('find-feature'), args))
 
-def intersecting(a0: GeometryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('intersecting'), [a0]))
+def convex_hull(a0: AnyGeometryCollectionResult) -> AreaTraits:
+    args = [a0]
+    return AreaResult(Call(Symbol('convex-hull'), args))
 
-def intersecting_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('intersecting-cap'), [a0, a1]))
+def length(a0: PathFeatureTraits) -> FloatTraits:
+    args = [a0]
+    return FloatResult(Call(Symbol('length'), args))
 
 def degree(a0: PointFeatureTraits) -> IntTraits:
-    return IntResult(Call(Symbol('degree'), [a0]))
+    args = [a0]
+    return IntResult(Call(Symbol('degree'), args))
 
-def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('s2-points'), [a0, a1, a2]))
-
-def add_tag(a0: IdentifiableTraits, a1: TagTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('add-tag'), [a0, a1]))
+def paths_to_reach(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureIDIntCollectionResult:
+    args = [a0, a1, a2, a3]
+    return FeatureIDIntCollectionResult(Call(Symbol('paths-to-reach'), args))
 
-map = diagonal_b6.expression._map
+def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
+    args = [a0, a1]
+    return ChangeResult(Call(Symbol('connect'), args))
 
-def first(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('first'), [a0]))
+def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    args = [a0]
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), args))
 
-def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), [a0, a1]))
+filter = diagonal_b6.expression._filter
 
-def clamp(a0: IntTraits, a1: IntTraits, a2: IntTraits) -> IntTraits:
-    return IntResult(Call(Symbol('clamp'), [a0, a1, a2]))
+def sum_by_key(a0: CollectionResult) -> CollectionResult:
+    args = [a0]
+    return CollectionResult(Call(Symbol('sum-by-key'), args))
 
-def paths_to_reach(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureIDIntCollectionResult:
-    return FeatureIDIntCollectionResult(Call(Symbol('paths-to-reach'), [a0, a1, a2, a3]))
+def within(a0: AreaTraits) -> QueryTraits:
+    args = [a0]
+    return QueryResult(Call(Symbol('within'), args))
 
-def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
-    return PointFeatureResult(Call(Symbol('find-point'), [a0]))
+def s2_center(a0: StringTraits) -> PointTraits:
+    args = [a0]
+    return PointResult(Call(Symbol('s2-center'), args))
 
-def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('find-points'), [a0]))
+def add_tag(a0: IdentifiableTraits, a1: TagTraits) -> ChangeTraits:
+    args = [a0, a1]
+    return ChangeResult(Call(Symbol('add-tag'), args))
 
-def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('tag'), [a0, a1]))
+def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
+    args = [a0, a1]
+    return StringStringCollectionResult(Call(Symbol('s2-grid'), args))
 
-def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-tag-value'), [a0, a1]))
+def snap_area_edges(a0: AreaTraits, a1: QueryTraits, a2: FloatTraits) -> AreaTraits:
+    args = [a0, a1, a2]
+    return AreaResult(Call(Symbol('snap-area-edges'), args))
 
-def count(a0: CollectionResult) -> IntTraits:
-    return IntResult(Call(Symbol('count'), [a0]))
+def take(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
+    args = [a0, a1]
+    return CollectionResult(Call(Symbol('take'), args))
 
-def reachable(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureCollectionResult:
-    return FeatureCollectionResult(Call(Symbol('reachable'), [a0, a1, a2, a3]))
+def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
+    args = [a0]
+    return PointFeatureCollectionResult(Call(Symbol('find-points'), args))
 
-def map_parallel(a0: CollectionResult, a1: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-    return CollectionResult(Call(Symbol('map-parallel'), [a0, a1]))
+def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    args = [a0, a1]
+    return PathResult(Call(Symbol('join'), args))
 
-def top(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('top'), [a0, a1]))
+def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    args = [a0]
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), args))
 
-def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), [a0]))
+def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
+    args = [a0, a1]
+    return PairResult(Call(Symbol('pair'), args))
 
-def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('ordered-join'), [a0, a1]))
+def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    args = [a0, a1]
+    return QueryResult(Call(Symbol('and'), args))
 
-def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('get-int'), [a0, a1]))
+def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
+    args = [a0, a1]
+    return IntResult(Call(Symbol('add-ints'), args))
 
-def within(a0: AreaTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('within'), [a0]))
+def debug_all_query(a0: StringTraits) -> QueryTraits:
+    args = [a0]
+    return QueryResult(Call(Symbol('debug-all-query'), args))
 
-def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), [a0, a1, a2, a3]))
+def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    args = [a0, a1]
+    return QueryResult(Call(Symbol('or'), args))
 
-def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('debug-tokens'), [a0]))
+def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
+    args = [a0, a1]
+    return TagResult(Call(Symbol('tag'), args))
 
-def take(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('take'), [a0, a1]))
+def area(a0: AreaTraits) -> FloatTraits:
+    args = [a0]
+    return FloatResult(Call(Symbol('area'), args))
 
-def add_point(a0: PointTraits, a1: StringPointCollectionResult) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('add-point'), [a0, a1]))
+def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
+    args = [a0]
+    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), args))
 
-def with_change(a0: ChangeTraits, a1: Callable[[],AnyTraits]) -> AnyTraits:
-    return AnyResult(Call(Symbol('with-change'), [a0, a1]))
+def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
+    args = [a0]
+    return IntStringCollectionResult(Call(Symbol('debug-tokens'), args))
 
-def count_values(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-values'), [a0]))
+def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
+    args = [a0, a1, a2, a3]
+    return FeatureResult(Call(Symbol('closest'), args))
 
 def import_geojson(a0: GeoJSONTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('import-geojson'), [a0, a1]))
+    args = [a0, a1]
+    return ChangeResult(Call(Symbol('import-geojson'), args))
 
-def type_path() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-path'), []))
+def all() -> QueryTraits:
+    args = []
+    return QueryResult(Call(Symbol('all'), args))
 
-def within_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('within-cap'), [a0, a1]))
+def has_key(a0: FeatureTraits, a1: StringTraits) -> BoolTraits:
+    args = [a0, a1]
+    return BoolResult(Call(Symbol('has-key'), args))
 
-def divide_int(a0: IntTraits, a1: FloatTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('divide-int'), [a0, a1]))
+def interpolate(a0: PathTraits, a1: FloatTraits) -> PointTraits:
+    args = [a0, a1]
+    return PointResult(Call(Symbol('interpolate'), args))
 
-def distance_to_point_meters(a0: PathTraits, a1: PointTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('distance-to-point-meters'), [a0, a1]))
+def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    args = [a0, a1]
+    return AreaResult(Call(Symbol('cap-polygon'), args))
 
-def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
-    return CollectionResult(Call(Symbol('map-items'), [a0, a1]))
+def centroid(a0: GeometryTraits) -> PointTraits:
+    args = [a0]
+    return PointResult(Call(Symbol('centroid'), args))
 
-def collection(a0: AnyTraits, a1: AnyTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('collection'), [a0, a1]))
+def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
+    args = [a0]
+    return GeoJSONResult(Call(Symbol('to-geojson-collection'), args))
 
-def area(a0: AreaTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('area'), [a0]))
+def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    args = [a0, a1]
+    return AreaResult(Call(Symbol('sightline'), args))
 
-def rectangle_polygon(a0: PointTraits, a1: PointTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('rectangle-polygon'), [a0, a1]))
+def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
+    args = [a0]
+    return ChangeResult(Call(Symbol('add-tags'), args))
 
-def parse_geojson(a0: StringTraits) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('parse-geojson'), [a0]))
+def count_values(a0: CollectionResult) -> CollectionResult:
+    args = [a0]
+    return CollectionResult(Call(Symbol('count-values'), args))
 
-def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('point-features'), [a0]))
+def intersecting(a0: GeometryTraits) -> QueryTraits:
+    args = [a0]
+    return QueryResult(Call(Symbol('intersecting'), args))
 
-def reachable_area(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('reachable-area'), [a0, a1, a2]))
+def keyed(a0: StringTraits) -> QueryTraits:
+    args = [a0]
+    return QueryResult(Call(Symbol('keyed'), args))
 
-def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('closest'), [a0, a1, a2, a3]))
+def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
+    args = [a0]
+    return IntTagCollectionResult(Call(Symbol('all-tags'), args))
 
-def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('add-tags'), [a0]))
+def clamp(a0: IntTraits, a1: IntTraits, a2: IntTraits) -> IntTraits:
+    args = [a0, a1, a2]
+    return IntResult(Call(Symbol('clamp'), args))
 
-def sum_by_key(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('sum-by-key'), [a0]))
+def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
+    args = [a0, a1, a2, a3]
+    return FloatResult(Call(Symbol('closest-distance'), args))
 
-def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('find-feature'), [a0]))
+def with_change(a0: ChangeTraits, a1: Callable[[],AnyTraits]) -> AnyTraits:
+    args = [a0, a1]
+    return AnyResult(Call(Symbol('with-change'), args))
 
-def keyed(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('keyed'), [a0]))
+def type_point() -> QueryProtoTraits:
+    args = []
+    return QueryProtoResult(Call(Symbol('type-point'), args))
 
-def value(a0: TagTraits) -> StringTraits:
-    return StringResult(Call(Symbol('value'), [a0]))
+def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
+    args = [a0, a1]
+    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), args))
 
-def second(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('second'), [a0]))
+def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
+    args = [a0, a1, a2]
+    return StringPointCollectionResult(Call(Symbol('s2-points'), args))
 
-def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), [a0, a1]))
+def s2_polygon(a0: StringTraits) -> AreaTraits:
+    args = [a0]
+    return AreaResult(Call(Symbol('s2-polygon'), args))
 
-def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
-    return AreaFeatureResult(Call(Symbol('find-area'), [a0]))
+def reachable_area(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits) -> FloatTraits:
+    args = [a0, a1, a2]
+    return FloatResult(Call(Symbol('reachable-area'), args))
 
-def length(a0: PathFeatureTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('length'), [a0]))
+def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
+    args = [a0, a1, a2, a3]
+    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), args))
 
-def interpolate(a0: PathTraits, a1: FloatTraits) -> PointTraits:
-    return PointResult(Call(Symbol('interpolate'), [a0, a1]))
+def empty_points() -> StringPointCollectionResult:
+    args = []
+    return StringPointCollectionResult(Call(Symbol('empty-points'), args))
 
-def points(a0: GeometryTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('points'), [a0]))
+def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
+    args = [a0]
+    return PathFeatureResult(Call(Symbol('find-path'), args))
 
-def s2_center(a0: StringTraits) -> PointTraits:
-    return PointResult(Call(Symbol('s2-center'), [a0]))
+def type_area() -> QueryProtoTraits:
+    args = []
+    return QueryProtoResult(Call(Symbol('type-area'), args))
 
-def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
-    return StringResult(Call(Symbol('get-string'), [a0, a1]))
+def float_value(a0: TagTraits) -> FloatTraits:
+    args = [a0]
+    return FloatResult(Call(Symbol('float-value'), args))
 
-def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('point-paths'), [a0]))
+def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
+    args = [a0]
+    return ChangeResult(Call(Symbol('connect-to-network'), args))
+
+def ll(a0: FloatTraits, a1: FloatTraits) -> PointTraits:
+    args = [a0, a1]
+    return PointResult(Call(Symbol('ll'), args))
 
 def distance_meters(a0: PointTraits, a1: PointTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('distance-meters'), [a0, a1]))
+    args = [a0, a1]
+    return FloatResult(Call(Symbol('distance-meters'), args))
 
-def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('get-float'), [a0, a1]))
+def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
+    args = [a0]
+    return PointFeatureResult(Call(Symbol('find-point'), args))
 
-def ll(a0: FloatTraits, a1: FloatTraits) -> PointTraits:
-    return PointResult(Call(Symbol('ll'), [a0, a1]))
+def count(a0: CollectionResult) -> IntTraits:
+    args = [a0]
+    return IntResult(Call(Symbol('count'), args))
 
-def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
-    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), [a0]))
+def rectangle_polygon(a0: PointTraits, a1: PointTraits) -> AreaTraits:
+    args = [a0, a1]
+    return AreaResult(Call(Symbol('rectangle-polygon'), args))
 
-def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('get'), [a0, a1]))
+def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
+    args = [a0]
+    return AreaFeatureResult(Call(Symbol('find-area'), args))
 
-filter = diagonal_b6.expression._filter
+def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
+    args = [a0]
+    return RelationFeatureResult(Call(Symbol('find-relation'), args))
 
-def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('closest-distance'), [a0, a1, a2, a3]))
+def divide_int(a0: IntTraits, a1: FloatTraits) -> FloatTraits:
+    args = [a0, a1]
+    return FloatResult(Call(Symbol('divide-int'), args))
 
-def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('cap-polygon'), [a0, a1]))
+def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    args = [a0]
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), args))
 
-def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
-    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), [a0]))
+map = diagonal_b6.expression._map
 
-def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
-    return PathFeatureResult(Call(Symbol('find-path'), [a0]))
+def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
+    args = [a0, a1]
+    return FloatResult(Call(Symbol('get-float'), args))
 
 def sample_points(a0: PathTraits, a1: FloatTraits) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('sample-points'), [a0, a1]))
+    args = [a0, a1]
+    return StringPointCollectionResult(Call(Symbol('sample-points'), args))
 
-def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('and'), [a0, a1]))
+def distance_to_point_meters(a0: PathTraits, a1: PointTraits) -> FloatTraits:
+    args = [a0, a1]
+    return FloatResult(Call(Symbol('distance-to-point-meters'), args))
 
-def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson'), [a0]))
+def parse_geojson(a0: StringTraits) -> GeoJSONTraits:
+    args = [a0]
+    return GeoJSONResult(Call(Symbol('parse-geojson'), args))
 
-def debug_all_query(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('debug-all-query'), [a0]))
+def geojson_areas(a0: GeoJSONTraits) -> StringAreaCollectionResult:
+    args = [a0]
+    return StringAreaCollectionResult(Call(Symbol('geojson-areas'), args))
 
-def type_point() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-point'), []))
+def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
+    args = [a0, a1]
+    return QueryResult(Call(Symbol('tagged'), args))
 
-def type_area() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-area'), []))
+def find(a0: QueryTraits) -> FeatureCollectionResult:
+    args = [a0]
+    return FeatureCollectionResult(Call(Symbol('find'), args))
 
-def float_value(a0: TagTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('float-value'), [a0]))
+def add(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
+    args = [a0, a1]
+    return NumberResult(Call(Symbol('add'), args))
 
-def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tags'), [a0]))
+def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
+    args = [a0, a1]
+    return IntStringCollectionResult(Call(Symbol('tile-paths'), args))
 
-def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), [a0]))
+def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+    args = [a0, a1]
+    return GeoJSONResult(Call(Symbol('map-geometries'), args))
 
-def all() -> QueryTraits:
-    return QueryResult(Call(Symbol('all'), []))
+def export_world(a0: StringTraits) -> IntTraits:
+    args = [a0]
+    return IntResult(Call(Symbol('export-world'), args))
 
-def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('join'), [a0, a1]))
+def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
+    args = [a0, a1]
+    return CollectionResult(Call(Symbol('map-items'), args))
 
-def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-covering'), [a0, a1, a2]))
+def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
+    args = [a0, a1]
+    return StringResult(Call(Symbol('get-string'), args))
 
-def import_geojson_file(a0: StringTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('import-geojson-file'), [a0, a1]))
+def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
+    args = [a0, a1]
+    return BoolResult(Call(Symbol('gt'), args))
+
+def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
+    args = [a0, a1]
+    return NumberResult(Call(Symbol('divide'), args))
 
+register_builtin_result(str,StringResult)
+register_builtin_result(int,IntResult)
+register_builtin_result(float,FloatResult)
+register_builtin_result(bool,BoolResult)
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/api_pb2.py` & `diagonal_b6-0.0.4/diagonal_b6/api_pb2.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.3/diagonal_b6/api_pb2_grpc.py` & `diagonal_b6-0.0.4/diagonal_b6/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.3/diagonal_b6/b6_test.py` & `diagonal_b6-0.0.4/diagonal_b6/b6_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,37 +462,80 @@
 
     def test_import_geojson_file(self):
         ids = self.connection(b6.import_geojson_file("data/tests/granary-square.geojson", "diagonal.works/test"))
         self.assertGreater(len(ids), 0)
         id = list(ids.values())[0]
         self.assertGreater(self.connection(b6.find_area(id).area()), 100.0)
 
-    def test_evaluate_with_changed_world(self):
+    def test_parse_geojson_file(self):
+        areas = b6.parse_geojson_file("data/tests/granary-square.geojson").geojson_areas()
+        area = self.connection(b6.convex_hull(areas).area())
+        self.assertGreater(area, 2400.0)
+        self.assertLess(area, 2500.0)
+
+    def test_reachable_with_changed_world(self):
         close_road = b6.remove_tag(b6.osm_way_id(STABLE_STREET_BRIDGE_ID), "#highway")
         reachable = b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_SOUTH_END_ID)).reachable("walk", 200.0, b6.keyed("#amenity")).get_string("name")
         before = len(self.connection(reachable))
         after = len(self.connection(b6.with_change(close_road, lambda: reachable)))
         self.assertGreater(before, after)
 
+    def test_remove_tags(self):
+        roads = b6.find(b6.keyed("#highway"))
+        before = self.connection(roads.count())
+        close_roads = b6.remove_tags(roads.map(lambda road: "#highway"))
+        after = self.connection(b6.with_change(close_roads, lambda: roads.count()))
+        self.assertGreater(before, 0)
+        self.assertEqual(after, 0)
+
+    def test_merge_changes(self):
+        roads = b6.find(b6.keyed("#highway"))
+        before = self.connection(roads.count())
+        close_roads = b6.merge_changes(roads.map(lambda h: b6.remove_tag(h, "#highway")))
+        after = self.connection(b6.with_change(close_roads, lambda: roads.count()))
+        self.assertGreater(before, 0)
+        self.assertEqual(after, 0)
+
     def test_get_tags_from_list_of_ids(self):
-        names = b6.feature_ids([b6.osm_way_area_id(id) for id in (LIGHTERMAN_WAY_ID, GRANARY_SQUARE_WAY_ID)]).map(lambda f: f.get_string("name"))
+        names = b6.map([b6.osm_way_area_id(id) for id in (LIGHTERMAN_WAY_ID, GRANARY_SQUARE_WAY_ID)], lambda f: b6.get_string(f, "name"))
         expected = [(0, "The Lighterman"), (1, "Granary Square")]
         self.assertEqual(expected, self.connection(names))
 
     def test_make_tags_from_list_of_strings(self):
-        tags = b6.strings(["primary", "secondary"]).map(lambda v: b6.tag("#highway", v))
+        tags = b6.map(["primary", "secondary"], lambda v: b6.tag("#highway", v))
         expected = [(0, ("#highway", "primary")), (1, ("#highway", "secondary"))]
         self.assertEqual(expected, self.connection(tags))
 
     def test_convex_hull_from_list_of_lat_lngs(self):
-        caps = b6.lls([(51.535387, -0.125277), (51.537088, -0.125781)]).map(lambda c: b6.cap_polygon(c, 20.0))
+        caps = b6.map([b6.ll(51.535387, -0.125277), b6.ll(51.537088, -0.125781)], lambda c: b6.cap_polygon(c, 20.0))
         areas = self.connection(caps.map(b6.area))
         hull_area = self.connection(b6.convex_hull(caps).area())
         self.assertGreater(hull_area, sum([a for _, a in areas]))
 
+    def test_collection(self):
+        ids = b6.collection(b6.pair(0, b6.osm_way_area_id(GRANARY_SQUARE_WAY_ID)), b6.pair(1, b6.osm_way_area_id(LIGHTERMAN_WAY_ID)))
+        areas = self.connection(ids.map(lambda id: b6.area(b6.find_area(id))))
+        for (i, (j, area)) in enumerate(areas):
+            self.assertEqual(i, j)
+            self.assertGreater(area, 0.0)
+            self.assertLess(area, 6000.0)
+
+    def test_map_literal_collection_from_dict(self):
+        collection = {
+            b6.tag("highway", "motorway"): 3,
+            b6.tag("highway", "primary"): 7,
+        }
+        result = self.connection(b6.map(collection, lambda count: b6.add(count, 1)))
+        self.assertEqual([4, 8], sorted([count for ((key, value), count) in result]))
+
+    def test_map_literal_collection_from_list(self):
+        collection = [36, 42]
+        result = self.connection(b6.map(collection, lambda count: b6.add(count, 1)))
+        self.assertEqual([37, 43], sorted([count for (key, count) in result]))
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--http-port", default="10080", help="Host and port on which to serve HTTP")
     parser.add_argument("--grpc-port", default="10081", help="Host and port on which to serve GRPC")
     parser.add_argument("--platform", default=None, help="Current platform, eg darwin/x86_64")
     parser.add_argument("tests", type=str, nargs="*")
     args = parser.parse_args()
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/connect.py` & `diagonal_b6-0.0.4/diagonal_b6/connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
     def __init__(self, stub):
         self.stub = stub
 
     def __call__(self, e):
         request = api_pb2.EvaluateRequestProto()
         request.version = VERSION
-        request.request.CopyFrom(expression.to_node_proto(e))
+        node = expression.to_node(e)
+        request.request.CopyFrom(node.to_node_proto())
         return expression.from_node_proto(self.stub.Evaluate(request).result)
 
 def connect_insecure(address):
     channel = grpc.insecure_channel(address)
     return Connection(api_pb2_grpc.B6Stub(channel))
 
 def connect(address, token, root_certificates=None):
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/expression.py` & `diagonal_b6-0.0.4/diagonal_b6/expression.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,36 +15,67 @@
         node = api_pb2.NodeProto()
         node.literal.CopyFrom(self.to_literal_proto())
         return node
 
     def to_literal_proto(self):
         raise NotImplementedError()
 
+class LiteralInt(Literal):
+
+    def __init__(self, v):
+        self.v = v
+
+    def to_literal_proto(self):
+        n = api_pb2.LiteralNodeProto()
+        n.intValue = self.v
+        return n
+
+class LiteralFloat(Literal):
+
+    def __init__(self, v):
+        self.v = v
+
+    def to_literal_proto(self):
+        n = api_pb2.LiteralNodeProto()
+        n.floatValue = self.v
+        return n
+
+class LiteralString(Literal):
+
+    def __init__(self, v):
+        self.v = v
+
+    def to_literal_proto(self):
+        n = api_pb2.LiteralNodeProto()
+        n.stringValue = self.v
+        return n
+
 class Symbol(Node):
 
     def __init__(self, name):
         self.name = name
 
     def to_node_proto(self):
-        node = api_pb2.NodeProto()
-        node.symbol = self.name
-        return node
+        n = api_pb2.NodeProto()
+        n.symbol = self.name
+        return n
 
 class Call(Node):
 
     def __init__(self, function, args):
         self.function = function
         self.args = args
 
     def to_node_proto(self):
-        node = api_pb2.NodeProto()
-        node.call.function.CopyFrom(self.function.to_node_proto())
+        n = api_pb2.NodeProto()
+        n.call.function.CopyFrom(self.function.to_node_proto())
         for arg in self.args:
-            node.call.args.add().CopyFrom(to_node_proto(arg))
-        return node
+            node = to_node(arg)
+            n.call.args.add().CopyFrom(node.to_node_proto())
+        return n
 
 class Lambda(Node):
 
     def __init__(self, function, arg_types):
         self.function = function
         self.arg_types = arg_types
 
@@ -52,15 +83,16 @@
         return Lambda(self.function, arg_types)
 
     def to_node_proto(self):
         n = api_pb2.NodeProto()
         args = ["_%s_%d" % (name, id(n)) for name in inspect.signature(self.function).parameters]
         for arg in args:
             n.lambda_.args.append(arg)
-        n.lambda_.node.CopyFrom(to_node_proto(self.function(*[type(Symbol(name)) for (name, type) in zip(args, self.arg_types)])))
+        node = to_node(self.function(*[type(Symbol(name)) for (name, type) in zip(args, self.arg_types)]))
+        n.lambda_.node.CopyFrom(node.to_node_proto())
         return n
 
     def __call__(self, *args):
         return self.function(*args)
 
 def to_lambda(f):
     if isinstance(f, Lambda):
@@ -77,71 +109,95 @@
 
     def __init__(self, node):
         self.node = node
 
     def to_node_proto(self):
         return self.node.to_node_proto()
 
+class ListCollectionResult(Result):
+
+    @classmethod
+    def _values(cls):
+        return Result
+
+class DictCollectionResult(Result):
+
+    @classmethod
+    def _values(cls):
+        return Result
+
 class Placeholder(Node):
 
     def to_node_proto(self):
         raise Exception("Placeholder can't be converted to a proto")
 
-def to_node_proto(v):
+def to_node(v):
     if isinstance(v, Node):
-        return v.to_node_proto()
+        return v
     elif isinstance(v, int):
-       n = api_pb2.NodeProto()
-       n.literal.intValue = v
-       return n
+       return LiteralInt(v)
     elif isinstance(v, float):
-        n = api_pb2.NodeProto()
-        n.literal.floatValue = v
-        return n
+       return LiteralFloat(v)
     elif isinstance(v, str):
-        n = api_pb2.NodeProto()
-        n.literal.stringValue = v
-        return n
+       return LiteralString(v)
+    elif isinstance(v, list):
+        pairs = [Call(Symbol("pair"), [LiteralInt(i), to_node(vv)]) for (i, vv) in enumerate(v)]
+        return ListCollectionResult(Call(Symbol("collection"), pairs))
+    elif isinstance(v, dict):
+        pairs = [Call(Symbol("pair"), [to_node(k), to_node(vv)]) for (k, vv) in v.items()]
+        return DictCollectionResult(Call(Symbol("collection"), pairs))
     elif callable(v):
-        return to_lambda(v).to_node_proto()
+        return to_lambda(v)
     else:
         raise ValueError("Can't convert %s to proto" % (v,))
 
 def from_node_proto(n):
     if n.WhichOneof("node") != "literal":
         raise Exception("Can't convert node type %s to a value" % (n.WhichOneof("node"),))
     return from_literal_node_proto(n.literal)
 
-_literals = {}
+_literal_from_proto = {}
 
-def register_literal(oneof, from_proto):
-    _literals[oneof] = from_proto
+def register_literal_from_proto(oneof, from_proto):
+    _literal_from_proto[oneof] = from_proto
 
-register_literal("nilValue", lambda v: None)
-register_literal("intValue", lambda v: v)
-register_literal("floatValue", lambda v: v)
-register_literal("stringValue", lambda v: v)
-register_literal("tagValue", lambda v: (v.key, v.value))
-register_literal("geoJSONValue", lambda v: json.loads(gzip.decompress(v)))
+register_literal_from_proto("nilValue", lambda v: None)
+register_literal_from_proto("intValue", lambda v: v)
+register_literal_from_proto("floatValue", lambda v: v)
+register_literal_from_proto("stringValue", lambda v: v)
+register_literal_from_proto("tagValue", lambda v: (v.key, v.value))
+register_literal_from_proto("geoJSONValue", lambda v: json.loads(gzip.decompress(v)))
 
 def from_literal_node_proto(literal):
     oneof = literal.WhichOneof("value")
-    from_proto = _literals.get(oneof, None)
+    from_proto = _literal_from_proto.get(oneof, None)
     if from_proto is not None:
         return from_proto(getattr(literal, oneof))
     else:
         raise Exception("can't convert %s to value" % (oneof,))
 
 def from_collection_proto(collection):
     return [(from_literal_node_proto(collection.keys[i]), from_literal_node_proto(collection.values[i]))
             for i in range(0, len(collection.keys))]
 
-register_literal("collectionValue", from_collection_proto)
+register_literal_from_proto("collectionValue", from_collection_proto)
+
+_builtin_results = {}
+
+def register_builtin_result(type, result):
+    _builtin_results[type] = result
+
+def collection_result(result):
+    if type(result) in _builtin_results:
+        return _builtin_results[type(result)]._collection()
+    return result._collection()
 
 def _map(collection, f):
+    collection = to_node(collection)
     result = f(collection._values()(Placeholder()))
-    return result._collection()(Call(Symbol("map"), [collection, to_lambda(f).with_arg_types((collection._values(),))]))
+    return collection_result(result)(Call(Symbol("map"), [collection, to_lambda(f).with_arg_types((collection._values(),))]))
 
 def _filter(collection, f):
+    collection = to_node(collection)
     return type(collection)(Call(Symbol("filter"), [collection, to_lambda(f).with_arg_types((collection._values(),))]))
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/features.py` & `diagonal_b6-0.0.4/diagonal_b6/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,23 +168,23 @@
 
     def __str__(self):
         return "<RelationMember %s" % (str(self.id),)
 
 def from_id_proto(p):
     return FeatureID(p.type, p.namespace, p.value)
 
-expression.register_literal("featureIDValue", from_id_proto)
+expression.register_literal_from_proto("featureIDValue", from_id_proto)
 
 def from_applied_change_proto(change):
     applied = {}
     for i in range(0, len(change.original)):
         applied[from_id_proto(change.original[i])] = from_id_proto(change.modified[i])
     return applied
 
-expression.register_literal("appliedChangeValue", from_applied_change_proto)
+expression.register_literal_from_proto("appliedChangeValue", from_applied_change_proto)
 
 def id_to_proto(id):
     pb = features_pb2.FeatureIDProto()
     pb.type = id.type
     pb.namespace = id.namespace
     pb.value = id.value
     return pb
@@ -214,15 +214,15 @@
         return _from_area_proto(p)
     elif oneof == "relation":
         return _from_relation_proto(p)
     elif oneof == None:
         return None
     raise Exception("Unexpected feature %s" % (p,))
 
-expression.register_literal("featureValue", from_proto)
+expression.register_literal_from_proto("featureValue", from_proto)
 
 def osm_node_id(id):
     return FeatureID(FEATURE_TYPE_POINT, NAMESPACE_OSM_NODE, id)
 
 def osm_way_id(id):
     return FeatureID(FEATURE_TYPE_PATH, NAMESPACE_OSM_WAY, id)
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/features_pb2.py` & `diagonal_b6-0.0.4/diagonal_b6/features_pb2.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.3/diagonal_b6/generate_api.py` & `diagonal_b6-0.0.4/diagonal_b6/generate_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 import sys
 import json
 
 from copy import copy
 from datetime import datetime
 
+SPECIAL_FUNCTIONS = ("map", "filter")
+
+COLLECTION_PARENTS = {
+    "PointFeatureCollection": "PointCollection",
+    "PathFeatureCollection": "PathCollection",
+    "AreaFeatureCollection": "AreaCollection",
+}
+
 def name_for_function(name):
     if name in ["or", "and"]:
         return name + "_"
     return name.replace("-", "_")
 
 def name_for_type(t):
     if t == "string":
@@ -44,14 +52,21 @@
 
 def name_for_collection_of_result(t, collections):
     for (name, (key, value)) in collections.items():
         if key == "any" and value == t:
             return name_for_result(name)
     return "CollectionResult"
 
+BUILTIN_RESULTS = {
+    str: name_for_result("string"),
+    int: name_for_result("int"),
+    float: name_for_result("float64"),
+    bool: name_for_result("bool"),
+}
+
 def output_traits(t, functions, collections, hints, parents):
     if len(parents.get(t, [])) > 0:
         print("class %s(%s):" % (name_for_traits(t), ", ".join([name_for_traits(p) for p in parents[t]])))
     else:
         print("class %s:" % name_for_traits(t))
     methods = 0
     for f in functions:            
@@ -110,22 +125,14 @@
     print("        Result.__init__(self, node)")
     print("")
     args = ", ".join(["a%d : %s" % (i, hints[at]) for (i, at) in enumerate(t["Args"])])
     print("    def __call__(self, %s) -> %s:" % (args, hints[t["Result"]]))
     print("        raise NotImplementedError()")
     print("")
 
-SPECIAL_FUNCTIONS = ("map", "filter")
-
-COLLECTION_PARENTS = {
-    "PointFeatureCollection": "PointCollection",
-    "PathFeatureCollection": "PathCollection",
-    "AreaFeatureCollection": "AreaCollection",
-}
-
 def ancestors(t, parents):
     queue = copy(parents.get(t, []))
     ancestors = []
     while len(queue) > 0:
         ancestors.append(queue.pop())
         queue.extend(parents.get(ancestors[-1], []))
     return ancestors
@@ -136,15 +143,15 @@
     print("# Client library for Diagonal's geospatial analysis engine, b6.")
     print("")
     print("from __future__ import annotations")
     print("")
     print("from typing import Callable")
     print("")
     print("import diagonal_b6.expression")
-    print("from diagonal_b6.expression import Call, Symbol, Lambda, Result")
+    print("from diagonal_b6.expression import Call, Symbol, Lambda, Result, register_builtin_result")
     print("")
     print("VERSION = %s" % repr(api["Version"]))
     print("")
 
     traits = set()
     parents = {}
     hints = {}
@@ -210,15 +217,26 @@
     for t in api["FunctionArgs"]:
         output_function_arg_result(t, hints)
 
     for f in api["Functions"]:
         if f["Name"] in SPECIAL_FUNCTIONS:
             print("%s = diagonal_b6.expression._%s" % (f["Name"], f["Name"]))
         else:
-            signature = ", ".join(["a%d: %s" % (i, hints[a]) for (i, a) in enumerate(f["Args"])])
+            signature_args = ["a%d: %s" % (i, hints[a]) for (i, a) in enumerate(f["Args"])]
+            if f["IsVariadic"]:
+                signature_args[-1] = "*" + signature_args[-1]
+            signature = ", ".join(signature_args)
             print("def %s(%s) -> %s:" % (name_for_function(f["Name"]), signature, hints[f["Result"]]))
-            args = "[" + ", ".join(["a%d" % i for i in range(0, len(f["Args"]))])+ "]"
-            print("    return %s(Call(Symbol(%s), %s))" % (name_for_result(f["Result"]), repr(f["Name"]), args))
+            n = len(f["Args"])
+            if f["IsVariadic"]:
+                n -= 1
+            print("    args = [%s]" % ", ".join(["a%d" % i for i in range(0, n)]))
+            if f["IsVariadic"]:
+                print("    args.extend(a%d)" % (len(f["Args"]) - 1))
+            print("    return %s(Call(Symbol(%s), args))" % (name_for_result(f["Result"]), repr(f["Name"])))
         print("")
 
+    for type, result in BUILTIN_RESULTS.items():
+        print("register_builtin_result(%s,%s)" % (type.__name__, result))
+
 if __name__ == "__main__":
     main()
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/geometry.py` & `diagonal_b6-0.0.4/diagonal_b6/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from diagonal_b6 import api_pb2
 from diagonal_b6 import geometry_pb2
 
 def from_point_proto(p):
     return (float(p.lat_e7) / 1e7, float(p.lng_e7) / 1e7)
 
-expression.register_literal("pointValue", from_point_proto)
+expression.register_literal_from_proto("pointValue", from_point_proto)
 
 def to_point_proto(ll):
     p = geometry_pb2.PointProto()
     p.lat_e7 = int(ll[0] * 1e7)
     p.lng_e7 = int(ll[1] * 1e7)
     return p
 
 def from_polyline_proto(p):
     return Polyline(p)
 
-expression.register_literal("pathValue", from_polyline_proto)
+expression.register_literal_from_proto("pathValue", from_polyline_proto)
 
 def from_multipolygon_proto(p):
     return MultiPolygon(p)
 
-expression.register_literal("areaValue", from_multipolygon_proto)
+expression.register_literal_from_proto("areaValue", from_multipolygon_proto)
 
 class Polyline(expression.Node):
 
     def __init__(self, pb):
         self._pb = pb
 
     def length_meters(self):
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6/geometry_pb2.py` & `diagonal_b6-0.0.4/diagonal_b6/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.3/diagonal_b6/query.py` & `diagonal_b6-0.0.4/diagonal_b6/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         l = api_pb2.LiteralNodeProto()
         l.queryValue.CopyFrom(self.query)
         return l
 
 def from_proto(pb):
     return Query(pb)
 
-expression.register_literal("queryValue", from_proto)
+expression.register_literal_from_proto("queryValue", from_proto)
 
 def union(*queries):
     q = api_pb2.QueryProto()
     for query in queries:
         _flattern_union(q, query.query)
     return Query(q)
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6.egg-info/PKG-INFO` & `diagonal_b6-0.0.4/diagonal_b6.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagonal-b6
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
 Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `diagonal_b6-0.0.3/diagonal_b6.egg-info/SOURCES.txt` & `diagonal_b6-0.0.4/diagonal_b6.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 README.md
 pyproject.toml
 diagonal_b6/__init__.py
 diagonal_b6/api_generated.py
 diagonal_b6/api_pb2.py
 diagonal_b6/api_pb2_grpc.py
 diagonal_b6/b6_test.py
-diagonal_b6/collection.py
 diagonal_b6/connect.py
 diagonal_b6/expression.py
 diagonal_b6/features.py
 diagonal_b6/features_pb2.py
 diagonal_b6/generate_api.py
 diagonal_b6/geometry.py
 diagonal_b6/geometry_pb2.py
```

### Comparing `diagonal_b6-0.0.3/pyproject.toml` & `diagonal_b6-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diagonal_b6"
 description = "A Python client library for b6, Diagonal's geospatial analysis engine."
 readme = "README.md"
 license = {text = "Apache License"}
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Diagonal Works", email="hello@diagonal.works"},
 ]
 requires-python = ">=3.10"
 dependencies = [
     "grpcio>=1.43.0",
     "protobuf>=3.14.0",
```

