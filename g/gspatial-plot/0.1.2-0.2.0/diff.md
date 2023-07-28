# Comparing `tmp/gspatial_plot-0.1.2.tar.gz` & `tmp/gspatial_plot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspatial_plot-0.1.2.tar", last modified: Wed Jul 12 05:04:50 2023, max compression
+gzip compressed data, was "gspatial_plot-0.2.0.tar", last modified: Fri Jul 28 07:50:28 2023, max compression
```

## Comparing `gspatial_plot-0.1.2.tar` & `gspatial_plot-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.189175 gspatial_plot-0.1.2/
--rwxr-xr-x   0 ambee      (501) staff       (20)     1062 2023-01-24 13:48:22.000000 gspatial_plot-0.1.2/LICENSE
--rwxr-xr-x   0 ambee      (501) staff       (20)       43 2023-01-24 20:41:15.000000 gspatial_plot-0.1.2/MANIFEST.in
--rw-r--r--   0 ambee      (501) staff       (20)     2650 2023-07-12 05:04:50.189236 gspatial_plot-0.1.2/PKG-INFO
--rwxr-xr-x   0 ambee      (501) staff       (20)     2130 2023-02-28 08:11:29.000000 gspatial_plot-0.1.2/README.md
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.180552 gspatial_plot-0.1.2/gspatial_plot/
--rwxr-xr-x   0 ambee      (501) staff       (20)       20 2023-02-03 21:03:20.000000 gspatial_plot-0.1.2/gspatial_plot/__init__.py
--rwxr-xr-x   0 ambee      (501) staff       (20)     1183 2023-02-04 09:15:27.000000 gspatial_plot-0.1.2/gspatial_plot/config.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.188781 gspatial_plot-0.1.2/gspatial_plot/datasets/
--rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:46.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.cpg
--rwxr-xr-x   0 ambee      (501) staff       (20)   786828 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf
--rwxr-xr-x   0 ambee      (501) staff       (20)      143 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.prj
--rwxr-xr-x   0 ambee      (501) staff       (20)  1613020 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shp
--rwxr-xr-x   0 ambee      (501) staff       (20)     2036 2022-05-09 04:46:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shx
--rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.cpg
--rwxr-xr-x   0 ambee      (501) staff       (20)    39112 2021-11-14 23:27:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.dbf
--rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-11-14 23:27:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.prj
--rwxr-xr-x   0 ambee      (501) staff       (20)    38836 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shp
--rwxr-xr-x   0 ambee      (501) staff       (20)      148 2021-08-31 07:43:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shx
--rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.cpg
--rwxr-xr-x   0 ambee      (501) staff       (20)  2994462 2021-11-29 04:07:23.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.dbf
--rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-29 06:05:04.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.prj
--rwxr-xr-x   0 ambee      (501) staff       (20)   339832 2021-11-23 07:23:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shp
--rwxr-xr-x   0 ambee      (501) staff       (20)     3396 2021-11-23 07:23:19.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shx
--rwxr-xr-x   0 ambee      (501) staff       (20)        5 2017-08-12 22:28:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.cpg
--rwxr-xr-x   0 ambee      (501) staff       (20)      176 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.dbf
--rwxr-xr-x   0 ambee      (501) staff       (20)      143 2017-08-12 22:28:26.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.prj
--rwxr-xr-x   0 ambee      (501) staff       (20)   978340 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shp
--rwxr-xr-x   0 ambee      (501) staff       (20)      108 2017-10-16 01:22:56.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shx
--rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.cpg
--rwxr-xr-x   0 ambee      (501) staff       (20)  3323764 2021-11-29 04:07:23.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf
--rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-01 17:23:50.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.prj
--rwxr-xr-x   0 ambee      (501) staff       (20)   440568 2021-11-23 08:22:00.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp
--rwxr-xr-x   0 ambee      (501) staff       (20)     3924 2021-11-23 08:22:00.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx
--rwxr-xr-x   0 ambee      (501) staff       (20)   438813 2023-02-04 09:12:29.000000 gspatial_plot-0.1.2/gspatial_plot/datasets/us_states.geojson
--rwxr-xr-x   0 ambee      (501) staff       (20)    47404 2023-07-12 05:01:11.000000 gspatial_plot-0.1.2/gspatial_plot/plot.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.181168 gspatial_plot-0.1.2/gspatial_plot.egg-info/
--rwxr-xr-x   0 ambee      (501) staff       (20)     2650 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/PKG-INFO
--rwxr-xr-x   0 ambee      (501) staff       (20)     1574 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/SOURCES.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)        1 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/dependency_links.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)      183 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/requires.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)       14 2023-07-12 05:04:50.000000 gspatial_plot-0.1.2/gspatial_plot.egg-info/top_level.txt
--rwxr-xr-x   0 ambee      (501) staff       (20)       79 2023-07-12 05:04:50.189423 gspatial_plot-0.1.2/setup.cfg
--rwxr-xr-x   0 ambee      (501) staff       (20)     1279 2023-07-12 05:01:28.000000 gspatial_plot-0.1.2/setup.py
-drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-12 05:04:50.189075 gspatial_plot-0.1.2/tests/
--rwxr-xr-x   0 ambee      (501) staff       (20)      460 2023-01-24 19:47:35.000000 gspatial_plot-0.1.2/tests/test_functions.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:50:28.819881 gspatial_plot-0.2.0/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1062 2023-01-24 13:48:22.000000 gspatial_plot-0.2.0/LICENSE
+-rwxr-xr-x   0 ambee      (501) staff       (20)       43 2023-01-24 20:41:15.000000 gspatial_plot-0.2.0/MANIFEST.in
+-rw-r--r--   0 ambee      (501) staff       (20)     2650 2023-07-28 07:50:28.819943 gspatial_plot-0.2.0/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2130 2023-02-28 08:11:29.000000 gspatial_plot-0.2.0/README.md
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:50:28.790585 gspatial_plot-0.2.0/gspatial_plot/
+-rwxr-xr-x   0 ambee      (501) staff       (20)       20 2023-02-03 21:03:20.000000 gspatial_plot-0.2.0/gspatial_plot/__init__.py
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1183 2023-02-04 09:15:27.000000 gspatial_plot-0.2.0/gspatial_plot/config.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:50:28.818195 gspatial_plot-0.2.0/gspatial_plot/datasets/
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:46.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)   786828 2022-05-09 04:46:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      143 2022-05-09 04:46:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)  1613020 2022-05-09 04:46:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2036 2022-05-09 04:46:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-31 07:43:04.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)    39112 2021-11-14 23:27:26.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-11-14 23:27:26.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)    38836 2021-08-31 07:43:04.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)      148 2021-08-31 07:43:04.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)  2994462 2021-11-29 04:07:23.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-29 06:05:04.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   339832 2021-11-23 07:23:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     3396 2021-11-23 07:23:19.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2017-08-12 22:28:26.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)      176 2017-10-16 01:22:56.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      143 2017-08-12 22:28:26.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   978340 2017-10-16 01:22:56.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)      108 2017-10-16 01:22:56.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)        5 2021-08-01 17:23:50.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.cpg
+-rwxr-xr-x   0 ambee      (501) staff       (20)  3323764 2021-11-29 04:07:23.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf
+-rwxr-xr-x   0 ambee      (501) staff       (20)      145 2021-08-01 17:23:50.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.prj
+-rwxr-xr-x   0 ambee      (501) staff       (20)   440568 2021-11-23 08:22:00.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp
+-rwxr-xr-x   0 ambee      (501) staff       (20)     3924 2021-11-23 08:22:00.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx
+-rwxr-xr-x   0 ambee      (501) staff       (20)   438813 2023-02-04 09:12:29.000000 gspatial_plot-0.2.0/gspatial_plot/datasets/us_states.geojson
+-rwxr-xr-x   0 ambee      (501) staff       (20)    50832 2023-07-28 07:13:28.000000 gspatial_plot-0.2.0/gspatial_plot/plot.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:50:28.791208 gspatial_plot-0.2.0/gspatial_plot.egg-info/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     2650 2023-07-28 07:50:28.000000 gspatial_plot-0.2.0/gspatial_plot.egg-info/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1574 2023-07-28 07:50:28.000000 gspatial_plot-0.2.0/gspatial_plot.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)        1 2023-07-28 07:50:28.000000 gspatial_plot-0.2.0/gspatial_plot.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)      217 2023-07-28 07:50:28.000000 gspatial_plot-0.2.0/gspatial_plot.egg-info/requires.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       14 2023-07-28 07:50:28.000000 gspatial_plot-0.2.0/gspatial_plot.egg-info/top_level.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       79 2023-07-28 07:50:28.820134 gspatial_plot-0.2.0/setup.cfg
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1335 2023-07-28 07:22:55.000000 gspatial_plot-0.2.0/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:50:28.819787 gspatial_plot-0.2.0/tests/
+-rwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-28 07:27:24.000000 gspatial_plot-0.2.0/tests/test_functions.py
```

### Comparing `gspatial_plot-0.1.2/LICENSE` & `gspatial_plot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/PKG-INFO` & `gspatial_plot-0.2.0/gspatial_plot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gspatial_plot
-Version: 0.1.2
+Name: gspatial-plot
+Version: 0.2.0
 Summary: A geospatial plotting library built on top of geopandas.
 Home-page: https://github.com/ambeelabs/gspatial_plot/
 Author: Ambee
 License: MIT
 Keywords: geospatial plot geopandas maps plotting graph folium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gspatial_plot-0.1.2/README.md` & `gspatial_plot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/config.py` & `gspatial_plot-0.2.0/gspatial_plot/config.py`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shp` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_admin_0_countries.shx` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.dbf` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_geographic_lines.shp` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_geographic_lines.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.dbf` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shp` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_lakes.shx` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_lakes.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_ocean.shp` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_ocean.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.dbf`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shp`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx` & `gspatial_plot-0.2.0/gspatial_plot/datasets/ne_50m_rivers_lake_centerlines.shx`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/datasets/us_states.geojson` & `gspatial_plot-0.2.0/gspatial_plot/datasets/us_states.geojson`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/gspatial_plot/plot.py` & `gspatial_plot-0.2.0/gspatial_plot/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 import folium
 from sklearn.neighbors import KNeighborsRegressor
 from geopandas.plotting import _PolygonPatch
 from shapely.affinity import scale
 from shapely.geometry import Polygon
 from shapely.validation import make_valid
+import rioxarray
+from rasterio.plot import show
 from .config import (
     colors,
     countries,
     ocean,
     gridlines,
     rivers,
     lakes,
@@ -57,15 +59,15 @@
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
         colors (list/tuple, optional): List of colors to sample from. Defaults to a predefined set of colors.
         **geopandas_plot_kwds: Geopandas plot keyword arguments
 
     Returns:
         ax: matplotlib axis object
-    
+
     """
     np.random.seed(seed=seed)
     colors = np.random.choice(colors, size=len(data))
 
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize, facecolor=facecolor)
 
@@ -270,15 +272,14 @@
     title_kwds={},
     figsize=(15, 15),
     cmap="YlOrRd",
     facecolor="white",
     scheme="percentiles",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     legend=True,
     annot=False,
     annot_column=None,
     annot_align="center",
     annot_kwds={},
     ax=None,
     axis_on=False,
@@ -294,15 +295,14 @@
         title_kwds (dict, optional): Keyword arguments to matplotlib.pyplot.title. Defaults to {}.
         figsize (tuple, optional): Figure size. Defaults to (15, 15).
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         facecolor (str, optional): Figure's face color. Defaults to "white".
         scheme (str, optional): mapclassify scheme for assigning colors. Defaults to "percentiles".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         legend (bool, optional): If True, legend is displayed. Defaults to True.
         annot (bool, optional): If True, annotations are generated. Defaults to False.
         annot_column (str/GeoDataFrame column, optional): If annot is True, column should b passed as source for annotation. Defaults to None.
         annot_align (str, optional): Text alignment for annotation. Defaults to "center".
         annot_kwds (dict, optional): Keyword arguments for annotation. Defaults to {}.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
@@ -321,29 +321,23 @@
     ax.axis("off")
 
     if axis_on == True:
         ax.axis("on")
 
     ax = data.boundary.plot(color=boundarycolor, linewidth=boundary_linewidth, ax=ax)
 
-    if scale_colorbar == True:
-        legend = False
-
     data.plot(
         ax=ax,
         column=column,
         cmap=cmap,
         scheme=scheme,
         legend=legend,
         **geopandas_plot_kwds,
     )
 
-    if scale_colorbar == True:
-        ax.figure.colorbar(ax.collections[1], fraction=0.023, ax=ax)
-
     if annot == True and annot_column is not None:
         data.apply(
             lambda x: ax.annotate(
                 text=x[annot_column],
                 xy=x.geometry.representative_point().coords[0],
                 ha=annot_align,
                 **annot_kwds,
@@ -369,15 +363,14 @@
     linewidth=0.5,
     cmap="YlOrRd",
     edgecolor="black",
     facecolor="white",
     scheme="percentiles",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     legend=True,
     annot=False,
     annot_column=None,
     annot_align="center",
     annot_kwds={},
     ax=None,
     axis_on=False,
@@ -401,15 +394,14 @@
         linewidth (float, optional): Width of lines for shapes. Defaults to 0.5.
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         edgecolor (str, optional): Map's edge color. Defaults to "black".
         facecolor (str, optional): Figure's face color. Defaults to "white".
         scheme (str, optional): mapclassify scheme for assigning colors. Defaults to "percentiles".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         legend (bool, optional): If True, legend is displayed. Defaults to True.
         annot (bool, optional): If True, annotations are generated. Defaults to False.
         annot_column (str/GeoDataFrame column, optional): If annot is True, column should b passed as source for annotation. Defaults to None.
         annot_align (str, optional): Text alignment for annotation. Defaults to "center".
         annot_kwds (dict, optional): Keyword arguments for annotation. Defaults to {}.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
@@ -468,32 +460,26 @@
                     linewidth=boundary_linewidth,
                     zorder=0,
                     ax=ax,
                 )
             else:
                 ax = shapeplot(base, color=basecolor, linewidth=linewidth, ax=ax)
 
-    if scale_colorbar == True:
-        legend = False
-
     plot_data.plot(
         ax=ax,
         column=column,
         markersize="size",
         linewidth=linewidth,
         cmap=cmap,
         edgecolor=edgecolor,
         scheme=scheme,
         legend=legend,
         **geopandas_plot_kwds,
     )
 
-    if scale_colorbar == True:
-        ax.figure.colorbar(ax.collections[1], fraction=0.023, ax=ax)
-
     if annot == True and annot_column is not None:
         data.apply(
             lambda x: ax.annotate(
                 text=x[annot_column],
                 xy=x.geometry.representative_point().coords[0],
                 ha=annot_align,
                 **annot_kwds,
@@ -516,15 +502,14 @@
     linewidth=0.5,
     cmap="YlOrRd",
     edgecolor="black",
     facecolor="white",
     scheme="percentiles",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     legend=True,
     annot=False,
     annot_column=None,
     annot_align="center",
     annot_kwds={},
     ax=None,
     axis_on=False,
@@ -545,15 +530,14 @@
         linewidth (float, optional): Width of lines for shapes. Defaults to 0.5.
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         edgecolor (str, optional): Map's edge color. Defaults to "black".
         facecolor (str, optional): Figure's face color. Defaults to "white".
         scheme (str, optional): mapclassify scheme for assigning colors. Defaults to "percentiles".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         legend (bool, optional): If True, legend is displayed. Defaults to True.
         annot (bool, optional): If True, annotations are generated. Defaults to False.
         annot_column (str/GeoDataFrame column, optional): If annot is True, column should b passed as source for annotation. Defaults to None.
         annot_align (str, optional): Text alignment for annotation. Defaults to "center".
         annot_kwds (dict, optional): Keyword arguments for annotation. Defaults to {}.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
@@ -599,32 +583,26 @@
         if base_boundary == True:
             ax = data.boundary.plot(
                 color=boundarycolor, linewidth=boundary_linewidth, ax=ax
             )
         else:
             ax = shapeplot(data, color=basecolor, linewidth=linewidth, ax=ax)
 
-    if scale_colorbar == True:
-        legend = False
-
     plot_data.plot(
         ax=ax,
         column=column,
         markersize="size",
         cmap=cmap,
         linewidth=linewidth,
         edgecolor=edgecolor,
         scheme=scheme,
         legend=legend,
         **geopandas_plot_kwds,
     )
 
-    if scale_colorbar == True:
-        ax.figure.colorbar(ax.collections[1], fraction=0.023, ax=ax)
-
     if annot == True and annot_column is not None:
         data.apply(
             lambda x: ax.annotate(
                 text=x[annot_column],
                 xy=x.geometry.representative_point().coords[0],
                 ha=annot_align,
                 **annot_kwds,
@@ -644,15 +622,14 @@
     title=None,
     title_kwds={},
     figsize=(15, 15),
     cmap="YlOrRd",
     facecolor="white",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     ax=None,
     axis_on=False,
     **geopandas_plot_kwds,
 ):
     """
     Plots a kde plot over a GeoDataFrame
 
@@ -664,15 +641,14 @@
         point_data (bool, optional): Must be true if the type of data being mapped is point shape. Defaults to False.
         title (str, optional): Title of the map. Defaults to None.
         title_kwds (dict, optional): Keyword arguments to matplotlib.pyplot.title. Defaults to {}.
         figsize (tuple, optional): Figure size. Defaults to (15, 15).
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
         **geopandas_plot_kwds: Geopandas plot keyword arguments
 
 
     Returns:
         ax: matplotlib axis object
@@ -705,17 +681,14 @@
                 ax=ax,
                 **geopandas_plot_kwds,
             )
     plot_data = data.copy()
     if point_data == False:
         plot_data["geometry"] = plot_data.representative_point()
 
-    if scale_colorbar == True:
-        legend = False
-
     sns.kdeplot(
         x=plot_data["geometry"].x,
         y=plot_data["geometry"].y,
         fill=True,
         cmap=cmap,
         ax=ax,
     )
@@ -764,15 +737,14 @@
     title_kwds={},
     figsize=(15, 15),
     cmap="YlOrRd",
     facecolor="white",
     scheme="percentiles",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     legend=True,
     ax=None,
     annot=False,
     annot_column=None,
     annot_align="center",
     annot_kwds={},
     axis_on=False,
@@ -794,15 +766,14 @@
         title_kwds (dict, optional): Keyword arguments to matplotlib.pyplot.title. Defaults to {}.
         figsize (tuple, optional): Figure size. Defaults to (15, 15).
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         facecolor (str, optional): Figure's face color. Defaults to "white".
         scheme (str, optional): mapclassify scheme for assigning colors. Defaults to "percentiles".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         legend (bool, optional): If True, legend is displayed. Defaults to True.
         annot (bool, optional): If True, annotations are generated. Defaults to False.
         annot_column (str/GeoDataFrame column, optional): If annot is True, column should b passed as source for annotation. Defaults to None.
         annot_align (str, optional): Text alignment for annotation. Defaults to "center".
         annot_kwds (dict, optional): Keyword arguments for annotation. Defaults to {}.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
@@ -878,29 +849,23 @@
 
         grid = gpd.GeoDataFrame(
             grid, geometry=gpd.points_from_xy(grid["lon"], grid["lat"]), crs=data.crs
         )
 
         plot_data = grid
 
-    if scale_colorbar == True:
-        legend = False
-
     plot_data.plot(
         ax=ax,
         column=column,
         cmap=cmap,
         scheme=scheme,
         legend=legend,
         **geopandas_plot_kwds,
     )
 
-    if scale_colorbar == True:
-        ax.figure.colorbar(ax.collections[1], fraction=0.023, ax=ax)
-
     if clip == True:
         if base is not None:
             not_clip = base.copy()
         else:
             not_clip = data.copy()
 
         not_clip["dissolve"] = "Dissolve"
@@ -958,15 +923,14 @@
     linewidth=0.5,
     cmap="YlOrRd",
     edgecolor=None,
     facecolor="white",
     scheme="percentiles",
     boundarycolor="black",
     boundary_linewidth=0.5,
-    scale_colorbar=False,
     legend=True,
     annot=False,
     annot_column=None,
     annot_align="center",
     annot_kwds={},
     ax=None,
     axis_on=False,
@@ -994,15 +958,14 @@
         linewidth (float, optional): Width of lines for shapes. Defaults to 0.5.
         cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
         edgecolor (str, optional): Map's edge color. Defaults to "black".
         facecolor (str, optional): Figure's face color. Defaults to "white".
         scheme (str, optional): mapclassify scheme for assigning colors. Defaults to "percentiles".
         boundarycolor (str, optional): Map's boundary color. Defaults to "black".
         boundary_linewidth (float, optional): Linewidth of boundaries. Defaults to 0.5.
-        scale_colorbar (bool, optional): If True, the colorbar is scaled to the map extents. Defaults to False.
         legend (bool, optional): If True, legend is displayed. Defaults to True.
         annot (bool, optional): If True, annotations are generated. Defaults to False.
         annot_column (str/GeoDataFrame column, optional): If annot is True, column should b passed as source for annotation. Defaults to None.
         annot_align (str, optional): Text alignment for annotation. Defaults to "center".
         annot_kwds (dict, optional): Keyword arguments for annotation. Defaults to {}.
         ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
         axis_on (bool, optional): If True, axes will be visible. Defaults to False.
@@ -1051,16 +1014,14 @@
                     linewidth=boundary_linewidth,
                     zorder=0,
                     ax=ax,
                 )
             else:
                 ax = shapeplot(base, color=basecolor, linewidth=linewidth, ax=ax)
 
-    if scale_colorbar == True:
-        legend = False
     if not_wgs84 == True:
         original_crs = data.crs
         plot_data = plot_data.to_crs("4326")
     if shape == "rectangle":
         plot_data["geometry"] = plot_data.apply(
             lambda a: Polygon(
                 [
@@ -1098,17 +1059,14 @@
         cmap=cmap,
         edgecolor=edgecolor,
         scheme=scheme,
         legend=legend,
         **geopandas_plot_kwds,
     )
 
-    if scale_colorbar == True:
-        ax.figure.colorbar(ax.collections[1], fraction=0.023, ax=ax)
-
     if annot == True and annot_column is not None:
         data.apply(
             lambda x: ax.annotate(
                 text=x[annot_column],
                 xy=x.geometry.representative_point().coords[0],
                 ha=annot_align,
                 **annot_kwds,
@@ -1334,7 +1292,142 @@
     ocean_json.add_to(m)
     lines_json.add_to(m)
     rivers_json.add_to(m)
     lakes_json.add_to(m)
 
     return m
 
+
+def plot_xarray_raster(
+    data,
+    field=None,
+    title=None,
+    title_kwds={},
+    figsize=(15, 15),
+    cmap="YlOrRd",
+    clip_bbox=False,
+    bounds=None,
+    bounds_crs=None,
+    clip_gdf=False,
+    gdf=None,
+    lower_limit=None,
+    upper_limit=None,
+    facecolor="white",
+    robust=True,
+    legend_kwds={},
+    ax=None,
+    axis_on=False,
+    **xarray_plot_kwds,
+):
+    """Plots raster xarray data and returns axis. This is a wrapper around xarray plot function.
+
+    Args:
+        data (xarray Dataset/DataArray): Xarray raster data to plot
+        field (str, optional): The field of Dataset to plot. This is only applicable for Dataset. Defaults to None.
+        title (str, optional): Title for the plot. Defaults to None.
+        title_kwds (dict, optional): title_kwds (dict, optional): Keyword arguments to matplotlib.pyplot.title. Defaults to {}.
+        figsize (tuple, optional): Figure size. Defaults to (15, 15).
+        cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
+        clip_bbox (bool, optional): Clips to bounds if True. Defaults to False.
+        bounds (list, optional): Bounding box for clipping. Defaults to None.
+        bounds_crs (str, optional): CRS for Bounding Box. Defaults to None.
+        clip_gdf (bool, optional): Clips to a GeoDataFrame if True. Defaults to False.
+        gdf (GeoDataFrame, optional): GeoDataFrame to clip the raster. Defaults to None.
+        lower_limit (float, optional): Lower limit for the scale. Defaults to None.
+        upper_limit (float, optional):  Upper limit for the scale. Defaults to None.
+        facecolor (str, optional): Figure's face color. Defaults to "white".
+        robust (bool, optional): Uses data between 2% to 98% for figure scale if True. Defaults to True.
+        legend_kwds (dict, optional): Keywords for colorbar/legend. Defaults to {}.
+        ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
+        axis_on (bool, optional): If True, axes will be visible. Defaults to False.
+        **xarray_plot_kwds: Keywords for xarray plot.
+
+    Returns:
+        ax: matplotlib axis object
+    """
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize, facecolor=facecolor)
+
+    ax.axis("off")
+
+    if axis_on == True:
+        ax.axis("on")
+    if field is not None:
+        data = data[field]
+    if clip_bbox == True:
+        if bounds_crs is not None:
+            data = data.rio.clip_box(
+                bounds[0], bounds[1], bounds[2], bounds[3], crs=bounds_crs
+            )
+        else:
+            data = data.rio.clip_box(bounds[0], bounds[1], bounds[2], bounds[3])
+    if clip_gdf == True:
+        data = data.rio.clip(gdf.geometry.values, gdf.crs, drop=True)
+    if lower_limit is not None:
+        data = data.where(data >= lower_limit)
+    if upper_limit is not None:
+        data = data.where(data <= upper_limit)
+    if len(legend_kwds) > 0:
+        data.plot(
+            ax=ax,
+            cmap=cmap,
+            robust=robust,
+            cbar_kwargs=legend_kwds,
+            **xarray_plot_kwds,
+        )
+    else:
+        data.plot(
+            ax=ax,
+            cmap=cmap,
+            robust=robust,
+            **xarray_plot_kwds,
+        )
+    if title is not None:
+        ax.set_title(title, **title_kwds)
+    return ax
+
+
+def show_raster(
+    data,
+    title=None,
+    title_kwds={},
+    figsize=(15, 15),
+    cmap="YlOrRd",
+    facecolor="white",
+    colorbar=False,
+    legend_kwds={},
+    ax=None,
+    axis_on=False,
+    **show_kwds,
+):
+    """Wrapper around rasterio show with additional functionalities like better defaults and colorbar.
+
+    Args:
+        data (rasterio DatasetReader): Data to plot
+        title (str, optional): Title for the plot. Defaults to None.
+        title_kwds (dict, optional): title_kwds (dict, optional): Keyword arguments to matplotlib.pyplot.title. Defaults to {}.
+        figsize (tuple, optional): Figure size. Defaults to (15, 15).
+        cmap (str, optional): Colormap for the plot. Defaults to "YlOrRd".
+        facecolor (str, optional): Figure's face color. Defaults to "white".
+        colorbar (bool, optional): Inserts colorbar if True. Defaults to False.
+        legend_kwds (dict, optional): Keywords for colorbar/legend. Defaults to {}.
+        ax (matplotlib axis, optional): axis must be passed if plotting needs to be done on an existing axis. Defaults to None.
+        axis_on (bool, optional): If True, axes will be visible. Defaults to False.
+        **show_kwds: Additional keywords for rasterio show function
+    Returns:
+        ax: matplotlib axis object
+    """
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize, facecolor=facecolor)
+
+    if title is not None:
+        plt.title(title, **title_kwds)
+
+    ax.axis("off")
+    if axis_on == True:
+        ax.axis("on")
+
+    plot = show(data, ax=ax, cmap=cmap, **show_kwds)
+    if colorbar == True:
+        im = plot.get_images()[0]
+        fig.colorbar(im, ax=ax, **legend_kwds)
+    return ax
```

