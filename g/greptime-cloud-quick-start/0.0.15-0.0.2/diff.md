# Comparing `tmp/greptime_cloud_quick_start-0.0.15.tar.gz` & `tmp/greptime_cloud_quick_start-0.0.2.tar.gz`

## Comparing `greptime_cloud_quick_start-0.0.15.tar` & `greptime_cloud_quick_start-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/.DS_Store
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/start/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/start/__main__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/start/main.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/LICENSE
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/README.md
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/__init__.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/app.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/LICENSE
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/PKG-INFO
```

### Comparing `greptime_cloud_quick_start-0.0.15/requirements.txt` & `greptime_cloud_quick_start-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.15/start/main.py` & `greptime_cloud_quick_start-0.0.2/src/quick-start/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,11 +57,7 @@
     }
     SystemMetricsInstrumentor(config=configuration).instrument()
 
     print("Sending metrics...")
 
     while True:
         time.sleep(2)
-
-if __name__ == "__main__":
-    main()
-
```

### Comparing `greptime_cloud_quick_start-0.0.15/.gitignore` & `greptime_cloud_quick_start-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.15/LICENSE` & `greptime_cloud_quick_start-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.15/pyproject.toml` & `greptime_cloud_quick_start-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "greptime_cloud_quick_start"
-version = "0.0.15"
+name = "greptime-cloud-quick-start"
+version = "0.0.2"
 authors = [
   { name="CUI YIRAN", email="cuiyiran3@gmail.com" },
 ]
 description = "A quick start demo for GreptimeCloud"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-    "opentelemetry-api==1.19.0",
-    "opentelemetry-exporter-otlp-proto-http==1.19.0",
-    "opentelemetry-instrumentation==0.40b0",
-    "opentelemetry-instrumentation-system-metrics==0.40b0",
-    "opentelemetry-proto==1.19.0",
-    "opentelemetry-sdk==1.19.0",
-]
 
 [project.urls]
 "Homepage" = "https://github.com/GreptimeCloudStarters/quick-start-python"
 "Bug Tracker" = "https://github.com/GreptimeCloudStarters/quick-start-python/issues"
 
 [project.scripts]
-greptime_cloud_quick_start = "start.main:main"
-
-[tool.setuptools.packages]
-find = {}  # Scanning implicit namespaces is active by default
-
+greptime-cloud-quick-start = 'quick-start.app:main'
```

### Comparing `greptime_cloud_quick_start-0.0.15/PKG-INFO` & `greptime_cloud_quick_start-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 Metadata-Version: 2.1
-Name: greptime_cloud_quick_start
-Version: 0.0.15
+Name: greptime-cloud-quick-start
+Version: 0.0.2
 Summary: A quick start demo for GreptimeCloud
 Project-URL: Homepage, https://github.com/GreptimeCloudStarters/quick-start-python
 Project-URL: Bug Tracker, https://github.com/GreptimeCloudStarters/quick-start-python/issues
 Author-email: CUI YIRAN <cuiyiran3@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: opentelemetry-api==1.19.0
-Requires-Dist: opentelemetry-exporter-otlp-proto-http==1.19.0
-Requires-Dist: opentelemetry-instrumentation-system-metrics==0.40b0
-Requires-Dist: opentelemetry-instrumentation==0.40b0
-Requires-Dist: opentelemetry-proto==1.19.0
-Requires-Dist: opentelemetry-sdk==1.19.0
 Description-Content-Type: text/markdown
 
 # Introduction
 
 This is a quick start demo for [GreptimeCloud](https://greptime.cloud/). It collects the system metric data such as CPU and memory usage through Opentelemetry and sends the metrics to GreptimeCloud. You can view the metrics on the GreptimeCloud dashboard.
 
 Use the following command line to start it in Python 3.10:
```

