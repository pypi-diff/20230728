# Comparing `tmp/ign-pdal-tools-1.1.0.tar.gz` & `tmp/ign-pdal-tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-pdal-tools-1.1.0.tar", last modified: Tue Jul 18 06:54:23 2023, max compression
+gzip compressed data, was "ign-pdal-tools-1.1.1.tar", last modified: Fri Jul 28 08:14:13 2023, max compression
```

## Comparing `ign-pdal-tools-1.1.0.tar` & `ign-pdal-tools-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.088310 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.088310 ign-pdal-tools-1.1.0/pdaltools/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_add_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/replace_attribute_in_las.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/standardize_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/unlock_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_add_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_replace_attribute_in_las.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_standardize_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_unlock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:14:13.342139 ign-pdal-tools-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-28 08:14:13.342139 ign-pdal-tools-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:14:13.334139 ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-28 08:14:13.000000 ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-28 08:14:13.000000 ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:14:13.000000 ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 08:14:13.000000 ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:14:13.338139 ign-pdal-tools-1.1.1/pdaltools/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/las_add_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/las_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/las_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/las_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/replace_attribute_in_las.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/standardize_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pdaltools/unlock_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:14:13.342139 ign-pdal-tools-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:14:13.342139 ign-pdal-tools-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_las_add_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_las_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_las_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_las_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_replace_attribute_in_las.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_standardize_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-28 08:13:35.000000 ign-pdal-tools-1.1.1/test/test_unlock.py
```

### Comparing `ign-pdal-tools-1.1.0/LICENSE.md` & `ign-pdal-tools-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/PKG-INFO` & `ign-pdal-tools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ign-pdal-tools
```

### Comparing `ign-pdal-tools-1.1.0/README.md` & `ign-pdal-tools-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/PKG-INFO` & `ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ign-pdal-tools
```

### Comparing `ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/SOURCES.txt` & `ign-pdal-tools-1.1.1/ign_pdal_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/color.py` & `ign-pdal-tools-1.1.1/pdaltools/color.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/las_add_buffer.py` & `ign-pdal-tools-1.1.1/pdaltools/las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/las_clip.py` & `ign-pdal-tools-1.1.1/pdaltools/las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/las_info.py` & `ign-pdal-tools-1.1.1/pdaltools/las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/las_merge.py` & `ign-pdal-tools-1.1.1/pdaltools/las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/replace_attribute_in_las.py` & `ign-pdal-tools-1.1.1/pdaltools/replace_attribute_in_las.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/standardize_format.py` & `ign-pdal-tools-1.1.1/pdaltools/standardize_format.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/pdaltools/unlock_file.py` & `ign-pdal-tools-1.1.1/pdaltools/unlock_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,11 +53,13 @@
     parser = argparse.ArgumentParser("Unlock las/laz files generated by TerraSolid (it overwrites the input)")
     parser.add_argument(
         "--input", "-i",
         type=str,
         required=True,
         help="Input file")
 
+    return parser.parse_args()
+
 
 if __name__ == "__main__":
     args = parse_args()
     unlock_file(args.input)
```

### Comparing `ign-pdal-tools-1.1.0/test/test_color.py` & `ign-pdal-tools-1.1.1/test/test_color.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,38 +20,42 @@
 
 TEST_PATH = os.path.dirname(os.path.abspath(__file__))
 INPUT_PATH = os.path.join(TEST_PATH, 'data/test_noepsg_043500_629205_IGN69.laz')
 
 OUTPUT_FILE = TMPDIR + "Semis_2021_0435_6292_LA93_IGN69.las"
 
 
+@pytest.mark.geoportail
 def test_epsg_fail():
     with pytest.raises(requests.exceptions.HTTPError, match="400 Client Error: BadRequest for url") :
         color.color(INPUT_PATH, OUTPUT_FILE, "", 0.1, 15)
 
 
 epsg = "2154"
 layer= "ORTHOIMAGERY.ORTHOPHOTOS"
 minx=435000
 miny=6291000
 maxx=436000
 maxy=6292000
 pixel_per_meter=0.1
 
 
+@pytest.mark.geoportail
 def test_download_image_ok():
     color.download_image_from_geoportail(epsg, layer, minx, miny, maxx, maxy, pixel_per_meter, OUTPUT_FILE, 15)
 
 
