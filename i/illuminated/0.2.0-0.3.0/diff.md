# Comparing `tmp/illuminated-0.2.0.tar.gz` & `tmp/illuminated-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illuminated-0.2.0.tar", max compression
+gzip compressed data, was "illuminated-0.3.0.tar", max compression
```

## Comparing `illuminated-0.2.0.tar` & `illuminated-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0     1072 2023-04-01 19:55:45.142614 illuminated-0.2.0/LICENSE
--rw-r--r--   0        0        0       22 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/__init__.py
--rw-r--r--   0        0        0       29 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/adapter/__init__.py
--rw-r--r--   0        0        0     2046 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/adapter/adapter.py
--rw-r--r--   0        0        0     4507 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/cli.py
--rw-r--r--   0        0        0      219 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/common/__init__.py
--rw-r--r--   0        0        0       57 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/common/project_definitions.py
--rw-r--r--   0        0        0      535 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/common/project_logging.py
--rw-r--r--   0        0        0    14120 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/common/project_templates.py
--rw-r--r--   0        0        0      130 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/decorators/__init__.py
--rw-r--r--   0        0        0     2790 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/decorators/cli.py
--rw-r--r--   0        0        0     4481 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/decorators/logging.py
--rw-r--r--   0        0        0      272 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/__init__.py
--rw-r--r--   0        0        0      156 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/adapter.py
--rw-r--r--   0        0        0       88 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/basic.py
--rw-r--r--   0        0        0      158 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/exporter.py
--rw-r--r--   0        0        0      161 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/manager.py
--rw-r--r--   0        0        0      164 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/observation.py
--rw-r--r--   0        0        0      158 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exceptions/observer.py
--rw-r--r--   0        0        0       61 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exporter/__init__.py
--rw-r--r--   0        0        0      615 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exporter/exporter.py
--rw-r--r--   0        0        0     2133 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/exporter/sql.py
--rw-r--r--   0        0        0      226 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/__init__.py
--rw-r--r--   0        0        0      201 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/adapter.py
--rw-r--r--   0        0        0     1052 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/assistant.py
--rw-r--r--   0        0        0      179 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/exporter.py
--rw-r--r--   0        0        0       55 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/finding.py
--rw-r--r--   0        0        0      801 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/manager.py
--rw-r--r--   0        0        0      186 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/observation.py
--rw-r--r--   0        0        0      270 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/interface/observer.py
--rw-r--r--   0        0        0       62 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/manager/__init__.py
--rw-r--r--   0        0        0     7870 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/manager/assistant.py
--rw-r--r--   0        0        0    16943 2023-04-01 19:55:45.142614 illuminated-0.2.0/illuminate/manager/manager.py
--rw-r--r--   0        0        0        0 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/meta/__init__.py
--rw-r--r--   0        0        0       27 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/meta/type/__init__.py
--rw-r--r--   0        0        0      316 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/meta/type/result.py
--rw-r--r--   0        0        0      174 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observation/__init__.py
--rw-r--r--   0        0        0     2569 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observation/file.py
--rw-r--r--   0        0        0     5219 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observation/http.py
--rw-r--r--   0        0        0     1100 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observation/observation.py
--rw-r--r--   0        0        0     2583 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observation/sql.py
--rw-r--r--   0        0        0       60 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observer/__init__.py
--rw-r--r--   0        0        0      176 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observer/finding.py
--rw-r--r--   0        0        0     1483 2023-04-01 19:55:45.146614 illuminated-0.2.0/illuminate/observer/observer.py
--rw-r--r--   0        0        0     1587 2023-04-01 19:55:45.146614 illuminated-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1263 2023-04-01 19:55:55.151872 illuminated-0.2.0/setup.py
--rw-r--r--   0        0        0     1120 2023-04-01 19:55:55.152316 illuminated-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1093 2022-12-21 15:55:05.442433 illuminated-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0       23 2023-07-28 19:54:36.397918 illuminated-0.3.0/illuminate/__init__.py
+-rwxr-xr-x   0        0        0       30 2023-04-01 21:37:30.363030 illuminated-0.3.0/illuminate/adapter/__init__.py
+-rwxr-xr-x   0        0        0     2046 2023-04-01 21:37:30.373821 illuminated-0.3.0/illuminate/adapter/adapter.py
+-rwxr-xr-x   0        0        0     4507 2023-07-05 12:05:30.956124 illuminated-0.3.0/illuminate/cli.py
+-rwxr-xr-x   0        0        0      277 2023-07-28 19:54:36.412918 illuminated-0.3.0/illuminate/common/__init__.py
+-rwxr-xr-x   0        0        0       94 2023-07-28 19:54:36.424917 illuminated-0.3.0/illuminate/common/project_definitions.py
+-rwxr-xr-x   0        0        0      558 2022-12-21 15:55:05.528298 illuminated-0.3.0/illuminate/common/project_logging.py
+-rwxr-xr-x   0        0        0    17219 2023-07-28 19:54:36.436919 illuminated-0.3.0/illuminate/common/project_templates.py
+-rwxr-xr-x   0        0        0      134 2023-07-02 15:14:00.503821 illuminated-0.3.0/illuminate/decorators/__init__.py
+-rwxr-xr-x   0        0        0     3850 2023-07-28 19:54:36.451918 illuminated-0.3.0/illuminate/decorators/cli.py
+-rwxr-xr-x   0        0        0     4635 2023-07-02 15:17:14.798756 illuminated-0.3.0/illuminate/decorators/logging.py
+-rwxr-xr-x   0        0        0      279 2023-04-01 21:37:30.469616 illuminated-0.3.0/illuminate/exceptions/__init__.py
+-rwxr-xr-x   0        0        0      161 2023-04-01 21:37:30.480617 illuminated-0.3.0/illuminate/exceptions/adapter.py
+-rwxr-xr-x   0        0        0       88 2022-12-21 15:55:05.566662 illuminated-0.3.0/illuminate/exceptions/basic.py
+-rwxr-xr-x   0        0        0      163 2023-04-01 21:37:30.490616 illuminated-0.3.0/illuminate/exceptions/exporter.py
+-rwxr-xr-x   0        0        0      161 2023-04-01 21:37:30.501617 illuminated-0.3.0/illuminate/exceptions/manager.py
+-rwxr-xr-x   0        0        0      169 2023-04-01 21:37:30.512616 illuminated-0.3.0/illuminate/exceptions/observation.py
+-rwxr-xr-x   0        0        0      163 2023-04-01 21:37:30.523617 illuminated-0.3.0/illuminate/exceptions/observer.py
+-rwxr-xr-x   0        0        0      104 2023-07-28 19:54:36.466919 illuminated-0.3.0/illuminate/exporter/__init__.py
+-rwxr-xr-x   0        0        0      615 2023-04-01 21:37:30.548617 illuminated-0.3.0/illuminate/exporter/exporter.py
+-rwxr-xr-x   0        0        0     2522 2023-07-28 19:54:36.475918 illuminated-0.3.0/illuminate/exporter/influxdb.py
+-rwxr-xr-x   0        0        0     2133 2023-04-01 21:37:30.560616 illuminated-0.3.0/illuminate/exporter/sql.py
+-rwxr-xr-x   0        0        0      233 2023-04-01 21:37:30.575617 illuminated-0.3.0/illuminate/interface/__init__.py
+-rwxr-xr-x   0        0        0      207 2022-12-21 15:55:05.614662 illuminated-0.3.0/illuminate/interface/adapter.py
+-rwxr-xr-x   0        0        0     1089 2022-12-21 15:55:05.620662 illuminated-0.3.0/illuminate/interface/assistant.py
+-rwxr-xr-x   0        0        0      185 2022-12-21 15:55:05.625662 illuminated-0.3.0/illuminate/interface/exporter.py
+-rwxr-xr-x   0        0        0       57 2022-12-21 15:55:05.630662 illuminated-0.3.0/illuminate/interface/finding.py
+-rwxr-xr-x   0        0        0      827 2022-12-21 15:55:05.635662 illuminated-0.3.0/illuminate/interface/manager.py
+-rwxr-xr-x   0        0        0      192 2022-12-21 15:55:05.641662 illuminated-0.3.0/illuminate/interface/observation.py
+-rwxr-xr-x   0        0        0      279 2022-12-21 15:55:05.646664 illuminated-0.3.0/illuminate/interface/observer.py
+-rwxr-xr-x   0        0        0       64 2023-04-01 21:37:30.588616 illuminated-0.3.0/illuminate/manager/__init__.py
+-rwxr-xr-x   0        0        0     9548 2023-07-28 19:54:36.490917 illuminated-0.3.0/illuminate/manager/assistant.py
+-rwxr-xr-x   0        0        0    17505 2023-07-28 19:54:36.503918 illuminated-0.3.0/illuminate/manager/manager.py
+-rwxr-xr-x   0        0        0        0 2023-04-01 21:37:30.615616 illuminated-0.3.0/illuminate/meta/__init__.py
+-rwxr-xr-x   0        0        0       34 2023-03-26 20:23:51.823344 illuminated-0.3.0/illuminate/meta/class/__init__.py
+-rwxr-xr-x   0        0        0      479 2022-11-19 21:45:24.704813 illuminated-0.3.0/illuminate/meta/class/singleton.py
+-rwxr-xr-x   0        0        0       28 2023-04-01 21:37:30.630617 illuminated-0.3.0/illuminate/meta/type/__init__.py
+-rwxr-xr-x   0        0        0      328 2023-04-01 21:37:30.638617 illuminated-0.3.0/illuminate/meta/type/result.py
+-rwxr-xr-x   0        0        0      180 2023-06-05 14:08:08.839287 illuminated-0.3.0/illuminate/observation/__init__.py
+-rwxr-xr-x   0        0        0     2766 2023-07-28 19:54:36.518918 illuminated-0.3.0/illuminate/observation/file.py
+-rwxr-xr-x   0        0        0     5500 2023-07-28 19:54:36.530918 illuminated-0.3.0/illuminate/observation/http.py
+-rwxr-xr-x   0        0        0     2715 2023-05-10 19:11:27.119804 illuminated-0.3.0/illuminate/observation/kafka.py
+-rwxr-xr-x   0        0        0     1256 2023-07-28 19:54:36.542920 illuminated-0.3.0/illuminate/observation/observation.py
+-rwxr-xr-x   0        0        0     2779 2023-07-28 19:54:36.554920 illuminated-0.3.0/illuminate/observation/sql.py
+-rwxr-xr-x   0        0        0       62 2023-04-01 21:37:30.699779 illuminated-0.3.0/illuminate/observer/__init__.py
+-rwxr-xr-x   0        0        0      184 2023-04-01 21:37:30.709777 illuminated-0.3.0/illuminate/observer/finding.py
+-rwxr-xr-x   0        0        0     1483 2023-04-01 21:37:30.719777 illuminated-0.3.0/illuminate/observer/observer.py
+-rwxr-xr-x   0        0        0     1711 2023-07-28 19:54:36.572917 illuminated-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1361 2023-07-28 20:19:56.162924 illuminated-0.3.0/setup.py
+-rw-r--r--   0        0        0     1234 2023-07-28 20:19:56.163266 illuminated-0.3.0/PKG-INFO
```

### Comparing `illuminated-0.2.0/LICENSE` & `illuminated-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Nikola Milojica
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Nikola Milojica
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `illuminated-0.2.0/illuminate/adapter/adapter.py` & `illuminated-0.3.0/illuminate/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `illuminated-0.2.0/illuminate/cli.py` & `illuminated-0.3.0/illuminate/cli.py`

 * *Files identical despite different names*

### Comparing `illuminated-0.2.0/illuminate/common/project_logging.py` & `illuminated-0.3.0/illuminate/common/project_logging.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from illuminate import __version__
-
-LOGGING_LEVELS = (
-    "TRACE",
-    "DEBUG",
-    "INFO",
-    "SUCCESS",
-    "WARNING",
-    "ERROR",
-    "CRITICAL",
-)
-
-LOGO = f"""
-  ___ _     _    _   _ __  __ ___ _   _    _  _____ _____
- |_ _| |   | |  | | | |  \/  |_ _| \ | |  / \|_   _| ____|
-  | || |   | |  | | | | |\/| || ||  \| | / _ \ | | |  _|
-  | || |___| |__| |_| | |  | || || |\  |/ ___ \| | | |___
- |___|_____|_____\___/|_|  |_|___|_| \_/_/   \_\_| |_____|
-
-Version: {__version__}
-"""  # noqa:  W291, W605
-
-LOGO_COLOR = "239,242,201"
+from illuminate import __version__
+
+LOGGING_LEVELS = (
+    "TRACE",
+    "DEBUG",
+    "INFO",
+    "SUCCESS",
+    "WARNING",
+    "ERROR",
+    "CRITICAL",
+)
+
+LOGO = f"""
+  ___ _     _    _   _ __  __ ___ _   _    _  _____ _____
+ |_ _| |   | |  | | | |  \/  |_ _| \ | |  / \|_   _| ____|
+  | || |   | |  | | | | |\/| || ||  \| | / _ \ | | |  _|
+  | || |___| |__| |_| | |  | || || |\  |/ ___ \| | | |___
+ |___|_____|_____\___/|_|  |_|___|_| \_/_/   \_\_| |_____|
+
+Version: {__version__}
+"""  # noqa:  W291, W605
+
+LOGO_COLOR = "239,242,201"
```

### Comparing `illuminated-0.2.0/illuminate/common/project_templates.py` & `illuminated-0.3.0/illuminate/common/project_templates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 _ADAPTER_EXAMPLE = """
 from __future__ import annotations
 
 from collections.abc import AsyncGenerator
 from typing import Type, Union
 
 from illuminate.adapter import Adapter
+from illuminate.observation import FileObservation
 from illuminate.observation import HTTPObservation
+from illuminate.observation import SQLObservation
+from illuminate.observation import SplashObservation
 from illuminate.observer import Finding
 
-from exporters.example import ExporterExample
+from exporters.example import ExporterInfluxDBExample
+from exporters.example import ExporterSQLExample
 from findings.example import FindingExample
 from models.example import ModelExample
 
 
 class AdapterExample(Adapter):
     \"\"\"
     Adapter class is responsible for turning Finding objects into Exporter or
@@ -39,17 +43,41 @@
     \"\"\"
 
     priority: int = 10
     subscribers: tuple[Type[Finding]] = (FindingExample,)
 
     async def adapt(
         self, finding: FindingExample, *args, **kwargs
-    ) -> AsyncGenerator[Union[ExporterExample, HTTPObservation], None]:
-        yield ExporterExample(
-            models=[ModelExample(title=finding.title, url=finding.url)]
+    ) -> AsyncGenerator[
+        Union[
+            ExporterInfluxDBExample,
+            ExporterSQLExample,
+            FileObservation,
+            HTTPObservation,
+            SQLObservation,
+            SplashObservation,
+        ],
+        None,
+    ]:
+        yield ExporterSQLExample(
+            models=[
+                ModelExample(
+                    load_time=finding.load_time,
+                    title=finding.title,
+                    url=finding.url
+                )
+            ]
+        )
+
+        yield ExporterInfluxDBExample(
+            points={{
+                "measurement": "{name}",
+                "tags": {{"url": finding.url, "title": finding.title}},
+                "fields": {{"load_time": finding.load_time}},
+            }}
         )
 
 """
 
 _ALEMBIC_ENV_PY = """
 from pydoc import locate
 
@@ -129,14 +157,43 @@
     ${{downgrades if downgrades else "pass"}}
 
 """
 
 _DOCKER_COMPOSE = """
 version: '3.8'
 services:
+  grafana:
+   image: grafana/grafana
+   container_name: grafana
+   restart: always
+   depends_on:
+     - influxdb
+   environment:
+     - GF_SECURITY_ADMIN_USER=illuminate
+     - GF_SECURITY_ADMIN_PASSWORD=$ILLUMINATE_GRAFANA_PASSWORD
+     - GF_INSTALL_PLUGINS=
+   links:
+     - influxdb
+   ports:
+     - '3000:3000'
+   volumes:
+     - grafana:/var/lib/grafana
+  influxdb:
+    image: influxdb:1.8
+    container_name: influxdb
+    restart: always
+    environment:
+      - INFLUXDB_ADMIN_USER=illuminate
+      - INFLUXDB_ADMIN_PASSWORD=$ILLUMINATE_MEASUREMENTS_DB_PASSWORD
+      - INFLUXDB_DB={name}
+      - INFLUXDB_HTTP_AUTH_ENABLED=true
+    ports:
+      - '8086:8086'
+    volumes:
+      - influxdb:/var/lib/influxdb
   pg:
     container_name: pg
     image: postgres:latest
     restart: always
     environment:
       - POSTGRES_USER=illuminate
       - POSTGRES_PASSWORD=$ILLUMINATE_MAIN_DB_PASSWORD
@@ -157,33 +214,60 @@
   splash:
     container_name: splash
     image: scrapinghub/splash
     restart: always
     ports:
       - "8050:8050"
 volumes:
+  grafana:
+    driver: local
+  influxdb:
+    driver: local
   postgres:
     driver: local
 
 """
 
 _EMPTY = """
 """
 
 _EXPORTER_EXAMPLE = """
 from __future__ import annotations
 
-from typing import Union
+from typing import Iterable, Union
 
+from illuminate.exporter import InfluxDBExporter
 from illuminate.exporter import SQLExporter
+from pandas import DataFrame
 
 from models.example import ModelExample
 
 
-class ExporterExample(SQLExporter):
+class ExporterInfluxDBExample(InfluxDBExporter):
+    \"\"\"
+    InfluxDBExporter class will write points to database using session. Points
+    are passed at initialization, while database session is found by name
+    attribute in the pool of existing sessions. Name must co-respond to DB
+    section in {name}/settings.py. For more information how to initialize
+    InfluxDBExporter class, check {name}/adapters/example.py
+    \"\"\"
+
+    name: str = "measurements"
+
+    def __init__(
+        self,
+        points: Union[
+            Union[DataFrame, dict, str, bytes],
+            Iterable[Union[DataFrame, dict, str, bytes]],
+        ],
+    ):
+        super().__init__(points)
+
+
+class ExporterSQLExample(SQLExporter):
     \"\"\"
     SQLExporter class will commit models to database using session. Models are
     passed at initialization, while database session is found by name attribute
     in the pool of existing sessions. Name must co-respond to DB section in
     {name}/settings.py. For more information how to initialize SQLExporter
     class, check {name}/adapters/example.py
     \"\"\"
@@ -197,18 +281,20 @@
 
 _FIXTURE_EXAMPLE = """
 [
     {{
     "name": "{name}",
     "data": [
         {{
+            "load_time": "1.0",
             "url": "https://webscraper.io/",
             "title": "Web Scraper - The #1 web scraping extension"
         }},
         {{
+            "load_time": "1.0",
             "url": "https://webscraper.io/tutorials",
             "title": "Web Scraper Tutorials"
         }}
     ]
     }}
 ]
 """
@@ -217,33 +303,37 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 
 """
 
 _MODEL_EXAMPLE = """
-from sqlalchemy import Column, Integer, String
+from sqlalchemy import Column, Float, Integer, String
 
 from models import Base
 
 
 class ModelExample(Base):
     \"\"\"
     SQLAlchemy model used by SQLExporter object. For more information about
     SQLExporter class check {name}/exporters/example.py.
     \"\"\"
 
     __tablename__ = "{name}"
     id: int = Column(Integer, primary_key=True)
+    load_time: float = Column(Float)
     title: str = Column(String)
     url: str = Column(String)
 
     def __repr__(self):
         \"\"\"ModelExample's __repr__ method.\"\"\"
-        return f'ModelExample(title="{{self.title}}",url="{{self.url}}")'
+        return (
+            f'ModelExample(load_time={{self.load_time}},'
+            f'title="{{self.title}}",url="{{self.url}}")'
+        )
 
 """
 
 _ILLUMINATE_SETTINGS = """
 \"\"\"
 This file represents project {name}'s settings. It will be imported by a
 framework and used to configure run. The sections are as following:
@@ -282,15 +372,22 @@
 DB = {{
     "main": {{
         "host": "localhost",
         "pass": os.environ.get("ILLUMINATE_MAIN_DB_PASSWORD"),
         "port": "5432",
         "user": "illuminate",
         "type": "postgresql",
-    }}
+    }},
+    "measurements": {{
+        "host": "localhost",
+        "pass": os.environ.get("ILLUMINATE_MEASUREMENTS_DB_PASSWORD"),
+        "port": "8086",
+        "user": "illuminate",
+        "type": "influxdb",
+    }},
 }}
 
 MODELS = [
     "models.example.ModelExample",
 ]
 
 NAME = "{name}"
@@ -334,14 +431,15 @@
     Finding is a data class, meant to hold raw data extracted by Observation's
     callback. Finding will be passed to Adapter object's adapt method if
     it is subscribed to Adapter.
 
     Check {name}/adapters/example.py to learn more about subscription.
     \"\"\"
 
+    load_time: float = field()
     title: str = field()
     url: str = field()
 
 """
 
 _OBSERVER_EXAMPLE = """
 from __future__ import annotations
@@ -353,15 +451,16 @@
 
 from bs4 import BeautifulSoup
 from illuminate.manager import Manager
 from illuminate.observation import HTTPObservation
 from illuminate.observer import Observer
 from tornado.httpclient import HTTPResponse
 
-from exporters.example import ExporterExample
+from exporters.example import ExporterInfluxDBExample
+from exporters.example import ExporterSQLExample
 from findings.example import FindingExample
 
 
 def _create_soup(response: HTTPResponse) -> BeautifulSoup:
     html = response.body.decode(errors="ignore")
     soup = BeautifulSoup(html, "html.parser")
     return soup
@@ -421,15 +520,21 @@
                 callback=self.observe,
             ),
         ]
 
     async def observe(
         self, response: HTTPResponse, *args, **kwargs
     ) -> AsyncGenerator[
-        Union[ExporterExample, FindingExample, HTTPObservation], None
+        Union[
+            ExporterInfluxDBExample,
+            ExporterSQLExample,
+            FindingExample,
+            HTTPObservation,
+        ],
+        None,
     ]:
         \"\"\"
         ETL flow is regulated by a yielded object type of Observation's
         callback method. Each object type corresponds to ETL stage:
 
         * Observation -> Extract
         * Finding -> Transform
@@ -458,15 +563,19 @@
         hrefs = _extract_hrefs(soup, response.effective_url)
         for href in hrefs:
             yield HTTPObservation(
                 href,
                 allowed=self.ALLOWED,
                 callback=self.observe,
             )
-        yield FindingExample(soup.title.text, response.effective_url)
+        yield FindingExample(
+            response.request_time,
+            soup.title.text,
+            response.effective_url
+        )
 
 """
 
 FILES = {
     "docker-compose.yaml": _DOCKER_COMPOSE,
     "settings.py": _ILLUMINATE_SETTINGS,
     "adapters/__init__.py": _EMPTY,
```

### Comparing `illuminated-0.2.0/illuminate/decorators/logging.py` & `illuminated-0.3.0/illuminate/decorators/logging.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-from __future__ import annotations
-
-import functools
-from pydoc import locate
-from timeit import default_timer
-from typing import Callable, TYPE_CHECKING
-
-from loguru import logger
-
-from illuminate.common import LOGO
-from illuminate.common import LOGO_COLOR
-
-if TYPE_CHECKING:
-    from illuminate.manager import Manager
-
-
-def show_info(func: Callable) -> Callable:
-    """
-    Displays ETL process information.
-
-    :param func: Manager's public method
-    :return: Manager's public method wrapper
-    """
-
-    @functools.wraps(func)
-    def wrapper(self: Manager) -> None:
-        """
-        Displays ETL process information.
-
-        :param self: Manager object
-        :return: None
-        """
-        logger.info("Process started")
-        start = default_timer()
-        log_context(self)
-        log_settings(self)
-        func(self)
-        end = default_timer() - start
-        log_results(self)
-        logger.opt(colors=True).info(
-            f"Process finished in <yellow>{end:.2f}</yellow> seconds"
-        )
-
-    def log_context(self: Manager) -> None:
-        """
-        Displays ETL context information.
-
-        :param self: Manager object
-        :return: None
-        """
-        logger.opt(colors=True).info(
-            f"Project files for project "
-            f"<yellow>{self.name}</yellow> loaded into context"
-        )
-        logger.info(f"Adapters discovered {[i for i in self.adapters]}")
-        logger.info(
-            f"Models discovered {[locate(i) for i in self.settings.MODELS]}"
-        )
-        logger.info(f"Observers discovered {[i for i in self.observers]}")
-
-    def log_results(self: Manager) -> None:
-        """
-        Displays ETL results information.
-
-        :param self: Manager object
-        :return: None
-        """
-        logger.success("Results gathered")
-        logger.opt(colors=True).info(
-            f"<yellow>Unsuccessful</yellow> observations: "
-            f"<magenta>{len(self.not_observed)}</magenta>"
-        )
-        logger.debug(f"Unsuccessful attempts {self.not_observed}")
-        logger.opt(colors=True).info(
-            f"<yellow>Successful</yellow> observations: "
-            f"<magenta>{len(self.observed) - len(self.not_observed)}</magenta>"
-        )
-        logger.opt(colors=True).info(
-            f"Number of <yellow>exports</yellow>: "
-            f"<magenta>{len(self.exported)}</magenta>"
-        )
-
-    def log_settings(self: Manager) -> None:
-        """
-        Displays ETL settings information.
-
-        :param self: Manager object
-        :return: None
-        """
-        settings_conn = self.settings.CONCURRENCY
-        settings_db = self.settings.DB.copy()
-        for db in settings_db:
-            settings_db[db]["pass"] = "****"  # nosec
-        settings_obs = self.settings.OBSERVATION_CONFIGURATION.copy()
-        settings_obs["http"]["auth_password"] = "****"  # nosec
-        logger.debug(f"Concurrency settings {settings_conn}")
-        logger.debug(f"Database settings {settings_db}")
-        logger.debug(f"Observation settings {settings_obs}")
-
-    return wrapper
-
-
-def show_logo(func: Callable) -> Callable:
-    """
-    Displays framework's logo.
-
-    :param func: Manager's public method
-    :return: Manager's public method wrapper
-    """
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> None:
-        """
-        Displays framework's logo.
-
-        :return: None
-        """
-        logo = f"<fg {LOGO_COLOR}>{LOGO}</fg {LOGO_COLOR}>"
-        logger.opt(colors=True).success(logo)
-        func(*args, **kwargs)
-
-    return wrapper
-
-
-def show_observer_catalogue(func: Callable) -> Callable:
-    """
-    Displays Observers found in project files.
-
-    :param func: CLI's function
-    :return: CLI's function wrapper
-    """
-
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs) -> None:
-        """
-        Displays Observers found in project files.
-
-        :return: None
-        """
-        context = func(*args, **kwargs)
-        if not context["observers"]:
-            logger.info("No observers found")
-        outputs = []
-        for observer in context["observers"]:
-            _observer = observer()
-            _io = _observer.initial_observations
-            outputs.append(
-                f"<yellow>{_observer.__class__}</yellow> -> "
-                f"<cyan>{[(i.url, i._callback.__name__)for i in _io]}</cyan>"
-            )
-        for output in outputs:
-            logger.opt(colors=True).info(output)
-
-    return wrapper
+from __future__ import annotations
+
+import functools
+from pydoc import locate
+from timeit import default_timer
+from typing import Callable, TYPE_CHECKING
+
+from loguru import logger
+
+from illuminate.common import LOGO
+from illuminate.common import LOGO_COLOR
+
+if TYPE_CHECKING:
+    from illuminate.manager import Manager
+
+
+def show_info(func: Callable) -> Callable:
+    """
+    Displays ETL process information.
+
+    :param func: Manager's public method
+    :return: Manager's public method wrapper
+    """
+
+    @functools.wraps(func)
+    def wrapper(self: Manager) -> None:
+        """
+        Displays ETL process information.
+
+        :param self: Manager object
+        :return: None
+        """
+        logger.info("Process started")
+        start = default_timer()
+        log_context(self)
+        log_settings(self)
+        func(self)
+        end = default_timer() - start
+        log_results(self)
+        logger.opt(colors=True).info(
+            f"Process finished in <yellow>{end:.2f}</yellow> seconds"
+        )
+
+    def log_context(self: Manager) -> None:
+        """
+        Displays ETL context information.
+
+        :param self: Manager object
+        :return: None
+        """
+        logger.opt(colors=True).info(
+            f"Project files for project "
+            f"<yellow>{self.name}</yellow> loaded into context"
+        )
+        logger.info(f"Adapters discovered {[i for i in self.adapters]}")
+        logger.info(
+            f"Models discovered {[locate(i) for i in self.settings.MODELS]}"
+        )
+        logger.info(f"Observers discovered {[i for i in self.observers]}")
+
+    def log_results(self: Manager) -> None:
+        """
+        Displays ETL results information.
+
+        :param self: Manager object
+        :return: None
+        """
+        logger.success("Results gathered")
+        logger.opt(colors=True).info(
+            f"<yellow>Unsuccessful</yellow> observations: "
+            f"<magenta>{len(self.not_observed)}</magenta>"
+        )
+        logger.debug(f"Unsuccessful attempts {self.not_observed}")
+        logger.opt(colors=True).info(
+            f"<yellow>Successful</yellow> observations: "
+            f"<magenta>{len(self.observed) - len(self.not_observed)}</magenta>"
+        )
+        logger.opt(colors=True).info(
+            f"Number of <yellow>exports</yellow>: "
+            f"<magenta>{len(self.exported)}</magenta>"
+        )
+
+    def log_settings(self: Manager) -> None:
+        """
+        Displays ETL settings information.
+
+        :param self: Manager object
+        :return: None
+        """
+        settings_conn = self.settings.CONCURRENCY
+        settings_db = self.settings.DB.copy()
+        for db in settings_db:
+            settings_db[db]["pass"] = "****"  # nosec
+        settings_obs = self.settings.OBSERVATION_CONFIGURATION.copy()
+        settings_obs["http"]["auth_password"] = "****"  # nosec
+        logger.debug(f"Concurrency settings {settings_conn}")
+        logger.debug(f"Database settings {settings_db}")
+        logger.debug(f"Observation settings {settings_obs}")
+
+    return wrapper
+
+
+def show_logo(func: Callable) -> Callable:
+    """
+    Displays framework's logo.
+
+    :param func: Manager's public method
+    :return: Manager's public method wrapper
+    """
+
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs) -> None:
+        """
+        Displays framework's logo.
+
+        :return: None
+        """
+        logo = f"<fg {LOGO_COLOR}>{LOGO}</fg {LOGO_COLOR}>"
+        logger.opt(colors=True).success(logo)
+        func(*args, **kwargs)
+
+    return wrapper
+
+
+def show_observer_catalogue(func: Callable) -> Callable:
+    """
+    Displays Observers found in project files.
+
+    :param func: CLI's function
+    :return: CLI's function wrapper
+    """
+
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs) -> None:
+        """
+        Displays Observers found in project files.
+
+        :return: None
+        """
+        context = func(*args, **kwargs)
+        if not context["observers"]:
+            logger.info("No observers found")
+        outputs = []
+        for observer in context["observers"]:
+            _observer = observer()
+            _io = _observer.initial_observations
+            outputs.append(
+                f"<yellow>{_observer.__class__}</yellow> -> "
+                f"<cyan>{[(i.url, i._callback.__name__)for i in _io]}</cyan>"
+            )
+        for output in outputs:
+            logger.opt(colors=True).info(output)
+
+    return wrapper
```

### Comparing `illuminated-0.2.0/illuminate/exporter/exporter.py` & `illuminated-0.3.0/illuminate/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `illuminated-0.2.0/illuminate/exporter/sql.py` & `illuminated-0.3.0/illuminate/exporter/sql.py`

 * *Files identical despite different names*

