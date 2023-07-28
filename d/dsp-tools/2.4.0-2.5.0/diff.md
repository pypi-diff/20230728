# Comparing `tmp/dsp_tools-2.4.0.tar.gz` & `tmp/dsp_tools-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.4.0.tar", max compression
+gzip compressed data, was "dsp_tools-2.5.0.tar", max compression
```

## Comparing `dsp_tools-2.4.0.tar` & `dsp_tools-2.5.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    35149 2023-07-12 09:35:04.011926 dsp_tools-2.4.0/LICENSE
--rw-r--r--   0        0        0     4602 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/docs/index.md
--rw-r--r--   0        0        0     5007 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    20863 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    89253 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    31627 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14293 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4185 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0     1059 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     8708 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3325 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8851 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16528 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     8979 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    20524 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      463 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    14896 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2350 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    16761 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1744 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    18840 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1930 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    20694 2023-07-12 09:35:04.031927 dsp_tools-2.4.0/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    29833 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      496 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0     1040 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    25439 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    33397 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     1971 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      594 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0     1504 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2172 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8720 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2141 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0        0 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23544 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     2460 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15142 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4912 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     8237 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10530 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3189 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0     1134 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/logging.py
--rw-r--r--   0        0        0    42361 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8373 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4694 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18815 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4259 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    13326 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0    13540 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    51547 2023-07-12 09:35:04.035927 dsp_tools-2.4.0/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 dsp_tools-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-28 08:19:29.730879 dsp_tools-2.5.0/LICENSE
+-rw-r--r--   0        0        0     4602 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/docs/index.md
+-rw-r--r--   0        0        0     5007 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    24318 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    89253 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    38361 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14344 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4185 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0     1059 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     8718 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3325 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8851 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16528 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     8979 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    20524 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      463 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    14896 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2350 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    16761 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1744 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    18840 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1930 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    20694 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    29833 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      496 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0     1087 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    25439 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    33397 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     1971 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      594 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1504 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2172 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8720 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2141 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0        0 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23808 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     2460 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15142 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4912 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     8237 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10530 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3189 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0     1424 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/logging.py
+-rw-r--r--   0        0        0    42361 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8373 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4694 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18815 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4259 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    13326 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0    13872 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    52419 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 dsp_tools-2.5.0/PKG-INFO
```

### Comparing `dsp_tools-2.4.0/LICENSE` & `dsp_tools-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/docs/index.md` & `dsp_tools-2.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/pyproject.toml` & `dsp_tools-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.4.0"
+version = "2.5.0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.5.0/src/dsp_tools/dsp_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 The code in this file handles the arguments passed by the user from the command line and calls the requested actions.
 """
 import argparse
 import datetime
 import sys
 from importlib.metadata import version
 
+import regex
+
 from dsp_tools.excel2xml import excel2xml
 from dsp_tools.fast_xmlupload.process_files import process_files
 from dsp_tools.fast_xmlupload.upload_files import upload_files
 from dsp_tools.fast_xmlupload.upload_xml import fast_xmlupload
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.excel_to_json_lists import excel2lists, validate_lists_section_with_schema
 from dsp_tools.utils.excel_to_json_project import excel2json
@@ -26,33 +28,30 @@
 from dsp_tools.utils.shared import validate_xml_against_schema
 from dsp_tools.utils.stack_handling import StackConfiguration, StackHandler
 from dsp_tools.utils.xml_upload import xml_upload
 
 logger = get_logger(__name__)
 
 
-def make_parser() -> argparse.ArgumentParser:
+def _make_parser(
+    default_dsp_api_url: str,
+    root_user_email: str,
+    root_user_pw: str,
+) -> argparse.ArgumentParser:
     """
     Create a parser for the command line arguments
 
     Returns:
         parser
     """
     # help texts
-    username_text = "username (e-mail) used for authentication with the DSP-API "
-    password_text = "password used for authentication with the DSP-API "
+    username_text = "username (e-mail) used for authentication with the DSP-API"
+    password_text = "password used for authentication with the DSP-API"
     dsp_server_text = "URL of the DSP server"
     verbose_text = "print more information about the progress to the console"
-    sipi_text = "URL of the Sipi server"
-
-    # default values
-    default_dsp_api_url = "http://0.0.0.0:3333"
-    default_user = "root@example.com"
-    default_pw = "test"
-    default_sipi = "http://0.0.0.0:1024"
 
     # make a parser
     parser = argparse.ArgumentParser(
         description=f"DSP-TOOLS (version {version('dsp-tools')}, © {datetime.datetime.now().year} by DaSCH)"
     )
     subparsers = parser.add_subparsers(
         title="Subcommands", description="Valid subcommands are", help="sub-command help"
@@ -62,16 +61,16 @@
     parser_create = subparsers.add_parser(
         name="create",
         help="Create a project defined in a JSON project file on a DSP server. "
         "A project can consist of lists, groups, users, and ontologies (data models).",
     )
     parser_create.set_defaults(action="create")
     parser_create.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
-    parser_create.add_argument("-u", "--user", default=default_user, help=username_text)
-    parser_create.add_argument("-p", "--password", default=default_pw, help=password_text)
+    parser_create.add_argument("-u", "--user", default=root_user_email, help=username_text)
+    parser_create.add_argument("-p", "--password", default=root_user_pw, help=password_text)
     parser_create.add_argument(
         "-V",
         "--validate-only",
         action="store_true",
         help="validate the JSON file without creating it on the DSP server",
     )
     parser_create.add_argument(
@@ -87,34 +86,28 @@
     # get
     parser_get = subparsers.add_parser(
         name="get",
         help="Retrieve a project with its data model(s) from a DSP server and write it into a JSON file",
     )
     parser_get.set_defaults(action="get")
     parser_get.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
-    parser_get.add_argument("-u", "--user", default=default_user, help=username_text)
-    parser_get.add_argument("-p", "--password", default=default_pw, help=password_text)
+    parser_get.add_argument("-u", "--user", default=root_user_email, help=username_text)
+    parser_get.add_argument("-p", "--password", default=root_user_pw, help=password_text)
     parser_get.add_argument("-P", "--project", help="shortcode, shortname or IRI of the project", required=True)
     parser_get.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_get.add_argument("project_definition", help="path to the file the project should be written to")
 
     # xmlupload
     parser_upload = subparsers.add_parser(name="xmlupload", help="Upload data defined in an XML file to a DSP server")
     parser_upload.set_defaults(action="xmlupload")
     parser_upload.add_argument(
         "-s", "--server", default=default_dsp_api_url, help="URL of the DSP server where DSP-TOOLS sends the data to"
     )
-    parser_upload.add_argument("-u", "--user", default=default_user, help=username_text)
-    parser_upload.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_upload.add_argument(
-        "-S",
-        "--sipi",
-        default=default_sipi,
-        help="URL of the SIPI server where DSP-TOOLS sends the multimedia files to",
-    )
+    parser_upload.add_argument("-u", "--user", default=root_user_email, help=username_text)
+    parser_upload.add_argument("-p", "--password", default=root_user_pw, help=password_text)
     parser_upload.add_argument(
         "-i", "--imgdir", default=".", help="folder from where the paths in the <bitstream> tags are evaluated"
     )
     parser_upload.add_argument(
         "-I",
         "--incremental",
         action="store_true",
@@ -136,41 +129,42 @@
     parser_process_files.add_argument(
         "--input-dir", help="path to the input directory where the files should be read from"
     )
     parser_process_files.add_argument(
         "--output-dir", help="path to the output directory where the processed/transformed files should be written to"
     )
     parser_process_files.add_argument("--nthreads", type=int, default=None, help="number of threads to use")
+    parser_process_files.add_argument(
+        "--batchsize", type=int, default=5000, help="number of files to process before Python exits"
+    )
     parser_process_files.add_argument("xml_file", help="path to XML file containing the data")
 
     # upload-files
     parser_upload_files = subparsers.add_parser(
         name="upload-files",
         help="For internal use only: upload already processed files",
     )
     parser_upload_files.set_defaults(action="upload-files")
     parser_upload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_upload_files.add_argument("-d", "--processed-dir", help="path to the directory with the processed files")
     parser_upload_files.add_argument("-n", "--nthreads", type=int, default=4, help="number of threads to use")
     parser_upload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
-    parser_upload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
-    parser_upload_files.add_argument("-u", "--user", default=default_user, help=username_text)
-    parser_upload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
+    parser_upload_files.add_argument("-u", "--user", default=root_user_email, help=username_text)
+    parser_upload_files.add_argument("-p", "--password", default=root_user_pw, help=password_text)
 
     # fast-xmlupload
     parser_fast_xmlupload_files = subparsers.add_parser(
         name="fast-xmlupload",
         help="For internal use only: create resources with already uploaded files",
     )
     parser_fast_xmlupload_files.set_defaults(action="fast-xmlupload")
     parser_fast_xmlupload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_fast_xmlupload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
-    parser_fast_xmlupload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
-    parser_fast_xmlupload_files.add_argument("-u", "--user", default=default_user, help=username_text)
-    parser_fast_xmlupload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
+    parser_fast_xmlupload_files.add_argument("-u", "--user", default=root_user_email, help=username_text)
+    parser_fast_xmlupload_files.add_argument("-p", "--password", default=root_user_pw, help=password_text)
     parser_fast_xmlupload_files.add_argument("xml_file", help="path to XML file containing the data")
 
     # excel2json
     parser_excel2json = subparsers.add_parser(
         name="excel2json",
         help="Create an entire JSON project file from a folder containing the required Excel files",
     )
@@ -266,14 +260,37 @@
         name="rosetta", help="Clone the most up to data rosetta repository, create the data model and upload the data"
     )
     parser_rosetta.set_defaults(action="rosetta")
 
     return parser
 
 
+def _parse_arguments(
+    user_args: list[str],
+    parser: argparse.ArgumentParser,
+) -> argparse.Namespace:
+    """
+    Parse the user-provided CLI arguments.
+    If no action is provided,
+    print the help text and exit with error code 1.
+
+    Args:
+        user_args: user-provided CLI arguments
+        parser: parser used to parse the arguments
+
+    Returns:
+        parsed arguments
+    """
+    args = parser.parse_args(user_args)
+    if not hasattr(args, "action"):
+        parser.print_help(sys.stderr)
+        sys.exit(1)
+    return args
+
+
 def _log_cli_arguments(parsed_args: argparse.Namespace) -> None:
     """
     Log the CLI arguments passed by the user from the command line.
 
     Args:
         parsed_args: parsed arguments
     """
@@ -295,40 +312,113 @@
     logger.info("*" * asterisk_count)
     logger.info(msg)
     for line in lines:
         logger.info(line)
     logger.info("*" * asterisk_count)
 
 
-def call_requested_action(
-    user_args: list[str],
-    parser: argparse.ArgumentParser,
-) -> bool:
+def _get_canonical_server_and_sipi_url(
+    server: str,
+    default_dsp_api_url: str,
+    default_sipi_url: str,
+) -> tuple[str, str]:
     """
