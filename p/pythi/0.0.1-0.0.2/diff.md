# Comparing `tmp/pythi-0.0.1.tar.gz` & `tmp/pythi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythi-0.0.1.tar", last modified: Fri Jul 28 08:00:01 2023, max compression
+gzip compressed data, was "pythi-0.0.2.tar", last modified: Fri Jul 28 08:13:38 2023, max compression
```

## Comparing `pythi-0.0.1.tar` & `pythi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 08:00:01.628022 pythi-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-07-28 07:35:38.000000 pythi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      319 2023-07-28 08:00:01.627021 pythi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2159 2023-07-28 07:59:52.000000 pythi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 08:00:01.610021 pythi-0.0.1/pythi/
--rw-rw-rw-   0        0        0        0 2023-07-28 07:37:03.000000 pythi-0.0.1/pythi/__init__.py
--rw-rw-rw-   0        0        0      292 2023-07-28 07:43:12.000000 pythi-0.0.1/pythi/pythi.py
-drwxrwxrwx   0        0        0        0 2023-07-28 08:00:01.626021 pythi-0.0.1/pythi.egg-info/
--rw-rw-rw-   0        0        0      319 2023-07-28 08:00:01.000000 pythi-0.0.1/pythi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-07-28 08:00:01.000000 pythi-0.0.1/pythi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 08:00:01.000000 pythi-0.0.1/pythi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-28 08:00:01.000000 pythi-0.0.1/pythi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 08:00:01.628022 pythi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-07-28 07:58:34.000000 pythi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:13:38.704625 pythi-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-07-28 07:35:38.000000 pythi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      319 2023-07-28 08:13:38.703625 pythi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2502 2023-07-28 08:10:06.000000 pythi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 08:13:38.697626 pythi-0.0.2/pythi/
+-rw-rw-rw-   0        0        0       76 2023-07-28 08:09:09.000000 pythi-0.0.2/pythi/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-07-28 07:43:12.000000 pythi-0.0.2/pythi/pythi.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:13:38.702625 pythi-0.0.2/pythi.egg-info/
+-rw-rw-rw-   0        0        0      319 2023-07-28 08:13:38.000000 pythi-0.0.2/pythi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-07-28 08:13:38.000000 pythi-0.0.2/pythi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 08:13:38.000000 pythi-0.0.2/pythi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 08:13:38.000000 pythi-0.0.2/pythi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 08:13:38.704625 pythi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-07-28 08:12:27.000000 pythi-0.0.2/setup.py
```

### Comparing `pythi-0.0.1/LICENSE` & `pythi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythi-0.0.1/README.md` & `pythi-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Project Helpers
+# Pythi, Python Projects Helper
+
+This module contains basic function that help you with your python/jupyter projects.
 
 ## Project Root CWD Unifier
 
-This Python function `unify_cwd()` helps you navigate to the project's root folder that contains the `.git` subfolder. It is particularly useful when you are working in a deep directory structure and want to ensure that your current working directory (CWD) is set to the root of the project for consistent and reliable file access.
+This Python function `unify_cwd()` helps you navigate to the project's root folder that contains the `.git` subfolder. It is particularly useful when you are working in a deep directory structure and want to ensure that your current working directory (CWD) is set to the root of the project for consistent and reliable file access. It is also useful with jupyter notebooks, as their CWD is always their own folder, and this function can be used to set the CWD to the project root.
 
 ### How to Use
 
 1. Install and import the module `pythi` into your Python code.
 
 2. Simply call the `unify_cwd()` function wherever you need to set your CWD to the project's root directory containing the `.git` subfolder.
 
@@ -14,19 +16,21 @@
 
 4. The function will change the CWD to the project root, ensuring that any subsequent file operations or imports are correctly relative to the root directory.
 
 ### Example Usage
 
 ```python
 import os
-import pythi as pj
+from pythi import unify_cwd
 
 def main():
+    # the place where you are in the directory hierarchy
     print("Before unify_cwd():", os.getcwd())
-    pj.unify_cwd()
+    unify_cwd()
+    # the git project root
     print("After unify_cwd():", os.getcwd())
 
 if __name__ == "__main__":
     main()
 ```
 
 In this example, calling `unify_cwd()` inside the `main()` function will change the CWD to the project root, and you will see the updated CWD printed in the console.
```

