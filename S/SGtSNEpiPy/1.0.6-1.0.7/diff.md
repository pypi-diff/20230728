# Comparing `tmp/SGtSNEpiPy-1.0.6.tar.gz` & `tmp/SGtSNEpiPy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.0.6.tar", last modified: Mon Jul 10 15:55:30 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.0.7.tar", last modified: Fri Jul 28 17:37:48 2023, max compression
```

## Comparing `SGtSNEpiPy-1.0.6.tar` & `SGtSNEpiPy-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 15:55:30.356126 SGtSNEpiPy-1.0.6/
--rw-r--r--   0 aaronzhong   (501) staff       (20)      647 2023-07-10 15:55:30.355945 SGtSNEpiPy-1.0.6/PKG-INFO
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 15:55:30.354995 SGtSNEpiPy-1.0.6/SGtSNEpiPy/
--rw-r--r--   0 aaronzhong   (501) staff       (20)     1053 2023-07-10 15:52:51.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy/SGtSNEpiPy.py
--rw-r--r--   0 aaronzhong   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy/__init__.py
-drwxr-xr-x   0 aaronzhong   (501) staff       (20)        0 2023-07-10 15:55:30.355729 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/
--rw-r--r--   0 aaronzhong   (501) staff       (20)      647 2023-07-10 15:55:30.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 aaronzhong   (501) staff       (20)      225 2023-07-10 15:55:30.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)        1 2023-07-10 15:55:30.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       10 2023-07-10 15:55:30.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       11 2023-07-10 15:55:30.000000 SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/top_level.txt
--rw-r--r--   0 aaronzhong   (501) staff       (20)       38 2023-07-10 15:55:30.356182 SGtSNEpiPy-1.0.6/setup.cfg
--rw-r--r--   0 aaronzhong   (501) staff       (20)      830 2023-07-10 15:54:04.000000 SGtSNEpiPy-1.0.6/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.122972 SGtSNEpiPy-1.0.7/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-28 17:37:48.123089 SGtSNEpiPy-1.0.7/PKG-INFO
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.121786 SGtSNEpiPy-1.0.7/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-28 17:37:48.122805 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      647 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      235 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       10 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-28 17:37:48.000000 SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/top_level.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-28 17:37:48.123406 SGtSNEpiPy-1.0.7/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      830 2023-07-28 17:34:53.000000 SGtSNEpiPy-1.0.7/setup.py
```

### Comparing `SGtSNEpiPy-1.0.6/PKG-INFO` & `SGtSNEpiPy-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.6
+Version: 1.0.7
 Summary: SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 
 This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.
 Email:
 chenshuhao.qin@duke.edu
```

### Comparing `SGtSNEpiPy-1.0.6/SGtSNEpiPy.egg-info/PKG-INFO` & `SGtSNEpiPy-1.0.7/SGtSNEpiPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.0.6
+Version: 1.0.7
 Summary: SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 
 This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.
 Email:
 chenshuhao.qin@duke.edu
```

### Comparing `SGtSNEpiPy-1.0.6/setup.py` & `SGtSNEpiPy-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name='SGtSNEpiPy',
-    version='1.0.6',
+    version='1.0.7',
     description='SGtSNEpiPy is a Python interface for the SG-t-SNE-П algorithm, a powerful tool for visualizing large, sparse, stochastic graphs.',
     long_description= "This is a Python wrapper for SG-t-SNE-П (https://github.com/fcdimitr/SGtSNEpi.jl), implemented using the JuliaCall module (https://cjdoris.github.io/PythonCall.jl/stable/juliacall) from PythonCall & JuliaCall package (https://cjdoris.github.io/PythonCall.jl). If you meet any issue, feel free to contact authors.\nEmail:\nchenshuhao.qin@duke.edu\nyihua.zhong@duke.edu",
     author=['Chenshuhao Qin','Yihua Zhong'],
     author_email="cq27@duke.edu, yz737@duke.edu,",
     packages=setuptools.find_packages(),
     install_requires=[
         'juliacall',
```

