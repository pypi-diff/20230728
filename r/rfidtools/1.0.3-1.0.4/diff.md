# Comparing `tmp/rfidtools-1.0.3.tar.gz` & `tmp/rfidtools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfidtools-1.0.3.tar", max compression
+gzip compressed data, was "rfidtools-1.0.4.tar", max compression
```

## Comparing `rfidtools-1.0.3.tar` & `rfidtools-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-1.0.3/README.md
--rw-r--r--   0        0        0      419 2023-07-28 08:27:23.543115 rfidtools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    32921 2023-07-28 06:44:42.532833 rfidtools-1.0.3/rfidtools/RFID_Icon.ico
--rw-r--r--   0        0        0      721 2023-07-28 07:43:46.280718 rfidtools-1.0.3/rfidtools/__init__.py
--rw-r--r--   0        0        0      905 2023-07-28 08:27:08.959509 rfidtools-1.0.3/rfidtools/__main__.py
--rw-r--r--   0        0        0      678 2023-07-28 05:19:44.057505 rfidtools-1.0.3/rfidtools/config_template.yaml
--rw-r--r--   0        0        0     2944 2023-07-28 07:49:33.475293 rfidtools-1.0.3/rfidtools/core.py
--rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-1.0.3/rfidtools/labels/__init__.py
--rw-r--r--   0        0        0     5322 2023-07-28 07:00:45.995574 rfidtools-1.0.3/rfidtools/labels/add.py
--rw-r--r--   0        0        0     4661 2023-07-28 03:39:58.341496 rfidtools-1.0.3/rfidtools/labels/print.py
--rw-r--r--   0        0        0     5229 2023-07-28 07:33:05.476165 rfidtools-1.0.3/rfidtools/labels/utils.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 rfidtools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-1.0.4/README.md
+-rw-r--r--   0        0        0      419 2023-07-28 08:31:55.688124 rfidtools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    32921 2023-07-28 06:44:42.532833 rfidtools-1.0.4/rfidtools/RFID_Icon.ico
+-rw-r--r--   0        0        0      721 2023-07-28 07:43:46.280718 rfidtools-1.0.4/rfidtools/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-28 08:31:33.741059 rfidtools-1.0.4/rfidtools/__main__.py
+-rw-r--r--   0        0        0      678 2023-07-28 05:19:44.057505 rfidtools-1.0.4/rfidtools/config_template.yaml
+-rw-r--r--   0        0        0     2944 2023-07-28 07:49:33.475293 rfidtools-1.0.4/rfidtools/core.py
+-rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-1.0.4/rfidtools/labels/__init__.py
+-rw-r--r--   0        0        0     5322 2023-07-28 07:00:45.995574 rfidtools-1.0.4/rfidtools/labels/add.py
+-rw-r--r--   0        0        0     4661 2023-07-28 03:39:58.341496 rfidtools-1.0.4/rfidtools/labels/print.py
+-rw-r--r--   0        0        0     5229 2023-07-28 07:33:05.476165 rfidtools-1.0.4/rfidtools/labels/utils.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 rfidtools-1.0.4/PKG-INFO
```

### Comparing `rfidtools-1.0.3/rfidtools/RFID_Icon.ico` & `rfidtools-1.0.4/rfidtools/RFID_Icon.ico`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/__init__.py` & `rfidtools-1.0.4/rfidtools/__init__.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/__main__.py` & `rfidtools-1.0.4/rfidtools/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import platform
 import argparse
 import PyInstaller.__main__ as build
 
 from rfidtools.core import gui_loop
 
 
@@ -18,18 +19,19 @@
 BUILD = vars(parser.parse_args())['build_exe']
 
 
 if not BUILD:
     gui_loop()
 
 else:
+    dir_path = os.path.dirname(os.path.realpath(__file__))
     if platform.system() == 'Windows':
         build.run([
             '__main__.py',
-            '--distpath C:\\',
+            f'--distpath {dir_path}',
             '-F',
             '-n RFID_Tools',
             '--windowed',
             '-i RFID_Icon.ico'])
     else:
         print('Building to .exe is only supported on Windows.')
         raise SystemError
```

### Comparing `rfidtools-1.0.3/rfidtools/config_template.yaml` & `rfidtools-1.0.4/rfidtools/config_template.yaml`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/core.py` & `rfidtools-1.0.4/rfidtools/core.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/labels/add.py` & `rfidtools-1.0.4/rfidtools/labels/add.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/labels/print.py` & `rfidtools-1.0.4/rfidtools/labels/print.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/rfidtools/labels/utils.py` & `rfidtools-1.0.4/rfidtools/labels/utils.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.0.3/PKG-INFO` & `rfidtools-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfidtools
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tool for RFID production at CIOT.
 Author: ar-bebop
 Author-email: aribeir4@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fabric (>=3.1.0,<4.0.0)
```