### Comparing `illuminated-0.2.0/illuminate/interface/assistant.py` & `illuminated-0.3.0/illuminate/interface/assistant.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-class IAssistant:
-    """Interface for Assistant class."""
-
-    @staticmethod
-    def provide_alembic_config(path, selector, url):
-        """Creates Alembic's configuration object."""
-        raise NotImplementedError
-
-    @staticmethod
-    def provide_alembic_operations(selector, url):
-        """Creates Alembic's operations object."""
-        raise NotImplementedError
-
-    @staticmethod
-    def provide_context(sessions, _filter):
-        """Creates Manager's constructor kwargs."""
-        raise NotImplementedError
-
-    @staticmethod
-    def provide_models():
-        """Gathers project models."""
-        raise NotImplementedError
-
-    @staticmethod
-    def _provide_db_url(selector):
-        """Creates database URL."""
-        raise NotImplementedError
-
-    @staticmethod
-    def _provide_sessions():
-        """Creates a dictionary of database sessions."""
-        raise NotImplementedError
-
-    @staticmethod
-    def _provide_settings():
-        """Imports project's settings.py module and returns it."""
-        raise NotImplementedError
+class IAssistant:
+    """Interface for Assistant class."""
+
+    @staticmethod
+    def provide_alembic_config(path, selector, url):
+        """Creates Alembic's configuration object."""
+        raise NotImplementedError
+
+    @staticmethod
+    def provide_alembic_operations(selector, url):
+        """Creates Alembic's operations object."""
+        raise NotImplementedError
+
+    @staticmethod
+    def provide_context(sessions, _filter):
+        """Creates Manager's constructor kwargs."""
+        raise NotImplementedError
+
+    @staticmethod
+    def provide_models():
+        """Gathers project models."""
+        raise NotImplementedError
+
+    @staticmethod
+    def _provide_db_url(selector):
+        """Creates database URL."""
+        raise NotImplementedError
+
+    @staticmethod
+    def _provide_sessions():
+        """Creates a dictionary of database sessions."""
+        raise NotImplementedError
+
+    @staticmethod
+    def _provide_settings():
+        """Imports project's settings.py module and returns it."""
+        raise NotImplementedError
```

### Comparing `illuminated-0.2.0/illuminate/interface/manager.py` & `illuminated-0.3.0/illuminate/interface/manager.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-class IManager:
-    """Interface for Manager class."""
-
-    @staticmethod
-    def db_populate(fixtures, models, operations, selector):
-        """Populates database with fixtures."""
-        raise NotImplementedError
-
-    @staticmethod
-    def db_revision(config, revision):
-        """Creates Alembic's revision file in migration directory."""
-        raise NotImplementedError
-
-    @staticmethod
-    def db_upgrade(config, revision, selector):
-        """Applies migration file to a database."""
-        raise NotImplementedError
-
-    @staticmethod
-    def project_setup(name, path):
-        """Creates a project directory with all needed files."""
-        raise NotImplementedError
-
-    def observe_start(self):
-        """Starts producer/consumer ETL process."""
-        raise NotImplementedError
+class IManager:
+    """Interface for Manager class."""
+
+    @staticmethod
+    def db_populate(fixtures, models, operations, selector):
+        """Populates database with fixtures."""
+        raise NotImplementedError
+
+    @staticmethod
+    def db_revision(config, revision):
+        """Creates Alembic's revision file in migration directory."""
+        raise NotImplementedError
+
+    @staticmethod
+    def db_upgrade(config, revision, selector):
+        """Applies migration file to a database."""
+        raise NotImplementedError
+
+    @staticmethod
+    def project_setup(name, path):
+        """Creates a project directory with all needed files."""
+        raise NotImplementedError
+
+    def observe_start(self):
+        """Starts producer/consumer ETL process."""
+        raise NotImplementedError
```

### Comparing `illuminated-0.2.0/illuminate/manager/assistant.py` & `illuminated-0.3.0/illuminate/manager/assistant.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import inspect
 import os
 import sys
 from pydoc import locate
 from types import ModuleType
 from typing import Optional, Type, Union
 
