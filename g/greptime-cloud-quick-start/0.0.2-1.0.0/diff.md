# Comparing `tmp/greptime_cloud_quick_start-0.0.2.tar.gz` & `tmp/greptime_cloud_quick_start-1.0.0.tar.gz`

## Comparing `greptime_cloud_quick_start-0.0.2.tar` & `greptime_cloud_quick_start-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/__init__.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/src/quick-start/app.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/LICENSE
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/README.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/.DS_Store
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/start/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/start/__main__.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/start/main.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/LICENSE
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 greptime_cloud_quick_start-1.0.0/PKG-INFO
```

### Comparing `greptime_cloud_quick_start-0.0.2/requirements.txt` & `greptime_cloud_quick_start-1.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.2/src/quick-start/app.py` & `greptime_cloud_quick_start-1.0.0/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,7 +57,11 @@
     }
     SystemMetricsInstrumentor(config=configuration).instrument()
 
     print("Sending metrics...")
 
     while True:
         time.sleep(2)
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `greptime_cloud_quick_start-0.0.2/.gitignore` & `greptime_cloud_quick_start-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.2/LICENSE` & `greptime_cloud_quick_start-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `greptime_cloud_quick_start-0.0.2/pyproject.toml` & `greptime_cloud_quick_start-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "greptime-cloud-quick-start"
-version = "0.0.2"
+name = "greptime_cloud_quick_start"
+version = "1.0.0"
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
+dependencies = [
+    "opentelemetry-api==1.19.0",
+    "opentelemetry-exporter-otlp-proto-http==1.19.0",
+    "opentelemetry-instrumentation==0.40b0",
+    "opentelemetry-instrumentation-system-metrics==0.40b0",
+    "opentelemetry-proto==1.19.0",
+    "opentelemetry-sdk==1.19.0",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/GreptimeCloudStarters/quick-start-python"
 "Bug Tracker" = "https://github.com/GreptimeCloudStarters/quick-start-python/issues"
 
 [project.scripts]
-greptime-cloud-quick-start = 'quick-start.app:main'
+greptime_cloud_quick_start = "start.main:main"
+
+[tool.setuptools.packages]
+find = {}  # Scanning implicit namespaces is active by default
+
```

