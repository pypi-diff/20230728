# Comparing `tmp/aiearth-engine-3.0.2.tar.gz` & `tmp/aiearth-engine-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiearth-engine-3.0.2.tar", last modified: Mon Jun 12 02:55:28 2023, max compression
+gzip compressed data, was "aiearth-engine-3.1.0.tar", last modified: Fri Jul 28 07:39:25 2023, max compression
```

## Comparing `aiearth-engine-3.0.2.tar` & `aiearth-engine-3.1.0.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.999801 aiearth-engine-3.0.2/
--rw-r--r--   0 songci     (502) staff       (20)       32 2023-05-18 06:35:57.000000 aiearth-engine-3.0.2/MANIFEST.in
--rw-r--r--   0 songci     (502) staff       (20)      421 2023-06-12 02:55:27.999065 aiearth-engine-3.0.2/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aiearth-engine-3.0.2/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.938815 aiearth-engine-3.0.2/aiearth/
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.947667 aiearth-engine-3.0.2/aiearth/engine/
--rw-r--r--   0 songci     (502) staff       (20)     1376 2023-06-12 02:54:39.000000 aiearth-engine-3.0.2/aiearth/engine/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2362 2023-05-18 02:00:14.000000 aiearth-engine-3.0.2/aiearth/engine/aie_env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.959107 aiearth-engine-3.0.2/aiearth/engine/aie_object/
--rw-r--r--   0 songci     (502) staff       (20)    16912 2023-06-12 02:54:38.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/classifier.py
--rw-r--r--   0 songci     (502) staff       (20)     5393 2023-06-12 02:54:31.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/collection.py
--rw-r--r--   0 songci     (502) staff       (20)     3061 2023-06-12 02:54:39.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/confusion_matrix.py
--rw-r--r--   0 songci     (502) staff       (20)    25558 2023-06-12 02:54:34.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/feature.py
--rw-r--r--   0 songci     (502) staff       (20)    28093 2023-06-12 02:54:35.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/feature_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    23020 2023-06-12 02:54:36.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/filter.py
--rw-r--r--   0 songci     (502) staff       (20)    24475 2023-06-12 02:54:33.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/geometry.py
--rw-r--r--   0 songci     (502) staff       (20)    83655 2023-06-12 02:54:31.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/image.py
--rw-r--r--   0 songci     (502) staff       (20)    24406 2023-06-12 02:54:32.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/image_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    29409 2023-06-12 02:54:38.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/kernel.py
--rw-r--r--   0 songci     (502) staff       (20)     1558 2023-06-12 02:54:39.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/model.py
--rw-r--r--   0 songci     (502) staff       (20)    14258 2023-06-12 02:54:36.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/reducer.py
--rw-r--r--   0 songci     (502) staff       (20)     3123 2023-06-12 02:54:37.000000 aiearth-engine-3.0.2/aiearth/engine/aie_object/terrain.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.964491 aiearth-engine-3.0.2/aiearth/engine/client/
--rw-r--r--   0 songci     (502) staff       (20)      265 2023-05-18 01:46:50.000000 aiearth-engine-3.0.2/aiearth/engine/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     3035 2023-05-17 12:22:50.000000 aiearth-engine-3.0.2/aiearth/engine/client/client.py
--rw-r--r--   0 songci     (502) staff       (20)     3305 2023-05-17 12:22:50.000000 aiearth-engine-3.0.2/aiearth/engine/client/dataset.py
--rw-r--r--   0 songci     (502) staff       (20)     8279 2023-05-17 12:32:13.000000 aiearth-engine-3.0.2/aiearth/engine/client/interactive_session.py
--rw-r--r--   0 songci     (502) staff       (20)     1768 2023-05-17 13:12:06.000000 aiearth-engine-3.0.2/aiearth/engine/client/maps.py
--rw-r--r--   0 songci     (502) staff       (20)     2555 2023-05-18 01:46:50.000000 aiearth-engine-3.0.2/aiearth/engine/client/task.py
--rw-r--r--   0 songci     (502) staff       (20)      183 2023-05-18 02:00:14.000000 aiearth-engine-3.0.2/aiearth/engine/customfunction_node.py
--rw-r--r--   0 songci     (502) staff       (20)     4320 2023-05-18 02:07:20.000000 aiearth-engine-3.0.2/aiearth/engine/export.py
--rw-r--r--   0 songci     (502) staff       (20)     1796 2023-05-18 06:40:03.000000 aiearth-engine-3.0.2/aiearth/engine/function_helper.py
--rw-r--r--   0 songci     (502) staff       (20)      514 2023-05-18 02:00:14.000000 aiearth-engine-3.0.2/aiearth/engine/function_node.py
--rw-r--r--   0 songci     (502) staff       (20)    11542 2023-05-17 12:26:48.000000 aiearth-engine-3.0.2/aiearth/engine/gen_python_functions.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.968854 aiearth-engine-3.0.2/aiearth/engine/map/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aiearth-engine-3.0.2/aiearth/engine/map/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aiearth-engine-3.0.2/aiearth/engine/map/aie_color.py
--rw-r--r--   0 songci     (502) staff       (20)     8621 2023-05-18 06:43:22.000000 aiearth-engine-3.0.2/aiearth/engine/map/aie_layer.py
--rw-r--r--   0 songci     (502) staff       (20)     4998 2023-05-18 01:46:50.000000 aiearth-engine-3.0.2/aiearth/engine/map/aie_map.py
--rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aiearth-engine-3.0.2/aiearth/engine/map/color.csv
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.972433 aiearth-engine-3.0.2/aiearth/engine/serialize/
--rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aiearth-engine-3.0.2/aiearth/engine/serialize/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     4713 2023-05-18 01:50:02.000000 aiearth-engine-3.0.2/aiearth/engine/serialize/gen_visitor.py
--rw-r--r--   0 songci     (502) staff       (20)     3376 2023-05-18 02:00:14.000000 aiearth-engine-3.0.2/aiearth/engine/serialize/optimizer.py
--rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aiearth-engine-3.0.2/aiearth/engine/serialize/serializer_impl.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.973287 aiearth-engine-3.0.2/aiearth/engine/template/
--rw-r--r--   0 songci     (502) staff       (20)    12738 2023-05-17 13:00:06.000000 aiearth-engine-3.0.2/aiearth/engine/template/plugin_impl.py
--rw-r--r--   0 songci     (502) staff       (20)      222 2023-05-18 02:07:20.000000 aiearth-engine-3.0.2/aiearth/engine/variable_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-12 02:55:27.977703 aiearth-engine-3.0.2/aiearth_engine.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      421 2023-06-12 02:55:27.000000 aiearth-engine-3.0.2/aiearth_engine.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)     1539 2023-06-12 02:55:27.000000 aiearth-engine-3.0.2/aiearth_engine.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-06-12 02:55:27.000000 aiearth-engine-3.0.2/aiearth_engine.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)      113 2023-06-12 02:55:27.000000 aiearth-engine-3.0.2/aiearth_engine.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        8 2023-06-12 02:55:27.000000 aiearth-engine-3.0.2/aiearth_engine.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-06-12 02:55:27.999946 aiearth-engine-3.0.2/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)      993 2023-05-26 05:54:21.000000 aiearth-engine-3.0.2/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.411174 aiearth-engine-3.1.0/
+-rw-r--r--   0 songci     (502) staff       (20)       32 2023-05-18 06:35:57.000000 aiearth-engine-3.1.0/MANIFEST.in
+-rw-r--r--   0 songci     (502) staff       (20)      421 2023-07-28 07:39:25.410545 aiearth-engine-3.1.0/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aiearth-engine-3.1.0/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.345198 aiearth-engine-3.1.0/aiearth/
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.375756 aiearth-engine-3.1.0/aiearth/engine/
+-rw-r--r--   0 songci     (502) staff       (20)     1478 2023-07-28 07:39:23.000000 aiearth-engine-3.1.0/aiearth/engine/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2362 2023-05-18 02:00:14.000000 aiearth-engine-3.1.0/aiearth/engine/aie_env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.387137 aiearth-engine-3.1.0/aiearth/engine/aie_object/
+-rw-r--r--   0 songci     (502) staff       (20)    16943 2023-07-28 07:39:21.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/classifier.py
+-rw-r--r--   0 songci     (502) staff       (20)     8846 2023-07-28 07:39:15.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/collection.py
+-rw-r--r--   0 songci     (502) staff       (20)     3351 2023-07-28 07:39:21.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/confusion_matrix.py
+-rw-r--r--   0 songci     (502) staff       (20)    25713 2023-07-28 07:39:17.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/feature.py
+-rw-r--r--   0 songci     (502) staff       (20)    29340 2023-07-28 07:39:18.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/feature_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    23051 2023-07-28 07:39:19.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/filter.py
+-rw-r--r--   0 songci     (502) staff       (20)    25269 2023-07-28 07:39:16.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/geometry.py
+-rw-r--r--   0 songci     (502) staff       (20)    84476 2023-07-28 07:39:14.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/image.py
+-rw-r--r--   0 songci     (502) staff       (20)    25868 2023-07-28 07:39:16.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/image_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    29440 2023-07-28 07:39:20.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/kernel.py
+-rw-r--r--   0 songci     (502) staff       (20)     2365 2023-07-28 07:39:22.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/list.py
+-rw-r--r--   0 songci     (502) staff       (20)     1589 2023-07-28 07:39:22.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/model.py
+-rw-r--r--   0 songci     (502) staff       (20)    17409 2023-07-28 07:39:23.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/number.py
+-rw-r--r--   0 songci     (502) staff       (20)    14289 2023-07-28 07:39:19.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/reducer.py
+-rw-r--r--   0 songci     (502) staff       (20)     3154 2023-07-28 07:39:20.000000 aiearth-engine-3.1.0/aiearth/engine/aie_object/terrain.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.390231 aiearth-engine-3.1.0/aiearth/engine/client/
+-rw-r--r--   0 songci     (502) staff       (20)      265 2023-05-18 01:46:50.000000 aiearth-engine-3.1.0/aiearth/engine/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     3035 2023-05-17 12:22:50.000000 aiearth-engine-3.1.0/aiearth/engine/client/client.py
+-rw-r--r--   0 songci     (502) staff       (20)     3305 2023-05-17 12:22:50.000000 aiearth-engine-3.1.0/aiearth/engine/client/dataset.py
+-rw-r--r--   0 songci     (502) staff       (20)     8279 2023-05-17 12:32:13.000000 aiearth-engine-3.1.0/aiearth/engine/client/interactive_session.py
+-rw-r--r--   0 songci     (502) staff       (20)     1768 2023-05-17 13:12:06.000000 aiearth-engine-3.1.0/aiearth/engine/client/maps.py
+-rw-r--r--   0 songci     (502) staff       (20)     2555 2023-05-18 01:46:50.000000 aiearth-engine-3.1.0/aiearth/engine/client/task.py
+-rw-r--r--   0 songci     (502) staff       (20)      183 2023-05-18 02:00:14.000000 aiearth-engine-3.1.0/aiearth/engine/customfunction_node.py
+-rw-r--r--   0 songci     (502) staff       (20)     4390 2023-07-04 03:13:17.000000 aiearth-engine-3.1.0/aiearth/engine/export.py
+-rw-r--r--   0 songci     (502) staff       (20)     1958 2023-07-26 05:37:35.000000 aiearth-engine-3.1.0/aiearth/engine/function_helper.py
+-rw-r--r--   0 songci     (502) staff       (20)      514 2023-05-18 02:00:14.000000 aiearth-engine-3.1.0/aiearth/engine/function_node.py
+-rw-r--r--   0 songci     (502) staff       (20)    11542 2023-05-17 12:26:48.000000 aiearth-engine-3.1.0/aiearth/engine/gen_python_functions.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.394431 aiearth-engine-3.1.0/aiearth/engine/map/
+-rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aiearth-engine-3.1.0/aiearth/engine/map/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aiearth-engine-3.1.0/aiearth/engine/map/aie_color.py
+-rw-r--r--   0 songci     (502) staff       (20)     8621 2023-05-18 06:43:22.000000 aiearth-engine-3.1.0/aiearth/engine/map/aie_layer.py
+-rw-r--r--   0 songci     (502) staff       (20)     4998 2023-05-18 01:46:50.000000 aiearth-engine-3.1.0/aiearth/engine/map/aie_map.py
+-rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aiearth-engine-3.1.0/aiearth/engine/map/color.csv
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.399028 aiearth-engine-3.1.0/aiearth/engine/serialize/
+-rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aiearth-engine-3.1.0/aiearth/engine/serialize/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     5132 2023-07-28 04:07:20.000000 aiearth-engine-3.1.0/aiearth/engine/serialize/gen_visitor.py
+-rw-r--r--   0 songci     (502) staff       (20)     3376 2023-05-18 02:00:14.000000 aiearth-engine-3.1.0/aiearth/engine/serialize/optimizer.py
+-rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aiearth-engine-3.1.0/aiearth/engine/serialize/serializer_impl.py
+-rw-r--r--   0 songci     (502) staff       (20)     3593 2023-07-28 04:07:20.000000 aiearth-engine-3.1.0/aiearth/engine/serialize/udf_manager.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.400165 aiearth-engine-3.1.0/aiearth/engine/template/
+-rw-r--r--   0 songci     (502) staff       (20)    15076 2023-07-26 08:30:46.000000 aiearth-engine-3.1.0/aiearth/engine/template/plugin_impl.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.405795 aiearth-engine-3.1.0/aiearth/engine/udf_base/
+-rwxr-xr-x   0 songci     (502) staff       (20)     2029 2023-07-25 12:46:18.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/UDFImages_pb2.py
+-rwxr-xr-x   0 songci     (502) staff       (20)       46 2023-07-25 12:46:18.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/__init__.py
+-rwxr-xr-x   0 songci     (502) staff       (20)      564 2023-07-25 12:46:18.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/aie_udf_base.py
+-rw-r--r--   0 songci     (502) staff       (20)     2648 2023-07-28 04:07:20.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/annotation.py
+-rwxr-xr-x   0 songci     (502) staff       (20)      927 2023-07-25 12:46:18.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/images.py
+-rwxr-xr-x   0 songci     (502) staff       (20)     4420 2023-07-27 06:54:58.000000 aiearth-engine-3.1.0/aiearth/engine/udf_base/udf_utils.py
+-rw-r--r--   0 songci     (502) staff       (20)      222 2023-05-18 02:07:20.000000 aiearth-engine-3.1.0/aiearth/engine/variable_node.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-07-28 07:39:25.409618 aiearth-engine-3.1.0/aiearth_engine.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      421 2023-07-28 07:39:24.000000 aiearth-engine-3.1.0/aiearth_engine.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)     1875 2023-07-28 07:39:24.000000 aiearth-engine-3.1.0/aiearth_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-07-28 07:39:24.000000 aiearth-engine-3.1.0/aiearth_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)      253 2023-07-28 07:39:24.000000 aiearth-engine-3.1.0/aiearth_engine.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        8 2023-07-28 07:39:24.000000 aiearth-engine-3.1.0/aiearth_engine.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-07-28 07:39:25.411341 aiearth-engine-3.1.0/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)      993 2023-05-26 05:54:21.000000 aiearth-engine-3.1.0/setup.py
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/__init__.py` & `aiearth-engine-3.1.0/aiearth/engine/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = "3.0.2"
+__version__ = "3.1.0"
 
 import aiearth.core
 
 from aiearth.engine.aie_env import AIEEnv
 from aiearth.core import g_var
 from aiearth.engine import serialize
 from aiearth.core import auth
