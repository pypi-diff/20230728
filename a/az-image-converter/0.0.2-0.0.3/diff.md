# Comparing `tmp/az_image-converter-0.0.2.tar.gz` & `tmp/az_image-converter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az_image-converter-0.0.2.tar", last modified: Fri Jul 28 11:41:59 2023, max compression
+gzip compressed data, was "az_image-converter-0.0.3.tar", last modified: Fri Jul 28 12:15:09 2023, max compression
```

## Comparing `az_image-converter-0.0.2.tar` & `az_image-converter-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-28 11:06:18.000000 az_image-converter-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3742 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2954 2023-07-28 09:48:45.000000 az_image-converter-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 11:41:59.831100 az_image-converter-0.0.2/az_image_converter.egg-info/
--rw-rw-rw-   0        0        0     3742 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:41:59.000000 az_image-converter-0.0.2/az_image_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 11:41:59.846726 az_image-converter-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     4080 2023-07-28 11:39:32.000000 az_image-converter-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:15:09.354034 az_image-converter-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-28 11:06:18.000000 az_image-converter-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3768 2023-07-28 12:15:09.354034 az_image-converter-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2980 2023-07-28 12:09:11.000000 az_image-converter-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:15:09.354034 az_image-converter-0.0.3/az_image_converter.egg-info/
+-rw-rw-rw-   0        0        0     3768 2023-07-28 12:15:08.000000 az_image-converter-0.0.3/az_image_converter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-28 12:15:08.000000 az_image-converter-0.0.3/az_image_converter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:15:08.000000 az_image-converter-0.0.3/az_image_converter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 12:15:08.000000 az_image-converter-0.0.3/az_image_converter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:15:08.000000 az_image-converter-0.0.3/az_image_converter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:15:09.354034 az_image-converter-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     4106 2023-07-28 12:13:01.000000 az_image-converter-0.0.3/setup.py
```

### Comparing `az_image-converter-0.0.2/LICENSE` & `az_image-converter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `az_image-converter-0.0.2/PKG-INFO` & `az_image-converter-0.0.3/az_image_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: az_image-converter
-Version: 0.0.2
+Name: az-image-converter
+Version: 0.0.3
 Summary: Az Image Converter is a Python library that provides a simple and convenient way to convert images. A Library by Azeem Akhtar
 Author: Azeem Akhtar
 Author-email: hellomazeem@gmail.com
 Keywords: Image,Image Converter,PNG TO JPG Converter,JPG TO PNG Converter,Azeem Akhtar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,15 @@
 ## Version
 0.1.0 (see Changelog for release notes)
 
 
 
 ## Documentation
 
-[Read Documentation](https://linktodocumentation)
+[Read Documentation](https://azeemprogrammer.github.io/az-image-converter/)
 
 
 ## FAQ
 
 #### What image formats does the Az Image Converter Library support for conversion?
 
 The Az Image Converter Library currently supports the conversion of JPG to PNG format and PNG to JPG format. It leverages the Pillow library to handle the image processing tasks efficiently.
```

### Comparing `az_image-converter-0.0.2/README.md` & `az_image-converter-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ## Version
 0.1.0 (see Changelog for release notes)
 
 
 
 ## Documentation
 
-[Read Documentation](https://linktodocumentation)
+[Read Documentation](https://azeemprogrammer.github.io/az-image-converter/)
 
 
 ## FAQ
 
 #### What image formats does the Az Image Converter Library support for conversion?
 
 The Az Image Converter Library currently supports the conversion of JPG to PNG format and PNG to JPG format. It leverages the Pillow library to handle the image processing tasks efficiently.
```

### Comparing `az_image-converter-0.0.2/az_image_converter.egg-info/PKG-INFO` & `az_image-converter-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: az-image-converter
-Version: 0.0.2
+Name: az_image-converter
+Version: 0.0.3
 Summary: Az Image Converter is a Python library that provides a simple and convenient way to convert images. A Library by Azeem Akhtar
 Author: Azeem Akhtar
 Author-email: hellomazeem@gmail.com
 Keywords: Image,Image Converter,PNG TO JPG Converter,JPG TO PNG Converter,Azeem Akhtar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -67,15 +67,15 @@
 ## Version
 0.1.0 (see Changelog for release notes)
 
 
 
 ## Documentation
 
-[Read Documentation](https://linktodocumentation)
+[Read Documentation](https://azeemprogrammer.github.io/az-image-converter/)
 
 
 ## FAQ
 
 #### What image formats does the Az Image Converter Library support for conversion?
 
 The Az Image Converter Library currently supports the conversion of JPG to PNG format and PNG to JPG format. It leverages the Pillow library to handle the image processing tasks efficiently.
```

### Comparing `az_image-converter-0.0.2/setup.py` & `az_image-converter-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Az Image Converter is a Python library that provides a simple and convenient way to convert images. A Library by Azeem Akhtar'
 LONG_DESCRIPTION = '''
 # Az Image Converter Library
 
 ![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
 
@@ -57,15 +57,15 @@
 ## Version
 0.1.0 (see Changelog for release notes)
 
 
 
 ## Documentation
 
-[Read Documentation](https://linktodocumentation)
+[Read Documentation](https://azeemprogrammer.github.io/az-image-converter/)
 
 
 ## FAQ
 
 #### What image formats does the Az Image Converter Library support for conversion?
 
 The Az Image Converter Library currently supports the conversion of JPG to PNG format and PNG to JPG format. It leverages the Pillow library to handle the image processing tasks efficiently.
```

