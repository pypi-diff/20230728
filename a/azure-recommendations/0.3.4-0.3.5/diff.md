# Comparing `tmp/azure_recommendations-0.3.4.tar.gz` & `tmp/azure_recommendations-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_recommendations-0.3.4.tar", last modified: Tue Jul  4 13:15:52 2023, max compression
+gzip compressed data, was "azure_recommendations-0.3.5.tar", last modified: Fri Jul 28 09:15:36 2023, max compression
```

## Comparing `azure_recommendations-0.3.4.tar` & `azure_recommendations-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.880880 azure_recommendations-0.3.4/
--rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.4/LICENCE
--rw-rw-rw-   0        0        0      533 2023-07-04 13:15:52.879902 azure_recommendations-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.749052 azure_recommendations-0.3.4/azure_recommendations/
--rw-rw-rw-   0        0        0      602 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/azure_recommendations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.875022 azure_recommendations-0.3.4/azure_recommendations/recommendation/
--rw-rw-rw-   0        0        0     7333 2023-05-13 15:13:20.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/advisor_recommendations.py
--rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/network_recommendations.py
--rw-rw-rw-   0        0        0    10152 2023-05-13 14:55:05.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/utils.py
--rw-rw-rw-   0        0        0    21578 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/azure_recommendations/recommendation/vm_recommendations.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:15:52.771517 azure_recommendations-0.3.4/azure_recommendations.egg-info/
--rw-rw-rw-   0        0        0      533 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-04 13:15:52.000000 azure_recommendations-0.3.4/azure_recommendations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-07-04 13:12:54.000000 azure_recommendations-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 13:15:52.881856 azure_recommendations-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 09:15:36.860986 azure_recommendations-0.3.5/
+-rw-rw-rw-   0        0        0        0 2023-03-24 12:23:56.000000 azure_recommendations-0.3.5/LICENCE
+-rw-rw-rw-   0        0        0      533 2023-07-28 09:15:36.849564 azure_recommendations-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-03-24 12:23:56.000000 azure_recommendations-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 09:15:36.749011 azure_recommendations-0.3.5/azure_recommendations/
+-rw-rw-rw-   0        0        0      602 2023-07-28 09:14:52.000000 azure_recommendations-0.3.5/azure_recommendations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:15:36.849564 azure_recommendations-0.3.5/azure_recommendations/recommendation/
+-rw-rw-rw-   0        0        0     7333 2023-05-13 15:13:20.000000 azure_recommendations-0.3.5/azure_recommendations/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 06:34:47.000000 azure_recommendations-0.3.5/azure_recommendations/recommendation/advisor_recommendations.py
+-rw-rw-rw-   0        0        0    14586 2023-05-05 06:34:47.000000 azure_recommendations-0.3.5/azure_recommendations/recommendation/network_recommendations.py
+-rw-rw-rw-   0        0        0    10237 2023-07-28 09:14:52.000000 azure_recommendations-0.3.5/azure_recommendations/recommendation/utils.py
+-rw-rw-rw-   0        0        0    22761 2023-07-28 09:14:53.000000 azure_recommendations-0.3.5/azure_recommendations/recommendation/vm_recommendations.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:15:36.758710 azure_recommendations-0.3.5/azure_recommendations.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-07-28 09:15:36.000000 azure_recommendations-0.3.5/azure_recommendations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-07-28 09:15:36.000000 azure_recommendations-0.3.5/azure_recommendations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:15:36.000000 azure_recommendations-0.3.5/azure_recommendations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-28 09:15:36.000000 azure_recommendations-0.3.5/azure_recommendations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-28 09:15:36.000000 azure_recommendations-0.3.5/azure_recommendations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      718 2023-07-28 09:14:53.000000 azure_recommendations-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:15:36.861488 azure_recommendations-0.3.5/setup.cfg
```

### Comparing `azure_recommendations-0.3.4/PKG-INFO` & `azure_recommendations-0.3.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_recommendations
-Version: 0.3.4
+Version: 0.3.5
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.4/azure_recommendations/__init__.py` & `azure_recommendations-0.3.5/azure_recommendations/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from azure_recommendations.recommendation import recommendation
 
 import logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 
 
 class az_session(recommendation):
     def __init__(self, tenant_id: str, client_id: str, client_secret: str):
         """
         :param tenant_id: tenant Id from Azure
         :param client_id: Access ID
```

### Comparing `azure_recommendations-0.3.4/azure_recommendations/recommendation/__init__.py` & `azure_recommendations-0.3.5/azure_recommendations/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.4/azure_recommendations/recommendation/advisor_recommendations.py` & `azure_recommendations-0.3.5/azure_recommendations/recommendation/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.4/azure_recommendations/recommendation/network_recommendations.py` & `azure_recommendations-0.3.5/azure_recommendations/recommendation/network_recommendations.py`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.4/azure_recommendations/recommendation/utils.py` & `azure_recommendations-0.3.5/azure_recommendations/recommendation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,26 +229,27 @@
 
             # print('*******************')
             # print(resource)
             res = {
                 'unitOfMeasure': None,
                 'retail_price': 0
             }
-            for obj in json_obj['Items']:
-                if 'reservationTerm' in obj:
-                    if obj['reservationTerm'] == '':
+            if 'Items' in json_obj:
+                for obj in json_obj['Items']:
+                    if 'reservationTerm' in obj:
+                        if obj['reservationTerm'] == '':
+                            # print(json.dumps(obj, indent=4))
+                            res['unitOfMeasure'] = obj['unitOfMeasure']
+                            res['retail_price'] = obj['retailPrice']
+                            break
+                    else:
                         # print(json.dumps(obj, indent=4))
                         res['unitOfMeasure'] = obj['unitOfMeasure']
                         res['retail_price'] = obj['retailPrice']
                         break
-                else:
-                    # print(json.dumps(obj, indent=4))
-                    res['unitOfMeasure'] = obj['unitOfMeasure']
-                    res['retail_price'] = obj['retailPrice']
-                    break
 
             return res
 
     # returns the list of resource groups
     def list_resource_groups(self, subscriptions: list) -> dict:
         """
         :param subscriptions:
