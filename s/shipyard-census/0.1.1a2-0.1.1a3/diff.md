# Comparing `tmp/shipyard_census-0.1.1a2.tar.gz` & `tmp/shipyard_census-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_census-0.1.1a2.tar", max compression
+gzip compressed data, was "shipyard_census-0.1.1a3.tar", max compression
```

## Comparing `shipyard_census-0.1.1a2.tar` & `shipyard_census-0.1.1a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      632 2023-07-28 02:43:54.080844 shipyard_census-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a2/shipyard_census/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-28 02:38:24.623706 shipyard_census-0.1.1a2/shipyard_census/census.py
--rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a2/shipyard_census/cli/authtest.py
--rw-r--r--   0        0        0     2787 2023-07-28 02:43:54.084731 shipyard_census-0.1.1a2/shipyard_census/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a2/shipyard_census/test/tests.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0      632 2023-07-28 02:48:32.865997 shipyard_census-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a3/shipyard_census/__init__.py
+-rw-r--r--   0        0        0     5852 2023-07-28 02:46:43.842558 shipyard_census-0.1.1a3/shipyard_census/census.py
+-rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a3/shipyard_census/cli/authtest.py
+-rw-r--r--   0        0        0     2844 2023-07-28 02:48:25.059554 shipyard_census-0.1.1a3/shipyard_census/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a3/shipyard_census/test/tests.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a3/PKG-INFO
```

### Comparing `shipyard_census-0.1.1a2/pyproject.toml` & `shipyard_census-0.1.1a3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-census"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = "A local client for connecting and working with Census"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>","wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{include = "shipyard_census"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_census-0.1.1a2/shipyard_census/census.py` & `shipyard_census-0.1.1a3/shipyard_census/census.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,28 @@
         try:
             response = request(method, url, headers=self.api_headers)
         except Exception as error:
             self.logger.exception(f"Request to {url} failed")
             raise ExitCodeException(error, self.EXIT_CODE_UNKNOWN_ERROR) from error
 
         if response.ok:
-            self.logger.info("Request successful")
             return response.json()
-        else:
         # self.logger.debug(f"Request failed with status code {response.status_code}")
-            if response.status_code == 401:
-                raise ExitCodeException(
-                    response.text, self.EXIT_CODE_INVALID_CREDENTIALS
-                )
-            elif response.status_code == 404:
-                raise ExitCodeException(response.text, self.EXIT_CODE_BAD_REQUEST)
-            elif response.status_code == 409:
-                raise ExitCodeException(
-                    response.text, self.EXIT_CODE_SYNC_ALREADY_RUNNING
-                )
-            else:
-                raise ExitCodeException(response.text, self.EXIT_CODE_UNKNOWN_ERROR)
+        if response.status_code == 401:
+            raise ExitCodeException(
+                response.text, self.EXIT_CODE_INVALID_CREDENTIALS
+            )
+        elif response.status_code == 404:
+            raise ExitCodeException(response.text, self.EXIT_CODE_BAD_REQUEST)
+        elif response.status_code == 409:
+            raise ExitCodeException(
+                response.text, self.EXIT_CODE_SYNC_ALREADY_RUNNING
+            )
+        else:
+            raise ExitCodeException(response.text, self.EXIT_CODE_UNKNOWN_ERROR)
 
     def get_sync_status(self, sync_run_id: str) -> dict:
         """
         Get information about a specific sync run.
 
         Args:
             sync_run_id (str): The ID of the sync run.
```

### Comparing `shipyard_census-0.1.1a2/shipyard_census/cli/trigger_sync_cli.py` & `shipyard_census-0.1.1a3/shipyard_census/cli/trigger_sync_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,19 +58,19 @@
             sys.exit(census.EXIT_CODE_INVALID_POKE_INTERVAL)
 
         status = None
         while status != "completed":
             try:
                 sync_run_data = census.get_sync_status(sync_run_id)
                 status = census.determine_sync_status(sync_run_data)
-
-                census.logger.info(
-                    f"Waiting {poke_interval} minute(s) to check sync status..."
-                )
-                time.sleep(poke_interval * 60)
+                if status != "completed":
+                    census.logger.info(
+                        f"Waiting {poke_interval} minute(s) to check sync status..."
+                    )
+                    time.sleep(poke_interval * 60)
             except ExitCodeException as error:
                 census.logger.error(error)
                 sys.exit(error.exit_code)
 
     elif not wait and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0:
         # Create the artifact for legacy blueprints to continue to work
         create_artifact(sync_run_id)
```

### Comparing `shipyard_census-0.1.1a2/PKG-INFO` & `shipyard_census-0.1.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-census
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A local client for connecting and working with Census
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

