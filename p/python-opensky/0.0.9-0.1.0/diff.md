# Comparing `tmp/python_opensky-0.0.9.tar.gz` & `tmp/python_opensky-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.9.tar", max compression
+gzip compressed data, was "python_opensky-0.1.0.tar", max compression
```

## Comparing `python_opensky-0.0.9.tar` & `python_opensky-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-06-08 08:13:32.549572 python_opensky-0.0.9/LICENSE.md
--rw-r--r--   0        0        0     5328 2023-06-08 08:13:32.549572 python_opensky-0.0.9/README.md
--rw-r--r--   0        0        0     3661 2023-06-08 08:13:50.987213 python_opensky-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      444 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      849 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/const.py
--rw-r--r--   0        0        0      384 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     3573 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/models.py
--rw-r--r--   0        0        0     9203 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-06-08 08:13:32.549572 python_opensky-0.0.9/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 python_opensky-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-28 10:26:54.231170 python_opensky-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     5321 2023-07-28 10:26:54.231170 python_opensky-0.1.0/README.md
+-rw-r--r--   0        0        0     3661 2023-07-28 10:27:11.628697 python_opensky-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3714 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/models.py
+-rw-r--r--   0        0        0     9397 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 python_opensky-0.1.0/PKG-INFO
```

### Comparing `python_opensky-0.0.9/LICENSE.md` & `python_opensky-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.9/README.md` & `python_opensky-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,14 @@
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/joostlek/python-opensky.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
-[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-stable-green.svg
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/python-opensky
 [releases-shield]: https://img.shields.io/github/release/joostlek/python-opensky.svg
 [releases]: https://github.com/joostlek/python-opensky/releases
 [semver]: http://semver.org/spec/v2.0.0.html
 [sonarcloud]: https://sonarcloud.io/summary/new_code?id=joostlek_python-opensky
 [pypi]: https://pypi.org/project/python-opensky/
```

### Comparing `python_opensky-0.0.9/pyproject.toml` & `python_opensky-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.9"
+version = "0.1.0"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
@@ -28,27 +28,27 @@
 python = "^3.10"
 aiohttp = ">=3.0.0"
 yarl = ">=1.6.0"
 pydantic = ">=1.10.8"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "2.1.6"
-black = "23.3.0"
-blacken-docs = "1.13.0"
-codespell = "2.2.4"
+black = "23.7.0"
+blacken-docs = "1.15.0"
+codespell = "2.2.5"
 covdefaults = "2.3.0"
 coverage = {version = "7.2.7", extras = ["toml"]}
-mypy = "1.3.0"
-pre-commit = "3.3.2"
+mypy = "1.4.1"
+pre-commit = "3.3.3"
 pre-commit-hooks = "4.4.0"
-pylint = "2.17.4"
-pytest = "7.3.1"
-pytest-asyncio = "0.21.0"
+pylint = "2.17.5"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
-ruff = "0.0.272"
+ruff = "0.0.280"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-opensky/issues"
 Changelog = "https://github.com/joostlek/python-opensky/releases"
```

### Comparing `python_opensky-0.0.9/src/python_opensky/const.py` & `python_opensky-0.1.0/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.9/src/python_opensky/models.py` & `python_opensky-0.1.0/src/python_opensky/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Asynchronous Python client for the OpenSky API."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from pydantic import BaseModel, Field
+try:
+    from pydantic.v1 import BaseModel, Field
+except ImportError:  # pragma: no cover
+    from pydantic import BaseModel, Field  # type: ignore[assignment] # pragma: no cover
 
 from .const import AircraftCategory, PositionSource
 from .exceptions import OpenSkyCoordinateError
 
 
 class StatesResponse(BaseModel):
     """Represents the states response."""
```

### Comparing `python_opensky-0.0.9/src/python_opensky/opensky.py` & `python_opensky-0.1.0/src/python_opensky/opensky.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,21 @@
             params[MAX_LATITUDE] = bounding_box.max_latitude
             params[MIN_LONGITUDE] = bounding_box.min_longitude
             params[MAX_LONGITUDE] = bounding_box.max_longitude
             credit_cost = self.calculate_credit_costs(bounding_box)
 
         data = await self._request("states/all", data=params)
 
-        data = {
-            **data,
-            "states": [self._convert_state(state) for state in data["states"]],
-        }
+        if data["states"] is None:
+            data["states"] = []
+        else:
+            data = {
+                **data,
+                "states": [self._convert_state(state) for state in data["states"]],
+            }
 
         self._register_credit_usage(credit_cost)
 
         return StatesResponse.parse_obj(data)
 
     async def get_own_states(self, time: int = 0) -> StatesResponse:
         """Retrieve state vectors from your own sensors."""
@@ -158,18 +161,21 @@
             raise OpenSkyUnauthenticatedError
         params = {
             "time": time,
         }
 
         data = await self._request("states/own", data=params)
 
-        data = {
-            **data,
-            "states": [self._convert_state(state) for state in data["states"]],
-        }
+        if data["states"] is None:
+            data["states"] = []
+        else:
+            data = {
+                **data,
+                "states": [self._convert_state(state) for state in data["states"]],
+            }
 
         return StatesResponse.parse_obj(data)
 
     @staticmethod
     def calculate_credit_costs(bounding_box: BoundingBox) -> int:
         """Calculate the amount of credits a request costs."""
         latitude_degrees = bounding_box.max_latitude - bounding_box.min_latitude
```

### Comparing `python_opensky-0.0.9/PKG-INFO` & `python_opensky-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.9
+Version: 0.1.0
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -171,15 +171,15 @@
 [joostlek]: https://github.com/joostlek
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/joostlek/python-opensky.svg
 [maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
-[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-stable-green.svg
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/python-opensky
 [releases-shield]: https://img.shields.io/github/release/joostlek/python-opensky.svg
 [releases]: https://github.com/joostlek/python-opensky/releases
 [semver]: http://semver.org/spec/v2.0.0.html
 [sonarcloud]: https://sonarcloud.io/summary/new_code?id=joostlek_python-opensky
 [pypi]: https://pypi.org/project/python-opensky/
```

