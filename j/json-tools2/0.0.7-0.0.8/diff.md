# Comparing `tmp/json-tools2-0.0.7.tar.gz` & `tmp/json-tools2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-tools2-0.0.7.tar", last modified: Fri Jul 28 09:36:51 2023, max compression
+gzip compressed data, was "json-tools2-0.0.8.tar", last modified: Fri Jul 28 10:53:52 2023, max compression
```

## Comparing `json-tools2-0.0.7.tar` & `json-tools2-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.598134 json-tools2-0.0.7/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1067 2021-10-05 22:07:19.000000 json-tools2-0.0.7/LICENSE
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.7/MANIFEST.in
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3003 2023-07-28 09:36:51.598134 json-tools2-0.0.7/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2634 2023-07-28 09:29:32.000000 json-tools2-0.0.7/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-28 09:36:51.598134 json-tools2-0.0.7/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2023-07-28 09:29:41.000000 json-tools2-0.0.7/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.594134 json-tools2-0.0.7/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.594134 json-tools2-0.0.7/src/json_tools2/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       93 2023-07-28 07:36:36.000000 json-tools2-0.0.7/src/json_tools2/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.7/src/json_tools2/flat_json.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     8295 2023-07-28 08:53:42.000000 json-tools2-0.0.7/src/json_tools2/schema.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 22:26:53.000000 json-tools2-0.0.7/src/json_tools2/spark.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.7/src/json_tools2/util.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 09:36:51.598134 json-tools2-0.0.7/src/json_tools2.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3003 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      364 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2023-07-28 09:36:51.000000 json-tools2-0.0.7/src/json_tools2.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.099943 json-tools2-0.0.8/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1067 2021-10-05 22:07:19.000000 json-tools2-0.0.8/LICENSE
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       18 2021-10-05 22:07:19.000000 json-tools2-0.0.8/MANIFEST.in
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4044 2023-07-28 10:53:52.095943 json-tools2-0.0.8/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3675 2023-07-28 10:19:42.000000 json-tools2-0.0.8/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-28 10:53:52.099943 json-tools2-0.0.8/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      987 2023-07-28 10:13:24.000000 json-tools2-0.0.8/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/json_tools2/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      118 2023-07-28 09:44:32.000000 json-tools2-0.0.8/src/json_tools2/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    13180 2021-10-05 22:07:19.000000 json-tools2-0.0.8/src/json_tools2/flat_json.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     9370 2023-07-28 10:52:13.000000 json-tools2-0.0.8/src/json_tools2/schema.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1045 2021-11-02 22:26:53.000000 json-tools2-0.0.8/src/json_tools2/spark.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      637 2021-10-05 22:07:19.000000 json-tools2-0.0.8/src/json_tools2/util.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-28 10:53:52.095943 json-tools2-0.0.8/src/json_tools2.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4044 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      364 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       11 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       12 2023-07-28 10:53:52.000000 json-tools2-0.0.8/src/json_tools2.egg-info/top_level.txt
```

### Comparing `json-tools2-0.0.7/LICENSE` & `json-tools2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.7/PKG-INFO` & `json-tools2-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: json-tools2
-Version: 0.0.7
-Summary: JSON Tools Library
-Home-page: https://github.com/stonezhong/json_tools2
-Author: Stone Zhong
-Author-email: stonezhong@hotmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Index
+* [Infer Schema](#infer-schema)
+* [Schema evolvement](#schema-evolvement)
 
-# JSON related tools
-
-## Infer Schema
+# Infer Schema
 
 With function `infer_schema`, you can get schema from json object. The output complys to [JSON Schema Specification](https://json-schema.org/specification.html). Here is an example:
 
 ```python
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
@@ -95,7 +84,54 @@
     schema = infer_schema(payload)
     validate(instance=payload, schema=schema) # it should not throw exception
 
 if __name__ == '__main__':
     main()
 
 ```
+
+# Schema evolvement
+
+Think about such case:
+* You have json object stream
+* You can to merge schema for each object from the stream
+* You want to save the merged schema, so in case you need, to can load schema saved and continue to merge more objects from the stream.
+
+Here is an example:
+```python
+#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
+
+from json_tools2 import get_schema, ValueSchema
+import json
+
+def main():
+    schema = get_schema(1)
+    print(json.dumps(schema.to_json(), indent=4))
+    saved_schema = schema.dump_json()
+    # You got a json object saved_schema which you can save the inferred schema
+
+    # load schema
+    schema = ValueSchema.load_json(saved_schema)
+    schema.merge_from(get_schema(None))
+    print(json.dumps(schema.to_json(), indent=4))
+
+
+if __name__ == '__main__':
+    main()
+```
+Output
+```
+{
+    "type": "integer"
+}
+{
+    "anyOf": [
+        {
+            "type": "integer"
+        },
+        {
+            "type": "null"
+        }
+    ]
+}
+```
```

### Comparing `json-tools2-0.0.7/README.md` & `json-tools2-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-# JSON related tools
+Metadata-Version: 2.1
+Name: json-tools2
+Version: 0.0.8
+Summary: JSON Tools Library
+Home-page: https://github.com/stonezhong/json_tools2
+Author: Stone Zhong
+Author-email: stonezhong@hotmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Index
+* [Infer Schema](#infer-schema)
+* [Schema evolvement](#schema-evolvement)
 
-## Infer Schema
+# Infer Schema
 
 With function `infer_schema`, you can get schema from json object. The output complys to [JSON Schema Specification](https://json-schema.org/specification.html). Here is an example:
 
 ```python
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
@@ -81,8 +96,55 @@
     payload = {"foo": 1}
     schema = infer_schema(payload)
     validate(instance=payload, schema=schema) # it should not throw exception
 
 if __name__ == '__main__':
     main()
 
-```
+```
+
+# Schema evolvement
+
+Think about such case:
+* You have json object stream
+* You can to merge schema for each object from the stream
+* You want to save the merged schema, so in case you need, to can load schema saved and continue to merge more objects from the stream.
+
+Here is an example:
+```python
+#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
+
+from json_tools2 import get_schema, ValueSchema
+import json
+
+def main():
+    schema = get_schema(1)
+    print(json.dumps(schema.to_json(), indent=4))
+    saved_schema = schema.dump_json()
+    # You got a json object saved_schema which you can save the inferred schema
+
+    # load schema
+    schema = ValueSchema.load_json(saved_schema)
+    schema.merge_from(get_schema(None))
+    print(json.dumps(schema.to_json(), indent=4))
+
+
+if __name__ == '__main__':
+    main()
+```
+Output
+```
+{
+    "type": "integer"
+}
+{
+    "anyOf": [
+        {
+            "type": "integer"
+        },
+        {
+            "type": "null"
+        }
+    ]
+}
+```
```

### Comparing `json-tools2-0.0.7/setup.py` & `json-tools2-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="json-tools2",
-    version="0.0.7",
+    version="0.0.8",
     description="JSON Tools Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/json_tools2",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `json-tools2-0.0.7/src/json_tools2/flat_json.py` & `json-tools2-0.0.8/src/json_tools2/flat_json.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.7/src/json_tools2/schema.py` & `json-tools2-0.0.8/src/json_tools2/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,25 +27,25 @@
         if type(value) == list:
             return cls.ARRAY
         if type(value) == dict:
             return cls.OBJECT
         
         raise SchemaError(f"{type(value)} is not a valid JSON value")
     
-class _ValueSchema:
+class ValueSchema:
     value_type      : _ValueType
-    item_type       :  Optional["_ValueSchema"]
-    property_types  : Optional[Dict[str, "_ValueSchema"]]
+    item_type       :  Optional["ValueSchema"]
+    property_types  : Optional[Dict[str, "ValueSchema"]]
     null_merged     : bool
 
     def __init__(
         self, 
         value_type:_ValueType, 
-        item_type:Optional["_ValueSchema"]=None,
-        property_types:Optional[Dict[str, "_ValueSchema"]]=None
+        item_type:Optional["ValueSchema"]=None,
+        property_types:Optional[Dict[str, "ValueSchema"]]=None
     ):
         self.value_type     = value_type
         self.item_type      = item_type
         self.property_types = property_types
 
         # have we merged null?
         self.null_merged    = self.value_type == _ValueType.NULL
@@ -59,24 +59,51 @@
         return {
             "anyOf": [
                 self.to_json_raw(),
                 {"type": "null"}
             ]
         }
 
-    def clone(self) -> "_ValueSchema":
+    def clone(self) -> "ValueSchema":
         new_item_type = None if self.item_type is None else self.item_type.clone()
         if self.property_types is None:
             new_property_types = None
         else:
             new_property_types = {
                 property_name:property_type.clone() for property_name, property_type \
                     in self.property_types.items()
             }
-        return _ValueSchema(self.value_type, item_type=new_item_type, property_types=new_property_types)
+        return ValueSchema(self.value_type, item_type=new_item_type, property_types=new_property_types)
+
+    def dump_json(self):
+        return {
+            "value_type": self.value_type.value,
+            "item_type": None if self.item_type is None else self.item_type.dumps(),
+            "property_types": None if self.property_types is None else \
+                {
+                    property_name: property_type.dumps() for property_name, property_type in self.property_types
+                },
+            "null_merged": self.null_merged
+        }
+
+    @classmethod
+    def load_json(cls, payload):
+        value_type = _ValueType(payload["value_type"])
+        item_type = None if payload["item_type"] is None else cls.load_json(payload["item_type"])
+        if payload["property_types"] is None:
+            property_types = None
+        else:
+            property_types = {
+                property_name: cls.load_json(property_type) \
+                    for property_name, property_type in payload["property_types"].items()
+            }
+        ret = cls(value_type, item_type=item_type, property_types=property_types)
+        ret.null_merged = payload["null_merged"]
+        return ret
+        
 
     def to_json_raw(self) -> Any:
         if self.value_type == _ValueType.NULL:
             return {"type":"null"}
         if self.value_type == _ValueType.STRING:
             return {"type":"string"}
         if self.value_type == _ValueType.NUMBER:
@@ -99,15 +126,15 @@
                 "type": "array", 
                 "items": {"type": "null" } if self.item_type is None \
                     else self.item_type.to_json()
             }
 
         assert False  # impossible
     
-    def merge_from(self, schema:"_ValueSchema") -> None:
+    def merge_from(self, schema:"ValueSchema") -> None:
         if self.value_type == _ValueType.NULL:
             # ok, switch to the new schema, null_merged should be set already            
             self.value_type = schema.value_type
             if schema.value_type == _ValueType.OBJECT:
                 self.property_types = {
                     property_name: property_type.clone() for property_name, property_type \
                         in schema.property_types.items()
@@ -182,40 +209,40 @@
                     self.item_type.merge_from(schema.item_type)
                 return
             raise SchemaError(f"Cannot merge {schema.value_type.name} to ARRAY")
         
         assert False # impossible
 
 
-def infer_schema(value:Any) -> _ValueSchema:
-    return _infer_schema(value).to_json()
+def infer_schema(value:Any) -> Any:
+    return get_schema(value).to_json()
 
 
-def _infer_schema(value:Any) -> _ValueSchema:
+def get_schema(value:Any) -> ValueSchema:
     value_type = _ValueType.from_value(value)
 
     if value_type == _ValueType.OBJECT:
-        obj_schema = _ValueSchema(value_type=value_type, property_types={})
+        obj_schema = ValueSchema(value_type=value_type, property_types={})
         for property_name, property_value in value.items():
-            property_schema = _infer_schema(property_value)
+            property_schema = get_schema(property_value)
             if property_name in obj_schema.property_types:
                 obj_schema.property_types[property_name].merge_from(property_schema)
             else:
                 obj_schema.property_types[property_name] = property_schema
         return obj_schema
 
     if value_type == _ValueType.ARRAY:
-        array_schema = _ValueSchema(value_type=value_type, item_type=None)
+        array_schema = ValueSchema(value_type=value_type, item_type=None)
         for item in value:
-            item_schema = _infer_schema(item)
+            item_schema = get_schema(item)
             if array_schema.item_type is None:
                 array_schema.item_type = item_schema
             else:
                 array_schema.item_type.merge_from(item_schema)
         return array_schema
 
     # it must be primitive type
-    return _ValueSchema(value_type=value_type)  
+    return ValueSchema(value_type=value_type)  
 
 
 class SchemaError(Exception):
     pass
```

### Comparing `json-tools2-0.0.7/src/json_tools2/spark.py` & `json-tools2-0.0.8/src/json_tools2/spark.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.7/src/json_tools2/util.py` & `json-tools2-0.0.8/src/json_tools2/util.py`

 * *Files identical despite different names*

### Comparing `json-tools2-0.0.7/src/json_tools2.egg-info/PKG-INFO` & `json-tools2-0.0.8/src/json_tools2.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: json-tools2
-Version: 0.0.7
+Version: 0.0.8
 Summary: JSON Tools Library
 Home-page: https://github.com/stonezhong/json_tools2
 Author: Stone Zhong
 Author-email: stonezhong@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSON related tools
+# Index
+* [Infer Schema](#infer-schema)
+* [Schema evolvement](#schema-evolvement)
 
-## Infer Schema
+# Infer Schema
 
 With function `infer_schema`, you can get schema from json object. The output complys to [JSON Schema Specification](https://json-schema.org/specification.html). Here is an example:
 
 ```python
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 
@@ -95,7 +97,54 @@
     schema = infer_schema(payload)
     validate(instance=payload, schema=schema) # it should not throw exception
 
 if __name__ == '__main__':
     main()
 
 ```
+
+# Schema evolvement
+
+Think about such case:
+* You have json object stream
+* You can to merge schema for each object from the stream
+* You want to save the merged schema, so in case you need, to can load schema saved and continue to merge more objects from the stream.
+
+Here is an example:
+```python
+#!/usr/bin/env python
+# -*- coding: UTF-8 -*-
+
+from json_tools2 import get_schema, ValueSchema
+import json
+
+def main():
+    schema = get_schema(1)
+    print(json.dumps(schema.to_json(), indent=4))
+    saved_schema = schema.dump_json()
+    # You got a json object saved_schema which you can save the inferred schema
+
+    # load schema
+    schema = ValueSchema.load_json(saved_schema)
+    schema.merge_from(get_schema(None))
+    print(json.dumps(schema.to_json(), indent=4))
+
+
+if __name__ == '__main__':
+    main()
+```
+Output
+```
+{
+    "type": "integer"
+}
+{
+    "anyOf": [
+        {
+            "type": "integer"
+        },
+        {
+            "type": "null"
+        }
+    ]
+}
+```
```

