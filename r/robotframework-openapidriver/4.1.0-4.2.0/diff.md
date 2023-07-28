# Comparing `tmp/robotframework_openapidriver-4.1.0.tar.gz` & `tmp/robotframework_openapidriver-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapidriver-4.1.0.tar", max compression
+gzip compressed data, was "robotframework_openapidriver-4.2.0.tar", max compression
```

## Comparing `robotframework_openapidriver-4.1.0.tar` & `robotframework_openapidriver-4.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     4817 2023-06-12 08:01:12.404483 robotframework_openapidriver-4.1.0/docs/README.md
--rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.1.0/LICENSE
--rw-r--r--   0        0        0     2966 2023-06-09 13:44:41.052342 robotframework_openapidriver-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     1103 2022-01-11 08:27:46.400406 robotframework_openapidriver-4.1.0/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32993 2023-06-12 07:31:09.890507 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_executors.py
--rw-r--r--   0        0        0     4573 2023-05-22 14:48:18.048301 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    25265 2023-06-12 08:01:12.327460 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    15519 2023-06-12 08:01:08.206636 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.py
--rw-r--r--   0        0        0        0 2023-06-12 07:27:05.636214 robotframework_openapidriver-4.1.0/src/OpenApiDriver/py.typed
--rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.1.0/setup.py
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4817 2023-07-28 14:31:11.193987 robotframework_openapidriver-4.2.0/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.2.0/LICENSE
+-rw-r--r--   0        0        0     3016 2023-07-28 13:14:36.379283 robotframework_openapidriver-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1331 2023-06-22 13:31:43.975787 robotframework_openapidriver-4.2.0/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32436 2023-07-28 14:31:02.490239 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_executors.py
+-rw-r--r--   0        0        0     4573 2023-05-22 14:48:18.048301 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    27530 2023-07-28 14:31:11.116590 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15519 2023-06-12 08:10:53.573048 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:10:53.574048 robotframework_openapidriver-4.2.0/src/OpenApiDriver/py.typed
+-rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.2.0/PKG-INFO
```

### Comparing `robotframework_openapidriver-4.1.0/docs/README.md` & `robotframework_openapidriver-4.2.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.1.0/LICENSE` & `robotframework_openapidriver-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.1.0/pyproject.toml` & `robotframework_openapidriver-4.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapidriver"
-version = "4.1.0"
+version = "4.2.0"
 description = "A library for contract-testing OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapidriver"
 classifiers = [
@@ -20,15 +20,15 @@
     { include = "OpenApiDriver", from = "src" },
 ]
 include = ["*.libspec"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 robotframework-datadriver = ">=1.6.1"
-robotframework-openapi-libcore = "^1.9.0"
+robotframework-openapi-libcore = "^1.10.0"
 
 [tool.poetry.group.dev.dependencies]
 fastapi = ">=0.95.0"
 uvicorn = ">=0.22.0"
 invoke = ">=2.0.0"
 coverage = {version=">=7.2.5", extras = ["toml"]}
 robotframework-stacktrace = ">=0.4.1"
@@ -111,15 +111,16 @@
 [tool.robotidy]
 line_length = 120
 spacecount = 4
 
 [tool.robocop]
 filetypes = [".robot", ".resource"]
 configure = [
-    "line-too-long:line_length:120"
+    "line-too-long:line_length:120",
+    "too-many-calls-in-test-case:max_calls:15"
 ]
 exclude = [
     "missing-doc-suite",
     "missing-doc-test-case",
     "missing-doc-keyword",
     "too-few-calls-in-test-case"
 ]
```

### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/__init__.py` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,7 +23,19 @@
 
 from OpenApiDriver.openapidriver import OpenApiDriver
 
 try:
     __version__ = version("robotframework-openapidriver")
 except Exception:  # pragma: no cover
     pass
+
+__all__ = [
+    "Dto",
+    "IdDependency",
+    "IdReference",
+    "PathPropertiesConstraint",
+    "PropertyValueConstraint",
+    "Relation",
+    "UniquePropertyValueConstraint",
+    "IGNORE",
+    "OpenApiDriver",
+]
```

### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Module containing the classes to perform automatic OpenAPI contract validation."""
 
 import json as _json
-from dataclasses import asdict
 from enum import Enum
 from logging import getLogger
 from pathlib import Path
 from random import choice
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
+from openapi_core.exceptions import OpenAPIError
 from openapi_core.templating.paths.exceptions import ServerNotFound
-from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
 from OpenApiLibCore import OpenApiLibCore, RequestData, RequestValues, resolve_schema
 from requests import Response
 from requests.auth import AuthBase
 from requests.cookies import RequestsCookieJar as CookieJar
 from robot.api import SkipExecution
 from robot.api.deco import keyword, library
 from robot.libraries.BuiltIn import BuiltIn
@@ -138,15 +137,15 @@
 
         params, headers, json_data = None, None, None
         if self.require_body_for_invalid_url:
             request_data = self.get_request_data(method=method, endpoint=path)
             params = request_data.params
             headers = request_data.headers
             dto = request_data.dto
-            json_data = asdict(dto)
+            json_data = dto.as_dict()
         response: Response = run_keyword(
             "authorized_request", url, method, params, headers, json_data
         )
         if response.status_code != expected_status_code:
             raise AssertionError(
                 f"Response {response.status_code} was not {expected_status_code}"
             )
@@ -166,15 +165,15 @@
         json_data: Optional[Dict[str, Any]] = None
         original_data = None
 
         url: str = run_keyword("get_valid_url", path, method)
         request_data: RequestData = self.get_request_data(method=method, endpoint=path)
         params = request_data.params
         headers = request_data.headers
-        json_data = asdict(request_data.dto)
+        json_data = request_data.dto.as_dict()
         # when patching, get the original data to check only patched data has changed
         if method == "PATCH":
             original_data = self.get_original_data(url=url)
         # in case of a status code indicating an error, ensure the error occurs
         if status_code >= 400:
             invalidation_keyword_data = {
                 "get_invalid_json_data": [
@@ -483,32 +482,23 @@
         )
         if self.disable_server_validation:
             validation_result.errors = [
                 e for e in validation_result.errors if not isinstance(e, ServerNotFound)
             ]
 
         # The OAS concepts of optional / nullable are not compatible with Python.
-        # Filter the schema errors caused by this incompatibility.
+        # Filter the errors caused by this incompatibility.
         errors_to_keep = []
         for error in validation_result.errors:
-            if isinstance(error, InvalidSchemaValue):
-                schema_errors_to_keep = []
-                for schema_error in error.schema_errors:
-                    message = str(schema_error)
-                    if message == "None for not nullable" or message.startswith(
-                        "None is not "
-                    ):
-                        logger.debug("'None for not nullable' ValidationError ignored.")
-                    else:
-                        schema_errors_to_keep.append(schema_error)
-                if schema_errors_to_keep:
-                    error.schema_errors = tuple(schema_errors_to_keep)
-                    errors_to_keep.append(error)
+            message = str(error)
+            if message == "None for not nullable" or message.startswith("None is not "):
+                logger.debug("'None for not nullable' OpenAPIError ignored.")
             else:
                 errors_to_keep.append(error)
+
         validation_result.errors = errors_to_keep
 
         if self.response_validation == ValidationLevel.STRICT:
             validation_result.raise_for_errors()
         if self.response_validation in [ValidationLevel.WARN, ValidationLevel.INFO]:
             for validation_error in validation_result.errors:
                 if self.response_validation == ValidationLevel.WARN:
```

### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec`

 * *Files 16% similar despite different names*

#### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,153 +1,225 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-12T08:01:12+00:00" specversion="4" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="351">
-  <version>4.1.0</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-07-28T14:31:11+00:00" specversion="5" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="351">
+  <version>4.2.0</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="143">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="base_path: str = ">
           <name>base_path</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="included_paths: Iterable[str] | None = None">
           <name>included_paths</name>
-          <type>Iterable[str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Iterable[str] | None
+            <type name="Iterable">
+              Iterable[str]
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_paths: Iterable[str] | None = None">
           <name>ignored_paths</name>
-          <type>Iterable[str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Iterable[str] | None
+            <type name="Iterable">
+              Iterable[str]
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_responses: Iterable[int] | None = None">
           <name>ignored_responses</name>
-          <type>Iterable[int]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Iterable[int] | None
+            <type name="Iterable">
+              Iterable[int]
+              <type name="int" typedoc="integer">int</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_testcases: Iterable[Tuple[str, str, int]] | None = None">
           <name>ignored_testcases</name>
-          <type>Iterable[Tuple[str, str, int]]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Iterable[Tuple[str, str, int]] | None
+            <type name="Iterable">
+              Iterable[Tuple[str, str, int]]
+              <type name="Tuple" typedoc="tuple">
+                Tuple[str, str, int]
+                <type name="str" typedoc="string">str</type>
+                <type name="str" typedoc="string">str</type>
+                <type name="int" typedoc="integer">int</type>
+              </type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="response_validation: ValidationLevel = WARN">
           <name>response_validation</name>
-          <type typedoc="ValidationLevel">ValidationLevel</type>
+          <type name="ValidationLevel" typedoc="ValidationLevel">ValidationLevel</type>
           <default>WARN</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="disable_server_validation: bool = True">
           <name>disable_server_validation</name>
-          <type typedoc="boolean">bool</type>
+          <type name="bool" typedoc="boolean">bool</type>
           <default>True</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="mappings_path: str | Path = ">
           <name>mappings_path</name>
-          <type typedoc="string">str</type>
-          <type typedoc="Path">Path</type>
+          <type name="Union" union="true">
+            str | Path
+            <type name="str" typedoc="string">str</type>
+            <type name="Path" typedoc="Path">Path</type>
+          </type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="invalid_property_default_response: int = 422">
           <name>invalid_property_default_response</name>
-          <type typedoc="integer">int</type>
+          <type name="int" typedoc="integer">int</type>
           <default>422</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="default_id_property_name: str = id">
           <name>default_id_property_name</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default>id</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="faker_locale: str | List[str] | None = None">
           <name>faker_locale</name>
-          <type typedoc="string">str</type>
-          <type typedoc="list">List[str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            str | List[str] | None
+            <type name="str" typedoc="string">str</type>
+            <type name="List" typedoc="list">
+              List[str]
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="require_body_for_invalid_url: bool = False">
           <name>require_body_for_invalid_url</name>
-          <type typedoc="boolean">bool</type>
+          <type name="bool" typedoc="boolean">bool</type>
           <default>False</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_limit: int = 1">
           <name>recursion_limit</name>
-          <type typedoc="integer">int</type>
+          <type name="int" typedoc="integer">int</type>
           <default>1</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_default: Any = {}">
           <name>recursion_default</name>
-          <type>Any</type>
+          <type name="Any" typedoc="Any">Any</type>
           <default>{}</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="username: str = ">
           <name>username</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="password: str = ">
           <name>password</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="security_token: str = ">
           <name>security_token</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="auth: AuthBase | None = None">
           <name>auth</name>
-          <type>AuthBase</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            AuthBase | None
+            <type name="AuthBase">AuthBase</type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cert: str | Tuple[str, str] | None = None">
           <name>cert</name>
-          <type typedoc="string">str</type>
-          <type typedoc="tuple">Tuple[str, str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            str | Tuple[str, str] | None
+            <type name="str" typedoc="string">str</type>
+            <type name="Tuple" typedoc="tuple">
+              Tuple[str, str]
+              <type name="str" typedoc="string">str</type>
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="verify_tls: bool | str | None = True">
           <name>verify_tls</name>
-          <type typedoc="boolean">bool</type>
-          <type typedoc="string">str</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            bool | str | None
+            <type name="bool" typedoc="boolean">bool</type>
+            <type name="str" typedoc="string">str</type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>True</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="extra_headers: Dict[str, str] | None = None">
           <name>extra_headers</name>
-          <type typedoc="dictionary">Dict[str, str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Dict[str, str] | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, str]
+              <type name="str" typedoc="string">str</type>
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cookies: Dict[str, str] | RequestsCookieJar | None = None">
           <name>cookies</name>
-          <type typedoc="dictionary">Dict[str, str]</type>
-          <type typedoc="dictionary">RequestsCookieJar</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Dict[str, str] | RequestsCookieJar | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, str]
+              <type name="str" typedoc="string">str</type>
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="RequestsCookieJar" typedoc="dictionary">RequestsCookieJar</type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="proxies: Dict[str, str] | None = None">
           <name>proxies</name>
-          <type typedoc="dictionary">Dict[str, str]</type>
-          <type typedoc="None">None</type>
+          <type name="Union" union="true">
+            Dict[str, str] | None
+            <type name="Dict" typedoc="dictionary">
+              Dict[str, str]
+              <type name="str" typedoc="string">str</type>
+              <type name="str" typedoc="string">str</type>
+            </type>
+            <type name="None" typedoc="None">None</type>
+          </type>
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;h3&gt;Base parameters&lt;/h3&gt;
 &lt;h4&gt;source&lt;/h4&gt;
 &lt;p&gt;An absolute path to an openapi.json or openapi.yaml file or an url to such a file.&lt;/p&gt;
 &lt;h4&gt;origin&lt;/h4&gt;
@@ -210,65 +282,65 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="155">
+    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="154">
       <arguments repr="path: str, method: str, status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
-          <type typedoc="integer">int</type>
+          <type name="int" typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
       <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
-    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="113">
+    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="112">
       <arguments repr="path: str, method: str, expected_status_code: int = 404">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="expected_status_code: int = 404">
           <name>expected_status_code</name>
-          <type typedoc="integer">int</type>
+          <type name="int" typedoc="integer">int</type>
           <default>404</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request for the provided 'path' and 'method' where the url for the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; is invalidated.&lt;/p&gt;
 &lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the path contains no parts that can be invalidated.&lt;/p&gt;
 &lt;p&gt;The optional &lt;span class=&quot;name&quot;&gt;expected_status_code&lt;/span&gt; parameter (default: 404) can be set to the expected status code for APIs that do not return a 404 on invalid urls.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: Depending on API design, the url may be validated before or after validation of headers, query parameters and / or (json) body. By default, no parameters are send with the request. The &lt;span class=&quot;name&quot;&gt;require_body_for_invalid_url&lt;/span&gt; parameter can be set to &lt;span class=&quot;name&quot;&gt;True&lt;/span&gt; if needed.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for the provided 'path' and 'method' where the url for the `path` is invalidated.</shortdoc>
     </kw>
-    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="93">
+    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="92">
       <arguments repr="path: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
-          <type typedoc="string">str</type>
+          <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request for &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; on the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt;, with no authorization.&lt;/p&gt;
 &lt;p&gt;This keyword only passes if the response code is 401: Unauthorized.&lt;/p&gt;
 &lt;p&gt;Any authorization parameters used to initialize the library are ignored for this request. &amp;gt; Note: No headers or (json) body are send with the request. For security reasons, the authorization validation should be checked first.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for `method` on the `path`, with no authorization.</shortdoc>
     </kw>
@@ -283,14 +355,23 @@
           <member name="WARN" value="WARN"/>
           <member name="STRICT" value="STRICT"/>
         </members>
       </enum>
     </enums>
   </datatypes>
   <typedocs>
+    <type name="Any" type="Standard">
+      <doc>&lt;p&gt;Any value is accepted. No conversion is done.&lt;/p&gt;</doc>
+      <accepts>
+        <type>Any</type>
+      </accepts>
+      <usages>
+        <usage>__init__</usage>
+      </usages>
+    </type>
     <type name="boolean" type="Standard">
       <doc>&lt;p&gt;Strings &lt;code&gt;TRUE&lt;/code&gt;, &lt;code&gt;YES&lt;/code&gt;, &lt;code&gt;ON&lt;/code&gt; and &lt;code&gt;1&lt;/code&gt; are converted to Boolean &lt;code&gt;True&lt;/code&gt;, the empty string as well as strings &lt;code&gt;FALSE&lt;/code&gt;, &lt;code&gt;NO&lt;/code&gt;, &lt;code&gt;OFF&lt;/code&gt; and &lt;code&gt;0&lt;/code&gt; are converted to Boolean &lt;code&gt;False&lt;/code&gt;, and the string &lt;code&gt;NONE&lt;/code&gt; is converted to the Python &lt;code&gt;None&lt;/code&gt; object. Other strings and other accepted values are passed as-is, allowing keywords to handle them specially if needed. All string comparisons are case-insensitive.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;TRUE&lt;/code&gt; (converted to &lt;code&gt;True&lt;/code&gt;), &lt;code&gt;off&lt;/code&gt; (converted to &lt;code&gt;False&lt;/code&gt;), &lt;code&gt;example&lt;/code&gt; (used as-is)&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
         <type>integer</type>
         <type>float</type>
```

### Comparing `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.py` & `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.1.0/setup.py` & `robotframework_openapidriver-4.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,150 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: robotframework-openapidriver
+Version: 4.2.0
+Summary: A library for contract-testing OpenAPI / Swagger APIs.
+Home-page: https://github.com/MarketSquare/robotframework-openapidriver
+License: Apache-2.0
+Author: Robin Mackaij
+Author-email: r.a.mackaij@gmail.com
+Maintainer: Robin Mackaij
+Maintainer-email: r.a.mackaij@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Framework :: Robot Framework
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Requires-Dist: robotframework-datadriver (>=1.6.1)
+Requires-Dist: robotframework-openapi-libcore (>=1.10.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+---
+---
+
+# OpenApiDriver for Robot Framework®
+
+OpenApiDriver is an extension of the Robot Framework® DataDriver library that allows
+for generation and execution of test cases based on the information in an OpenAPI
+document (also known as Swagger document).
+This document explains how to use the OpenApiDriver library.
+
+For more information about Robot Framework®, see http://robotframework.org.
+
+For more information about the DataDriver library, see
+https://github.com/Snooz82/robotframework-datadriver.
+
+---
+
+> Note: OpenApiDriver is still under development so there are currently
+restrictions / limitations that you may encounter when using this library to run
+tests against an API. See [Limitations](#limitations) for details.
+
+---
+
+## Installation
+
+If you already have Python >= 3.8 with pip installed, you can simply run:
+
+`pip install --upgrade robotframework-openapidriver`
+
+---
+
+## OpenAPI (aka Swagger)
+
+The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
+to RESTful APIs, see https://swagger.io/specification/
+
+The OpenApiDriver module implements a reader class that generates a test case for
+each path, method and response (i.e. every response for each endpoint) that is defined
+in an OpenAPI document, typically an openapi.json or openapi.yaml file.
+
+> Note: OpenApiDriver is designed for APIs based on the OAS v3
+The library has not been tested for APIs based on the OAS v2.
+
+---
+
+## Getting started
+
+Before trying to use OpenApiDriver to run automatic validations on the target API
+it's recommended to first ensure that the openapi document for the API is valid
+under the OpenAPI Specification.
+
+This can be done using the command line interface of a package that is installed as
+a prerequisite for OpenApiDriver.
+Both a local openapi.json or openapi.yaml file or one hosted by the API server
+can be checked using the `prance validate <reference_to_file>` shell command:
+
+```shell
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
+Processing "http://localhost:8000/openapi.json"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
+Processing "/tests/files/petstore_openapi.yaml"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+```
+
+You'll have to change the url or file reference to the location of the openapi
+document for your API.
+
+> Note: Although recursion is technically allowed under the OAS, tool support is limited
+and changing the OAS to not use recursion is recommended.
+OpenApiDriver has limited support for parsing OpenAPI documents with
+recursion in them. See the `recursion_limit` and `recursion_default` parameters.
+
+If the openapi document passes this validation, the next step is trying to do a test
+run with a minimal test suite.
+The example below can be used, with `source` and `origin` altered to fit your situation.
+
+``` robotframework
+*** Settings ***
+Library            OpenApiDriver
+...                    source=http://localhost:8000/openapi.json
+...                    origin=http://localhost:8000
+Test Template      Validate Using Test Endpoint Keyword
+
+*** Test Cases ***
+Test Endpoint for ${method} on ${path} where ${status_code} is expected
+
+*** Keywords ***
+Validate Using Test Endpoint Keyword
+    [Arguments]    ${path}    ${method}    ${status_code}
+    Test Endpoint
+    ...    path=${path}    method=${method}    status_code=${status_code}
+
+```
+
+Running the above suite for the first time is likely to result in some
+errors / failed tests.
+You should look at the Robot Framework `log.html` to determine the reasons
+for the failing tests.
+Depending on the reasons for the failures, different solutions are possible.
+
+Details about the OpenApiDriver library parameters that you may need can be found
+[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).
+
+The OpenApiDriver also support handling of relations between resources within the scope
+of the API being validated as well as handling dependencies on resources outside the
+scope of the API. In addition there is support for handling restrictions on the values
+of parameters and properties.
+
+Details about the `mappings_path` variable usage can be found
+[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).
+
+---
+
+## Limitations
+
+There are currently a number of limitations to supported API structures, supported
+data types and properties. The following list details the most important ones:
+- Only JSON request and response bodies are supported.
+- No support for per-path authorization levels (only simple 401 / 403 validation).
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['OpenApiDriver']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['robotframework-datadriver>=1.6.1',
- 'robotframework-openapi-libcore>=1.9.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'robotframework-openapidriver',
-    'version': '4.1.0',
-    'description': 'A library for contract-testing OpenAPI / Swagger APIs.',
-    'long_description': '---\n---\n\n# OpenApiDriver for Robot Framework®\n\nOpenApiDriver is an extension of the Robot Framework® DataDriver library that allows\nfor generation and execution of test cases based on the information in an OpenAPI\ndocument (also known as Swagger document).\nThis document explains how to use the OpenApiDriver library.\n\nFor more information about Robot Framework®, see http://robotframework.org.\n\nFor more information about the DataDriver library, see\nhttps://github.com/Snooz82/robotframework-datadriver.\n\n---\n\n> Note: OpenApiDriver is still under development so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapidriver`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiDriver module implements a reader class that generates a test case for\neach path, method and response (i.e. every response for each endpoint) that is defined\nin an OpenAPI document, typically an openapi.json or openapi.yaml file.\n\n> Note: OpenApiDriver is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use OpenApiDriver to run automatic validations on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiDriver.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the OAS to not use recursion is recommended.\nOpenApiDriver has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source` and `origin` altered to fit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiDriver\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\nTest Template      Validate Using Test Endpoint Keyword\n\n*** Test Cases ***\nTest Endpoint for ${method} on ${path} where ${status_code} is expected\n\n*** Keywords ***\nValidate Using Test Endpoint Keyword\n    [Arguments]    ${path}    ${method}    ${status_code}\n    Test Endpoint\n    ...    path=${path}    method=${method}    status_code=${status_code}\n\n```\n\nRunning the above suite for the first time is likely to result in some\nerrors / failed tests.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiDriver library parameters that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).\n\nThe OpenApiDriver also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-path authorization levels (only simple 401 / 403 validation).\n\n',
-    'author': 'Robin Mackaij',
-    'author_email': 'r.a.mackaij@gmail.com',
-    'maintainer': 'Robin Mackaij',
-    'maintainer_email': 'r.a.mackaij@gmail.com',
-    'url': 'https://github.com/MarketSquare/robotframework-openapidriver',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

