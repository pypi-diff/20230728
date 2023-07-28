# Comparing `tmp/influenzanet.api-1.1.2.tar.gz` & `tmp/influenzanet.api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influenzanet.api-1.1.2.tar", last modified: Wed Dec  7 08:15:34 2022, max compression
+gzip compressed data, was "influenzanet.api-1.1.3.tar", last modified: Fri Jul 28 17:52:30 2023, max compression
```

## Comparing `influenzanet.api-1.1.2.tar` & `influenzanet.api-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2022-12-07 08:15:34.152458 influenzanet.api-1.1.2/
--rw-r--r--   0 clementturbelin   (501) staff       (20)    11357 2022-10-27 12:16:12.000000 influenzanet.api-1.1.2/LICENCE
--rw-r--r--   0 clementturbelin   (501) staff       (20)      764 2022-12-07 08:15:34.152079 influenzanet.api-1.1.2/PKG-INFO
-drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2022-12-07 08:15:34.145677 influenzanet.api-1.1.2/influenzanet/
-drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2022-12-07 08:15:34.151614 influenzanet.api-1.1.2/influenzanet/api/
--rw-r--r--   0 clementturbelin   (501) staff       (20)       60 2022-11-11 10:34:12.000000 influenzanet.api-1.1.2/influenzanet/api/__init__.py
--rw-r--r--   0 clementturbelin   (501) staff       (20)    27259 2022-12-05 13:44:41.000000 influenzanet.api-1.1.2/influenzanet/api/management_api.py
--rw-r--r--   0 clementturbelin   (501) staff       (20)     9177 2022-11-11 10:34:12.000000 influenzanet.api-1.1.2/influenzanet/api/response_parser.py
-drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2022-12-07 08:15:34.150373 influenzanet.api-1.1.2/influenzanet.api.egg-info/
--rw-r--r--   0 clementturbelin   (501) staff       (20)      764 2022-12-07 08:15:34.000000 influenzanet.api-1.1.2/influenzanet.api.egg-info/PKG-INFO
--rw-r--r--   0 clementturbelin   (501) staff       (20)      330 2022-12-07 08:15:34.000000 influenzanet.api-1.1.2/influenzanet.api.egg-info/SOURCES.txt
--rw-r--r--   0 clementturbelin   (501) staff       (20)        1 2022-12-07 08:15:34.000000 influenzanet.api-1.1.2/influenzanet.api.egg-info/dependency_links.txt
--rw-r--r--   0 clementturbelin   (501) staff       (20)       17 2022-12-07 08:15:34.000000 influenzanet.api-1.1.2/influenzanet.api.egg-info/requires.txt
--rw-r--r--   0 clementturbelin   (501) staff       (20)       13 2022-12-07 08:15:34.000000 influenzanet.api-1.1.2/influenzanet.api.egg-info/top_level.txt
--rw-r--r--   0 clementturbelin   (501) staff       (20)      897 2022-11-08 18:17:59.000000 influenzanet.api-1.1.2/pyproject.toml
--rw-r--r--   0 clementturbelin   (501) staff       (20)       38 2022-12-07 08:15:34.152572 influenzanet.api-1.1.2/setup.cfg
--rw-r--r--   0 clementturbelin   (501) staff       (20)       37 2022-10-27 12:32:16.000000 influenzanet.api-1.1.2/setup.py
+drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2023-07-28 17:52:30.108702 influenzanet.api-1.1.3/
+-rw-r--r--   0 clementturbelin   (501) staff       (20)    11357 2022-10-27 12:16:12.000000 influenzanet.api-1.1.3/LICENCE
+-rw-r--r--   0 clementturbelin   (501) staff       (20)      764 2023-07-28 17:52:30.108333 influenzanet.api-1.1.3/PKG-INFO
+drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2023-07-28 17:52:30.097818 influenzanet.api-1.1.3/influenzanet/
+drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2023-07-28 17:52:30.107799 influenzanet.api-1.1.3/influenzanet/api/
+-rw-r--r--   0 clementturbelin   (501) staff       (20)       60 2022-11-11 10:34:12.000000 influenzanet.api-1.1.3/influenzanet/api/__init__.py
+-rw-r--r--   0 clementturbelin   (501) staff       (20)    27261 2023-07-28 17:51:22.000000 influenzanet.api-1.1.3/influenzanet/api/management_api.py
+-rw-r--r--   0 clementturbelin   (501) staff       (20)     9177 2022-11-11 10:34:12.000000 influenzanet.api-1.1.3/influenzanet/api/response_parser.py
+drwxr-xr-x   0 clementturbelin   (501) staff       (20)        0 2023-07-28 17:52:30.105535 influenzanet.api-1.1.3/influenzanet.api.egg-info/
+-rw-r--r--   0 clementturbelin   (501) staff       (20)      764 2023-07-28 17:52:30.000000 influenzanet.api-1.1.3/influenzanet.api.egg-info/PKG-INFO
+-rw-r--r--   0 clementturbelin   (501) staff       (20)      340 2023-07-28 17:52:30.000000 influenzanet.api-1.1.3/influenzanet.api.egg-info/SOURCES.txt
+-rw-r--r--   0 clementturbelin   (501) staff       (20)        1 2023-07-28 17:52:30.000000 influenzanet.api-1.1.3/influenzanet.api.egg-info/dependency_links.txt
+-rw-r--r--   0 clementturbelin   (501) staff       (20)       17 2023-07-28 17:52:30.000000 influenzanet.api-1.1.3/influenzanet.api.egg-info/requires.txt
+-rw-r--r--   0 clementturbelin   (501) staff       (20)       13 2023-07-28 17:52:30.000000 influenzanet.api-1.1.3/influenzanet.api.egg-info/top_level.txt
+-rw-r--r--   0 clementturbelin   (501) staff       (20)      897 2022-11-08 18:17:59.000000 influenzanet.api-1.1.3/pyproject.toml
+-rw-r--r--   0 clementturbelin   (501) staff       (20)      160 2022-11-01 08:53:35.000000 influenzanet.api-1.1.3/readme.md
+-rw-r--r--   0 clementturbelin   (501) staff       (20)       38 2023-07-28 17:52:30.108820 influenzanet.api-1.1.3/setup.cfg
+-rw-r--r--   0 clementturbelin   (501) staff       (20)       37 2022-10-27 12:32:16.000000 influenzanet.api-1.1.3/setup.py
```

### Comparing `influenzanet.api-1.1.2/LICENCE` & `influenzanet.api-1.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `influenzanet.api-1.1.2/PKG-INFO` & `influenzanet.api-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influenzanet.api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Influenzanet API python library
 Author-email: Peter Hevesi <hevesi@coneno.com>, Clement Turbelin <clement.turbelin@iplesp.upmc.fr>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/influenzanet/python-influenzanet-api.git
 Project-URL: Bug Tracker, https://github.com/influenzanet/python-influenzanet-api/issues
 Keywords: influenzanet,surveys
 Classifier: Programming Language :: Python :: 3
```

