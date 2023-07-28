# Comparing `tmp/shipyard_census-0.1.1a1.tar.gz` & `tmp/shipyard_census-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_census-0.1.1a1.tar", max compression
+gzip compressed data, was "shipyard_census-0.1.1a2.tar", max compression
```

## Comparing `shipyard_census-0.1.1a1.tar` & `shipyard_census-0.1.1a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      632 2023-07-28 02:40:03.357015 shipyard_census-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a1/shipyard_census/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-28 02:38:24.623706 shipyard_census-0.1.1a1/shipyard_census/census.py
--rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a1/shipyard_census/cli/authtest.py
--rw-r--r--   0        0        0     2808 2023-07-03 14:05:58.555641 shipyard_census-0.1.1a1/shipyard_census/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a1/shipyard_census/test/tests.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0      632 2023-07-28 02:43:54.080844 shipyard_census-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a2/shipyard_census/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-28 02:38:24.623706 shipyard_census-0.1.1a2/shipyard_census/census.py
+-rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a2/shipyard_census/cli/authtest.py
+-rw-r--r--   0        0        0     2787 2023-07-28 02:43:54.084731 shipyard_census-0.1.1a2/shipyard_census/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a2/shipyard_census/test/tests.py
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a2/PKG-INFO
```

### Comparing `shipyard_census-0.1.1a1/pyproject.toml` & `shipyard_census-0.1.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-census"
-version = "0.1.1a1"
+version = "0.1.1a2"
 description = "A local client for connecting and working with Census"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>","wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{include = "shipyard_census"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_census-0.1.1a1/shipyard_census/census.py` & `shipyard_census-0.1.1a2/shipyard_census/census.py`

 * *Files identical despite different names*

### Comparing `shipyard_census-0.1.1a1/shipyard_census/cli/trigger_sync_cli.py` & `shipyard_census-0.1.1a2/shipyard_census/cli/trigger_sync_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     parser.add_argument("--poke-interval", default=1)
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     census = CensusClient(args.access_token)
-    census.connect()
     try:
         trigger_sync = census.trigger_sync(args.sync_id)
     except ExitCodeException as error:
         census.logger.error(error)
         sys.exit(error.exit_code)
 
     sync_run_id = trigger_sync["data"]["sync_run_id"]
```

### Comparing `shipyard_census-0.1.1a1/PKG-INFO` & `shipyard_census-0.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-census
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A local client for connecting and working with Census
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

