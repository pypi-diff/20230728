# Comparing `tmp/zipline.py-0.8.0.tar.gz` & `tmp/zipline.py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline.py-0.8.0.tar", last modified: Fri Jul 28 08:52:33 2023, max compression
+gzip compressed data, was "zipline.py-0.8.1.tar", last modified: Fri Jul 28 08:54:07 2023, max compression
```

## Comparing `zipline.py-0.8.0.tar` & `zipline.py-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:52:33.444472 zipline.py-0.8.0/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.8.0/LICENSE
--rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:52:33.444306 zipline.py-0.8.0/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.8.0/README.md
--rw-r--r--   0 rdrescher   (501) staff       (20)      879 2023-07-28 08:52:12.000000 zipline.py-0.8.0/pyproject.toml
--rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-07-28 08:52:33.444512 zipline.py-0.8.0/setup.cfg
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:52:33.443139 zipline.py-0.8.0/zipline/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-07-28 08:52:03.000000 zipline.py-0.8.0/zipline/__init__.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    22979 2023-07-28 08:51:33.000000 zipline.py-0.8.0/zipline/client.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1261 2023-07-18 18:11:05.000000 zipline.py-0.8.0/zipline/enums.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1851 2023-07-18 18:48:18.000000 zipline.py-0.8.0/zipline/errors.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    15314 2023-07-18 18:11:05.000000 zipline.py-0.8.0/zipline/models.py
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:52:33.444084 zipline.py-0.8.0/zipline.py.egg-info/
--rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:52:33.000000 zipline.py-0.8.0/zipline.py.egg-info/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-07-28 08:52:33.000000 zipline.py-0.8.0/zipline.py.egg-info/SOURCES.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-07-28 08:52:33.000000 zipline.py-0.8.0/zipline.py.egg-info/dependency_links.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-07-28 08:52:33.000000 zipline.py-0.8.0/zipline.py.egg-info/requires.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-07-28 08:52:33.000000 zipline.py-0.8.0/zipline.py.egg-info/top_level.txt
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.367167 zipline.py-0.8.1/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.8.1/LICENSE
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:54:07.367038 zipline.py-0.8.1/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.8.1/README.md
+-rw-r--r--   0 rdrescher   (501) staff       (20)      879 2023-07-28 08:53:44.000000 zipline.py-0.8.1/pyproject.toml
+-rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-07-28 08:54:07.367205 zipline.py-0.8.1/setup.cfg
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.366285 zipline.py-0.8.1/zipline/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-07-28 08:53:39.000000 zipline.py-0.8.1/zipline/__init__.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    22979 2023-07-28 08:51:33.000000 zipline.py-0.8.1/zipline/client.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1261 2023-07-18 18:11:05.000000 zipline.py-0.8.1/zipline/enums.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1851 2023-07-18 18:48:18.000000 zipline.py-0.8.1/zipline/errors.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    15314 2023-07-18 18:11:05.000000 zipline.py-0.8.1/zipline/models.py
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-28 08:54:07.366856 zipline.py-0.8.1/zipline.py.egg-info/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2007 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/SOURCES.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/dependency_links.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/requires.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-07-28 08:54:07.000000 zipline.py-0.8.1/zipline.py.egg-info/top_level.txt
```

### Comparing `zipline.py-0.8.0/LICENSE` & `zipline.py-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.0/PKG-INFO` & `zipline.py-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.8.0
+Version: 0.8.1
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `zipline.py-0.8.0/pyproject.toml` & `zipline.py-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zipline.py"
-version = "0.8.0"
+version = "0.8.1"
 description = "An async wrapper for the Zipline api."
 readme = "README.md"
 authors = [{ name = "fretgfr", email = "fretgfr@sudomail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zipline.py-0.8.0/zipline/__init__.py` & `zipline.py-0.8.1/zipline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from .errors import *
 from .models import *
 
 __title__ = "zipline.py"
 __author__ = "fretgfr"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 fretgfr"
-__version__ = "0.8.0"
+__version__ = "0.8.1"
```

### Comparing `zipline.py-0.8.0/zipline/client.py` & `zipline.py-0.8.1/zipline/client.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.0/zipline/enums.py` & `zipline.py-0.8.1/zipline/enums.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.0/zipline/errors.py` & `zipline.py-0.8.1/zipline/errors.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.0/zipline/models.py` & `zipline.py-0.8.1/zipline/models.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.8.0/zipline.py.egg-info/PKG-INFO` & `zipline.py-0.8.1/zipline.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.8.0
+Version: 0.8.1
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

