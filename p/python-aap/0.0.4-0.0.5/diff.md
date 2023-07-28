# Comparing `tmp/python_aap-0.0.4.tar.gz` & `tmp/python-aap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "python-aap-0.0.5.tar", last modified: Fri Jul 28 12:59:27 2023, max compression
```

## Comparing `python_aap-0.0.4.tar` & `python-aap-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,23 @@
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 python_aap-0.0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.4/requirements.txt
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/__init__.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/__main__.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/base.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/endpoints.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/mixins.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.4/.gitignore
--rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.4/LICENSE
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_aap-0.0.4/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 python_aap-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 python_aap-0.0.4/PKG-INFO
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-28 12:59:27.068884 python-aap-0.0.5/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     2735 2023-07-28 11:04:18.000000 python-aap-0.0.5/.gitignore
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1963 2023-07-28 12:41:32.000000 python-aap-0.0.5/.gitlab-ci.yml
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)    18020 2023-07-26 20:20:58.000000 python-aap-0.0.5/LICENSE
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      856 2023-07-28 12:59:27.068884 python-aap-0.0.5/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      262 2023-07-28 12:25:55.000000 python-aap-0.0.5/README.md
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      817 2023-07-28 12:59:12.000000 python-aap-0.0.5/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       17 2023-07-28 11:04:18.000000 python-aap-0.0.5/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       38 2023-07-28 12:59:27.068884 python-aap-0.0.5/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-28 12:59:27.063884 python-aap-0.0.5/src/
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-28 12:59:27.066884 python-aap-0.0.5/src/aap/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      265 2023-07-28 12:41:32.000000 python-aap-0.0.5/src/aap/__init__.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     4036 2023-07-28 12:41:32.000000 python-aap-0.0.5/src/aap/__main__.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     5364 2023-07-28 12:41:32.000000 python-aap-0.0.5/src/aap/base.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3090 2023-07-28 12:41:32.000000 python-aap-0.0.5/src/aap/endpoints.py
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1901 2023-07-28 12:41:32.000000 python-aap-0.0.5/src/aap/mixins.py
+drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-28 12:59:27.067884 python-aap-0.0.5/src/python_aap.egg-info/
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      856 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      400 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        1 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       40 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       18 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        4 2023-07-28 12:59:27.000000 python-aap-0.0.5/src/python_aap.egg-info/top_level.txt
```

### Comparing `python_aap-0.0.4/.gitlab-ci.yml` & `python-aap-0.0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/src/aap/__main__.py` & `python-aap-0.0.5/src/aap/__main__.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/src/aap/base.py` & `python-aap-0.0.5/src/aap/base.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/src/aap/endpoints.py` & `python-aap-0.0.5/src/aap/endpoints.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/src/aap/mixins.py` & `python-aap-0.0.5/src/aap/mixins.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/.gitignore` & `python-aap-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/LICENSE` & `python-aap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.4/pyproject.toml` & `python-aap-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-aap"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
   'requests',
   'datetime'
 ]
 authors = [
   { name="Ivan Mitruk", email="imitruk@redhat.com" },
 ]
@@ -13,17 +13,20 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [project.urls]
 "Homepage" = "https://gitlab.corp.redhat.com/network/python-aap/"
 "Bug Tracker" = "https://gitlab.corp.redhat.com/network/python-aap/issues"
 
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
 
 [project.scripts]
 python_aap = "aap:main"
```

### Comparing `python_aap-0.0.4/PKG-INFO` & `python-aap-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: python-aap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unofficial python wrapper over Ansible Automation Platform REST API
+Author-email: Ivan Mitruk <imitruk@redhat.com>
 Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
 Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
-Author-email: Ivan Mitruk <imitruk@redhat.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: datetime
-Requires-Dist: requests
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
 ## Example
 
 Python module can be invoked directly to execute job in aap and report status to terminal.
 ```
 python_aap run-job --id <job-id> -f
-```
+```
```

