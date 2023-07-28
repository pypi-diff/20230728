# Comparing `tmp/dcicutils-7.6.0.2b6.tar.gz` & `tmp/dcicutils-7.6.0.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b6.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.2b7.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b6.tar` & `dcicutils-7.6.0.2b7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/README.rst
--rw-r--r--   0        0        0        0 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    23914 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-07-28 18:53:33.705273 dcicutils-7.6.0.2b6/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38101 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-07-28 18:53:33.709273 dcicutils-7.6.0.2b6/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4387 2023-07-28 18:53:33.713273 dcicutils-7.6.0.2b6/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b6/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b6/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/README.rst
+-rw-r--r--   0        0        0        0 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    23914 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-07-28 21:14:31.449372 dcicutils-7.6.0.2b7/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    38497 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20511 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-07-28 21:14:31.453372 dcicutils-7.6.0.2b7/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4387 2023-07-28 21:14:31.457372 dcicutils-7.6.0.2b7/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b7/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b7/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b6/LICENSE.txt` & `dcicutils-7.6.0.2b7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/README.rst` & `dcicutils-7.6.0.2b7/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/base.py` & `dcicutils-7.6.0.2b7/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/command_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/common.py` & `dcicutils-7.6.0.2b7/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/contribution_scripts.py` & `dcicutils-7.6.0.2b7/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/contribution_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/creds_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/data_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/diff_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/docker_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.2b7/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/env_base.py` & `dcicutils-7.6.0.2b7/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/env_manager.py` & `dcicutils-7.6.0.2b7/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/env_scripts.py` & `dcicutils-7.6.0.2b7/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/env_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.2b7/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/es_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/exceptions.py` & `dcicutils-7.6.0.2b7/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.2b7/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ff_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.2b7/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/jh_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.2b7/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.2b7/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/lang_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/license_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/license_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,16 @@
         analysis = LicenseAnalysis()
         cls.analyze_license_dependencies_by_framework(analysis=analysis, frameworks=frameworks)
         cls.analyze_license_file(analysis=analysis)
         cls.show_unacceptable_licenses(analysis=analysis)
         if analysis.unexpected_missing:
             warnings.warn(there_are(analysis.unexpected_missing, kind='unexpectedly missing license', punctuate=True))
         if analysis.no_longer_missing:
-            warnings.warn(there_are(analysis.no_longer_missing, kind='no-longer-missing license', punctuate=True))
+            # This is not so major as to need a warning, but it's still something that should show up somewhere.
+            PRINT(there_are(analysis.no_longer_missing, kind='no-longer-missing license', punctuate=True))
         for message in analysis.miscellaneous:
             warnings.warn(message)
         if analysis.unacceptable:
             raise LicenseAcceptabilityCheckFailure(unacceptable_licenses=analysis.unacceptable)
 
 
 class LicenseCheckFailure(Exception):
@@ -699,23 +700,28 @@
         # Ref: https://github.com/repoze/repoze.debug/blob/master/LICENSE.txt
         'repoze.debug',
 
         # This is an Apache-2.0 license
         # Ref: https://github.com/getsentry/responses/blob/master/LICENSE
         'responses',
 
+        # This seems to get flagged sometimes, but is not the pypi snovault library, it's what our dcicsnovault
+        # calls itself internally.. In any case, it's under MIT license and OK.
+        # Ref: https://github.com/4dn-dcic/snovault/blob/master/LICENSE.txt
+        'snovault',
+
         # PyPi identifies the supervisor library license as "BSD-derived (http://www.repoze.org/LICENSE.txt)"
         # Ref: https://pypi.org/project/supervisor/
         # In fact, though, the license is a bit more complicated, though apparently still permissive.
         # Ref: https://github.com/Supervisor/supervisor/blob/main/LICENSES.txt
         'supervisor',
 
         # This seems to be a BSD-3-Clause-Modification license.
         # Ref: https://github.com/Pylons/translationstring/blob/master/LICENSE.txt
-        'translationstring',
+        # 'translationstring',
 
         # This seems to be a BSD-3-Clause-Modification license.
         # Ref: https://github.com/Pylons/venusian/blob/master/LICENSE.txt
         'venusian',
 
         # PyPi identifies zope.deprecation as using the "Zope Public License (ZPL 2.1)" license.
         # Ref: https://github.com/zopefoundation/Zope/blob/master/LICENSE.txt
```

### Comparing `dcicutils-7.6.0.2b6/dcicutils/log_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/misc_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/project_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.2b7/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/qa_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/redis_tools.py` & `dcicutils-7.6.0.2b7/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/redis_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/s3_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.2b7/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/task_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/dcicutils/trace_utils.py` & `dcicutils-7.6.0.2b7/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b6/pyproject.toml` & `dcicutils-7.6.0.2b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b6"
+version = "7.6.0.2b7"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.6.0.2b6/setup.py` & `dcicutils-7.6.0.2b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
                      'show-contributors = '
                      'dcicutils.contribution_scripts:show_contributors_main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b6',
+    'version': '7.6.0.2b7',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b6/PKG-INFO` & `dcicutils-7.6.0.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b6
+Version: 7.6.0.2b7
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

