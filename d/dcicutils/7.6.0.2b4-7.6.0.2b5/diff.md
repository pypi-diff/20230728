# Comparing `tmp/dcicutils-7.6.0.2b4.tar.gz` & `tmp/dcicutils-7.6.0.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.6.0.2b4.tar", max compression
+gzip compressed data, was "dcicutils-7.6.0.2b5.tar", max compression
```

## Comparing `dcicutils-7.6.0.2b4.tar` & `dcicutils-7.6.0.2b5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1103 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/README.rst
--rw-r--r--   0        0        0        0 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3763 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    23725 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-07-28 12:52:44.655389 dcicutils-7.6.0.2b4/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68885 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-07-28 12:52:44.659389 dcicutils-7.6.0.2b4/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27797 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    38083 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20511 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    13576 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-07-28 12:52:44.663389 dcicutils-7.6.0.2b4/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-07-28 12:52:44.667389 dcicutils-7.6.0.2b4/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-07-28 12:52:44.667389 dcicutils-7.6.0.2b4/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-07-28 12:52:44.667389 dcicutils-7.6.0.2b4/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-07-28 12:52:44.667389 dcicutils-7.6.0.2b4/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     4263 2023-07-28 12:52:44.667389 dcicutils-7.6.0.2b4/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b4/setup.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b4/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/README.rst
+-rw-r--r--   0        0        0        0 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-07-28 17:31:30.176739 dcicutils-7.6.0.2b5/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3763 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    23914 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68885 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27797 2023-07-28 17:31:30.180740 dcicutils-7.6.0.2b5/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    38083 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20511 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-07-28 17:31:30.184740 dcicutils-7.6.0.2b5/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     4387 2023-07-28 17:31:30.188741 dcicutils-7.6.0.2b5/pyproject.toml
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b5/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.6.0.2b5/PKG-INFO
```

### Comparing `dcicutils-7.6.0.2b4/LICENSE.txt` & `dcicutils-7.6.0.2b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/README.rst` & `dcicutils-7.6.0.2b5/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/base.py` & `dcicutils-7.6.0.2b5/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/beanstalk_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/cloudformation_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/codebuild_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/command_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/common.py` & `dcicutils-7.6.0.2b5/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/contribution_scripts.py` & `dcicutils-7.6.0.2b5/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/contribution_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/contribution_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,41 +133,147 @@
             name,  # this names by alphabetical order not because one is better, but to make sort results deterministic
         )
 
 
 ContributorIndex = Optional[Dict[str, Contributor]]
 
 
-class Contributions(GitAnalysis):
+class BasicContributions(GitAnalysis):
 
     VERBOSE = False
 
     def __init__(self, *, repo: Optional[str] = None,
                  exclude_fork: Optional[str] = None,
                  verbose: Optional[bool] = None):
+        self.email_timestamps: Dict[str, datetime.datetime] = {}
+        self.name_timestamps: Dict[str, datetime.datetime] = {}
+        self.exclude_fork: Optional[str] = exclude_fork
         if not repo:
             # Doing it this way gets around an ambiguity about '/foo/' vs '/foo' since both
             # os.path.join('/foo/', 'bar') and os.path.join('/foo', 'bar') yield '/foo/bar',
             # and from there one can do os.path.basename(os.path.dirname(...)) to get 'foo' out.
             cache_file = os.path.join(os.path.abspath(os.path.curdir), self.CONTRIBUTORS_CACHE_FILE)
             dir = os.path.dirname(cache_file)
             repo = os.path.basename(dir)
-        self.email_timestamps: Dict[str, datetime.datetime] = {}
-        self.name_timestamps: Dict[str, datetime.datetime] = {}
         self.repo: str = repo
-        self.exclude_fork: Optional[str] = exclude_fork
         self.excluded_contributions = None
         self.forked_at: Optional[datetime.datetime] = None
         self.contributors_by_name: Optional[ContributorIndex] = None
         self.contributors_by_email: Optional[ContributorIndex] = None
         self.pre_fork_contributors_by_email: Optional[ContributorIndex] = None
         self.pre_fork_contributors_by_name: Optional[ContributorIndex] = None
-        self.verbose = self.VERBOSE if verbose is None else verbose
         self.loaded_contributor_data = None
         self.cache_discrepancies: Optional[dict] = None
