# Comparing `tmp/cai_causal_graph-0.1.0.dev0.tar.gz` & `tmp/cai_causal_graph-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cai_causal_graph-0.1.0.dev0.tar", max compression
+gzip compressed data, was "cai_causal_graph-0.1.0.dev1.tar", max compression
```

## Comparing `cai_causal_graph-0.1.0.dev0.tar` & `cai_causal_graph-0.1.0.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-07-28 09:23:56.871846 cai_causal_graph-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0      733 2023-07-28 09:23:56.871846 cai_causal_graph-0.1.0.dev0/README.md
--rw-r--r--   0        0        0      861 2023-07-28 09:24:08.088122 cai_causal_graph-0.1.0.dev0/cai_causal_graph/__init__.py
--rw-r--r--   0        0        0    83490 2023-07-28 09:23:56.871846 cai_causal_graph-0.1.0.dev0/cai_causal_graph/causal_graph.py
--rw-r--r--   0        0        0     2599 2023-07-28 09:23:56.875846 cai_causal_graph-0.1.0.dev0/cai_causal_graph/exceptions.py
--rw-r--r--   0        0        0    11867 2023-07-28 09:23:56.875846 cai_causal_graph-0.1.0.dev0/cai_causal_graph/graph_components.py
--rw-r--r--   0        0        0     1865 2023-07-28 09:23:56.875846 cai_causal_graph-0.1.0.dev0/cai_causal_graph/interfaces.py
--rw-r--r--   0        0        0     3732 2023-07-28 09:23:56.875846 cai_causal_graph-0.1.0.dev0/cai_causal_graph/type_definitions.py
--rw-r--r--   0        0        0     1790 2023-07-28 09:24:08.040121 cai_causal_graph-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 cai_causal_graph-0.1.0.dev0/setup.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 cai_causal_graph-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0      985 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0      861 2023-07-28 13:25:47.048636 cai_causal_graph-0.1.0.dev1/cai_causal_graph/__init__.py
+-rw-r--r--   0        0        0    83490 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/cai_causal_graph/causal_graph.py
+-rw-r--r--   0        0        0     2599 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/cai_causal_graph/exceptions.py
+-rw-r--r--   0        0        0    11867 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/cai_causal_graph/graph_components.py
+-rw-r--r--   0        0        0     1865 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/cai_causal_graph/interfaces.py
+-rw-r--r--   0        0        0     3732 2023-07-28 13:25:28.076295 cai_causal_graph-0.1.0.dev1/cai_causal_graph/type_definitions.py
+-rw-r--r--   0        0        0     1805 2023-07-28 13:25:47.044635 cai_causal_graph-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 cai_causal_graph-0.1.0.dev1/setup.py
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 cai_causal_graph-0.1.0.dev1/PKG-INFO
```

### Comparing `cai_causal_graph-0.1.0.dev0/LICENSE` & `cai_causal_graph-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/README.md` & `cai_causal_graph-0.1.0.dev1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-# cai-causal-graph: A package for causal graphs
+# cai-causal-graph
 
