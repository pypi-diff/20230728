# Comparing `tmp/nlmpy-1.1.1.tar.gz` & `tmp/nlmpy-1.1.2.tar.gz`

## Comparing `nlmpy-1.1.1.tar` & `nlmpy-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 nlmpy-1.1.1/CITATION.cff
--rwxr-xr-x   0        0        0   198331 2020-02-02 00:00:00.000000 nlmpy-1.1.1/images/logo.png
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 nlmpy-1.1.1/src/nlmpy/__init__.py
--rwxr-xr-x   0        0        0    44559 2020-02-02 00:00:00.000000 nlmpy-1.1.1/src/nlmpy/nlmpy.py
--rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 nlmpy-1.1.1/LICENSE.txt
--rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 nlmpy-1.1.1/README.md
--rwxr-xr-x   0        0        0      636 2020-02-02 00:00:00.000000 nlmpy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 nlmpy-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 nlmpy-1.1.2/CITATION.cff
+-rwxr-xr-x   0        0        0   198331 2020-02-02 00:00:00.000000 nlmpy-1.1.2/images/logo.png
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 nlmpy-1.1.2/src/nlmpy/__init__.py
+-rwxr-xr-x   0        0        0    44556 2020-02-02 00:00:00.000000 nlmpy-1.1.2/src/nlmpy/nlmpy.py
+-rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 nlmpy-1.1.2/LICENSE.txt
+-rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 nlmpy-1.1.2/README.md
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 nlmpy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 nlmpy-1.1.2/PKG-INFO
```

### Comparing `nlmpy-1.1.1/CITATION.cff` & `nlmpy-1.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nlmpy-1.1.1/images/logo.png` & `nlmpy-1.1.2/images/logo.png`

 * *Files identical despite different names*

### Comparing `nlmpy-1.1.1/src/nlmpy/nlmpy.py` & `nlmpy-1.1.2/src/nlmpy/nlmpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
     Returns
     -------
     out : array
         2D array.
     """
     # Determine the dimension of the smallest square
     maxDim = np.max(np.array([nRow, nCol]))
-    N = np.int(np.ceil(np.log2(maxDim - 1)))
+    N = int(np.ceil(np.log2(maxDim - 1)))
     dim = 2 ** N + 1
     # Create surface and extract required array size if needed
     surface = diamondsquare(dim, h)
     if (nRow, nCol) != surface.shape:
         surface = extractRandomArrayFromSquareArray(surface, nRow, nCol)
     # Apply mask and rescale 0-1
     if mask is not None:
```

### Comparing `nlmpy-1.1.1/LICENSE.txt` & `nlmpy-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nlmpy-1.1.1/README.md` & `nlmpy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nlmpy-1.1.1/pyproject.toml` & `nlmpy-1.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nlmpy"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Thomas R. Etherington", email="etheringtont@landcareresearch.co.nz" },
   { name="E. Penelope Holland" },
   { name="David O'Sullivan" },
   { name="Pierre Vigier" }
 ]
 description = "A Python package to create neutral landscape models"
@@ -17,8 +17,8 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
+"Homepage" = "https://github.com/tretherington/nlmpy"
```

### Comparing `nlmpy-1.1.1/PKG-INFO` & `nlmpy-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nlmpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package to create neutral landscape models
-Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Homepage, https://github.com/tretherington/nlmpy
 Author: E. Penelope Holland, David O'Sullivan, Pierre Vigier
 Author-email: "Thomas R. Etherington" <etheringtont@landcareresearch.co.nz>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
```

