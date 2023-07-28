# Comparing `tmp/simple_lama_inpainting-0.1.1.tar.gz` & `tmp/simple_lama_inpainting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_lama_inpainting-0.1.1.tar", max compression
+gzip compressed data, was "simple_lama_inpainting-0.1.2.tar", max compression
```

## Comparing `simple_lama_inpainting-0.1.1.tar` & `simple_lama_inpainting-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-07-23 07:23:28.922434 simple_lama_inpainting-0.1.1/LICENSE
--rw-r--r--   0        0        0     1254 2023-07-11 21:55:51.529964 simple_lama_inpainting-0.1.1/README.md
--rw-r--r--   0        0        0      690 2023-07-23 08:31:15.918958 simple_lama_inpainting-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-23 08:31:15.919316 simple_lama_inpainting-0.1.1/simple_lama_inpainting/__init__.py
--rw-r--r--   0        0        0     1260 2023-07-23 08:31:15.919665 simple_lama_inpainting-0.1.1/simple_lama_inpainting/cli.py
--rw-r--r--   0        0        0        0 2023-07-23 08:31:15.919734 simple_lama_inpainting-0.1.1/simple_lama_inpainting/models/__init__.py
--rw-r--r--   0        0        0     1454 2023-07-23 08:31:15.920100 simple_lama_inpainting-0.1.1/simple_lama_inpainting/models/model.py
--rw-r--r--   0        0        0        0 2023-07-23 08:31:15.920152 simple_lama_inpainting-0.1.1/simple_lama_inpainting/utils/__init__.py
--rw-r--r--   0        0        0     2972 2023-07-23 08:31:15.920451 simple_lama_inpainting-0.1.1/simple_lama_inpainting/utils/util.py
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 simple_lama_inpainting-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-23 07:23:28.922434 simple_lama_inpainting-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1254 2023-07-11 21:55:51.529964 simple_lama_inpainting-0.1.2/README.md
+-rw-r--r--   0        0        0      689 2023-07-28 13:03:03.383700 simple_lama_inpainting-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-23 08:31:15.919316 simple_lama_inpainting-0.1.2/simple_lama_inpainting/__init__.py
+-rw-r--r--   0        0        0     1260 2023-07-23 08:31:15.919665 simple_lama_inpainting-0.1.2/simple_lama_inpainting/cli.py
+-rw-r--r--   0        0        0        0 2023-07-23 08:31:15.919734 simple_lama_inpainting-0.1.2/simple_lama_inpainting/models/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-23 08:31:15.920100 simple_lama_inpainting-0.1.2/simple_lama_inpainting/models/model.py
+-rw-r--r--   0        0        0        0 2023-07-23 08:31:15.920152 simple_lama_inpainting-0.1.2/simple_lama_inpainting/utils/__init__.py
+-rw-r--r--   0        0        0     2972 2023-07-23 08:31:15.920451 simple_lama_inpainting-0.1.2/simple_lama_inpainting/utils/util.py
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 simple_lama_inpainting-0.1.2/PKG-INFO
```

### Comparing `simple_lama_inpainting-0.1.1/LICENSE` & `simple_lama_inpainting-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_lama_inpainting-0.1.1/README.md` & `simple_lama_inpainting-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simple_lama_inpainting-0.1.1/pyproject.toml` & `simple_lama_inpainting-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "simple-lama-inpainting"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["enesmsahin <enessahin@outlook.com>"]
 readme = "README.md"
 packages = [{include = "simple_lama_inpainting"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "^1.25.1"
+numpy = "^1.24.3"
 opencv-python = "^4.8.0.74"
-pillow = "^10.0.0"
+pillow = "^9.5.0"
 torch = ">=1.13.1, !=2.0.1"
 torchvision = ">=0.14.1"
 fire = "^0.5.0"
 
 [tool.poetry.scripts]
 simple_lama = "simple_lama_inpainting.cli:lama_cli"
```

### Comparing `simple_lama_inpainting-0.1.1/simple_lama_inpainting/cli.py` & `simple_lama_inpainting-0.1.2/simple_lama_inpainting/cli.py`

 * *Files identical despite different names*

### Comparing `simple_lama_inpainting-0.1.1/simple_lama_inpainting/models/model.py` & `simple_lama_inpainting-0.1.2/simple_lama_inpainting/models/model.py`

 * *Files identical despite different names*

### Comparing `simple_lama_inpainting-0.1.1/simple_lama_inpainting/utils/util.py` & `simple_lama_inpainting-0.1.2/simple_lama_inpainting/utils/util.py`

 * *Files identical despite different names*

### Comparing `simple_lama_inpainting-0.1.1/PKG-INFO` & `simple_lama_inpainting-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: simple-lama-inpainting
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: enesmsahin
 Author-email: enessahin@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.8.0.74,<5.0.0.0)
-Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: torch (>=1.13.1,!=2.0.1)
 Requires-Dist: torchvision (>=0.14.1)
 Description-Content-Type: text/markdown
 
 # simple-lama-inpainting
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: simple-lama-inpainting Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: simple-lama-inpainting Version: 0.1.2 Summary:
 Author: enesmsahin Author-email: enessahin@outlook.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: numpy
-(>=1.25.1,<2.0.0) Requires-Dist: opencv-python (>=4.8.0.74,<5.0.0.0) Requires-
-Dist: pillow (>=10.0.0,<11.0.0) Requires-Dist: torch (>=1.13.1,!=2.0.1)
+(>=1.24.3,<2.0.0) Requires-Dist: opencv-python (>=4.8.0.74,<5.0.0.0) Requires-
+Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: torch (>=1.13.1,!=2.0.1)
 Requires-Dist: torchvision (>=0.14.1) Description-Content-Type: text/markdown #
 simple-lama-inpainting
                   Simple pip package for LaMa[1] inpainting.
                                 [PyPI_version]
 ## Installation ``` pip install simple-lama-inpainting ``` ## Usage ### CLI ```
 simple_lama    ``` ### Integration to Your Code Input formats: `np.ndarray` or
 `PIL.Image.Image`. (3 channel input image & 1 channel binary mask image where
```

