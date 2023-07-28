# Comparing `tmp/statspack-0.1.0.tar.gz` & `tmp/statspack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statspack-0.1.0.tar", last modified: Thu Jul 27 10:35:08 2023, max compression
+gzip compressed data, was "statspack-0.1.2.tar", last modified: Fri Jul 28 11:43:52 2023, max compression
```

## Comparing `statspack-0.1.0.tar` & `statspack-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-27 10:35:08.613931 statspack-0.1.0/
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     3078 2023-07-25 10:47:13.000000 statspack-0.1.0/.gitignore
--rw-rw-r--   0 herpich   (1000) herpich   (1000)    35149 2023-07-25 10:47:13.000000 statspack-0.1.0/LICENSE
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     3359 2023-07-27 10:35:08.613931 statspack-0.1.0/PKG-INFO
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     2544 2023-07-26 15:42:09.000000 statspack-0.1.0/README.md
--rw-r--r--   0 herpich   (1000) herpich   (1000)      548 2023-07-26 16:22:58.000000 statspack-0.1.0/__init__.py
--rw-r--r--   0 herpich   (1000) herpich   (1000)     3918 2023-07-26 15:54:22.000000 statspack-0.1.0/binning.py
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     3628 2023-07-26 16:09:42.000000 statspack-0.1.0/contour_pdf.py
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     3340 2023-07-26 16:07:58.000000 statspack-0.1.0/density_contour.py
--rw-r--r--   0 herpich   (1000) herpich   (1000)     1607 2023-07-26 15:57:00.000000 statspack-0.1.0/find_confidence_interval.py
--rw-rw-r--   0 herpich   (1000) herpich   (1000)      546 2023-07-27 10:16:13.000000 statspack-0.1.0/pyproject.toml
--rw-rw-r--   0 herpich   (1000) herpich   (1000)       38 2023-07-27 10:35:08.613931 statspack-0.1.0/setup.cfg
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     1094 2023-07-27 10:16:00.000000 statspack-0.1.0/setup.py
-drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-27 10:35:08.613931 statspack-0.1.0/statspack.egg-info/
--rw-rw-r--   0 herpich   (1000) herpich   (1000)     3359 2023-07-27 10:35:08.000000 statspack-0.1.0/statspack.egg-info/PKG-INFO
--rw-rw-r--   0 herpich   (1000) herpich   (1000)      301 2023-07-27 10:35:08.000000 statspack-0.1.0/statspack.egg-info/SOURCES.txt
--rw-rw-r--   0 herpich   (1000) herpich   (1000)        1 2023-07-27 10:35:08.000000 statspack-0.1.0/statspack.egg-info/dependency_links.txt
--rw-rw-r--   0 herpich   (1000) herpich   (1000)       32 2023-07-27 10:35:08.000000 statspack-0.1.0/statspack.egg-info/requires.txt
--rw-rw-r--   0 herpich   (1000) herpich   (1000)        1 2023-07-27 10:35:08.000000 statspack-0.1.0/statspack.egg-info/top_level.txt
+drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-28 11:43:52.242207 statspack-0.1.2/
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)     3078 2023-07-25 10:47:13.000000 statspack-0.1.2/.gitignore
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)    35149 2023-07-25 10:47:13.000000 statspack-0.1.2/LICENSE
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)     3291 2023-07-28 11:43:52.242207 statspack-0.1.2/PKG-INFO
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)     2544 2023-07-26 15:42:09.000000 statspack-0.1.2/README.md
+drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-28 11:43:52.242207 statspack-0.1.2/bin/
+-rwxr--r--   0 herpich   (1000) herpich   (1000)      571 2023-07-28 07:51:28.000000 statspack-0.1.2/bin/__init__.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3922 2023-07-28 07:50:17.000000 statspack-0.1.2/bin/binning.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3632 2023-07-28 07:50:32.000000 statspack-0.1.2/bin/contour_pdf.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3344 2023-07-28 07:50:45.000000 statspack-0.1.2/bin/density_contour.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     1611 2023-07-28 07:51:05.000000 statspack-0.1.2/bin/find_confidence_interval.py
+-rw-r--r--   0 herpich   (1000) herpich   (1000)      885 2023-07-28 11:43:08.000000 statspack-0.1.2/pyproject.toml
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)       38 2023-07-28 11:43:52.242207 statspack-0.1.2/setup.cfg
+-rw-r--r--   0 herpich   (1000) herpich   (1000)     1076 2023-07-28 11:29:39.000000 statspack-0.1.2/setup.py
+drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-28 11:43:52.242207 statspack-0.1.2/statspack/
+-rwxr--r--   0 herpich   (1000) herpich   (1000)      626 2023-07-28 11:34:27.000000 statspack-0.1.2/statspack/__init__.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3922 2023-07-28 11:24:40.000000 statspack-0.1.2/statspack/binning.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3632 2023-07-28 11:24:40.000000 statspack-0.1.2/statspack/contour_pdf.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     3344 2023-07-28 11:24:40.000000 statspack-0.1.2/statspack/density_contour.py
+-rwxr--r--   0 herpich   (1000) herpich   (1000)     1611 2023-07-28 11:24:40.000000 statspack-0.1.2/statspack/find_confidence_interval.py
+drwxrwxr-x   0 herpich   (1000) herpich   (1000)        0 2023-07-28 11:43:52.242207 statspack-0.1.2/statspack.egg-info/
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)     3291 2023-07-28 11:43:52.000000 statspack-0.1.2/statspack.egg-info/PKG-INFO
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)      456 2023-07-28 11:43:52.000000 statspack-0.1.2/statspack.egg-info/SOURCES.txt
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)        1 2023-07-28 11:43:52.000000 statspack-0.1.2/statspack.egg-info/dependency_links.txt
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)       49 2023-07-28 11:43:52.000000 statspack-0.1.2/statspack.egg-info/requires.txt
+-rw-rw-r--   0 herpich   (1000) herpich   (1000)       10 2023-07-28 11:43:52.000000 statspack-0.1.2/statspack.egg-info/top_level.txt
```

### Comparing `statspack-0.1.0/.gitignore` & `statspack-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `statspack-0.1.0/LICENSE` & `statspack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statspack-0.1.0/PKG-INFO` & `statspack-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: statspack
-Version: 0.1.0
+Version: 0.1.2
 Summary: A statistical visualization package optimized to work with percentiles and histograms.
 Home-page: https://github.com/herpichfr/statspack
 Author: Fabio R Herpich
 Author-email: fabio.herpich@ast.cam.ac.uk
 License: GNU GENERAL PUBLIC LICENSE Version 3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -124,9 +122,7 @@
 ```
 
 These are some of the functions provided by the StatsPack package for statistical visualization. You can refer to the function documentation in the source code for more details on their parameters and usage.
 
 ## License
 
 StatsPack is licensed under the [GNU General Public License v3.0](LICENSE). You can find the full text of the license in the `LICENSE` file included with the package.
