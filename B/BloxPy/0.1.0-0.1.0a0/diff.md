# Comparing `tmp/BloxPy-0.1.0.tar.gz` & `tmp/BloxPy-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BloxPy-0.1.0.tar", last modified: Fri Jul 28 20:35:50 2023, max compression
+gzip compressed data, was "BloxPy-0.1.0a0.tar", last modified: Fri Jul 28 20:51:43 2023, max compression
```

## Comparing `BloxPy-0.1.0.tar` & `BloxPy-0.1.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:35:50.202365 BloxPy-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-28 20:35:50.200366 BloxPy-0.1.0/BloxPy.egg-info/
--rw-rw-rw-   0        0        0     2919 2023-07-28 20:35:50.000000 BloxPy-0.1.0/BloxPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-07-28 20:35:50.000000 BloxPy-0.1.0/BloxPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:35:50.000000 BloxPy-0.1.0/BloxPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 20:35:50.000000 BloxPy-0.1.0/BloxPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:35:50.000000 BloxPy-0.1.0/BloxPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2919 2023-07-28 20:35:50.201366 BloxPy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-07-28 20:35:14.000000 BloxPy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 20:35:50.202365 BloxPy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1738 2023-07-28 20:34:34.000000 BloxPy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 20:51:43.375703 BloxPy-0.1.0a0/
+drwxrwxrwx   0        0        0        0 2023-07-28 20:51:43.373705 BloxPy-0.1.0a0/BloxPy.egg-info/
+-rw-rw-rw-   0        0        0     2921 2023-07-28 20:51:43.000000 BloxPy-0.1.0a0/BloxPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-07-28 20:51:43.000000 BloxPy-0.1.0a0/BloxPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:51:43.000000 BloxPy-0.1.0a0/BloxPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 20:51:43.000000 BloxPy-0.1.0a0/BloxPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 20:51:43.000000 BloxPy-0.1.0a0/BloxPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2921 2023-07-28 20:51:43.374704 BloxPy-0.1.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-07-28 20:35:14.000000 BloxPy-0.1.0a0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 20:51:43.375703 BloxPy-0.1.0a0/setup.cfg
+-rw-rw-rw-   0        0        0     1781 2023-07-28 20:42:39.000000 BloxPy-0.1.0a0/setup.py
```

### Comparing `BloxPy-0.1.0/BloxPy.egg-info/PKG-INFO` & `BloxPy-0.1.0a0/BloxPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: BloxPy: Your All-in-One Python Library for Roblox Development
 Home-page: https://github.com/yourusername/bloxpy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `BloxPy-0.1.0/PKG-INFO` & `BloxPy-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: BloxPy: Your All-in-One Python Library for Roblox Development
 Home-page: https://github.com/yourusername/bloxpy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `BloxPy-0.1.0/README.md` & `BloxPy-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.0/setup.py` & `BloxPy-0.1.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = 'BloxPy'
-VERSION = '0.1.0'
+VERSION = '0.1.0-alpha'
 DESCRIPTION = 'BloxPy: Your All-in-One Python Library for Roblox Development'
 LONG_DESCRIPTION = 'BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.'
 AUTHOR = 'Developer X'
 EMAIL = 'developer.x.business@gmail.com'
 URL = 'https://github.com/yourusername/bloxpy'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
@@ -26,14 +26,15 @@
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     license=LICENSE,
     python_requires=PYTHON_REQUIRES,
     packages=find_packages(exclude=['tests']), 
     install_requires=REQUIRES,
+    development_status='3 - Alpha',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