### Comparing `influenzanet.api-1.1.2/influenzanet/api/management_api.py` & `influenzanet.api-1.1.3/influenzanet/api/management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,20 +275,20 @@
         data = r.json()
         if extract_infos and 'infos' in data:
             return data['infos']
         return data
 
     def get_survey_definition(self, study_key, survey_key, version_id=''):
         """
-            Load a Survey definition 
+            Load a Survey definition
             If version_id is empty load the last published version (currents)
         """
         if self.auth_header is None:
             raise ValueError('need to login first')
-        url = self.management_api_url + '/v1/study/' + study_key + '/survey/' + survey_key 
+        url = self.management_api_url + '/v1/study/' + study_key + '/survey/' + survey_key
         if version_id != "":
             url += '/' + version_id
         r = requests.get(url, headers={'Authorization': 'Bearer ' + self.token})
         if r.status_code != 200:
             if json.loads(r.content.decode())["error"] == "mongo: no documents in result":
                 print('Survey key does not exist in this study yet.')
             else:
@@ -344,15 +344,15 @@
         if r.status_code != 200:
             raise ValueError(r.content)
         print("survey successfully removed")
 
     def get_participant_states(self, study_key: str, status:str=None):
         if self.auth_header is None:
             raise ValueError('need to login first')
-        url = "{}/v1/data/{}/participants".format(
+        url = "{}/v1/data/{}/participants/all".format(
                 self.management_api_url,
                 study_key,
             )
 
         if status is not None:
             params = {
                 "status": status
```

### Comparing `influenzanet.api-1.1.2/influenzanet/api/response_parser.py` & `influenzanet.api-1.1.3/influenzanet/api/response_parser.py`

 * *Files identical despite different names*

### Comparing `influenzanet.api-1.1.2/influenzanet.api.egg-info/PKG-INFO` & `influenzanet.api-1.1.3/influenzanet.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influenzanet.api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Influenzanet API python library
 Author-email: Peter Hevesi <hevesi@coneno.com>, Clement Turbelin <clement.turbelin@iplesp.upmc.fr>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/influenzanet/python-influenzanet-api.git
 Project-URL: Bug Tracker, https://github.com/influenzanet/python-influenzanet-api/issues
 Keywords: influenzanet,surveys
 Classifier: Programming Language :: Python :: 3
```

### Comparing `influenzanet.api-1.1.2/pyproject.toml` & `influenzanet.api-1.1.3/pyproject.toml`

 * *Files identical despite different names*

