# Comparing `tmp/emobject-0.7.0b3.tar.gz` & `tmp/emobject-0.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.0b3.tar", last modified: Fri Jul 28 18:35:36 2023, max compression
+gzip compressed data, was "emobject-0.7.0b4.tar", last modified: Fri Jul 28 20:23:08 2023, max compression
```

## Comparing `emobject-0.7.0b3.tar` & `emobject-0.7.0b4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.153705 emobject-0.7.0b3/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 18:35:26.000000 emobject-0.7.0b3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:35:36.153705 emobject-0.7.0b3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 18:35:26.000000 emobject-0.7.0b3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.151705 emobject-0.7.0b3/emobject/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39223 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/database.py
--rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emexperiment.py
--rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emimage.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emlayer.py
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emobject.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/empublicaccess.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/emroitools.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.153705 emobject-0.7.0b3/emobject/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/utils/visualization.py
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 18:35:26.000000 emobject-0.7.0b3/emobject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 18:35:36.152705 emobject-0.7.0b3/emobject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 18:35:36.000000 emobject-0.7.0b3/emobject.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 18:35:36.153705 emobject-0.7.0b3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 18:35:26.000000 emobject-0.7.0b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.863490 emobject-0.7.0b4/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-28 20:22:58.000000 emobject-0.7.0b4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 20:23:08.863490 emobject-0.7.0b4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-28 20:22:58.000000 emobject-0.7.0b4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.861490 emobject-0.7.0b4/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39419 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.862490 emobject-0.7.0b4/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-28 20:22:58.000000 emobject-0.7.0b4/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 20:23:08.861490 emobject-0.7.0b4/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 20:23:08.000000 emobject-0.7.0b4/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-28 20:23:08.863490 emobject-0.7.0b4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 20:22:58.000000 emobject-0.7.0b4/setup.py
```

### Comparing `emobject-0.7.0b3/LICENSE` & `emobject-0.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/PKG-INFO` & `emobject-0.7.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b3
+Version: 0.7.0b4
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.0b3/README.md` & `emobject-0.7.0b4/README.md`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/core.py` & `emobject-0.7.0b4/emobject/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                                     object_codec=JSON())
             _ = mask.create_dataset(name='maskpos', data=np.array(list(E.mask.pos.values())))
             for name in E.mask.mask.keys():
                 _ = mask.create_dataset(name=name, data=E.mask.mask[name], compressor=compressor)
 
     if E._meta is not None:
         _ = core.create_dataset(name='meta',
-                                data=E.meta,
+                                data=E.meta.to_numpy(),
                                 compressor=compressor,
                                 dtype=object,
                                 object_codec=JSON())
 
     # Build core data group
     # add layers as hierarchy:
     for layer in E.layers:
@@ -579,14 +579,19 @@
     # Now it's time to build the EMObject
 
     # Load the meta attributes
     meta = None
     meta_path = os.path.join(path, 'core', 'meta')
     if os.path.exists(meta_path):
         meta = zarr.convenience.load(meta_path)
+        if meta.shape[1] == 2:
+            col_names = ['FEATURE_NAME', 'FEATURE_VALUE']
+        else:
+            col_names = None
+        meta = pd.DataFrame(meta, columns=col_names)
 
     object_name = os.path.basename(path).split('.')[0]
 
     E = EMObject(data=None,
                  obs=None,
                  var=None,
                  sobs=None,
```

### Comparing `emobject-0.7.0b3/emobject/database.py` & `emobject-0.7.0b4/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/emexperiment.py` & `emobject-0.7.0b4/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/emimage.py` & `emobject-0.7.0b4/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/emlayer.py` & `emobject-0.7.0b4/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/emobject.py` & `emobject-0.7.0b4/emobject/emobject.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/empublicaccess.py` & `emobject-0.7.0b4/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/emroitools.py` & `emobject-0.7.0b4/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/utils/graph.py` & `emobject-0.7.0b4/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/utils/helpers.py` & `emobject-0.7.0b4/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/utils/io.py` & `emobject-0.7.0b4/emobject/utils/io.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject/utils/visualization.py` & `emobject-0.7.0b4/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/emobject.egg-info/PKG-INFO` & `emobject-0.7.0b4/emobject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.0b3
+Version: 0.7.0b4
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.0b3/emobject.egg-info/SOURCES.txt` & `emobject-0.7.0b4/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.0b3/setup.py` & `emobject-0.7.0b4/setup.py`

 * *Files identical despite different names*