+from aioinflux import InfluxDBClient  # type: ignore
 from alembic.config import Config
 from alembic.migration import MigrationContext
 from alembic.operations import Operations
 from loguru import logger
 from sqlalchemy import create_engine
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy.orm import sessionmaker
 
 from illuminate.adapter import Adapter
-from illuminate.common import SUPPORTED_RELATIONAL_DATABASES
+from illuminate.common import SUPPORTED_NOSQL_DATABASES
+from illuminate.common import SUPPORTED_SQL_DATABASES
 from illuminate.exceptions import BasicManagerException
 from illuminate.interface import IAssistant
 from illuminate.observer import Observer
 
 
 class Assistant(IAssistant):
     """
@@ -177,42 +179,35 @@
             return "{type}+{driver}://{user}:{pass}@{host}/{db}".format(
                 driver=driver, **db
             )
 
         return "{type}://{user}:{pass}@{host}/{db}".format(**db)
 
     @staticmethod
-    def _provide_sessions() -> dict[str, Type[AsyncSession]]:
+    def _provide_sessions() -> dict[
+        str, Union[Type[AsyncSession], InfluxDBClient]
+    ]:
         """
         Creates a dictionary of database sessions.
 
-        :return: Database sessions
+        :return: Database sessions dictionary
         """
         _sessions: dict = {}
         settings = Assistant._provide_settings()
         logger.opt(colors=True).info(
             f"Number of expected db connections: "
             f"<yellow>{len(settings.DB)}</yellow>"
         )
         for db in settings.DB:
             _type = settings.DB[db]["type"]
-            if _type in SUPPORTED_RELATIONAL_DATABASES:
-                url = Assistant._provide_db_url(db, _async=True)
-                engine = create_async_engine(url)
-                session = sessionmaker(
-                    engine,
-                    class_=AsyncSession,
-                    expire_on_commit=False,
-                )
-                host = settings.DB[db]["host"]
-                port = settings.DB[db]["port"]
-                logger.opt(colors=True).info(
-                    f"Adding session with <yellow>{db}</yellow> at "
-                    f"<magenta>{host}:{port}</magenta> to context"
-                )
+            if _type in SUPPORTED_NOSQL_DATABASES:
+                session = Assistant.__provide_nosql_sessions(db, settings)
+                _sessions.update({db: session})
+            elif _type in SUPPORTED_SQL_DATABASES:
+                session = Assistant.__provide_sql_sessions(db, settings)
                 _sessions.update({db: session})
             else:
                 logger.warning(f"Database type {_type} is not supported")
 
         return _sessions
 
     @staticmethod
@@ -227,7 +222,62 @@
             import settings  # type: ignore
 
             return settings
         except ImportError:
             raise BasicManagerException(
                 "Framework did not found settings.py in the current directory"
             )
+
+    @staticmethod
+    def __log_database_connection(db: str, settings: ModuleType) -> None:
+        """
+        Log database connection.
+
+        :param db: database name from settings.py module
+        :param settings: settings.py module
+        :return: None
+        """
+        host = settings.DB[db]["host"]
+        port = settings.DB[db]["port"]
+        logger.opt(colors=True).info(
+            f"Adding session with <yellow>{db}</yellow> at "
+            f"<magenta>{host}:{port}</magenta> to context"
+        )
+
+    @staticmethod
+    def __provide_nosql_sessions(
+        db: str, settings: ModuleType
+    ) -> InfluxDBClient:
+        """
+        Provides NoSQL database session.
+
+        :param db: database name from settings.py module
+        :param settings: settings.py module
+        :return: InfluxDBClient object
+        """
+        Assistant.__log_database_connection(db, settings)
+        if settings.DB[db]["type"] == "influxdb":
+            return InfluxDBClient(
+                host=settings.DB[db]["host"],
+                port=settings.DB[db]["port"],
+                db=settings.NAME,
+                username=settings.DB[db]["user"],
+                password=settings.DB[db]["pass"],
+            )
+
+    @staticmethod
+    def __provide_sql_sessions(
+        db: str, settings: ModuleType
+    ) -> sessionmaker[AsyncSession]:
+        """
+        Provides SQL database session.
+
+        :param db: database name from settings.py module
+        :param settings: settings.py module
+        :return: AsyncSession created with session maker
+        """
+        Assistant.__log_database_connection(db, settings)
+        return sessionmaker(
+            create_async_engine(Assistant._provide_db_url(db, _async=True)),
+            class_=AsyncSession,
+            expire_on_commit=False,
+        )
```

### Comparing `illuminated-0.2.0/illuminate/manager/manager.py` & `illuminated-0.3.0/illuminate/manager/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 import json
 import os
 import traceback
 from glob import glob
 from types import ModuleType
 from typing import Type, Union
 
+from aioinflux import InfluxDBClient  # type: ignore
 from alembic import command
 from alembic.config import Config
 from alembic.operations import Operations
 from loguru import logger
 from sqlalchemy.ext.asyncio import AsyncSession
 from tornado import gen, ioloop, queues
 
 from illuminate.adapter import Adapter
 from illuminate.common import FILES
 from illuminate.decorators import adapt
 from illuminate.decorators import show_info
 from illuminate.decorators import show_logo
 from illuminate.decorators import show_observer_catalogue
+from illuminate.exceptions import BasicExporterException
 from illuminate.exceptions import BasicManagerException
 from illuminate.exporter import Exporter
+from illuminate.exporter import InfluxDBExporter
 from illuminate.exporter import SQLExporter
 from illuminate.interface import IManager
 from illuminate.meta.type import Result
 from illuminate.observation import FileObservation
 from illuminate.observation import HTTPObservation
 from illuminate.observation import Observation
 from illuminate.observation import SQLObservation
@@ -47,15 +50,15 @@
 
     def __init__(
         self,
         adapters: list[Type[Adapter]],
         name: str,
         observers: list[Type[Observer]],
         path: str,
-        sessions: dict[str, Type[AsyncSession]],
+        sessions: dict[str, Union[Type[AsyncSession], InfluxDBClient]],
         settings: ModuleType,
         *args,
         **kwargs,
     ):
         """
         Manager's __init__ method.
 
