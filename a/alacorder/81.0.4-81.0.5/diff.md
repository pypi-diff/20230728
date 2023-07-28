# Comparing `tmp/alacorder-81.0.4.tar.gz` & `tmp/alacorder-81.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.0.4.tar", max compression
+gzip compressed data, was "alacorder-81.0.5.tar", max compression
```

## Comparing `alacorder-81.0.4.tar` & `alacorder-81.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.0.4/LICENSE
--rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.0.4/README.md
--rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.0.4/alacorder/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.0.4/alacorder/__main__.py
--rw-r--r--   0        0        0   227486 2023-07-28 17:26:58.159845 alacorder-81.0.4/alacorder/alac.py
--rw-r--r--   0        0        0      557 2023-07-28 17:27:05.811720 alacorder-81.0.4/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.0.5/LICENSE
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.0.5/README.md
+-rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.0.5/alacorder/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.0.5/alacorder/__main__.py
+-rw-r--r--   0        0        0   227454 2023-07-28 17:35:01.113282 alacorder-81.0.5/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-07-28 17:35:05.208062 alacorder-81.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.0.5/PKG-INFO
```

### Comparing `alacorder-81.0.4/LICENSE` & `alacorder-81.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-81.0.4/README.md` & `alacorder-81.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.0.4/alacorder/alac.py` & `alacorder-81.0.5/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
 ┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
 (c) 2023 Sam Robson
 
 Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
 """
 
-__version__ = "81.0.4"
+__version__ = "81.0.5"
 
 import os
 import re
 import glob
 import time
 import typer
 from typing_extensions import Annotated
@@ -2444,15 +2444,14 @@
                             .cast(pl.Float64, strict=False)
                         )
                         .otherwise(pl.col("AmountHold"))
                         .alias("AmountHold"),
                     ]
                 )
                 df = df.select(
-                    "FeeSheet",
                     "CaseNumber",
                     "Total",
                     "FeeStatus",
                     "AdminFee",
                     "FeeCode",
                     "Payor",
                     "Payee",
```

### Comparing `alacorder-81.0.4/pyproject.toml` & `alacorder-81.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.0.4"
+version = "81.0.5"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `alacorder-81.0.4/PKG-INFO` & `alacorder-81.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.0.4
+Version: 81.0.5
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

