# Comparing `tmp/greptime_cloud_quick_start-0.0.1.tar.gz` & `tmp/greptime_cloud_quick_start-0.0.2.tar.gz`

## Comparing `greptime_cloud_quick_start-0.0.1.tar` & `greptime_cloud_quick_start-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/src/quick-start/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/src/quick-start/app.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/LICENSE
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/__init__.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/app.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/LICENSE
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/PKG-INFO
```

### Comparing `greptime_cloud_quick_start-0.0.1/requirements.txt` & `greptime_cloud_quick_start-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.1/src/quick-start/app.py` & `greptime_cloud_quick_start-0.0.2/src/quick-start/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,63 @@
+#!/usr/bin/env python
+
 import time
 import argparse
 import base64
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import (
     ConsoleMetricExporter,
     PeriodicExportingMetricReader,
 )
 from opentelemetry import metrics
 from opentelemetry.instrumentation.system_metrics import SystemMetricsInstrumentor
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
 
-parser = argparse.ArgumentParser(
-                    prog='greptime-cloud-quick-start-python',
-                    description='Quick start Python demo for greptime cloud')
-
-parser.add_argument('-host', required=True, help='The host address of the GreptimeCloud service')
-parser.add_argument('-db', '--database', required=True, help='The database of the GreptimeCloud service')
-parser.add_argument('-u', '--username', required=True, help='The username of the database')
-parser.add_argument('-p', '--password', required=True, help='The password of the database')
-args = parser.parse_args()
-host = args.host
-db = args.database
-username = args.username
-password = args.password
-
-auth = f"{username}:{password}"
-b64_auth = base64.b64encode(auth.encode()).decode("ascii")
-
-# Service name is required for most backends
-resource = Resource(attributes={
-    SERVICE_NAME: "quick-start-python"
-})
-
-endpoint = f"https://{host}/v1/otlp/v1/metrics"
-
-exporter = OTLPMetricExporter(
-    endpoint=endpoint,
-    headers={"Authorization": f"Basic {b64_auth}", "x-greptime-db-name": db},
-    timeout=5)
-# exporter = ConsoleMetricExporter()
-metric_reader = PeriodicExportingMetricReader(exporter, 2000)
-provider = MeterProvider(resource=resource, metric_readers=[metric_reader])
-
-# Sets the global default meter provider
-metrics.set_meter_provider(provider)
-configuration = {
-    "system.memory.usage": ["used", "free", "cached"],
-    "system.cpu.time": ["idle", "user", "system", "irq"],
-    "process.runtime.memory": ["rss", "vms"],
-    "process.runtime.cpu.time": ["user", "system"],
-}
-SystemMetricsInstrumentor(config=configuration).instrument()
 
-print("Sending metrics...")
+def main():
+    parser = argparse.ArgumentParser(
+                        prog='greptime-cloud-quick-start-python',
+                        description='Quick start Python demo for greptime cloud')
+
+    parser.add_argument('-host', required=True, help='The host address of the GreptimeCloud service')
+    parser.add_argument('-db', '--database', required=True, help='The database of the GreptimeCloud service')
+    parser.add_argument('-u', '--username', required=True, help='The username of the database')
+    parser.add_argument('-p', '--password', required=True, help='The password of the database')
+    args = parser.parse_args()
+    host = args.host
+    db = args.database
+    username = args.username
+    password = args.password
+
+    auth = f"{username}:{password}"
+    b64_auth = base64.b64encode(auth.encode()).decode("ascii")
+
+    # Service name is required for most backends
+    resource = Resource(attributes={
+        SERVICE_NAME: "quick-start-python"
+    })
+
+    endpoint = f"https://{host}/v1/otlp/v1/metrics"
+
+    exporter = OTLPMetricExporter(
+        endpoint=endpoint,
+        headers={"Authorization": f"Basic {b64_auth}", "x-greptime-db-name": db},
+        timeout=5)
+    # exporter = ConsoleMetricExporter()
+    metric_reader = PeriodicExportingMetricReader(exporter, 2000)
+    provider = MeterProvider(resource=resource, metric_readers=[metric_reader])
+
+    # Sets the global default meter provider
+    metrics.set_meter_provider(provider)
+    configuration = {
+        "system.memory.usage": ["used", "free", "cached"],
+        "system.cpu.time": ["idle", "user", "system", "irq"],
+        "process.runtime.memory": ["rss", "vms"],
+        "process.runtime.cpu.time": ["user", "system"],
+    }
+    SystemMetricsInstrumentor(config=configuration).instrument()
+
+    print("Sending metrics...")
 
-while True:
-    time.sleep(2)
+    while True:
+        time.sleep(2)
```

### Comparing `greptime_cloud_quick_start-0.0.1/.gitignore` & `greptime_cloud_quick_start-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.1/LICENSE` & `greptime_cloud_quick_start-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.1/pyproject.toml` & `greptime_cloud_quick_start-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "greptime-cloud-quick-start"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="CUI YIRAN", email="cuiyiran3@gmail.com" },
 ]
 description = "A quick start demo for GreptimeCloud"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -16,7 +16,10 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GreptimeCloudStarters/quick-start-python"
 "Bug Tracker" = "https://github.com/GreptimeCloudStarters/quick-start-python/issues"
+
+[project.scripts]
+greptime-cloud-quick-start = 'quick-start.app:main'
```

### Comparing `greptime_cloud_quick_start-0.0.1/PKG-INFO` & `greptime_cloud_quick_start-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greptime-cloud-quick-start
-Version: 0.0.1
+Version: 0.0.2
 Summary: A quick start demo for GreptimeCloud
 Project-URL: Homepage, https://github.com/GreptimeCloudStarters/quick-start-python
 Project-URL: Bug Tracker, https://github.com/GreptimeCloudStarters/quick-start-python/issues
 Author-email: CUI YIRAN <cuiyiran3@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

