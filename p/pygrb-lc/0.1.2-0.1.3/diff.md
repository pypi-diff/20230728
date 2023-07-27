# Comparing `tmp/pygrb_lc-0.1.2.tar.gz` & `tmp/pygrb_lc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.1.2.tar", last modified: Tue Jul 25 20:26:50 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.3.tar", last modified: Thu Jul 27 22:37:21 2023, max compression
```

## Comparing `pygrb_lc-0.1.2.tar` & `pygrb_lc-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.494186 pygrb_lc-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 20:26:50.000000 pygrb_lc-0.1.2/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:50.498186 pygrb_lc-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-25 20:26:41.000000 pygrb_lc-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:21.076946 pygrb_lc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 22:37:21.076946 pygrb_lc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 22:37:21.076946 pygrb_lc-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:21.068946 pygrb_lc-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:21.072946 pygrb_lc-0.1.3/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:21.076946 pygrb_lc-0.1.3/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 22:37:21.000000 pygrb_lc-0.1.3/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 22:37:21.000000 pygrb_lc-0.1.3/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:37:21.000000 pygrb_lc-0.1.3/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 22:37:21.000000 pygrb_lc-0.1.3/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:21.076946 pygrb_lc-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 22:37:09.000000 pygrb_lc-0.1.3/tests/test_utils.py
```

### Comparing `pygrb_lc-0.1.2/LICENSE` & `pygrb_lc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/PKG-INFO` & `pygrb_lc-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb_lc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.2/README.md` & `pygrb_lc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/setup.cfg` & `pygrb_lc-0.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.1.2
+version = 0.1.3
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.3/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/catalogs.py` & `pygrb_lc-0.1.3/src/pygrb_lc/catalogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     def crossmatch(self, other, precision: int = 5):
         '''
         Args:
             other (Catalog): instance of other catalog to match with
             precision (int, optional): precision of crossmatching in seconds
         '''
         for i,event in self.iterrows():
-            idx = self.find_event(event[self.event_column],other[other.event_column], precision)
+            idx = other.find_event(event[self.event_column], precision)
             if idx is not None:
                 for column in other.param_columns:
-                    column = column if column not in self.param_columns else column + '_other'
-                    self.loc[i,[column]] = other.iloc[idx][column]
+                    column_new = column if column not in self.param_columns else column + '_other'
+                    self.loc[self.index==i,[column_new]] = other.loc[other.index==idx,[column]].values
         return self
     
     def save(self, path):
         with open(path + '.pkl', 'wb') as f:
             pickle.dump(self, f)
 
     @classmethod
```

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/config.py` & `pygrb_lc-0.1.3/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.3/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.3/src/pygrb_lc/furie.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.3/src/pygrb_lc/light_curves.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/time.py` & `pygrb_lc-0.1.3/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.3/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.2/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.3/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.2/tests/test_utils.py` & `pygrb_lc-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

