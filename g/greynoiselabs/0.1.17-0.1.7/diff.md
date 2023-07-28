# Comparing `tmp/greynoiselabs-0.1.17.tar.gz` & `tmp/greynoiselabs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greynoiselabs-0.1.17.tar", max compression
+gzip compressed data, was "greynoiselabs-0.1.7.tar", last modified: Thu Jul 27 18:38:35 2023, max compression
```

## Comparing `greynoiselabs-0.1.17.tar` & `greynoiselabs-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,41 @@
--rw-r--r--   0        0        0     1079 2023-06-16 04:21:17.985676 greynoiselabs-0.1.17/LICENSE
--rw-r--r--   0        0        0     1278 2023-07-28 18:46:54.890247 greynoiselabs-0.1.17/README.rst
--rw-r--r--   0        0        0     2335 2023-07-28 18:46:40.821357 greynoiselabs-0.1.17/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 04:05:43.447421 greynoiselabs-0.1.17/src/greynoiselabs/__init__.py
--rw-r--r--   0        0        0     1611 2023-07-28 17:52:53.932529 greynoiselabs-0.1.17/src/greynoiselabs/api/__init__.py
--rw-r--r--   0        0        0     7371 2023-07-28 17:52:53.933179 greynoiselabs-0.1.17/src/greynoiselabs/api/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-07-28 17:52:53.933784 greynoiselabs-0.1.17/src/greynoiselabs/api/base_model.py
--rw-r--r--   0        0        0     4296 2023-07-28 17:52:53.934349 greynoiselabs-0.1.17/src/greynoiselabs/api/client.py
--rw-r--r--   0        0        0       84 2023-07-28 17:52:53.934583 greynoiselabs-0.1.17/src/greynoiselabs/api/enums.py
--rw-r--r--   0        0        0     2366 2023-07-28 17:52:53.934939 greynoiselabs-0.1.17/src/greynoiselabs/api/exceptions.py
--rw-r--r--   0        0        0      461 2023-07-28 17:52:53.935238 greynoiselabs-0.1.17/src/greynoiselabs/api/generate_g_n_q_l.py
--rw-r--r--   0        0        0      593 2023-07-28 17:52:53.935602 greynoiselabs-0.1.17/src/greynoiselabs/api/get_c2s.py
--rw-r--r--   0        0        0      698 2023-07-28 17:52:53.935786 greynoiselabs-0.1.17/src/greynoiselabs/api/get_i_ps.py
--rw-r--r--   0        0        0      775 2023-07-28 17:52:53.935960 greynoiselabs-0.1.17/src/greynoiselabs/api/get_knocks.py
--rw-r--r--   0        0        0      689 2023-07-28 17:52:53.936152 greynoiselabs-0.1.17/src/greynoiselabs/api/get_noise_ranks.py
--rw-r--r--   0        0        0      755 2023-07-28 17:52:53.936344 greynoiselabs-0.1.17/src/greynoiselabs/api/get_requests.py
--rw-r--r--   0        0        0      221 2023-07-28 17:52:53.936513 greynoiselabs-0.1.17/src/greynoiselabs/api/input_types.py
--rw-r--r--   0        0        0      942 2023-07-27 01:19:27.930060 greynoiselabs-0.1.17/src/greynoiselabs/api/noise_rank.py
--rw-r--r--   0        0        0      220 2023-07-28 17:52:53.936697 greynoiselabs-0.1.17/src/greynoiselabs/api/scalars.py
--rw-r--r--   0        0        0     1138 2023-07-27 01:19:27.930299 greynoiselabs-0.1.17/src/greynoiselabs/api/top_h_t_t_p_requests.py
--rw-r--r--   0        0        0     1060 2023-07-27 01:19:27.930417 greynoiselabs-0.1.17/src/greynoiselabs/api/top_knocks.py
--rw-r--r--   0        0        0      993 2023-07-27 01:19:27.930530 greynoiselabs-0.1.17/src/greynoiselabs/api/top_popular_i_ps.py
--rw-r--r--   0        0        0        0 2023-07-27 03:55:22.108240 greynoiselabs-0.1.17/src/greynoiselabs/cli/__init__.py
--rwxr-xr-x   0        0        0     5840 2023-07-28 18:10:03.439937 greynoiselabs-0.1.17/src/greynoiselabs/cli/auth.py
--rw-r--r--   0        0        0     7371 2023-07-28 17:52:53.937221 greynoiselabs-0.1.17/src/greynoiselabs/cli/main.py
--rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 greynoiselabs-0.1.17/PKG-INFO
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736639 greynoiselabs-0.1.7/
+-rw-r--r--   0 matt       (502) staff       (20)     1079 2023-06-16 04:21:17.000000 greynoiselabs-0.1.7/LICENSE
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.736729 greynoiselabs-0.1.7/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)      960 2023-07-27 16:38:11.000000 greynoiselabs-0.1.7/README.rst
+-rw-r--r--   0 matt       (502) staff       (20)      281 2023-07-27 18:38:35.737016 greynoiselabs-0.1.7/setup.cfg
+-rw-r--r--   0 matt       (502) staff       (20)     1698 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/setup.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.729256 greynoiselabs-0.1.7/src/
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.730993 greynoiselabs-0.1.7/src/greynoiselabs/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 04:05:43.000000 greynoiselabs-0.1.7/src/greynoiselabs/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)      254 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/__version__.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736050 greynoiselabs-0.1.7/src/greynoiselabs/api/
+-rw-r--r--   0 matt       (502) staff       (20)     1611 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py
+-rw-r--r--   0 matt       (502) staff       (20)     7371 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py
+-rw-r--r--   0 matt       (502) staff       (20)     1951 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py
+-rw-r--r--   0 matt       (502) staff       (20)     4181 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/client.py
+-rw-r--r--   0 matt       (502) staff       (20)       84 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/enums.py
+-rw-r--r--   0 matt       (502) staff       (20)     2366 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py
+-rw-r--r--   0 matt       (502) staff       (20)      461 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/generate_g_n_q_l.py
+-rw-r--r--   0 matt       (502) staff       (20)      593 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py
+-rw-r--r--   0 matt       (502) staff       (20)      614 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_i_ps.py
+-rw-r--r--   0 matt       (502) staff       (20)      775 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      689 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py
+-rw-r--r--   0 matt       (502) staff       (20)      755 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)      221 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/input_types.py
+-rw-r--r--   0 matt       (502) staff       (20)      942 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/noise_rank.py
+-rw-r--r--   0 matt       (502) staff       (20)      220 2023-07-27 18:12:11.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/scalars.py
+-rw-r--r--   0 matt       (502) staff       (20)     1138 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_h_t_t_p_requests.py
+-rw-r--r--   0 matt       (502) staff       (20)     1060 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_knocks.py
+-rw-r--r--   0 matt       (502) staff       (20)      993 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/api/top_popular_i_ps.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.736481 greynoiselabs-0.1.7/src/greynoiselabs/cli/
+-rw-r--r--   0 matt       (502) staff       (20)        0 2023-07-27 03:55:22.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/__init__.py
+-rwxr-xr-x   0 matt       (502) staff       (20)     5763 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py
+-rw-r--r--   0 matt       (502) staff       (20)     4985 2023-07-27 01:19:27.000000 greynoiselabs-0.1.7/src/greynoiselabs/cli/main.py
+drwxr-xr-x   0 matt       (502) staff       (20)        0 2023-07-27 18:38:35.732309 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/
+-rw-r--r--   0 matt       (502) staff       (20)     2005 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (502) staff       (20)     1148 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (502) staff       (20)       61 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/entry_points.txt
+-rw-r--r--   0 matt       (502) staff       (20)        1 2023-07-27 03:56:32.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (502) staff       (20)      246 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/requires.txt
+-rw-r--r--   0 matt       (502) staff       (20)       14 2023-07-27 18:38:35.000000 greynoiselabs-0.1.7/src/greynoiselabs.egg-info/top_level.txt
```

### Comparing `greynoiselabs-0.1.17/LICENSE` & `greynoiselabs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/__init__.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from .async_base_client import AsyncBaseClient
 from .base_model import BaseModel
 from .client import Client
 from .exceptions import (
     GraphQLClientError,
     GraphQLClientGraphQLError,
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/async_base_client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/base_model.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/client.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from .async_base_client import AsyncBaseClient
 from .generate_g_n_q_l import GenerateGNQL
 from .get_c2s import GetC2s
 from .get_i_ps import GetIPs
 from .get_knocks import GetKnocks
@@ -84,26 +84,26 @@
             """
         )
         variables: dict[str, object] = {"ip": ip}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetKnocks.parse_obj(data)
 
-    async def generate_g_n_q_l(self, input_text: str) -> GenerateGNQL:
+    async def generate_g_n_q_l(self, input: str) -> GenerateGNQL:
         query = gql(
             """
-            query generateGNQL($input_text: String!) {
-              generateGNQL(input_text: $input_text) {
+            query generateGNQL($input: String!) {
+              generateGNQL(input: $input) {
                 input_text
                 queries
               }
             }
             """
         )
-        variables: dict[str, object] = {"input_text": input_text}
+        variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GenerateGNQL.parse_obj(data)
 
     async def get_noise_ranks(self, ip: str) -> GetNoiseRanks:
         query = gql(
             """
@@ -132,17 +132,14 @@
             """
             query getIPs {
               topPopularIPs {
                 popularIPs {
                   ip
                   request_count
                   users_count
-                  last_requested
-                  noise
-                  last_seen
                 }
               }
             }
             """
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/exceptions.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/get_c2s.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_c2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/get_i_ps.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_popular_i_ps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-06-16 04:37
 # Source: queries
 
-from typing import Any, List, Optional
+from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
 
 
-class GetIPs(BaseModel):
-    top_popular_i_ps: "GetIPsTopPopularIPs" = Field(alias="topPopularIPs")
+class TopPopularIPs(BaseModel):
+    top_popular_i_ps: "TopPopularIPsTopPopularIPs" = Field(alias="topPopularIPs")
 
 
-class GetIPsTopPopularIPs(BaseModel):
-    popular_i_ps: List["GetIPsTopPopularIPsPopularIPs"] = Field(alias="popularIPs")
+class TopPopularIPsTopPopularIPs(BaseModel):
+    query_info: "TopPopularIPsTopPopularIPsQueryInfo" = Field(alias="queryInfo")
+    popular_i_ps: List["TopPopularIPsTopPopularIPsPopularIPs"] = Field(
+        alias="popularIPs"
+    )
 
 
-class GetIPsTopPopularIPsPopularIPs(BaseModel):
+class TopPopularIPsTopPopularIPsQueryInfo(BaseModel):
+    results_available: int = Field(alias="resultsAvailable")
+    results_limit: int = Field(alias="resultsLimit")
+
+
+class TopPopularIPsTopPopularIPsPopularIPs(BaseModel):
     ip: str
     request_count: int
     users_count: int
-    last_requested: Any
-    noise: bool
-    last_seen: Optional[Any]
 
 
-GetIPs.update_forward_refs()
-GetIPsTopPopularIPs.update_forward_refs()
-GetIPsTopPopularIPsPopularIPs.update_forward_refs()
+TopPopularIPs.update_forward_refs()
+TopPopularIPsTopPopularIPs.update_forward_refs()
+TopPopularIPsTopPopularIPsQueryInfo.update_forward_refs()
+TopPopularIPsTopPopularIPsPopularIPs.update_forward_refs()
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/get_knocks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_knocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import Any, List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/get_noise_ranks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_noise_ranks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/get_requests.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/get_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-28 13:12
+# Generated by ariadne-codegen on 2023-07-27 18:00
 # Source: queries
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/noise_rank.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/noise_rank.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/top_h_t_t_p_requests.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_h_t_t_p_requests.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/api/top_knocks.py` & `greynoiselabs-0.1.7/src/greynoiselabs/api/top_knocks.py`

 * *Files identical despite different names*

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/cli/auth.py` & `greynoiselabs-0.1.7/src/greynoiselabs/cli/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 #!/usr/bin/env python3
 
+import time
 import json
 import os
-import time
-
-import jwt
-import requests
-import typer
+from requests_oauthlib import OAuth2Session
 from auth0.authentication.token_verifier import (
-    AsymmetricSignatureVerifier,
     TokenVerifier,
+    AsymmetricSignatureVerifier,
 )
-from requests_oauthlib import OAuth2Session
+import jwt
+import requests
+import typer
 
 AUTH0_DOMAIN = "greynoise2.auth0.com"
 AUTH0_CLIENT_ID = "IM8Old6x7WCr2wqVI0Cz3I0c4JPSR1gn"
 TOKEN_URL = f"https://{AUTH0_DOMAIN}/oauth/token"
 JWKS_URL = f"https://{AUTH0_DOMAIN}/.well-known/jwks.json"
 ISSUER_URL = f"https://{AUTH0_DOMAIN}/"
 ALGORITHMS = ["RS256"]
 
 
-def get_token_from_file(token_filename: str):
+def get_token_from_file(token_filename):
     """
     Gets the token from a file
     """
     try:
         fp = os.path.expanduser(token_filename)
         with open(fp, "r") as f:
             token_data = json.load(f)
             return token_data
-    except Exception:
+    except Exception as ex:
+        print(f"Unable to load token from {token_filename}, {ex}")
         return None
 
 
-def token_saver(token_filename: str, token_data: any):
+def token_saver(token_filename, token_data):
     """
     Saves the token to a file
     """
     try:
         fp = os.path.expanduser(token_filename)
         os.makedirs(os.path.dirname(fp), exist_ok=True)
         with open(fp, "w+") as f:
             json.dump(token_data, f)
-        print(f"Token saved to {token_filename}.")
     except Exception as ex:
         print(f"Unable to save token to {token_filename}, {ex}")
         raise typer.Abort()
 
 
-def token_refresh(token_filename: str, token_data_in: any):
+def token_refresh(token_filename, token_data_in):
     """
     Refreshes the token
     """
     extra = {
         "client_id": AUTH0_CLIENT_ID,
     }
     try:
@@ -62,28 +61,29 @@
         token_saver(token_filename, token_data)
         return token_data
     except Exception as ex:
         print(f"Unable to refresh token {ex}.")
         return None
 
 
-def validate_token(id_token: any):
+def validate_token(id_token):
     """
     Verify the token and its precedence
 
     :param id_token:
     """
     sv = AsymmetricSignatureVerifier(JWKS_URL)
     tv = TokenVerifier(
         signature_verifier=sv, issuer=ISSUER_URL, audience=AUTH0_CLIENT_ID
     )
     try:
         tv.verify(id_token)
         return True
-    except Exception:
+    except Exception as ex:
+        print(f"Unable to validate token {ex}.")
         return False
 
 
 def init_device_flow():
     """
     Initiate Oauth 2.0 Device Authorization Flow with Auth0
     """
@@ -126,22 +126,21 @@
             print(token_data["error_description"])
             raise typer.Exit(code=1)
         else:
             time.sleep(device_code_data["interval"])
     return token_data, current_user
 
 
-def authenticate(config_dir: str):
+def authenticate(token_filename):
     """
     Checks for local token and validates it, if invalid, attempts to refresh it.
     """
     global token_data
     global current_user
     validated = False
-    token_filename = os.path.join(config_dir, "token.json")
 
     token_data = get_token_from_file(token_filename)
     if token_data:
         validated = validate_token(token_data["id_token"])
         if validated:
             current_user = jwt.decode(
                 token_data["id_token"],
@@ -161,24 +160,22 @@
                     options={"verify_signature": False},
                 )
                 return token_data, current_user
     else:
         return None, None
 
 
-def login(config_dir: str):
+def login(token_filename):
     """
     Runs the device authorization flow and stores the user object in memory
     """
 
     global token_data
     global current_user
     validated = False
-    token_filename = os.path.join(config_dir, "token.json")
-
     token_data, current_user = init_device_flow()
     token_saver(token_filename, token_data)
     validated = validate_token(token_data["id_token"])
     if validated:
         current_user = jwt.decode(
             token_data["id_token"],
             algorithms=ALGORITHMS,
```

### Comparing `greynoiselabs-0.1.17/src/greynoiselabs/cli/main.py` & `greynoiselabs-0.1.7/src/greynoiselabs/cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,263 +1,172 @@
 #!/usr/bin/env python3
 
 import asyncio
-import importlib.metadata
 import json
+import jsonlines
 import os
 
-import httpx
-import jsonlines
+from greynoiselabs.__version__ import __version__
+from greynoiselabs.api.client import Client
+from greynoiselabs.cli.auth import login, authenticate
 import typer
-from platformdirs import PlatformDirs
 from typing_extensions import Annotated
 
-from greynoiselabs.api.client import Client
-from greynoiselabs.cli.auth import authenticate, login
-
 AUTH0_DOMAIN = os.getenv("AUTH0_DOMAIN", default="greynoise2.auth0.com")
 AUTH0_CLIENT_ID = os.getenv(
     "AUTH0_CLIENT_ID", default="IM8Old6x7WCr2wqVI0Cz3I0c4JPSR1gn"
 )
 ALGORITHMS = ["RS256"]
+DEFAULT_TOKEN_FILE = "~/.greynoiselabs/token.json"
+
+app = typer.Typer(no_args_is_help=True)
 
 current_user = None
 token_data = None
 client = None
 
 
-def get_version():
-    try:
-        version = importlib.metadata.version("greynoiselabs")
-    except importlib.metadata.PackageNotFoundError:
-        version = None
-    return version
-
-
-config_dir = typer.Option(
-    "--config",
-    "-c",
-    help="Output directory for CLI config.",
-    show_default=True,
-    default_factory=PlatformDirs(
-        "greynoiselabs", "greynoise", version=get_version()
-    ).user_config_dir,
-)
-token = typer.Option(
-    "--token", "-t", envvar="GNL_TOKEN", help="HTTP JWT auth bearer token."
-)
-output = typer.Option(
-    "--output",
-    "-o",
-    help="JSON lines output file location.",
-    show_default=False,
-    default_factory=lambda: "",
-)
-ip = typer.Argument(
-    help="Specify the IP to retrieve.", show_default=False, default_factory=lambda: ""
-)
-input: typer.Argument(
-    help="Specify the input text to translate.",
-    show_default=False,
-    default_factory=lambda: "",
-)
-app = typer.Typer(no_args_is_help=True, pretty_exceptions_enable=False)
-
-
-def initOutfile(outfile: str):
+def initOutfile(outfile):
     if outfile != "":
         try:
             writer = jsonlines.open(outfile, mode="w")
             return writer
         except Exception as ex:
             print(f"unable to open {outfile} for writing: {ex}")
             raise typer.Abort()
     else:
         return None
 
 
-def init_conf_dir(config_dir: str):
-    try:
-        dirs = PlatformDirs("greynoiselabs", "greynoise", version=get_version())
-        if config_dir != "":
-            config_dir = os.path.expanduser(config_dir)
-            os.makedirs(config_dir, exist_ok=True)
-        else:
-            config_dir = dirs.user_config_dir
-            os.makedirs(config_dir, exist_ok=True)
-        return config_dir
-    except Exception as ex:
-        print(f"unable to create config directory {config_dir}: {ex}")
-        raise typer.Abort()
-
-
-def out(obj: any, outfile_writer: jsonlines.Writer):
+def out(obj, outfile_writer):
     """
     Output the object as JSON
     """
-    if isinstance(obj, str):
-        try:
-            if outfile_writer:
-                outfile_writer.write(obj)
-            else:
-                print(obj)
-        except Exception as ex:
-            print(f"unable to dump object {ex}")
-            typer.Abort()
-    else:
-        try:
-            if outfile_writer:
-                outfile_writer.write(obj.__dict__)
-            else:
-                print(json.dumps(obj.__dict__))
-        except Exception as ex:
-            print(f"unable to dump object {ex}")
-            typer.Abort()
+    try:
+        if outfile_writer:
+            outfile_writer.write(obj.__dict__)
+        else:
+            print(json.dumps(obj.__dict__))
+    except Exception as ex:
+        print(f"unable to dump object {ex}")
+        typer.Abort()
 
 
-def new_client(id_token: any):
-    transport = httpx.AsyncHTTPTransport(retries=1)
+def new_client(id_token):
     return Client(
-        "https://api.labs.greynoise.io/1/query",
-        {"Authorization": f"Bearer {id_token}"},
-        httpx.AsyncClient(
-            headers={"Authorization": f"Bearer {id_token}"},
-            transport=transport,
-            timeout=90.0,
-        ),
+        "https://api.labs.greynoise.io/1/query", {"Authorization": f"Bearer {id_token}"}
     )
 
 
 @app.command()
 def version():
     """
     Return the version of the GreyNoise Labs CLI.
     """
-    print(get_version())
+    print(__version__)
 
 
 @app.command()
 def init(
-    config_dir: Annotated[str, config_dir],
+    token: Annotated[
+        str, typer.Option(help="Output location of the token file.")
+    ] = DEFAULT_TOKEN_FILE
 ):
     """
     Initialize the client by authenticating with Auth0 and saving the token to a file.
     """
     global current_user, token_data, client
-    init_conf_dir(config_dir)
-    token_data, current_user = authenticate(config_dir)
+    token_data, current_user = authenticate(token)
     if token_data is None or current_user is None:
         run_init = typer.confirm(
             "You are not authenticated, would you like to do this now?"
         )
         if run_init:
-            token_data, current_user = login(config_dir)
-            print("Authentication successful")
+            token_data, current_user = login(token)
+            print("Authentication successful, please re-run your command")
             raise typer.Abort()
         else:
             print("You must authenticate to use this CLI")
             raise typer.Abort()
     if token_data is not None and current_user is not None:
         try:
             client = new_client(token_data["id_token"])
         except Exception as ex:
             print(f"Unable to create client {ex}")
             raise typer.Abort()
     else:
-        print("Authentication failed, please try again or contact labs@greynoise.io.")
+        print("Authentication failed, please try again")
         raise typer.Abort()
 
 
 @app.command()
-def c2s(output: Annotated[str, output], config_dir: Annotated[str, config_dir]):
+def c2s(output: Annotated[str, typer.Option(help="JSON output file location.")] = ""):
     """
     Return the top 1% of C2s ranked by pervasiveness.
     This data may be up to 4.5 hours old but covers the previous 24 hours.
     """
-    init(config_dir)
+    init()
     writer = initOutfile(output)
     response = asyncio.run(client.get_c2s())
     for c2 in response.top_c2s.c2s:
         out(c2, writer)
     if writer:
         writer.close()
 
 
 @app.command()
 def knocks(
-    ip: Annotated[str, ip],
-    output: Annotated[str, output],
-    config_dir: Annotated[str, config_dir],
+    ip: Annotated[str, typer.Argument(help="Specify the IP to retrieve.")] = "",
+    output: Annotated[str, typer.Option(help="JSON output file location.")] = "",
 ):
     """
     Return the top 1% of Knock results by most recently seen.
     A Knock represents an IP observed by GreyNoise that we have scanned back.
     This data may be up to 12 hours old.
     This endpoint supports filtering by a single IP.
     """
-    init(config_dir)
+    init()
     writer = initOutfile(output)
     response = asyncio.run(client.get_knocks(ip))
     for knock in response.top_knocks.knock:
         out(knock, writer)
     if writer:
         writer.close()
 
 
 @app.command()
-def popular_ips(output: Annotated[str, output], config_dir: Annotated[str, config_dir]):
+def popular_ips(
+    output: Annotated[str, typer.Option(help="JSON output file location.")] = ""
+):
     """
     Return the top 1% of IPs searched in GreyNoise.
     These results are ordered by the number of users observed over the last 7 days.
     This data may be up to 24 hours old.
     This also returns the user and request counts.
     This also returns a boolean if this IP was observed by GreyNoise sensors.
     """
-    init(config_dir)
+    init()
     writer = initOutfile(output)
     response = asyncio.run(client.get_i_ps())
     for ip in response.top_popular_i_ps.popular_i_ps:
         out(ip, writer)
     if writer:
         writer.close()
 
 
 @app.command()
 def noise_rank(
-    ip: Annotated[str, ip],
-    output: Annotated[str, output],
-    config_dir: Annotated[str, config_dir],
+    ip: Annotated[str, typer.Argument(help="Specify the IP to retrieve.")] = "",
+    output: Annotated[str, typer.Option(help="JSON output file location.")] = "",
 ):
     """
     Return the top 1% of ranked IPs by noise score over the previous 7 days of traffic.
     This also returns the pervasiveness and diversity scores.
     This endpoint supports filtering by a single IP.
     """
-    init(config_dir)
+    init()
     writer = initOutfile(output)
     response = asyncio.run(client.get_noise_ranks(ip))
     for ip in response.noise_rank.ips:
         out(ip, writer)
     if writer:
         writer.close()
-
-
-@app.command()
-def gengnql(
-    input: Annotated[str, input],
-    output: Annotated[str, output],
-    config_dir: Annotated[str, config_dir],
-):
-    """
-    Translate text into usable GreyNoise GNQL queries.
-    """
-    init(config_dir)
-    writer = initOutfile(output)
-    response = asyncio.run(client.generate_g_n_q_l(input))
-    for query in response.generate_g_n_q_l.queries:
-        out(query, writer)
-    if writer:
-        writer.close()
-
-
-if __name__ == "__main__":
-    app()
```

