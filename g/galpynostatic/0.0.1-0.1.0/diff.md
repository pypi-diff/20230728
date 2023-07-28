# Comparing `tmp/galpynostatic-0.0.1.tar.gz` & `tmp/galpynostatic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galpynostatic-0.0.1.tar", last modified: Thu Jul 27 22:58:36 2023, max compression
+gzip compressed data, was "galpynostatic-0.1.0.tar", last modified: Fri Jul 28 00:23:21 2023, max compression
```

## Comparing `galpynostatic-0.0.1.tar` & `galpynostatic-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 ffernandez  (1000) ffernandez  (1000)        0 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     1084 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/CHANGELOG.md
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     1081 2023-06-23 16:51:15.000000 galpynostatic-0.0.1/LICENSE
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)      278 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/MANIFEST.in
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     5185 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/PKG-INFO
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     3034 2023-07-27 22:51:32.000000 galpynostatic-0.0.1/README.md
-drwxrwxr-x   0 ffernandez  (1000) ffernandez  (1000)        0 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/galpynostatic/
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     1379 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/__init__.py
-drwxrwxr-x   0 ffernandez  (1000) ffernandez  (1000)        0 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/galpynostatic/datasets/
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     2203 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/datasets/__init__.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)    22929 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/datasets/cylindrical.csv
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     3481 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/datasets/map.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)    22082 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/datasets/planar.csv
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)    22403 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/datasets/spherical.csv
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     3786 2023-06-27 23:17:00.000000 galpynostatic-0.0.1/galpynostatic/make_prediction.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)    11994 2023-07-06 15:52:13.000000 galpynostatic-0.0.1/galpynostatic/model.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     6025 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/plot.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     4605 2023-07-05 23:52:44.000000 galpynostatic-0.0.1/galpynostatic/preprocessing.py
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     2352 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/galpynostatic/utils.py
-drwxrwxr-x   0 ffernandez  (1000) ffernandez  (1000)        0 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/galpynostatic.egg-info/
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     5185 2023-07-27 22:58:36.000000 galpynostatic-0.0.1/galpynostatic.egg-info/PKG-INFO
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)      574 2023-07-27 22:58:36.000000 galpynostatic-0.0.1/galpynostatic.egg-info/SOURCES.txt
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)        1 2023-07-27 22:58:36.000000 galpynostatic-0.0.1/galpynostatic.egg-info/dependency_links.txt
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)       62 2023-07-27 22:58:36.000000 galpynostatic-0.0.1/galpynostatic.egg-info/requires.txt
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)       14 2023-07-27 22:58:36.000000 galpynostatic-0.0.1/galpynostatic.egg-info/top_level.txt
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)     1493 2023-06-23 16:51:41.000000 galpynostatic-0.0.1/pyproject.toml
--rw-rw-r--   0 ffernandez  (1000) ffernandez  (1000)       38 2023-07-27 22:58:36.382323 galpynostatic-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:21.592158 galpynostatic-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-28 00:23:21.592158 galpynostatic-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:21.588158 galpynostatic-0.1.0/galpynostatic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:21.592158 galpynostatic-0.1.0/galpynostatic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/datasets/cylindrical.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22082 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/datasets/planar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/datasets/spherical.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/make_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/galpynostatic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:23:21.588158 galpynostatic-0.1.0/galpynostatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-28 00:23:21.000000 galpynostatic-0.1.0/galpynostatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-28 00:23:21.000000 galpynostatic-0.1.0/galpynostatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:23:21.000000 galpynostatic-0.1.0/galpynostatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 00:23:21.000000 galpynostatic-0.1.0/galpynostatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 00:23:21.000000 galpynostatic-0.1.0/galpynostatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 00:23:04.000000 galpynostatic-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:23:21.592158 galpynostatic-0.1.0/setup.cfg
```

### Comparing `galpynostatic-0.0.1/CHANGELOG.md` & `galpynostatic-0.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog of galpynostatic
 
-# v0.1.0 (2023-??-??)
+# v0.1.0 (2023-07-27)
 
 This is the first Python object-oriented version of galpynostatic.
 
 ## Features
 
 - A galvanostatic regressor to fit maximum State-of-Charge (SOC) values versus C-rates experimental data with the physics-based heuristic model implemented here. 
 - Visualization in different formats through a plotter.
