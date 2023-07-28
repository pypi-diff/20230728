# Comparing `tmp/odin_sdk_python-0.0.5.tar.gz` & `tmp/odin_sdk_python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_sdk_python-0.0.5.tar", max compression
+gzip compressed data, was "odin_sdk_python-0.0.6.tar", max compression
```

## Comparing `odin_sdk_python-0.0.5.tar` & `odin_sdk_python-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1349 2023-07-26 15:41:42.692116 odin_sdk_python-0.0.5/README.md
--rw-r--r--   0        0        0     1102 2023-07-26 15:41:42.692507 odin_sdk_python-0.0.5/odin/__init__.py
--rw-r--r--   0        0        0     4046 2023-07-26 15:41:42.692726 odin_sdk_python-0.0.5/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-26 15:41:42.693153 odin_sdk_python-0.0.5/odin/exceptions.py
--rw-r--r--   0        0        0      932 2023-07-26 15:41:42.693496 odin_sdk_python-0.0.5/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-26 15:41:42.693754 odin_sdk_python-0.0.5/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-26 15:41:42.694008 odin_sdk_python-0.0.5/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-26 15:41:42.694304 odin_sdk_python-0.0.5/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-26 15:41:42.694466 odin_sdk_python-0.0.5/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-26 15:41:42.694636 odin_sdk_python-0.0.5/odin/models/get_host_count.py
--rw-r--r--   0        0        0     1166 2023-07-26 15:41:42.694819 odin_sdk_python-0.0.5/odin/models/get_hosts_cve_details.py
--rw-r--r--   0        0        0     7022 2023-07-27 05:09:19.179558 odin_sdk_python-0.0.5/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-26 15:41:42.695234 odin_sdk_python-0.0.5/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7628 2023-07-26 15:41:42.695421 odin_sdk_python-0.0.5/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     6375 2023-07-26 15:41:42.695618 odin_sdk_python-0.0.5/odin/odin_client.py
--rw-r--r--   0        0        0      453 2023-07-28 06:12:26.160652 odin_sdk_python-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1336 2023-07-28 09:21:54.338620 odin_sdk_python-0.0.6/README.md
+-rw-r--r--   0        0        0     1102 2023-07-26 15:41:42.692507 odin_sdk_python-0.0.6/odin/__init__.py
+-rw-r--r--   0        0        0     4046 2023-07-26 15:41:42.692726 odin_sdk_python-0.0.6/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-26 15:41:42.693153 odin_sdk_python-0.0.6/odin/exceptions.py
+-rw-r--r--   0        0        0      932 2023-07-26 15:41:42.693496 odin_sdk_python-0.0.6/odin/models/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-26 15:41:42.693754 odin_sdk_python-0.0.6/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-26 15:41:42.694008 odin_sdk_python-0.0.6/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-26 15:41:42.694304 odin_sdk_python-0.0.6/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-26 15:41:42.694466 odin_sdk_python-0.0.6/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-26 15:41:42.694636 odin_sdk_python-0.0.6/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     1166 2023-07-26 15:41:42.694819 odin_sdk_python-0.0.6/odin/models/get_hosts_cve_details.py
+-rw-r--r--   0        0        0     7022 2023-07-27 05:09:19.179558 odin_sdk_python-0.0.6/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-26 15:41:42.695234 odin_sdk_python-0.0.6/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7628 2023-07-26 15:41:42.695421 odin_sdk_python-0.0.6/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     6375 2023-07-26 15:41:42.695618 odin_sdk_python-0.0.6/odin/odin_client.py
+-rw-r--r--   0        0        0      453 2023-07-28 09:27:16.534440 odin_sdk_python-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.6/PKG-INFO
```

### Comparing `odin_sdk_python-0.0.5/README.md` & `odin_sdk_python-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```python
 from odin import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
 
-def ex_certificate_count():
-    """Example for using get_certificate_count"""
+def ex_hosts_count():
+    # Example for using get_hosts_count
     try:
-        response = client.get_certificate_count("string")
+        response = client.get_hosts_count("string")
         print(response.success)
         print(response.data.count)
+        
     except APIException as e:
         print(e.status_code)
         print(e.message)
 ```
 
 Make sure to replace `<APIKey>` with your actual Odin API key.
```

### Comparing `odin_sdk_python-0.0.5/odin/__init__.py` & `odin_sdk_python-0.0.6/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/example.py` & `odin_sdk_python-0.0.6/odin/example.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/__init__.py` & `odin_sdk_python-0.0.6/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/certificate_search_response_model.py` & `odin_sdk_python-0.0.6/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/get_certificate_hash_details.py` & `odin_sdk_python-0.0.6/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/get_certificates_summary.py` & `odin_sdk_python-0.0.6/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/get_hosts_cve_details.py` & `odin_sdk_python-0.0.6/odin/models/get_hosts_cve_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/get_hosts_ip_details_response.py` & `odin_sdk_python-0.0.6/odin/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/get_hosts_summary_response.py` & `odin_sdk_python-0.0.6/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/models/search_hosts_response_model.py` & `odin_sdk_python-0.0.6/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/odin/odin_client.py` & `odin_sdk_python-0.0.6/odin/odin_client.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.5/PKG-INFO` & `odin_sdk_python-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin-sdk-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Allows to interact easily with the Odin API and access various cybersecurity services, certificate information, and more.
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,20 +32,21 @@
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```python
 from odin import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
 
-def ex_certificate_count():
-    """Example for using get_certificate_count"""
+def ex_hosts_count():
+    # Example for using get_hosts_count
     try:
-        response = client.get_certificate_count("string")
+        response = client.get_hosts_count("string")
         print(response.success)
         print(response.data.count)
+        
     except APIException as e:
         print(e.status_code)
         print(e.message)
 ```
 
 Make sure to replace `<APIKey>` with your actual Odin API key.
```

