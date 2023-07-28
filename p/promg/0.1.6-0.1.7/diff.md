# Comparing `tmp/promg-0.1.6.tar.gz` & `tmp/promg-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promg-0.1.6.tar", last modified: Thu Jul 27 11:39:08 2023, max compression
+gzip compressed data, was "promg-0.1.7.tar", last modified: Fri Jul 28 14:47:20 2023, max compression
```

## Comparing `promg-0.1.6.tar` & `promg-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.763670 promg-0.1.6/
--rw-rw-rw-   0        0        0     7817 2023-04-24 11:35:40.000000 promg-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     5806 2023-07-27 11:39:08.762644 promg-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5558 2023-07-25 13:07:47.000000 promg-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 11:39:08.763670 promg-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-07-27 11:31:54.000000 promg-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.622630 promg-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.636717 promg-0.1.6/src/promg/
--rw-rw-rw-   0        0        0      516 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.690322 promg-0.1.6/src/promg/cypher_queries/
--rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/__init__.py
--rw-rw-rw-   0        0        0     4275 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/analysis_ql.py
--rw-rw-rw-   0        0        0     8514 2023-07-26 12:17:37.000000 promg-0.1.6/src/promg/cypher_queries/data_importer_ql.py
--rw-rw-rw-   0        0        0     5207 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/db_managment_ql.py
--rw-rw-rw-   0        0        0     5867 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/inference_engine_ql.py
--rw-rw-rw-   0        0        0    21132 2023-07-27 09:29:36.000000 promg-0.1.6/src/promg/cypher_queries/semantic_header_ql.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.707503 promg-0.1.6/src/promg/data_managers/
--rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/data_managers/__init__.py
--rw-rw-rw-   0        0        0    22701 2023-07-26 12:08:52.000000 promg-0.1.6/src/promg/data_managers/datastructures.py
--rw-rw-rw-   0        0        0    37835 2023-07-27 09:48:28.000000 promg-0.1.6/src/promg/data_managers/semantic_header.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.722050 promg-0.1.6/src/promg/database_managers/
--rw-rw-rw-   0        0        0    16050 2023-07-26 12:18:33.000000 promg-0.1.6/src/promg/database_managers/EventKnowledgeGraph.py
--rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/__init__.py
--rw-rw-rw-   0        0        0      588 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/authentication.py
--rw-rw-rw-   0        0        0     3157 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/db_connection.py
--rw-rw-rw-   0        0        0      235 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/remote_authentication.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.750120 promg-0.1.6/src/promg/ekg_modules/
--rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/__init__.py
--rw-rw-rw-   0        0        0     6923 2023-07-26 12:20:16.000000 promg-0.1.6/src/promg/ekg_modules/data_importer.py
--rw-rw-rw-   0        0        0     3867 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/db_management.py
--rw-rw-rw-   0        0        0      755 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/ekg_analysis.py
--rw-rw-rw-   0        0        0     8562 2023-07-26 13:30:57.000000 promg-0.1.6/src/promg/ekg_modules/ekg_builder_semantic_header.py
--rw-rw-rw-   0        0        0     1644 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/inference_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.760626 promg-0.1.6/src/promg/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/auxiliary_functions.py
--rw-rw-rw-   0        0        0     1072 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/context_manager_tqdm.py
--rw-rw-rw-   0        0        0     1876 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/get_db_size.py
--rw-rw-rw-   0        0        0     2134 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/performance_handling.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.650242 promg-0.1.6/src/promg.egg-info/
--rw-rw-rw-   0        0        0     5806 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1272 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.921752 promg-0.1.7/
+-rw-rw-rw-   0        0        0     7817 2023-04-24 11:35:40.000000 promg-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     5806 2023-07-28 14:47:20.920757 promg-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5558 2023-07-25 13:07:47.000000 promg-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 14:47:20.921752 promg-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-07-28 14:32:01.000000 promg-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.719460 promg-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.730792 promg-0.1.7/src/promg/
+-rw-rw-rw-   0        0        0      516 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.802863 promg-0.1.7/src/promg/cypher_queries/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/cypher_queries/__init__.py
+-rw-rw-rw-   0        0        0     3955 2023-07-28 14:31:35.000000 promg-0.1.7/src/promg/cypher_queries/analysis_ql.py
+-rw-rw-rw-   0        0        0     8514 2023-07-26 12:17:37.000000 promg-0.1.7/src/promg/cypher_queries/data_importer_ql.py
+-rw-rw-rw-   0        0        0     5207 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/cypher_queries/db_managment_ql.py
+-rw-rw-rw-   0        0        0     5867 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/cypher_queries/inference_engine_ql.py
+-rw-rw-rw-   0        0        0    21725 2023-07-28 14:31:35.000000 promg-0.1.7/src/promg/cypher_queries/semantic_header_ql.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.819942 promg-0.1.7/src/promg/data_managers/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/data_managers/__init__.py
+-rw-rw-rw-   0        0        0    22701 2023-07-26 12:08:52.000000 promg-0.1.7/src/promg/data_managers/datastructures.py
+-rw-rw-rw-   0        0        0    37875 2023-07-28 14:31:35.000000 promg-0.1.7/src/promg/data_managers/semantic_header.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.850353 promg-0.1.7/src/promg/database_managers/
+-rw-rw-rw-   0        0        0    15996 2023-07-28 14:31:35.000000 promg-0.1.7/src/promg/database_managers/EventKnowledgeGraph.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/database_managers/__init__.py
+-rw-rw-rw-   0        0        0      588 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/database_managers/authentication.py
+-rw-rw-rw-   0        0        0     3157 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/database_managers/db_connection.py
+-rw-rw-rw-   0        0        0      235 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/database_managers/remote_authentication.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.890713 promg-0.1.7/src/promg/ekg_modules/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/ekg_modules/__init__.py
+-rw-rw-rw-   0        0        0     6923 2023-07-26 12:20:16.000000 promg-0.1.7/src/promg/ekg_modules/data_importer.py
+-rw-rw-rw-   0        0        0     3867 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/ekg_modules/db_management.py
+-rw-rw-rw-   0        0        0      714 2023-07-28 14:31:35.000000 promg-0.1.7/src/promg/ekg_modules/ekg_analysis.py
+-rw-rw-rw-   0        0        0     8562 2023-07-26 13:30:57.000000 promg-0.1.7/src/promg/ekg_modules/ekg_builder_semantic_header.py
+-rw-rw-rw-   0        0        0     1644 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/ekg_modules/inference_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.918235 promg-0.1.7/src/promg/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/utilities/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     1072 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/utilities/context_manager_tqdm.py
+-rw-rw-rw-   0        0        0     1876 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/utilities/get_db_size.py
+-rw-rw-rw-   0        0        0     2134 2023-07-25 13:07:47.000000 promg-0.1.7/src/promg/utilities/performance_handling.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:47:20.756291 promg-0.1.7/src/promg.egg-info/
+-rw-rw-rw-   0        0        0     5806 2023-07-28 14:47:20.000000 promg-0.1.7/src/promg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2023-07-28 14:47:20.000000 promg-0.1.7/src/promg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:47:20.000000 promg-0.1.7/src/promg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-28 14:47:20.000000 promg-0.1.7/src/promg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 14:47:20.000000 promg-0.1.7/src/promg.egg-info/top_level.txt
```

### Comparing `promg-0.1.6/LICENSE` & `promg-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/PKG-INFO` & `promg-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promg-0.1.6/README.md` & `promg-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/setup.py` & `promg-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='promg',
-    version='0.1.6',
+    version='0.1.7',
     description='Pyhton library to build Event Knowledge Graphs',
     author='A. Swevels, D.Fahland',
     python_requires='>=3.7',
     install_requires=['neo4j', 'numpy', 'pandas', 'tabulate', 'tqdm'],
     license='GPL 3.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `promg-0.1.6/src/promg/__init__.py` & `promg-0.1.7/src/promg/__init__.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/cypher_queries/analysis_ql.py` & `promg-0.1.7/src/promg/cypher_queries/analysis_ql.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             return f'DF_C_{entity_type.upper()}'
         else:
             return f'DF_C'
 
     @staticmethod
     def get_aggregate_df_relations_query(entity: ConstructedNodes,
                                          include_label_in_c_df: bool = True,
-                                         classifiers: Optional[List[str]] = None, df_threshold: int = 0,
+                                         df_threshold: int = 0,
                                          relative_df_threshold: float = 0,
                                          exclude_self_loops=True) -> Query:
 
         # add relations between classes when desired
         if df_threshold == 0 and relative_df_threshold == 0:
             # corresponds to aggregate_df_relations &  aggregate_df_relations_for_entities in graphdb-event-logs
             # aggregate only for a specific entity type and event classifier
