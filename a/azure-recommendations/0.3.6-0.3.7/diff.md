# Comparing `tmp/azure_recommendations-0.3.6.tar.gz` & `tmp/azure_recommendations-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_recommendations-0.3.6.tar", last modified: Fri Jul 28 10:19:38 2023, max compression
+gzip compressed data, was "azure_recommendations-0.3.7.tar", last modified: Fri Jul 28 10:51:09 2023, max compression
```

## Comparing `azure_recommendations-0.3.6.tar` & `azure_recommendations-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:19:38.913033 azure_recommendations-0.3.6/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.6/LICENCE
--rw-rw-rw-   0        0        0      533 2023-07-28 10:19:38.911272 azure_recommendations-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 10:19:38.664799 azure_recommendations-0.3.6/azure_recommendations/
--rw-rw-rw-   0        0        0      602 2023-07-28 10:14:28.000000 azure_recommendations-0.3.6/azure_recommendations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:19:38.908054 azure_recommendations-0.3.6/azure_recommendations/recommendation/
--rw-rw-rw-   0        0        0     8130 2023-07-28 10:03:50.000000 azure_recommendations-0.3.6/azure_recommendations/recommendation/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.6/azure_recommendations/recommendation/advisor_recommendations.py
--rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.6/azure_recommendations/recommendation/network_recommendations.py
--rw-rw-rw-   0        0        0    10237 2023-07-28 09:14:52.000000 azure_recommendations-0.3.6/azure_recommendations/recommendation/utils.py
--rw-rw-rw-   0        0        0    22861 2023-07-28 09:58:40.000000 azure_recommendations-0.3.6/azure_recommendations/recommendation/vm_recommendations.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:19:38.682100 azure_recommendations-0.3.6/azure_recommendations.egg-info/
--rw-rw-rw-   0        0        0      533 2023-07-28 10:19:38.000000 azure_recommendations-0.3.6/azure_recommendations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-07-28 10:19:38.000000 azure_recommendations-0.3.6/azure_recommendations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:19:38.000000 azure_recommendations-0.3.6/azure_recommendations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-07-28 10:19:38.000000 azure_recommendations-0.3.6/azure_recommendations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-28 10:19:38.000000 azure_recommendations-0.3.6/azure_recommendations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-07-28 10:14:28.000000 azure_recommendations-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 10:19:38.913530 azure_recommendations-0.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:09.136766 azure_recommendations-0.3.7/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.7/LICENCE
+-rw-rw-rw-   0        0        0      533 2023-07-28 10:51:09.135070 azure_recommendations-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:08.992302 azure_recommendations-0.3.7/azure_recommendations/
+-rw-rw-rw-   0        0        0      602 2023-07-28 10:50:36.000000 azure_recommendations-0.3.7/azure_recommendations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:09.129063 azure_recommendations-0.3.7/azure_recommendations/recommendation/
+-rw-rw-rw-   0        0        0     8126 2023-07-28 10:31:32.000000 azure_recommendations-0.3.7/azure_recommendations/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.7/azure_recommendations/recommendation/advisor_recommendations.py
+-rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.7/azure_recommendations/recommendation/network_recommendations.py
+-rw-rw-rw-   0        0        0    10237 2023-07-28 09:14:52.000000 azure_recommendations-0.3.7/azure_recommendations/recommendation/utils.py
+-rw-rw-rw-   0        0        0    22861 2023-07-28 09:58:40.000000 azure_recommendations-0.3.7/azure_recommendations/recommendation/vm_recommendations.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:51:09.009051 azure_recommendations-0.3.7/azure_recommendations.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-07-28 10:51:08.000000 azure_recommendations-0.3.7/azure_recommendations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-07-28 10:51:08.000000 azure_recommendations-0.3.7/azure_recommendations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:51:08.000000 azure_recommendations-0.3.7/azure_recommendations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-28 10:51:08.000000 azure_recommendations-0.3.7/azure_recommendations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-28 10:51:08.000000 azure_recommendations-0.3.7/azure_recommendations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-07-28 10:50:36.000000 azure_recommendations-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:51:09.137769 azure_recommendations-0.3.7/setup.cfg
```

### Comparing `azure_recommendations-0.3.6/PKG-INFO` & `azure_recommendations-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_recommendations
-Version: 0.3.6
+Version: 0.3.7
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.6/azure_recommendations/__init__.py` & `azure_recommendations-0.3.7/azure_recommendations/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from azure_recommendations.recommendation import recommendation
 
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 
 class az_session(recommendation):
     def __init__(self, tenant_id: str, client_id: str, client_secret: str):
         """
         :param tenant_id: tenant Id from Azure
         :param client_id: Access ID
```

### Comparing `azure_recommendations-0.3.6/azure_recommendations/recommendation/__init__.py` & `azure_recommendations-0.3.7/azure_recommendations/recommendation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
 
         try:
             vm_list = self.list_vms(subscriptions)
         except Exception as e:
             pass
         else:
             try:
-                # response.extend(self.check_for_ssh_authentication_type(vm_list))
+                response.extend(self.check_for_ssh_authentication_type(vm_list))
             except Exception as e:
                 pass
             try:
-                # response.extend(self.disable_premium_ssd(vm_list))
+                response.extend(self.disable_premium_ssd(vm_list))
             except Exception as e:
                 pass
             try:
                 response.extend(self.enable_auto_shutdown(vm_list))
             except Exception as e:
                 pass
```

### Comparing `azure_recommendations-0.3.6/azure_recommendations/recommendation/advisor_recommendations.py` & `azure_recommendations-0.3.7/azure_recommendations/recommendation/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.6/azure_recommendations/recommendation/network_recommendations.py` & `azure_recommendations-0.3.7/azure_recommendations/recommendation/network_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.6/azure_recommendations/recommendation/utils.py` & `azure_recommendations-0.3.7/azure_recommendations/recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.6/azure_recommendations/recommendation/vm_recommendations.py` & `azure_recommendations-0.3.7/azure_recommendations/recommendation/vm_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.6/azure_recommendations.egg-info/PKG-INFO` & `azure_recommendations-0.3.7/azure_recommendations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-recommendations
-Version: 0.3.6
+Version: 0.3.7
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.6/azure_recommendations.egg-info/SOURCES.txt` & `azure_recommendations-0.3.7/azure_recommendations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.6/pyproject.toml` & `azure_recommendations-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "azure_recommendations"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
 ]
 description = "Provides Azure recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

