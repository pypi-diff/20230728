# Comparing `tmp/pyintelx-0.2.2.tar.gz` & `tmp/pyintelx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.2.2.tar", last modified: Wed Jul 26 18:36:49 2023, max compression
+gzip compressed data, was "pyintelx-0.2.3.tar", last modified: Fri Jul 28 20:04:38 2023, max compression
```

## Comparing `pyintelx-0.2.2.tar` & `pyintelx-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 18:36:49.294386 pyintelx-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-26 18:36:38.000000 pyintelx-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/pyintelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:36:49.294386 pyintelx-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-26 18:36:38.000000 pyintelx-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-28 20:04:38.294822 pyintelx-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-28 20:04:28.000000 pyintelx-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/pyintelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:04:38.294822 pyintelx-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-28 20:04:28.000000 pyintelx-0.2.3/setup.py
```

### Comparing `pyintelx-0.2.2/PKG-INFO` & `pyintelx-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.2
+Version: 0.2.3
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pyintelx-0.2.2/README.md` & `pyintelx-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyintelx-0.2.2/pyintelx/cli/pyintelx` & `pyintelx-0.2.3/pyintelx/cli/pyintelx`

 * *Files identical despite different names*

### Comparing `pyintelx-0.2.2/pyintelx/pyintelx.py` & `pyintelx-0.2.3/pyintelx/pyintelx.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         }
         done = False
         results = []
         r = requests.get(self.API_ROOT + '/live/search/internal',
                          headers=self.HEADERS, params=p)
         if r.status_code == 200:
             search_id = r.json()['id']
+        else:
+            return (r.status_code, r.text)
         if (len(str(search_id)) <= 3):
             print(
                 f"[!] intelx.IDENTITY_SEARCH() Received {self.get_error(search_id)}")
         while not done:
             time.sleep(1)
             r = self.get_search_results(search_id, maxresults=maxresults)
             if (r["status"] == 0 and r["records"]):
```

### Comparing `pyintelx-0.2.2/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.2.3/pyintelx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.2
+Version: 0.2.3
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `pyintelx-0.2.2/setup.py` & `pyintelx-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 
 setup(
     name='pyintelx',
-    version='0.2.2',
+    version='0.2.3',
     description='This lib add support to use the Identity API from Intelx.io',
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Fermin Baudino, Einar Lanfranco, Federico Carrilao',
     url='https://github.com/csirtamericas/pyintelxio',
```

