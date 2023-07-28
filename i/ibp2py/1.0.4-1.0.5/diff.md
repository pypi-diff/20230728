# Comparing `tmp/Ibp2py-1.0.4.tar.gz` & `tmp/ibp2py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ibp2py-1.0.4.tar", last modified: Thu Jul 27 04:26:11 2023, max compression
+gzip compressed data, was "ibp2py-1.0.5.tar", last modified: Fri Jul 28 17:55:50 2023, max compression
```

## Comparing `Ibp2py-1.0.4.tar` & `ibp2py-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.995810 Ibp2py-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.958810 Ibp2py-1.0.4/Ibp2py.egg-info/
--rw-rw-rw-   0        0        0     2857 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 Ibp2py-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2857 2023-07-27 04:26:10.991808 Ibp2py-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 Ibp2py-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.981807 Ibp2py-1.0.4/ibp2py/
--rw-rw-rw-   0        0        0    21802 2023-07-27 01:39:48.000000 Ibp2py-1.0.4/ibp2py/Ibp2py.py
--rw-rw-rw-   0        0        0       23 2023-07-27 04:25:52.000000 Ibp2py-1.0.4/ibp2py/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 Ibp2py-1.0.4/ibp2py/teste.py
--rw-rw-rw-   0        0        0       42 2023-07-27 04:26:10.997807 Ibp2py-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-07-27 04:26:00.000000 Ibp2py-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:55:50.790264 ibp2py-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-28 17:55:50.747260 ibp2py-1.0.5/Ibp2py.egg-info/
+-rw-rw-rw-   0        0        0     2857 2023-07-28 17:55:50.000000 ibp2py-1.0.5/Ibp2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-28 17:55:50.000000 ibp2py-1.0.5/Ibp2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:55:50.000000 ibp2py-1.0.5/Ibp2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-28 17:55:50.000000 ibp2py-1.0.5/Ibp2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 17:55:50.000000 ibp2py-1.0.5/Ibp2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 ibp2py-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2857 2023-07-28 17:55:50.783262 ibp2py-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 ibp2py-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:55:50.777260 ibp2py-1.0.5/ibp2py/
+-rw-rw-rw-   0        0        0    21802 2023-07-28 17:33:32.000000 ibp2py-1.0.5/ibp2py/Ibp2py.py
+-rw-rw-rw-   0        0        0       28 2023-07-28 17:55:35.000000 ibp2py-1.0.5/ibp2py/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 ibp2py-1.0.5/ibp2py/teste.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:55:50.790264 ibp2py-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-07-28 17:55:30.000000 ibp2py-1.0.5/setup.py
```

### Comparing `Ibp2py-1.0.4/Ibp2py.egg-info/PKG-INFO` & `ibp2py-1.0.5/Ibp2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Ibp2py
-Version: 1.0.4
+Name: ibp2py
+Version: 1.0.5
 Summary: SAP Data Retrieval and Processing Library for IBP
 Home-page: https://github.com/pedrorastha/ibp2py
 Author: Pedro Rastha
 Author-email: pedrorastha@gmail.com
 Keywords: SAP IBP API ODATA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Ibp2py-1.0.4/LICENSE` & `ibp2py-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.4/PKG-INFO` & `ibp2py-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Ibp2py
-Version: 1.0.4
+Name: ibp2py
+Version: 1.0.5
 Summary: SAP Data Retrieval and Processing Library for IBP
 Home-page: https://github.com/pedrorastha/ibp2py
 Author: Pedro Rastha
 Author-email: pedrorastha@gmail.com
 Keywords: SAP IBP API ODATA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Ibp2py-1.0.4/README.md` & `ibp2py-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.4/ibp2py/Ibp2py.py` & `ibp2py-1.0.5/ibp2py/Ibp2py.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from pathlib import Path  # Import pathlib to work with file paths
 import json
 import logging
 
 # Set up logging with a basic configuration
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
-class Ibp2py:
+class ibp2py:
     """
     A class used to interact with SAP IBP.
 
     Attributes
     ----------
     username : str
         The username for Communication Users.
```

### Comparing `Ibp2py-1.0.4/ibp2py/teste.py` & `ibp2py-1.0.5/ibp2py/teste.py`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.4/setup.py` & `ibp2py-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open ('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(
-    name='Ibp2py',
-    version='1.0.4',
+    name='ibp2py',
+    version='1.0.5',
     author='Pedro Rastha',
     author_email='pedrorastha@gmail.com',
     description='SAP Data Retrieval and Processing Library for IBP',
-    long_description=f'{readme}',
+    long_description= readme,
     long_description_content_type='text/markdown',
     url='https://github.com/pedrorastha/ibp2py',
     keywords='SAP IBP API ODATA',
     packages=['ibp2py'],
     install_requires=[
         'requests>=2.28.1',
         'pandas>=1.5.2',
```

