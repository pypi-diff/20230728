# Comparing `tmp/aiovodafone-0.0.4.tar.gz` & `tmp/aiovodafone-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiovodafone-0.0.4.tar", max compression
+gzip compressed data, was "aiovodafone-0.0.5.tar", max compression
```

## Comparing `aiovodafone-0.0.4.tar` & `aiovodafone-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-01 21:54:25.274871 aiovodafone-0.0.4/LICENSE
--rw-r--r--   0        0        0     3314 2023-07-01 21:54:25.274871 aiovodafone-0.0.4/README.md
--rw-r--r--   0        0        0     1945 2023-07-01 21:54:26.202867 aiovodafone-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      293 2023-07-01 21:54:26.166868 aiovodafone-0.0.4/src/aiovodafone/__init__.py
--rw-r--r--   0        0        0     9450 2023-07-01 21:54:25.274871 aiovodafone-0.0.4/src/aiovodafone/api.py
--rw-r--r--   0        0        0      347 2023-07-01 21:54:25.274871 aiovodafone-0.0.4/src/aiovodafone/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-01 21:54:25.274871 aiovodafone-0.0.4/src/aiovodafone/py.typed
--rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 aiovodafone-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-28 20:59:28.822862 aiovodafone-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3314 2023-07-28 20:59:28.822862 aiovodafone-0.0.5/README.md
+-rw-r--r--   0        0        0     1946 2023-07-28 20:59:29.550861 aiovodafone-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-07-28 20:59:29.518861 aiovodafone-0.0.5/src/aiovodafone/__init__.py
+-rw-r--r--   0        0        0     9713 2023-07-28 20:59:28.826862 aiovodafone-0.0.5/src/aiovodafone/api.py
+-rw-r--r--   0        0        0      226 2023-07-28 20:59:28.826862 aiovodafone-0.0.5/src/aiovodafone/const.py
+-rw-r--r--   0        0        0      441 2023-07-28 20:59:28.826862 aiovodafone-0.0.5/src/aiovodafone/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-28 20:59:28.826862 aiovodafone-0.0.5/src/aiovodafone/py.typed
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 aiovodafone-0.0.5/PKG-INFO
```

### Comparing `aiovodafone-0.0.4/LICENSE` & `aiovodafone-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovodafone-0.0.4/README.md` & `aiovodafone-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiovodafone-0.0.4/pyproject.toml` & `aiovodafone-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiovodafone"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python library to control Vodafone Station"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiovodafone"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -18,15 +18,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chemelli74/aiovodafone/issues"
 "Changelog" = "https://github.com/chemelli74/aiovodafone/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 aiohttp = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 
 [tool.semantic_release]
```

### Comparing `aiovodafone-0.0.4/src/aiovodafone/api.py` & `aiovodafone-0.0.5/src/aiovodafone/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Support for Vodafone Station."""
 import asyncio
 import hashlib
 import hmac
 import html
-import logging
 import re
 import urllib.parse
 from dataclasses import dataclass
 from datetime import datetime
 from http.cookies import SimpleCookie
 from typing import Any
 
 import aiohttp
 
-from .exceptions import CannotAuthenticate, CannotConnect
-
-_LOGGER = logging.getLogger(__package__)
+from .const import _LOGGER, LOGIN
+from .exceptions import AlreadyLogged, CannotAuthenticate, CannotConnect
 
 
 @dataclass
 class VodafoneStationDevice:
     """Vodafone Station device class."""
 
     connected: bool
@@ -251,18 +249,27 @@
             url,
             data=payload,
             headers=self.headers,
             timeout=10,
             verify_ssl=False,
             allow_redirects=True,
         )
-        if reply.status != 200:
+        reply_json = await reply.json(content_type="text/html")
+        _LOGGER.debug("Login result: %s[%s]", LOGIN[int(reply_json)], reply_json)
+
+        if reply_json == "1":
+            return True
+
+        if reply_json == "2":
+            raise AlreadyLogged
+
+        if reply_json in ["3", "4"]:
             raise CannotAuthenticate
 
-        return True
+        return False
 
     async def logout(self) -> None:
         """Router logout."""
         self.session.cookie_jar.clear()
 
     async def close(self) -> None:
         """Router close session."""
```

### Comparing `aiovodafone-0.0.4/PKG-INFO` & `aiovodafone-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: aiovodafone
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library to control Vodafone Station
 Home-page: https://github.com/chemelli74/aiovodafone
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp
 Project-URL: Bug Tracker, https://github.com/chemelli74/aiovodafone/issues
 Project-URL: Changelog, https://github.com/chemelli74/aiovodafone/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/chemelli74/aiovodafone
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1 Name: aiovodafone Version: 0.0.4 Summary: Python library
+Metadata-Version: 2.1 Name: aiovodafone Version: 0.0.5 Summary: Python library
 to control Vodafone Station Home-page: https://github.com/chemelli74/
 aiovodafone License: Apache Software License 2.0 Author: Simone Chemelli
-Author-email: simone.chemelli@gmail.com Requires-Python: >=3.7,<4.0 Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Natural Language
-:: English Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: aiohttp Project-URL:
-Bug Tracker, https://github.com/chemelli74/aiovodafone/issues Project-URL:
-Changelog, https://github.com/chemelli74/aiovodafone/blob/main/CHANGELOG.md
-Project-URL: Repository, https://github.com/chemelli74/aiovodafone Description-
-Content-Type: text/markdown # aiovodafone
+Author-email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: Other/Proprietary License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries Requires-Dist: aiohttp
+Project-URL: Bug Tracker, https://github.com/chemelli74/aiovodafone/issues
+Project-URL: Changelog, https://github.com/chemelli74/aiovodafone/blob/main/
+CHANGELOG.md Project-URL: Repository, https://github.com/chemelli74/aiovodafone
+Description-Content-Type: text/markdown # aiovodafone
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Python library to control Vodafone Station ## Installation Install this via pip
 (or your favourite package manager): `pip install aiovodafone` ## Contributors
 â¨ Thanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):       This project follows the [all-
```

