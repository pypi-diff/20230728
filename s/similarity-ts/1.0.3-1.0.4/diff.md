# Comparing `tmp/similarity_ts-1.0.3.tar.gz` & `tmp/similarity_ts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity_ts-1.0.3.tar", last modified: Wed Jul 19 11:49:19 2023, max compression
+gzip compressed data, was "similarity_ts-1.0.4.tar", last modified: Thu Jul 27 22:17:16 2023, max compression
```

## Comparing `similarity_ts-1.0.3.tar` & `similarity_ts-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.646683 similarity_ts-1.0.3/
--rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.3/LICENSE
--rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-19 11:49:19.646443 similarity_ts-1.0.3/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)    16688 2023-07-19 11:48:18.000000 similarity_ts-1.0.3/README.md
--rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-19 11:43:47.000000 similarity_ts-1.0.3/pyproject.toml
--rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-19 11:49:19.646743 similarity_ts-1.0.3/setup.cfg
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.632861 similarity_ts-1.0.3/src/
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.635627 similarity_ts-1.0.3/src/similarity_ts/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/__init__.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.638168 similarity_ts-1.0.3/src/similarity_ts/helpers/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/csv_reader_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/dynamic_import_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.3/src/similarity_ts/helpers/window_sampler.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.642182 similarity_ts-1.0.3/src/similarity_ts/metrics/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/cc.py
--rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/cp.py
--rw-r--r--   0 afdez      (501) staff       (20)     1164 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/hi.py
--rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/js.py
--rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/kl.py
--rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/ks.py
--rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric.py
--rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/metric_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.3/src/similarity_ts/metrics/mmd.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.646040 similarity_ts-1.0.3/src/similarity_ts/plots/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.3/src/similarity_ts/plots/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.3/src/similarity_ts/plots/delta.py
--rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.3/src/similarity_ts/plots/dimensionalty_reduction.py
--rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/pca.py
--rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot.py
--rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.3/src/similarity_ts/plots/plot_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.3/src/similarity_ts/plots/tsne.py
--rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.3/src/similarity_ts/plots/two_dimensions.py
--rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_analysis_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_ts.py
--rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.3/src/similarity_ts/similarity_ts_config.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-19 11:49:19.636972 similarity_ts-1.0.3/src/similarity_ts.egg-info/
--rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/SOURCES.txt
--rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/dependency_links.txt
--rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/requires.txt
--rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-19 11:49:19.000000 similarity_ts-1.0.3/src/similarity_ts.egg-info/top_level.txt
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.886408 similarity_ts-1.0.4/
+-rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.4/LICENSE
+-rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-27 22:17:16.886125 similarity_ts-1.0.4/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)    16688 2023-07-19 11:48:18.000000 similarity_ts-1.0.4/README.md
+-rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-27 22:17:09.000000 similarity_ts-1.0.4/pyproject.toml
+-rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-27 22:17:16.886477 similarity_ts-1.0.4/setup.cfg
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.872956 similarity_ts-1.0.4/src/
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.875751 similarity_ts-1.0.4/src/similarity_ts/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.4/src/similarity_ts/__init__.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.878812 similarity_ts-1.0.4/src/similarity_ts/helpers/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.4/src/similarity_ts/helpers/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.4/src/similarity_ts/helpers/csv_reader_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.4/src/similarity_ts/helpers/dynamic_import_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.4/src/similarity_ts/helpers/window_sampler.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.882679 similarity_ts-1.0.4/src/similarity_ts/metrics/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/cc.py
+-rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/cp.py
+-rw-r--r--   0 afdez      (501) staff       (20)      776 2023-07-27 22:09:10.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/hi.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/js.py
+-rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/kl.py
+-rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/ks.py
+-rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/metric.py
+-rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/metric_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/metric_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/metric_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.4/src/similarity_ts/metrics/mmd.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.885710 similarity_ts-1.0.4/src/similarity_ts/plots/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.4/src/similarity_ts/plots/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.4/src/similarity_ts/plots/delta.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.4/src/similarity_ts/plots/dimensionalty_reduction.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.4/src/similarity_ts/plots/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.4/src/similarity_ts/plots/pca.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.4/src/similarity_ts/plots/plot.py
+-rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.4/src/similarity_ts/plots/plot_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.4/src/similarity_ts/plots/plot_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.4/src/similarity_ts/plots/plot_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.4/src/similarity_ts/plots/tsne.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.4/src/similarity_ts/plots/two_dimensions.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.4/src/similarity_ts/similarity_analysis_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.4/src/similarity_ts/similarity_ts.py
+-rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.4/src/similarity_ts/similarity_ts_config.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-27 22:17:16.877452 similarity_ts-1.0.4/src/similarity_ts.egg-info/
+-rw-r--r--   0 afdez      (501) staff       (20)    17416 2023-07-27 22:17:16.000000 similarity_ts-1.0.4/src/similarity_ts.egg-info/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-27 22:17:16.000000 similarity_ts-1.0.4/src/similarity_ts.egg-info/SOURCES.txt
+-rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-27 22:17:16.000000 similarity_ts-1.0.4/src/similarity_ts.egg-info/dependency_links.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-27 22:17:16.000000 similarity_ts-1.0.4/src/similarity_ts.egg-info/requires.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-27 22:17:16.000000 similarity_ts-1.0.4/src/similarity_ts.egg-info/top_level.txt
```

### Comparing `similarity_ts-1.0.3/LICENSE` & `similarity_ts-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/PKG-INFO` & `similarity_ts-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity_ts
-Version: 1.0.3
+Version: 1.0.4
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `similarity_ts-1.0.3/README.md` & `similarity_ts-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/pyproject.toml` & `similarity_ts-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "similarity_ts"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Alejandro Fernández-Montes", email = "afdez@us.es" },
     { name = "Damián Fernández-Cerero", email = "damiancerero@us.es" },
     { name = "Felipe Escalera González", email = "fescalera@us.es" },
 ]
 dependencies = ["dtaidistance", "matplotlib", "pandas", "scikit-learn", "tqdm", "natsort", "chardet"]
 description = "SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data"
```

