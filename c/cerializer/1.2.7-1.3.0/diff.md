# Comparing `tmp/cerializer-1.2.7.tar.gz` & `tmp/cerializer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerializer-1.2.7.tar", last modified: Tue Feb  7 12:05:01 2023, max compression
+gzip compressed data, was "cerializer-1.3.0.tar", max compression
```

## Comparing `cerializer-1.2.7.tar` & `cerializer-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,75 @@
-drwxrwxr-x   0 development  (1001) development  (1001)        0 2023-02-07 12:05:01.837080 cerializer-1.2.7/
--rw-rw-r--   0 development  (1001) development  (1001)       19 2022-11-08 08:30:27.000000 cerializer-1.2.7/MANIFEST.in
--rw-rw-r--   0 development  (1001) development  (1001)      195 2023-02-07 12:05:01.837080 cerializer-1.2.7/PKG-INFO
--rw-rw-r--   0 development  (1001) development  (1001)     6590 2022-11-08 08:30:27.000000 cerializer-1.2.7/README.md
-drwxrwxr-x   0 development  (1001) development  (1001)        0 2023-02-07 12:05:01.837080 cerializer-1.2.7/cerializer/
--rw-rw-r--   0 development  (1001) development  (1001)        0 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/__init__.py
--rw-rw-r--   0 development  (1001) development  (1001)     1954 2023-02-07 12:00:39.000000 cerializer-1.2.7/cerializer/cerializer_handler.py
--rw-rw-r--   0 development  (1001) development  (1001)     2013 2023-02-07 12:00:39.000000 cerializer-1.2.7/cerializer/compiler.py
--rw-rw-r--   0 development  (1001) development  (1001)      829 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/constants.py
--rw-rw-r--   0 development  (1001) development  (1001)        0 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/py.typed
--rw-rw-r--   0 development  (1001) development  (1001)    22900 2023-02-07 12:00:39.000000 cerializer-1.2.7/cerializer/schema_handler.py
--rw-rw-r--   0 development  (1001) development  (1001)     6228 2023-02-07 12:00:39.000000 cerializer-1.2.7/cerializer/schema_parser.py
-drwxrwxr-x   0 development  (1001) development  (1001)        0 2023-02-07 12:05:01.837080 cerializer-1.2.7/cerializer/templates/
--rw-rw-r--   0 development  (1001) development  (1001)      466 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/array_deserialization.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      255 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/array_serialization.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      469 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/map_deserialization.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      385 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/map_serialization.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      395 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/meta_template.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      303 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/template.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      508 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/union_deserialization.jinja2
--rw-rw-r--   0 development  (1001) development  (1001)      721 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/templates/union_serialization.jinja2
-drwxrwxr-x   0 development  (1001) development  (1001)        0 2023-02-07 12:05:01.837080 cerializer-1.2.7/cerializer/tests/
--rw-rw-r--   0 development  (1001) development  (1001)        0 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/tests/__init__.py
--rw-rw-r--   0 development  (1001) development  (1001)     2458 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/tests/benchmark.py
--rw-rw-r--   0 development  (1001) development  (1001)     3943 2023-02-07 12:00:39.000000 cerializer-1.2.7/cerializer/tests/test_cerializer.py
--rw-rw-r--   0 development  (1001) development  (1001)     3062 2022-11-08 08:30:27.000000 cerializer-1.2.7/cerializer/utils.py
-drwxrwxr-x   0 development  (1001) development  (1001)        0 2023-02-07 12:05:01.837080 cerializer-1.2.7/cerializer.egg-info/
--rw-rw-r--   0 development  (1001) development  (1001)      195 2023-02-07 12:05:01.000000 cerializer-1.2.7/cerializer.egg-info/PKG-INFO
--rw-rw-r--   0 development  (1001) development  (1001)      984 2023-02-07 12:05:01.000000 cerializer-1.2.7/cerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 development  (1001) development  (1001)        1 2023-02-07 12:05:01.000000 cerializer-1.2.7/cerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 development  (1001) development  (1001)      124 2023-02-07 12:05:01.000000 cerializer-1.2.7/cerializer.egg-info/requires.txt
--rw-rw-r--   0 development  (1001) development  (1001)       19 2023-02-07 12:05:01.000000 cerializer-1.2.7/cerializer.egg-info/top_level.txt
--rw-rw-r--   0 development  (1001) development  (1001)   401345 2022-11-08 08:31:08.000000 cerializer-1.2.7/prepare.c
--rw-rw-r--   0 development  (1001) development  (1001)      763 2022-11-08 08:30:27.000000 cerializer-1.2.7/prepare.pxd
--rw-rw-r--   0 development  (1001) development  (1001)     8243 2022-11-08 08:30:27.000000 cerializer-1.2.7/prepare.pyx
--rw-rw-r--   0 development  (1001) development  (1001)     2836 2022-11-08 08:30:27.000000 cerializer-1.2.7/read.pxd
--rw-rw-r--   0 development  (1001) development  (1001)       38 2023-02-07 12:05:01.837080 cerializer-1.2.7/setup.cfg
--rw-rw-r--   0 development  (1001) development  (1001)     1404 2023-02-07 12:00:39.000000 cerializer-1.2.7/setup.py
--rw-rw-r--   0 development  (1001) development  (1001)        5 2023-02-07 12:05:00.000000 cerializer-1.2.7/version.txt
--rw-rw-r--   0 development  (1001) development  (1001)     3146 2022-11-08 08:30:27.000000 cerializer-1.2.7/write.pxd
+-rw-r--r--   0        0        0     6770 2023-07-26 14:31:22.465400 cerializer-1.3.0/README.md
+-rw-r--r--   0        0        0      566 2023-07-27 15:13:19.092555 cerializer-1.3.0/build.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/__init__.py
+-rw-r--r--   0        0        0     1954 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/cerializer_handler.py
+-rw-r--r--   0        0        0     2143 2023-07-20 18:54:01.085491 cerializer-1.3.0/cerializer/compiler.py
+-rw-r--r--   0        0        0      829 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/constants.py
+-rw-r--r--   0        0        0        0 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/py.typed
+-rw-r--r--   0        0        0    22900 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/schema_handler.py
+-rw-r--r--   0        0        0     6228 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/schema_parser.py
+-rw-r--r--   0        0        0      466 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/array_deserialization.jinja2
+-rw-r--r--   0        0        0      255 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/array_serialization.jinja2
+-rw-r--r--   0        0        0      469 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/map_deserialization.jinja2
+-rw-r--r--   0        0        0      385 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/map_serialization.jinja2
+-rw-r--r--   0        0        0      395 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/templates/meta_template.jinja2
+-rw-r--r--   0        0        0      303 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/templates/template.jinja2
+-rw-r--r--   0        0        0      508 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/union_deserialization.jinja2
+-rw-r--r--   0        0        0      721 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/templates/union_serialization.jinja2
+-rw-r--r--   0        0        0        0 2023-07-20 12:04:36.046946 cerializer-1.3.0/cerializer/tests/__init__.py
+-rw-r--r--   0        0        0     2458 2023-07-20 19:13:45.650277 cerializer-1.3.0/cerializer/tests/benchmark.py
+-rw-r--r--   0        0        0       34 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:1/example.yaml
+-rw-r--r--   0        0        0      193 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:1/schema.yaml
+-rw-r--r--   0        0        0     1020 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:2/example.yaml
+-rw-r--r--   0        0        0      193 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:2/schema.yaml
+-rw-r--r--   0        0        0      736 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:3/example.yaml
+-rw-r--r--   0        0        0      190 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:3/schema.yaml
+-rw-r--r--   0        0        0       40 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:4/example.yaml
+-rw-r--r--   0        0        0      200 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.array_schema:4/schema.yaml
+-rw-r--r--   0        0        0       52 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.bytes_decimal_schema:1/example.yaml
+-rw-r--r--   0        0        0      201 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.bytes_decimal_schema:1/schema.yaml
+-rw-r--r--   0        0        0        5 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:1/example.yaml
+-rw-r--r--   0        0        0      175 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:1/schema.yaml
+-rw-r--r--   0        0        0       13 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:2/example.yaml
+-rw-r--r--   0        0        0      164 2023-07-20 17:29:57.979455 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:2/schema.yaml
+-rw-r--r--   0        0        0       12 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:3/example.yaml
+-rw-r--r--   0        0        0      137 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.default_schema:3/schema.yaml
+-rw-r--r--   0        0        0       11 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.enum_schema:1/example.yaml
+-rw-r--r--   0        0        0      152 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.enum_schema:1/schema.yaml
+-rw-r--r--   0        0        0      161 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.fixed_decimal_schema:1/example.yaml
+-rw-r--r--   0        0        0      505 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.fixed_decimal_schema:1/schema.yaml
+-rw-r--r--   0        0        0       39 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.fixed_schema:1/example.yaml
+-rw-r--r--   0        0        0      130 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.fixed_schema:1/schema.yaml
+-rw-r--r--   0        0        0       87 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.huge_schema:1/example.yaml
+-rw-r--r--   0        0        0      406 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.huge_schema:1/schema.yaml
+-rw-r--r--   0        0        0       54 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.int_date_schema:1/example.yaml
+-rw-r--r--   0        0        0      163 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.int_date_schema:1/schema.yaml
+-rw-r--r--   0        0        0       48 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.long_time_micros_schema:1/example.yaml
+-rw-r--r--   0        0        0      170 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.long_time_micros_schema:1/schema.yaml
+-rw-r--r--   0        0        0       24 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.map_schema:1/example.yaml
+-rw-r--r--   0        0        0      228 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.map_schema:1/schema.yaml
+-rw-r--r--   0        0        0       24 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.map_schema:2/example.yaml
+-rw-r--r--   0        0        0      107 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.map_schema:2/schema.yaml
+-rw-r--r--   0        0        0        3 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.plain_int:1/example.yaml
+-rw-r--r--   0        0        0       49 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.plain_int:1/schema.yaml
+-rw-r--r--   0        0        0      425 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.reference_schema:1/example.yaml
+-rw-r--r--   0        0        0      796 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.reference_schema:1/schema.yaml
+-rw-r--r--   0        0        0       39 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.string_schema:1/example.yaml
+-rw-r--r--   0        0        0      175 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.string_schema:1/schema.yaml
+-rw-r--r--   0        0        0       41 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.string_uuid_schema:1/example.yaml
+-rw-r--r--   0        0        0      141 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.string_uuid_schema:1/schema.yaml
+-rw-r--r--   0        0        0       39 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.timestamp_schema:1/example.yaml
+-rw-r--r--   0        0        0      149 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.timestamp_schema:1/schema.yaml
+-rw-r--r--   0        0        0       39 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.timestamp_schema_micros:1/example.yaml
+-rw-r--r--   0        0        0      149 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.timestamp_schema_micros:1/schema.yaml
+-rw-r--r--   0        0        0       53 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.tree_schema:1/example.yaml
+-rw-r--r--   0        0        0      346 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.tree_schema:1/schema.yaml
+-rw-r--r--   0        0        0        6 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.union_schema:1/example.yaml
+-rw-r--r--   0        0        0      101 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/schemata/cerializer.union_schema:1/schema.yaml
+-rw-r--r--   0        0        0     3943 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/tests/test_cerializer.py
+-rw-r--r--   0        0        0     3062 2023-07-20 17:29:57.982789 cerializer-1.3.0/cerializer/utils.py
+-rw-r--r--   0        0        0      763 2023-07-20 12:04:36.053613 cerializer-1.3.0/prepare.pxd
+-rw-r--r--   0        0        0     8243 2023-07-20 17:29:57.982789 cerializer-1.3.0/prepare.pyx
+-rw-r--r--   0        0        0     2108 2023-07-28 09:13:10.566252 cerializer-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2836 2023-07-20 17:29:57.982789 cerializer-1.3.0/read.pxd
+-rw-r--r--   0        0        0     3146 2023-07-20 12:04:36.053613 cerializer-1.3.0/write.pxd
+-rw-r--r--   0        0        0     8154 1970-01-01 00:00:00.000000 cerializer-1.3.0/PKG-INFO
```

### Comparing `cerializer-1.2.7/README.md` & `cerializer-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# WIP: Cerializer
+# Cerializer
+
+![PyPI](https://img.shields.io/pypi/v/Cerializer)
+
 Cerializer is an Avro de/serialization library that aims at providing an even faster alternative to FastAvro and Avro standard library.
 
 This speed increase does not come without a cost. Cerializer will work only with predefined set of schemata for which it will generate tailor made Cython code. This way, the overhead caused by the universality of other serialization libraries will be avoided.
 
 Special credit needs to be given to [FastAvro](https://github.com/fastavro/fastavro) library, by which is this project heavily inspired.
 
-**Example of a schema and the corresponding code**
+## Example of a schema and the corresponding code
 
 SCHEMA
-```
+```python
 {
     'name': 'array_schema',
     'doc': 'Array schema',
     'namespace': 'cerializer',
     'type': 'record',
     'fields': [
         {
@@ -28,15 +31,15 @@
             }
         }
     ]
 }
 ```
 
 CORRESPONDING CODE
-```
+```python
 def serialize(data, output):
     cdef bytearray buffer = bytearray()
     cdef dict datum
     cdef str type_0
     write.write_string(buffer, data['order_id'])
     if len(data['trades']) > 0:
         write.write_long(buffer, len(data['trades']))
@@ -85,94 +88,93 @@
                 val_2 = read.read_int(fo)
             data['trades'].append(val_2)
         i_1 = read.read_long(fo)
     return data
 ```
 
 
-**Usage Example:**
+## Usage Example
 1. Create an instance of CerializerSchemata
 For initializing CerializerSchemata it is necessary to supply a list of tuples in form of (schema_identifier, schema)
 where schema_identifier is a string and schema is a dict representing the Avro schema.
-schema tuple = (namespace.schema_name, schema)
- eg.
- ```python
-import cerializer.schema_handler
-import os
-import yaml
-
-def list_schemata():
-    # iterates through all your schemata and yields schema_identifier and path to schema folder
-    raise NotImplemented
-
-def schemata() -> cerializer.schema_handler.CerializerSchemata:
-    schemata = []
-	for schema_identifier, schema_root in list_schemata():
-		schema_tuple = schema_identifier, yaml.unsafe_load( # type: ignore
-			open(os.path.join(schema_root, 'schema.yaml'))
-		)
-		schemata.append(schema_tuple)
-	return cerializer.schema_handler.CerializerSchemata(schemata)
-```
+schema tuple = (namespace.schema_name, schema). eg.:
+    ```python
+    import cerializer.schema_handler
+    import os
+    import yaml
+    
+    def list_schemata():
+        # iterates through all your schemata and yields schema_identifier and path to schema folder
+        raise NotImplemented
+    
+    def schemata() -> cerializer.schema_handler.CerializerSchemata:
+        schemata = []
+        for schema_identifier, schema_root in list_schemata():
+            schema_tuple = schema_identifier, yaml.unsafe_load( # type: ignore
+                open(os.path.join(schema_root, 'schema.yaml'))
+            )
+            schemata.append(schema_tuple)
+        return cerializer.schema_handler.CerializerSchemata(schemata)
+    ```
 
-2. Create an instance of Cerializer for each of your schemata by calling `cerializer_handler.Cerializer` .
+2. Create an instance of Cerializer for each of your schemata by calling `cerializer_handler.Cerializer`.
 eg. `cerializer_instance = cerializer_handler.Cerializer(cerializer_schemata, schema_namespace, schema_name)`
 This will create an instance of Cerializer that can serialize and deserialize data in the particular schema format.
 
 3. Use the instance accordingly.
-  eg.
-  ```python
- data_record = {
-    'order_id': 'aaaa',
-    'trades': [123, 456, 765]
-}
-
- cerializer_instance = cerializer.cerializer_handler.Cerializer(cerializer_schemata, 'school', 'student')
- serialized_data = cerializer_instance.serialize(data_record)
- print(serialized_data)
-```
+    eg.:
+    ```python
+    data_record = {
+        'order_id': 'aaaa',
+        'trades': [123, 456, 765]
+    }
+    
+    cerializer_instance = cerializer.cerializer_handler.Cerializer(cerializer_schemata, 'school', 'student')
+    serialized_data = cerializer_instance.serialize(data_record)
+    print(serialized_data)
+    ```
 
 Serialized data
 ```
 b'\x08aaaa\x06\x02\xf6\x01\x02\x90\x07\x02\xfa\x0b\x00'
 ```
 
 You can also use `serialize_into` if you already have an IO buffer:
 
 ```python
 output = io.BytesIO()
 cerializer_instance.serialize_into(output, data_record)
 print(output.getvalue())
 ```
 
-**benchmark**
+## Benchmark
 ```
-cerializer.huge_schema:1               3.6394 times faster,   1.4231s : 0.3910s
-cerializer.timestamp_schema_micros:1   1.7470 times faster,   0.2759s : 0.1579s
-cerializer.default_schema:1            1.4456 times faster,   0.2392s : 0.1655s
-cerializer.fixed_schema:1              1.6654 times faster,   0.0980s : 0.0589s
-cerializer.map_schema:2                1.6411 times faster,   0.2103s : 0.1281s
-cerializer.enum_schema:1               1.5498 times faster,   0.1079s : 0.0696s
-cerializer.array_schema:2              1.3455 times faster,   4.9207s : 3.6572s
-cerializer.array_schema:3              1.3385 times faster,   2.3153s : 1.7297s
-cerializer.array_schema:4              4.2781 times faster,   12.3307s : 2.8823s
-cerializer.timestamp_schema:1          1.6614 times faster,   0.2454s : 0.1477s
-cerializer.default_schema:3            1.5040 times faster,   0.1191s : 0.0792s
-cerializer.tree_schema:1               4.1126 times faster,   0.6619s : 0.1609s
-cerializer.default_schema:2            1.5767 times faster,   0.1261s : 0.0800s
-cerializer.string_schema:1             1.5083 times faster,   0.2119s : 0.1405s
-cerializer.plain_int:1                 1.8953 times faster,   0.1286s : 0.0678s
-cerializer.union_schema:1              1.9114 times faster,   0.1755s : 0.0918s
-cerializer.fixed_decimal_schema:1      1.2929 times faster,   2.2791s : 1.7627s
-cerializer.int_date_schema:1           2.3736 times faster,   0.1702s : 0.0717s
-cerializer.reference_schema:1          2.1570 times faster,   0.9120s : 0.4228s
-cerializer.bytes_decimal_schema:1      1.6603 times faster,   0.3401s : 0.2049s
-cerializer.string_uuid_schema:1        1.5366 times faster,   0.3236s : 0.2106s
-cerializer.map_schema:1                4.1051 times faster,   0.5873s : 0.1431s
-cerializer.long_time_micros_schema:1   1.9305 times faster,   0.2250s : 0.1166s
-cerializer.array_schema:1              1.4784 times faster,   0.1987s : 0.1344s
-AVERAGE: 2.1894 times faster
+cerializer.default_schema:3            2.5661 times faster,   0.0209s : 0.0082s
+cerializer.fixed_decimal_schema:1      1.2795 times faster,   0.1588s : 0.1241s
+cerializer.int_date_schema:1           2.8285 times faster,   0.0273s : 0.0097s
+cerializer.plain_int:1                 2.2334 times faster,   0.0146s : 0.0065s
+cerializer.timestamp_schema_micros:1   2.3759 times faster,   0.0577s : 0.0243s
+cerializer.default_schema:2            2.8129 times faster,   0.0240s : 0.0085s
+cerializer.array_schema:3              1.2177 times faster,   0.3088s : 0.2536s
+cerializer.timestamp_schema:1          2.5928 times faster,   0.0577s : 0.0223s
+cerializer.array_schema:2              1.4756 times faster,   0.6542s : 0.4434s
+cerializer.union_schema:1              3.0796 times faster,   0.0284s : 0.0092s
+cerializer.bytes_decimal_schema:1      1.8449 times faster,   0.0490s : 0.0266s
+cerializer.array_schema:1              2.1771 times faster,   0.0344s : 0.0158s
+cerializer.string_uuid_schema:1        1.8887 times faster,   0.0494s : 0.0262s
+cerializer.map_schema:2                2.0896 times faster,   0.0331s : 0.0158s
+cerializer.fixed_schema:1              3.4042 times faster,   0.0213s : 0.0062s
+cerializer.long_time_micros_schema:1   2.3747 times faster,   0.0352s : 0.0148s
+cerializer.array_schema:4              2.8779 times faster,   0.0591s : 0.0205s
+cerializer.default_schema:1            2.0182 times faster,   0.0393s : 0.0195s
+cerializer.map_schema:1                3.4610 times faster,   0.0597s : 0.0172s
+cerializer.string_schema:1             2.2048 times faster,   0.0352s : 0.0159s
+cerializer.reference_schema:1          2.9309 times faster,   0.1525s : 0.0520s
+cerializer.enum_schema:1               3.0065 times faster,   0.0217s : 0.0072s
+cerializer.tree_schema:1               4.0494 times faster,   0.0869s : 0.0215s
+cerializer.huge_schema:1               2.8161 times faster,   0.1453s : 0.0516s
+AVERAGE: 1.7814 times faster
 ```
 
 Measured against Fastavro using the benchmark in Cerializer/tests.
 
-Device: MacBook Pro 13-inch, 2020, 1,4 GHz Quad-Core Intel Core i5, 16 GB 2133 MHz LPDDR3
+Device: ASUS ZenBook 14 UM425QA, AMD Ryzen 7 5800H, 16 GB 2133 MHz LPDDR4X
```

### Comparing `cerializer-1.2.7/cerializer/cerializer_handler.py` & `cerializer-1.3.0/cerializer/cerializer_handler.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/compiler.py` & `cerializer-1.3.0/cerializer/compiler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # pylint: disable=protected-access, deprecated-method, no-value-for-parameter
 import distutils.core  # pylint: disable=deprecated-module
 import hashlib
 import importlib.machinery
+import importlib.util
 import os.path  # pylint: disable=no-name-in-module
 import sys
-from typing import Any, List
+from typing import Any, List, cast
 
 import Cython.Build.Dependencies
 import Cython.Build.Inline
 import Cython.Compiler.Main
 import Cython.Utils
 
 
 def compile_code(code: str) -> Any:
 	return _cython_inline(code)
 
 
 def _load_dynamic(name: str, module_path: str) -> Any:
-	# mypy does not understand ExtensionFileLoader init
-	return importlib.machinery.ExtensionFileLoader(name, module_path).load_module()  # type: ignore
+	loader = importlib.machinery.ExtensionFileLoader(name, module_path)
+	spec = cast(importlib.machinery.ModuleSpec, importlib.util.spec_from_loader(name, loader))
+	module = importlib.util.module_from_spec(spec)
+	loader.exec_module(module)
+	return module
 
 
 def _cython_inline(
 	complete_code: str,
 	lib_dir: str = os.path.join(Cython.Utils.get_cython_cache_dir(), 'inline'),
 ) -> Any:
 	key = complete_code, sys.version_info, sys.executable, 3, Cython.__version__
```

### Comparing `cerializer-1.2.7/cerializer/constants.py` & `cerializer-1.3.0/cerializer/constants.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/schema_handler.py` & `cerializer-1.3.0/cerializer/schema_handler.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/schema_parser.py` & `cerializer-1.3.0/cerializer/schema_parser.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/templates/union_serialization.jinja2` & `cerializer-1.3.0/cerializer/templates/union_serialization.jinja2`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/tests/benchmark.py` & `cerializer-1.3.0/cerializer/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/tests/test_cerializer.py` & `cerializer-1.3.0/cerializer/tests/test_cerializer.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/cerializer/utils.py` & `cerializer-1.3.0/cerializer/utils.py`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/prepare.pxd` & `cerializer-1.3.0/prepare.pxd`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/prepare.pyx` & `cerializer-1.3.0/prepare.pyx`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/read.pxd` & `cerializer-1.3.0/read.pxd`

 * *Files identical despite different names*

### Comparing `cerializer-1.2.7/write.pxd` & `cerializer-1.3.0/write.pxd`

 * *Files identical despite different names*