@@ -58,22 +58,17 @@
                                 WHERE (df_freq*$relative_df_threshold > df_freq2)
                                 MERGE 
                                 (c1) 
                                     -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_C'}]-> 
                                 (c2) 
                                 ON CREATE SET rel2.count=df_freq'''
 
-        classifier_condition = ""
-        if classifiers is not None:
-            classifier_string = "_".join(classifiers)
-            classifier_condition = f"AND c1.classType = '{classifier_string}'"
 
         return Query(query_str=query_str,
                      template_string_parameters={
                          "df_label": entity.get_df_label(),
                          "entity_type": entity.node_type,
-                         "classifier_condition": classifier_condition,
                          "classifier_self_loops": "WHERE c1 <> c2" if exclude_self_loops else "",
                          "dfc_label": AnalysisQueryLibrary.get_dfc_label(entity.node_type, include_label_in_c_df),
                          "df_threshold": df_threshold,
                          "relative_df_threshold": relative_df_threshold
                      })
```

### Comparing `promg-0.1.6/src/promg/cypher_queries/data_importer_ql.py` & `promg-0.1.7/src/promg/cypher_queries/data_importer_ql.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/cypher_queries/db_managment_ql.py` & `promg-0.1.7/src/promg/cypher_queries/db_managment_ql.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/cypher_queries/inference_engine_ql.py` & `promg-0.1.7/src/promg/cypher_queries/inference_engine_ql.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/cypher_queries/semantic_header_ql.py` & `promg-0.1.7/src/promg/cypher_queries/semantic_header_ql.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,31 +190,46 @@
                          "rel_type": node_constructor.relation.get_relation_type(),
                          "result_labels": node_constructor.result.get_label_str(as_list=True)
                      },
                      parameters={"limit": batch_size})
 
     @staticmethod
     def get_create_relation_by_relations_query(relation_constructor: RelationConstructor, batch_size: int) -> Query:
+        if relation_constructor.model_as_node:
+            # language=sql
+            merge_str = '''
+                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> (
+                            $to_node_name)
+                            '''
+        else:
+            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
+
         # language=SQL
         query_str = '''
                 CALL apoc.periodic.iterate(
                 '$relation_queries                        
                 RETURN distinct $from_node_name, $to_node_name',
-                'MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)',                        
+                '$merge_str',                        
                 {batchSize: $batch_size})
             '''
 
+        query_str = Template(query_str).safe_substitute({
+            "merge_str": merge_str
+        })
+
         return Query(query_str=query_str,
                      template_string_parameters={
                          "relation_queries": relation_constructor.get_relations_query(),
                          "from_node_name": relation_constructor.from_node.get_name(),
                          "to_node_name": relation_constructor.to_node.get_name(),
                          "rel_pattern": relation_constructor.result.get_pattern(),
-                         "batch_size": batch_size
-                     })
+                         "relation_label_str": relation_constructor.result.get_relation_types_str()
+                     },
+                     parameters={
+                         "batch_size": batch_size})
 
     @staticmethod
     def get_create_relation_using_record_query(relation_constructor: RelationConstructor, batch_size: int) -> Query:
         # find events that are related to different entities of which one event also has a reference to the other entity
         # create a relation between these two entities
         add_str = ""
         if relation_constructor.model_as_node:
```

### Comparing `promg-0.1.6/src/promg/data_managers/datastructures.py` & `promg-0.1.7/src/promg/data_managers/datastructures.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/data_managers/semantic_header.py` & `promg-0.1.7/src/promg/data_managers/semantic_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def get_pattern(self, is_set=False, node_name=None):
         if not is_set:
             return f"{self.attribute}: {self.value}"
         else:
             if node_name is None:
                 return f"{self.attribute} = {self.value}"
             else:
-                return f"{node_name}.{self.attribute} = {self.value}"
+                return f"{node_name}.{self.attribute} = COALESCE({node_name}.{self.attribute}, {self.value})"
 
     def __repr__(self):
         return self.get_pattern()
 
 
 @dataclass()
 class Node:
```

### Comparing `promg-0.1.6/src/promg/database_managers/EventKnowledgeGraph.py` & `promg-0.1.7/src/promg/database_managers/EventKnowledgeGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
         relative_position = self.semantic_header.get_entity(relative_position_type)
         if entity_type is None:
             raise ValueError(f"{entity_type} is not defined in semantic header")
         self.inference_engine.infer_items_propagate_downwards_multiple_level_w_batching(entity, relative_position)
 
     # endregion
 
-    def create_df_process_model(self, entity_type: str, classifiers: Optional[List[str]] = None):
+    def create_df_process_model(self, entity_type: str):
         """
         Pass on method to ekg_analysis to create a DF process model
 
         :param entity_type: The type of the entity
         :type entity_type: str
         :param classifiers: the attributes used as classifiers
         :type classifiers: Optional[List[str]], defaults to None
@@ -350,15 +350,15 @@
         :return: None
 
         :raise ValueError: when the entity has not been defined
         """
         entity = self.semantic_header.get_entity(entity_type)
         if entity_type is None:
             raise ValueError(f"{entity_type} is not defined in semantic header")
-        self.ekg_analysis.create_df_process_model(entity, classifiers)
+        self.ekg_analysis.create_df_process_model(entity)
 
     def do_custom_query(self, query_name: str, **kwargs: Optional[Dict[str, any]]) -> any:
         r"""
         Pass on the custom query to the custom module with optional key words arguments
 
         :param query_name: the name of the function that contains the query
         :type query_name: str
```

### Comparing `promg-0.1.6/src/promg/database_managers/authentication.py` & `promg-0.1.7/src/promg/database_managers/authentication.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/database_managers/db_connection.py` & `promg-0.1.7/src/promg/database_managers/db_connection.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/ekg_modules/data_importer.py` & `promg-0.1.7/src/promg/ekg_modules/data_importer.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/ekg_modules/db_management.py` & `promg-0.1.7/src/promg/ekg_modules/db_management.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/ekg_modules/ekg_analysis.py` & `promg-0.1.7/src/promg/ekg_modules/ekg_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,10 @@
         self.connection = db_connection
         self.perf = perf
 
     def _write_message_to_performance(self, message: str):
         if self.perf is not None:
             self.perf.finished_step(activity=message)
 
-    def create_df_process_model(self, entity, classifiers):
+    def create_df_process_model(self, entity):
         self.connection.exec_query(analysis_ql.get_aggregate_df_relations_query,
-                                   **{"entity": entity, "classifiers": classifiers})
+                                   **{"entity": entity})
```

### Comparing `promg-0.1.6/src/promg/ekg_modules/ekg_builder_semantic_header.py` & `promg-0.1.7/src/promg/ekg_modules/ekg_builder_semantic_header.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/ekg_modules/inference_engine.py` & `promg-0.1.7/src/promg/ekg_modules/inference_engine.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/utilities/auxiliary_functions.py` & `promg-0.1.7/src/promg/utilities/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/utilities/context_manager_tqdm.py` & `promg-0.1.7/src/promg/utilities/context_manager_tqdm.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/utilities/get_db_size.py` & `promg-0.1.7/src/promg/utilities/get_db_size.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg/utilities/performance_handling.py` & `promg-0.1.7/src/promg/utilities/performance_handling.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.6/src/promg.egg-info/PKG-INFO` & `promg-0.1.7/src/promg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promg-0.1.6/src/promg.egg-info/SOURCES.txt` & `promg-0.1.7/src/promg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