-    With the help of the parser, parse the user arguments and call the appropriate method of DSP-TOOLS.
+    Based on the DSP server URL passed by the user,
+    transform it to its canonical form,
+    and derive the SIPI URL from it.
+
+    If the DSP server URL points to port 3333 on localhost,
+    the SIPI URL will point to port 1024 on localhost.
+
+    If the DSP server URL points to a remote server ending in "dasch.swiss",
+    modify it (if necessary) to point to the "api" subdomain of that server,
+    and add a new "sipi_url" argument pointing to the "iiif" subdomain of that server.
 
     Args:
-        user_args: list of arguments passed by the user from the command line
-        parser: parser to parse the user arguments
+        server: DSP server URL passed by the user
+        default_dsp_api_url: default DSP server on localhost
+        default_sipi_url: default SIPI server on localhost
+
+    Raises:
+        UserError: if the DSP server URL passed by the user is invalid
+
+    Returns:
+        canonical DSP URL and SIPI URL
+    """
+    localhost_match = regex.search(r"(0\.0\.0\.0|localhost):3333", server)
+    remote_url_match = regex.search(r"^(?:https?:\/\/)?(?:admin\.|api\.|iiif\.|app\.)?((?:.+\.)?dasch)\.swiss", server)
+
+    if localhost_match:
+        server = default_dsp_api_url
+        sipi_url = default_sipi_url
+    elif remote_url_match:
+        server = f"https://api.{remote_url_match.group(1)}.swiss"
+        sipi_url = f"https://iiif.{remote_url_match.group(1)}.swiss"
+    else:
+        logger.error(f"Invalid DSP server URL '{server}'")
+        raise UserError(f"ERROR: Invalid DSP server URL '{server}'")
+
+    logger.info(f"Using DSP server '{server}' and SIPI server '{sipi_url}'")
+    print(f"Using DSP server '{server}' and SIPI server '{sipi_url}'")
+
+    return server, sipi_url
+
+
+def _derive_sipi_url(
+    parsed_arguments: argparse.Namespace,
+    default_dsp_api_url: str,
+    default_sipi_url: str,
+) -> argparse.Namespace:
+    """
+    Modify the parsed arguments so that the DSP and SIPI URLs are correct.
+    Based on the DSP server URL passed by the user,
+    transform it to its canonical form,
+    and derive the SIPI URL from it.
+
+    Args:
+        parsed_arguments: CLI arguments passed by the user, parsed by argparse
+        default_dsp_api_url: default DSP server on localhost
+        default_sipi_url: default SIPI server on localhost
+
+    Raises:
+        UserError: if the DSP server URL passed by the user is invalid
+
+    Returns:
+        the modified arguments
+    """
+    if not hasattr(parsed_arguments, "server"):
+        # some CLI actions (like excel2json, excel2xml, start-stack, ...) don't have a server at all
+        return parsed_arguments
+
+    server, sipi_url = _get_canonical_server_and_sipi_url(
+        server=parsed_arguments.server,
+        default_dsp_api_url=default_dsp_api_url,
+        default_sipi_url=default_sipi_url,
+    )
+    parsed_arguments.server = server
+    parsed_arguments.sipi_url = sipi_url
+
+    return parsed_arguments
+
+
+def _call_requested_action(args: argparse.Namespace) -> bool:
+    """
+    Call the appropriate method of DSP-TOOLS.
+
+    Args:
+        args: parsed CLI arguments
 
     Raises:
         BaseError from the called methods
         UserError from the called methods
         unexpected errors from the called methods and underlying libraries
 
     Returns:
         success status
     """
-    args = parser.parse_args(user_args)
-    if not hasattr(args, "action"):
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-
-    _log_cli_arguments(args)
-
     if args.action == "create":
         if args.lists_only:
             if args.validate_only:
                 success = validate_lists_section_with_schema(path_to_json_project_file=args.project_definition)
                 print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
             else:
                 _, success = create_lists(
@@ -366,27 +456,27 @@
         else:
             success = xml_upload(
                 input_file=args.xmlfile,
                 server=args.server,
                 user=args.user,
                 password=args.password,
                 imgdir=args.imgdir,
-                sipi=args.sipi,
+                sipi=args.sipi_url,
                 verbose=args.verbose,
                 incremental=args.incremental,
                 save_metrics=args.metrics,
                 preprocessing_done=False,
             )
-
     elif args.action == "process-files":
         success = process_files(
             input_dir=args.input_dir,
             output_dir=args.output_dir,
             xml_file=args.xml_file,
             nthreads=args.nthreads,
+            batch_size=args.batchsize,
         )
     elif args.action == "upload-files":
         success = upload_files(
             pkl_file=args.pkl_file,
             dir_with_processed_files=args.processed_dir,
             nthreads=args.nthreads,
             user=args.user,
@@ -459,18 +549,40 @@
         print(f"ERROR: Unknown action '{args.action}'")
         logger.error(f"Unknown action '{args.action}'")
 
     return success
 
 
 def main() -> None:
-    """Main entry point of the program as referenced in pyproject.toml"""
-    parser = make_parser()
+    """
+    Main entry point of the program as referenced in pyproject.toml
+    """
+    default_dsp_api_url = "http://0.0.0.0:3333"
+    default_sipi_url = "http://0.0.0.0:1024"
+    root_user_email = "root@example.com"
+    root_user_pw = "test"
+
+    parser = _make_parser(
+        default_dsp_api_url=default_dsp_api_url,
+        root_user_email=root_user_email,
+        root_user_pw=root_user_pw,
+    )
+    parsed_arguments = _parse_arguments(
+        user_args=sys.argv[1:],
+        parser=parser,
+    )
+    _log_cli_arguments(parsed_arguments)
+
     try:
-        success = call_requested_action(user_args=sys.argv[1:], parser=parser)
+        parsed_arguments = _derive_sipi_url(
+            parsed_arguments=parsed_arguments,
+            default_dsp_api_url=default_dsp_api_url,
+            default_sipi_url=default_sipi_url,
+        )
+        success = _call_requested_action(parsed_arguments)
     except UserError as err:
         print(err.message)
         sys.exit(1)
     # let BaseError and all unexpected errors escalate, so that a stack trace is printed
 
     if not success:
         sys.exit(1)
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/excel2xml.py` & `dsp_tools-2.5.0/src/dsp_tools/excel2xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,172 +13,185 @@
 from typing import Any, Optional, Union
 
 import docker
 import requests
 from docker.models.containers import Container
 from lxml import etree
 
-from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logging import get_logger
 
-logger = get_logger(__name__)
+logger = get_logger(__name__, filesize_mb=100, backupcount=36)
 sipi_container: Optional[Container] = None
 export_moving_image_frames_script: Optional[Path] = None
 
 
 def _get_export_moving_image_frames_script() -> None:
     """
     Downloads the shell script that is used to extract the preview image from a video.
     """
     user_folder = Path.home() / Path(".dsp-tools/fast-xmlupload")
     user_folder.mkdir(parents=True, exist_ok=True)
     global export_moving_image_frames_script
     export_moving_image_frames_script = user_folder / "export-moving-image-frames.sh"
     script_text = requests.get(
         "https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh",
-        timeout=5,
+        timeout=10,
     ).text
     with open(export_moving_image_frames_script, "w", encoding="utf-8") as f:
         f.write(script_text)
 
 
-def _check_if_all_files_were_processed(
-    result: list[tuple[Path, Optional[Path]]],
-    all_paths: list[Path],
-) -> bool:
-    """
-    Go through the result list and print all files that could not be processed.
-
-    Args:
-        result: list of tuples of Paths. If the second Path is None, the file could not be processed.
-        all_paths: list of all paths that should have been processed
+def _determine_success_status_and_exit_code(
+    files_to_process: list[Path],
+    processed_files: list[tuple[Path, Optional[Path]]],
+    is_last_batch: bool,
+) -> tuple[bool, int]:
+    """
+    Based on the result of the file processing,
+    this function determines the success status and the exit code.
+    If some files of the current batch could not be processed,
+    the success status is false, and the exit code is 1.
+    If all files of the current batch were processed, the success status is true,
+    and the exit code is 0 if this is the last batch,
+    and 2 if there are more batches to process.
+
+    Args:
+        files_to_process: list of all paths that should have been processed (current batch)
+        processed_files: list of tuples of Paths. If the second Path is None, the file could not be processed.
+        is_last_batch: true if this is the last batch of files to process
 
     Returns:
-        success status
+        tuple (success status, exit_code)
     """