### Comparing `similarity_ts-1.0.3/src/similarity_ts/helpers/csv_reader_helper.py` & `similarity_ts-1.0.4/src/similarity_ts/helpers/csv_reader_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/helpers/dynamic_import_helper.py` & `similarity_ts-1.0.4/src/similarity_ts/helpers/dynamic_import_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/helpers/window_sampler.py` & `similarity_ts-1.0.4/src/similarity_ts/helpers/window_sampler.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/cc.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/cc.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/cp.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/cp.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/hi.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/hi.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/js.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/js.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/kl.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/ks.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/ks.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/metric_computer.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/metric_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/metric_factory.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/metrics/mmd.py` & `similarity_ts-1.0.4/src/similarity_ts/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/delta.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/delta.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/dimensionalty_reduction.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/dimensionalty_reduction.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/dtw.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/dtw.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/pca.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/pca.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/plot.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/plot.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/plot_computer.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/plot_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/plot_config.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/plot_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/plot_factory.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/plot_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/tsne.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/tsne.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/plots/two_dimensions.py` & `similarity_ts-1.0.4/src/similarity_ts/plots/two_dimensions.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/similarity_analysis_computer.py` & `similarity_ts-1.0.4/src/similarity_ts/similarity_analysis_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/similarity_ts.py` & `similarity_ts-1.0.4/src/similarity_ts/similarity_ts.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts/similarity_ts_config.py` & `similarity_ts-1.0.4/src/similarity_ts/similarity_ts_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.3/src/similarity_ts.egg-info/PKG-INFO` & `similarity_ts-1.0.4/src/similarity_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-ts
-Version: 1.0.3
+Version: 1.0.4
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `similarity_ts-1.0.3/src/similarity_ts.egg-info/SOURCES.txt` & `similarity_ts-1.0.4/src/similarity_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

