# Comparing `tmp/pybsky-0.0.18.tar.gz` & `tmp/pybsky-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybsky-0.0.18.tar", last modified: Fri Jul 28 12:10:07 2023, max compression
+gzip compressed data, was "pybsky-0.0.2.tar", last modified: Sun Jul 23 19:40:03 2023, max compression
```

## Comparing `pybsky-0.0.18.tar` & `pybsky-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:10:07.801110 pybsky-0.0.18/
--rw-rw-rw-   0        0        0     1100 2023-07-23 19:53:13.000000 pybsky-0.0.18/LICENSE
--rw-rw-rw-   0        0        0     1371 2023-07-28 12:10:07.801110 pybsky-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-07-28 11:37:14.000000 pybsky-0.0.18/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 12:10:07.770108 pybsky-0.0.18/pybsky/
-drwxrwxrwx   0        0        0        0 2023-07-28 12:10:07.777109 pybsky-0.0.18/pybsky/core/
--rw-rw-rw-   0        0        0      101 2023-07-25 18:51:39.000000 pybsky-0.0.18/pybsky/core/__init__.py
--rw-rw-rw-   0        0        0      769 2023-07-28 08:27:10.000000 pybsky-0.0.18/pybsky/core/configs.py
--rw-rw-rw-   0        0        0      432 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/core/exceptions.py
--rw-rw-rw-   0        0        0     5947 2023-07-23 19:53:13.000000 pybsky-0.0.18/pybsky/core/user_agents.py
--rw-rw-rw-   0        0        0     1161 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:10:07.786109 pybsky-0.0.18/pybsky/mixins/
--rw-rw-rw-   0        0        0      217 2023-07-28 07:23:56.000000 pybsky-0.0.18/pybsky/mixins/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-23 19:53:13.000000 pybsky-0.0.18/pybsky/mixins/base.py
--rw-rw-rw-   0        0        0     2158 2023-07-28 06:58:53.000000 pybsky-0.0.18/pybsky/mixins/feed.py
--rw-rw-rw-   0        0        0     2946 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/mixins/graph.py
--rw-rw-rw-   0        0        0     1587 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/mixins/login.py
--rw-rw-rw-   0        0        0     2189 2023-07-28 08:27:10.000000 pybsky-0.0.18/pybsky/mixins/post.py
--rw-rw-rw-   0        0        0      491 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/mixins/profile.py
--rw-rw-rw-   0        0        0      910 2023-07-28 08:27:10.000000 pybsky-0.0.18/pybsky/mixins/repo.py
--rw-rw-rw-   0        0        0      368 2023-07-27 23:24:50.000000 pybsky-0.0.18/pybsky/mixins/server.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:10:07.799121 pybsky-0.0.18/pybsky/pybsky.egg-info/
--rw-rw-rw-   0        0        0     1371 2023-07-28 12:10:07.000000 pybsky-0.0.18/pybsky/pybsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-28 12:10:07.000000 pybsky-0.0.18/pybsky/pybsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:10:07.000000 pybsky-0.0.18/pybsky/pybsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 12:10:07.000000 pybsky-0.0.18/pybsky/pybsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-28 12:10:07.000000 pybsky-0.0.18/pybsky/pybsky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1248 2023-07-28 12:09:51.000000 pybsky-0.0.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 12:10:07.801110 pybsky-0.0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.421621 pybsky-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-23 19:26:05.000000 pybsky-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.420621 pybsky-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-07-23 19:38:22.000000 pybsky-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.399622 pybsky-0.0.2/pybsky/
+-rw-rw-rw-   0        0        0       68 2023-07-23 18:34:27.000000 pybsky-0.0.2/pybsky/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 18:18:34.000000 pybsky-0.0.2/pybsky/client.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.416622 pybsky-0.0.2/pybsky/core/
+-rw-rw-rw-   0        0        0      122 2023-07-23 18:34:23.000000 pybsky-0.0.2/pybsky/core/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-07-21 12:03:54.000000 pybsky-0.0.2/pybsky/core/configs.py
+-rw-rw-rw-   0        0        0      266 2023-07-21 11:59:59.000000 pybsky-0.0.2/pybsky/core/exceptions.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:13:17.000000 pybsky-0.0.2/pybsky/core/log.py
+-rw-rw-rw-   0        0        0     5947 2023-07-23 18:36:54.000000 pybsky-0.0.2/pybsky/core/user_agents.py
+-rw-rw-rw-   0        0        0     1038 2023-07-23 18:38:10.000000 pybsky-0.0.2/pybsky/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.419622 pybsky-0.0.2/pybsky/mixins/
+-rw-rw-rw-   0        0        0       60 2023-07-23 18:34:35.000000 pybsky-0.0.2/pybsky/mixins/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 19:51:23.000000 pybsky-0.0.2/pybsky/mixins/base.py
+-rw-rw-rw-   0        0        0      878 2023-07-23 18:18:45.000000 pybsky-0.0.2/pybsky/mixins/feed.py
+-rw-rw-rw-   0        0        0     1399 2023-07-23 18:18:50.000000 pybsky-0.0.2/pybsky/mixins/login.py
+drwxrwxrwx   0        0        0        0 2023-07-23 19:40:03.411622 pybsky-0.0.2/pybsky.egg-info/
+-rw-rw-rw-   0        0        0     1183 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-23 19:40:03.000000 pybsky-0.0.2/pybsky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1031 2023-07-23 19:39:45.000000 pybsky-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-23 19:40:03.421621 pybsky-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-23 19:20:21.000000 pybsky-0.0.2/setup.py
```

### Comparing `pybsky-0.0.18/LICENSE` & `pybsky-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybsky-0.0.18/PKG-INFO` & `pybsky-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.18
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
-Project-URL: BugTracker, https://github.com/softrebel/pybsky/issues
-Project-URL: Repository, https://github.com/softrebel/pybsky
+Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
-# Requirements
-Python 3.10+
-
-Pybsky stands on the shoulder of:
-- requests package
-
-# Installation
-<div class="termy">
-  
-```console
- $ pip install pybsky
-
----> 100%
-```
-</div>
 
