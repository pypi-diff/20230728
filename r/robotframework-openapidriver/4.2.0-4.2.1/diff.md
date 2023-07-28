# Comparing `tmp/robotframework_openapidriver-4.2.0.tar.gz` & `tmp/robotframework_openapidriver-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapidriver-4.2.0.tar", max compression
+gzip compressed data, was "robotframework_openapidriver-4.2.1.tar", max compression
```

## Comparing `robotframework_openapidriver-4.2.0.tar` & `robotframework_openapidriver-4.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4817 2023-07-28 14:31:11.193987 robotframework_openapidriver-4.2.0/docs/README.md
--rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.2.0/LICENSE
--rw-r--r--   0        0        0     3016 2023-07-28 13:14:36.379283 robotframework_openapidriver-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1331 2023-06-22 13:31:43.975787 robotframework_openapidriver-4.2.0/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32436 2023-07-28 14:31:02.490239 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_executors.py
--rw-r--r--   0        0        0     4573 2023-05-22 14:48:18.048301 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    27530 2023-07-28 14:31:11.116590 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    15519 2023-06-12 08:10:53.573048 robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.py
--rw-r--r--   0        0        0        0 2023-06-12 08:10:53.574048 robotframework_openapidriver-4.2.0/src/OpenApiDriver/py.typed
--rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4817 2023-07-28 15:48:25.807793 robotframework_openapidriver-4.2.1/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.2.1/LICENSE
+-rw-r--r--   0        0        0     3016 2023-07-28 15:45:07.830628 robotframework_openapidriver-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1331 2023-06-22 13:31:43.975787 robotframework_openapidriver-4.2.1/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32386 2023-07-28 14:31:36.899531 robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapi_executors.py
+-rw-r--r--   0        0        0     4573 2023-05-22 14:48:18.048301 robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    27530 2023-07-28 15:48:25.711495 robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15519 2023-06-12 08:10:53.573048 robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapidriver.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:10:53.574048 robotframework_openapidriver-4.2.1/src/OpenApiDriver/py.typed
+-rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.2.1/PKG-INFO
```

### Comparing `robotframework_openapidriver-4.2.0/docs/README.md` & `robotframework_openapidriver-4.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.2.0/LICENSE` & `robotframework_openapidriver-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.2.0/pyproject.toml` & `robotframework_openapidriver-4.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapidriver"
-version = "4.2.0"
+version = "4.2.1"
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
-robotframework-openapi-libcore = "^1.10.0"
+robotframework-openapi-libcore = "^1.10.1"
 
 [tool.poetry.group.dev.dependencies]
 fastapi = ">=0.95.0"
 uvicorn = ">=0.22.0"
 invoke = ">=2.0.0"
 coverage = {version=">=7.2.5", extras = ["toml"]}
 robotframework-stacktrace = ">=0.4.1"
```

### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/__init__.py` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapi_executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from random import choice
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
-from openapi_core.exceptions import OpenAPIError
 from openapi_core.templating.paths.exceptions import ServerNotFound
 from OpenApiLibCore import OpenApiLibCore, RequestData, RequestValues, resolve_schema
 from requests import Response
 from requests.auth import AuthBase
 from requests.cookies import RequestsCookieJar as CookieJar
 from robot.api import SkipExecution
 from robot.api.deco import keyword, library
```

### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapidriver.libspec`

 * *Files 1% similar despite different names*

#### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-07-28T14:31:11+00:00" specversion="5" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="351">
-  <version>4.2.0</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-07-28T15:48:26+00:00" specversion="5" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="351">
+  <version>4.2.1</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="143">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
@@ -282,15 +282,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="154">
+    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="153">
       <arguments repr="path: str, method: str, status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -302,15 +302,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
       <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
-    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="112">
+    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="111">
       <arguments repr="path: str, method: str, expected_status_code: int = 404">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -324,15 +324,15 @@
       </arguments>
       <doc>&lt;p&gt;Perform a request for the provided 'path' and 'method' where the url for the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; is invalidated.&lt;/p&gt;
 &lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the path contains no parts that can be invalidated.&lt;/p&gt;
 &lt;p&gt;The optional &lt;span class=&quot;name&quot;&gt;expected_status_code&lt;/span&gt; parameter (default: 404) can be set to the expected status code for APIs that do not return a 404 on invalid urls.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: Depending on API design, the url may be validated before or after validation of headers, query parameters and / or (json) body. By default, no parameters are send with the request. The &lt;span class=&quot;name&quot;&gt;require_body_for_invalid_url&lt;/span&gt; parameter can be set to &lt;span class=&quot;name&quot;&gt;True&lt;/span&gt; if needed.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for the provided 'path' and 'method' where the url for the `path` is invalidated.</shortdoc>
     </kw>
-    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="92">
+    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="91">
       <arguments repr="path: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapidriver-4.2.0/src/OpenApiDriver/openapidriver.py` & `robotframework_openapidriver-4.2.1/src/OpenApiDriver/openapidriver.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.2.0/PKG-INFO` & `robotframework_openapidriver-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapidriver
-Version: 4.2.0
+Version: 4.2.1
 Summary: A library for contract-testing OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapidriver
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Dist: robotframework-datadriver (>=1.6.1)
-Requires-Dist: robotframework-openapi-libcore (>=1.10.0,<2.0.0)
+Requires-Dist: robotframework-openapi-libcore (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 ---
 ---
 
 # OpenApiDriver for Robot Framework®
```

