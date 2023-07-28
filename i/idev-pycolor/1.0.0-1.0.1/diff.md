# Comparing `tmp/idev-pycolor-1.0.0.tar.gz` & `tmp/idev-pycolor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pycolor-1.0.0.tar", last modified: Fri Jul 28 08:46:43 2023, max compression
+gzip compressed data, was "idev-pycolor-1.0.1.tar", last modified: Fri Jul 28 20:30:49 2023, max compression
```

## Comparing `idev-pycolor-1.0.0.tar` & `idev-pycolor-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 08:46:43.188381 idev-pycolor-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7014 2023-07-28 08:46:43.189387 idev-pycolor-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6268 2023-07-28 05:40:21.000000 idev-pycolor-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 08:46:43.153222 idev-pycolor-1.0.0/idev-pycolor/
-drwxrwxrwx   0        0        0        0 2023-07-28 08:46:43.167385 idev-pycolor-1.0.0/idev-pycolor/PyColor/
--rw-rw-rw-   0        0        0    35141 2023-07-28 06:33:41.000000 idev-pycolor-1.0.0/idev-pycolor/PyColor/Colors.py
--rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.0/idev-pycolor/PyColor/Palettes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.0/idev-pycolor/PyColor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 08:46:43.187387 idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/
--rw-rw-rw-   0        0        0     7014 2023-07-28 08:46:43.000000 idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-28 08:46:43.000000 idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 08:46:43.000000 idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 08:46:43.000000 idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      740 2023-07-28 08:45:57.000000 idev-pycolor-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      889 2023-07-28 08:46:43.191419 idev-pycolor-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-28 08:45:55.000000 idev-pycolor-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.479784 idev-pycolor-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7275 2023-07-28 20:30:49.480785 idev-pycolor-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6529 2023-07-28 20:30:17.000000 idev-pycolor-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.432784 idev-pycolor-1.0.1/idev-pycolor/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.462783 idev-pycolor-1.0.1/idev-pycolor/PyColor/
+-rw-rw-rw-   0        0        0    35141 2023-07-28 06:33:41.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/Colors.py
+-rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/Palettes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.478785 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/
+-rw-rw-rw-   0        0        0     7275 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      740 2023-07-28 20:29:39.000000 idev-pycolor-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-28 20:30:49.482029 idev-pycolor-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-28 20:29:44.000000 idev-pycolor-1.0.1/setup.py
```

### Comparing `idev-pycolor-1.0.0/LICENSE` & `idev-pycolor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.0/PKG-INFO` & `idev-pycolor-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,28 @@
 - **XYZ** (*x*, *y*, *z*)
 - **YCC** (*y*, *cb*, *cr*)
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
+
+## Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyColor.git
+```
+or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
+```
+pip install idev-pycolor
+```
+<br />
+<br />
+<br />
+<br />
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
```

### Comparing `idev-pycolor-1.0.0/README.md` & `idev-pycolor-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,28 @@
 - **XYZ** (*x*, *y*, *z*)
 - **YCC** (*y*, *cb*, *cr*)
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
+
+## Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyColor.git
+```
+or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
+```
+pip install idev-pycolor
+```
+<br />
+<br />
+<br />
+<br />
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
```

