# Comparing `tmp/foursight_cgap-3.6.0.1b2.tar.gz` & `tmp/foursight_cgap-3.6.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.6.0.1b2.tar", max compression
+gzip compressed data, was "foursight_cgap-3.6.0.1b3.tar", max compression
```

## Comparing `foursight_cgap-3.6.0.1b2.tar` & `foursight_cgap-3.6.0.1b3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.6.0.1b2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.6.0.1b2/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1071 2023-07-16 15:38:24.354182 foursight_cgap-3.6.0.1b2/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.6.0.1b2/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4805 2023-07-16 15:38:24.354684 foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17006 2023-06-17 14:10:51.489200 foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-07-16 16:00:24.552615 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2023-07-16 12:57:18.590153 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58234 2023-07-16 15:38:24.355462 foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.6.0.1b2/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.6.0.1b2/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      235 2023-07-27 22:59:05.918959 foursight_cgap-3.6.0.1b2/chalicelib_cgap/scripts/local_check_execution.py
--rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.6.0.1b2/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1247 2023-07-28 03:55:03.863407 foursight_cgap-3.6.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0.1b2/setup.py
--rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.6.0.1b3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.6.0.1b3/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-16 15:38:24.354182 foursight_cgap-3.6.0.1b3/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.6.0.1b3/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4805 2023-07-16 15:38:24.354684 foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17006 2023-06-17 14:10:51.489200 foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-07-16 16:00:24.552615 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2023-07-16 12:57:18.590153 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58234 2023-07-16 15:38:24.355462 foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.6.0.1b3/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.6.0.1b3/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      235 2023-07-27 22:59:05.918959 foursight_cgap-3.6.0.1b3/chalicelib_cgap/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.6.0.1b3/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1244 2023-07-28 04:00:20.176254 foursight_cgap-3.6.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0.1b3/setup.py
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0.1b3/PKG-INFO
```

### Comparing `foursight_cgap-3.6.0.1b2/LICENSE.txt` & `foursight_cgap-3.6.0.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/app_utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/buckets.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_schedules.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_setup.json` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/deploy.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/chalicelib_cgap/package.py` & `foursight_cgap-3.6.0.1b3/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.6.0.1b2/pyproject.toml` & `foursight_cgap-3.6.0.1b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "3.6.0.1b2"  # TODO: To become 3.6.1
+version = "3.6.0.1b3"  # TODO: To become 3.6.1
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
 
 [tool.poetry.dependencies]
 # Cannot go to Python 3.8 because cgap-pipeilne is stuck on Python 3.7.
 python = ">=3.7.1,<3.8"
 click = "^7.1.2"
-dcicutils = "7.6.0.1b4"
+dcicutils = "^7.5.2"
 cgap-pipeline-utils = "23.0"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 foursight-core = "4.4.0.1b2"
 geocoder = "1.38.1"
```

### Comparing `foursight_cgap-3.6.0.1b2/setup.py` & `foursight_cgap-3.6.0.1b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'cgap-pipeline-utils==23.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils==7.6.0.1b4',
+ 'dcicutils>=7.5.2,<8.0.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
  'foursight-core==4.4.0.1b2',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.12.5,<2.0.0',
  'google-auth>=2.22.0,<3.0.0',
@@ -33,15 +33,15 @@
 {'console_scripts': ['local-check-execution = '
                      'chalicelib_cgap.scripts.local_check_execution:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-cgap',
-    'version': '3.6.0.1b2',
+    'version': '3.6.0.1b3',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_cgap-3.6.0.1b2/PKG-INFO` & `foursight_cgap-3.6.0.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 3.6.0.1b2
+Version: 3.6.0.1b3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: cgap-pipeline-utils (==23.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (==7.6.0.1b4)
+Requires-Dist: dcicutils (>=7.5.2,<8.0.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: foursight-core (==4.4.0.1b2)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth (>=2.22.0,<3.0.0)
```