-## Feature List:
+## TODO List:
 
 - [x] Create Client
 - [x] Add Login logic
-- [x] Get Profile logic
-- [x] Get Follwer/Following logic
-- [x] Follow/Unfollow
-- [x] Get likes
-- [x] Get post, thread via replies
-- [x] Get Author Feed/Timeline
-- [x] Create post (text and image)
+- [ ] Get Profile logic
+- [ ] Get Follwer/Following logic
+- [ ] Follow/Unfollow
+- [ ] Get Likers
+- [ ] Get Commenters
+- [ ] Get Feed/Timeline
+- [ ] Post skeets
 
 ## License
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 
 - This project is licensed under the terms of the **[MIT license](LICENSE)**
```

### Comparing `pybsky-0.0.18/pybsky/core/user_agents.py` & `pybsky-0.0.2/pybsky/core/user_agents.py`

 * *Files identical despite different names*

### Comparing `pybsky-0.0.18/pybsky/core/utils.py` & `pybsky-0.0.2/pybsky/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 import json
 import requests
-from .exceptions import (
-    AuthenticationRequiredException,
-    UnknownResponseException,
-    BadRequestResponseException,
-)
-
+from .exceptions import AuthenticationRequiredException,UnknownResponseException,\
+    BadRequestResponseException
 Response = requests.models.Response
 
 
 def validate_value(value, cls):
     if not isinstance(value, cls):
-        raise TypeError(f"{value} must be in type {cls}")
+        raise TypeError(f'{value} must be in type {cls}')
     return True
 
 
 def json_decode(s: str) -> list | dict:
     return json.loads(s)
 
 
 def json_encode(obj: object) -> str:
     return json.dumps(obj, indent=4, ensure_ascii=False)
 
 
 def validate_get_response(response: Response):
-    if response.text and response.text != "":
-        content = response.json()
-    else:
-        content = response.text
+    content = response.json()
     if response.status_code == 200:
         return content
     elif response.status_code == 401:
-        raise AuthenticationRequiredException(content["message"])
+        raise AuthenticationRequiredException(content['message'])
     elif response.status_code == 400:
-        raise BadRequestResponseException(content["message"])
+        raise BadRequestResponseException(content['message'])
     else:
         raise UnknownResponseException(
-            f"status code => {response.status_code} , response => {response.text}"
-        )
+            f"status code => {response.status_code} , response => {response.text}")
 
     # TODO => handle all type of response
```

### Comparing `pybsky-0.0.18/pybsky/mixins/feed.py` & `pybsky-0.0.2/pybsky/mixins/feed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,27 @@
-from ..core import (
-    validate_get_response,
-    validate_value,
-    FEED_URL,
-    BSKY_BASE_URL,
-    GET_TIMELINE_URL,
-    GET_POSTS_URL,
-    GET_POST_THREAD,
-)
 
 
-class FeedMixin:
+from ..core import validate_get_response, validate_value, FEED_URL, BSKY_BASE_URL
+
+
+class FeedMixin():
+
     def get_author_feed(self, actor: str, limit: int = 30):
         validate_value(actor, str)
         headers = {
-            "origin": "https://bsky.app",
-            "referer": "https://bsky.app/",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "cross-site",
-            "user-agent": self.user_agent,
-            "authorization": f"Bearer {self.access_jwt}",
+            'origin': 'https://bsky.app',
+            'referer': 'https://bsky.app/',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'cross-site',
+            'user-agent': self.user_agent,
+            'authorization': f'Bearer {self.access_jwt}'
         }
 
         params = {
-            "actor": self.get_actor(actor),
-            "limit": limit,
+            'actor': self.get_actor(actor),
+            'limit': limit,
         }
-        url = f"{BSKY_BASE_URL}{FEED_URL}"
+        url = f'{BSKY_BASE_URL}{FEED_URL}'
         response = self.session.get(url, params=params, headers=headers)
         validated_response = validate_get_response(response)
         return validated_response
-
-    def get_timeline(self, algorithm: str = "reverse-chronological", limit: int = 30):
-        validate_value(algorithm, str)
-        validate_value(limit, int)
-        params = {
-            "actor": algorithm,
-            "limit": limit,
-        }
-        url = f"{BSKY_BASE_URL}{GET_TIMELINE_URL}"
-        response = self.send_request(method="GET", url=url, params=params)
-        validated_response = validate_get_response(response)
-        return validated_response
-
-    def get_posts(self, uris: str):
-        validate_value(uris, str)
-        params = {
-            "uris": uris,
-        }
-        url = f"{BSKY_BASE_URL}{GET_POSTS_URL}"
-        response = self.send_request(method="GET", url=url, params=params)
-        validated_response = validate_get_response(response)
-        return validated_response
-
-    def get_post_thread(self, uri: str):
-        validate_value(uri, str)
-        params = {
-            "uri": uri,
-        }
-        url = f"{BSKY_BASE_URL}{GET_POST_THREAD}"
-        response = self.send_request(method="GET", url=url, params=params)
-        validated_response = validate_get_response(response)
-        return validated_response
```

### Comparing `pybsky-0.0.18/pybsky/mixins/login.py` & `pybsky-0.0.2/pybsky/mixins/login.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import random
 import requests
 
 from ..core import USER_AGENTS, validate_value, validate_get_response
 
 
-class LoginMixin:
+class LoginMixin():
+
     def login(self, username: str, password: str):
         validate_value(username, str)
         validate_value(password, str)
         if len(username) == 0:
-            raise ValueError("username should not be empty")
+            raise ValueError('username should not be empty')
         if len(password) == 0:
-            raise ValueError("username should not be empty")
+            raise ValueError('username should not be empty')
 
         session = requests.Session()
         session.timeout = 30
         session.proxies = self.session.proxies
 
         self.user_agent = random.choice(USER_AGENTS)
 
         headers = {
-            "origin": "https://bsky.app",
-            "referer": "https://bsky.app/",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "cross-site",
-            "user-agent": self.user_agent,
+            'origin': 'https://bsky.app',
+            'referer': 'https://bsky.app/',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'cross-site',
+            'user-agent': self.user_agent
         }
 
         payload = {
-            "identifier": self.get_actor(username),
-            "password": password,
+            'identifier': self.get_actor(username),
+            'password': password,
         }
