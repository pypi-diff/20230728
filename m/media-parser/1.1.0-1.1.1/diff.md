# Comparing `tmp/media_parser-1.1.0.tar.gz` & `tmp/media_parser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-1.1.0.tar", max compression
+gzip compressed data, was "media_parser-1.1.1.tar", max compression
```

## Comparing `media_parser-1.1.0.tar` & `media_parser-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-07-28 12:01:54.716964 media_parser-1.1.0/LICENSE
--rw-r--r--   0        0        0     2477 2023-07-28 12:01:54.716964 media_parser-1.1.0/README.md
--rw-r--r--   0        0        0      273 2023-07-28 12:01:54.716964 media_parser-1.1.0/media_parser/__init__.py
--rw-r--r--   0        0        0     1833 2023-07-28 12:01:54.716964 media_parser-1.1.0/media_parser/client.py
--rw-r--r--   0        0        0       44 2023-07-28 12:01:54.716964 media_parser-1.1.0/media_parser/models/__init__.py
--rw-r--r--   0        0        0     2187 2023-07-28 12:01:54.716964 media_parser-1.1.0/media_parser/models/medias.py
--rw-r--r--   0        0        0     1232 2023-07-28 12:01:54.716964 media_parser-1.1.0/media_parser/models/server.py
--rw-r--r--   0        0        0     2735 2023-07-28 12:01:54.720964 media_parser-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 media_parser-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-28 12:19:33.647356 media_parser-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2994 2023-07-28 12:19:33.647356 media_parser-1.1.1/README.md
+-rw-r--r--   0        0        0      273 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/__init__.py
+-rw-r--r--   0        0        0     1833 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/client.py
+-rw-r--r--   0        0        0       44 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     2187 2023-07-28 12:19:33.651356 media_parser-1.1.1/media_parser/models/medias.py
+-rw-r--r--   0        0        0     1232 2023-07-28 12:19:33.651356 media_parser-1.1.1/media_parser/models/server.py
+-rw-r--r--   0        0        0     2753 2023-07-28 12:19:33.651356 media_parser-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4943 1970-01-01 00:00:00.000000 media_parser-1.1.1/PKG-INFO
```

### Comparing `media_parser-1.1.0/LICENSE` & `media_parser-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.0/README.md` & `media_parser-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,52 +46,72 @@
         volumes:
             - ./data:/data/db
 ```
 
 ### Parsers Configuration
 
 All configs for parsers stored in `config/parsers.json`. JSON Schema for
-this: [schemas/parser_schema.json](schemas/parser_schema.json).
+this: [schemas/parser_schema.json](https://github.com/jag-k/media-parser/blob/main/schemas/parser_schema.json).
 
-For enable parser, you need to add config for this parser.
-If parser haven't config, like `tiktok` set empty object (`{}`) to enable it.
+To enable parser, you need to add config for this parser.
+If parser hasn't config, like `tiktok` set an empty object (`{}`) to enable it.
 
 Example:
 
 ```json5
+// config/parsers.json
 {
     "$schema": "https://raw.github.com/jag-k/media-parsers/blob/main/schemas/parser_schema.json",
     "instagram": {
         // Optional
         "lamadava_saas_token": "asdasd"
     },
     "reddit": {
         "client_id": "",
         "client_secret": "",
         // Optional
         "user_agent": "video downloader (by u/Jag_k)"
     },
     "tiktok": {},
     "twitter": {
-        "twitter_bearer_token": ""
+        "twitter_bearer_token": "asdasd"
     },
     "youtube": {}
 }
 ```
 
+Or you can use YAML file like `config/parsers.yaml` or `config/parsers.yml`:
+
+```yaml
+# config/parsers.yml
+$schema: "https://raw.github.com/jag-k/media-parsers/blob/main/schemas/parser_schema.json"
+instagram:
+    # Optional
+    lamadava_saas_token: "asdasd"
+reddit:
+    client_id: ""
+    client_secret: ""
+    # Optional
+    user_agent: "video downloader (by u/Jag_k)"
+tiktok: {}
+twitter:
+    twitter_bearer_token: "asdasd"
+youtube: {}
+```
+
 ## Usage
 
 API documentation available on `/docs` endpoint.
 
 ## Clients
 
 ### Installation
 
 ```bash
-poetry add git+https://github.com/jag-k/media-parser.git
+poetry add media-parser  # or pip install media-parser
 ```
 
 ### Usage
 
 ```python
 from media_parser import Client, FeedbackTypes