### Comparing `idev-pycolor-1.0.0/idev-pycolor/PyColor/Colors.py` & `idev-pycolor-1.0.1/idev-pycolor/PyColor/Colors.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.0/idev-pycolor/PyColor/Palettes.py` & `idev-pycolor-1.0.1/idev-pycolor/PyColor/Palettes.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.0/idev-pycolor/idev_pycolor.egg-info/PKG-INFO` & `idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,28 @@
 - **XYZ** (*x*, *y*, *z*)
 - **YCC** (*y*, *cb*, *cr*)
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
+
+## Installation
+With `git` [GitHub](https://github.com):
+```
+git clone https://github.com/IrtsaDevelopment/PyColor.git
+```
+or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
+```
+pip install idev-pycolor
+```
+<br />
+<br />
+<br />
+<br />
 <br />
 <br />
 
 ## Usage
 To import, simply put:
 ```py
 from PyColor.Colors import *
```

### Comparing `idev-pycolor-1.0.0/pyproject.toml` & `idev-pycolor-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pycolor"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idev-pycolor-1.0.0/setup.cfg` & `idev-pycolor-1.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e30  .version = 1.0.0
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e31  .version = 1.0.1
 00000030: 0d0a 6175 7468 6f72 203d 2049 7274 7361  ..author = Irtsa
 00000040: 4465 7665 6c6f 706d 656e 740d 0a61 7574  Development..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6972 7473  hor_email = irts
 00000060: 612e 6465 7665 6c6f 706d 656e 7440 676d  a.development@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 636f 6c6c 6563 7469 6f6e 206f 6620 636c  collection of cl
@@ -19,38 +19,38 @@
 00000120: 7273 2e0d 0a6c 6f6e 675f 6465 7363 7269  rs...long_descri
 00000130: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
 00000140: 4144 4d45 2e6d 642c 204c 4943 454e 5345  ADME.md, LICENSE
 00000150: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000160: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
 00000170: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
 00000180: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
-00000190: 6974 6c61 622e 636f 6d2f 636f 6461 7374  itlab.com/codast
-000001a0: 6572 6f69 642f 6261 7369 6370 6b67 0d0a  eroid/basicpkg..
-000001b0: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-000001c0: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-000001d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001e0: 6f6d 2f49 7274 7361 4465 7665 6c6f 706d  om/IrtsaDevelopm
-000001f0: 656e 742f 5079 436f 6c6f 722f 6973 7375  ent/PyColor/issu
-00000200: 6573 0d0a 0972 6570 6f73 6974 6f72 7920  es...repository 
-00000210: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000220: 2e63 6f6d 2f49 7274 7361 4465 7665 6c6f  .com/IrtsaDevelo
-00000230: 706d 656e 742f 5079 436f 6c6f 720d 0a63  pment/PyColor..c
-00000240: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-00000250: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000260: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000270: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-00000280: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000290: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-000002a0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-000002b0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000002c0: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-000002d0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-000002e0: 093d 2069 6465 762d 7079 636f 6c6f 720d  .= idev-pycolor.
-000002f0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000300: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000310: 6573 203d 203e 3d33 2e36 0d0a 0d0a 5b6f  es = >=3.6....[o
-00000320: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000330: 6669 6e64 5d0d 0a77 6865 7265 203d 2069  find]..where = i
-00000340: 6465 762d 7079 636f 6c6f 720d 0a0d 0a5b  dev-pycolor....[
-00000350: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000360: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000370: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000190: 6974 6875 622e 636f 6d2f 4972 7473 6144  ithub.com/IrtsaD
+000001a0: 6576 656c 6f70 6d65 6e74 2f50 7943 6f6c  evelopment/PyCol
+000001b0: 6f72 0d0a 7072 6f6a 6563 745f 7572 6c73  or..project_urls
+000001c0: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+000001d0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+000001e0: 7562 2e63 6f6d 2f49 7274 7361 4465 7665  ub.com/IrtsaDeve
+000001f0: 6c6f 706d 656e 742f 5079 436f 6c6f 722f  lopment/PyColor/
+00000200: 6973 7375 6573 0d0a 0972 6570 6f73 6974  issues...reposit
+00000210: 6f72 7920 3d20 6874 7470 733a 2f2f 6769  ory = https://gi
+00000220: 7468 7562 2e63 6f6d 2f49 7274 7361 4465  thub.com/IrtsaDe
+00000230: 7665 6c6f 706d 656e 742f 5079 436f 6c6f  velopment/PyColo
+00000240: 720d 0a63 6c61 7373 6966 6965 7273 203d  r..classifiers =
+00000250: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000270: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+00000280: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000290: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000002a0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000002b0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000002c0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+000002d0: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+000002e0: 3d20 0d0a 093d 2069 6465 762d 7079 636f  = ...= idev-pyco
+000002f0: 6c6f 720d 0a70 6163 6b61 6765 7320 3d20  lor..packages = 
+00000300: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000310: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
+00000320: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000330: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000340: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
+00000350: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000360: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000370: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `idev-pycolor-1.0.0/setup.py` & `idev-pycolor-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pycolor",
-    version = "1.0.0",
+    version = "1.0.1",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
     description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyColor",
     project_urls = {
```

