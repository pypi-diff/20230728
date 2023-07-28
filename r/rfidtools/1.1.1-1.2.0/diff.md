# Comparing `tmp/rfidtools-1.1.1.tar.gz` & `tmp/rfidtools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfidtools-1.1.1.tar", max compression
+gzip compressed data, was "rfidtools-1.2.0.tar", max compression
```

## Comparing `rfidtools-1.1.1.tar` & `rfidtools-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-1.1.1/README.md
--rw-r--r--   0        0        0      419 2023-07-28 08:42:28.226077 rfidtools-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    32921 2023-07-28 06:44:42.532833 rfidtools-1.1.1/rfidtools/RFID_Icon.ico
--rw-r--r--   0        0        0      721 2023-07-28 07:43:46.280718 rfidtools-1.1.1/rfidtools/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-28 08:42:18.312569 rfidtools-1.1.1/rfidtools/__main__.py
--rw-r--r--   0        0        0      678 2023-07-28 05:19:44.057505 rfidtools-1.1.1/rfidtools/config_template.yaml
--rw-r--r--   0        0        0     2944 2023-07-28 07:49:33.475293 rfidtools-1.1.1/rfidtools/core.py
--rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-1.1.1/rfidtools/labels/__init__.py
--rw-r--r--   0        0        0     5322 2023-07-28 07:00:45.995574 rfidtools-1.1.1/rfidtools/labels/add.py
--rw-r--r--   0        0        0     4661 2023-07-28 03:39:58.341496 rfidtools-1.1.1/rfidtools/labels/print.py
--rw-r--r--   0        0        0     5229 2023-07-28 07:33:05.476165 rfidtools-1.1.1/rfidtools/labels/utils.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 rfidtools-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-1.2.0/README.md
+-rw-r--r--   0        0        0      419 2023-07-28 09:31:50.112639 rfidtools-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    32921 2023-07-28 06:44:42.532833 rfidtools-1.2.0/rfidtools/RFID_Icon.ico
+-rw-r--r--   0        0        0      733 2023-07-28 09:13:54.391034 rfidtools-1.2.0/rfidtools/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-28 09:31:03.151848 rfidtools-1.2.0/rfidtools/__main__.py
+-rw-r--r--   0        0        0      678 2023-07-28 05:19:44.057505 rfidtools-1.2.0/rfidtools/config_template.yaml
+-rw-r--r--   0        0        0     2944 2023-07-28 07:49:33.475293 rfidtools-1.2.0/rfidtools/core.py
+-rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-1.2.0/rfidtools/labels/__init__.py
+-rw-r--r--   0        0        0     5322 2023-07-28 07:00:45.995574 rfidtools-1.2.0/rfidtools/labels/add.py
+-rw-r--r--   0        0        0     4661 2023-07-28 03:39:58.341496 rfidtools-1.2.0/rfidtools/labels/print.py
+-rw-r--r--   0        0        0     5229 2023-07-28 07:33:05.476165 rfidtools-1.2.0/rfidtools/labels/utils.py
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 rfidtools-1.2.0/PKG-INFO
```

### Comparing `rfidtools-1.1.1/rfidtools/RFID_Icon.ico` & `rfidtools-1.2.0/rfidtools/RFID_Icon.ico`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/rfidtools/__init__.py` & `rfidtools-1.2.0/rfidtools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path
+from os import path
 
 import yaml
 
 
 global DB_SERVER
 global DB_TABLE
 global DB_USER
@@ -10,15 +10,15 @@
 
 global SSH_SERVER
 global SSH_USER
 global SSH_PASS
 global SSH_LOGS_PATH
 global SSH_ARCHIVES_PATH
 
-config_path = Path(__file__).parent.joinpath('config.yaml')
+config_path = path.abspath(path.join(path.dirname(__file__), 'config.yaml'))
 with open(config_path) as config_file:
     config = yaml.load(config_file, Loader=yaml.Loader)
 
     DB_SERVER = config['db']['server']
     DB_TABLE = config['db']['table']
     DB_USER = config['db']['user']
     DB_PASS = config['db']['pass']
```

### Comparing `rfidtools-1.1.1/rfidtools/__main__.py` & `rfidtools-1.2.0/rfidtools/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import platform
 import argparse
 import PyInstaller.__main__ as build
 
 from rfidtools.core import gui_loop
 
+PATH = os.path.dirname(os.path.realpath(__file__))
 
 parser = argparse.ArgumentParser(
     prog='rfidtools',
     description='Tool for RFID tag production at CIOT.',
     epilog='Use "python -m rfidtools" to run from the command line.')
 
 parser.add_argument('-b', '--build-exe',
@@ -20,19 +21,20 @@
 
 
 if not BUILD:
     gui_loop()
 
 else:
     if platform.system() == 'Windows':
-        dir_path = os.path.dirname(os.path.realpath(__file__))
-        desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
+        desktop = os.environ['USERPROFILE'] + '\\Desktop'
         build.run([
-            f'{dir_path}\\__main__.py',
+            f'{PATH}\\__main__.py',
             '-F',
-            f'--distpath {desktop}',
+            f'--distpath={desktop}',
+            f'--add-data={PATH}\\config.yaml;rfidtools',
             '-n RFID_Tools',
             '--windowed',
-            '-i RFID_Icon.ico'])
+            f'--icon={PATH}\\RFID_Icon.ico'])
+
     else:
         print('Building to .exe is only supported on Windows.')
         raise SystemError
```

### Comparing `rfidtools-1.1.1/rfidtools/config_template.yaml` & `rfidtools-1.2.0/rfidtools/config_template.yaml`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/rfidtools/core.py` & `rfidtools-1.2.0/rfidtools/core.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/rfidtools/labels/add.py` & `rfidtools-1.2.0/rfidtools/labels/add.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/rfidtools/labels/print.py` & `rfidtools-1.2.0/rfidtools/labels/print.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/rfidtools/labels/utils.py` & `rfidtools-1.2.0/rfidtools/labels/utils.py`

 * *Files identical despite different names*

### Comparing `rfidtools-1.1.1/PKG-INFO` & `rfidtools-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfidtools
-Version: 1.1.1
+Version: 1.2.0
 Summary: A tool for RFID production at CIOT.
 Author: ar-bebop
 Author-email: aribeir4@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fabric (>=3.1.0,<4.0.0)
```

