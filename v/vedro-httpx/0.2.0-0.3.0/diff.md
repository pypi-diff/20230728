# Comparing `tmp/vedro-httpx-0.2.0.tar.gz` & `tmp/vedro-httpx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.2.0.tar", last modified: Wed Jun 14 15:18:29 2023, max compression
+gzip compressed data, was "vedro-httpx-0.3.0.tar", last modified: Fri Jul 28 16:46:53 2023, max compression
```

## Comparing `vedro-httpx-0.2.0.tar` & `vedro-httpx-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/_vedro_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:18.000000 vedro-httpx-0.2.0/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:18:29.150343 vedro-httpx-0.2.0/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 15:18:29.000000 vedro-httpx-0.2.0/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.755904 vedro-httpx-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_print_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.755904 vedro-httpx-0.3.0/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.2.0/LICENSE` & `vedro-httpx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/PKG-INFO` & `vedro-httpx-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
```

### Comparing `vedro-httpx-0.2.0/README.md` & `vedro-httpx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/setup.cfg` & `vedro-httpx-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-httpx-0.2.0/setup.py` & `vedro-httpx-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.2.0",
+    version="0.3.0",
     description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
```

### Comparing `vedro-httpx-0.2.0/tests/test_async_interface.py` & `vedro-httpx-0.3.0/tests/test_async_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/tests/test_format_response.py` & `vedro-httpx-0.3.0/tests/test_format_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/tests/test_response.py` & `vedro-httpx-0.3.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/tests/test_sync_interface.py` & `vedro-httpx-0.3.0/tests/test_sync_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/vedro_httpx/_async_http_interface.py` & `vedro-httpx-0.3.0/vedro_httpx/_async_http_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/vedro_httpx/_render_response.py` & `vedro-httpx-0.3.0/vedro_httpx/_render_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 import os
-from typing import Any, Tuple, Union
+from typing import Any, Optional, Tuple, Union
 
 from httpx import Response
 from pygments.lexer import Lexer
 from pygments.lexers import HttpLexer, JsonLexer, TextLexer, get_lexer_for_mimetype
 from pygments.util import ClassNotFound
 from rich.console import RenderResult
 from rich.syntax import Syntax
 
 __all__ = ("render_response",)
 
 
 def render_response(response: Response, *,
-                    theme: str = "ansi_dark", code_width: int = 1024 ** 2) -> RenderResult:
+                    theme: str = "ansi_dark", width: Optional[int] = None) -> RenderResult:
     yield "Response:"
     headers, http_lexer = format_response_headers(response)
-    yield Syntax(headers, http_lexer, theme=theme, code_width=code_width)
+    yield Syntax(headers, http_lexer, theme=theme, word_wrap=True, code_width=width)
 
     body, lexer = format_response_body(response)
-    yield Syntax(body, lexer, theme=theme, indent_guides=True, code_width=code_width)
+    yield Syntax(body, lexer,
+                 theme=theme, word_wrap=True, indent_guides=True, code_width=width)
 
 
 def format_response_headers(response: Response) -> Tuple[str, Lexer]:
     lines = [f"{response.http_version} {response.status_code} {response.reason_phrase}"]
     for header in response.headers:
         values = response.headers.get_list(header)
         for value in values:
```

### Comparing `vedro-httpx-0.2.0/vedro_httpx/_sync_http_interface.py` & `vedro-httpx-0.3.0/vedro_httpx/_sync_http_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.2.0/vedro_httpx.egg-info/PKG-INFO` & `vedro-httpx-0.3.0/vedro_httpx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.2.0
+Version: 0.3.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
```

### Comparing `vedro-httpx-0.2.0/vedro_httpx.egg-info/SOURCES.txt` & `vedro-httpx-0.3.0/vedro_httpx.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 tests/test_async_interface.py
 tests/test_format_response.py
+tests/test_print_response.py
 tests/test_response.py
 tests/test_sync_interface.py
 vedro_httpx/__init__.py
 vedro_httpx/_async_http_interface.py
 vedro_httpx/_render_response.py
 vedro_httpx/_response.py
 vedro_httpx/_sync_http_interface.py
```

