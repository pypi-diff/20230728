# Comparing `tmp/kfp-dsl-2.1.1.tar.gz` & `tmp/kfp-dsl-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-dsl-2.1.1.tar", last modified: Thu Jul 27 00:47:01 2023, max compression
+gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.6qxs8VML/kfp-dsl-2.1.2.tar", last modified: Fri Jul 28 20:46:22 2023, max compression
```

## Comparing `kfp-dsl-2.1.1.tar` & `kfp-dsl-2.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 00:47:01.848742 kfp-dsl-2.1.1/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      310 2023-07-27 00:47:01.848594 kfp-dsl-2.1.1/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1919 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 00:47:01.841585 kfp-dsl-2.1.1/kfp/
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 00:47:01.846543 kfp-dsl-2.1.1/kfp/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7574 2023-07-27 00:12:18.000000 kfp-dsl-2.1.1/kfp/dsl/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5990 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/base_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5988 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25348 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/component_factory.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/constants.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/container_component_artifact_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1502 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/container_component_class.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1903 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/container_component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15796 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/executor.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3628 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/executor_main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11007 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3472 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1001 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/importer_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5454 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/importer_node.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/kfp_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13620 2023-07-27 00:12:18.000000 kfp-dsl-2.1.1/kfp/dsl/pipeline_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6408 2023-07-27 00:12:18.000000 kfp-dsl-2.1.1/kfp/dsl/pipeline_context.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27196 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/pipeline_task.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16427 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/placeholders.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1528 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/python_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    43004 2023-07-26 22:46:54.000000 kfp-dsl-2.1.1/kfp/dsl/structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/task_final_status.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7683 2023-07-27 00:12:18.000000 kfp-dsl-2.1.1/kfp/dsl/tasks_group.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 00:47:01.847574 kfp-dsl-2.1.1/kfp/dsl/types/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/types/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/types/artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8038 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/types/custom_artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7837 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/types/type_annotations.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19088 2023-07-26 22:46:54.000000 kfp-dsl-2.1.1/kfp/dsl/types/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/v1_modelbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27550 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/v1_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2247 2023-07-26 00:11:33.000000 kfp-dsl-2.1.1/kfp/dsl/yaml_component.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-27 00:47:01.848366 kfp-dsl-2.1.1/kfp_dsl.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      310 2023-07-27 00:47:01.000000 kfp-dsl-2.1.1/kfp_dsl.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1052 2023-07-27 00:47:01.000000 kfp-dsl-2.1.1/kfp_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-07-27 00:47:01.000000 kfp-dsl-2.1.1/kfp_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       55 2023-07-27 00:47:01.000000 kfp-dsl-2.1.1/kfp_dsl.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-07-27 00:47:01.000000 kfp-dsl-2.1.1/kfp_dsl.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-07-27 00:47:01.848787 kfp-dsl-2.1.1/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1095 2023-07-27 00:46:23.000000 kfp-dsl-2.1.1/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      310 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1919 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp/
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7574 2023-07-27 17:14:48.000000 kfp-dsl-2.1.2/kfp/dsl/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5990 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/base_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5988 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25348 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/component_factory.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/constants.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/container_component_artifact_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1502 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/container_component_class.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1903 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/container_component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15796 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/executor.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3628 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/executor_main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11007 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3472 2023-07-27 02:32:25.000000 kfp-dsl-2.1.2/kfp/dsl/graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1001 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/importer_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5454 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/importer_node.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/kfp_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13620 2023-07-27 17:14:48.000000 kfp-dsl-2.1.2/kfp/dsl/pipeline_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6408 2023-07-27 17:14:48.000000 kfp-dsl-2.1.2/kfp/dsl/pipeline_context.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27196 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/pipeline_task.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16427 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/placeholders.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1528 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/python_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    43004 2023-07-26 22:46:54.000000 kfp-dsl-2.1.2/kfp/dsl/structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/task_final_status.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7683 2023-07-27 17:14:48.000000 kfp-dsl-2.1.2/kfp/dsl/tasks_group.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp/dsl/types/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/types/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/types/artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8038 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/types/custom_artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7837 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/types/type_annotations.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19088 2023-07-26 22:46:54.000000 kfp-dsl-2.1.2/kfp/dsl/types/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/v1_modelbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27550 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/v1_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2247 2023-07-26 00:11:33.000000 kfp-dsl-2.1.2/kfp/dsl/yaml_component.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      310 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1052 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       55 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/kfp_dsl.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-07-28 20:46:22.000000 kfp-dsl-2.1.2/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1095 2023-07-28 18:10:05.000000 kfp-dsl-2.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `kfp-dsl-2.1.1/README.md` & `kfp-dsl-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/__init__.py` & `kfp-dsl-2.1.2/kfp/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/base_component.py` & `kfp-dsl-2.1.2/kfp/dsl/base_component.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/component_decorator.py` & `kfp-dsl-2.1.2/kfp/dsl/component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/component_factory.py` & `kfp-dsl-2.1.2/kfp/dsl/component_factory.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/constants.py` & `kfp-dsl-2.1.2/kfp/dsl/constants.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/container_component_artifact_channel.py` & `kfp-dsl-2.1.2/kfp/dsl/container_component_artifact_channel.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/container_component_class.py` & `kfp-dsl-2.1.2/kfp/dsl/container_component_class.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/container_component_decorator.py` & `kfp-dsl-2.1.2/kfp/dsl/container_component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/executor.py` & `kfp-dsl-2.1.2/kfp/dsl/executor.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/executor_main.py` & `kfp-dsl-2.1.2/kfp/dsl/executor_main.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/for_loop.py` & `kfp-dsl-2.1.2/kfp/dsl/for_loop.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/graph_component.py` & `kfp-dsl-2.1.2/kfp/dsl/graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/importer_component.py` & `kfp-dsl-2.1.2/kfp/dsl/importer_component.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/importer_node.py` & `kfp-dsl-2.1.2/kfp/dsl/importer_node.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/kfp_config.py` & `kfp-dsl-2.1.2/kfp/dsl/kfp_config.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/pipeline_channel.py` & `kfp-dsl-2.1.2/kfp/dsl/pipeline_channel.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/pipeline_context.py` & `kfp-dsl-2.1.2/kfp/dsl/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/pipeline_task.py` & `kfp-dsl-2.1.2/kfp/dsl/pipeline_task.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/placeholders.py` & `kfp-dsl-2.1.2/kfp/dsl/placeholders.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/python_component.py` & `kfp-dsl-2.1.2/kfp/dsl/python_component.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/structures.py` & `kfp-dsl-2.1.2/kfp/dsl/structures.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/task_final_status.py` & `kfp-dsl-2.1.2/kfp/dsl/task_final_status.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/tasks_group.py` & `kfp-dsl-2.1.2/kfp/dsl/tasks_group.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/types/__init__.py` & `kfp-dsl-2.1.2/kfp/dsl/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/types/artifact_types.py` & `kfp-dsl-2.1.2/kfp/dsl/types/artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/types/custom_artifact_types.py` & `kfp-dsl-2.1.2/kfp/dsl/types/custom_artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/types/type_annotations.py` & `kfp-dsl-2.1.2/kfp/dsl/types/type_annotations.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/types/type_utils.py` & `kfp-dsl-2.1.2/kfp/dsl/types/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/utils.py` & `kfp-dsl-2.1.2/kfp/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/v1_modelbase.py` & `kfp-dsl-2.1.2/kfp/dsl/v1_modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/v1_structures.py` & `kfp-dsl-2.1.2/kfp/dsl/v1_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp/dsl/yaml_component.py` & `kfp-dsl-2.1.2/kfp/dsl/yaml_component.py`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/kfp_dsl.egg-info/SOURCES.txt` & `kfp-dsl-2.1.2/kfp_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-dsl-2.1.1/setup.py` & `kfp-dsl-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
 setuptools.setup(
     name='kfp-dsl',
-    version='2.1.1',
+    version='2.1.2',
     description='A KFP SDK subpackage containing the DSL and runtime code.',
     author='google',
     author_email='kubeflow-pipelines@google.com',
     url='https://github.com/kubeflow/pipelines',
     packages=setuptools.find_namespace_packages(include=['kfp.*']),
     python_requires='>=3.7.0',
     install_requires=['typing-extensions>=3.7.4,<5; python_version<"3.9"'],
```

