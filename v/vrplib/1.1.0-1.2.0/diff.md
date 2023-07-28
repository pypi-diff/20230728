# Comparing `tmp/vrplib-1.1.0.tar.gz` & `tmp/vrplib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrplib-1.1.0.tar", max compression
+gzip compressed data, was "vrplib-1.2.0.tar", max compression
```

## Comparing `vrplib-1.1.0.tar` & `vrplib-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1065 2022-04-16 13:56:24.912717 vrplib-1.1.0/LICENSE
--rw-r--r--   0        0        0     8247 2023-05-02 14:33:26.191015 vrplib-1.1.0/README.md
--rw-r--r--   0        0        0     1133 2023-05-15 09:50:28.677738 vrplib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-02-06 13:16:48.597040 vrplib-1.1.0/vrplib/__init__.py
--rw-r--r--   0        0        0      133 2023-04-18 19:36:43.150095 vrplib-1.1.0/vrplib/download/__init__.py
--rw-r--r--   0        0        0      358 2023-02-13 16:45:49.189310 vrplib-1.1.0/vrplib/download/constants.py
--rw-r--r--   0        0        0     1014 2023-04-26 17:05:13.976320 vrplib-1.1.0/vrplib/download/download_instance.py
--rw-r--r--   0        0        0      952 2023-04-26 17:05:13.977912 vrplib-1.1.0/vrplib/download/download_solution.py
--rw-r--r--   0        0        0     1263 2023-04-19 08:41:44.020458 vrplib-1.1.0/vrplib/download/download_utils.py
--rw-r--r--   0        0        0    18524 2023-02-06 13:16:48.598179 vrplib-1.1.0/vrplib/download/instance_data.csv
--rw-r--r--   0        0        0     1682 2023-04-19 08:31:58.419704 vrplib-1.1.0/vrplib/download/list_names.py
--rw-r--r--   0        0        0      123 2023-02-06 13:16:48.598476 vrplib-1.1.0/vrplib/parse/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 13:16:48.598565 vrplib-1.1.0/vrplib/parse/distances/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-15 09:50:15.783042 vrplib-1.1.0/vrplib/parse/parse_distances.py
--rw-r--r--   0        0        0     2084 2023-05-15 09:50:15.783357 vrplib-1.1.0/vrplib/parse/parse_solomon.py
--rw-r--r--   0        0        0     1069 2023-05-15 09:50:15.783884 vrplib-1.1.0/vrplib/parse/parse_solution.py
--rw-r--r--   0        0        0      424 2023-02-06 13:16:48.599632 vrplib-1.1.0/vrplib/parse/parse_utils.py
--rw-r--r--   0        0        0     4045 2023-05-15 09:50:15.784353 vrplib-1.1.0/vrplib/parse/parse_vrplib.py
--rw-r--r--   0        0        0       82 2023-02-06 13:16:48.601550 vrplib-1.1.0/vrplib/read/__init__.py
--rw-r--r--   0        0        0     1070 2023-05-15 09:44:35.624203 vrplib-1.1.0/vrplib/read/read_instance.py
--rw-r--r--   0        0        0      466 2023-05-15 09:44:35.624518 vrplib-1.1.0/vrplib/read/read_solution.py
--rw-r--r--   0        0        0     9252 1970-01-01 00:00:00.000000 vrplib-1.1.0/setup.py
--rw-r--r--   0        0        0     8993 1970-01-01 00:00:00.000000 vrplib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-04-16 13:56:24.912717 vrplib-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8361 2023-07-28 18:24:06.148139 vrplib-1.2.0/README.md
+-rw-r--r--   0        0        0     1113 2023-07-28 18:26:38.857939 vrplib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-02-06 13:16:48.597040 vrplib-1.2.0/vrplib/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-18 19:36:43.150095 vrplib-1.2.0/vrplib/download/__init__.py
+-rw-r--r--   0        0        0      358 2023-02-13 16:45:49.189310 vrplib-1.2.0/vrplib/download/constants.py
+-rw-r--r--   0        0        0     1014 2023-04-26 17:05:13.976320 vrplib-1.2.0/vrplib/download/download_instance.py
+-rw-r--r--   0        0        0      952 2023-04-26 17:05:13.977912 vrplib-1.2.0/vrplib/download/download_solution.py
+-rw-r--r--   0        0        0     1263 2023-04-19 08:41:44.020458 vrplib-1.2.0/vrplib/download/download_utils.py
+-rw-r--r--   0        0        0    18524 2023-02-06 13:16:48.598179 vrplib-1.2.0/vrplib/download/instance_data.csv
+-rw-r--r--   0        0        0     1682 2023-04-19 08:31:58.419704 vrplib-1.2.0/vrplib/download/list_names.py
+-rw-r--r--   0        0        0      123 2023-02-06 13:16:48.598476 vrplib-1.2.0/vrplib/parse/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 13:16:48.598565 vrplib-1.2.0/vrplib/parse/distances/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-15 09:50:15.783042 vrplib-1.2.0/vrplib/parse/parse_distances.py
+-rw-r--r--   0        0        0     2084 2023-05-15 09:50:15.783357 vrplib-1.2.0/vrplib/parse/parse_solomon.py
+-rw-r--r--   0        0        0     1069 2023-05-15 09:50:15.783884 vrplib-1.2.0/vrplib/parse/parse_solution.py
+-rw-r--r--   0        0        0      555 2023-07-28 18:21:23.517888 vrplib-1.2.0/vrplib/parse/parse_utils.py
+-rw-r--r--   0        0        0     4045 2023-07-22 19:01:50.524994 vrplib-1.2.0/vrplib/parse/parse_vrplib.py
+-rw-r--r--   0        0        0       82 2023-02-06 13:16:48.601550 vrplib-1.2.0/vrplib/read/__init__.py
+-rw-r--r--   0        0        0     1070 2023-05-15 09:44:35.624203 vrplib-1.2.0/vrplib/read/read_instance.py
+-rw-r--r--   0        0        0      466 2023-05-15 09:44:35.624518 vrplib-1.2.0/vrplib/read/read_solution.py
+-rw-r--r--   0        0        0     9066 1970-01-01 00:00:00.000000 vrplib-1.2.0/PKG-INFO
```

### Comparing `vrplib-1.1.0/LICENSE` & `vrplib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/README.md` & `vrplib-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,17 @@
     - `FLOOR_2D`: Round down all distances to down to an integer.
     - `EXACT_2D`: Multiply the distances by 1000, round to the nearest integer.
 - `EXPLICIT`: the distance data is explicitly provided, in partial or full form. The `EDGE_WEIGHT_FORMAT` specification must be present. We support the following two edge weight formats:
   - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.
   - `FULL_MATRIX`: Explicit full matrix representation.
   
 
