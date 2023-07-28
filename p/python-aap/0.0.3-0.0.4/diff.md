# Comparing `tmp/python_aap-0.0.3.tar.gz` & `tmp/python_aap-0.0.4.tar.gz`

## Comparing `python_aap-0.0.3.tar` & `python_aap-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 python_aap-0.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.3/requirements.txt
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/__init__.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/__main__.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/base.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/endpoints.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.3/src/aap/mixins.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.3/.gitignore
--rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.3/LICENSE
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_aap-0.0.3/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 python_aap-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 python_aap-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 python_aap-0.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/__init__.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/__main__.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/base.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/endpoints.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.4/src/aap/mixins.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.4/.gitignore
+-rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.4/LICENSE
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_aap-0.0.4/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 python_aap-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 python_aap-0.0.4/PKG-INFO
```

### Comparing `python_aap-0.0.3/.gitlab-ci.yml` & `python_aap-0.0.4/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -84,11 +84,10 @@
   extends: .base
   stage: publish
   dependencies:
     - build job
   script:
    - pip3 install --upgrade twine
    - python3 -m twine upload  -u __token__ -p $PYPI_TOKEN dist/*
-  when: manual
   rules:
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
       when: on_success
```

### Comparing `python_aap-0.0.3/src/aap/__main__.py` & `python_aap-0.0.4/src/aap/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import argparse
 import json
 import urllib3
 
 from . import JobTemplate, API
 
 
-if __name__ == "__main__":
-
+def main():
     parser = argparse.ArgumentParser(
         description="Trigger jobs and workflows from terminal",
     )
     # More will be added later
     parser.add_argument("action", choices=["run-job"])
     parser.add_argument('-i', '--id', dest="id", action="store",
                         required=True, help="ID of job to run")
@@ -93,7 +92,11 @@
         job._reload()
 
     stdout = job.stdout.splitlines()
     if len(stdout) > last_line:
         print("\n".join(stdout[last_line:]))
         last_line = len(stdout)
     exit(not (job.is_successfull or args.ingore_fail))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `python_aap-0.0.3/src/aap/base.py` & `python_aap-0.0.4/src/aap/base.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.3/src/aap/endpoints.py` & `python_aap-0.0.4/src/aap/endpoints.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.3/src/aap/mixins.py` & `python_aap-0.0.4/src/aap/mixins.py`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.3/.gitignore` & `python_aap-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.3/LICENSE` & `python_aap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.3/pyproject.toml` & `python_aap-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 [project]
 name = "python-aap"
-version = "0.0.3"
+version = "0.0.4"
+dependencies = [
+  'requests',
+  'datetime'
+]
 authors = [
   { name="Ivan Mitruk", email="imitruk@redhat.com" },
 ]
 description = "Unofficial python wrapper over Ansible Automation Platform REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,8 +22,8 @@
 "Bug Tracker" = "https://gitlab.corp.redhat.com/network/python-aap/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project.scripts]
-python_aap = "aap"
+python_aap = "aap:main"
```

### Comparing `python_aap-0.0.3/PKG-INFO` & `python_aap-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: python-aap
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial python wrapper over Ansible Automation Platform REST API
 Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
 Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
 Author-email: Ivan Mitruk <imitruk@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: datetime
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
 ## Example
```

