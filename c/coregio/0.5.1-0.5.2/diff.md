# Comparing `tmp/coregio-0.5.1.tar.gz` & `tmp/coregio-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coregio-0.5.1.tar", last modified: Thu Jul 13 08:32:32 2023, max compression
+gzip compressed data, was "coregio-0.5.2.tar", last modified: Fri Jul 28 10:38:01 2023, max compression
```

## Comparing `coregio-0.5.1.tar` & `coregio-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-13 08:32:24.000000 coregio-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-13 08:32:32.416153 coregio-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-13 08:32:24.000000 coregio-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.412153 coregio-0.5.1/coregio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/coregio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-13 08:32:24.000000 coregio-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:32:32.416153 coregio-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:01.593000 coregio-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-28 10:37:51.000000 coregio-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-28 10:38:01.593000 coregio-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-28 10:37:51.000000 coregio-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:01.589000 coregio-0.5.2/coregio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:37:51.000000 coregio-0.5.2/coregio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-28 10:37:51.000000 coregio-0.5.2/coregio/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-28 10:37:51.000000 coregio-0.5.2/coregio/registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 10:37:51.000000 coregio-0.5.2/coregio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:01.593000 coregio-0.5.2/coregio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-28 10:38:01.000000 coregio-0.5.2/coregio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-28 10:38:01.000000 coregio-0.5.2/coregio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:38:01.000000 coregio-0.5.2/coregio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 10:38:01.000000 coregio-0.5.2/coregio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 10:38:01.000000 coregio-0.5.2/coregio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-28 10:37:51.000000 coregio-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:38:01.593000 coregio-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:01.593000 coregio-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-28 10:37:51.000000 coregio-0.5.2/tests/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-28 10:37:51.000000 coregio-0.5.2/tests/test_registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-28 10:37:51.000000 coregio-0.5.2/tests/test_utils.py
```

### Comparing `coregio-0.5.1/LICENSE.txt` & `coregio-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coregio-0.5.1/PKG-INFO` & `coregio-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coregio
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python container registry API library.
 Author-email: Ales Raszka <araszka@redhat.com>
 License: Copyright (c) 2023 Ales Raszka
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `coregio-0.5.1/README.md` & `coregio-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `coregio-0.5.1/coregio/registry_api.py` & `coregio-0.5.2/coregio/registry_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Container registry API implementation."""
 import json
 import logging
-import re
 from typing import Any, Dict, List, Optional, Callable
 from urllib.parse import urljoin, urlparse
 
 import requests
 
 from coregio import utils
 from coregio.registry_auth import HTTPBearerAuth, HTTPOAuth2, HTTPBasicAuthWithB64
@@ -28,14 +27,15 @@
 # it is stored in index.docker.io
 # From the observation this is something specific only to docker.io
 # and it needs to be handled specifically using lookup table
 SPECIAL_DOCKER_ALIASES = {
     "docker.io": "index.docker.io",
     "registry-1.docker.io": "index.docker.io",
     "hub.docker.com": "index.docker.io",
+    "registry.hub.docker.com": "index.docker.io",
 }
 
 
 class ContainerRegistry:
     """
     Class which calls container registry API
     """
@@ -55,23 +55,48 @@
     ) -> None:
         """
         Args:
         url (str): URL of the registry to auth to
         docker_cfg (Optional, str): DockerConfigJson string
         """
 
-        self.url = SPECIAL_DOCKER_ALIASES.get(url, url)
+        self.url = self._normalize_registry_url(url)
         self._original_url = url
         self.docker_cfg = docker_cfg
 
         self.session = session or requests.Session()
         self.proxy = proxy
 
         self.auth_header = None
 
+    @staticmethod
+    def _normalize_registry_url(url: str) -> str:
+        """
+        Normalize registry URL:
+        - If needed, the hostname is replaced according
+          to the SPECIAL_DOCKER_ALIASES mapping.
+        - Scheme is added if missing.
+        - Port number is preserved if present.
+        - Path is discarded if present.
+
+        Args:
+            url: Registry URL
+
+        Returns:
+            str: Normalized registry URL
+        """
+        url_with_scheme = utils.add_scheme_if_missing(url)
+        parsed = urlparse(url_with_scheme)
+        hostname = SPECIAL_DOCKER_ALIASES.get(parsed.hostname, parsed.hostname)
+
+        normalized_url = f"{parsed.scheme}://{hostname}"
+        if parsed.port:
+            normalized_url = f"{normalized_url}:{parsed.port}"
+        return normalized_url
+
     def _get_auth_token(self) -> Any:
         """
         Extract registry auth token from docker_config_json.
 
         Returns:
             Any: Registry auth token (base64 encoded) if available
         """
@@ -116,16 +141,15 @@
             # to more complex
 
             # First let's try simple URL comparison
             if self._cmp_registry_key(registry_key):
                 return auth
 
             # Add a schema to the URL if missing
-            if not re.search(r"^[A-Za-z0-9+.\-]+://", registry_key):
-                registry_key = f"https://{registry_key}"
+            registry_key = utils.add_scheme_if_missing(registry_key)
 
             # Parse URL and compare matching hostname
             parsed_key = urlparse(registry_key)
             hostname = parsed_key.hostname
             if not hostname:
                 continue
             if self._cmp_registry_key(hostname):
@@ -235,15 +259,15 @@
             params: Params to pass to Registry API endpoint
             headers: Headers to pass to Registry API endpoint
 
         Returns:
             Response: The resulting Response object
         """
 