+#### Line comments
+Lines starting with `#` are interpreted as comments and not parsed when reading the instance.
+
 #### More information about VRPLIB
 The VRPLIB format is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. 
 Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
 
 ### Solomon instance format
 The Solomon format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. A Solomon instance looks like this:
 ``` bash
```

### Comparing `vrplib-1.1.0/pyproject.toml` & `vrplib-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "vrplib"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python library for working with vehicle routing problem instances."
 authors = ["Leon Lan <leon.lanyidong@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/leonlan/VRPLIB"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.19"
-codecov = "^2.1.13"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.9"
 pytest = "^7.1.2"
 codecov = "^2.1.13"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.19.0"
```

### Comparing `vrplib-1.1.0/vrplib/download/download_instance.py` & `vrplib-1.2.0/vrplib/download/download_instance.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/download/download_solution.py` & `vrplib-1.2.0/vrplib/download/download_solution.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/download/download_utils.py` & `vrplib-1.2.0/vrplib/download/download_utils.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/download/instance_data.csv` & `vrplib-1.2.0/vrplib/download/instance_data.csv`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/download/list_names.py` & `vrplib-1.2.0/vrplib/download/list_names.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/parse/parse_distances.py` & `vrplib-1.2.0/vrplib/parse/parse_distances.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/parse/parse_solomon.py` & `vrplib-1.2.0/vrplib/parse/parse_solomon.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/parse/parse_solution.py` & `vrplib-1.2.0/vrplib/parse/parse_solution.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/parse/parse_vrplib.py` & `vrplib-1.2.0/vrplib/parse/parse_vrplib.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/vrplib/read/read_instance.py` & `vrplib-1.2.0/vrplib/read/read_instance.py`

 * *Files identical despite different names*

### Comparing `vrplib-1.1.0/setup.py` & `vrplib-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,197 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: vrplib
+Version: 1.2.0
+Summary: Python library for working with vehicle routing problem instances.
+Home-page: https://github.com/leonlan/VRPLIB
+License: MIT
+Author: Leon Lan
+Author-email: leon.lanyidong@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.19,<2.0)
+Project-URL: Repository, https://github.com/leonlan/VRPLIB
+Description-Content-Type: text/markdown
+
+# VRPLIB
+[![PyPI version](https://badge.fury.io/py/vrplib.svg)](https://badge.fury.io/py/vrplib)
+[![vrplib](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml/badge.svg)](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml)
+[![codecov](https://codecov.io/gh/leonlan/VRPLIB/branch/master/graph/badge.svg?token=X0X66LBNZ7)](https://codecov.io/gh/leonlan/VRPLIB)
+
+`vrplib` is a Python package for working with Vehicle Routing Problem (VRP) instances. The main features are:
+- reading VRPLIB and Solomon instances and solutions, and
+- downloading instances and best known solutions from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+
+## Installation
+`vrplib` works with Python 3.8+ and only depends on `numpy`.
+
+```shell
+pip install vrplib
+```
+
+## Example usage
+### Reading instances and solutions
+```python
+import vrplib
+
+# Read VRPLIB formatted instances (default)
+instance = vrplib.read_instance("/path/to/X-n101-k25.vrp")
+solution = vrplib.read_solution("/path/to/X-n101-k25.sol")
+
+# Read Solomon formatted instances
+instance = vrplib.read_instance("/path/to/C101.txt", instance_format="solomon")
+solution = vrplib.read_solution("/path/to/C101.sol") # only 1 solution format
+```
+
+`instance` and `solution` are dictionaries that contain all parsed data. 
+``` python
+>>> instance.keys()
+dict_keys(['name', ..., 'edge_weight'])
+
+>>> solution.keys()
+dict_keys(['routes', 'cost'])
+```
+
+
+### Downloading instances from CVRPLIB 
+``` python
+import vrplib
+
+# Download an instance and a solution file 
+vrplib.download_instance("X-n101-k25", "/path/to/instances/")
+vrplib.download_solution("X-n101-k25", "/path/to/solutions/")
+
+# List all instance names that can be downloaded 
+vrplib.list_names()                      # All instance names
+vrplib.list_names(low=100, high=200)     # Instances with between [100, 200] customers
+vrplib.list_names(vrp_type="cvrp")       # Only CVRP instances
+vrplib.list_names(vrp_type="vrptw")      # Only VRPTW instances
+```
+
+
+## Documentation
+- [VRPLIB instance format](#vrplib-instance-format)
+- [Solomon instance format](#solomon-instance-format)
+- [Solution format](#solution-format)
+- [Other remarks](#other-remarks)
+
+### VRPLIB instance format
+The VRPLIB format is the standard format for the Capacitated Vehicle Routing Problem (CVRP). An example VRPLIB instance looks as follows:
+``` bash
+NAME: Example 
+EDGE_WEIGHT_TYPE: EUC_2D
+NODE_COORD_SECTION
+1 0 0
+2 5 5
+SERVICE_TIME_SECTION
+1 0
+2 3
+DEPOT_SECTION
+1
+EOF
+```
+
+A VRPLIB instance contains problem **specifications** and problem **data**. 
+- Specifications are key-value pairs separated by a colon. In the example above, `NAME` and `EDGE_WEIGHT_TYPE` are the two data specifications.
+- Data are explicit array-like values such as customer coordinates or service times. 
+Each data section should start with a header name that ends with `_SECTION`, e.g., `NODE_COORD_SECTION` and `SERVICE_TIME_SECTION`. It is then followed by rows of values and each row must start with an index representing the depot or customer. 
+There are two exceptions: values in `EDGE_WEIGHT_SECTION` and `DEPOT_SECTION` should not start with an index.
+
+Besides the rules outlined above, `vrplib` is not strict about the naming of specifications or sections. 
+This means that you can use `vrplib` to read VRPLIB instances with custom specifications like `MY_SPECIFICATION: SOME_VALUE` and custom section names like `MY_SECTION`.
+
+Reading the above example instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'edge_weight_type': 'EUC_2D',
+ 'node_coord': array([[0, 0], [5, 5]]),
+ 'service_time': array([1, 3]),
+ 'depot': array([0]),
+ 'edge_weight': array([[0.  , 7.07106781], [7.07106781, 0.  ]])}
+```
+
+The depot section specifies which location index corresponds to the depot data. 
+The convention is to let index 1 represent the depot. 
+`vrplib` subtracts one from the depot value to make it easier to index.
+
+#### Computing edge weights 
+Note that the example instance did not include any explicit information about the edge weights, yet the output includes edge weights data.
+This is because `vrplib` automatically computes the edge weights based on the instance specifications, if applicable.
+In the example, the edge weight type specification and node coordinates data are used to compute the Euclidean distance.
+You can set the `compute_distances` argument in `read_instance` to disable this feature.
+
+Following the VRPLIB conventions, the edge weights are computed based on the `EDGE_WEIGHT_TYPE` specification, and in some cases the `EDGE_WEIGHT_FORMAT` specification. `vrplib` currently supports two categories of edge weight types:
+- `*_2D`: Euclidean distances based on the node coordinates data.
+    - `EUC_2D`: Double precision distances without rounding.
+    - `FLOOR_2D`: Round down all distances to down to an integer.
+    - `EXACT_2D`: Multiply the distances by 1000, round to the nearest integer.
+- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. The `EDGE_WEIGHT_FORMAT` specification must be present. We support the following two edge weight formats:
+  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.
+  - `FULL_MATRIX`: Explicit full matrix representation.
+  
+
+#### Line comments
+Lines starting with `#` are interpreted as comments and not parsed when reading the instance.
+
+#### More information about VRPLIB
+The VRPLIB format is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. 
+Additional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).
+
+### Solomon instance format
+The Solomon format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. A Solomon instance looks like this:
+``` bash
+Example
+
+VEHICLE
+NUMBER     CAPACITY
+  50          200
+
+CUSTOMER
+CUST NO.  XCOORD.    YCOORD.    DEMAND   READY TIME  DUE DATE   SERVICE TIME
+    0      70         70          0          0       1351          0
+    1      33         78         20        750        809         90
+```
+
+Reading this Solomon instance returns the following dictionary:
+``` python
+{'name': 'Example',
+ 'vehicles': 50,
+ 'capacity': 200,
+ 'node_coord': array([[70, 70], [33, 78]]),
+ 'demand': array([ 0, 20]),
+ 'time_window': array([[ 0, 1351], [ 750,  809]]),
+ 'service_time': array([ 0, 90]),
+ 'edge_weight': array([[ 0.  , 37.85498646], [37.85498646,  0.  ]])}
+```
+
+The edge weights are computed by default using the Euclidean distances. 
+
+### Solution format
+Here's an example of a solution format:
+``` { .html } 
+Route #1: 1 2 3
+Route #2: 4 5
+Cost: 100
+```
+
+A solution is represented by a set of routes, where each route specifies the sequence of customers to visit. 
+Each route should start with "Route", followed by the route number, and followed by a colon. 
+The customers to be served on the route are then listed.
+The solution file can also include other keywords like `Cost`, which will be separated on the first colon or whitespace.
+
+The convention is that customer indices start counting from 1, but `vrplib` simply parses the file without strict requirements about those indices.
+
+Reading the above example solution returns the following dictionary:
+``` python
+{'routes': [[1, 2, 3], [4, 5]], 'cost': 100}
+```
+
+### Other remarks
+- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).
+- In the literature, some instances use rounding conventions different from what is specified in the instance. For example, X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read this instance, it will return non-rounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type which implies no rounding. To adhere to the convention used in the literature, you can manually round the distances matrix.
+- For large instances (>5000 customers) it's recommended to set the `compute_edge_weights` argument to `False` in `read_instance`.
 
-packages = \
-['vrplib',
- 'vrplib.download',
- 'vrplib.parse',
- 'vrplib.parse.distances',
- 'vrplib.read']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['codecov>=2.1.13,<3.0.0', 'numpy>=1.19,<2.0']
-
-setup_kwargs = {
-    'name': 'vrplib',
-    'version': '1.1.0',
-    'description': 'Python library for working with vehicle routing problem instances.',
-    'long_description': '# VRPLIB\n[![PyPI version](https://badge.fury.io/py/vrplib.svg)](https://badge.fury.io/py/vrplib)\n[![vrplib](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml/badge.svg)](https://github.com/leonlan/vrplib/actions/workflows/vrplib.yaml)\n[![codecov](https://codecov.io/gh/leonlan/VRPLIB/branch/master/graph/badge.svg?token=X0X66LBNZ7)](https://codecov.io/gh/leonlan/VRPLIB)\n\n`vrplib` is a Python package for working with Vehicle Routing Problem (VRP) instances. The main features are:\n- reading VRPLIB and Solomon instances and solutions, and\n- downloading instances and best known solutions from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).\n\n## Installation\n`vrplib` works with Python 3.8+ and only depends on `numpy`.\n\n```shell\npip install vrplib\n```\n\n## Example usage\n### Reading instances and solutions\n```python\nimport vrplib\n\n# Read VRPLIB formatted instances (default)\ninstance = vrplib.read_instance("/path/to/X-n101-k25.vrp")\nsolution = vrplib.read_solution("/path/to/X-n101-k25.sol")\n\n# Read Solomon formatted instances\ninstance = vrplib.read_instance("/path/to/C101.txt", instance_format="solomon")\nsolution = vrplib.read_solution("/path/to/C101.sol") # only 1 solution format\n```\n\n`instance` and `solution` are dictionaries that contain all parsed data. \n``` python\n>>> instance.keys()\ndict_keys([\'name\', ..., \'edge_weight\'])\n\n>>> solution.keys()\ndict_keys([\'routes\', \'cost\'])\n```\n\n\n### Downloading instances from CVRPLIB \n``` python\nimport vrplib\n\n# Download an instance and a solution file \nvrplib.download_instance("X-n101-k25", "/path/to/instances/")\nvrplib.download_solution("X-n101-k25", "/path/to/solutions/")\n\n# List all instance names that can be downloaded \nvrplib.list_names()                      # All instance names\nvrplib.list_names(low=100, high=200)     # Instances with between [100, 200] customers\nvrplib.list_names(vrp_type="cvrp")       # Only CVRP instances\nvrplib.list_names(vrp_type="vrptw")      # Only VRPTW instances\n```\n\n\n## Documentation\n- [VRPLIB instance format](#vrplib-instance-format)\n- [Solomon instance format](#solomon-instance-format)\n- [Solution format](#solution-format)\n- [Other remarks](#other-remarks)\n\n### VRPLIB instance format\nThe VRPLIB format is the standard format for the Capacitated Vehicle Routing Problem (CVRP). An example VRPLIB instance looks as follows:\n``` bash\nNAME: Example \nEDGE_WEIGHT_TYPE: EUC_2D\nNODE_COORD_SECTION\n1 0 0\n2 5 5\nSERVICE_TIME_SECTION\n1 0\n2 3\nDEPOT_SECTION\n1\nEOF\n```\n\nA VRPLIB instance contains problem **specifications** and problem **data**. \n- Specifications are key-value pairs separated by a colon. In the example above, `NAME` and `EDGE_WEIGHT_TYPE` are the two data specifications.\n- Data are explicit array-like values such as customer coordinates or service times. \nEach data section should start with a header name that ends with `_SECTION`, e.g., `NODE_COORD_SECTION` and `SERVICE_TIME_SECTION`. It is then followed by rows of values and each row must start with an index representing the depot or customer. \nThere are two exceptions: values in `EDGE_WEIGHT_SECTION` and `DEPOT_SECTION` should not start with an index.\n\nBesides the rules outlined above, `vrplib` is not strict about the naming of specifications or sections. \nThis means that you can use `vrplib` to read VRPLIB instances with custom specifications like `MY_SPECIFICATION: SOME_VALUE` and custom section names like `MY_SECTION`.\n\nReading the above example instance returns the following dictionary:\n``` python\n{\'name\': \'Example\',\n \'edge_weight_type\': \'EUC_2D\',\n \'node_coord\': array([[0, 0], [5, 5]]),\n \'service_time\': array([1, 3]),\n \'depot\': array([0]),\n \'edge_weight\': array([[0.  , 7.07106781], [7.07106781, 0.  ]])}\n```\n\nThe depot section specifies which location index corresponds to the depot data. \nThe convention is to let index 1 represent the depot. \n`vrplib` subtracts one from the depot value to make it easier to index.\n\n#### Computing edge weights \nNote that the example instance did not include any explicit information about the edge weights, yet the output includes edge weights data.\nThis is because `vrplib` automatically computes the edge weights based on the instance specifications, if applicable.\nIn the example, the edge weight type specification and node coordinates data are used to compute the Euclidean distance.\nYou can set the `compute_distances` argument in `read_instance` to disable this feature.\n\nFollowing the VRPLIB conventions, the edge weights are computed based on the `EDGE_WEIGHT_TYPE` specification, and in some cases the `EDGE_WEIGHT_FORMAT` specification. `vrplib` currently supports two categories of edge weight types:\n- `*_2D`: Euclidean distances based on the node coordinates data.\n    - `EUC_2D`: Double precision distances without rounding.\n    - `FLOOR_2D`: Round down all distances to down to an integer.\n    - `EXACT_2D`: Multiply the distances by 1000, round to the nearest integer.\n- `EXPLICIT`: the distance data is explicitly provided, in partial or full form. The `EDGE_WEIGHT_FORMAT` specification must be present. We support the following two edge weight formats:\n  - `LOWER_ROW`: Lower row triangular matrix without diagonal entries.\n  - `FULL_MATRIX`: Explicit full matrix representation.\n  \n\n#### More information about VRPLIB\nThe VRPLIB format is an extension of the [TSPLIB95](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/tsp95.pdf) format. \nAdditional information about the VRPLIB format can be found [here]( http://webhotel4.ruc.dk/~keld/research/LKH-3/LKH-3_REPORT.pdf).\n\n### Solomon instance format\nThe Solomon format was used to introduce the Solomon instances for the Vehicle Routing Problem with Time Window (VRPTW) and also the extended instance set by Homberger and Gehring. A Solomon instance looks like this:\n``` bash\nExample\n\nVEHICLE\nNUMBER     CAPACITY\n  50          200\n\nCUSTOMER\nCUST NO.  XCOORD.    YCOORD.    DEMAND   READY TIME  DUE DATE   SERVICE TIME\n    0      70         70          0          0       1351          0\n    1      33         78         20        750        809         90\n```\n\nReading this Solomon instance returns the following dictionary:\n``` python\n{\'name\': \'Example\',\n \'vehicles\': 50,\n \'capacity\': 200,\n \'node_coord\': array([[70, 70], [33, 78]]),\n \'demand\': array([ 0, 20]),\n \'time_window\': array([[ 0, 1351], [ 750,  809]]),\n \'service_time\': array([ 0, 90]),\n \'edge_weight\': array([[ 0.  , 37.85498646], [37.85498646,  0.  ]])}\n```\n\nThe edge weights are computed by default using the Euclidean distances. \n\n### Solution format\nHere\'s an example of a solution format:\n``` { .html } \nRoute #1: 1 2 3\nRoute #2: 4 5\nCost: 100\n```\n\nA solution is represented by a set of routes, where each route specifies the sequence of customers to visit. \nEach route should start with "Route", followed by the route number, and followed by a colon. \nThe customers to be served on the route are then listed.\nThe solution file can also include other keywords like `Cost`, which will be separated on the first colon or whitespace.\n\nThe convention is that customer indices start counting from 1, but `vrplib` simply parses the file without strict requirements about those indices.\n\nReading the above example solution returns the following dictionary:\n``` python\n{\'routes\': [[1, 2, 3], [4, 5]], \'cost\': 100}\n```\n\n### Other remarks\n- The `XML100` benchmark set is not listed in `list_names` and cannot be downloaded through this package. You can download these instances directly from [CVRPLIB](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/).\n- In the literature, some instances use rounding conventions different from what is specified in the instance. For example, X instance set proposed by [Uchoa et al. (2017)](http://vrp.atd-lab.inf.puc-rio.br/index.php/en/new-instances) assumes that the distances are rounded to the nearest integer. When you use the `vrplib` package to read this instance, it will return non-rounded Euclidean distances because the instance specifies the `EUC_2D` edge weight type which implies no rounding. To adhere to the convention used in the literature, you can manually round the distances matrix.\n- For large instances (>5000 customers) it\'s recommended to set the `compute_edge_weights` argument to `False` in `read_instance`.\n',
-    'author': 'Leon Lan',
-    'author_email': 'leon.lanyidong@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/leonlan/VRPLIB',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

