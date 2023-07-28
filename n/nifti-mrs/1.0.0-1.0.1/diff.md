# Comparing `tmp/nifti_mrs-1.0.0.tar.gz` & `tmp/nifti_mrs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti_mrs-1.0.0.tar", last modified: Fri Jul  7 11:01:25 2023, max compression
+gzip compressed data, was "nifti_mrs-1.0.1.tar", last modified: Fri Jul 28 07:45:50 2023, max compression
```

## Comparing `nifti_mrs-1.0.0.tar` & `nifti_mrs-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.973532 nifti_mrs-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/mrs_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/mrs_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/mrs_tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/src/nifti_mrs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 11:01:25.981532 nifti_mrs-1.0.0/src/nifti_mrs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/nifti_mrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/nifti_mrs/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/tools/split_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/src/nifti_mrs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 11:01:25.000000 nifti_mrs-1.0.0/src/nifti_mrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:01:25.977532 nifti_mrs-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_split_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_script_mrs_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-07 11:01:17.000000 nifti_mrs-1.0.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.942534 nifti_mrs-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-28 07:45:50.942534 nifti_mrs-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-28 07:45:50.942534 nifti_mrs-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.934534 nifti_mrs-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.938534 nifti_mrs-1.0.1/src/mrs_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/mrs_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/mrs_tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.938534 nifti_mrs-1.0.1/src/nifti_mrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 07:45:50.942534 nifti_mrs-1.0.1/src/nifti_mrs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23767 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/nifti_mrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.938534 nifti_mrs-1.0.1/src/nifti_mrs/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/tools/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/tools/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/tools/split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/src/nifti_mrs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.938534 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 07:45:50.000000 nifti_mrs-1.0.1/src/nifti_mrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:45:50.942534 nifti_mrs-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_script_mrs_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-28 07:45:42.000000 nifti_mrs-1.0.1/tests/test_validator.py
```

### Comparing `nifti_mrs-1.0.0/LICENSE` & `nifti_mrs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/PKG-INFO` & `nifti_mrs-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nifti_mrs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: VIS
 License-File: LICENSE
 
 # Python Tools for NIfTI-MRS
 
 ![PyPI](https://img.shields.io/pypi/v/nifti-mrs)
```

### Comparing `nifti_mrs-1.0.0/README.md` & `nifti_mrs-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/setup.cfg` & `nifti_mrs-1.0.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = MRS
 license = BSD 3-Clause License
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 author = William Clarke
 author_email = william.clarke@ndcn.ox.ac.uk
 
 [options]
 install_requires = 
 	numpy
 	nibabel
 	fslpy
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 VIS = 
 	fsl-mrs
 
 [options.entry_points]
 console_scripts =
```

### Comparing `nifti_mrs-1.0.0/src/mrs_tools/__init__.py` & `nifti_mrs-1.0.1/src/mrs_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/create_nmrs.py` & `nifti_mrs-1.0.1/src/nifti_mrs/create_nmrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 
     # Touch up header with required NIfTI-MRS metadata
     header['pixdim'][4] = dwelltime
     v_major = nifti_mrs_version[0]
     v_minor = nifti_mrs_version[1]
     header['intent_name'] = f'mrs_v{v_major}_{v_minor}'.encode()
 
+    # Ensure that xyzt_units is set correctly
+    # define NIFTI_UNITS_MM      2 /! NIFTI code for millimeters. /
+    # define NIFTI_UNITS_SEC     8 /! NIFTI code for seconds. /
+    header.set_xyzt_units(xyz=2, t=8)
+
     # Add header extension to header
     json_s = hdr_ext.to_json()
     extension = nib.nifti1.Nifti1Extension(44, json_s.encode('UTF-8'))
     header.extensions.append(extension)
 
     if no_conj:
         return NIFTI_MRS(data.conj(), header=header)
```

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/definitions.py` & `nifti_mrs-1.0.1/src/nifti_mrs/definitions.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/hdr_ext.py` & `nifti_mrs-1.0.1/src/nifti_mrs/hdr_ext.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/nifti_mrs.py` & `nifti_mrs-1.0.1/src/nifti_mrs/nifti_mrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class NIFTI_MRS():
     """A class to load and represent NIfTI-MRS formatted data.
     Utilises the fslpy Image class and nibabel nifti headers.
 
     Access the underlying fslpy Image object for useful attributes using obj.image.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, validate_on_creation=True, **kwargs):
         """Create a NIFTI_MRS object with the given image data or file name.
 
         Arguments mirror those of the leveraged fsl.data.image.IMage class.
 
         :arg image:      A string containing the name of an image file to load,
                          or a Path object pointing to an image file, or a
                          :mod:`numpy` array, or a :mod:`nibabel` image object,
@@ -71,14 +71,18 @@
                          :func:`loadMeta` function. Defaults to ``False``.
 
         :arg dataMgr:    Object implementing the :class:`DataManager`
                          interface, for managing access to the image data.
 
         All other arguments are passed through to the ``nibabel.load`` function
         (if it is called).
+
+        :arg validate_on_creation:   If True (default) then the header extension will
+                                     be validated on creation of the NIfTI-MRS object.
+                                     Use False to just print warnings.
         """
         # Handle various options for the first (data source) argument
         input_hdr_ext = None
         if isinstance(args[0], np.ndarray):
             # If generated from np.array include conjugation
             # to make sure generation from data of existing NIfTI-MRS
             # object results in consistent phase/freq convention.
@@ -119,18 +123,27 @@
                 raise NotNIFTI_MRS('NIFTI-MRS must have a header extension.')
 
             self._hdr_ext = Hdr_Ext.from_header_ext(
                 json.loads(
                     self.header.extensions[hdr_ext_codes.index(44)].get_content()))
 
         # Some validation upon creation
-        validator.validate_hdr_ext(
-            self._hdr_ext.to_json(),
-            self.image.shape,
-            np.max((self._hdr_ext.ndim, self.image.ndim)))
+        if validate_on_creation:
+            validator.validate_hdr_ext(
+                self._hdr_ext.to_json(),
+                self.image.shape,
+                np.max((self._hdr_ext.ndim, self.image.ndim)))
+        else:
+            try:
+                validator.validate_hdr_ext(
+                    self._hdr_ext.to_json(),
+                    self.image.shape,
+                    np.max((self._hdr_ext.ndim, self.image.ndim)))
+            except validator.headerExtensionError as exc:
+                print(f"This file's header extension is currently invalid. Reason: {str(exc)}")
 
         try:
             self.nucleus
             self.spectrometer_frequency
         except KeyError:
             raise NotNIFTI_MRS('NIFTI-MRS header extension must have nucleus and spectrometerFrequency keys.')
```

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/tools/reorder.py` & `nifti_mrs-1.0.1/src/nifti_mrs/tools/reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/tools/reshape.py` & `nifti_mrs-1.0.1/src/nifti_mrs/tools/reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/tools/split_merge.py` & `nifti_mrs-1.0.1/src/nifti_mrs/tools/split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/utils.py` & `nifti_mrs-1.0.1/src/nifti_mrs/utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs/validator.py` & `nifti_mrs-1.0.1/src/nifti_mrs/validator.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs.egg-info/PKG-INFO` & `nifti_mrs-1.0.1/src/nifti_mrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nifti-mrs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: VIS
 License-File: LICENSE
 
 # Python Tools for NIfTI-MRS
 
 ![PyPI](https://img.shields.io/pypi/v/nifti-mrs)
```

### Comparing `nifti_mrs-1.0.0/src/nifti_mrs.egg-info/SOURCES.txt` & `nifti_mrs-1.0.1/src/nifti_mrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_create_nmrs.py` & `nifti_mrs-1.0.1/tests/test_create_nmrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     assert nmrs.dwelltime == 1 / 2000.0
     assert nmrs.nucleus == ['1H']
     assert nmrs.spectrometer_frequency == [128.0]
     assert nmrs.bandwidth == 2000.0
     assert nmrs.dim_tags == ['DIM_COIL', None, None]
     assert 'dim_5' in nmrs.hdr_ext
 
+    assert nmrs.header.get_xyzt_units() == ('mm', 'sec')
+
     nmrs.save(tmp_path / 'out')
     assert (tmp_path / 'out.nii.gz').exists()
 
 
 def test_gen_new_nifti_mrs_hdr_ext(tmp_path):
     data = np.zeros((1, 1, 1, 1024, 4), dtype=np.complex64)
     affine = np.eye(4)
```

### Comparing `nifti_mrs-1.0.0/tests/test_hdr_ext.py` & `nifti_mrs-1.0.1/tests/test_hdr_ext.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_nifti_mrs.py` & `nifti_mrs-1.0.1/tests/test_nifti_mrs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 '''Test the NIFTI-MRS class implementation
 
 Copyright Will Clarke, University of Oxford, 2023'''
 
 # Imports
 from pathlib import Path
 from copy import deepcopy
+import json
 
 import pytest
 import numpy as np
+from nibabel.nifti1 import Nifti1Extension
 
 from nifti_mrs.nifti_mrs import NIFTI_MRS
 from nifti_mrs.validator import headerExtensionError
 from nifti_mrs.create_nmrs import gen_nifti_mrs, gen_nifti_mrs_hdr_ext
 
 # Files
 testsPath = Path(__file__).parent
@@ -57,15 +59,15 @@
     obj.set_version_info(1, 3)
     assert obj.nifti_mrs_version == '1.3'
 
 
 def test_hdr_ext():
     obj = NIFTI_MRS(data['unprocessed'])
 
-    # Test dictionay like access of keys
+    # Test dictionary like access of keys
     assert 'EchoTime' in obj.hdr_ext
     assert obj.hdr_ext['EchoTime'] == 0.011
 
     # Test direct manipulation of hdr_ext
     obj.hdr_ext.set_user_def('bogus', 'test', 'Description')
     assert 'bogus' in obj.hdr_ext
 
@@ -343,7 +345,31 @@
 
 
 def test_getaffine():
     obj = NIFTI_MRS(data['unprocessed'])
     assert np.allclose(
         obj.getAffine('voxel', 'world'),
         obj.image.getAffine('voxel', 'world'))
+
+
+def test_on_load_validator(capsys):
+    obj = NIFTI_MRS(data['unprocessed'])
+    hdr_ext = obj.hdr_ext.to_dict()
+    hdr_ext.pop('dim_5')
+    header = obj.header
+
+    bad_extension = Nifti1Extension(
+        44,
+        json.dumps(hdr_ext).encode('UTF-8'))
+    header.extensions.clear()
+    header.extensions.append(bad_extension)
+
+    with pytest.raises(
+            headerExtensionError,
+            match="With 6 dimensions the header extension must contain 'dim_5'."):
+        NIFTI_MRS(obj[:], header=header)
+
+    NIFTI_MRS(obj[:], header=header, validate_on_creation=False)
+    captured = capsys.readouterr()
+    assert captured.out == \
+        "This file's header extension is currently invalid. "\
+        "Reason:  With 6 dimensions the header extension must contain 'dim_5'.\n"
```

### Comparing `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reorder.py` & `nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_reshape.py` & `nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_split_merge.py` & `nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_nifti_mrs_tools_utils.py` & `nifti_mrs-1.0.1/tests/test_nifti_mrs_tools_utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_script_mrs_tools.py` & `nifti_mrs-1.0.1/tests/test_script_mrs_tools.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.0.0/tests/test_validator.py` & `nifti_mrs-1.0.1/tests/test_validator.py`

 * *Files identical despite different names*

