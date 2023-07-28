# Comparing `tmp/pkgUdit-1.1.5.8.tar.gz` & `tmp/pkgUdit-1.1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgUdit-1.1.5.8.tar", last modified: Fri Jul 28 09:32:19 2023, max compression
+gzip compressed data, was "pkgUdit-1.1.5.9.tar", last modified: Fri Jul 28 09:38:36 2023, max compression
```

## Comparing `pkgUdit-1.1.5.8.tar` & `pkgUdit-1.1.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:32:19.403868 pkgUdit-1.1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:32:19.403868 pkgUdit-1.1.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:32:19.399868 pkgUdit-1.1.5.8/pkgUdit/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/pkgUdit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:32:19.403868 pkgUdit-1.1.5.8/pkgUdit/data/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/pkgUdit/data/Names.csv
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/pkgUdit/data/Places.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/pkgUdit/pswdGen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/pkgUdit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:32:19.403868 pkgUdit-1.1.5.8/pkgUdit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:32:19.000000 pkgUdit-1.1.5.8/pkgUdit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:32:19.000000 pkgUdit-1.1.5.8/pkgUdit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:32:19.000000 pkgUdit-1.1.5.8/pkgUdit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:32:19.000000 pkgUdit-1.1.5.8/pkgUdit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 09:32:19.000000 pkgUdit-1.1.5.8/pkgUdit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:32:19.403868 pkgUdit-1.1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 09:32:06.000000 pkgUdit-1.1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/data/Names.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/data/Places.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/pswdGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/pkgUdit/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/pkgUdit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 09:38:36.000000 pkgUdit-1.1.5.9/pkgUdit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:38:36.223381 pkgUdit-1.1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 09:38:23.000000 pkgUdit-1.1.5.9/setup.py
```

### Comparing `pkgUdit-1.1.5.8/pkgUdit/pswdGen.py` & `pkgUdit-1.1.5.9/pkgUdit/pswdGen.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 upper_chars = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J',
              'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 
              'U', 'V', 'W', 'X', 'Y', 'Z']
 
 combined_chars = numerals + lower_caps + upper_chars
 module_dir = os.path.dirname(__file__)
 
+# print("module_dir>>>>>>>" , module_dir)
+
 def read_csv_file(file_name):
     """
     Read a CSV file and return its contents as a list.
 
     Args:
         file_name (str): The name of the CSV file to read.
 
     Returns:
         list: A list containing the values read from the CSV file.
     """
-    file_path = os.path.join(module_dir, file_name)
+    file_path = os.path.join(module_dir,"data",file_name)
+    # print("file_path>>>>>>",file_path)
     with open(file_path) as csv_file:
         csv_reader = csv.reader(csv_file)
         return [row[0] for row in csv_reader]
 
 name_list = read_csv_file('Names.csv')
 place_list = read_csv_file('Places.csv')
```

### Comparing `pkgUdit-1.1.5.8/pkgUdit/test.py` & `pkgUdit-1.1.5.9/pkgUdit/test.py`

 * *Files identical despite different names*

### Comparing `pkgUdit-1.1.5.8/setup.py` & `pkgUdit-1.1.5.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="pkgUdit",                     # This is the name of the package
-    version="1.1.5.8",                        # The current release version
+    version="1.1.5.9",                        # The current release version
     author="Udit Sharma",                     # Full name of the author
     description="The is a sample package",
     zip_safe=False,
     package_data={'pkgUdit': ['data/*.csv']},
     include_package_data=True,
     # long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
```