@@ -36,14 +36,18 @@
 
 from aiearth.engine.aie_object.classifier import Classifier
 
 from aiearth.engine.aie_object.confusion_matrix import ConfusionMatrix
 
 from aiearth.engine.aie_object.model import Model
 
+from aiearth.engine.aie_object.list import List
+
+from aiearth.engine.aie_object.number import Number
+
 
 Authenticate = aiearth.core.Authenticate
 
 
 def Initialize(debug_level=g_var.LogLevel.INFO_LEVEL, debug=False):
     if debug:
         debug_level = g_var.LogLevel.DEBUG_LEVEL
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_env.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_env.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/classifier.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/collection.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/collection.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -152,7 +153,96 @@
         }
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         if "baseAlgorithm" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数baseAlgorithm不能为空")
 
         return FunctionHelper.apply("Collection.map", "engine.Collection", invoke_args)
+
+    def iterate(self, func: FunctionType, first: object) -> object:
+        if func is not None and not isinstance(func, FunctionType):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"func 只支持FunctionType类型参数, 传入类型为{type(func)}"
+            )
+
+        if first is not None and not isinstance(first, object):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"first 只支持object类型参数, 传入类型为{type(first)}"
+            )
+
+        args = inspect.getfullargspec(func).args
+        mapping_args = [
+            "_MAPPING_VAR_#arg" + str(k) + "_" + v for k, v in enumerate(args)
+        ]
+        variables = [VariableNode(mapping_arg) for mapping_arg in mapping_args]
+
+        element_type = self.elementType()
+
+        def func_warp(collection_element_self, param_object: object):
+            return func(element_type(collection_element_self), param_object)
+
+        from copy import deepcopy
+
+        deepcopy_first = deepcopy(first)
+        setattr(deepcopy_first, "iterables", variables[1].var_name)
+        body = func_warp(variables[0], deepcopy_first)
+        if body is None:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "自定义map函数必须有返回值")
+        customfunc = CustomFunctionNode(mapping_args, body)
+
+        invoke_args = {
+            "collection": self,
+            "baseAlgorithm": customfunc,
+            "first": first,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "baseAlgorithm" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数func不能为空")
+
+        if "first" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数first不能为空")
+
+        return FunctionHelper.apply("Collection.iterate", "object", invoke_args)
+
+    def remap(
+        self, lookupIn: list, lookupOut: list, columnName: str
+    ) -> engine.Collection:
+        if lookupIn is not None and not isinstance(lookupIn, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"lookupIn 只支持list类型参数, 传入类型为{type(lookupIn)}"
+            )
+
+        if lookupOut is not None and not isinstance(lookupOut, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"lookupOut 只支持list类型参数, 传入类型为{type(lookupOut)}",
+            )
+
+        if columnName is not None and not isinstance(columnName, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"columnName 只支持str类型参数, 传入类型为{type(columnName)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "lookupIn": lookupIn,
+            "lookupOut": lookupOut,
+            "columnName": columnName,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "lookupIn" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数lookupIn不能为空")
+
+        if "lookupOut" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数lookupOut不能为空")
+
+        if "columnName" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数columnName不能为空")
+
+        return FunctionHelper.apply(
+            "Collection.remap", "engine.Collection", invoke_args
+        )
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/confusion_matrix.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/confusion_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -94,7 +95,16 @@
         invoke_args = {
             "input": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("ConfusionMatrix.array", "object", invoke_args)
+
+    def labels(self) -> object:
+        invoke_args = {
+            "input": self,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("ConfusionMatrix.labels", "object", invoke_args)
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/feature.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
 
 
 class Feature(FunctionNode):
     def __init__(self, geometry, properties=None) -> engine.Feature:
         args = geometry
         if isinstance(args, engine.Geometry):
-            if properties is not None and not isinstance(properties, dict):
+            if properties is not None and not isinstance(
+                properties, (dict, engine.function_node.FunctionNode)
+            ):
                 raise AIEError(
                     AIEErrorCode.ARGS_ERROR,
-                    f"properties 只支持dict类型参数, 传入类型为{type(properties)}",
+                    f"properties 只支持dict|engine.function_node.FunctionNode类型参数, 传入类型为{type(properties)}",
                 )
 
             invoke_args = {
                 "geometry": geometry,
                 "properties": properties,
             }
 
@@ -172,18 +175,19 @@
             "properties": properties,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Feature.toDictionary", "object", invoke_args)
 
-    def set(self, var_args: dict) -> engine.Feature:
-        if var_args is not None and not isinstance(var_args, dict):
+    def set(self, var_args: object) -> engine.Feature:
+        if var_args is not None and not isinstance(var_args, object):
             raise AIEError(
-                AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
+                AIEErrorCode.ARGS_ERROR,
+                f"var_args 只支持object类型参数, 传入类型为{type(var_args)}",
             )
 
         invoke_args = {
             "element": self,
             "var_args": var_args,
         }
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/feature_collection.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/feature_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -30,18 +31,22 @@
             )
         elif isinstance(args, (list, tuple)):
             features = [engine.Feature(i) for i in args]
             invoke_args = {"features": features}
             super(FeatureCollection, self).__init__(
                 "FeatureCollection.fromFeatures", invoke_args
             )
+        elif isinstance(args, engine.List):
+            super(FeatureCollection, self).__init__(
+                "FeatureCollection.fromFeatures", {"features": args}
+            )
         else:
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
-                f"args 只支持str|engine.Feature|list类型参数, 传入类型为{type(args)}",
+                f"args 只支持str|engine.Feature|list|engine.List类型参数, 传入类型为{type(args)}",
             )
 
     def getMapId(self, vis_params):
         if vis_params is not None and not isinstance(vis_params, dict):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
                 f"vis_params 只支持dict类型参数, 传入类型为{type(vis_params)}",
@@ -759,7 +764,36 @@
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.renamePropertyNames",
             "engine.FeatureCollection",
             invoke_args,
         )
+
+    def makeArray(
+        self, properties: list, name: str = "array"
+    ) -> engine.FeatureCollection:
+        if properties is not None and not isinstance(properties, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"properties 只支持list类型参数, 传入类型为{type(properties)}",
+            )
+
+        if name is not None and not isinstance(name, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"name 只支持str类型参数, 传入类型为{type(name)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "properties": properties,
+            "name": name,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "properties" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数properties不能为空")
+
+        return FunctionHelper.apply(
+            "FeatureCollection.makeArray", "engine.FeatureCollection", invoke_args
+        )
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/filter.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/geometry.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -690,7 +691,28 @@
         invoke_args = {
             "geometry": self,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply("Geometry.geometries", "object", invoke_args)
+
+    def coveringGrid(self, interval: [int, float]) -> engine.FeatureCollection:
+        if interval is not None and not isinstance(interval, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"interval 只支持(int,float)类型参数, 传入类型为{type(interval)}",
+            )
+
+        invoke_args = {
+            "geometry": self,
+            "interval": interval,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "interval" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数interval不能为空")
+
+        return FunctionHelper.apply(
+            "Geometry.coveringGrid", "engine.FeatureCollection", invoke_args
+        )
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/image.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -2381,7 +2382,31 @@
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         if "var_args" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
 
         return FunctionHelper.apply("Image.set", "engine.Image", invoke_args)
+
+    def glcmTexture(self, size: int = 1) -> engine.Image:
+        if size is not None and not isinstance(size, int):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"size 只支持int类型参数, 传入类型为{type(size)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "size": size,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Image.glcmTexture", "engine.Image", invoke_args)
+
+    def zeroCrossing(self) -> engine.Image:
+        invoke_args = {
+            "input": self,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Image.zeroCrossing", "engine.Image", invoke_args)
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/image_collection.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/image_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
@@ -28,18 +29,22 @@
             )
         elif isinstance(args, (list, tuple)):
             images = [engine.Image(i) for i in args]
             invoke_args = {"images": images}
             super(ImageCollection, self).__init__(
                 "ImageCollection.fromImages", invoke_args
             )
+        elif isinstance(args, engine.List):
+            super(ImageCollection, self).__init__(
+                "ImageCollection.fromImages", {"images": args}
+            )
         else:
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR,
-                f"args 只支持str|engine.Image|list类型参数, 传入类型为{type(args)}",
+                f"args 只支持str|engine.Image|list|engine.List类型参数, 传入类型为{type(args)}",
             )
 
     def elementType(self):
         return engine.Image
 
     def getMapId(self, vis_params):
         if vis_params is not None and not isinstance(vis_params, dict):
@@ -325,18 +330,19 @@
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         return FunctionHelper.apply(
             "ImageCollection.toBands", "engine.Image", invoke_args
         )
 
     @staticmethod
-    def fromImages(images: list) -> engine.ImageCollection:
-        if images is not None and not isinstance(images, list):
+    def fromImages(images: Union[list, engine.List]) -> engine.ImageCollection:
+        if images is not None and not isinstance(images, (list, engine.List)):
             raise AIEError(
-                AIEErrorCode.ARGS_ERROR, f"images 只支持list类型参数, 传入类型为{type(images)}"
+                AIEErrorCode.ARGS_ERROR,
+                f"images 只支持(list,engine.List)类型参数, 传入类型为{type(images)}",
             )
 
         invoke_args = {
             "images": images,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
@@ -687,7 +693,38 @@
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
 
         return FunctionHelper.apply(
             "ImageCollection.aggregate_first", "object", invoke_args
         )
+
+    def reduceToImage(self, properties: list, reducer: engine.Reducer) -> engine.Image:
+        if properties is not None and not isinstance(properties, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"properties 只支持list类型参数, 传入类型为{type(properties)}",
+            )
+
+        if reducer is not None and not isinstance(reducer, engine.Reducer):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"reducer 只支持engine.Reducer类型参数, 传入类型为{type(reducer)}",
+            )
+
+        invoke_args = {
+            "collection": self,
+            "properties": properties,
+            "reducer": reducer,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "properties" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数properties不能为空")
+
+        if "reducer" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数reducer不能为空")
+
+        return FunctionHelper.apply(
+            "ImageCollection.reduceToImage", "engine.Image", invoke_args
+        )
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/kernel.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/model.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/reducer.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/reducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/aie_object/terrain.py` & `aiearth-engine-3.1.0/aiearth/engine/aie_object/terrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import abc
 import inspect
 from typing import Union
+from types import FunctionType
 
 from aiearth import engine
 from aiearth.engine.variable_node import VariableNode
 from aiearth.engine.function_node import FunctionNode
 from aiearth.engine.customfunction_node import CustomFunctionNode
 from aiearth.engine.function_helper import FunctionHelper
 from aiearth.core.error.aie_error import AIEError, AIEErrorCode
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/client/client.py` & `aiearth-engine-3.1.0/aiearth/engine/client/client.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/client/dataset.py` & `aiearth-engine-3.1.0/aiearth/engine/client/dataset.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/client/interactive_session.py` & `aiearth-engine-3.1.0/aiearth/engine/client/interactive_session.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/client/maps.py` & `aiearth-engine-3.1.0/aiearth/engine/client/maps.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/client/task.py` & `aiearth-engine-3.1.0/aiearth/engine/client/task.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/export.py` & `aiearth-engine-3.1.0/aiearth/engine/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 from aiearth.core.g_var import *
 from aiearth.core.auth import Authenticate
 
 
 class Export(object):
     class image(object):
         @staticmethod
-        def toAsset(image: engine.Image, assetId: str, scale: int = 1000, config: dict = None):
+        def toAsset(image: engine.Image, assetId: str, scale: int = 1000, config: dict = None, needPyramid: bool = True):
             if not isinstance(image, engine.Image):
                 raise AIEError(AIEErrorCode.ARGS_ERROR,
                                f"image 只支持 aie.Image 类型参数, 传入类型为{type(image)}")
             if not isinstance(assetId, str):
                 raise AIEError(AIEErrorCode.ARGS_ERROR,
                                f"assetId 只支持 str 类型参数, 传入类型为{type(image)}")
 
             options = {
                 "taskType": "ExportImage",
                 "assetId": assetId,
                 "scale": scale,
-                "function": "image.toAsset"
+                "function": "image.toAsset",
+                "needPyramid": needPyramid
             }
 
             if config is not None:
                 options["config"] = config
             return Task(image, options)
 
     class feature(object):
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/function_helper.py` & `aiearth-engine-3.1.0/aiearth/engine/function_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,18 @@
             node.__class__ = engine.Terrain
         elif kclass == "engine.Kernel":
             node.__class__ = engine.Kernel
         elif kclass == "engine.Classifier":
             node.__class__ = engine.Classifier
         elif kclass == "engine.ConfusionMatrix":
             node.__class__ = engine.ConfusionMatrix
+        elif kclass == 'engine.List':
+            node.__class__ = engine.List
+        elif kclass == 'engine.Number':
+            node.__class__ = engine.Number
         elif kclass in ("int", "float", "bool", "str", "list", "tuple", "dict", "object"):
             pass
         else:
             raise AIEError(AIEErrorCode.DEFAULT_INTERNAL_ERROR,
                            "", "FunctionHelper::cast kclass " + kclass + " not support")
         return node
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/function_node.py` & `aiearth-engine-3.1.0/aiearth/engine/function_node.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/gen_python_functions.py` & `aiearth-engine-3.1.0/aiearth/engine/gen_python_functions.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/map/aie_color.py` & `aiearth-engine-3.1.0/aiearth/engine/map/aie_color.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/map/aie_layer.py` & `aiearth-engine-3.1.0/aiearth/engine/map/aie_layer.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/map/aie_map.py` & `aiearth-engine-3.1.0/aiearth/engine/map/aie_map.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/map/color.csv` & `aiearth-engine-3.1.0/aiearth/engine/map/color.csv`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/serialize/gen_visitor.py` & `aiearth-engine-3.1.0/aiearth/engine/serialize/gen_visitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+from aiearth.engine.aie_object.list import List
 
 from aiearth import engine
 import collections
 from aiearth.core.error import AIEError, AIEErrorCode
+from types import FunctionType
+from aiearth.engine.serialize.udf_manager import manage
 
 class GenVisitor(object):
     def __init__(self, is_compacted=True):
         self.is_compacted = is_compacted
         # {obj_id: ref}
         self.refs = {}
         # [(ref, value)]
@@ -19,15 +22,19 @@
         obj_id = id(obj)
         if self.is_compacted:
             ref = self.refs.get(obj_id, None)
             if ref:
                 self.ref_uses_cnt[ref] += 1
                 return ref
 
-        if isinstance(obj, engine.customfunction_node.CustomFunctionNode):
+        if hasattr(obj, "iterables"):
+            result = {
+                    "argumentReference": getattr(obj, "iterables")
+                }
+        elif isinstance(obj, engine.customfunction_node.CustomFunctionNode):
             result = {
                 "functionDefinitionValue": {
                     "argumentNames": obj.arg_names,
                     "body": self.visit(obj.body)
                 }
             }
         elif isinstance(obj, engine.function_node.FunctionNode):
@@ -109,14 +116,17 @@
                     }
                 else:
                     result = {
                         "dictionaryValue": {
                             "values": values
                         }
                     }
+        # elif isinstance(obj, FunctionType):
+        #     func_uuid = manage(obj)
+        #     result = {"constantValue": func_uuid}
         else:
             raise AIEError(AIEErrorCode.DEFAULT_INTERNAL_ERROR,
                                                "", "serialize.GenVisitor.visit not support obj type %s" % type(
                                                    obj)
                                                )
 
         if self.is_compacted:
```

### Comparing `aiearth-engine-3.0.2/aiearth/engine/serialize/optimizer.py` & `aiearth-engine-3.1.0/aiearth/engine/serialize/optimizer.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/serialize/serializer_impl.py` & `aiearth-engine-3.1.0/aiearth/engine/serialize/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `aiearth-engine-3.0.2/aiearth/engine/template/plugin_impl.py` & `aiearth-engine-3.1.0/aiearth/engine/template/plugin_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,24 +52,28 @@
             args = [args]
             invoke_args = {"images": args}
             super(ImageCollection, self).__init__("ImageCollection.fromImages", invoke_args)
         elif isinstance(args, (list, tuple)):
             images = [engine.Image(i) for i in args]
             invoke_args = {"images": images}
             super(ImageCollection, self).__init__("ImageCollection.fromImages", invoke_args)
+        elif isinstance(args, engine.List):
+            super(ImageCollection, self).__init__(
+                "ImageCollection.fromImages", {"images": args}
+            )
         else:
-            raise AIEError(AIEErrorCode.ARGS_ERROR, f"args 只支持str|engine.Image|list类型参数, 传入类型为{type(args)}")
+            raise AIEError(AIEErrorCode.ARGS_ERROR, f"args 只支持str|engine.Image|list|engine.List类型参数, 传入类型为{type(args)}")
 '''
 
 FeatureConstructorsImpl = '''
     def __init__(self, geometry, properties=None) -> engine.Feature:
         args = geometry
         if isinstance(args, engine.Geometry):
-            if properties is not None and not isinstance(properties, dict):
-                raise AIEError(AIEErrorCode.ARGS_ERROR, f"properties 只支持dict类型参数, 传入类型为{type(properties)}")
+            if properties is not None and not isinstance(properties, (dict, engine.function_node.FunctionNode)):
+                raise AIEError(AIEErrorCode.ARGS_ERROR, f"properties 只支持dict|engine.function_node.FunctionNode类型参数, 传入类型为{type(properties)}")
 
             invoke_args = {
                 "geometry": geometry,
                 "properties": properties,
             }
             
             invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
@@ -100,16 +104,20 @@
             args = [args]
             invoke_args = {"features": args}
             super(FeatureCollection, self).__init__("FeatureCollection.fromFeatures", invoke_args)
         elif isinstance(args, (list, tuple)):
             features = [engine.Feature(i) for i in args]
             invoke_args = {"features": features}
             super(FeatureCollection, self).__init__("FeatureCollection.fromFeatures", invoke_args)
+        elif isinstance(args, engine.List):
+            super(FeatureCollection, self).__init__(
+                "FeatureCollection.fromFeatures", {"features": args}
+            )
         else:
-            raise AIEError(AIEErrorCode.ARGS_ERROR, f"args 只支持str|engine.Feature|list类型参数, 传入类型为{type(args)}")
+            raise AIEError(AIEErrorCode.ARGS_ERROR, f"args 只支持str|engine.Feature|list|engine.List类型参数, 传入类型为{type(args)}")
 '''
 
 CollectionElementTypeImpl = '''
     @abc.abstractmethod
     def elementType(self):
         pass
 '''
@@ -147,14 +155,62 @@
 
         if "baseAlgorithm" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数baseAlgorithm不能为空")
 
         return FunctionHelper.apply("Collection.map", "engine.Collection", invoke_args)
 '''
 
+CollectionIterateImpl = '''
+    def iterate(self, func: FunctionType, first: object) -> object:
+        if func is not None and not isinstance(func, FunctionType):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"func 只支持FunctionType类型参数, 传入类型为{type(func)}"
+            )
+
+        if first is not None and not isinstance(first, object):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"first 只支持object类型参数, 传入类型为{type(first)}"
+            )
+
+        args = inspect.getfullargspec(func).args
+        mapping_args = [
+            "_MAPPING_VAR_#arg" + str(k) + "_" + v for k, v in enumerate(args)
+        ]
+        variables = [VariableNode(mapping_arg) for mapping_arg in mapping_args]
+
+        element_type = self.elementType()
+
+        def func_warp(collection_element_self, param_object: object):
+            return func(element_type(collection_element_self), param_object)
+
+        from copy import deepcopy
+        deepcopy_first = deepcopy(first)
+        setattr(deepcopy_first, "iterables", variables[1].var_name)
+        body = func_warp(variables[0], deepcopy_first)
+        if body is None:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "自定义map函数必须有返回值")
+        customfunc = CustomFunctionNode(mapping_args, body)
+
+        invoke_args = {
+            "collection": self,
+            "baseAlgorithm": customfunc,
+            "first": first,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "baseAlgorithm" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数func不能为空")
+
+        if "first" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数first不能为空")
+
+        return FunctionHelper.apply("Collection.iterate", "object", invoke_args)
+'''
+
 ImageCollectionMapImpl = """
     def map(self, baseAlgorithm: types.FunctionType) -> Union[engine.ImageCollection, engine.FeatureCollection]:
 
         node = super(ImageCollection, self).map(baseAlgorithm)
         baseAlgorithm_return_type = type(node.invoke_args["baseAlgorithm"].body)
         if engine.Feature == baseAlgorithm_return_type:
             return FunctionHelper.cast(node, "engine.FeatureCollection")
```

### Comparing `aiearth-engine-3.0.2/aiearth_engine.egg-info/SOURCES.txt` & `aiearth-engine-3.1.0/aiearth_engine.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 aiearth/engine/aie_object/feature.py
 aiearth/engine/aie_object/feature_collection.py
 aiearth/engine/aie_object/filter.py
 aiearth/engine/aie_object/geometry.py
 aiearth/engine/aie_object/image.py
 aiearth/engine/aie_object/image_collection.py
 aiearth/engine/aie_object/kernel.py
+aiearth/engine/aie_object/list.py
 aiearth/engine/aie_object/model.py
+aiearth/engine/aie_object/number.py
 aiearth/engine/aie_object/reducer.py
 aiearth/engine/aie_object/terrain.py
 aiearth/engine/client/__init__.py
 aiearth/engine/client/client.py
 aiearth/engine/client/dataset.py
 aiearth/engine/client/interactive_session.py
 aiearth/engine/client/maps.py
@@ -33,13 +35,20 @@
 aiearth/engine/map/aie_layer.py
 aiearth/engine/map/aie_map.py
 aiearth/engine/map/color.csv
 aiearth/engine/serialize/__init__.py
 aiearth/engine/serialize/gen_visitor.py
 aiearth/engine/serialize/optimizer.py
 aiearth/engine/serialize/serializer_impl.py
+aiearth/engine/serialize/udf_manager.py
 aiearth/engine/template/plugin_impl.py
+aiearth/engine/udf_base/UDFImages_pb2.py
+aiearth/engine/udf_base/__init__.py
+aiearth/engine/udf_base/aie_udf_base.py
+aiearth/engine/udf_base/annotation.py
+aiearth/engine/udf_base/images.py
+aiearth/engine/udf_base/udf_utils.py
 aiearth_engine.egg-info/PKG-INFO
 aiearth_engine.egg-info/SOURCES.txt
 aiearth_engine.egg-info/dependency_links.txt
 aiearth_engine.egg-info/requires.txt
 aiearth_engine.egg-info/top_level.txt
```

### Comparing `aiearth-engine-3.0.2/setup.py` & `aiearth-engine-3.1.0/setup.py`

 * *Files identical despite different names*

