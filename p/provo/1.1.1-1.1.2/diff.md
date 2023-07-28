# Comparing `tmp/provo-1.1.1.tar.gz` & `tmp/provo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provo-1.1.1.tar", last modified: Thu Jul 27 12:44:34 2023, max compression
+gzip compressed data, was "provo-1.1.2.tar", last modified: Fri Jul 28 07:58:55 2023, max compression
```

## Comparing `provo-1.1.1.tar` & `provo-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.989484 provo-1.1.1/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1070 2023-06-23 06:54:13.000000 provo-1.1.1/LICENSE
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-07-27 12:44:34.989484 provo-1.1.1/PKG-INFO
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25859 2023-07-27 11:28:09.000000 provo-1.1.1/README.md
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.985484 provo-1.1.1/provo/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       54 2023-06-23 06:54:13.000000 provo-1.1.1/provo/__init__.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3627 2023-06-26 15:24:38.000000 provo-1.1.1/provo/idvault.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    23251 2023-07-27 12:39:44.000000 provo-1.1.1/provo/provontologygraph.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    10519 2023-06-26 14:19:28.000000 provo-1.1.1/provo/startingpointclasses.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      572 2023-07-27 12:01:09.000000 provo-1.1.1/provo/staticfunctions.py
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.989484 provo-1.1.1/provo/tests/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/__init__.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1363 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/test_provenance_graph.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     4777 2023-06-26 15:25:26.000000 provo-1.1.1/provo/tests/test_rdf_output.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3332 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/test_starting_point_classes.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1423 2023-06-26 15:28:25.000000 provo-1.1.1/provo/tests/test_vault.py
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.985484 provo-1.1.1/provo.egg-info/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/PKG-INFO
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      448 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/SOURCES.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        1 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/dependency_links.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       23 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/requires.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        6 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/top_level.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       38 2023-07-27 12:44:34.989484 provo-1.1.1/setup.cfg
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      862 2023-07-27 12:44:22.000000 provo-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:58:55.116539 provo-1.1.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-23 06:54:13.000000 provo-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      529 2023-07-28 07:58:55.115540 provo-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25859 2023-07-27 11:28:09.000000 provo-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 07:58:55.083540 provo-1.1.2/provo/
+-rw-rw-rw-   0        0        0       54 2023-06-23 06:54:13.000000 provo-1.1.2/provo/__init__.py
+-rw-rw-rw-   0        0        0     3627 2023-06-26 15:24:38.000000 provo-1.1.2/provo/idvault.py
+-rw-rw-rw-   0        0        0    23269 2023-07-28 07:55:32.000000 provo-1.1.2/provo/provontologygraph.py
+-rw-rw-rw-   0        0        0    10519 2023-06-26 14:19:28.000000 provo-1.1.2/provo/startingpointclasses.py
+-rw-rw-rw-   0        0        0      572 2023-07-27 12:01:09.000000 provo-1.1.2/provo/staticfunctions.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:58:55.113542 provo-1.1.2/provo/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-23 06:54:13.000000 provo-1.1.2/provo/tests/__init__.py
+-rw-rw-rw-   0        0        0     1363 2023-06-23 06:54:13.000000 provo-1.1.2/provo/tests/test_provenance_graph.py
+-rw-rw-rw-   0        0        0     4777 2023-06-26 15:25:26.000000 provo-1.1.2/provo/tests/test_rdf_output.py
+-rw-rw-rw-   0        0        0     3332 2023-06-23 06:54:13.000000 provo-1.1.2/provo/tests/test_starting_point_classes.py
+-rw-rw-rw-   0        0        0     1423 2023-06-26 15:28:25.000000 provo-1.1.2/provo/tests/test_vault.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:58:55.104539 provo-1.1.2/provo.egg-info/
+-rw-rw-rw-   0        0        0      529 2023-07-28 07:58:55.000000 provo-1.1.2/provo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-28 07:58:55.000000 provo-1.1.2/provo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 07:58:55.000000 provo-1.1.2/provo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-28 07:58:55.000000 provo-1.1.2/provo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 07:58:55.000000 provo-1.1.2/provo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 07:58:55.117541 provo-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-07-28 07:56:27.000000 provo-1.1.2/setup.py
```

### Comparing `provo-1.1.1/LICENSE` & `provo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/PKG-INFO` & `provo-1.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: provo
-Version: 1.1.1
-Summary: Construct  PROV-O compliant provenance graphs.
-Home-page: https://github.com/rue-a/provo
-Author: Arne Rümmler
-Author-email: arne.ruemmler@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.09
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: provo
+Version: 1.1.2
+Summary: Construct  PROV-O compliant provenance graphs.
+Home-page: https://github.com/rue-a/provo
+Author: Arne Rümmler
+Author-email: arne.ruemmler@gmail.com
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.09
+License-File: LICENSE
```

### Comparing `provo-1.1.1/README.md` & `provo-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/idvault.py` & `provo-1.1.2/provo/idvault.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/provontologygraph.py` & `provo-1.1.2/provo/provontologygraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,9 +558,9 @@
                         lines.append(
                             f"{item.node_id}-{agent_stroke_style} <a {attrs}>instructed</a> {agent_stroke_style}->{agent.node_id}"
                         )
 
         lines.append("```")
         lines = "\n".join(lines)
 
-        with open(file_name, "w") as f:
+        with open(file_name, "w", encoding="utf-8") as f:
             f.write(lines)
```

### Comparing `provo-1.1.1/provo/startingpointclasses.py` & `provo-1.1.2/provo/startingpointclasses.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/staticfunctions.py` & `provo-1.1.2/provo/staticfunctions.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/tests/test_provenance_graph.py` & `provo-1.1.2/provo/tests/test_provenance_graph.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/tests/test_rdf_output.py` & `provo-1.1.2/provo/tests/test_rdf_output.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/tests/test_starting_point_classes.py` & `provo-1.1.2/provo/tests/test_starting_point_classes.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo/tests/test_vault.py` & `provo-1.1.2/provo/tests/test_vault.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.1/provo.egg-info/PKG-INFO` & `provo-1.1.2/provo.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: provo
-Version: 1.1.1
-Summary: Construct  PROV-O compliant provenance graphs.
-Home-page: https://github.com/rue-a/provo
-Author: Arne Rümmler
-Author-email: arne.ruemmler@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.09
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: provo
+Version: 1.1.2
+Summary: Construct  PROV-O compliant provenance graphs.
+Home-page: https://github.com/rue-a/provo
+Author: Arne Rümmler
+Author-email: arne.ruemmler@gmail.com
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.09
+License-File: LICENSE
```

### Comparing `provo-1.1.1/setup.py` & `provo-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 this_directory = Path(__file__).parent
 
 setup(
     name="provo",
     author="Arne Rümmler",
     author_email="arne.ruemmler@gmail.com",
-    version="1.1.1",
+    version="1.1.2",
     description="Construct  PROV-O compliant provenance graphs.",
     url="https://github.com/rue-a/provo",
     packages=find_packages(".", exclude=["tests", "tests.*"]),
     install_requires=["rdflib", "validators", "uuid"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