```

### Comparing `media_parser-1.1.0/media_parser/client.py` & `media_parser-1.1.1/media_parser/client.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.0/media_parser/models/medias.py` & `media_parser-1.1.1/media_parser/models/medias.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.0/media_parser/models/server.py` & `media_parser-1.1.1/media_parser/models/server.py`

 * *Files identical despite different names*

### Comparing `media_parser-1.1.0/pyproject.toml` & `media_parser-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "media-parser"
-version = "1.1.0"
+version = "1.1.1"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
@@ -39,14 +39,15 @@
 contextvars = "^2.4"
 pydantic = { version = "^1.10.9", extras = ["dotenv"] }
 jsonref = "^1.1.0"
 pytube = "^15.0.0"
 uvicorn = "^0.23.1"
 motor = "^3.1.2"
 async-lru = "^2.0.2"
+pyyaml = "^6.0.1"
 
 [tool.poetry.extras]
 server = ["uvicorn", "motor", "fastapi", "contextvars", "pytube", "jsonref", "async-lru"]
 sentry = ["sentry-sdk"]
 all = ["uvicorn", "motor", "fastapi", "contextvars", "pytube", "jsonref", "async-lru", "sentry-sdk"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `media_parser-1.1.0/PKG-INFO` & `media_parser-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 1.1.0
+Version: 1.1.1
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
@@ -30,14 +30,15 @@
 Requires-Dist: async-lru (>=2.0.2,<3.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: contextvars (>=2.4,<3.0) ; extra == "server" or extra == "all"
 Requires-Dist: fastapi (>=0.100.0,<0.101.0) ; extra == "server" or extra == "all"
 Requires-Dist: jsonref (>=1.1.0,<2.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: motor (>=3.1.2,<4.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0) ; extra == "server" or extra == "all"
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sentry-sdk[fastapi,httpx,pure-eval,pymongo] (>=1.28.1,<2.0.0) ; extra == "sentry" or extra == "all"
 Requires-Dist: uvicorn (>=0.23.1,<0.24.0) ; extra == "server" or extra == "all"
 Project-URL: Documentation, https://github.com/jag-k/media-parser#clients
 Project-URL: Repository, https://github.com/jag-k/media-parser
 Description-Content-Type: text/markdown
 
 # Media Parser
@@ -88,52 +89,72 @@
         volumes:
             - ./data:/data/db
 ```
 
 ### Parsers Configuration
 
 All configs for parsers stored in `config/parsers.json`. JSON Schema for
-this: [schemas/parser_schema.json](schemas/parser_schema.json).
+this: [schemas/parser_schema.json](https://github.com/jag-k/media-parser/blob/main/schemas/parser_schema.json).
 
-For enable parser, you need to add config for this parser.
-If parser haven't config, like `tiktok` set empty object (`{}`) to enable it.
+To enable parser, you need to add config for this parser.
+If parser hasn't config, like `tiktok` set an empty object (`{}`) to enable it.
 
 Example:
 
 ```json5
+// config/parsers.json
 {
     "$schema": "https://raw.github.com/jag-k/media-parsers/blob/main/schemas/parser_schema.json",
     "instagram": {
         // Optional
         "lamadava_saas_token": "asdasd"
     },
     "reddit": {
         "client_id": "",
         "client_secret": "",
         // Optional
         "user_agent": "video downloader (by u/Jag_k)"
     },
     "tiktok": {},
     "twitter": {
-        "twitter_bearer_token": ""
+        "twitter_bearer_token": "asdasd"
     },
     "youtube": {}
 }
 ```
 
+Or you can use YAML file like `config/parsers.yaml` or `config/parsers.yml`:
+
+```yaml
+# config/parsers.yml
+$schema: "https://raw.github.com/jag-k/media-parsers/blob/main/schemas/parser_schema.json"
+instagram:
+    # Optional
+    lamadava_saas_token: "asdasd"
+reddit:
+    client_id: ""
+    client_secret: ""
+    # Optional
+    user_agent: "video downloader (by u/Jag_k)"
+tiktok: {}
+twitter:
+    twitter_bearer_token: "asdasd"
+youtube: {}
+```
+
 ## Usage
 
 API documentation available on `/docs` endpoint.
 
 ## Clients
 
 ### Installation
 
 ```bash
-poetry add git+https://github.com/jag-k/media-parser.git
+poetry add media-parser  # or pip install media-parser
 ```
 
 ### Usage
 
 ```python
 from media_parser import Client, FeedbackTypes
```

