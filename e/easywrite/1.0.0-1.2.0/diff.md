# Comparing `tmp/easywrite-1.0.0.tar.gz` & `tmp/easywrite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easywrite-1.0.0.tar", last modified: Fri Jul 28 14:49:46 2023, max compression
+gzip compressed data, was "easywrite-1.2.0.tar", last modified: Fri Jul 28 15:58:08 2023, max compression
```

## Comparing `easywrite-1.0.0.tar` & `easywrite-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 14:49:46.370000 easywrite-1.0.0/
--rw-rw-rw-   0        0        0      433 2023-07-28 14:49:48.000000 easywrite-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-28 14:48:58.000000 easywrite-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 14:49:46.390000 easywrite-1.0.0/easywrite.egg-info/
--rw-rw-rw-   0        0        0      433 2023-07-28 14:49:48.000000 easywrite-1.0.0/easywrite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-28 14:49:48.000000 easywrite-1.0.0/easywrite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 14:49:48.000000 easywrite-1.0.0/easywrite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-28 14:49:48.000000 easywrite-1.0.0/easywrite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      476 2023-07-28 14:48:46.000000 easywrite-1.0.0/easywrite.py
--rw-rw-rw-   0        0        0       42 2023-07-28 14:49:48.000000 easywrite-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-07-28 14:48:14.000000 easywrite-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:58:08.580000 easywrite-1.2.0/
+-rw-rw-rw-   0        0        0      430 2023-07-28 15:58:10.000000 easywrite-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-28 14:48:58.000000 easywrite-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 15:58:08.620000 easywrite-1.2.0/easywrite.egg-info/
+-rw-rw-rw-   0        0        0      430 2023-07-28 15:58:10.000000 easywrite-1.2.0/easywrite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-28 15:58:10.000000 easywrite-1.2.0/easywrite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 15:58:10.000000 easywrite-1.2.0/easywrite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 15:58:10.000000 easywrite-1.2.0/easywrite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      480 2023-07-28 15:45:22.000000 easywrite-1.2.0/easywrite.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 15:58:10.000000 easywrite-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-28 15:57:42.000000 easywrite-1.2.0/setup.py
```

### Comparing `easywrite-1.0.0/setup.py` & `easywrite-1.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='easywrite',
-    version='1.0.0',
-    author='Your Name',
+    version='1.2.0',
+    author='skxllhead',
     description='A Python module for easy text output with colors',
     long_description='Put a more detailed description of your module here',
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/easywrite',
+    url='https://github.com/skxllhead/easywrite',
     py_modules=['easywrite'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

