# Comparing `tmp/bullhorn-0.0.4.tar.gz` & `tmp/bullhorn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullhorn-0.0.4.tar", last modified: Fri Jul 21 16:23:12 2023, max compression
+gzip compressed data, was "bullhorn-0.0.5.tar", last modified: Fri Jul 28 09:41:55 2023, max compression
```

## Comparing `bullhorn-0.0.4.tar` & `bullhorn-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.115668 bullhorn-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2240 2023-07-21 16:23:12.112628 bullhorn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2023-07-21 16:19:15.000000 bullhorn-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:11.954877 bullhorn-0.0.4/bullhorn/
--rw-rw-rw-   0        0        0       93 2023-07-21 16:21:50.000000 bullhorn-0.0.4/bullhorn/__init__.py
--rw-rw-rw-   0        0        0     8313 2023-07-21 15:12:58.000000 bullhorn-0.0.4/bullhorn/client.py
--rw-rw-rw-   0        0        0     4864 2023-07-21 10:35:13.000000 bullhorn-0.0.4/bullhorn/exceptions.py
--rw-rw-rw-   0        0        0     1739 2023-07-21 10:35:17.000000 bullhorn-0.0.4/bullhorn/route.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.087562 bullhorn-0.0.4/bullhorn/types/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.4/bullhorn/types/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/agreement_line.py
--rw-rw-rw-   0        0        0       33 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/billing_profile.py
--rw-rw-rw-   0        0        0       25 2023-07-21 13:35:23.000000 bullhorn-0.0.4/bullhorn/types/branch.py
--rw-rw-rw-   0        0        0     7532 2023-07-21 14:49:16.000000 bullhorn-0.0.4/bullhorn/types/candidate.py
--rw-rw-rw-   0        0        0       27 2023-07-21 13:38:39.000000 bullhorn-0.0.4/bullhorn/types/category.py
--rw-rw-rw-   0        0        0     3805 2023-07-21 13:36:23.000000 bullhorn-0.0.4/bullhorn/types/client_contact.py
--rw-rw-rw-   0        0        0     2594 2023-07-21 14:10:39.000000 bullhorn-0.0.4/bullhorn/types/client_corporation.py
--rw-rw-rw-   0        0        0      748 2023-07-21 11:40:00.000000 bullhorn-0.0.4/bullhorn/types/corporate_user.py
--rw-rw-rw-   0        0        0       26 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/job_code.py
--rw-rw-rw-   0        0        0     4816 2023-07-21 13:43:16.000000 bullhorn-0.0.4/bullhorn/types/job_order.py
--rw-rw-rw-   0        0        0       32 2023-07-21 13:33:13.000000 bullhorn-0.0.4/bullhorn/types/job_submission.py
--rw-rw-rw-   0        0        0       23 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/lead.py
--rw-rw-rw-   0        0        0       27 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/location.py
--rw-rw-rw-   0        0        0     3098 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/opportunity.py
--rw-rw-rw-   0        0        0       81 2023-07-21 13:32:38.000000 bullhorn-0.0.4/bullhorn/types/person.py
--rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.4/bullhorn/types/ping.py
--rw-rw-rw-   0        0        0     8325 2023-07-21 13:38:40.000000 bullhorn-0.0.4/bullhorn/types/placement.py
--rw-rw-rw-   0        0        0      477 2023-07-21 14:58:56.000000 bullhorn-0.0.4/bullhorn/types/placement_commission.py
--rw-rw-rw-   0        0        0      572 2023-07-21 13:36:49.000000 bullhorn-0.0.4/bullhorn/types/shift.py
--rw-rw-rw-   0        0        0      190 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/workers_compensation.py
--rw-rw-rw-   0        0        0      213 2023-07-21 13:54:17.000000 bullhorn-0.0.4/bullhorn/types/workers_compensation_rate.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:11.983303 bullhorn-0.0.4/bullhorn.egg-info/
--rw-rw-rw-   0        0        0     2240 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1055 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-21 16:23:11.000000 bullhorn-0.0.4/bullhorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.095583 bullhorn-0.0.4/examples/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.4/examples/__init__.py
--rw-rw-rw-   0        0        0      845 2023-07-21 10:46:50.000000 bullhorn-0.0.4/examples/get_placements_and_candidates.py
--rw-rw-rw-   0        0        0       42 2023-07-21 16:23:12.116672 bullhorn-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-21 10:38:28.000000 bullhorn-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:23:12.106611 bullhorn-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     8197 2023-07-21 15:40:15.000000 bullhorn-0.0.4/tests/test_client.py
--rw-rw-rw-   0        0        0     1069 2023-07-21 10:47:02.000000 bullhorn-0.0.4/tests/test_route.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.660148 bullhorn-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-07-07 06:22:40.000000 bullhorn-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2240 2023-07-28 09:41:55.659145 bullhorn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1774 2023-07-21 16:19:15.000000 bullhorn-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.375167 bullhorn-0.0.5/bullhorn/
+-rw-rw-rw-   0        0        0       93 2023-07-28 09:40:50.000000 bullhorn-0.0.5/bullhorn/__init__.py
+-rw-rw-rw-   0        0        0     8363 2023-07-28 09:35:07.000000 bullhorn-0.0.5/bullhorn/client.py
+-rw-rw-rw-   0        0        0     4864 2023-07-21 10:35:13.000000 bullhorn-0.0.5/bullhorn/exceptions.py
+-rw-rw-rw-   0        0        0     1739 2023-07-21 10:35:17.000000 bullhorn-0.0.5/bullhorn/route.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.625086 bullhorn-0.0.5/bullhorn/types/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.5/bullhorn/types/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-21 13:35:23.000000 bullhorn-0.0.5/bullhorn/types/agreement_line.py
+-rw-rw-rw-   0        0        0       33 2023-07-21 13:35:23.000000 bullhorn-0.0.5/bullhorn/types/billing_profile.py
+-rw-rw-rw-   0        0        0       25 2023-07-21 13:35:23.000000 bullhorn-0.0.5/bullhorn/types/branch.py
+-rw-rw-rw-   0        0        0     7532 2023-07-21 14:49:16.000000 bullhorn-0.0.5/bullhorn/types/candidate.py
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:38:39.000000 bullhorn-0.0.5/bullhorn/types/category.py
+-rw-rw-rw-   0        0        0     3805 2023-07-21 13:36:23.000000 bullhorn-0.0.5/bullhorn/types/client_contact.py
+-rw-rw-rw-   0        0        0     2594 2023-07-21 14:10:39.000000 bullhorn-0.0.5/bullhorn/types/client_corporation.py
+-rw-rw-rw-   0        0        0      748 2023-07-21 11:40:00.000000 bullhorn-0.0.5/bullhorn/types/corporate_user.py
+-rw-rw-rw-   0        0        0       26 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/job_code.py
+-rw-rw-rw-   0        0        0     4816 2023-07-21 13:43:16.000000 bullhorn-0.0.5/bullhorn/types/job_order.py
+-rw-rw-rw-   0        0        0       32 2023-07-21 13:33:13.000000 bullhorn-0.0.5/bullhorn/types/job_submission.py
+-rw-rw-rw-   0        0        0       23 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/lead.py
+-rw-rw-rw-   0        0        0       27 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/location.py
+-rw-rw-rw-   0        0        0     3098 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/opportunity.py
+-rw-rw-rw-   0        0        0       81 2023-07-21 13:32:38.000000 bullhorn-0.0.5/bullhorn/types/person.py
+-rw-rw-rw-   0        0        0       38 2023-06-13 12:11:53.000000 bullhorn-0.0.5/bullhorn/types/ping.py
+-rw-rw-rw-   0        0        0     8325 2023-07-21 13:38:40.000000 bullhorn-0.0.5/bullhorn/types/placement.py
+-rw-rw-rw-   0        0        0      477 2023-07-21 14:58:56.000000 bullhorn-0.0.5/bullhorn/types/placement_commission.py
+-rw-rw-rw-   0        0        0      572 2023-07-21 13:36:49.000000 bullhorn-0.0.5/bullhorn/types/shift.py
+-rw-rw-rw-   0        0        0      190 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/workers_compensation.py
+-rw-rw-rw-   0        0        0      213 2023-07-21 13:54:17.000000 bullhorn-0.0.5/bullhorn/types/workers_compensation_rate.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.411857 bullhorn-0.0.5/bullhorn.egg-info/
+-rw-rw-rw-   0        0        0     2240 2023-07-28 09:41:55.000000 bullhorn-0.0.5/bullhorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-07-28 09:41:55.000000 bullhorn-0.0.5/bullhorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:41:55.000000 bullhorn-0.0.5/bullhorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-28 09:41:55.000000 bullhorn-0.0.5/bullhorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-28 09:41:55.000000 bullhorn-0.0.5/bullhorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.639091 bullhorn-0.0.5/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:02:11.000000 bullhorn-0.0.5/examples/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-07-21 10:46:50.000000 bullhorn-0.0.5/examples/get_placements_and_candidates.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:41:55.661222 bullhorn-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-07-25 10:21:53.000000 bullhorn-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:41:55.655166 bullhorn-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:33:32.000000 bullhorn-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     8894 2023-07-28 09:40:08.000000 bullhorn-0.0.5/tests/test_client.py
+-rw-rw-rw-   0        0        0     1069 2023-07-21 10:47:02.000000 bullhorn-0.0.5/tests/test_route.py
```

### Comparing `bullhorn-0.0.4/LICENSE` & `bullhorn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/PKG-INFO` & `bullhorn-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullhorn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper for the Bullhorn REST API
 Home-page: https://github.com/recruithub/bullhorn
 Author: lloydtao
 Author-email: lewis@recruit-hub.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bullhorn-0.0.4/README.md` & `bullhorn-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/client.py` & `bullhorn-0.0.5/bullhorn/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import logging
 import sys
 import time
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
@@ -141,15 +140,15 @@
                 self.rest_url + "search/Candidate?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_client_contacts(
         self,
         query: str,
         fields: str,
     ) -> List[client_contact.ClientContact]:
         request = self.request(
@@ -158,15 +157,15 @@
                 self.rest_url + "search/ClientContact?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_client_corporations(
         self,
         query: str,
         fields: str,
     ) -> List[client_corporation.ClientCorporation]:
         request = self.request(
@@ -176,32 +175,32 @@
                 + "search/ClientCorporation?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_corporate_users(
         self,
-        query: str,
+        where: str,
         fields: str,
     ) -> List[corporate_user.CorporateUser]:
         request = self.request(
             Route(
                 "GET",
-                self.rest_url + "search/CorporateUser?query={query}&fields={fields}",
+                self.rest_url + "query/CorporateUser?where={where}&fields={fields}",
                 path_params={
-                    "query": query,
+                    "where": where,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_job_orders(
         self,
         query: str,
         fields: str,
     ) -> List[job_order.JobOrder]:
         request = self.request(
@@ -210,15 +209,15 @@
                 self.rest_url + "search/JobOrder?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_job_submissions(
         self,
         query: str,
         fields: str,
     ) -> List[job_submission.JobSubmission]:
         request = self.request(
@@ -227,15 +226,15 @@
                 self.rest_url + "search/JobSubmission?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_placements(
         self,
         query: str,
         fields: str,
     ) -> List[placement.Placement]:
         request = self.request(
@@ -244,15 +243,15 @@
                 self.rest_url + "search/Placement?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
 
     def get_placement_commissions(
         self,
         query: str,
         fields: str,
     ) -> List[placement_commission.PlacementCommission]:
         request = self.request(
@@ -262,8 +261,8 @@
                 + "search/PlacementCommission?query={query}&fields={fields}",
                 path_params={
                     "query": query,
                     "fields": fields,
                 },
             )
         )
-        return request
+        return request["data"]
```

### Comparing `bullhorn-0.0.4/bullhorn/exceptions.py` & `bullhorn-0.0.5/bullhorn/exceptions.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/route.py` & `bullhorn-0.0.5/bullhorn/route.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/candidate.py` & `bullhorn-0.0.5/bullhorn/types/candidate.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/client_contact.py` & `bullhorn-0.0.5/bullhorn/types/client_contact.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/client_corporation.py` & `bullhorn-0.0.5/bullhorn/types/client_corporation.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/corporate_user.py` & `bullhorn-0.0.5/bullhorn/types/corporate_user.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/job_order.py` & `bullhorn-0.0.5/bullhorn/types/job_order.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/opportunity.py` & `bullhorn-0.0.5/bullhorn/types/opportunity.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/placement.py` & `bullhorn-0.0.5/bullhorn/types/placement.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn/types/shift.py` & `bullhorn-0.0.5/bullhorn/types/shift.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/bullhorn.egg-info/PKG-INFO` & `bullhorn-0.0.5/bullhorn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullhorn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper for the Bullhorn REST API
 Home-page: https://github.com/recruithub/bullhorn
 Author: lloydtao
 Author-email: lewis@recruit-hub.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bullhorn-0.0.4/bullhorn.egg-info/SOURCES.txt` & `bullhorn-0.0.5/bullhorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/examples/get_placements_and_candidates.py` & `bullhorn-0.0.5/examples/get_placements_and_candidates.py`

 * *Files identical despite different names*

### Comparing `bullhorn-0.0.4/setup.py` & `bullhorn-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     author_email="lewis@recruit-hub.com",
     description="Python wrapper for the Bullhorn REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/recruithub/bullhorn",
     packages=find_packages(),
     install_requires=[
-        "requests==2.31.0",
+        "requests>=2,<3",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
```

### Comparing `bullhorn-0.0.4/tests/test_client.py` & `bullhorn-0.0.5/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,22 +41,27 @@
     # Get result
     result = bc.ping()
     assert "sessionExpires" in result
 
 
 def test_client_get_candidates(mocker):
     # Mock response
-    return_value: List[candidate.Candidate] = [
-        {
-            "id": 1234567891011,
-            "firstName": "Example",
-            "middleName": "C.",
-            "lastName": "Name",
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "firstName": "Example",
+                "middleName": "C.",
+                "lastName": "Name",
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -68,22 +73,27 @@
         fields="id,firstName,middleName,lastName",
     )
     assert "firstName" in result[0]
 
 
 def test_client_get_client_contacts(mocker):
     # Mock response
-    return_value: List[client_contact.ClientContact] = [
-        {
-            "id": 1234567891011,
-            "firstName": "Example",
-            "middleName": "C.",
-            "lastName": "Name",
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "firstName": "Example",
+                "middleName": "C.",
+                "lastName": "Name",
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -95,20 +105,25 @@
         fields="id,firstName,middleName,lastName",
     )
     assert "lastName" in result[0]
 
 
 def test_client_get_client_corporations(mocker):
     # Mock response
-    return_value: List[client_corporation.ClientCorporation] = [
-        {
-            "id": 1234567891011,
-            "name": "Example Inc.",
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "name": "Example Inc.",
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -120,55 +135,65 @@
         fields="id,name",
     )
     assert "name" in result[0]
 
 
 def test_client_get_corporate_users(mocker):
     # Mock response
-    return_value: List[corporate_user.CorporateUser] = [
-        {
-            "id": 1234567891011,
-            "firstName": "Example",
-            "middleName": "C.",
-            "lastName": "Name",
-            "username": "ExampleCName",
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "firstName": "Example",
+                "middleName": "C.",
+                "lastName": "Name",
+                "username": "ExampleCName",
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
         rest_url="https://rest123.bullhornstaffing.com/rest-services/1234/",
     )
     # Get result
     result = bc.get_corporate_users(
-        query="dateLastModified:{2023/01/01 TO *}",
+        where="id >= 0",
         fields="id,firstName,middleName,lastName,username",
     )
     assert "username" in result[0]
 
 
 def test_client_get_job_orders(mocker):
     # Mock response
-    return_value: List[job_order.JobOrder] = [
-        {
-            "id": 1234567891011,
-            "description": "An example open job to be filled.",
-            "owner": {
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
                 "id": 1234567891011,
-                "firstName": "Example",
-                "middleName": "C.",
-                "lastName": "Name",
-                "username": "ExampleCName",
+                "description": "An example open job to be filled.",
+                "owner": {
+                    "id": 1234567891011,
+                    "firstName": "Example",
+                    "middleName": "C.",
+                    "lastName": "Name",
+                    "username": "ExampleCName",
+                },
             },
-        },
-    ]
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -180,30 +205,35 @@
         fields="id,description,owner",
     )
     assert "owner" in result[0]
 
 
 def test_client_get_job_submissions(mocker):
     # Mock response
-    return_value: List[job_submission.JobSubmission] = [
-        {
-            "id": 1234567891011,
-            "endDate": 1234567891011,
-            "owners": [
-                {
-                    "id": 1234567891011,
-                    "firstName": "Example",
-                    "middleName": "C.",
-                    "lastName": "Name",
-                    "username": "ExampleCName",
-                },
-            ],
-            "startDate": 1234567891012,
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "endDate": 1234567891011,
+                "owners": [
+                    {
+                        "id": 1234567891011,
+                        "firstName": "Example",
+                        "middleName": "C.",
+                        "lastName": "Name",
+                        "username": "ExampleCName",
+                    },
+                ],
+                "startDate": 1234567891012,
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -215,20 +245,25 @@
         fields="id,endDate,owners,startDate",
     )
     assert "owners" in result[0]
 
 
 def test_client_get_placements(mocker):
     # Mock response
-    return_value: List[placement.Placement] = [
-        {
-            "id": 1234567891011,
-            "fee": 0.5,
-        },
-    ]
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
+                "id": 1234567891011,
+                "fee": 0.5,
+            },
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
@@ -240,27 +275,32 @@
         fields="id,fee",
     )
     assert "fee" in result[0]
 
 
 def test_client_get_placement_commissions(mocker):
     # Mock response
-    return_value: List[placement_commission.PlacementCommission] = [
-        {
-            "id": 1234567891011,
-            "user": {
+    return_value = {
+        "total": 1,
+        "start": 0,
+        "count": 1,
+        "data": [
+            {
                 "id": 1234567891011,
-                "firstName": "Example",
-                "middleName": "C.",
-                "lastName": "Name",
-                "username": "ExampleCName",
+                "user": {
+                    "id": 1234567891011,
+                    "firstName": "Example",
+                    "middleName": "C.",
+                    "lastName": "Name",
+                    "username": "ExampleCName",
+                },
+                "commissionPercentage": 0.05,
             },
-            "commissionPercentage": 0.05,
-        },
-    ]
+        ],
+    }
     mocker.patch(
         "bullhorn.client.BullhornClient.request",
         return_value=return_value,
     )
     # Initialise client
     bc = BullhornClient(
         token="12345_1234567_a12345bc-123a-45bc-67de-12345678910a",
```

### Comparing `bullhorn-0.0.4/tests/test_route.py` & `bullhorn-0.0.5/tests/test_route.py`

 * *Files identical despite different names*

