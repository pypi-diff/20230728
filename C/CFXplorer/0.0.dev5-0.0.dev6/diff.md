# Comparing `tmp/CFXplorer-0.0.dev5.tar.gz` & `tmp/CFXplorer-0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CFXplorer-0.0.dev5.tar", last modified: Thu Jul 27 21:52:51 2023, max compression
+gzip compressed data, was "CFXplorer-0.0.dev6.tar", last modified: Thu Jul 27 22:00:34 2023, max compression
```

## Comparing `CFXplorer-0.0.dev5.tar` & `CFXplorer-0.0.dev6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:52:51.001559 CFXplorer-0.0.dev5/
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:52:50.996842 CFXplorer-0.0.dev5/CFXplorer.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:52:50.000000 CFXplorer-0.0.dev5/CFXplorer.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      300 2023-07-27 21:52:50.000000 CFXplorer-0.0.dev5/CFXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 21:52:50.000000 CFXplorer-0.0.dev5/CFXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 21:52:50.000000 CFXplorer-0.0.dev5/CFXplorer.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev5/LICENSE
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:52:51.001770 CFXplorer-0.0.dev5/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev5/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:52:50.997959 CFXplorer-0.0.dev5/cfxplorer/
--rw-r--r--   0 kyosuke    (501) staff       (20)      603 2023-07-27 21:51:43.000000 CFXplorer-0.0.dev5/cfxplorer/__init__.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:52:51.001108 CFXplorer-0.0.dev5/cfxplorer/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev5/cfxplorer/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev5/cfxplorer/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev5/cfxplorer/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 21:52:48.000000 CFXplorer-0.0.dev5/cfxplorer/version.py
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 21:52:51.002480 CFXplorer-0.0.dev5/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev5/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:00:34.574643 CFXplorer-0.0.dev6/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:00:34.571528 CFXplorer-0.0.dev6/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 22:00:34.000000 CFXplorer-0.0.dev6/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      300 2023-07-27 22:00:34.000000 CFXplorer-0.0.dev6/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 22:00:34.000000 CFXplorer-0.0.dev6/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 22:00:34.000000 CFXplorer-0.0.dev6/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev6/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 22:00:34.574782 CFXplorer-0.0.dev6/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev6/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:00:34.572652 CFXplorer-0.0.dev6/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      603 2023-07-27 21:51:43.000000 CFXplorer-0.0.dev6/cfxplorer/__init__.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:00:34.574090 CFXplorer-0.0.dev6/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev6/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev6/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev6/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 22:00:30.000000 CFXplorer-0.0.dev6/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 22:00:34.575292 CFXplorer-0.0.dev6/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1550 2023-07-27 22:00:00.000000 CFXplorer-0.0.dev6/setup.py
```

### Comparing `CFXplorer-0.0.dev5/CFXplorer.egg-info/PKG-INFO` & `CFXplorer-0.0.dev6/CFXplorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0.dev5
+Version: 0.0.dev6
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CFXplorer-0.0.dev5/LICENSE` & `CFXplorer-0.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev5/PKG-INFO` & `CFXplorer-0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0.dev5
+Version: 0.0.dev6
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CFXplorer-0.0.dev5/README.rst` & `CFXplorer-0.0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev5/cfxplorer/__init__.py` & `CFXplorer-0.0.dev6/cfxplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev5/cfxplorer/tests/test_focus.py` & `CFXplorer-0.0.dev6/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev5/cfxplorer/tests/test_utils.py` & `CFXplorer-0.0.dev6/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev5/cfxplorer/version.py` & `CFXplorer-0.0.dev6/cfxplorer/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev5"  # pragma: no cover
+__version__ = "0.0.dev6"  # pragma: no cover
```

### Comparing `CFXplorer-0.0.dev5/setup.py` & `CFXplorer-0.0.dev6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 # read the contents of README.rst
 def readme():
     with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
         return f.read()
 
 
-# read the contents of requirements.txt
-with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
-    requirements = f.read().splitlines()
+# # read the contents of requirements.txt
+# with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
+#     requirements = f.read().splitlines()
 
 setup(
     name="CFXplorer",
     version=__version__,
     author="Kyosuke Morita",
     author_email="kq441morita@gmail.com",
     description=DESCRIPTION,
```

