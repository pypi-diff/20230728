# Comparing `tmp/graphreduce-1.5.1.tar.gz` & `tmp/graphreduce-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.5.1.tar", last modified: Tue Jul 25 22:17:22 2023, max compression
+gzip compressed data, was "graphreduce-1.5.2.tar", last modified: Fri Jul 28 02:31:59 2023, max compression
```

## Comparing `graphreduce-1.5.1.tar` & `graphreduce-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.183550 graphreduce-1.5.1/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-25 22:17:22.183436 graphreduce-1.5.1/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.1/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.182356 graphreduce-1.5.1/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.1/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-25 22:08:54.000000 graphreduce-1.5.1/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.5.1/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16596 2023-07-25 22:16:40.000000 graphreduce-1.5.1/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15244 2023-07-25 22:08:27.000000 graphreduce-1.5.1/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 22:17:22.183276 graphreduce-1.5.1/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.1/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 22:17:22.000000 graphreduce-1.5.1/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 22:17:22.183587 graphreduce-1.5.1/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1834 2023-07-25 22:17:12.000000 graphreduce-1.5.1/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:31:59.540444 graphreduce-1.5.2/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-28 02:31:59.540312 graphreduce-1.5.2/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.2/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:31:59.539552 graphreduce-1.5.2/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.2/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-26 01:15:17.000000 graphreduce-1.5.2/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-07-26 01:15:32.000000 graphreduce-1.5.2/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16681 2023-07-26 12:49:53.000000 graphreduce-1.5.2/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15431 2023-07-26 12:48:40.000000 graphreduce-1.5.2/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:31:59.540148 graphreduce-1.5.2/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-28 02:31:59.000000 graphreduce-1.5.2/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-28 02:31:59.000000 graphreduce-1.5.2/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-28 02:31:59.000000 graphreduce-1.5.2/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.2/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-07-28 02:31:59.000000 graphreduce-1.5.2/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-28 02:31:59.000000 graphreduce-1.5.2/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-28 02:31:59.540481 graphreduce-1.5.2/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-07-28 02:31:43.000000 graphreduce-1.5.2/setup.py
```

### Comparing `graphreduce-1.5.1/PKG-INFO` & `graphreduce-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.1
+Version: 1.5.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.1/README.md` & `graphreduce-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.1/graphreduce/context.py` & `graphreduce-1.5.2/graphreduce/context.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.1/graphreduce/graph_reduce.py` & `graphreduce-1.5.2/graphreduce/graph_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,16 +368,16 @@
         self.hydrate_graph_data()
 
         logger.info("checking for prefix uniqueness")
         self.prefix_uniqueness()
     
         for node in self.nodes():
             logger.info(f"running filters, clip cols, and annotations for {node.__class__.__name__}")
-            node.do_filters()
-            node.do_clip_cols()
+            node.do_filter()
+            node.do_transpose()
             node.do_annotate()
 
         logger.info(f"depth-first traversal through the graph from source: {self.parent_node.__class__.__name__}")
         for edge in self.depth_first_generator():
             parent_node = edge[0]
             relation_node = edge[1]
             edge_data = self.get_edge_data(parent_node, relation_node)
@@ -436,8 +436,9 @@
                         relation_node,
                         relation_df=label_df
                     )
                     parent_node.df = joined_with_labels
 
             # post-join annotations (if any)
             parent_node.do_post_join_annotate()
-
+            # post-join filters (if any)
+            parent_node.do_post_join_filter()
```

### Comparing `graphreduce-1.5.1/graphreduce/node.py` & `graphreduce-1.5.2/graphreduce/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,45 +145,53 @@
             pass
 
         elif self.compute_layer.value == 'redshift':
             pass
 
 
     @abc.abstractmethod
-    def do_filters (
+    def do_filter (
         self
     ):
         """
 do some filters on the data
         """
         pass
     
 
     @abc.abstractmethod
     def do_annotate(self):
         """
 Implement custom annotation functionality
 for annotating this particular data
         """
-        return
+        pass
 
     
     @abc.abstractmethod
     def do_post_join_annotate(self):
         """
 Implement custom annotation functionality
 for annotating data after joining with 
 child data
         """
         pass
 
-     
+
     @abc.abstractmethod
     def do_clip_cols(self):
-        return
+        pass
+
+
+    def do_post_join_filter(self):
+        """
+Filter operations that require some
+additional relational data to perform.
+        """
+        pass
 
 
     def dynamic_propagation (
             self,
             reduce_key : str,
             type_func_map : dict = {},
             compute_layer : ComputeLayerEnum = ComputeLayerEnum.pandas,
@@ -413,24 +421,27 @@
             ):
         """
 Constructor
         """
         super().__init__(*args, **kwargs)
 
 
-    def do_filters(self):
+    def do_filter(self):
         pass
 
     def do_annotate(self):
         pass
 
     def do_post_join_annotate(self):
         pass
 
     def do_clip_cols(self):
         pass
 
+    def do_post_join_filter(self):
+        pass
+
     def do_reduce(self):
         pass
 
     def do_labels(self):
         pass
```

### Comparing `graphreduce-1.5.1/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.5.2/graphreduce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.1
+Version: 1.5.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.1/setup.py` & `graphreduce-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = "1.5.1",
+        version = "1.5.2",
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
-            "dask==2023.6.0",
+            "dask",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
             "pyspark>=3.4.0",
             "pyvis>=0.3.1",
             "setuptools>=65.5.1",
             "structlog>=23.1.0"
             ],
```

