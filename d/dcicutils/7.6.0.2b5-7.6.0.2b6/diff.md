# Comparing `tmp/dcicutils-7.6.0.2b5.tar.gz` & `tmp/dcicutils-7.6.0.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b5.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.2b6.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b5.tar` & `dcicutils-7.6.0.2b6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/README.rst
--rw-r--r--   0        0        0        0 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    23914 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38083 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4387 2023-07-28 17:31:30.188741 dcicutils-7.6.0.2b5/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b5/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b5/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/README.rst
+-rw-r--r--   0        0        0        0 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    23914 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    38101 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20511 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4387 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b6/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b6/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b5/LICENSE.txt` & `dcicutils-7.6.0.2b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/README.rst` & `dcicutils-7.6.0.2b6/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/base.py` & `dcicutils-7.6.0.2b6/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/command_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/common.py` & `dcicutils-7.6.0.2b6/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/contribution_scripts.py` & `dcicutils-7.6.0.2b6/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/contribution_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/creds_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/data_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/diff_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/docker_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.2b6/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/env_base.py` & `dcicutils-7.6.0.2b6/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/env_manager.py` & `dcicutils-7.6.0.2b6/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/env_scripts.py` & `dcicutils-7.6.0.2b6/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/env_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.2b6/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/es_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/exceptions.py` & `dcicutils-7.6.0.2b6/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.2b6/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ff_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.2b6/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/jh_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.2b6/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.2b6/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/lang_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/license_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/license_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import contextlib
 import datetime
 import io
 import json
-import logging
+# import logging
 import os
 import re
 import subprocess
+import warnings
 
 try:
     import piplicenses
 except ImportError:  # pragma: no cover - not worth unit testing this case
     raise Exception("The dcicutils.license_utils module is intended for use at development time, not runtime."
                     " It does not export a requirement for the pip-licenses library,"
                     " but to use this in your unit tests, you are expected to assure a dev dependency on that library"
@@ -26,16 +27,16 @@
 
 # For obscure reasons related to how this file is used for early prototyping, these must use absolute references
 # to modules, not relative references. Later when things are better installed, we can make refs relative again.
 from dcicutils.lang_utils import there_are
 from dcicutils.misc_utils import PRINT, get_error_message, local_attrs
 
 
-logging.basicConfig()
-logger = logging.getLogger(__name__)
+# logging.basicConfig()
+# logger = logging.getLogger(__name__)
 
 _FRAMEWORK = 'framework'
 _LANGUAGE = 'language'
 _LICENSE = 'license'
 _LICENSE_CLASSIFIER = 'license_classifier'
 _LICENSES = 'licenses'
 _NAME = 'name'
@@ -266,15 +267,15 @@
                                      check_copyright_year: Union[bool, str] = True,
                                      check_copyright_owner: str = None,  # a copyright owner
                                      analysis: LicenseAnalysis = None):
         def report(message):
             if analysis:
                 analysis.miscellaneous.append(message)
             else:
-                logger.warning(message)
+                warnings.warn(message)
         parsed = cls.parse_simple_license_file(filename=filename)
         if check_license_title:
             license_title = parsed['license-title']
             if license_title != check_license_title:
                 report(f"The license, {license_title!r}, was expected to be {check_license_title!r}.")
         if check_copyright_year:
             if check_copyright_year is True:
@@ -484,19 +485,19 @@
         which we sometimes informally refer to collectively as 'C4'.
         """
         analysis = LicenseAnalysis()
         cls.analyze_license_dependencies_by_framework(analysis=analysis, frameworks=frameworks)
         cls.analyze_license_file(analysis=analysis)
         cls.show_unacceptable_licenses(analysis=analysis)
         if analysis.unexpected_missing:
-            logger.warning(there_are(analysis.unexpected_missing, kind='unexpectedly missing license', punctuate=True))
+            warnings.warn(there_are(analysis.unexpected_missing, kind='unexpectedly missing license', punctuate=True))
         if analysis.no_longer_missing:
-            logger.warning(there_are(analysis.no_longer_missing, kind='no-longer-missing license', punctuate=True))
+            warnings.warn(there_are(analysis.no_longer_missing, kind='no-longer-missing license', punctuate=True))
         for message in analysis.miscellaneous:
-            logger.warning(message)
+            warnings.warn(message)
         if analysis.unacceptable:
             raise LicenseAcceptabilityCheckFailure(unacceptable_licenses=analysis.unacceptable)
 
 
 class LicenseCheckFailure(Exception):
 
     DEFAULT_MESSAGE = "License check failure."
```

### Comparing `dcicutils-7.6.0.2b5/dcicutils/log_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/misc_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/project_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.2b6/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/qa_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/redis_tools.py` & `dcicutils-7.6.0.2b6/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/redis_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/s3_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.2b6/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/task_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/dcicutils/trace_utils.py` & `dcicutils-7.6.0.2b6/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b5/pyproject.toml` & `dcicutils-7.6.0.2b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b5"
+version = "7.6.0.2b6"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.6.0.2b5/setup.py` & `dcicutils-7.6.0.2b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
                      'show-contributors = '
                      'dcicutils.contribution_scripts:show_contributors_main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b5',
+    'version': '7.6.0.2b6',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b5/PKG-INFO` & `dcicutils-7.6.0.2b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b5
+Version: 7.6.0.2b6
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