-    processed_paths = [x[1] for x in result if x[1]]
-    if len(processed_paths) == len(all_paths):
+    processed_paths = [x[1] for x in processed_files if x and x[1]]
+    if len(processed_paths) == len(files_to_process):
         success = True
-        print(f"{datetime.now()}: Number of processed files: {len(result)}: Okay")
-        logger.info(f"Number of processed files: {len(result)}: Okay")
+        print(f"{datetime.now()}: All files ({len(files_to_process)}) of this batch were processed: Okay")
+        logger.info(f"All files ({len(files_to_process)}) of this batch were processed: Okay")
+        if is_last_batch:
+            exit_code = 0
+            print(f"{datetime.now()}: All multimedia files referenced in the XML are processed. No more batches.")
+            logger.info("All multimedia files referenced in the XML are processed. No more batches.")
+        else:
+            exit_code = 2
     else:
         success = False
-        ratio = f"{len(processed_paths)}/{len(all_paths)}"
-        msg = f"Some files could not be processed: Only {ratio} were processed. The failed ones are:"
+        ratio = f"{len(processed_paths)}/{len(files_to_process)}"
+        msg = f"Some files of this batch could not be processed: Only {ratio} were processed. The failed ones are:"
         print(f"{datetime.now()}: ERROR: {msg}")
         logger.error(msg)
+        for input_file, output_file in processed_files:
+            if not output_file:
+                print(f" - {input_file}")
+                logger.error(f" - {input_file}")
+        exit_code = 1
 
-    for input_file, output_file in result:
-        if not output_file:
-            print(f" - {input_file}")
-            logger.error(f" - {input_file}")
-
-    return success
+    return success, exit_code
 
 
 def _process_files_in_parallel(
-    paths: list[Path],
+    files_to_process: list[Path],
     input_dir: Path,
     output_dir: Path,
     nthreads: Optional[int],
 ) -> tuple[list[tuple[Path, Optional[Path]]], list[Path]]:
     """
     Creates a thread pool and executes the file processing in parallel.
     If a Docker API error occurs, the SIPI container is restarted,
     and the unprocessed files are returned,
     so that this function can be called again with the unprocessed files.
 
     Args:
-        paths: a list of all paths to the files that should be processed
+        files_to_process: a list of all paths to the files that should be processed
         input_dir: the root directory of the input files
         output_dir: the directory where the processed files should be written to
         nthreads: number of threads to use for processing
 
     Returns:
         - a list of tuples with the original file path and the path to the processed file.
           (if a file could not be processed, the second path is None)
         - a list of all paths that could not be processed
           (this list will only have content if a Docker API error led to a restart of the SIPI container)
     """
     with ThreadPoolExecutor(max_workers=nthreads) as pool:
-        processing_jobs = [pool.submit(_process_file, input_file, input_dir, output_dir) for input_file in paths]
+        processing_jobs = [pool.submit(_process_file, f, input_dir, output_dir) for f in files_to_process]
 
     orig_filepath_2_uuid: list[tuple[Path, Optional[Path]]] = []
     for processed in as_completed(processing_jobs):
         try:
             orig_filepath_2_uuid.append(processed.result())
         except docker.errors.APIError:
             print(f"{datetime.now()}: ERROR: A Docker exception occurred. Cancel jobs and restart SIPI...")
             logger.error("A Docker exception occurred. Cancel jobs and restart SIPI...", exc_info=True)
             for job in processing_jobs:
                 job.cancel()
             _stop_and_remove_sipi_container()
             _start_sipi_container_and_mount_volumes(input_dir, output_dir)
             processed_paths = [x[0] for x in orig_filepath_2_uuid]
-            unprocessed_paths = [x for x in paths if x not in processed_paths]
+            unprocessed_paths = [x for x in files_to_process if x not in processed_paths]
             return orig_filepath_2_uuid, unprocessed_paths
 
     return orig_filepath_2_uuid, []
 
 
-def _write_result_to_pkl_file(result: list[tuple[Path, Optional[Path]]]) -> bool:
+def _write_result_to_pkl_file(processed_files: list[tuple[Path, Optional[Path]]]) -> None:
     """
-    Writes the processing result to a pickle file.
+    Writes the processing result to a pickle file in the working directory.
 
     Args:
-        result: the result of the file processing
+        processed_files: the result of the file processing
 
-    Returns:
-        true if successful, false otherwise
+    Raises:
+        UserError if the file could not be written
     """
-    filename = "processing_result_" + datetime.now().strftime("%Y%m%d_%H%M%S") + ".pkl"
+    filename = f"processing_result_{datetime.now().strftime('%Y%m%d_%H%M%S')}.pkl"
     try:
         with open(filename, "wb") as pkl_file:
-            pickle.dump(result, pkl_file)
+            pickle.dump(processed_files, pkl_file)
         print(f"{datetime.now()}: The result was written to: {filename}")
-        return True
     except OSError:
-        err_msg = f"An error occurred while writing the result to the pickle file. Content of file: {result}"
-        print(f"{datetime.now()}: {err_msg}")
+        err_msg = f"An error occurred while writing the result to the pickle file. Content of file: {processed_files}"
         logger.error(err_msg, exc_info=True)
-        return False
+        raise UserError(err_msg) from None
 
 
-def _check_params(
+def _check_input_params(
     input_dir: str,
     out_dir: str,
     xml_file: str,
-) -> Optional[tuple[Path, Path, Path]]:
+) -> tuple[Path, Path, Path]:
     """
-    Checks the input parameters provided by the user and transforms them into the expected types.
+    Checks the input parameters provided by the user and transforms them into Path objects.
+    If the output directory doesn't exist, it is created.
 
     Args:
         input_dir: the root directory of the input files
         out_dir: the output directory where the created files should be written to
         xml_file: the XML file the paths are extracted from
 
+    Raises:
+        UserError: if one of the parameters is not valid
+
     Returns:
         A tuple with the Path objects of the input strings
     """
     input_dir_path = Path(input_dir)
     out_dir_path = Path(out_dir)
     xml_file_path = Path(xml_file)
 
-    if not _ensure_directory_exists(out_dir_path):
-        return None
+    try:
+        out_dir_path.mkdir(parents=True, exist_ok=True)
+    except Exception:  # pylint: disable=broad-exception-caught
+        raise UserError(f"Couldn't create directory {out_dir_path}") from None
 
     if not input_dir_path.is_dir():
-        print("input_dir is not a directory")
-        return None
-    if not out_dir_path.is_dir():
-        print("out_dir is not a directory")
-        return None
+        raise UserError("input_dir is not a directory")
     if not xml_file_path.is_file():
-        print("xml_file is not a file")
-        return None
+        raise UserError("xml_file is not a file")
 
     return input_dir_path, out_dir_path, xml_file_path
 
 
 def _get_file_paths_from_xml(xml_file: Path) -> list[Path]:
     """
     Parse XML file to get all file paths.
@@ -510,34 +523,14 @@
     result = subprocess.call(["/bin/bash", f"{export_moving_image_frames_script}", "-i", f"{file}"])
     if result != 0:
         return False
     else:
         return True
 
 
-def _ensure_directory_exists(path: Path) -> bool:
-    """
-    Try to create the directory at the given path.
-    If the directory already exists, nothing happens.
-
-    Args:
-        path: path to the directory that should be created
-
-    Returns:
-        True if the directory exists or was created successfully, False if an error occurred during the creation.
-    """
-    try:
-        path.mkdir(parents=True, exist_ok=True)
-        return True
-    except Exception:  # pylint: disable=broad-exception-caught
-        print(f"{datetime.now()}: ERROR: Couldn't create directory {path}")
-        logger.error(f"Couldn't create directory {path}", exc_info=True)
-        return False
-
-
 def _process_file(
     in_file: Path,
     input_dir: Path,
     output_dir: Path,
 ) -> tuple[Path, Optional[Path]]:
     """
     Creates all expected derivative files and writes the output into the provided output directory.
@@ -731,131 +724,277 @@
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for video '{in_file}'")
         logger.error(f"Couldn't create sidecar file for video '{in_file}'")
         return in_file, None
 
     return in_file, converted_file_full_path
 
 
+def _write_processed_and_unprocessed_files_to_txt_files(
+    all_files: list[Path],
+    processed_files: list[tuple[Path, Optional[Path]]],
+) -> None:
+    """
+    Determine the files that were processed until now
+    (taking into account a possibly existing file 'processed_files.txt')
+    and write them to 'processed_files.txt'.
+    Determine the files that were not processed until now,
+    and write them to 'unprocessed_files.txt'
+    (possibly overwriting an existing file).
+
+    Args:
+        all_files: list of all paths that should be processed
+        processed_files: list of tuples (orig path, processed path). 2nd path is None if a file could not be processed.
+    """
+    processed_original_paths = [x[0] for x in processed_files]
+    if Path("processed_files.txt").is_file():
+        with open("processed_files.txt", "r", encoding="utf-8") as f:
+            previously_processed_files = [Path(x) for x in f.read().splitlines()]
+        processed_original_paths = processed_original_paths + previously_processed_files
+
+    with open("processed_files.txt", "w", encoding="utf-8") as f:
+        f.write("\n".join([str(x) for x in processed_original_paths]))
+    msg = "Wrote 'processed_files.txt'"
+
+    unprocessed_original_paths = [x for x in all_files if x not in processed_original_paths]
+    if unprocessed_original_paths:
+        with open("unprocessed_files.txt", "w", encoding="utf-8") as f:
+            f.write("\n".join([str(x) for x in unprocessed_original_paths]))
+        msg += " and 'unprocessed_files.txt'"
+    elif Path("unprocessed_files.txt").is_file():
+        Path("unprocessed_files.txt").unlink()
+        msg += " and removed 'unprocessed_files.txt'"
+
+    print(f"{datetime.now()}: {msg}")
+    logger.info(msg)
+
+
 def handle_interruption(
-    all_paths: list[Path],
-    processed_paths: list[Path],
+    all_files: list[Path],
+    processed_files: list[tuple[Path, Optional[Path]]],
     exception: BaseException,
 ) -> None:
     """
     Handles an interruption of the processing.
-    Writes the processed and unprocessed files into two files,
+    Writes the pickle file,
+    and the txt files with the processed and unprocessed files,
     and exits the program with exit code 1.
 
     Args:
-        all_paths: list of all paths that should be processed
-        processed_paths: list of all paths that were processed successfully
+        all_files: list of all paths that should be processed
+        processed_files: list of tuples (orig path, processed path). 2nd path is None if a file could not be processed.
         exception: the exception that was raised
     """