-Link to docs site coming imminently.
+![causaLens logo](cl-logo.png)
+
+## From causaLens, a Causal AI package for causal graphs
+Documentation, including a quickstart and code reference docs, can be found [here](https://causalgraph.causalens.com/).
+
+[![PyPI version](https://badge.fury.io/py/cai-causal-graph.svg)](https://badge.fury.io/py/cai-causal-graph)
+[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ![TEST](https://github.com/causalens/cai-causal-graph/workflows/MAIN-CHECKS/badge.svg?branch=main)
 ![DEPENDENCIES](https://github.com/causalens/cai-causal-graph/workflows/DEPENDENCIES-CHECKS/badge.svg?branch=main) 
 ![RELEASE](https://github.com/causalens/cai-causal-graph/workflows/RELEASE/badge.svg) 
 ![POST-RELEASE](https://github.com/causalens/cai-causal-graph/workflows/POST-RELEASE/badge.svg?branch=main) 
 ![INTERROGATE](./docs/interrogate_badge.svg)
-[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 > **Note**  
 > The current development cycle of this branch is `v0.0.x`.
```

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/__init__.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,11 +19,11 @@
     'CausalGraph',
     'Skeleton',
     # Causal types
     'EDGE_T',
     'NODE_T',
 ]
 
-__version__ = '0.1.0.dev0'
+__version__ = '0.1.0.dev1'
 
 from cai_causal_graph.causal_graph import CausalGraph, Skeleton
 from cai_causal_graph.type_definitions import EDGE_T, NODE_T
```

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/causal_graph.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/causal_graph.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/exceptions.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/graph_components.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/graph_components.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/interfaces.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/interfaces.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/cai_causal_graph/type_definitions.py` & `cai_causal_graph-0.1.0.dev1/cai_causal_graph/type_definitions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.1.0.dev0/pyproject.toml` & `cai_causal_graph-0.1.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 check_untyped_defs = true
 ignore_missing_imports = true
 pretty = true
 cache_dir = '/dev/null'
 
 [tool.poetry]
 name = "cai-causal-graph"
-version = "0.1.0.dev0"
-description = "A causal graph package."
+version = "0.1.0.dev1"
+description = "A Causal AI package for causal graphs."
 license = "Apache-2.0"
 authors = ["causaLens <opensource@causalens.com>"]
 readme = "README.md"
 homepage = "https://causalgraph.causalens.com/"
 repository = "https://github.com/causalens/cai-causal-graph"
 documentation = "https://causalgraph.causalens.com/"
 packages = [{include = "cai_causal_graph"}]
```

### Comparing `cai_causal_graph-0.1.0.dev0/setup.py` & `cai_causal_graph-0.1.0.dev1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['networkx>=3.0.0,<4.0.0', 'numpy>=1.18.0,<2.0.0', 'pandas>=1.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'cai-causal-graph',
-    'version': '0.1.0.dev0',
-    'description': 'A causal graph package.',
-    'long_description': '# cai-causal-graph: A package for causal graphs\n\nLink to docs site coming imminently.\n\n![TEST](https://github.com/causalens/cai-causal-graph/workflows/MAIN-CHECKS/badge.svg?branch=main)\n![DEPENDENCIES](https://github.com/causalens/cai-causal-graph/workflows/DEPENDENCIES-CHECKS/badge.svg?branch=main) \n![RELEASE](https://github.com/causalens/cai-causal-graph/workflows/RELEASE/badge.svg) \n![POST-RELEASE](https://github.com/causalens/cai-causal-graph/workflows/POST-RELEASE/badge.svg?branch=main) \n![INTERROGATE](./docs/interrogate_badge.svg)\n[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\n> **Note**  \n> The current development cycle of this branch is `v0.0.x`.\n',
+    'version': '0.1.0.dev1',
+    'description': 'A Causal AI package for causal graphs.',
+    'long_description': '# cai-causal-graph\n\n![causaLens logo](cl-logo.png)\n\n## From causaLens, a Causal AI package for causal graphs\nDocumentation, including a quickstart and code reference docs, can be found [here](https://causalgraph.causalens.com/).\n\n[![PyPI version](https://badge.fury.io/py/cai-causal-graph.svg)](https://badge.fury.io/py/cai-causal-graph)\n[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\n![TEST](https://github.com/causalens/cai-causal-graph/workflows/MAIN-CHECKS/badge.svg?branch=main)\n![DEPENDENCIES](https://github.com/causalens/cai-causal-graph/workflows/DEPENDENCIES-CHECKS/badge.svg?branch=main) \n![RELEASE](https://github.com/causalens/cai-causal-graph/workflows/RELEASE/badge.svg) \n![POST-RELEASE](https://github.com/causalens/cai-causal-graph/workflows/POST-RELEASE/badge.svg?branch=main) \n![INTERROGATE](./docs/interrogate_badge.svg)\n\n> **Note**  \n> The current development cycle of this branch is `v0.0.x`.\n',
     'author': 'causaLens',
     'author_email': 'opensource@causalens.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://causalgraph.causalens.com/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cai_causal_graph-0.1.0.dev0/PKG-INFO` & `cai_causal_graph-0.1.0.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cai-causal-graph
-Version: 0.1.0.dev0
-Summary: A causal graph package.
+Version: 0.1.0.dev1
+Summary: A Causal AI package for causal graphs.
 Home-page: https://causalgraph.causalens.com/
 License: Apache-2.0
 Author: causaLens
 Author-email: opensource@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,21 +16,26 @@
 Requires-Dist: networkx (>=3.0.0,<4.0.0)
 Requires-Dist: numpy (>=1.18.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.0,<3.0.0)
 Project-URL: Documentation, https://causalgraph.causalens.com/
 Project-URL: Repository, https://github.com/causalens/cai-causal-graph
 Description-Content-Type: text/markdown
 
-# cai-causal-graph: A package for causal graphs
+# cai-causal-graph
 
-Link to docs site coming imminently.
+![causaLens logo](cl-logo.png)
+
+## From causaLens, a Causal AI package for causal graphs
+Documentation, including a quickstart and code reference docs, can be found [here](https://causalgraph.causalens.com/).
+
+[![PyPI version](https://badge.fury.io/py/cai-causal-graph.svg)](https://badge.fury.io/py/cai-causal-graph)
+[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ![TEST](https://github.com/causalens/cai-causal-graph/workflows/MAIN-CHECKS/badge.svg?branch=main)
 ![DEPENDENCIES](https://github.com/causalens/cai-causal-graph/workflows/DEPENDENCIES-CHECKS/badge.svg?branch=main) 
 ![RELEASE](https://github.com/causalens/cai-causal-graph/workflows/RELEASE/badge.svg) 
 ![POST-RELEASE](https://github.com/causalens/cai-causal-graph/workflows/POST-RELEASE/badge.svg?branch=main) 
 ![INTERROGATE](./docs/interrogate_badge.svg)
-[![LICENSE](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 > **Note**  
 > The current development cycle of this branch is `v0.0.x`.
```