+        self.verbose = self.VERBOSE if verbose is None else verbose
+
+    CONTRIBUTORS_CACHE_FILE = 'CONTRIBUTORS.json'
+
+    def contributors_json_file(self):
+        """
+        Returns the name of the CONTRIBUTORS.json file for the repo associated with this class.
+        """
+        return os.path.join(PROJECT_HOME, self.repo, self.CONTRIBUTORS_CACHE_FILE)
+
+    def existing_contributors_json_file(self):
+        """
+        Returns the name of the CONTRIBUTORS.json file for the repo associated with this class if that file exists,
+        or None if there is no such file.
+        """
+        file = self.contributors_json_file()
+        if os.path.exists(file):
+            return file
+        else:
+            return None
+
+    @classmethod
+    def notice_reference_time(cls, key: str, timestamp: datetime.datetime, timestamps: Dict[str, datetime.datetime]):
+        reference_timestamp: datetime.datetime = timestamps.get(key)
+        if not reference_timestamp:
+            timestamps[key] = timestamp
+        elif timestamp > reference_timestamp:
+            timestamps[key] = timestamp
+
+    def email_reference_time(self, email):
+        return self.email_timestamps.get(email)
+
+    def name_reference_time(self, name):
+        return self.name_timestamps.get(name)
+
+    @classmethod
+    def contributor_values_as_dicts(cls, contributor_index: Optional[ContributorIndex]):
+        if contributor_index is None:
+            return None
+        else:
+            return {
+                key: contributor.as_dict()
+                for key, contributor in contributor_index.items()
+            }
+
+    @classmethod
+    def contributor_values_as_objects(cls, contributor_index: Optional[Dict]):
+        if contributor_index is None:
+            return None
+        else:
+            return {
+                key: Contributor.from_dict(value, key=key)
+                for key, value in contributor_index.items()
+            }
+
+    def checkpoint_state(self):
+        return self.as_dict()
+
+    def as_dict(self):
+        data = {
+            "forked_at": self.forked_at.isoformat() if self.forked_at else None,
+            "excluded_fork": self.exclude_fork,
+            "pre_fork_contributors_by_name": self.contributor_values_as_dicts(self.pre_fork_contributors_by_name),
+            "contributors_by_name": self.contributor_values_as_dicts(self.contributors_by_name),
+        }
+        return data
+
+    def save_contributor_data(self, filename: Optional[str] = None) -> str:
+        if filename is None:
+            filename = self.contributors_json_file()
+        with io.open(filename, 'w') as fp:
+            PRINT(json.dumps(self.as_dict(), indent=2), file=fp)
+        return filename
+
+    def repo_contributor_names(self, with_email=False):
+        for name, contributor in self.contributors_by_name.items():
+            if with_email:
+                yield f"{name} ({', '.join([self.pretty_email(email) for email in contributor.emails])})"
+            else:
+                yield name
+
+    @classmethod
+    def pretty_email(cls, email):
+        m = GITHUB_USER_REGEXP.match(email)
+        if m:
+            user_name = m.group(1)
+            return f"{user_name}@github"
+        else:
+            return email
+
+    @classmethod
+    def get_contributors_json_from_file_cache(cls, filename):
+        try:
+            with io.open(filename, 'r') as fp:
+                data = json.load(fp)
+        except Exception:
+            PRINT(f"Error while reading data from {filename!r}.")
+            raise
+        return data
+
+
+class Contributions(BasicContributions):
+
+    def __init__(self, *, repo: Optional[str] = None,
+                 exclude_fork: Optional[str] = None,
+                 verbose: Optional[bool] = None):
+        super().__init__(repo=repo, exclude_fork=exclude_fork, verbose=verbose)
         existing_contributor_data_file = self.existing_contributors_json_file()
         if existing_contributor_data_file:
             # This will set .loaded_contributor_data and other values from CONTRIBUTORS.json
             self.load_contributors_from_json_file_cache(existing_contributor_data_file)
 
         if exclude_fork and not self.excluded_contributions:
             self.excluded_contributions = Contributions(repo=exclude_fork)
@@ -194,72 +300,16 @@
             if added:
                 cache_discrepancies['to_add'] = added
             if changed:
                 cache_discrepancies['to_change'] = changed
             if removed:
                 cache_discrepancies['to_remove'] = removed
 