-    unprocessed_paths = [x for x in all_paths if x not in processed_paths]
-    with open("unprocessed_files.txt", "w", encoding="utf-8") as f:
-        f.write("\n".join([str(x) for x in unprocessed_paths]))
-    with open("processed_files.txt", "w", encoding="utf-8") as f:
-        f.write("\n".join([str(x) for x in processed_paths]))
+    msg = "ERROR while processing the files. Writing pickle file and human-readable txt files..."
+    print(f"{datetime.now()}: {msg}")
+    logger.error(msg, exc_info=exception)
 
-    msg = (
-        "An error occurred while processing the files. "
-        "2 files were written, listing the processed and the unprocessed files:\n"
-        " - 'processed_files.txt'\n - 'unprocessed_files.txt'."
+    _write_processed_and_unprocessed_files_to_txt_files(
+        all_files=all_files,
+        processed_files=processed_files,
     )
-    print(f"{datetime.now()}: ERROR: {msg}. The exception was: {exception}")
-    logger.error(msg, exc_info=exception)
+    _write_result_to_pkl_file(processed_files)
 
     sys.exit(1)
 
 
+def double_check_unprocessed_files(
+    all_files: list[Path],
+    processed_files: list[Path],
+    unprocessed_files: list[Path],
+) -> None:
+    """
+    Checks if the files in 'unprocessed_files.txt' are consistent with the files in 'processed_files.txt'.
+
+    Args:
+        all_files: list of all paths in the <bitstream> tags of the XML file
+        processed_files: the paths from 'processed_files.txt'
+        unprocessed_files: the paths from 'unprocessed_files.txt' (or all_files if there is no such file)
+
+    Raises:
+        UserError: if there is a file 'unprocessed_files.txt', but no file 'processed_files.txt'
+        UserError: if the files 'unprocessed_files.txt' and 'processed_files.txt' are inconsistent
+    """
+    unprocessed_files_txt_exists = sorted(unprocessed_files) != sorted(all_files)
+    if unprocessed_files_txt_exists and not processed_files:
+        raise UserError("There is a file 'unprocessed_files.txt', but no file 'processed_files.txt'")
+
+    if processed_files and sorted(unprocessed_files) == sorted(all_files):
+        raise UserError("There is a file 'processed_files.txt', but no file 'unprocessed_files.txt'")
+
+    if unprocessed_files_txt_exists:
+        # there is a 'unprocessed_files.txt' file. check it for consistency
+        unprocessed_files_from_processed_files = [x for x in all_files if x not in processed_files]
+        if not sorted(unprocessed_files_from_processed_files) == sorted(unprocessed_files):
+            raise UserError("The files 'unprocessed_files.txt' and 'processed_files.txt' are inconsistent")
+
+
+def _determine_next_batch(
+    all_files: list[Path],
+    batch_size: int,
+) -> tuple[list[Path], bool]:
+    """
+    Looks in the input directory for txt files that contain the already processed files and the still unprocessed files.
+    If no such files are found, this run of `dsp-tools process-files` is the first one.
+    In this case, the first batch_size files (or less if there are less) are returned.
+    If such files are found, the already processed files are read from them,
+    and the next batch_size files are returned.
+    If all files have been processed, an empty list is returned.
+
+    Args:
+        all_files: list of all paths in the <bitstream> tags of the XML file
+        batch_size: number of files to process before Python exits
+
+    Raises:
+        UserError: if the files 'unprocessed_files.txt' and 'processed_files.txt' are inconsistent
+
+    Returns:
+        - the next batch of up to batch_size files that should be processed
+          (or empty list if all files have been processed)
+        - a boolean indicating if this is the last batch
+    """
+    # read the already processed files
+    if Path("processed_files.txt").is_file():
+        with open("processed_files.txt", "r", encoding="utf-8") as f:
+            processed_files = [Path(x.strip()) for x in f.readlines()]
+    else:
+        processed_files = []
+
+    # read the still unprocessed files
+    if Path("unprocessed_files.txt").is_file():
+        with open("unprocessed_files.txt", "r", encoding="utf-8") as f:
+            unprocessed_files = [Path(x.strip()) for x in f.readlines()]
+    else:
+        unprocessed_files = all_files
+
+    # consistency check
+    double_check_unprocessed_files(
+        all_files=all_files,
+        processed_files=processed_files,
+        unprocessed_files=unprocessed_files,
+    )
+
+    # determine next batch
+    if len(unprocessed_files) <= batch_size:
+        next_batch = unprocessed_files
+        is_last_batch = True
+    else:
+        next_batch = unprocessed_files[:batch_size]
+        is_last_batch = False
+
+    # print and log
+    msg = (
+        f"Found {len(all_files)} bitstreams in the XML file, {len(unprocessed_files)} of them unprocessed. "
+        f"Process batch of {len(next_batch)} files..."
+    )
+    print(f"{datetime.now()}: {msg}")
+    logger.info(msg)
+
+    return next_batch, is_last_batch
+
+
 def process_files(
     input_dir: str,
     output_dir: str,
     xml_file: str,
     nthreads: Optional[int],
+    batch_size: int,
 ) -> bool:
     """
     Process the files referenced in the given XML file.
     Writes the processed files
     (derivative, .orig file, sidecar file, as well as the preview file for movies)
     to the given output directory.
     Additionally, writes a pickle file containing the mapping between the original files and the processed files,
     e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
 
+    Due to a resource leak, the Python interpreter must be quitted after a while.
+    For this reason, the processing is done in batches, each batch containing batch_size files.
+    After each batch, the Python interpreter exits, and the CLI command must be executed again.
+    It automatically resumes where it left off.
+
     Args:
         input_dir: path to the directory where the files should be read from
         output_dir: path to the directory where the transformed / created files should be written to
         xml_file: path to xml file containing the resources
         nthreads: number of threads to use for processing
+        batch_size: number of files to process before Python exits
 
     Returns:
-        success status
+        True         --> exit code 0: all multimedia files in the XML file were processed
+        False        --> exit code 1: an error occurred while processing the current batch
+        Error raised --> exit code 1: an error occurred while processing the current batch
+        exit with code 2:             Python interpreter exits after each batch
     """
     # check the input parameters
-    param_check_result = _check_params(
+    input_dir_path, output_dir_path, xml_file_path = _check_input_params(
         input_dir=input_dir,
         out_dir=output_dir,
         xml_file=xml_file,
     )
-    if param_check_result:
-        input_dir_path, output_dir_path, xml_file_path = param_check_result
-    else:
-        raise BaseError("Error reading the input parameters. Please check them.")
 
     # startup the SIPI container
     _start_sipi_container_and_mount_volumes(
         input_dir=input_dir_path,
         output_dir=output_dir_path,
     )
 
-    # get the paths of the files referenced in the XML file
-    all_paths = _get_file_paths_from_xml(xml_file_path)
-    print(f"{datetime.now()}: Found {len(all_paths)} bitstreams in the XML file.")
-    logger.info(f"Found {len(all_paths)} bitstreams in the XML file.")
+    # get the files referenced in the XML file
+    all_files = _get_file_paths_from_xml(xml_file_path)
+
+    # find out if there was a previous processing attempt that should be continued
+    files_to_process, is_last_batch = _determine_next_batch(
+        all_files=all_files,
+        batch_size=batch_size,
+    )
 
     # get shell script for processing video files
-    if any(path.suffix == ".mp4" for path in all_paths):
+    if any(path.suffix == ".mp4" for path in files_to_process):
         _get_export_moving_image_frames_script()
 
     # process the files in parallel
     start_time = datetime.now()
     print(f"{start_time}: Start local file processing...")
     logger.info("Start local file processing...")
-    processed_files = []
-    unprocessed_files = all_paths
+    processed_files: list[tuple[Path, Optional[Path]]] = []
+    unprocessed_files = files_to_process
     while unprocessed_files:
         try:
             result, unprocessed_files = _process_files_in_parallel(
-                paths=all_paths,
+                files_to_process=files_to_process,
                 input_dir=input_dir_path,
                 output_dir=output_dir_path,
                 nthreads=nthreads,
             )
             processed_files.extend(result)
         except BaseException as exc:  # pylint: disable=broad-exception-caught
             handle_interruption(
-                all_paths=all_paths,
-                processed_paths=[x[1] for x in processed_files if x and x[1]],
+                all_files=all_files,
+                processed_files=processed_files,
                 exception=exc,
             )
-
-    # check if all files were processed
     end_time = datetime.now()
     print(f"{end_time}: Processing files took: {end_time - start_time}")
-    logger.info(f"{end_time}: Processing files took: {end_time - start_time}")
-    success = _check_if_all_files_were_processed(
-        result=processed_files,
-        all_paths=all_paths,
+    logger.info(f"Processing files took: {end_time - start_time}")
+
+    # write results to files
+    _write_processed_and_unprocessed_files_to_txt_files(
+        all_files=all_files,
+        processed_files=processed_files,
     )
+    _write_result_to_pkl_file(processed_files)
 
-    # write pickle file
-    if not _write_result_to_pkl_file(processed_files):
-        success = False
-        err_msg = f"An error occurred while writing the result to the pickle file. The result was: {processed_files}"
-        print(f"{datetime.now()}: {err_msg}")
-        logger.error(err_msg)
+    # check if all files were processed
+    success, exit_code = _determine_success_status_and_exit_code(
+        files_to_process=files_to_process,
+        processed_files=processed_files,
+        is_last_batch=is_last_batch,
+    )
 
     # remove the SIPI container
-    if success:
+    if exit_code == 0:
         _stop_and_remove_sipi_container()
 
+    # exit with correct exit code: 0 and 1 will automatically happen, but 2 must be done manually
+    if exit_code == 2:
+        sys.exit(2)
+
     return success
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     Returns:
         True if the file could be uploaded, False if an exception occurred.
     """
     try:
         with open(file, "rb") as bitstream:
             try:
                 response_upload = requests.post(
-                    url=f"{regex.sub(r'/$', '', sipi_url)}/upload_without_processing?token={con.get_token()}",
+                    url=f"{regex.sub(r'/$', '', sipi_url)}/upload_without_processing",
+                    headers={"Authorization": f"Bearer {con.get_token()}"},
                     files={"file": bitstream},
                     timeout=8 * 60,
                 )
             except Exception:  # pylint: disable=broad-exception-caught
                 err_msg = f"An exception was raised while calling the /upload_without_processing route for {file}"
                 print(f"{datetime.now()}: ERROR: {err_msg}")
                 logger.error(err_msg, exc_info=True)
@@ -126,15 +127,15 @@
         logger.error(err_msg, exc_info=True)
         return False
 
     if response_upload.json().get("message") == "server.fs.mkdir() failed: File exists":
         # This error can be safely ignored, since the file was uploaded correctly.
         logger.info(f"In spite of 'server.fs.mkdir() failed: File exists', successfully uploaded file {file}")
     elif response_upload.status_code != 200:
-        err_msg = f"An error occurred while uploading the file {file}. The response was {response_upload.json()}"
+        err_msg = f"An error occurred while uploading the file {file}. The response was {vars(response_upload)}"
         print(f"{datetime.now()}: ERROR: {err_msg}")
         logger.error(err_msg)
         return False
     else:
         logger.info(f"Successfully uploaded file {file}")
 
     return True
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.5.0/src/dsp_tools/models/bitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/connection.py` & `dsp_tools-2.5.0/src/dsp_tools/models/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         credentials = {"email": email, "password": password}
         jsondata = json.dumps(credentials)
 
         response = requests.post(
             self._server + "/v2/authentication",
             headers={"Content-Type": "application/json; charset=UTF-8"},
             data=jsondata,
-            timeout=5,
+            timeout=10,
         )
         check_for_api_error(response)
         result = response.json()
         self._token = result["token"]
 
     def get_token(self) -> str:
         """
@@ -101,15 +101,15 @@
         :return: None
         """
 
         if self._token is not None:
             response = requests.delete(
                 self._server + "/v2/authentication",
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=5,
+                timeout=10,
             )
             check_for_api_error(response)
             self._token = None
 
     def __del__(self):
         pass
         # self.logout()
@@ -188,27 +188,27 @@
         :return: Response from server
         """
 
         if path[0] != "/":
             path = "/" + path
         if not self._token:
             if not headers:
-                response = requests.get(self._server + path, timeout=5)
+                response = requests.get(self._server + path, timeout=10)
             else:
-                response = requests.get(self._server + path, headers, timeout=5)
+                response = requests.get(self._server + path, headers, timeout=10)
         else:
             if not headers:
                 response = requests.get(
                     self._server + path,
                     headers={"Authorization": "Bearer " + self._token},
-                    timeout=5,
+                    timeout=10,
                 )
             else:
                 headers["Authorization"] = "Bearer " + self._token
-                response = requests.get(self._server + path, headers, timeout=5)
+                response = requests.get(self._server + path, headers, timeout=10)
 
         check_for_api_error(response)
         json_response = response.json()
         return json_response
 
     def put(self, path: str, jsondata: Optional[str] = None, content_type: str = "application/json"):
         """
@@ -221,22 +221,22 @@
 
         if path[0] != "/":
             path = "/" + path
         if jsondata is None:
             response = requests.put(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=5,
+                timeout=10,
             )
         else:
             response = requests.put(
                 self._server + path,
                 headers={"Content-Type": content_type + "; charset=UTF-8", "Authorization": "Bearer " + self._token},
                 data=jsondata,
-                timeout=5,
+                timeout=10,
             )
         check_for_api_error(response)
         result = response.json()
         return result
 
     def delete(self, path: str, params: Optional[any] = None):
         """
@@ -248,19 +248,19 @@
         if path[0] != "/":
             path = "/" + path
         if params is not None:
             response = requests.delete(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
                 params=params,
-                timeout=5,
+                timeout=10,
             )
 
         else:
             response = requests.delete(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=5,
+                timeout=10,
             )
         check_for_api_error(response)
         result = response.json()
         return result
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.5.0/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/group.py` & `dsp_tools-2.5.0/src/dsp_tools/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/helpers.py` & `dsp_tools-2.5.0/src/dsp_tools/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/langstring.py` & `dsp_tools-2.5.0/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/listnode.py` & `dsp_tools-2.5.0/src/dsp_tools/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/ontology.py` & `dsp_tools-2.5.0/src/dsp_tools/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/permission.py` & `dsp_tools-2.5.0/src/dsp_tools/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/project.py` & `dsp_tools-2.5.0/src/dsp_tools/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.5.0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.5.0/src/dsp_tools/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.5.0/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/resource.py` & `dsp_tools-2.5.0/src/dsp_tools/models/resource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.5.0/src/dsp_tools/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/sipi.py` & `dsp_tools-2.5.0/src/dsp_tools/models/sipi.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             API response
         """
         with open(filepath, "rb") as bitstream_file:
             files = {
                 "file": (os.path.basename(filepath), bitstream_file),
             }
             response = requests.post(
-                self.sipi_server + "/upload?token=" + self.token,
+                self.sipi_server + "/upload",
+                headers={"Authorization": "Bearer " + self.token},
                 files=files,
                 timeout=5 * 60,
             )
         check_for_api_error(response)
         res: dict[Any, Any] = response.json()
         return res
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/user.py` & `dsp_tools-2.5.0/src/dsp_tools/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/value.py` & `dsp_tools-2.5.0/src/dsp_tools/models/value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.5.0/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/data.xsd`

 * *Files 2% similar despite different names*

#### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/data.xsd`

```diff
@@ -1,9 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xs:schema xmlns="https://dasch.swiss/schema" xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="https://dasch.swiss/schema" elementFormDefault="qualified">
+  <!-- nonEmptyString-->
+  <xs:simpleType name="nonEmptyString">
+    <xs:restriction base="xs:string">
+      <xs:minLength value="1"/>
+      <xs:pattern value=".*\S+.*"/>
+    </xs:restriction>
+  </xs:simpleType>
   <!-- data type for resrefs "ID|ID|..." -->
   <xs:simpleType name="resrefs_type">
     <xs:restriction base="xs:token">
       <xs:pattern value="([^|]+)(\|[^|]+)*"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- group type for allow..." -->
@@ -94,24 +101,24 @@
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- geoname value type -->
   <xs:complexType name="geoname_type">
     <xs:simpleContent>
-      <xs:extension base="xs:string">
+      <xs:extension base="nonEmptyString">
         <xs:attribute name="comment" type="xs:string"/>
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- list value type -->
   <xs:complexType name="list_type">
     <xs:simpleContent>
-      <xs:extension base="xs:string">
+      <xs:extension base="nonEmptyString">
         <xs:attribute name="comment" type="xs:string"/>
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- integer value type -->
   <xs:complexType name="integer_type">
@@ -130,24 +137,24 @@
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- period value type -->
   <xs:complexType name="period_type">
     <xs:simpleContent>
-      <xs:extension base="xs:string">
+      <xs:extension base="nonEmptyString">
         <xs:attribute name="comment" type="xs:string"/>
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- resptr_type (link to other resource) value type -->
   <xs:complexType name="resptr_type">
     <xs:simpleContent>
-      <xs:extension base="xs:string">
+      <xs:extension base="nonEmptyString">
         <xs:attribute name="comment" type="xs:string"/>
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- time value type -->
   <xs:complexType name="time_type">
@@ -325,15 +332,15 @@
       <xs:element name="color" type="color_type" minOccurs="1" maxOccurs="1"/>
     </xs:sequence>
     <xs:attribute name="name" type="xs:string" use="required" fixed="hasColor"/>
   </xs:complexType>
   <!-- bitstream tag -->
   <xs:complexType name="bitstream_type">
     <xs:simpleContent>
-      <xs:extension base="xs:string">
+      <xs:extension base="nonEmptyString">
         <xs:attribute name="permissions" type="xs:NCName" use="optional"/>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <!-- resource tag -->
   <xs:complexType name="resource_type">
     <xs:sequence>
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.5.0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version: '3.7'
 
 services:
 
   app:
     # on the verge of every deployment (fortnightly), update the "image" value from the "app" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/dsp-app:v10.22.0
+    image: daschswiss/dsp-app:v10.23.0
     ports:
       - "4200:4200"
     networks:
       - knora-net
 
   db:
     # on the verge of every deployment (fortnightly), update the "image" value from the "db" value of
@@ -24,15 +24,15 @@
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
     # on the verge of every deployment (fortnightly), take the same tag as DSP-API
-    image: daschswiss/knora-sipi:29.1.0
+    image: daschswiss/knora-sipi:29.1.1
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -45,15 +45,15 @@
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
     # on the verge of every deployment (fortnightly), update the "image" value from the "api" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/knora-api:29.1.0
+    image: daschswiss/knora-api:29.1.1
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/id_to_iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/logging.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import logging
 import logging.handlers
 from pathlib import Path
 
 
-def get_logger(name: str) -> logging.Logger:
+def get_logger(
+    name: str,
+    level: int = logging.INFO,
+    filesize_mb: int = 5,
+    backupcount: int = 4,
+) -> logging.Logger:
     """
     Create a logger instance,
     set its level to INFO,
     and configure it to write to a file in the user's home directory.
 
     Args:
         name: name of the logger
+        level: logging level, defaults to logging.INFO
+        filesize_mb: maximum size per log file in MB, defaults to 5
+        backupcount: number of log files to keep, defaults to 4
 
     Returns:
         the logger instance
     """
     _logger = logging.getLogger(name)
-    _logger.setLevel(logging.INFO)
+    _logger.setLevel(level)
     formatter = logging.Formatter(fmt="{asctime} {filename: <20} {levelname: <8} {message}", style="{")
     # a RotatingFileHandler fills "filename" until it is "maxBytes" big,
     # then appends ".1" to it and starts with a new file "filename",
     # fills it until it is "maxBytes" big,
     # then appends ".1" to it (replacing the old ".1" file)
     logfile_directory = Path.home() / Path(".dsp-tools")
     logfile_directory.mkdir(exist_ok=True)
     handler = logging.handlers.RotatingFileHandler(
         filename=logfile_directory / "logging.log",
         mode="a",
-        maxBytes=5 * 1024 * 1024,
-        backupCount=4,
+        maxBytes=filesize_mb * 1024 * 1024,
+        backupCount=backupcount,
     )
     handler.setFormatter(formatter)
     _logger.addHandler(handler)
     return _logger
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/project_get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/shared.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/stack_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,24 +78,25 @@
             URL prefix used to retrieve files from the DSP-API repository
         """
         url_prefix_base = "https://github.com/dasch-swiss/dsp-api/raw"
 
         if self.__stack_configuration.latest_dev_version:
             return f"{url_prefix_base}/main/"
 
-        config_file = Path("src/dsp_tools/resources/start-stack/start-stack-config.yml")
+        config_file = importlib.resources.files("dsp_tools").joinpath("resources/start-stack/start-stack-config.yml")
         if not config_file.is_file():
             return f"{url_prefix_base}/main/"
 
-        with open("src/dsp_tools/resources/start-stack/start-stack-config.yml", "r", encoding="utf-8") as f:
+        with config_file.open("r", encoding="utf-8") as f:
             try:
                 start_stack_config = yaml.safe_load(f)
             except yaml.YAMLError:
                 start_stack_config = {}
         commit_of_used_api_version = start_stack_config.get("DSP-API commit", "main")
+
         return f"{url_prefix_base}/{commit_of_used_api_version}/"
 
     def _copy_resources_to_home_dir(self) -> None:
         """
         On most systems, Docker is not allowed to access files outside of the user's home directory.
         For this reason, copy the contents of the distribution (src/dsp_tools/resources/start-stack)
         to the user's home directory (~/.dsp-tools/start-stack).
@@ -116,15 +117,15 @@
         """
         Retrieve the config file sipi.docker-config.lua from the DSP-API repository,
         and set the max_file_size parameter if necessary.
 
         Raises:
             UserError: if max_file_size is set but cannot be injected into sipi.docker-config.lua
         """
-        docker_config_lua_text = requests.get(f"{self.__url_prefix}sipi/config/sipi.docker-config.lua", timeout=5).text
+        docker_config_lua_text = requests.get(f"{self.__url_prefix}sipi/config/sipi.docker-config.lua", timeout=10).text
         if self.__stack_configuration.max_file_size:
             max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
             if not re.search(max_post_size_regex, docker_config_lua_text):
                 raise UserError("Unable to set max_file_size. Please try again without this flag.")
             docker_config_lua_text = re.sub(
                 max_post_size_regex,
                 f"max_post_size = '{self.__stack_configuration.max_file_size}M'",
@@ -144,25 +145,25 @@
             "docker compose up db -d",
             shell=True,
             cwd=self.__docker_path_of_user,
             check=False,
         )
         if not completed_process or completed_process.returncode != 0:
             msg = "Cannot start the API: Error while executing 'docker compose up db -d'"
-            logger.error(f"{msg}. completed_process = '{completed_process}'")
+            logger.error(f"{msg}. completed_process = '{vars(completed_process)}'")
             raise UserError(msg)
 
     def _wait_for_fuseki(self) -> None:
         """
         Wait up to 6 minutes, until the fuseki database is up and running.
         This function imitates the behaviour of the script dsp-api/webapi/scripts/wait-for-db.sh.
         """
         for _ in range(6 * 60):
             try:
-                response = requests.get(url="http://0.0.0.0:3030/$/server", auth=("admin", "test"), timeout=5)
+                response = requests.get(url="http://0.0.0.0:3030/$/server", auth=("admin", "test"), timeout=10)
                 if response.ok:
                     break
             except Exception:  # pylint: disable=broad-exception-caught
                 time.sleep(1)
             time.sleep(1)
 
     def _create_knora_test_repo(self) -> None:
@@ -171,29 +172,29 @@
         This function imitates the behaviour of the script dsp-api/webapi/scripts/fuseki-init-knora-test.sh.
 
         Raises:
             UserError: in case of failure
         """
         repo_template = requests.get(
             f"{self.__url_prefix}webapi/scripts/fuseki-repository-config.ttl.template",
-            timeout=5,
+            timeout=10,
         ).text
         repo_template = repo_template.replace("@REPOSITORY@", "knora-test")
         response = requests.post(
             url="http://0.0.0.0:3030/$/datasets",
             files={"file": ("file.ttl", repo_template, "text/turtle; charset=utf8")},
             auth=("admin", "test"),
-            timeout=5,
+            timeout=10,
         )
         if not response.ok:
             msg = (
                 "Cannot start DSP-API: Error when creating the 'knora-test' repository. "
                 "Is DSP-API perhaps running already?"
             )
-            logger.error(f"{msg}. response = {response}")
+            logger.error(f"{msg}. response = {vars(response)}")
             raise UserError(msg)
 
     def _load_data_into_repo(self) -> None:
         """
         Load some basic ontologies and data into the repository.
         This function imitates the behaviour of the script
         dsp-api/webapi/target/docker/stage/opt/docker/scripts/fuseki-init-knora-test.sh.
@@ -204,29 +205,34 @@
         graph_prefix = "http://0.0.0.0:3030/knora-test/data?graph="
         ttl_files = [
             ("knora-ontologies/knora-admin.ttl", "http://www.knora.org/ontology/knora-admin"),
             ("knora-ontologies/knora-base.ttl", "http://www.knora.org/ontology/knora-base"),
             ("knora-ontologies/standoff-onto.ttl", "http://www.knora.org/ontology/standoff"),
             ("knora-ontologies/standoff-data.ttl", "http://www.knora.org/data/standoff"),
             ("knora-ontologies/salsah-gui.ttl", "http://www.knora.org/ontology/salsah-gui"),
-            ("test_data/all_data/admin-data.ttl", "http://www.knora.org/data/admin"),
-            ("test_data/all_data/permissions-data.ttl", "http://www.knora.org/data/permissions"),
-            ("test_data/ontologies/anything-onto.ttl", "http://www.knora.org/ontology/0001/anything"),
-            ("test_data/all_data/anything-data.ttl", "http://www.knora.org/data/0001/anything"),
+            ("test_data/project_data/admin-data.ttl", "http://www.knora.org/data/admin"),
+            ("test_data/project_data/permissions-data.ttl", "http://www.knora.org/data/permissions"),
+            ("test_data/project_ontologies/anything-onto.ttl", "http://www.knora.org/ontology/0001/anything"),
+            ("test_data/project_data/anything-data.ttl", "http://www.knora.org/data/0001/anything"),
         ]
         for ttl_file, graph in ttl_files:
-            ttl_text = requests.get(self.__url_prefix + ttl_file, timeout=5).text
+            ttl_text_response = requests.get(self.__url_prefix + ttl_file, timeout=10)
+            if not ttl_text_response.ok:
+                msg = f"Cannot start DSP-API: Error when retrieving '{self.__url_prefix + ttl_file}'"
+                logger.error(f"{msg}'. response = {vars(ttl_text_response)}")
+                raise UserError(msg)
+            ttl_text = ttl_text_response.text
             response = requests.post(
                 url=graph_prefix + graph,
                 files={"file": ("file.ttl", ttl_text, "text/turtle; charset: utf-8")},
                 auth=("admin", "test"),
-                timeout=5,
+                timeout=10,
             )
             if not response.ok:
-                logger.error(f"Cannot start DSP-API: Error when creating graph '{graph}'. response = {response}")
+                logger.error(f"Cannot start DSP-API: Error when creating graph '{graph}'. response = {vars(response)}")
                 raise UserError(f"Cannot start DSP-API: Error when creating graph '{graph}'")
 
     def _initialize_fuseki(self) -> None:
         """
         Create the "knora-test" repository and load some basic ontologies and data into it.
         """
         self._create_knora_test_repo()
```

### Comparing `dsp_tools-2.4.0/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.5.0/src/dsp_tools/utils/xml_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,37 @@
                 logger.error(err_msg)
                 raise UserError(err_msg)
 
     print("Resource types and properties are consistent with the ontology.")
     logger.info("Resource types and properties are consistent with the ontology.")
 
 
+def _check_if_bitstreams_exist(
+    root: etree._Element,
+    imgdir: str,
+) -> None:
+    """
+    Make sure that all bitstreams referenced in the XML file exist in the imgdir.
+
+    Args:
+        root: parsed XML file
+        imgdir: folder where the bitstreams are stored
+
+    Raises:
+        UserError: if a bitstream does not exist in the imgdir
+    """
+    multimedia_resources = [x for x in root if any((y.tag == "bitstream" for y in x.iter()))]
+    for res in multimedia_resources:
+        pth = [Path(x.text) for x in res.iter() if x.tag == "bitstream" and x.text][0]
+        if not Path(imgdir / pth).is_file():
+            raise UserError(
+                f"Bitstream '{pth!s}' of resource '{res.attrib['label']}' does not exist in the imgdir '{imgdir}'."
+            )
+
+
 def xml_upload(
     input_file: Union[str, Path, etree._ElementTree[Any]],
     server: str,
     user: str,
     password: str,
     imgdir: str,
     sipi: str,
@@ -492,14 +515,16 @@
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
     # parse the XML file
     validate_xml_against_schema(input_file=input_file)
     root = _parse_xml_file(input_file=input_file)
+    if not preprocessing_done:
+        _check_if_bitstreams_exist(root=root, imgdir=imgdir)
     shortcode = root.attrib["shortcode"]
     default_ontology = root.attrib["default-ontology"]
     logger.info(f"Validated and parsed the XML file. Shortcode='{shortcode}' and default_ontology='{default_ontology}'")
 
     # determine save location that will be used for diagnostic info if the xmlupload is interrupted
     save_location, server_as_foldername, timestamp_str = _determine_save_location_of_diagnostic_info(
         server=server,
```

### Comparing `dsp_tools-2.4.0/PKG-INFO` & `dsp_tools-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.4.0
+Version: 2.5.0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

