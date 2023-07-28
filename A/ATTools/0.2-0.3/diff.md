# Comparing `tmp/ATTools-0.2.tar.gz` & `tmp/ATTools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATTools-0.2.tar", last modified: Fri Jul 28 10:35:33 2023, max compression
+gzip compressed data, was "ATTools-0.3.tar", last modified: Fri Jul 28 10:40:18 2023, max compression
```

## Comparing `ATTools-0.2.tar` & `ATTools-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:35:33.945462 ATTools-0.2/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:35:33.942465 ATTools-0.2/ATTools.egg-info/
--rw-rw-rw-   0        0        0      596 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:35:33.000000 ATTools-0.2/ATTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      596 2023-07-28 10:35:33.944465 ATTools-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 10:35:33.945462 ATTools-0.2/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-07-28 10:34:51.000000 ATTools-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:40:18.510405 ATTools-0.3/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:40:18.507407 ATTools-0.3/ATTools.egg-info/
+-rw-rw-rw-   0        0        0      173 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:40:18.000000 ATTools-0.3/ATTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      173 2023-07-28 10:40:18.509404 ATTools-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 10:40:18.510405 ATTools-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      914 2023-07-28 10:40:08.000000 ATTools-0.3/setup.py
```

### Comparing `ATTools-0.2/setup.py` & `ATTools-0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ATTools',
-    version='0.2',
+    version='0.3',
     author='NEVNORME',
     author_email='dev.nevermore696@gmail.com',
     description='Tools for The Open Network',
     packages=find_packages(),
     install_requires=[
         'asyncio',
         'aiohttp',
         'tonconnect',
         'dedust',
         'tontools',
         'xjet'
     ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
+    # classifiers=[
+    #     'Development Status :: 3 - Alpha',
+    #     'Intended Audience :: Developers',
+    #     'License :: OSI Approved :: MIT License',
+    #     'Programming Language :: Python :: 3',
+    #     'Programming Language :: Python :: 3.6',
+    #     'Programming Language :: Python :: 3.7',
+    #     'Programming Language :: Python :: 3.8',
+    #     'Programming Language :: Python :: 3.9',
+    #     'Programming Language :: Python :: 3.10',
+    # ],
+    python_requires='>=3.6'
 )
```

