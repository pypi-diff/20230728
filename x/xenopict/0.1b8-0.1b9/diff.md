# Comparing `tmp/xenopict-0.1b8.tar.gz` & `tmp/xenopict-0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenopict-0.1b8.tar", last modified: Mon Oct 24 19:27:12 2022, max compression
+gzip compressed data, was "xenopict-0.1b9.tar", last modified: Wed Nov 30 23:15:14 2022, max compression
```

## Comparing `xenopict-0.1b8.tar` & `xenopict-0.1b9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:27:12.851495 xenopict-0.1b8/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-10-24 19:27:12.000000 xenopict-0.1b8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1993 2022-10-24 19:27:12.851495 xenopict-0.1b8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      724 2022-10-24 19:27:12.000000 xenopict-0.1b8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-24 19:27:12.851495 xenopict-0.1b8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2367 2022-10-24 19:27:12.000000 xenopict-0.1b8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:27:12.851495 xenopict-0.1b8/xenopict/
--rw-r--r--   0 root         (0) root         (0)       75 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/__init__.py
--rw-r--r--   0 root         (0) root         (0)       61 2022-10-24 19:27:12.851495 xenopict-0.1b8/xenopict/_static_version.py
--rw-r--r--   0 root         (0) root         (0)     5773 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/_version.py
--rw-r--r--   0 root         (0) root         (0)    10346 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/colormap.py
--rw-r--r--   0 root         (0) root         (0)    26669 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/drawer.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/magic.py
--rw-r--r--   0 root         (0) root         (0)     5466 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/monkey.py
--rw-r--r--   0 root         (0) root         (0)     1759 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict/plotdot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:27:12.851495 xenopict-0.1b8/xenopict.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1993 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-10-24 19:27:12.000000 xenopict-0.1b8/xenopict.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 23:15:14.073924 xenopict-0.1b9/
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-11-30 23:15:13.000000 xenopict-0.1b9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1993 2022-11-30 23:15:14.073924 xenopict-0.1b9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2022-11-30 23:15:13.000000 xenopict-0.1b9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-30 23:15:14.073924 xenopict-0.1b9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2367 2022-11-30 23:15:13.000000 xenopict-0.1b9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 23:15:14.073924 xenopict-0.1b9/xenopict/
+-rw-r--r--   0 root         (0) root         (0)       75 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       61 2022-11-30 23:15:14.073924 xenopict-0.1b9/xenopict/_static_version.py
+-rw-r--r--   0 root         (0) root         (0)     5773 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/_version.py
+-rw-r--r--   0 root         (0) root         (0)    10346 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/colormap.py
+-rw-r--r--   0 root         (0) root         (0)    26992 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/drawer.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/magic.py
+-rw-r--r--   0 root         (0) root         (0)     5466 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/monkey.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2022-11-30 23:15:13.000000 xenopict-0.1b9/xenopict/plotdot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-30 23:15:14.073924 xenopict-0.1b9/xenopict.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1993 2022-11-30 23:15:14.000000 xenopict-0.1b9/xenopict.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      352 2022-11-30 23:15:14.000000 xenopict-0.1b9/xenopict.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-30 23:15:14.000000 xenopict-0.1b9/xenopict.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2022-11-30 23:15:14.000000 xenopict-0.1b9/xenopict.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-30 23:15:14.000000 xenopict-0.1b9/xenopict.egg-info/top_level.txt
```

### Comparing `xenopict-0.1b8/LICENSE` & `xenopict-0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/PKG-INFO` & `xenopict-0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenopict
-Version: 0.1b8
+Version: 0.1b9
 Summary: Library for publication quality depictions of small molecules.
 Home-page: https://github.com/swamidasslab/xenopict/
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xenopict-0.1b8/README.md` & `xenopict-0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/setup.py` & `xenopict-0.1b9/setup.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict/_version.py` & `xenopict-0.1b9/xenopict/_version.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict/colormap.py` & `xenopict-0.1b9/xenopict/colormap.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict/drawer.py` & `xenopict-0.1b9/xenopict/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 
 from urllib.parse import quote
 from collections import defaultdict
 from typing import Optional, Union
 import simplejson as json
 import hashlib
 import re
+import os
 
 from warnings import warn
 
 with contextlib.suppress(ImportError):
     from matplotlib.colors import Colormap
 
 from shapely.geometry import LineString, Point
 
 install_colormaps()
 
 __all__ = ["shaded_svg", "Xenopict"]
 
+_DEBUG = os.environ.get("XENOPICT_DEBUG", False)
+
+if _DEBUG:
+    from icecream import ic
+else:
+    ic = lambda x: x
+
 
 AtomIdx = int
 BondShading = tuple[Sequence[AtomIdx], Sequence[AtomIdx], Sequence[float]]
 AtomShading = Sequence[float]
 SVG = str
 
 
@@ -207,14 +215,19 @@
 
                     with contextlib.suppress(Exception):
                         del s["stroke-linecap"]
                         del s["stroke-linejoin"]
                         if s["fill"] == "none":
                             del s["fill"]
 
+                    if "stroke-dasharray" in s:
+                        c.setAttribute(
+                            "style", f"stroke-dasharray:{s['stroke-dasharray']}"
+                        )
+
                     self.groups["lines"].setAttribute("style", _dict2style(s))
                     self.groups["lines"].firstChild.appendChild(c)  # type: ignore
                 else:
                     self.groups["text"].firstChild.appendChild(c)  # type: ignore
             elif not c.TEXT_NODE:
                 self.groups["text"].appendChild(c)
```

### Comparing `xenopict-0.1b8/xenopict/magic.py` & `xenopict-0.1b9/xenopict/magic.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict/monkey.py` & `xenopict-0.1b9/xenopict/monkey.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict/plotdot.py` & `xenopict-0.1b9/xenopict/plotdot.py`

 * *Files identical despite different names*

### Comparing `xenopict-0.1b8/xenopict.egg-info/PKG-INFO` & `xenopict-0.1b9/xenopict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenopict
-Version: 0.1b8
+Version: 0.1b9
 Summary: Library for publication quality depictions of small molecules.
 Home-page: https://github.com/swamidasslab/xenopict/
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

