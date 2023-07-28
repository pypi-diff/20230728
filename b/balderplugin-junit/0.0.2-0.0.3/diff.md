# Comparing `tmp/balderplugin-junit-0.0.2.tar.gz` & `tmp/balderplugin-junit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balderplugin-junit-0.0.2.tar", last modified: Sat Jan 21 19:53:29 2023, max compression
+gzip compressed data, was "balderplugin-junit-0.0.3.tar", last modified: Fri Jul 28 07:24:16 2023, max compression
```

## Comparing `balderplugin-junit-0.0.2.tar` & `balderplugin-junit-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-01-21 19:53:29.219159 balderplugin-junit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-21 19:53:29.219159 balderplugin-junit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/src/balderplugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/src/balderplugin/junit/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/src/balderplugin/junit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin/junit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-01-21 19:53:17.000000 balderplugin-junit-0.0.2/src/balderplugin/junit/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 19:53:29.215159 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-21 19:53:29.000000 balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.037557 balderplugin-junit-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.037557 balderplugin-junit-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.037557 balderplugin-junit-0.0.3/src/balderplugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/src/balderplugin/junit/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/src/balderplugin/junit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 07:24:15.000000 balderplugin-junit-0.0.3/src/balderplugin/junit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-28 07:23:56.000000 balderplugin-junit-0.0.3/src/balderplugin/junit/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:24:16.041557 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 07:24:16.000000 balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/top_level.txt
```

### Comparing `balderplugin-junit-0.0.2/.github/workflows/python-publish.yml` & `balderplugin-junit-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `balderplugin-junit-0.0.2/.gitignore` & `balderplugin-junit-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `balderplugin-junit-0.0.2/LICENSE` & `balderplugin-junit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `balderplugin-junit-0.0.2/PKG-INFO` & `balderplugin-junit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balderplugin-junit
-Version: 0.0.2
+Version: 0.0.3
 Summary: balderplugin-junit: plugin to generate junit file reports for the balder test framework
 Home-page: https://docs.balder.dev
 Author: Max Stahlschmidt and others
 License: MIT
 Project-URL: Source, https://github.com/balder-dev/balderplugin-junit
 Project-URL: Tracker, https://github.com/balder-dev/balderplugin-junit/issues
 Keywords: test,systemtest,reusable,scenario,junit,balder
```

### Comparing `balderplugin-junit-0.0.2/README.md` & `balderplugin-junit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `balderplugin-junit-0.0.2/setup.cfg` & `balderplugin-junit-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	Source=https://github.com/balder-dev/balderplugin-junit
 	Tracker=https://github.com/balder-dev/balderplugin-junit/issues
 
 [options]
 packages = 
 	balderplugin.junit
 install_requires = 
-	baldertest>=0.1.0b3
+	baldertest>=0.1.0b7
 	junit-xml>=1.9
 python_requires = >=3.9
 package_dir = 
 	=src
 setup_requires = 
 	setuptools
 	setuptools-scm>=6.0
```

### Comparing `balderplugin-junit-0.0.2/src/balderplugin/junit/plugin.py` & `balderplugin-junit-0.0.3/src/balderplugin/junit/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         return test_case
 
     def session_finished(self, executor_tree: Union[ExecutorTree, None]):
         filepath_str = self.balder_session.parsed_args.junit_file
         if executor_tree is not None and filepath_str is not None:
             filepath = pathlib.Path(filepath_str)
             all_test_suites = []
-            for cur_setup_executor in executor_tree.setup_executors:
-                for cur_scenario_executor in cur_setup_executor.scenario_executors:
-                    for cur_variation_executor in cur_scenario_executor.variation_executors:
+            for cur_setup_executor in executor_tree.get_setup_executors():
+                for cur_scenario_executor in cur_setup_executor.get_scenario_executors():
+                    for cur_variation_executor in cur_scenario_executor.get_variation_executors():
                         all_testcases = []
-                        for cur_test_case_executor in cur_variation_executor.testcase_executors:
+                        for cur_test_case_executor in cur_variation_executor.get_testcase_executors():
                             test_case = self.create_test_case(cur_test_case_executor)
                             all_testcases.append(test_case)
 
                         mapping_str = "|".join(
                             [f"{cur_scenario_dev.__name__}:{cur_setup_dev.__name__}"
                              for cur_scenario_dev, cur_setup_dev in cur_variation_executor.base_device_mapping.items()])
                         suite_name = f"{cur_scenario_executor.base_scenario_class.__class__.__qualname__}:" \
```

### Comparing `balderplugin-junit-0.0.2/src/balderplugin_junit.egg-info/PKG-INFO` & `balderplugin-junit-0.0.3/src/balderplugin_junit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balderplugin-junit
-Version: 0.0.2
+Version: 0.0.3
 Summary: balderplugin-junit: plugin to generate junit file reports for the balder test framework
 Home-page: https://docs.balder.dev
 Author: Max Stahlschmidt and others
 License: MIT
 Project-URL: Source, https://github.com/balder-dev/balderplugin-junit
 Project-URL: Tracker, https://github.com/balder-dev/balderplugin-junit/issues
 Keywords: test,systemtest,reusable,scenario,junit,balder
```

