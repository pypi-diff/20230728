# Comparing `tmp/ATTools-0.1.tar.gz` & `tmp/ATTools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATTools-0.1.tar", last modified: Fri Jul 28 10:27:58 2023, max compression
+gzip compressed data, was "ATTools-0.2.tar", last modified: Fri Jul 28 10:35:33 2023, max compression
```

## Comparing `ATTools-0.1.tar` & `ATTools-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:27:58.317683 ATTools-0.1/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:27:58.313686 ATTools-0.1/ATTools.egg-info/
--rw-rw-rw-   0        0        0      493 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-28 10:27:58.000000 ATTools-0.1/ATTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      493 2023-07-28 10:27:58.316684 ATTools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 10:27:58.317683 ATTools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-28 10:27:07.000000 ATTools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:35:33.945462 ATTools-0.2/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:35:33.942465 ATTools-0.2/ATTools.egg-info/
+-rw-rw-rw-   0        0        0      596 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      596 2023-07-28 10:35:33.944465 ATTools-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:35:33.945462 ATTools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-07-28 10:34:51.000000 ATTools-0.2/setup.py
```

### Comparing `ATTools-0.1/setup.py` & `ATTools-0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ATTools',
-    version='0.1',
+    version='0.2',
     author='NEVNORME',
     author_email='dev.nevermore696@gmail.com',
     description='Tools for The Open Network',
     packages=find_packages(),
     install_requires=[
         'asyncio',
         'aiohttp',
@@ -19,9 +19,11 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