-        full_url = urljoin(f"https://{self.url}", path)
+        full_url = urljoin(self.url, path)
 
         LOGGER.debug("Querying registry: GET %s %s %s", full_url, headers, params)
         resp = self._get(full_url, params=params, headers=headers)
         utils.handle_response(resp)
         resp.raise_for_status()
 
         LOGGER.debug(
```

### Comparing `coregio-0.5.1/coregio/registry_auth.py` & `coregio-0.5.2/coregio/registry_auth.py`

 * *Files identical despite different names*

### Comparing `coregio-0.5.1/coregio/utils.py` & `coregio-0.5.2/coregio/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Utilities for http queries
 """
 import logging
+import re
 from typing import Any
 
 from requests import Session
 from requests.adapters import HTTPAdapter, Retry
 
 LOGGER = logging.getLogger(__name__)
 
@@ -72,7 +73,22 @@
         # This allows for more graceful exception handling using
         # Response.raise_for_status.
         raise_on_status=False,
     )
     adapter = HTTPAdapter(max_retries=retries)
     session.mount("http://", adapter)
     session.mount("https://", adapter)
+
+
+def add_scheme_if_missing(url: str) -> str:
+    """
+    Add https:// to the url if it does not contain a scheme.
+
+    Args:
+        url: Url to check
+
+    Returns:
+        str: Url containing a scheme
+    """
+    if not re.search(r"^[A-Za-z0-9+.\-]+://", url):
+        return f"https://{url}"
+    return url
```

### Comparing `coregio-0.5.1/coregio.egg-info/PKG-INFO` & `coregio-0.5.2/coregio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coregio
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python container registry API library.
 Author-email: Ales Raszka <araszka@redhat.com>
 License: Copyright (c) 2023 Ales Raszka
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `coregio-0.5.1/pyproject.toml` & `coregio-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "coregio"
-version = "0.5.1"
+version = "0.5.2"
 description = "Python container registry API library."
 authors = [{ name = "Ales Raszka", email = "araszka@redhat.com" }]
 dependencies = ["requests>=2.31.0"]
 requires-python = ">=3.8"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
```

### Comparing `coregio-0.5.1/tests/test_registry_api.py` & `coregio-0.5.2/tests/test_registry_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,41 @@
 import pytest
 import requests
 
 from coregio.registry_api import ContainerRegistry
 
 
 @pytest.mark.parametrize(
+    ["url", "expected_url"],
+    [
+        ("quay.io", "https://quay.io"),
+        ("http://quay.io", "http://quay.io"),
+        ("quay.io:8080", "https://quay.io:8080"),
+        ("quay.io/path", "https://quay.io"),
+        ("http://quay.io:8080/path", "http://quay.io:8080"),
+        ("registry-1.docker.io", "https://index.docker.io"),
+        ("hub.docker.com", "https://index.docker.io"),
+        ("registry.hub.docker.com", "https://index.docker.io"),
+        ("docker.io", "https://index.docker.io"),
+        ("http://docker.io", "http://index.docker.io"),
+        ("docker.io:8080", "https://index.docker.io:8080"),
+        ("docker.io/path", "https://index.docker.io"),
+        ("http://docker.io:8080/path", "http://index.docker.io:8080"),
+    ],
+)
+def test__normalize_registry_url(
+    url: str,
+    expected_url: str,
+) -> None:
+    result_url = ContainerRegistry._normalize_registry_url(url)
+
+    assert result_url == expected_url
+
+
+@pytest.mark.parametrize(
     ["registry", "cfg", "auth", "token"],
     [
         ("quay.io", None, None, None),
         ("quay.io", "qwe", None, None),
         ("quay.io", "{}", None, None),
         ("quay.io", "{}", {"auth": "Zm9vOmJhcg=="}, "Zm9vOmJhcg=="),
         ("quay.io", "{}", {"auth": "Zm9vOmJhcg==", "identitytoken": "abc"}, "abc"),
```

### Comparing `coregio-0.5.1/tests/test_registry_auth.py` & `coregio-0.5.2/tests/test_registry_auth.py`

 * *Files identical despite different names*

