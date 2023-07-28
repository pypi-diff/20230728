# Comparing `tmp/paramspace-2.6.1.tar.gz` & `tmp/paramspace-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramspace-2.6.1.tar", last modified: Sun Jul 23 15:06:25 2023, max compression
+gzip compressed data, was "paramspace-2.6.2.tar", last modified: Fri Jul 28 15:19:34 2023, max compression
```

## Comparing `paramspace-2.6.1.tar` & `paramspace-2.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 15:06:25.333122 paramspace-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     9537 2023-07-23 15:06:15.000000 paramspace-2.6.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-07-23 15:06:15.000000 paramspace-2.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-23 15:06:25.333122 paramspace-2.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11599 2023-07-23 15:06:15.000000 paramspace-2.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 15:06:25.331122 paramspace-2.6.1/paramspace/
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38054 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/paramdim.py
--rw-rw-rw-   0 root         (0) root         (0)    59852 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/paramspace.py
--rw-rw-rw-   0 root         (0) root         (0)    17865 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/yaml.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/yaml_constructors.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-23 15:06:15.000000 paramspace-2.6.1/paramspace/yaml_representers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 15:06:25.333122 paramspace-2.6.1/paramspace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3290 2023-07-23 15:06:25.000000 paramspace-2.6.1/paramspace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      397 2023-07-23 15:06:25.000000 paramspace-2.6.1/paramspace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 15:06:25.000000 paramspace-2.6.1/paramspace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-23 15:06:25.000000 paramspace-2.6.1/paramspace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-23 15:06:25.000000 paramspace-2.6.1/paramspace.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-23 15:06:15.000000 paramspace-2.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 15:06:25.333122 paramspace-2.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-07-23 15:06:15.000000 paramspace-2.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:19:34.114640 paramspace-2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     9596 2023-07-28 15:19:23.000000 paramspace-2.6.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-07-28 15:19:23.000000 paramspace-2.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-07-28 15:19:34.113640 paramspace-2.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11599 2023-07-28 15:19:23.000000 paramspace-2.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:19:34.112640 paramspace-2.6.2/paramspace/
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38054 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/paramdim.py
+-rw-rw-rw-   0 root         (0) root         (0)    59852 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/paramspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    17865 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/yaml_constructors.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-28 15:19:23.000000 paramspace-2.6.2/paramspace/yaml_representers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:19:34.113640 paramspace-2.6.2/paramspace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-07-28 15:19:34.000000 paramspace-2.6.2/paramspace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-28 15:19:34.000000 paramspace-2.6.2/paramspace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 15:19:34.000000 paramspace-2.6.2/paramspace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-28 15:19:34.000000 paramspace-2.6.2/paramspace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 15:19:34.000000 paramspace-2.6.2/paramspace.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-28 15:19:23.000000 paramspace-2.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 15:19:34.114640 paramspace-2.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-07-28 15:19:23.000000 paramspace-2.6.2/setup.py
```

### Comparing `paramspace-2.6.1/CHANGELOG.md` & `paramspace-2.6.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 `paramspace` aims to adhere to [semantic versioning](https://semver.org/).
 
+## v2.6.2
+- !79 removes left-over `print` statements 🤦
+
 ## v2.6.1
 Post-release of v2.6.0 due to botched PyPI deployment.
 
 ## v2.6.0
 This is a maintenance release, adding the following (mostly internal) improvements:
 
 - The repository now uses `main` as its default branch.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `paramspace-2.6.1/LICENSE` & `paramspace-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/PKG-INFO` & `paramspace-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramspace
-Version: 2.6.1
+Version: 2.6.2
 Summary: Dictionary-based, multi-dimensional parameter space iteration
 Home-page: https://gitlab.com/blsqr/paramspace
 Author: Yunus Sevinchan
 Author-email: yunussevinchan@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `paramspace-2.6.1/README.md` & `paramspace-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/paramspace/__init__.py` & `paramspace-2.6.2/paramspace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 dimensions, i.e. the *parameter space*.
 
 Furthermore, the :py:mod:`paramspace.yaml` module provides possibilities to
 define the parameter space fully from YAML configuration files, using custom
 YAML tags.
 """
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 
 from .paramdim import CoupledParamDim, ParamDim
 from .paramspace import ParamSpace
 from .yaml import yaml, yaml_safe, yaml_unsafe
```

### Comparing `paramspace-2.6.1/paramspace/paramdim.py` & `paramspace-2.6.2/paramspace/paramdim.py`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/paramspace/paramspace.py` & `paramspace-2.6.2/paramspace/paramspace.py`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/paramspace/tools.py` & `paramspace-2.6.2/paramspace/tools.py`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/paramspace/yaml.py` & `paramspace-2.6.2/paramspace/yaml.py`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/paramspace/yaml_constructors.py` & `paramspace-2.6.2/paramspace/yaml_constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     return _pspace_constructor(loader, node, sort_if_mapping=False)
 
 
 @yay.is_constructor("!pdim")
 def pdim(loader, node) -> ParamDim:
     """constructor for creating a ParamDim object from a mapping, but only
     return the default value."""
-    print("!pdim constructor")
     return _pdim_constructor(loader, node, Cls=ParamDim, default_order=np.inf)
 
 
 @yay.is_constructor("!coupled-pdim")
 def coupled_pdim(loader, node) -> ParamDim:
     """constructor for creating a ParamDim object from a mapping, but only
     return the default value."""
@@ -125,17 +124,15 @@
         # This is IMPORTANT because otherwise loading dumps from <2.6 will
         # yield different state numbers and thus different iteration order.
         if default_order is not None:
             if "order" not in kwargs or kwargs.get("order") is None:
                 kwargs["order"] = default_order
 
         # Can now construct the object:
-        print(kwargs)
         pdim = Cls(**kwargs)
-        print("order:", pdim.order)
 
     else:
         raise TypeError(
             f"{Cls} can only be constructed from a mapping node, got node "
             f"of type {type(node)} with value:\n{node}"
         )
```

### Comparing `paramspace-2.6.1/paramspace.egg-info/PKG-INFO` & `paramspace-2.6.2/paramspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramspace
-Version: 2.6.1
+Version: 2.6.2
 Summary: Dictionary-based, multi-dimensional parameter space iteration
 Home-page: https://gitlab.com/blsqr/paramspace
 Author: Yunus Sevinchan
 Author-email: yunussevinchan@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `paramspace-2.6.1/pyproject.toml` & `paramspace-2.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paramspace-2.6.1/setup.py` & `paramspace-2.6.2/setup.py`

 * *Files identical despite different names*