@@ -305,41 +308,41 @@
         """
         Calls FileObservation's observe method and pass result to resolve
         function.
 
         :param item: FileObservation object
         :return: None
         """
-        async with item.observe() as result:
+        async with item.observe(xcom=item.xcom) as result:
             await self.__observation_resolve(result, item.url)
 
     async def __observe_http(self, item: HTTPObservation) -> None:
         """
         Prepares HTTPObservation configuration, calls observe method and pass
         result to resolve function.
 
         :param item: HTTPObservation object
         :return: None
         """
         item.configuration = {
             **self.settings.OBSERVATION_CONFIGURATION["http"],
             **item.configuration,
         }
-        result = await item.observe()
+        result = await item.observe(xcom=item.xcom)
         await self.__observation_resolve(result, item.url)
 
     async def __observe_sql(self, item: SQLObservation) -> None:
         """
         Calls SQLObservation's observe method and pass result to resolve
         function.
 
         :param item: SQLObservation object
         :return: None
         """
-        result = await item.observe(self.sessions[item.url])
+        result = await item.observe(self.sessions[item.url], xcom=item.xcom)
         await self.__observation_resolve(result, f"{item.url}:{item.query}")
 
     async def __observe_splash(self, item: SplashObservation) -> None:
         """
         Prepares SplashObservation configuration, calls observe method and pass
         result to resolve function.
 
@@ -347,15 +350,15 @@
         :return: None
         """
         item.configuration = {
             **self.settings.OBSERVATION_CONFIGURATION["splash"],
             **item.configuration,
         }
         result = await item.observe(
-            self.settings.OBSERVATION_CONFIGURATION["http"]
+            self.settings.OBSERVATION_CONFIGURATION["http"], xcom=item.xcom
         )
         await self.__observation_resolve(result, item.url)
 
     async def __observation_resolve(
         self, result: Union[None, Result], url: str
     ):
         """
@@ -439,41 +442,45 @@
         self.__exportation method.
 
         :return: None
         """
         async for item in self.__export_queue:
             if not item:
                 return
