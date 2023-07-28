# Comparing `tmp/oarepo-model-builder-polymorphic-1.0.0.tar.gz` & `tmp/oarepo-model-builder-polymorphic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-polymorphic-1.0.0.tar", last modified: Mon May 22 10:36:30 2023, max compression
+gzip compressed data, was "oarepo-model-builder-polymorphic-1.0.1.tar", last modified: Fri Jul 28 10:48:06 2023, max compression
```

## Comparing `oarepo-model-builder-polymorphic-1.0.0.tar` & `oarepo-model-builder-polymorphic-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:36:30.936235 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/datatypes/polymorphic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 10:36:30.000000 oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:36:30.940235 oarepo-model-builder-polymorphic-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-22 10:33:35.000000 oarepo-model-builder-polymorphic-1.0.0/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:48:06.586447 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/datatypes/polymorphic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 10:48:06.000000 oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:48:06.590447 oarepo-model-builder-polymorphic-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-28 10:45:03.000000 oarepo-model-builder-polymorphic-1.0.1/tests/test_service.py
```

### Comparing `oarepo-model-builder-polymorphic-1.0.0/PKG-INFO` & `oarepo-model-builder-polymorphic-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-polymorphic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model builder plugin for oarepo-polymorphic
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-polymorphic-1.0.0/README.md` & `oarepo-model-builder-polymorphic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic/datatypes/polymorphic.py` & `oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic/datatypes/polymorphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import marshmallow as ma
 from oarepo_model_builder.datatypes import (DataTypeComponent, ModelDataType,
                                             ObjectDataType, Section, datatypes)
 from oarepo_model_builder.datatypes.components import (
     MarshmallowModelComponent, UIMarshmallowModelComponent)
-from oarepo_model_builder.datatypes.containers.object import ObjectPropertiesField
+from oarepo_model_builder.datatypes.containers.object import \
+    ObjectPropertiesField
 
 
 class PolymorphicDataType(ObjectDataType):
     model_type = "polymorphic"
 
     class ModelSchema(ObjectDataType.ModelSchema):
         schemas = ObjectPropertiesField()
@@ -20,14 +21,15 @@
 
         # marshmallow uses one-of, others use union - so create the union here
         # but keep the polymorphic children somewhere
         for schema_key, schema in self.definition["schemas"].items():
             dt = datatypes.get_datatype(
                 self, schema, schema_key, self.model, self.schema
             )
+            dt.skip_in_path = True
             dt.prepare(context)
             self.polymorphic_children[schema_key] = dt
             self.children.update(dt.children)
 
     def deep_iter(self):
         # skip direct children in deepiter and go to polymorphic instead
         yield from super(ObjectDataType, self).deep_iter()
```

### Comparing `oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/PKG-INFO` & `oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-polymorphic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model builder plugin for oarepo-polymorphic
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-polymorphic-1.0.0/oarepo_model_builder_polymorphic.egg-info/SOURCES.txt` & `oarepo-model-builder-polymorphic-1.0.1/oarepo_model_builder_polymorphic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-polymorphic-1.0.0/setup.cfg` & `oarepo-model-builder-polymorphic-1.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-polymorphic
-version = 1.0.0
+version = 1.0.1
 description = Model builder plugin for oarepo-polymorphic
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-polymorphic-1.0.0/tests/test_service.py` & `oarepo-model-builder-polymorphic-1.0.1/tests/test_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from invenio_access.permissions import system_identity
 from mock_record.proxies import current_service
 from mock_record.records.api import MockRecordRecord
 
 
-def test_service(app, db, search_clear):
+def test_service(app, db, search_clear, lang_data):
     created_record_a = current_service.create(
-        system_identity, {"metadata": {"a": {"disc": "1", "a": "a field"}}}
+        system_identity,
+        {"metadata": {"a": {"disc": "1", "a": "a field", "c": {"id": "en"}}}},
     )
     created_record_reread_a = current_service.read(
         system_identity, created_record_a["id"]
     )
     assert created_record_a.data["metadata"] == created_record_reread_a.data["metadata"]
+    assert "c" in created_record_a.data["metadata"]["a"]
+    assert created_record_a.data["metadata"]["a"]["c"]["title"] == {"en": "English"}
 
     created_record_b = current_service.create(
         system_identity, {"metadata": {"a": {"disc": "2", "b": "b field"}}}
     )
 
     MockRecordRecord.index.refresh()
```