-    @classmethod
-    def pretty_email(cls, email):
-        m = GITHUB_USER_REGEXP.match(email)
-        if m:
-            user_name = m.group(1)
-            return f"{user_name}@github"
-        else:
-            return email
-
-    @classmethod
-    def notice_reference_time(cls, key: str, timestamp: datetime.datetime, timestamps: Dict[str, datetime.datetime]):
-        reference_timestamp: datetime.datetime = timestamps.get(key)
-        if not reference_timestamp:
-            timestamps[key] = timestamp
-        elif timestamp > reference_timestamp:
-            timestamps[key] = timestamp
-
-    def email_reference_time(self, email):
-        return self.email_timestamps.get(email)
-
-    def name_reference_time(self, name):
-        return self.name_timestamps.get(name)
-
-    CONTRIBUTORS_CACHE_FILE = 'CONTRIBUTORS.json'
-
-    def contributors_json_file(self):
-        """
-        Returns the name of the CONTRIBUTORS.json file for the repo associated with this class.
-        """
-        return self.contributors_json_file_for_repo(self.repo)
-
-    @classmethod
-    def contributors_json_file_for_repo(cls, repo):
-        return os.path.join(PROJECT_HOME, repo, cls.CONTRIBUTORS_CACHE_FILE)
-
-    def existing_contributors_json_file(self):
-        """
-        Returns the name of the CONTRIBUTORS.json file for the repo associated with this class if that file exists,
-        or None if there is no such file.
-        """
-        self.existing_contributors_json_file_for_repo(self.repo)
-
-    @classmethod
-    def existing_contributors_json_file_for_repo(cls, repo):
-        file = cls.contributors_json_file_for_repo(repo)
-        if os.path.exists(file):
-            return file
-        else:
-            return None
-
     def load_contributors_from_json_file_cache(self, filename):
-        try:
-            with io.open(filename, 'r') as fp:
-                data = json.load(fp)
-        except Exception:
-            PRINT(f"Error while reading data from {filename!r}.")
-            raise
-        self.loaded_contributor_data = data
+        self.loaded_contributor_data = data = self.get_contributors_json_from_file_cache(filename)
         self.load_from_dict(data)
 
         if DEBUG_CONTRIBUTIONS:  # pragma: no cover - debugging only
             PRINT("After load_contributors_from_json_file_cache...")
             PRINT(f"{n_of(self.pre_fork_contributors_by_name, 'pre-fork contributor by name')}")
             PRINT(f"{n_of(self.pre_fork_contributors_by_email, 'pre-fork contributor by email')}")
             PRINT(f"{n_of(self.contributors_by_name, 'contributor by name')}")
@@ -413,46 +463,14 @@
                              contributors_by_name=contributors_by_name, seen=seen)
         for email in list(cursor.emails):
             contributor = contributors_by_email.get(email)
             if contributor and contributor not in seen:
                 cls.traverse(root=root, cursor=contributor, contributors_by_email=contributors_by_email,
                              contributors_by_name=contributors_by_name, seen=seen)
 
-    @classmethod
-    def contributor_values_as_dicts(cls, contributor_index: Optional[ContributorIndex]):
-        if contributor_index is None:
-            return None
-        else:
-            return {
-                key: contributor.as_dict()
-                for key, contributor in contributor_index.items()
-            }
-
-    @classmethod
-    def contributor_values_as_objects(cls, contributor_index: Optional[Dict]):
-        if contributor_index is None:
-            return None
-        else:
-            return {
-                key: Contributor.from_dict(value, key=key)
-                for key, value in contributor_index.items()
-            }
-
-    def checkpoint_state(self):
-        return self.as_dict()
-
-    def as_dict(self):
-        data = {
-            "forked_at": self.forked_at.isoformat() if self.forked_at else None,
-            "excluded_fork": self.exclude_fork,
-            "pre_fork_contributors_by_name": self.contributor_values_as_dicts(self.pre_fork_contributors_by_name),
-            "contributors_by_name": self.contributor_values_as_dicts(self.contributors_by_name),
-        }
-        return data
-
     def load_from_dict(self, data: Dict):
         forked_at: Optional[str] = data.get('forked_at')
         excluded_fork = data.get('excluded_fork')
         self.forked_at: Optional[datetime.datetime] = (None
                                                        if forked_at is None
                                                        else datetime.datetime.fromisoformat(forked_at))
         self.exclude_fork = excluded_fork
