# Comparing `tmp/DeepSlice-1.1.2.tar.gz` & `tmp/DeepSlice-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.2.tar", last modified: Thu Apr 27 09:58:21 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.3.tar", last modified: Fri Jul 28 11:35:57 2023, max compression
```

## Comparing `DeepSlice-1.1.2.tar` & `DeepSlice-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:58:21.000000 DeepSlice-1.1.2/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 09:58:21.753446 DeepSlice-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-27 09:58:09.000000 DeepSlice-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:35:57.268342 DeepSlice-1.1.3/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 11:35:57.000000 DeepSlice-1.1.3/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 11:35:57.272343 DeepSlice-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-28 11:35:47.000000 DeepSlice-1.1.3/setup.py
```

### Comparing `DeepSlice-1.1.2/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.3/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.3/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.3/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.3/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List
+from typing import Union, List, Optional
 import numpy as np
 import pandas as pd
 import re
 from .depth_estimation import calculate_brain_center_depths
 from .plane_alignment_functions import plane_alignment
 
 def trim_mean(arr: np.array, percent: int) -> float:
@@ -19,55 +19,50 @@
     """
     n = len(arr)
     k = int(round(n * (float(percent) / 100) / 2))
     return np.mean(arr[k + 1 : n - k])
 
 
 def calculate_average_section_thickness(
-    section_numbers: List[Union[int, float]], section_depth: List[Union[int, float]], method="weighted",
+    section_numbers: List[Union[int, float]], section_depth: List[Union[int, float]], bad_sections, method="weighted",
     species="mouse"
 ) -> float:
     """
     Calculates the average section thickness for a series of predictions
 
     :param section_numbers: List of section numbers
     :param section_depth: List of section depths
     :type section_numbers: List[int, float]
     :type section_depth: List[int, float]
     :return: the average section thickness
     :rtype: float
     """
     # inter section number differences
+    if bad_sections is not None:
+        section_numbers = section_numbers[bad_sections == False].reset_index(drop=True)
+        section_depth = section_depth[bad_sections == False]
     number_spacing = section_numbers[:-1].values - section_numbers[1:].values
     # inter section depth differences
     depth_spacing = section_depth[:-1] - section_depth[1:]
     # dividing depth spacing by number spacing allows us to control for missing sections
-    min = 0
-    max = np.max(section_numbers)
-    if species == "mouse":
-        min, max = 0, 528
-    elif species == "rat":
-        min, max = 0, 1024
-    if method == "weighted":
-        weighted_accuracy = plane_alignment.make_gaussian_weights(max + 1)
-        weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
-    elif method == None:
-        weighted_accuracy = [1 for y in section_numbers]
-
+    weighted_accuracy = calculate_weighted_accuracy(section_numbers, section_depth, species, None, method)
     section_thicknesses = depth_spacing / number_spacing
-    if len(section_numbers) <= 2:
-      weighted_accuracy = [1, 1]
     average_thickness = np.average(section_thicknesses, weights = weighted_accuracy[1:])
     return average_thickness
 
 
+
+
+
+
 def ideal_spacing(
     section_numbers: List[Union[int, float]],
     section_depth: List[Union[int, float]],
     average_thickness: Union[int, float],
+    bad_sections: List[bool] = None,
     method = "weighted",
     species = "mouse"
 ) -> float:
     """
     Calculates the ideal spacing for a series of predictions
 
     :param section_numbers: List of section numbers