```

### Comparing `azure_recommendations-0.3.4/azure_recommendations/recommendation/vm_recommendations.py` & `azure_recommendations-0.3.5/azure_recommendations/recommendation/vm_recommendations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import time
 from datetime import datetime, timedelta
 import re
 import pytz
 import requests
 from azure.identity import ClientSecretCredential
 from azure.mgmt.compute import ComputeManagementClient
 from azure.mgmt.resource import ResourceManagementClient
@@ -227,18 +228,41 @@
 
                     price_premium = get_cost_data(vm.location, 'Premium SSD Managed Disks', disk_data['properties']['tier']+' LRS')
                     # print(disk_data['properties']['tier'])
                     # print(price_premium)
                     price_standard = get_cost_data(vm.location, 'Standard SSD Managed Disks', disk_data['properties']['tier'].replace('P', 'E')+' LRS')
                     # print(price_standard)
 
-                    current_price = price_premium['Items'][0]['retailPrice']
-                    effective_price = price_standard['Items'][0]['retailPrice']
-                    savings = current_price - effective_price
-                    savings_p = (savings / current_price ) * 100
+                    try:
+                        current_price = price_premium['Items'][0]['retailPrice']
+                    except Exception as e:
+                        time.sleep(5)
+                        try:
+                            price_premium = get_cost_data(vm.location, 'Premium SSD Managed Disks',
+                                                          disk_data['properties']['tier'] + ' LRS')
+                            current_price = price_premium['Items'][0]['retailPrice']
+                        except Exception as e:
+                            current_price=0
+
+                    try:
+                        effective_price = price_standard['Items'][0]['retailPrice']
+                    except Exception as e:
+                        time.sleep(5)
+                        try:
+                            price_standard = get_cost_data(vm.location, 'Standard SSD Managed Disks', disk_data['properties']['tier'].replace('P', 'E')+' LRS')
+                            effective_price = price_premium['Items'][0]['retailPrice']
+                        except Exception as e:
+                            effective_price=0
+
+                    if current_price == 0:
+                        savings = 0
+                        savings_p = 0
+                    else:
+                        savings = current_price - effective_price
+                        savings_p = (savings / current_price ) * 100
 
                     temp = {
                         'recommendation': 'Disable premium SSD',
                         'Category': 'Cost',
                         'description': 'Microsoft Azure virtual machines (VMs) are using Premium SSD '
                                        'volumes, use Standard SSD disk volumes for cost-effective storage '
                                        'that fits a broad range of workloads',
```

### Comparing `azure_recommendations-0.3.4/azure_recommendations.egg-info/PKG-INFO` & `azure_recommendations-0.3.5/azure_recommendations.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-recommendations
-Version: 0.3.4
+Version: 0.3.5
 Summary: Provides Azure recommendations
 Author-email: "dheeraj.banodha" <dheeraj.banodha@impetus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `azure_recommendations-0.3.4/azure_recommendations.egg-info/SOURCES.txt` & `azure_recommendations-0.3.5/azure_recommendations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure_recommendations-0.3.4/pyproject.toml` & `azure_recommendations-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "azure_recommendations"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
 ]
 description = "Provides Azure recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