@@ -486,27 +504,14 @@
             seen.add(seen_key)
             for email in entry.get("emails", []) if isinstance(entry, dict) else entry.emails:
                 if result.get(email):
                     raise Exception(f"email address {email} is used more than once.")
                 result[email] = entry
         return result
 
-    def save_contributor_data(self, filename: Optional[str] = None):
-        if filename is None:
-            filename = self.contributors_json_file()
-        with io.open(filename, 'w') as fp:
-            PRINT(json.dumps(self.as_dict(), indent=2), file=fp)
-
-    def repo_contributor_names(self, with_email=False):
-        for name, contributor in self.contributors_by_name.items():
-            if with_email:
-                yield f"{name} ({', '.join([self.pretty_email(email) for email in contributor.emails])})"
-            else:
-                yield name
-
     def show_repo_contributors(self, analyze_discrepancies: bool = True, with_email: bool = True,
                                error_class: Optional[Type[BaseException]] = None):
         for author_name in self.repo_contributor_names(with_email=with_email):
             PRINT(author_name)
         if analyze_discrepancies:
             file = self.existing_contributors_json_file()
             if not file:
```

### Comparing `dcicutils-7.6.0.2b4/dcicutils/creds_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/data_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/deployment_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/diff_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/docker_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ecr_scripts.py` & `dcicutils-7.6.0.2b5/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ecr_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ecs_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/env_base.py` & `dcicutils-7.6.0.2b5/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/env_manager.py` & `dcicutils-7.6.0.2b5/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/env_scripts.py` & `dcicutils-7.6.0.2b5/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/env_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/env_utils_legacy.py` & `dcicutils-7.6.0.2b5/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/es_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/exceptions.py` & `dcicutils-7.6.0.2b5/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ff_mocks.py` & `dcicutils-7.6.0.2b5/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ff_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/function_cache_decorator.py` & `dcicutils-7.6.0.2b5/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/glacier_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/jh_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/kibana/dashboards.json` & `dcicutils-7.6.0.2b5/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/kibana/readme.md` & `dcicutils-7.6.0.2b5/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/lang_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/license_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/log_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/misc_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/obfuscation_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/opensearch_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/project_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/qa_checkers.py` & `dcicutils-7.6.0.2b5/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/qa_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/redis_tools.py` & `dcicutils-7.6.0.2b5/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/redis_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/s3_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.6.0.2b5/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/secrets_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/snapshot_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/task_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/dcicutils/trace_utils.py` & `dcicutils-7.6.0.2b5/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.6.0.2b4/pyproject.toml` & `dcicutils-7.6.0.2b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.6.0.2b4"
+version = "7.6.0.2b5"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -82,15 +82,17 @@
 publish-to-pypi = "dcicutils.scripts.publish_to_pypi:main"
 show-contributors = "dcicutils.contribution_scripts:show_contributors_main"
 
 [tool.pytest.ini_options]
 addopts = "--basetemp=/tmp/pytest"
 redis_exec = "/usr/local/bin/redis-server"
 filterwarnings = [
+    # TODO: These next two are about use of the Version class:
     "ignore:distutils Version classes are deprecated. Use packaging.version instead.:DeprecationWarning",
+    "ignore:Setuptools is replacing distutils.:UserWarning",
     # This is a pip-licenses problem (still present in 3.5.5):
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
     "ignore:Boto3 will no longer support Python 3.7 starting December 13, 2023.*:",
 ]
 markers = [
     "working: test should work",
     "integrated: an integration test",
```

### Comparing `dcicutils-7.6.0.2b4/setup.py` & `dcicutils-7.6.0.2b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 entry_points = \
 {'console_scripts': ['publish-to-pypi = dcicutils.scripts.publish_to_pypi:main',
                      'show-contributors = '
                      'dcicutils.contribution_scripts:show_contributors_main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.6.0.2b4',
+    'version': '7.6.0.2b5',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.6.0.2b4/PKG-INFO` & `dcicutils-7.6.0.2b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.6.0.2b4
+Version: 7.6.0.2b5
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

