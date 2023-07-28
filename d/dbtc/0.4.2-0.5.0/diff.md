# Comparing `tmp/dbtc-0.4.2.tar.gz` & `tmp/dbtc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtc-0.4.2.tar", max compression
+gzip compressed data, was "dbtc-0.5.0.tar", max compression
```

## Comparing `dbtc-0.4.2.tar` & `dbtc-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3872 2023-04-04 04:26:36.364810 dbtc-0.4.2/README.md
--rw-r--r--   0        0        0      124 2023-04-04 04:26:36.364810 dbtc-0.4.2/dbtc/__init__.py
--rw-r--r--   0        0        0       22 2023-04-04 04:26:36.364810 dbtc-0.4.2/dbtc/_version.py
--rw-r--r--   0        0        0    37445 2023-04-04 04:26:36.364810 dbtc-0.4.2/dbtc/cli.py
--rw-r--r--   0        0        0        0 2023-04-04 04:26:36.364810 dbtc-0.4.2/dbtc/client/__init__.py
--rw-r--r--   0        0        0    63656 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/admin.py
--rw-r--r--   0        0        0   352525 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/artifacts/metadata_schema.json
--rw-r--r--   0        0        0     2349 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/base.py
--rw-r--r--   0        0        0      258 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/main.py
--rw-r--r--   0        0        0    24548 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/metadata.py
--rw-r--r--   0        0        0    62305 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/client/schema.py
--rw-r--r--   0        0        0      103 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/console.py
--rw-r--r--   0        0        0       44 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/models/__init__.py
--rw-r--r--   0        0        0      524 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/models/webhooks.py
--rw-r--r--   0        0        0      428 2023-04-04 04:26:36.368810 dbtc-0.4.2/dbtc/utils.py
--rw-r--r--   0        0        0      905 2023-04-04 04:26:55.600813 dbtc-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 dbtc-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3872 2023-07-28 12:01:04.602736 dbtc-0.5.0/README.md
+-rw-r--r--   0        0        0      124 2023-07-28 12:01:04.602736 dbtc-0.5.0/dbtc/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/_version.py
+-rw-r--r--   0        0        0    37445 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/cli.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/__init__.py
+-rw-r--r--   0        0        0    64405 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/admin.py
+-rw-r--r--   0        0        0   352525 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/artifacts/metadata_schema.json
+-rw-r--r--   0        0        0     2349 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/base.py
+-rw-r--r--   0        0        0      258 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/main.py
+-rw-r--r--   0        0        0    24548 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/metadata.py
+-rw-r--r--   0        0        0    62305 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/client/schema.py
+-rw-r--r--   0        0        0      103 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/console.py
+-rw-r--r--   0        0        0       44 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/models/webhooks.py
+-rw-r--r--   0        0        0      428 2023-07-28 12:01:04.606736 dbtc-0.5.0/dbtc/utils.py
+-rw-r--r--   0        0        0      905 2023-07-28 12:01:19.090560 dbtc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4731 1970-01-01 00:00:00.000000 dbtc-0.5.0/PKG-INFO
```

### Comparing `dbtc-0.4.2/README.md` & `dbtc-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/cli.py` & `dbtc-0.5.0/dbtc/cli.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/client/admin.py` & `dbtc-0.5.0/dbtc/client/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,26 +167,27 @@
         return self._simple_request(
             f'accounts/{account_id}/service-tokens/{service_token_id}/permissions/',
             method='post',
             json=payload,
         )
 
     @v3
-    def assign_user_to_group(
-        self, account_id: int, project_id: int, payload: Dict
-    ) -> Dict:
+    def assign_user_to_group(self, account_id: int, payload: Dict) -> Dict:
         """Assign a user to a group
 
         Args:
             account_id (int): Numeric ID of the account
-            project_id (int): Numeric ID of the project
             payload (dict): Dictionary representing the user to assign
+            {
+                "user_id": int,
+                "desired_group_ids": list(int)
+            }
         """
         return self._simple_request(
-            f'accounts/{account_id}/projects/{project_id}/assign-groups/',
+            f'accounts/{account_id}/assign-groups/',
             method='post',
             json=payload,
         )
 
     @v2
     def cancel_run(self, account_id: int, run_id: int) -> Dict:
         """Cancel a run.
@@ -508,24 +509,32 @@
         """
         return self._simple_request(
             f'accounts/{account_id}/webhooks/subscription/{webhook_id}',
             method='delete',
         )
 
     @v3