+@pytest.mark.geoportail
 def test_download_image_raise1():
     retry_download = color.retry(2, 5)(color.download_image_from_geoportail)
     with pytest.raises(requests.exceptions.HTTPError):
         retry_download(epsg, "MAUVAISE_COUCHE", minx, miny, maxx, maxy, pixel_per_meter, OUTPUT_FILE, 15)
 
 
+@pytest.mark.geoportail
 def test_download_image_raise2():
     retry_download = color.retry(2, 5)(color.download_image_from_geoportail)
     with pytest.raises(requests.exceptions.HTTPError):
         retry_download("9001", layer, minx, miny, maxx, maxy, pixel_per_meter, OUTPUT_FILE, 15)
 
 
 def test_retry_on_server_error():
@@ -80,9 +84,7 @@
     # Here you can change retry params
     @color.retry(7, 15, 2, True)
     def raise_server_error():
         raise requests.exceptions.HTTPError("Server Error")
 
     with pytest.raises(requests.exceptions.HTTPError):
         raise_server_error()
-
-
```

### Comparing `ign-pdal-tools-1.1.0/test/test_las_add_buffer.py` & `ign-pdal-tools-1.1.1/test/test_las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/test/test_las_clip.py` & `ign-pdal-tools-1.1.1/test/test_las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/test/test_las_info.py` & `ign-pdal-tools-1.1.1/test/test_las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/test/test_las_merge.py` & `ign-pdal-tools-1.1.1/test/test_las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/test/test_replace_attribute_in_las.py` & `ign-pdal-tools-1.1.1/test/test_replace_attribute_in_las.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.1.0/test/test_standardize_format.py` & `ign-pdal-tools-1.1.1/test/test_standardize_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         exec_las2las("not_existing_input_file", "output_file")
 
 
 def test_standardize_does_NOT_produce_any_warning_with_Lasinfo():
     # bad file on the store (44 Mo)
     # input_file = "/var/data/store-lidarhd/developpement/standaLAS/demo_standardization/Semis_2022_0584_6880_LA93_IGN69.laz"
 
-    input_file = "./test/data/classified_laz/test_data_77050_627755_LA93_IGN69.laz"
-    output_file = "./tmp/test_standardize_produce_no_warning_with_lasinfo.las"
+    input_file = os.path.join(test_path, "data/classified_laz/test_data_77050_627755_LA93_IGN69.laz")
+    output_file = os.path.join(tmp_path, "test_standardize_produce_no_warning_with_lasinfo.las")
 
     # if you want to see input_file warnings
     # assert_lasinfo_no_warning(input_file)
 
     standardize(input_file, output_file, multiple_params[0])
     assert_lasinfo_no_warning(output_file)
```

### Comparing `ign-pdal-tools-1.1.0/test/test_unlock.py` & `ign-pdal-tools-1.1.1/test/test_unlock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import laspy
 import os
 import shutil
-import pdal
+import pytest
 
 from pdaltools.color import color, pdal_info_json
-from pdaltools.unlock_file import unlock_file
+from pdaltools.unlock_file import unlock_file, copy_and_hack_decorator
 
 
 TEST_PATH = os.path.dirname(os.path.abspath(__file__))
 TMPDIR = os.path.join(TEST_PATH, "tmp")
 LAZ_FILE = os.path.join(TEST_PATH, 'data/test_pdalfail_0643_6319_LA93_IGN69.laz')
 
 
@@ -16,15 +16,27 @@
     try:
         shutil.rmtree(TMPDIR)
     except (FileNotFoundError):
         pass
     os.mkdir(TMPDIR)
 
 
-def test_copy_and_hack_decorator():
+@copy_and_hack_decorator
+def decorated_pdal_info_json(input_file: str):
+    return pdal_info_json(input_file)
+
+
+def test_copy_and_hack_decorator_simple():
+    TMP_FILE = os.path.join(TMPDIR, "copy_and_hack_simple.laz")
+    shutil.copy(LAZ_FILE, TMP_FILE)
+    decorated_pdal_info_json(TMP_FILE)
+
+
+@pytest.mark.geoportail
+def test_copy_and_hack_decorator_color():
     # bug during laz opening in pdal (solved with copy_and_hack_decorator)
     LAS_FILE = os.path.join(TMPDIR, "test_pdalfail_0643_6319_LA93_IGN69.las")
 
     color(LAZ_FILE, LAS_FILE, "", 1)
 
     las = laspy.read(LAS_FILE)
     print(las.header)
```

