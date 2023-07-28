# Comparing `tmp/python_aap-0.0.2.tar.gz` & `tmp/python_aap-0.0.3.tar.gz`

## Comparing `python_aap-0.0.2.tar` & `python_aap-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 python_aap-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.2/requirements.txt
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/__init__.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/__main__.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/base.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/endpoints.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/mixins.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.2/.gitignore
--rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.2/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_aap-0.0.2/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 python_aap-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 python_aap-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 python_aap-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/__init__.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/__main__.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/base.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/endpoints.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/mixins.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.3/.gitignore
+-rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.3/LICENSE
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_aap-0.0.3/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 python_aap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 python_aap-0.0.3/PKG-INFO
```

### Comparing `python_aap-0.0.2/.gitlab-ci.yml` & `python_aap-0.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/src/aap/__main__.py` & `python_aap-0.0.3/src/aap/__main__.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/src/aap/base.py` & `python_aap-0.0.3/src/aap/base.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/src/aap/endpoints.py` & `python_aap-0.0.3/src/aap/endpoints.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/src/aap/mixins.py` & `python_aap-0.0.3/src/aap/mixins.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/.gitignore` & `python_aap-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/LICENSE` & `python_aap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.2/PKG-INFO` & `python_aap-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial python wrapper over Ansible Automation Platform REST API
 Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
 Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
 Author-email: Ivan Mitruk <imitruk@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -16,9 +16,9 @@
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
 ## Example
 
 Python module can be invoked directly to execute job in aap and report status to terminal.
 ```
-/bin/python3.8 -m aap run-job --id <job-id> -f
+python_aap run-job --id <job-id> -f
 ```
```