### Comparing `gspatial_plot-0.1.2/gspatial_plot.egg-info/PKG-INFO` & `gspatial_plot-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gspatial-plot
-Version: 0.1.2
+Name: gspatial_plot
+Version: 0.2.0
 Summary: A geospatial plotting library built on top of geopandas.
 Home-page: https://github.com/ambeelabs/gspatial_plot/
 Author: Ambee
 License: MIT
 Keywords: geospatial plot geopandas maps plotting graph folium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gspatial_plot-0.1.2/gspatial_plot.egg-info/SOURCES.txt` & `gspatial_plot-0.2.0/gspatial_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gspatial_plot-0.1.2/setup.py` & `gspatial_plot-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name="gspatial_plot",
     packages=find_packages(include=["gspatial_plot"]),
-    version="0.1.2",
+    version="0.2.0",
     author="Ambee",
     license="MIT",
     url='https://github.com/ambeelabs/gspatial_plot/',
     description="A geospatial plotting library built on top of geopandas.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[
         "Fiona>=1.8.22",
         "folium>=0.12.1.post1",
         "geopandas>=0.11.0",
         "mapclassify>=2.5.0",
         "matplotlib>=3.6.2",
         "pandas>=1.5.2",
         "pyproj>=3.4.1",
+        "rasterio>=1.3.8",
+        "rioxarray>=0.13.3",
         "scikit-learn>=1.0.1",
         "scipy>=1.10.0",
         "seaborn>=0.12.2",
         "Shapely>=1.8.2",
     ],
      classifiers=[
         'Development Status :: 4 - Beta',
```