-
-
```

### Comparing `statspack-0.1.0/README.md` & `statspack-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `statspack-0.1.0/__init__.py` & `statspack-0.1.2/bin/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 # statspack/__init__.py
 
 # Import sub-modules or functions
 from .binning import binning
 from .find_confidence_interval import find_confidence_interval
 from .density_contour import density_contour
 from .contour_pdf import contour_pdf
```

### Comparing `statspack-0.1.0/binning.py` & `statspack-0.1.2/bin/binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/env python3
+#!/usr/bin/env python3
 # package with modules for statistic visualization
 # Fabio R. Herpich 2023-07-26 CASU/IoA Cambridge
 # All rights reserved (see LICENSE file)
 
 import numpy as np
 from datetime import datetime
 import logging
```

### Comparing `statspack-0.1.0/contour_pdf.py` & `statspack-0.1.2/bin/contour_pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/env python3
+#!/usr/bin/env python3
 # package with modules for statistic visualization
 # Fabio R. Herpich 2023-07-26 CASU/IoA Cambridge
 # All rights reserved (see LICENSE file)
 
 import numpy as np
 import scipy.stats
 from datetime import datetime
```

### Comparing `statspack-0.1.0/density_contour.py` & `statspack-0.1.2/bin/density_contour.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/env python3
+#!/usr/bin/env python3
 # package with modules for statistic visualization
 # Fabio R. Herpich 2023-07-26 CASU/IoA Cambridge
 # All rights reserved (see LICENSE file)
 
 import numpy as np
 import logging
 import colorlog
```

### Comparing `statspack-0.1.0/find_confidence_interval.py` & `statspack-0.1.2/bin/find_confidence_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/env python3
+#!/usr/bin/env python3
 # package with modules for statistic visualization
 # Fabio R. Herpich 2023-07-26 CASU/IoA Cambridge
 # All rights reserved (see LICENSE file)
 
 import numpy as np
 from datetime import datetime
 import logging
```

### Comparing `statspack-0.1.0/setup.py` & `statspack-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-from setuptools import setup, find_packages
-from setuptools_scm import get_version
+[build-system]
+requires = [
+"setuptools>=42",
+"wheel"
+]
+
+[tool.poetry]
+name = "statspack"
+version = "0.1.2"
+description = "A statistical visualization package optimized to work with percentiles and histograms."
+authors = ["Fabio R. Herpich <fabio.herpich@ast.cam.ac.uk>"]
+license = "GPL-3.0-only"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+numpy = "^1.0"
+scipy = "^1.0"
+matplotlib = "^3.0"
+colorlog = "^5.0"
+
+[tool.poetry.dev-dependencies]
+
+[tool.poetry.scripts]
+
+[tool.poetry.extras]
+
+[tool.poetry.build]
 
-setup(
-    name='statspack',
-    version='0.1.0',
-    packages=find_packages(),
-    install_requires=[
-        'numpy',
-        'scipy',
-        'matplotlib',
-        'colorlog',
-    ],
-    author='Fabio R Herpich',
-    author_email='fabio.herpich@ast.cam.ac.uk',
-    description='A statistical visualization package optimized to work with percentiles and histograms.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/herpichfr/statspack',
-    license='GNU GENERAL PUBLIC LICENSE Version 3',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-)
```

### Comparing `statspack-0.1.0/statspack.egg-info/PKG-INFO` & `statspack-0.1.2/statspack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: statspack
-Version: 0.1.0
+Version: 0.1.2
 Summary: A statistical visualization package optimized to work with percentiles and histograms.
 Home-page: https://github.com/herpichfr/statspack
 Author: Fabio R Herpich
 Author-email: fabio.herpich@ast.cam.ac.uk
 License: GNU GENERAL PUBLIC LICENSE Version 3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -124,9 +122,7 @@
 ```
 
 These are some of the functions provided by the StatsPack package for statistical visualization. You can refer to the function documentation in the source code for more details on their parameters and usage.
 
 ## License
 
 StatsPack is licensed under the [GNU General Public License v3.0](LICENSE). You can find the full text of the license in the `LICENSE` file included with the package.
-
-
```

