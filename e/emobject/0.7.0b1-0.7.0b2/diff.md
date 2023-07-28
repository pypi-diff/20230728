# Comparing `tmp/emobject-0.7.0b1.tar.gz` & `tmp/emobject-0.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.0b1.tar", last modified: Fri Jul 28 13:32:58 2023, max compression
+gzip compressed data, was "emobject-0.7.0b2.tar", last modified: Fri Jul 28 18:21:39 2023, max compression
```

## Comparing `emobject-0.7.0b1.tar` & `emobject-0.7.0b2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 13:32:58.908859 emobject-0.7.0b1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-07-28 13:21:45.000000 emobject-0.7.0b1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-07-28 13:32:58.908859 emobject-0.7.0b1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3826 2023-07-28 13:21:45.000000 emobject-0.7.0b1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 13:32:58.904858 emobject-0.7.0b1/emobject/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40016 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15643 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/database.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32512 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/emexperiment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14806 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/emimage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9750 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/emlayer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49374 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/emobject.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6759 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/empublicaccess.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9493 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/emroitools.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/errors.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 13:32:58.908859 emobject-0.7.0b1/emobject/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3543 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/utils/graph.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2447 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24111 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/utils/io.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11201 2023-07-28 13:21:45.000000 emobject-0.7.0b1/emobject/utils/visualization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-07-28 13:32:49.000000 emobject-0.7.0b1/emobject/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 13:32:58.904858 emobject-0.7.0b1/emobject.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-07-28 13:32:58.000000 emobject-0.7.0b1/emobject.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      559 2023-07-28 13:32:58.000000 emobject-0.7.0b1/emobject.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-28 13:32:58.000000 emobject-0.7.0b1/emobject.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      229 2023-07-28 13:32:58.000000 emobject-0.7.0b1/emobject.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-28 13:32:58.000000 emobject-0.7.0b1/emobject.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2023-07-28 13:32:58.908859 emobject-0.7.0b1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1263 2023-07-28 13:22:28.000000 emobject-0.7.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.592228 emobject-0.7.0b2/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 18:21:30.000000 emobject-0.7.0b2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:21:39.592228 emobject-0.7.0b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 18:21:30.000000 emobject-0.7.0b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.590228 emobject-0.7.0b2/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    40016 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.592228 emobject-0.7.0b2/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 18:21:30.000000 emobject-0.7.0b2/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:21:39.591228 emobject-0.7.0b2/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 18:21:39.000000 emobject-0.7.0b2/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 18:21:39.593228 emobject-0.7.0b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 18:21:30.000000 emobject-0.7.0b2/setup.py
```

### Comparing `emobject-0.7.0b1/LICENSE` & `emobject-0.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/PKG-INFO` & `emobject-0.7.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b1
+Version: 0.7.0b2
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # emObject 
 
@@ -98,7 +100,9 @@
 
 # Licence
 emObject is available under the MIT License.
 
 **(c)** 2023 Enable Medicine, Inc. 
 
 <img src="./docs/img/em_logo.png" alt="emobject logo" width="350"/> 
+
+
```

### Comparing `emobject-0.7.0b1/README.md` & `emobject-0.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/core.py` & `emobject-0.7.0b2/emobject/core.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/database.py` & `emobject-0.7.0b2/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/emexperiment.py` & `emobject-0.7.0b2/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/emimage.py` & `emobject-0.7.0b2/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/emlayer.py` & `emobject-0.7.0b2/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/emobject.py` & `emobject-0.7.0b2/emobject/emobject.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/empublicaccess.py` & `emobject-0.7.0b2/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/emroitools.py` & `emobject-0.7.0b2/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/utils/graph.py` & `emobject-0.7.0b2/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/utils/helpers.py` & `emobject-0.7.0b2/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject/utils/io.py` & `emobject-0.7.0b2/emobject/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,25 @@
         E : EMObject to convert
     '''
     try:
         import anndata as ad
     except ImportError:
         raise EMObjectException('anndata not installed')
 
-    adata = ad.AnnData(X=E.data,
-                       obs=E.obs,
-                       var=E.var,
-                       uns=E.meta
-                       )
+    adata = ad.AnnData(X=E.data)
+    # make obs axis string
+    temp_obs = E.obs.copy()
+    temp_obs.index = temp_obs.index.astype(str)
+    adata.obs = temp_obs
+    adata.var = E.var
+
+    if E.meta is not None:
+        # convert df to dict
+        adata.uns = E.meta.to_dict()
+
     return adata
 
 
 def from_anndata(adata: AnnData,
                  dtype=int,
                  include_uns: Optional[bool] = False,
                  name: Optional[str] = None,
```

### Comparing `emobject-0.7.0b1/emobject/utils/visualization.py` & `emobject-0.7.0b2/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/emobject.egg-info/PKG-INFO` & `emobject-0.7.0b2/emobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b1
+Version: 0.7.0b2
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # emObject 
 
@@ -98,7 +100,9 @@
 
 # Licence
 emObject is available under the MIT License.
 
 **(c)** 2023 Enable Medicine, Inc. 
 
 <img src="./docs/img/em_logo.png" alt="emobject logo" width="350"/> 
+
+
```

### Comparing `emobject-0.7.0b1/emobject.egg-info/SOURCES.txt` & `emobject-0.7.0b2/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b1/setup.py` & `emobject-0.7.0b2/setup.py`

 * *Files identical despite different names*