-            await self.__exportation(item)
+            await self.__export_to(item)
             logger.debug(f"Coroutine exported {item}")
             del item
             self.__export_queue.task_done()
 
-    async def __exportation(self, item: Exporter) -> None:
+    async def __export_to(self, item: Exporter) -> None:
         """
         Passes Exporter object to proper method based on its class.
 
         :param item: Exporter object
         :return: None
         """
-        if isinstance(item, SQLExporter):
-            await self.__exportation_sql(item)
+        if isinstance(item, (InfluxDBExporter, SQLExporter)):
+            await self.__export_to_database(item)
 
-    async def __exportation_sql(self, item: SQLExporter) -> None:
+    async def __export_to_database(
+        self, item: Union[InfluxDBExporter, SQLExporter]
+    ) -> None:
         """
         Acquires database session based on Exporter's attributes and pass it to
-        SQLExporter's export method.
+        Exporter's export method.
 
-        :param item: SQLExporter object
+        :param item: InfluxDBExporter or SQLExporter object
         :return: None
         """
         try:
             session = self.sessions[item.name]
             await item.export(session)
             self.__exported.add(item)
+        except BasicExporterException:
+            pass
         except KeyError:
             logger.critical(f"Database {item.name} of is not found in context")
 
     @logger.catch
     async def _observe_start(self) -> None:
         """
         Starts producer/consumer ETL process.
@@ -501,7 +508,11 @@
             await self.__adapt_queue.put(None)
         for _ in range(_exporters):
             await self.__export_queue.put(None)
 
         await observers
         await adapters
         await exporters
+
+        for session in self.sessions:
+            if isinstance(self.sessions[session], InfluxDBClient):
+                await self.sessions[session].close()  # type: ignore
```

### Comparing `illuminated-0.2.0/illuminate/observation/file.py` & `illuminated-0.3.0/illuminate/observation/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-from __future__ import annotations
-
-from collections.abc import AsyncIterator
-from contextlib import AsyncExitStack, asynccontextmanager
-from typing import Callable, Union
-
-from aiofile import async_open
-from aiofile.utils import FileIOWrapperBase
-from caio import thread_aio_asyncio
-from loguru import logger
-
-from illuminate.meta.type import Result
-from illuminate.observation import Observation
-
-
-class FileObservation(Observation):
-    """
-    FileObservation class, reads file content asynchronously. Inherits
-    Observation class and implements observe method.
-    """
-
-    def __hash__(self) -> int:
-        """
-        FileObservation object hash value.
-
-        :return: int
-        """
-        return hash(self.url)
-
-    def __init__(
-        self,
-        url: str,
-        /,
-        callback: Callable[[FileIOWrapperBase, tuple, dict], Result],
-        *args,
-        **kwargs,
-    ):
-        """
-        FileObservation's __init__ method.
-
-        :param url: File path
-        :param callback: Async function/method that manipulates
-        FileIOWrapperBase object and returns Result
-        """
-        super().__init__(url)
-        self._callback = callback
-
-    @asynccontextmanager
-    async def observe(
-        self, *args, **kwargs
-    ) -> AsyncIterator[Union[None, Result]]:
-        """
-        Opens IO file stream asynchronously, pass stream object to a callback
-        and returns None or Result as a context manager.
-
-        :return: AsyncIterator with None or Result
-        """
-        _file = None
-        _items = None
-        async with AsyncExitStack() as stack:
-            context = await stack.enter_async_context(
-                thread_aio_asyncio.AsyncioContext()
-            )
-            try:
-                _file = await stack.enter_async_context(
-                    async_open(self.url, "r", context=context)
-                )
-                logger.info(f"{self}.observe() -> {_file}")
-                _items = self._callback(_file, *args, **kwargs)
-            except FileNotFoundError as exception:
-                logger.warning(f"{self}.observe() -> {exception}")
-            except Exception as exception:
-                logger.critical(f"{self}.observe() -> {exception}")
-            finally:
-                yield _items
-                if _file:
-                    await _file.close()
-
-    def __repr__(self):
-        """
-        FileObservation's __repr__ method.
-
-        :return: String representation of an instance
-        """
-        return f'FileObservation("{self.url}",callback="{self._callback}")'
+from __future__ import annotations
+
+from collections.abc import AsyncIterator
+from contextlib import AsyncExitStack, asynccontextmanager
+from typing import Any, Callable, Optional, Union
+
+from aiofile import async_open
+from aiofile.utils import FileIOWrapperBase
+from caio import thread_aio_asyncio
+from loguru import logger
+
+from illuminate.meta.type import Result
+from illuminate.observation import Observation
+
+
+class FileObservation(Observation):
+    """
+    FileObservation class, reads file content asynchronously. Inherits
+    Observation class and implements observe method.
+    """
+
+    def __hash__(self) -> int:
+        """
+        FileObservation object hash value.
+
+        :return: int
+        """
+        return hash(self.url)
+
+    def __init__(
+        self,
+        url: str,
+        /,
+        callback: Callable[[FileIOWrapperBase, tuple, dict], Result],
+        xcom: Optional[Any] = None,
+        *args,
+        **kwargs,
+    ):
+        """
+        FileObservation's __init__ method.
+
+        :param url: File path
+        :param callback: Async function/method that manipulates
+        FileIOWrapperBase object and returns Result
+        :param xcom: Cross communication object
+        """
+        super().__init__(url, xcom=xcom)
+        self._callback = callback
+
+    @asynccontextmanager
+    async def observe(
+        self, *args, **kwargs
+    ) -> AsyncIterator[Union[None, Result]]:
+        """
+        Opens IO file stream asynchronously, pass stream object to a callback
+        and returns None or Result as a context manager.
+
+        :return: AsyncIterator with None or Result
+        """
+        _file = None
+        _items = None
+        async with AsyncExitStack() as stack:
+            context = await stack.enter_async_context(
+                thread_aio_asyncio.AsyncioContext()
+            )
+            try:
+                _file = await stack.enter_async_context(
+                    async_open(self.url, "r", context=context)
+                )
+                logger.info(f"{self}.observe() -> {_file}")
+                _items = self._callback(_file, *args, **kwargs)
+            except FileNotFoundError as exception:
+                logger.warning(f"{self}.observe() -> {exception}")
+            except Exception as exception:
+                logger.critical(f"{self}.observe() -> {exception}")
+            finally:
+                yield _items
+                if _file:
+                    await _file.close()
+
+    def __repr__(self):
+        """
+        FileObservation's __repr__ method.
+
+        :return: String representation of an instance
+        """
+        return f'FileObservation("{self.url}",callback="{self._callback}")'
```

### Comparing `illuminated-0.2.0/illuminate/observation/http.py` & `illuminated-0.3.0/illuminate/observation/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,169 +1,171 @@
-from __future__ import annotations
-
-import urllib.parse
-from copy import copy
-from typing import Callable, Union
-
-from loguru import logger
-from tornado import httpclient
-from tornado.httpclient import HTTPClientError
-from tornado.httpclient import HTTPResponse
-
-from illuminate.meta.type import Result
-from illuminate.observation import Observation
-
-
-class HTTPObservation(Observation):
-    """
-    HTTPObservation class, reads data from HTTP server asynchronously. Inherits
-    Observation class and implements observe method.
-    """
-
-    def __hash__(self) -> int:
-        """
-        HTTPObservation object hash value.
-
-        :return: int
-        """
-        body = self.configuration.get("body")
-        method = self.configuration.get("method")
-        return hash(f"{method}|{self.url}|:{body}")
-
-    def __init__(
-        self,
-        url: str,
-        /,
-        allowed: Union[list[str], tuple[str]],
-        callback: Callable[[HTTPResponse, tuple, dict], Result],
-        *args,
-        **kwargs,
-    ):
-        """
-        HTTPObservation's __init__ method.
-
-        :param url: Data's HTTP URL
-        :param allowed: Collection of strings evaluated against self.url to
-        determent if URL is allowed
-        :param callback: Async function/method that manipulates HTTPResponse
-        object and returns Result.
-        """
-        super().__init__(url)
-        self._allowed = allowed
-        self._callback = callback
-        self.configuration = kwargs
-
-    @property
-    def allowed(self) -> bool:
-        """
-        Checks if HTTP URL is allowed to be requested.
-
-        :return: bool
-        """
-        for allowed in self._allowed:
-            if self.url.startswith(allowed):
-                return True
-        return False
-
-    async def observe(self, *args, **kwargs) -> Union[None, Result]:
-        """
-        Requests data from HTTP server, passes response object to a callback
-        and returns None or Result.
-
-        :return: None or Result
-        """
-        try:
-            response = await httpclient.AsyncHTTPClient().fetch(
-                self.url, **self.configuration
-            )
-            logger.info(f"{self}.observe() -> {response}")
-            return self._callback(response, *args, **kwargs)
-        except HTTPClientError as exception:
-            logger.warning(f"{self}.observe() -> {exception}")
-            return None
-        except Exception as exception:
-            logger.critical(f"{self}.observe() -> {exception}")
-            return None
-
-    def __repr__(self):
-        """
-        HTTPObservation's __repr__ method.
-
-        :return: String representation of an instance
-        """
-        return f'HTTPObservation("{self.url}",callback="{self._callback}")'
-
-
-class SplashObservation(HTTPObservation):
-    """
-    SplashObservation class, reads data from HTTP server asynchronously.
-    Inherits HTTPObservation class and implements observe method.
-
-    Constructor's kwargs are used to create Splash service URL. For full list
-    of parameters visit https://splash.readthedocs.io/en/stable/api.html.
-
-    Note: URL is passed as positional argument. It will be used as param
-    in Splash service URL.
-    """
-
-    def __hash__(self) -> int:
-        """
-        SplashObservation object hash value.
-
-        :return: int
-        """
-        return hash(self.service)
-
-    @property
-    def service(self):
-        """
-        Constructs URL of Splash service
-
-        :return: Splash URL string
-        """
-        defaults: dict = {
-            "host": "localhost",
-            "port": 8050,
-            "protocol": "http",
-            "render": "html",
-        }
-        parameters = copy(self.configuration)
-        for i in defaults:
-            if i in parameters:
-                defaults[i] = parameters[i]
-                del parameters[i]
-        parameters["url"] = self.url
-        endpoint = "{protocol}://{host}:{port}/render.{render}?"
-        endpoint = endpoint.format(**defaults)
-        parameters = urllib.parse.urlencode(parameters)
-        return f"{endpoint.format(**defaults)}{parameters}"
-
-    async def observe(
-        self, configuration: dict, *args, **kwargs
-    ) -> Union[None, Result]:
-        """
-        Requests data from HTTP server and renders response with Splash, passes
-        response object to a callback and returns None or Result.
-
-        :param configuration: HTTP configuration dict from settings.py
-        :return: None or Result
-        """
-        try:
-            response = await httpclient.AsyncHTTPClient().fetch(
-                self.service, **configuration
-            )
-            logger.info(f"{self}.observe() -> {response}")
-            return self._callback(response, *args, **kwargs)
-        except HTTPClientError as exception:
-            logger.warning(f"{self}.observe() -> {exception}")
-            return None
-        except Exception as exception:
-            logger.critical(f"{self}.observe() -> {exception}")
-            return None
-
-    def __repr__(self):
-        """
-        SplashObservation's __repr__ method.
-
-        :return: String representation of an instance
-        """
-        return f'SplashObservation("{self.url}",callback="{self._callback}")'
+from __future__ import annotations
+
+import urllib.parse
+from copy import copy
+from typing import Any, Callable, Optional, Union
+
+from loguru import logger
+from tornado import httpclient
+from tornado.httpclient import HTTPClientError
+from tornado.httpclient import HTTPResponse
+
+from illuminate.meta.type import Result
+from illuminate.observation import Observation
+
+
+class HTTPObservation(Observation):
+    """
+    HTTPObservation class, reads data from HTTP server asynchronously. Inherits
+    Observation class and implements observe method.
+    """
+
+    def __hash__(self) -> int:
+        """
+        HTTPObservation object hash value.
+
+        :return: int
+        """
+        body = self.configuration.get("body")
+        method = self.configuration.get("method")
+        return hash(f"{method}|{self.url}|:{body}")
+
+    def __init__(
+        self,
+        url: str,
+        /,
+        allowed: Union[list[str], tuple[str]],
+        callback: Callable[[HTTPResponse, tuple, dict], Result],
+        xcom: Optional[Any] = None,
+        *args,
+        **kwargs,
+    ):
+        """
+        HTTPObservation's __init__ method.
+
+        :param url: Data's HTTP URL
+        :param allowed: Collection of strings evaluated against self.url to
+        determent if URL is allowed
+        :param callback: Async function/method that manipulates HTTPResponse
+        object and returns Result.
+        :param xcom: Cross communication object
+        """
+        super().__init__(url, xcom=xcom)
+        self._allowed = allowed
+        self._callback = callback
+        self.configuration = kwargs
+
+    @property
+    def allowed(self) -> bool:
+        """
+        Checks if HTTP URL is allowed to be requested.
+
+        :return: bool
+        """
+        for allowed in self._allowed:
+            if self.url.startswith(allowed):
+                return True
+        return False
+
+    async def observe(self, *args, **kwargs) -> Union[None, Result]:
+        """
+        Requests data from HTTP server, passes response object to a callback
+        and returns None or Result.
+
+        :return: None or Result
+        """
+        try:
+            response = await httpclient.AsyncHTTPClient().fetch(
+                self.url, **self.configuration
+            )
+            logger.info(f"{self}.observe() -> {response}")
+            return self._callback(response, *args, **kwargs)
+        except HTTPClientError as exception:
+            logger.warning(f"{self}.observe() -> {exception}")
+            return None
+        except Exception as exception:
+            logger.critical(f"{self}.observe() -> {exception}")
+            return None
+
+    def __repr__(self):
+        """
+        HTTPObservation's __repr__ method.
+
+        :return: String representation of an instance
+        """
+        return f'HTTPObservation("{self.url}",callback="{self._callback}")'
+
+
+class SplashObservation(HTTPObservation):
+    """
+    SplashObservation class, reads data from HTTP server asynchronously.
+    Inherits HTTPObservation class and implements observe method.
+
+    Constructor's kwargs are used to create Splash service URL. For full list
+    of parameters visit https://splash.readthedocs.io/en/stable/api.html.
+
+    Note: URL is passed as positional argument. It will be used as param
+    in Splash service URL.
+    """
+
+    def __hash__(self) -> int:
+        """
+        SplashObservation object hash value.
+
+        :return: int
+        """
+        return hash(self.service)
+
+    @property
+    def service(self):
+        """
+        Constructs URL of Splash service
+
+        :return: Splash URL string
+        """
+        defaults: dict = {
+            "host": "localhost",
+            "port": 8050,
+            "protocol": "http",
+            "render": "html",
+        }
+        parameters = copy(self.configuration)
+        for i in defaults:
+            if i in parameters:
+                defaults[i] = parameters[i]
+                del parameters[i]
+        parameters["url"] = self.url
+        endpoint = "{protocol}://{host}:{port}/render.{render}?"
+        endpoint = endpoint.format(**defaults)
+        parameters = urllib.parse.urlencode(parameters)
+        return f"{endpoint.format(**defaults)}{parameters}"
+
+    async def observe(
+        self, configuration: dict, *args, **kwargs
+    ) -> Union[None, Result]:
+        """
+        Requests data from HTTP server and renders response with Splash, passes
+        response object to a callback and returns None or Result.
+
+        :param configuration: HTTP configuration dict from settings.py
+        :return: None or Result
+        """
+        try:
+            response = await httpclient.AsyncHTTPClient().fetch(
+                self.service, **configuration
+            )
+            logger.info(f"{self}.observe() -> {response}")
+            return self._callback(response, *args, **kwargs)
+        except HTTPClientError as exception:
+            logger.warning(f"{self}.observe() -> {exception}")
+            return None
+        except Exception as exception:
+            logger.critical(f"{self}.observe() -> {exception}")
+            return None
+
+    def __repr__(self):
+        """
+        SplashObservation's __repr__ method.
+
+        :return: String representation of an instance
+        """
+        return f'SplashObservation("{self.url}",callback="{self._callback}")'
```

### Comparing `illuminated-0.2.0/illuminate/observation/sql.py` & `illuminated-0.3.0/illuminate/observation/sql.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-from __future__ import annotations
-
-from typing import Callable, Type, Union
-
-from loguru import logger
-from sqlalchemy.engine.result import Result as AlchemyResult
-from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.ext.asyncio import AsyncSession
-from sqlalchemy.sql.elements import TextClause
-from sqlalchemy.sql.selectable import Select
-
-from illuminate.meta.type import Result
-from illuminate.observation import Observation
-
-
-class SQLObservation(Observation):
-    """
-    SQLObservation class, reads data from database asynchronously. Inherits
-    Observation class and implements observe method.
-    """
-
-    def __hash__(self) -> int:
-        """
-        SQLObservation object hash value.
-
-        :return: int
-        """
-        query = str(self.query)
-        return hash(f"{self.url}|:{query}")
-
-    def __init__(
-        self,
-        query: Union[Select, TextClause],
-        url: str,
-        /,
-        callback: Callable[[AlchemyResult, tuple, dict], Result],
-        *args,
-        **kwargs,
-    ):
-        """
-        SQLObservation's __init__ method.
-
-        :param query: SQLAlchemy query object.
-        :param url: Database name in project settings.
-        :param callback: Async function/method that manipulates AlchemyResult
-        object and returns Result.
-        """
-        super().__init__(url)
-        self._callback = callback
-        self.query = query
-
-    async def observe(
-        self, session: Type[AsyncSession], *args, **kwargs
-    ) -> Union[None, Result]:
-        """
-        Reads data from database, passes response object to a callback
-        and returns None or Result.
-
-        :return: None or Result
-        """
-        try:
-            async with session() as session:  # type: ignore
-                async with session.begin():  # type: ignore
-                    query = self.query
-                    response = await session.execute(query)  # type: ignore
-            logger.info(f'{self}.observe(session="{session}")')
-            return self._callback(response, *args, **kwargs)
-        except SQLAlchemyError as exception:
-            logger.warning(f"{self}.observe() -> {exception}")
-            return None
-        except Exception as exception:
-            logger.critical(f"{self}.observe() -> {exception}")
-            return None
-
-    def __repr__(self):
-        """
-        SQLObservation's __repr__ method.
-
-        :return: String representation of an instance
-        """
-        return (
-            f'SQLObservation("{self.query}","{self.url}",'
-            f'callback="{self._callback}")'
-        )
+from __future__ import annotations
+
+from typing import Any, Callable, Optional, Type, Union
+
+from loguru import logger
+from sqlalchemy.engine.result import Result as AlchemyResult
+from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy.sql.elements import TextClause
+from sqlalchemy.sql.selectable import Select
+
+from illuminate.meta.type import Result
+from illuminate.observation import Observation
+
+
+class SQLObservation(Observation):
+    """
+    SQLObservation class, reads data from database asynchronously. Inherits
+    Observation class and implements observe method.
+    """
+
+    def __hash__(self) -> int:
+        """
+        SQLObservation object hash value.
+
+        :return: int
+        """
+        query = str(self.query)
+        return hash(f"{self.url}|:{query}")
+
+    def __init__(
+        self,
+        query: Union[Select, TextClause],
+        url: str,
+        /,
+        callback: Callable[[AlchemyResult, tuple, dict], Result],
+        xcom: Optional[Any] = None,
+        *args,
+        **kwargs,
+    ):
+        """
+        SQLObservation's __init__ method.
+
+        :param query: SQLAlchemy query object.
+        :param url: Database name in project settings.
+        :param callback: Async function/method that manipulates AlchemyResult
+        object and returns Result.
+        :param xcom: Cross communication object
+        """
+        super().__init__(url, xcom=xcom)
+        self._callback = callback
+        self.query = query
+
+    async def observe(
+        self, session: Type[AsyncSession], *args, **kwargs
+    ) -> Union[None, Result]:
+        """
+        Reads data from database, passes response object to a callback
+        and returns None or Result.
+
+        :return: None or Result
+        """
+        try:
+            async with session() as session:  # type: ignore
+                async with session.begin():  # type: ignore
+                    query = self.query
+                    response = await session.execute(query)  # type: ignore
+            logger.info(f'{self}.observe(session="{session}")')
+            return self._callback(response, *args, **kwargs)
+        except SQLAlchemyError as exception:
+            logger.warning(f"{self}.observe() -> {exception}")
+            return None
+        except Exception as exception:
+            logger.critical(f"{self}.observe() -> {exception}")
+            return None
+
+    def __repr__(self):
+        """
+        SQLObservation's __repr__ method.
+
+        :return: String representation of an instance
+        """
+        return (
+            f'SQLObservation("{self.query}","{self.url}",'
+            f'callback="{self._callback}")'
+        )
```

### Comparing `illuminated-0.2.0/illuminate/observer/observer.py` & `illuminated-0.3.0/illuminate/observer/observer.py`

 * *Files identical despite different names*

### Comparing `illuminated-0.2.0/pyproject.toml` & `illuminated-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-[tool.poetry]
-authors = ["Nikola Milojica <nikola.milojica@protonmail.com>"]
-classifiers = [
-    "Environment :: Console",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License"
-]
-description = "Lightwieght ETL Framework"
-documentation = "https://nikolamilojica.github.io/illuminate/"
-homepage = "https://github.com/nikolamilojica/illuminate"
-include = [
-    "LICENSE",
-]
-keywords = [
-    "ETL",
-    "Scraping"
-]
-license = "MIT"
-name = "illuminated"
-packages = [
-    { include = "illuminate" }
-]
-repository = "https://github.com/nikolamilojica/illuminate"
-version = "0.2.0"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-aiofile = "^3.8.1"
-alembic = "^1.7.7"
-asyncmy = "^0.2.5"
-asyncpg = "^0.26.0"
-click = "^8.1.2"
-loguru = "^0.6.0"
-psycopg2 = "^2.9.3"
-SQLAlchemy = {extras = ["asyncio"], version = "^1.4.42"}
-tornado = "^6.1"
-
-[tool.poetry.dev-dependencies]
-aiosqlite = "^0.17.0"
-bandit = "^1.7.4"
-black = "^22.3.0"
-beautifulsoup4 = "^4.11.1"
-flake8 = "^5.0.4"
-markdown-include = "^0.8.0"
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.10"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
-mypy = "^0.982"
-pre-commit = "^2.20.0"
-pytest = "^7.2.1"
-pytest-asyncio = "^0.19.0"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.8.2"
-sqlalchemy2-stubs = "^0.0.2-alpha.27"
-tox = "^4.3.5"
-
-[tool.poetry.scripts]
-illuminate = "illuminate.cli:cli"
-
-[build-system]
-build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core>=1.0.0"]
+[tool.poetry]
+authors = ["Nikola Milojica <nikola.milojica@protonmail.com>"]
+classifiers = [
+    "Environment :: Console",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License"
+]
+description = "Lightwieght ETL Framework"
+documentation = "https://nikolamilojica.github.io/illuminate/"
+homepage = "https://github.com/nikolamilojica/illuminate"
+include = [
+    "LICENSE",
+]
+keywords = [
+    "ETL",
+    "Scraping"
+]
+license = "MIT"
+name = "illuminated"
+packages = [
+    { include = "illuminate" }
+]
+repository = "https://github.com/nikolamilojica/illuminate"
+version = "0.3.0"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+aiofile = "^3.8.1"
+aioinflux = "^0.9.0"
+alembic = "^1.7.7"
+asyncmy = "^0.2.5"
+asyncpg = "^0.26.0"
+click = "^8.1.2"
+loguru = "^0.6.0"
+numpy = "1.24.4"
+pandas = "^2.0.3"
+psycopg2 = "^2.9.3"
+SQLAlchemy = {extras = ["asyncio"], version = "^1.4.42"}
+tornado = "^6.1"
+
+[tool.poetry.dev-dependencies]
+aiosqlite = "^0.17.0"
+bandit = "^1.7.4"
+black = "^22.3.0"
+beautifulsoup4 = "^4.11.1"
+flake8 = "^5.0.4"
+markdown-include = "^0.8.0"
+mkdocs = "^1.4.2"
+mkdocs-material = "^8.5.10"
+mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mypy = "^0.982"
+pre-commit = "^2.20.0"
+pytest = "^7.2.1"
+pytest-asyncio = "^0.19.0"
+pytest-cov = "^4.0.0"
+pytest-mock = "^3.8.2"
+sqlalchemy2-stubs = "^0.0.2-alpha.27"
+tox = "^4.3.5"
+
+[tool.poetry.scripts]
+illuminate = "illuminate.cli:cli"
+
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `illuminated-0.2.0/setup.py` & `illuminated-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,38 +7,42 @@
  'illuminate.common',
  'illuminate.decorators',
  'illuminate.exceptions',
  'illuminate.exporter',
  'illuminate.interface',
  'illuminate.manager',
  'illuminate.meta',
+ 'illuminate.meta.class',
  'illuminate.meta.type',
  'illuminate.observation',
  'illuminate.observer']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy[asyncio]>=1.4.42,<2.0.0',
  'aiofile>=3.8.1,<4.0.0',
+ 'aioinflux>=0.9.0,<0.10.0',
  'alembic>=1.7.7,<2.0.0',
  'asyncmy>=0.2.5,<0.3.0',
  'asyncpg>=0.26.0,<0.27.0',
  'click>=8.1.2,<9.0.0',
  'loguru>=0.6.0,<0.7.0',
+ 'numpy==1.24.4',
+ 'pandas>=2.0.3,<3.0.0',
  'psycopg2>=2.9.3,<3.0.0',
  'tornado>=6.1,<7.0']
 
 entry_points = \
 {'console_scripts': ['illuminate = illuminate.cli:cli']}
 
 setup_kwargs = {
     'name': 'illuminated',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Lightwieght ETL Framework',
     'long_description': None,
     'author': 'Nikola Milojica',
     'author_email': 'nikola.milojica@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nikolamilojica/illuminate',
```

### Comparing `illuminated-0.2.0/PKG-INFO` & `illuminated-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illuminated
-Version: 0.2.0
+Version: 0.3.0
 Summary: Lightwieght ETL Framework
 Home-page: https://github.com/nikolamilojica/illuminate
 License: MIT
 Keywords: ETL,Scraping
 Author: Nikola Milojica
 Author-email: nikola.milojica@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,16 +13,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: SQLAlchemy[asyncio] (>=1.4.42,<2.0.0)
 Requires-Dist: aiofile (>=3.8.1,<4.0.0)
+Requires-Dist: aioinflux (>=0.9.0,<0.10.0)
 Requires-Dist: alembic (>=1.7.7,<2.0.0)
 Requires-Dist: asyncmy (>=0.2.5,<0.3.0)
 Requires-Dist: asyncpg (>=0.26.0,<0.27.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: numpy (==1.24.4)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: tornado (>=6.1,<7.0)
 Project-URL: Documentation, https://nikolamilojica.github.io/illuminate/
 Project-URL: Repository, https://github.com/nikolamilojica/illuminate
```