```

### Comparing `galpynostatic-0.0.1/LICENSE` & `galpynostatic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/PKG-INFO` & `galpynostatic-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galpynostatic
-Version: 0.0.1
+Version: 0.1.0
 Summary: A physics-based heuristic model to predict the optimal electrode particle size for a fast-charging of lithium-ion batteries.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,17 +38,17 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # galpynostatic
 
 [![galpynostatics CI](https://github.com/fernandezfran/galpynostatic/actions/workflows/CI.yml/badge.svg)](https://github.com/fernandezfran/galpynostatic/actions/workflows/CI.yml)
+[![coverage status](https://coveralls.io/repos/github/fernandezfran/galpynostatic/badge.svg)](https://coveralls.io/github/fernandezfran/galpynostatic)
 [![documentation status](https://readthedocs.org/projects/galpynostatic/badge/?version=latest)](https://galpynostatic.readthedocs.io/en/latest/?badge=latest)
 [![pypi version](https://img.shields.io/pypi/v/galpynostatic)](https://pypi.org/project/galpynostatic/)
-[![pypi downloads](https://img.shields.io/pypi/dw/galpynostatic?label=PyPI%20Downloads)](https://pypistats.org/packages/galpynostatic)
 [![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
 [![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
 [![doi](https://img.shields.io/badge/doi-10.1016/j.electacta.2023.142951-36abe8)](https://doi.org/10.1016/j.electacta.2023.142951)
 
 **galpynostatic** is a Python package with a physics-based heuristic model to 
 predict the optimal electrode particle size for a fast-charging of lithium-ion
 batteries.
@@ -90,27 +90,36 @@
 galpynostatic is under 
 [MIT License](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE).
 
 
 ## Citation
 
 If you use galpynostatic in a scientific publication, we would appreciate it if 
-you could cite the following [article](https://www.doi.org/):
+you could cite the following 
+[article](https://www.doi.org/10.1016/j.electacta.2023.142951)
 
 > F. Fernandez, E. M. Gavilán-Arriazu, D. E. Barraco, A. Visintin, Y. Ein-Eli, 
 > E. P. M. Leiva. "Towards a fast-charging of LIBs electrode materials: a 
-> heuristic model based on galvanostatic simulations" (2023). _TODO_
+> heuristic model based on galvanostatic simulations" (2023). _Electrochimica 
+> Acta_
 
 BibTeX entry:
 
 ```bibtex
 @article{fernandez2023towards,
-  title={Towards a fast-charging of LIBs electrode materials: a heuristic model based on galvanostatic simulations},
-  author={Fernandez, Francisco and Gavilán, Maximiliano and Barraco, Daniel and Visintín, Aldo and Ein-Eli, Yair and Leiva, Ezequiel},
-  year={2023}
+    title = {Towards a fast-charging of LIBs electrode materials: a heuristic model based on galvanostatic simulations},
+    journal = {Electrochimica Acta},
+    pages = {142951},
+    year = {2023},
+    issn = {0013-4686},
+    doi = {https://doi.org/10.1016/j.electacta.2023.142951},
+    url = {https://www.sciencedirect.com/science/article/pii/S001346862301126X},
+    author = {F. Fernandez and E.M. Gavilán-Arriazu and D.E. Barraco and A. Visintin and Y. Ein-Eli and E.P.M. Leiva},
+    keywords = {Fast-charging, Lithium-Ion Battery, Heuristic Model, Galvanostatic charge},
+    abstract = {Fast charging is one of the most important features to be accomplished for the improvement of electric vehicles. In the search for optimal use of active materials for this aim, we present a recipe to find the conditions for fast charging, fifteen minutes for 80 % of the State-of-Charge, of lithium-ion battery's single particle electrodes, thus taking advantage of the maximum possible capacity. A guide based on a general model that considers diffusion and charge transfer limitations under constant current is proposed. This guide was constructed on the basis of our previous theoretical development. A Python free and user-friendly package is provided to handle all experimental data processing and estimations.}
 }
 ```
 
 
 ## Contact
 
 You can contact me if you have any questions at <ffernandev@gmail.com>
```

### Comparing `galpynostatic-0.0.1/galpynostatic/__init__.py` & `galpynostatic-0.1.0/galpynostatic/__init__.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/datasets/__init__.py` & `galpynostatic-0.1.0/galpynostatic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/datasets/cylindrical.csv` & `galpynostatic-0.1.0/galpynostatic/datasets/cylindrical.csv`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/datasets/map.py` & `galpynostatic-0.1.0/galpynostatic/datasets/map.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/datasets/planar.csv` & `galpynostatic-0.1.0/galpynostatic/datasets/planar.csv`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/datasets/spherical.csv` & `galpynostatic-0.1.0/galpynostatic/datasets/spherical.csv`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/make_prediction.py` & `galpynostatic-0.1.0/galpynostatic/make_prediction.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/model.py` & `galpynostatic-0.1.0/galpynostatic/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     :ref:`galpynostatic.map`).
 
     References
     ----------
     .. [1] F. Fernandez, E. M. Gavilán-Arriazu, D. E. Barraco, A. Visintin,
        Y. Ein-Eli, E. P. M. Leiva, 2023. Towards a fast-charging of LIBs
        electrode materials: a heuristic model based on galvanostatic
-       simulations. _TODO_.
+       simulations. `Electrochimica Acta`.
 
     Attributes
     ----------
     dcoeff_ : float
         Predicted diffusion coefficient in :math:`cm^2/s`.
 
     dcoeff_err_ : float
```

### Comparing `galpynostatic-0.0.1/galpynostatic/plot.py` & `galpynostatic-0.1.0/galpynostatic/plot.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/preprocessing.py` & `galpynostatic-0.1.0/galpynostatic/preprocessing.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic/utils.py` & `galpynostatic-0.1.0/galpynostatic/utils.py`

 * *Files identical despite different names*

### Comparing `galpynostatic-0.0.1/galpynostatic.egg-info/PKG-INFO` & `galpynostatic-0.1.0/galpynostatic.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galpynostatic
-Version: 0.0.1
+Version: 0.1.0
 Summary: A physics-based heuristic model to predict the optimal electrode particle size for a fast-charging of lithium-ion batteries.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,17 +38,17 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # galpynostatic
 
 [![galpynostatics CI](https://github.com/fernandezfran/galpynostatic/actions/workflows/CI.yml/badge.svg)](https://github.com/fernandezfran/galpynostatic/actions/workflows/CI.yml)
+[![coverage status](https://coveralls.io/repos/github/fernandezfran/galpynostatic/badge.svg)](https://coveralls.io/github/fernandezfran/galpynostatic)
 [![documentation status](https://readthedocs.org/projects/galpynostatic/badge/?version=latest)](https://galpynostatic.readthedocs.io/en/latest/?badge=latest)
 [![pypi version](https://img.shields.io/pypi/v/galpynostatic)](https://pypi.org/project/galpynostatic/)
-[![pypi downloads](https://img.shields.io/pypi/dw/galpynostatic?label=PyPI%20Downloads)](https://pypistats.org/packages/galpynostatic)
 [![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
 [![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
 [![doi](https://img.shields.io/badge/doi-10.1016/j.electacta.2023.142951-36abe8)](https://doi.org/10.1016/j.electacta.2023.142951)
 
 **galpynostatic** is a Python package with a physics-based heuristic model to 
 predict the optimal electrode particle size for a fast-charging of lithium-ion
 batteries.
@@ -90,27 +90,36 @@
 galpynostatic is under 
 [MIT License](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE).
 
 
 ## Citation
 
 If you use galpynostatic in a scientific publication, we would appreciate it if 
-you could cite the following [article](https://www.doi.org/):
+you could cite the following 
+[article](https://www.doi.org/10.1016/j.electacta.2023.142951)
 
 > F. Fernandez, E. M. Gavilán-Arriazu, D. E. Barraco, A. Visintin, Y. Ein-Eli, 
 > E. P. M. Leiva. "Towards a fast-charging of LIBs electrode materials: a 
-> heuristic model based on galvanostatic simulations" (2023). _TODO_
+> heuristic model based on galvanostatic simulations" (2023). _Electrochimica 
+> Acta_
 
 BibTeX entry:
 
 ```bibtex
 @article{fernandez2023towards,
-  title={Towards a fast-charging of LIBs electrode materials: a heuristic model based on galvanostatic simulations},
-  author={Fernandez, Francisco and Gavilán, Maximiliano and Barraco, Daniel and Visintín, Aldo and Ein-Eli, Yair and Leiva, Ezequiel},
-  year={2023}
+    title = {Towards a fast-charging of LIBs electrode materials: a heuristic model based on galvanostatic simulations},
+    journal = {Electrochimica Acta},
+    pages = {142951},
+    year = {2023},
+    issn = {0013-4686},
+    doi = {https://doi.org/10.1016/j.electacta.2023.142951},
+    url = {https://www.sciencedirect.com/science/article/pii/S001346862301126X},
+    author = {F. Fernandez and E.M. Gavilán-Arriazu and D.E. Barraco and A. Visintin and Y. Ein-Eli and E.P.M. Leiva},
+    keywords = {Fast-charging, Lithium-Ion Battery, Heuristic Model, Galvanostatic charge},
+    abstract = {Fast charging is one of the most important features to be accomplished for the improvement of electric vehicles. In the search for optimal use of active materials for this aim, we present a recipe to find the conditions for fast charging, fifteen minutes for 80 % of the State-of-Charge, of lithium-ion battery's single particle electrodes, thus taking advantage of the maximum possible capacity. A guide based on a general model that considers diffusion and charge transfer limitations under constant current is proposed. This guide was constructed on the basis of our previous theoretical development. A Python free and user-friendly package is provided to handle all experimental data processing and estimations.}
 }
 ```
 
 
 ## Contact
 
 You can contact me if you have any questions at <ffernandev@gmail.com>
```

### Comparing `galpynostatic-0.0.1/galpynostatic.egg-info/SOURCES.txt` & `galpynostatic-0.1.0/galpynostatic.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+CITATION.bib
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 galpynostatic/__init__.py
 galpynostatic/make_prediction.py
 galpynostatic/model.py
```

### Comparing `galpynostatic-0.0.1/pyproject.toml` & `galpynostatic-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "galpynostatic"
-version = "0.0.1"
+version = "0.1.0"
 authors = [{name = "Francisco Fernandez", email = "ffernandev@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A physics-based heuristic model to predict the optimal electrode particle size for a fast-charging of lithium-ion batteries."
 keywords = [
     "battery",
     "physics-based",
```