-    def delete_user_group(self, account_id: int, group_id: int) -> Dict:
+    def delete_user_group(self, account_id: int, group_id: int, payload: Dict) -> Dict:
         """Delete group for a specified account
 
         Args:
             account_id (int): Numeric ID of the account
             group_id (int): Numeric ID of the group to delete
+            payload (dict): Dictionary representing the group to delete with the format
+                {
+                    "account_id": int,
+                    "name": str,
+                    "id": int,
+                    "state":2,
+                    "assign_by_default":false,
+                    "sso_mapping_groups": list
+                }
         """
         return self._simple_request(
-            f'accounts/{account_id}/groups/{group_id}/',
-            method='post',
+            f'accounts/{account_id}/groups/{group_id}/', method='post', payload=payload
         )
 
     @v2
     def get_account(self, account_id: int) -> Dict:
         """Get an account by its ID.
 
         Args:
@@ -1440,24 +1449,31 @@
                     if isinstance(value, bool):
                         string += f' --{arg}'
                     else:
                         string += f" --{arg} '{value}'"
             return string
 
         self.console.log(f'Restarting job {job_id} from last failed state.')
-        last_run_data = self.list_runs(
-            account_id=account_id,
-            include_related=['run_steps'],
-            job_definition_id=job_id,
-            order_by='-id',
-            limit=1,
-        )['data'][0]
+        try:
+            last_run_data = self.list_runs(
+                account_id=account_id,
+                include_related=['run_steps'],
+                job_definition_id=job_id,
+                order_by='-id',
+                limit=1,
+            )['data'][0]
+
+        # this happens when there are no prior runs of a job
+        except IndexError:
+            self.console.log(f'no prior runs of job_id {job_id}')
+            last_run_status = None
 
-        last_run_status = last_run_data['status_humanized'].lower()
-        last_run_id = last_run_data['id']
+        else:
+            last_run_status = last_run_data['status_humanized'].lower()
+            last_run_id = last_run_data['id']
 
         if last_run_status == 'error':
             rerun_steps = []
             job_info = self.get_job(account_id, job_id)['data']
             generate_docs = job_info.get('generate_docs', False)
             generate_sources = job_info.get('generate_sources', False)
             for run_step in last_run_data['run_steps']:
@@ -1544,16 +1560,20 @@
 
         else:
             self.console.log(
                 'Process triggered with restart_from_failure set to True but no '
                 'failed run steps found.'
             )
             if trigger_on_failure_only:
-                self.console.log('Not triggering job because prior run was successful.')
+                self.console.log(
+                    'Not triggering job because prior run was successful or there is '
+                    'no prior run, and trigger_on_failure_only set to True'
+                )
                 return
+
         run = self.trigger_job(
             account_id,
             job_id,
             payload,
             should_poll=should_poll,
             poll_interval=poll_interval,
         )
```

### Comparing `dbtc-0.4.2/dbtc/client/artifacts/metadata_schema.json` & `dbtc-0.5.0/dbtc/client/artifacts/metadata_schema.json`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/client/base.py` & `dbtc-0.5.0/dbtc/client/base.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/client/metadata.py` & `dbtc-0.5.0/dbtc/client/metadata.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/client/schema.py` & `dbtc-0.5.0/dbtc/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/dbtc/models/webhooks.py` & `dbtc-0.5.0/dbtc/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.4.2/pyproject.toml` & `dbtc-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbtc"
-version = "0.4.2"
+version = "0.5.0"
 description = "An unaffiliated python wrapper for dbt Cloud APIs"
 authors = ["Doug Guthrie <douglas.p.guthrie@gmail.com>"]
 documentation = "https://dbtc.dpguthrie.com"
 keywords=["dbt", "requests", "API", "dbt Cloud"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dbtc-0.4.2/PKG-INFO` & `dbtc-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtc
-Version: 0.4.2
+Version: 0.5.0
 Summary: An unaffiliated python wrapper for dbt Cloud APIs
 License: MIT
 Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie
 Author-email: douglas.p.guthrie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbtc Version: 0.4.2 Summary: An unaffiliated python
+Metadata-Version: 2.1 Name: dbtc Version: 0.5.0 Summary: An unaffiliated python
 wrapper for dbt Cloud APIs License: MIT Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie Author-email: douglas.p.guthrie@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist:
```