-        url = "https://bsky.social/xrpc/com.atproto.server.createSession"
+        url = 'https://bsky.social/xrpc/com.atproto.server.createSession'
         response = requests.post(url, headers=headers, json=payload)
 
         validated_response = validate_get_response(response)
         self.access_jwt = validated_response["accessJwt"]
         self.refresh_jwt = validated_response["refreshJwt"]
-        self.session.headers.update({"authorization": f"Bearer {self.access_jwt}"})
-        own_profile = self.get_profile(self.get_actor(username))
-        self.own_profile = own_profile
         return validated_response
```

### Comparing `pybsky-0.0.18/pybsky/pybsky.egg-info/PKG-INFO` & `pybsky-0.0.2/pybsky.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 Metadata-Version: 2.1
 Name: pybsky
-Version: 0.0.18
+Version: 0.0.2
 Summary: Python Client for bsky social media
+Author: softrebel, ovan
 Author-email: Mohammadreza softrebel <sh.mohammad66@yahoo.com>, Mahdi Ovan <mahdi.ovan@yahoo.com>
 Project-URL: Homepage, https://github.com/softrebel/pybsky
-Project-URL: BugTracker, https://github.com/softrebel/pybsky/issues
-Project-URL: Repository, https://github.com/softrebel/pybsky
+Project-URL: Bug Tracker, https://github.com/softrebel/pybsky/issues
+Keywords: python,pybsky,bsky
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pybsky
 
 <div align='center'>
-
-![./a](./assets/cover.png)
+    <img src="./assets/cover.png" height="150" width="500" alt="pybsky-logo" >
 
 </div>
 
-# Requirements
-Python 3.10+
-
-Pybsky stands on the shoulder of:
-- requests package
-
-# Installation
-<div class="termy">
-  
-```console
- $ pip install pybsky
-
----> 100%
-```
-</div>
 
-## Feature List:
+## TODO List:
 
 - [x] Create Client
 - [x] Add Login logic
-- [x] Get Profile logic
-- [x] Get Follwer/Following logic
-- [x] Follow/Unfollow
-- [x] Get likes
-- [x] Get post, thread via replies
-- [x] Get Author Feed/Timeline
-- [x] Create post (text and image)
+- [ ] Get Profile logic
+- [ ] Get Follwer/Following logic
+- [ ] Follow/Unfollow
+- [ ] Get Likers
+- [ ] Get Commenters
+- [ ] Get Feed/Timeline
+- [ ] Post skeets
 
 ## License
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
 
 - This project is licensed under the terms of the **[MIT license](LICENSE)**
```

### Comparing `pybsky-0.0.18/pyproject.toml` & `pybsky-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 [project]
 name = "pybsky"
-version = "0.0.18"
+version = "0.0.2"
 authors = [
   { name="Mohammadreza softrebel", email="sh.mohammad66@yahoo.com" },
     { name="Mahdi Ovan", email="mahdi.ovan@yahoo.com" },
 ]
 description ='Python Client for bsky social media'
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "requests==2.31.0",
-]
 
 [project.urls]
-Homepage = "https://github.com/softrebel/pybsky"
-BugTracker = "https://github.com/softrebel/pybsky/issues"
-Repository = "https://github.com/softrebel/pybsky"
-
+"Homepage" = "https://github.com/softrebel/pybsky"
+"Bug Tracker" = "https://github.com/softrebel/pybsky/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.ruff]
 # Enable flake8-bugbear (`B`) rules.
@@ -36,11 +31,7 @@
 
 # Avoid trying to fix flake8-bugbear (`B`) violations.
 unfixable = ["B"]
 
 # Ignore `E402` (import violations) in all `__init__.py` files`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402","F403","F401"]
-
-[tool.setuptools.packages.find]
-where = ["pybsky"]  # list of folders that contain the packages (["."] by default)
-
```