@@ -78,27 +73,16 @@
     :type average_thickness: int, float
     :return: the ideal spacing
     :rtype: float
     """
     # unaligned voxel position of section numbers (evenly spaced depths)
     index_spaced_depth = section_numbers * average_thickness
     # average distance between the depths and the evenly spaced depths
-    min = 0
-    max = np.max(section_numbers)
-    if species == "mouse":
-        min, max = 0, 528
-    elif species == "rat":
-        min, max = 0, 1024
-    if method == "weighted":
-        weighted_accuracy = plane_alignment.make_gaussian_weights(max + 1)
-        weighted_accuracy = [weighted_accuracy[int(y)] for y in section_numbers]
-    elif method == None:
-        weighted_accuracy = [1 for y in section_numbers]
-    if len(section_numbers) <= 2:
-        weighted_accuracy = [0.5, 0.5]
+    
+    weighted_accuracy = calculate_weighted_accuracy(section_numbers, section_depth, species, bad_sections, method)
     distance_to_ideal = np.average(section_depth - index_spaced_depth, weights = weighted_accuracy)
     # adjust the evenly spaced depths to minimise their distance to the predicted depths
     ideal_index_spaced_depth = index_spaced_depth + distance_to_ideal
     return ideal_index_spaced_depth
 
 
 def determine_direction_of_indexing(depth: List[Union[int, float]]) -> str:
@@ -136,24 +120,34 @@
         )
     else:
         predictions = predictions.reset_index(drop=True)
         depths = calculate_brain_center_depths(predictions)
         depths = np.array(depths)
         direction = determine_direction_of_indexing(depths)
         predictions["depths"] = depths
-
+        
         temp = predictions.copy()
         if direction == "caudal-rostro":
             ascending = False
         if direction == "rostro-caudal":
             ascending = True
-        temp = temp.sort_values(by=["depths"], ascending=ascending).reset_index(
-            drop=True
-        )
-        predictions["oy"] = temp["oy"]
+        if "bad_section" in temp:
+            temp_good = temp[temp["bad_section"] == False].copy().reset_index(drop=True)
+            temp_good_copy = temp_good.copy()
+            temp_good_copy = temp_good_copy.sort_values(by=["depths"], ascending=ascending).reset_index(
+                drop=True
+            )
+            temp_good["oy"] = temp_good_copy["oy"]
+            
+            predictions.loc[predictions["bad_section"] == False, "oy"] = temp_good["oy"].values
+        else:
+            temp = temp.sort_values(by=["depths"], ascending=ascending).reset_index(drop=True)
+
+        
+            predictions["oy"] = temp["oy"].values
     return predictions
 
 
 def space_according_to_index(predictions, section_thickness = None, voxel_size = None, suppress = False, species = "mouse"):
     """
     Space evenly according to the section indexes, if these indexes do not represent the precise order in which the sections were
     cut, this will lead to less accurate predictions. Section indexes must account for missing sections (ie, if section 3 is missing
@@ -162,38 +156,42 @@
     :param predictions: dataframe of predictions
     :type predictions: pandas.DataFrame
     :return: the input dataframe with evenly spaced sections
     :rtype: pandas.DataFrame
     """
     if voxel_size == None:
         raise ValueError("voxel_size must be specified")
-    if section_thickness != None:
+    if section_thickness is not None:
         section_thickness/=voxel_size
     predictions["oy"] = predictions["oy"].astype(float)
     if len(predictions) == 1:
         raise ValueError("Only one section found, cannot space according to index")
     if "nr" not in predictions:
         raise ValueError(
             "No section indexes found, cannot space according to a missing index. You likely did not run predict() with section_numbers=True"
         )
     else:
+        if 'bad_section' in predictions:
+            bad_sections = predictions['bad_section'].values
+        else:
+            bad_sections = None
         predictions = enforce_section_ordering(predictions)
         depths = calculate_brain_center_depths(predictions)
         depths = np.array(depths)
         if not section_thickness:
             section_thickness = calculate_average_section_thickness(
-                predictions["nr"], section_depth = depths, species=species
+                predictions["nr"], section_depth = depths, bad_sections=bad_sections, species=species
             )
             if not suppress:
                 print(f'predicted thickness is {section_thickness * voxel_size}µm')
         else:
             if not suppress:
                 print(f'specified thickness is {section_thickness * voxel_size}µm')
 
-        calculated_spacing = ideal_spacing(predictions["nr"], depths, section_thickness, None, species)
+        calculated_spacing = ideal_spacing(predictions["nr"], depths, section_thickness, bad_sections, species=species)
         distance_to_ideal = calculated_spacing - depths
         predictions["oy"] = predictions["oy"] + distance_to_ideal
     return predictions
 
 
 def number_sections(filenames: List[str], legacy=False) -> List[int]:
     """
@@ -221,30 +219,85 @@
             ###this gets the three numbers closest to the end
             section_numbers.append(match[-3:])
     if len(section_numbers) == 0:
         raise ValueError("No section numbers found in filenames")
     return section_numbers
 
 
-def set_bad_sections_util(df: pd.DataFrame, bad_sections: List[str]) -> pd.DataFrame:
+def set_bad_sections_util(df: pd.DataFrame, bad_sections: List[str], auto = False) -> pd.DataFrame:
     """
     Sets the damaged sections and sections which deepslice may not perform well on for a series of predictions
     
     :param bad_sections: List of bad sections
     :param df: dataframe of predictions
+    :param auto: automatically set bad sections based on if theyre badly positioned relative to their section index
     :type bad_sections: List[int]
     :type df: pandas.DataFrame
+    :type auto: bool
     :return: the input dataframe with bad sections labeled as such
     :rtype: pandas.DataFrame
     """
+
     bad_section_indexes = [
-        df.Filenames.contains(bad_section) for bad_section in bad_sections
+        df.Filenames.str.contains(bad_section) for bad_section in bad_sections
     ]
+    if np.any([np.sum(x)>1 for x in bad_section_indexes]):
+        raise ValueError("Multiple sections match the same bad section string, make sure each bad section string is unique")
+    bad_section_indexes = [np.where(x)[0] for x in bad_section_indexes]
+    bad_section_indexes = np.concatenate(bad_section_indexes)
+    df.loc[~df.index.isin(bad_section_indexes), "bad_section"] = False
+    if auto:
+        df['depths'] = calculate_brain_center_depths(df)
+        x = df['nr'].values
+        y = df['depths'].values
+        m,b = np.polyfit(x,y,1)
+        residuals = y - (m*x + b)
+        outliers = np.abs(residuals) > 1.5*np.std(residuals)
+        df.loc[outliers, 'bad_section'] = True
+        
     df.loc[bad_section_indexes, "bad_section"] = True
+    # make the other sections are False
+    
     bad_sections_found = np.sum(bad_section_indexes)
     # Tell the user which sections were identified as bad
     if bad_sections_found > 0:
         print(
             f"{bad_sections_found} sections out of {len(bad_sections)} were marked as bad, \n\
         They are:\n {df.Filenames[bad_section_indexes]}"
         )
     return df
+
+
+def calculate_weighted_accuracy(section_numbers: List[int], depths: List[float], species: str, bad_sections: List[Optional[bool]]  = None, method: str = "weighted") -> List[float]:
+    """
+    Calculates the weighted accuracy of a list of section numbers for a given species
+    
+    :param section_numbers: List of section numbers
+    :param species: Species to calculate accuracy for
+    :param bad_sections: List of bad sections
+    :param method: Method to use for weighting, defaults to "weighted"
+    :type section_numbers: List[int]
+    :type species: str
+    :type bad_sections: List[Optional[bool]]
+    :type method: str
+    :return: List of weighted accuracies
+    :rtype: List[float]
+    """
+    if species == "mouse":
+        min, max = 0, 528
+    elif species == "rat":
+        min, max = 0, 1024
+    if method == "weighted":
+        weighted_accuracy = plane_alignment.make_gaussian_weights(max + 1)
+        depths = np.array(depths)
+        depths[depths < min] = min
+        depths[depths > max] = max
+        weighted_accuracy = [weighted_accuracy[int(y)] for y in depths]
+    elif method is None:
+        weighted_accuracy = [1 for y in section_numbers]
+    if len(section_numbers) <= 2:
+        weighted_accuracy = [0.5, 0.5]
+        
+    if bad_sections is not None:
+        weighted_accuracy = [x if y == False else 0 for x,y in zip(weighted_accuracy,bad_sections)]
+        
+    return weighted_accuracy
```

### Comparing `DeepSlice-1.1.2/DeepSlice/main.py` & `DeepSlice-1.1.3/DeepSlice/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 
 
         #: pd.DataFrame: Filenames and predicted QuickNII coordinates of the input sections.
 
         self.predictions = predictions
         self.image_directory = image_directory
 
-    def set_bad_sections(self, bad_sections: list):
+    def set_bad_sections(self, bad_sections: list, auto = False):
         """
         sets the bad sections for a given brain. Must be run after predict()
 
         :param bad_sections: A list of bad sections to ignore when calculating angles and spacing
         :type bad_sections: list
         """
         self.predictions = spacing_and_indexing.set_bad_sections_util(
-            self.predictions, bad_sections
+            self.predictions, bad_sections, auto
         )
 
     def enforce_index_order(self):
         """
         reorders the section depths (oy) in the predictions such that they align with the section indexes
         """
         self.predictions = spacing_and_indexing.enforce_section_ordering(
```

### Comparing `DeepSlice-1.1.2/DeepSlice/metadata/config.json` & `DeepSlice-1.1.3/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.3/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.3/DeepSlice/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.3/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.3/DeepSlice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.2 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.3 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.2.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.3.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.2/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.3/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/LICENSE` & `DeepSlice-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/PKG-INFO` & `DeepSlice-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.2 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.3 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.2.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.3.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
 LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
```

### Comparing `DeepSlice-1.1.2/README.md` & `DeepSlice-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.2/setup.py` & `DeepSlice-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.2',
+    version='1.1.3',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.2.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.3.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
```

