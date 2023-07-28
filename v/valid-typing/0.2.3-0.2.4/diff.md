# Comparing `tmp/valid_typing-0.2.3.tar.gz` & `tmp/valid_typing-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valid_typing-0.2.3.tar", last modified: Thu Feb  3 11:01:46 2022, max compression
+gzip compressed data, was "valid_typing-0.2.4.tar", last modified: Fri Jul 28 15:11:11 2023, max compression
```

## Comparing `valid_typing-0.2.3.tar` & `valid_typing-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 11:01:46.018752 valid_typing-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-02-03 11:01:37.000000 valid_typing-0.2.3/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)      662 2022-02-03 11:01:46.018752 valid_typing-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-02-03 11:01:37.000000 valid_typing-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-02-03 11:01:46.019752 valid_typing-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      731 2022-02-03 11:01:37.000000 valid_typing-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 11:01:46.017752 valid_typing-0.2.3/valid_typing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-03 11:01:37.000000 valid_typing-0.2.3/valid_typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2022-02-03 11:01:37.000000 valid_typing-0.2.3/valid_typing/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2022-02-03 11:01:37.000000 valid_typing-0.2.3/valid_typing/check_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2022-02-03 11:01:37.000000 valid_typing-0.2.3/valid_typing/realize_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-03 11:01:46.018752 valid_typing-0.2.3/valid_typing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2022-02-03 11:01:45.000000 valid_typing-0.2.3/valid_typing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      326 2022-02-03 11:01:45.000000 valid_typing-0.2.3/valid_typing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 11:01:45.000000 valid_typing-0.2.3/valid_typing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 11:01:45.000000 valid_typing-0.2.3/valid_typing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       13 2022-02-03 11:01:45.000000 valid_typing-0.2.3/valid_typing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:11.384410 valid_typing-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-28 15:11:03.000000 valid_typing-0.2.4/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-28 15:11:11.384410 valid_typing-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-28 15:11:03.000000 valid_typing-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-28 15:11:11.385410 valid_typing-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-07-28 15:11:03.000000 valid_typing-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:11.383410 valid_typing-0.2.4/valid_typing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 15:11:03.000000 valid_typing-0.2.4/valid_typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-28 15:11:03.000000 valid_typing-0.2.4/valid_typing/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-07-28 15:11:03.000000 valid_typing-0.2.4/valid_typing/check_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-28 15:11:03.000000 valid_typing-0.2.4/valid_typing/realize_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:11.384410 valid_typing-0.2.4/valid_typing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-28 15:11:11.000000 valid_typing-0.2.4/valid_typing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-28 15:11:11.000000 valid_typing-0.2.4/valid_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 15:11:11.000000 valid_typing-0.2.4/valid_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 15:11:11.000000 valid_typing-0.2.4/valid_typing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 15:11:11.000000 valid_typing-0.2.4/valid_typing.egg-info/top_level.txt
```

### Comparing `valid_typing-0.2.3/LICENCE.txt` & `valid_typing-0.2.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `valid_typing-0.2.3/PKG-INFO` & `valid_typing-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valid_typing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple typing validator
 Home-page: https://gitlab.com/WilliamWCYoung/valid-typing
 Author: William Young
 Author-email: william.w.c.young@hotmail.com
 License: MIT
 Download-URL: https://gitlab.com/WilliamWCYoung/valid-typing/-/archive/0.1.0/valid-typing-0.1.0.tar.gz
 Platform: UNKNOWN
```

### Comparing `valid_typing-0.2.3/setup.py` & `valid_typing-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="valid_typing",
-    version="0.2.3",
+    version="0.2.4",
     description="A simple typing validator",
     long_description=long_description,
     url="https://gitlab.com/WilliamWCYoung/valid-typing",
     author="William Young",
     author_email="william.w.c.young@hotmail.com",
     license="MIT",
     packages=["valid_typing"],
```

### Comparing `valid_typing-0.2.3/valid_typing/check_type.py` & `valid_typing-0.2.4/valid_typing/check_type.py`

 * *Files identical despite different names*

### Comparing `valid_typing-0.2.3/valid_typing/realize_types.py` & `valid_typing-0.2.4/valid_typing/realize_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,24 @@
     if mapping is None:
         mapping = {}
 
     if isinstance(definition, typing.TypeVar):
         mapping[definition] = actual
 
     if hasattr(actual, "__origin__") and hasattr(definition, "__origin__"):
-        for i in range(len(actual.__args__)):
-            mapping = generate_mapping(
-                actual.__args__[i], definition.__args__[i], mapping=mapping
-            )
+        if len(actual.__args__) == len(definition.__args__):
+            for i in range(len(actual.__args__)):
+                mapping = generate_mapping(
+                    actual.__args__[i], definition.__args__[i], mapping=mapping
+                )
+        else:
+            for i in range(len(definition.__args__)):
+                mapping = generate_mapping(
+                    actual, definition.__args__[i], mapping=mapping
+                )
     return mapping
 
 
 def realize_types(actual, definition, return_hint):
     assert check_type(actual, definition)
 
     mapping = generate_mapping(actual, definition)
```

### Comparing `valid_typing-0.2.3/valid_typing.egg-info/PKG-INFO` & `valid_typing-0.2.4/valid_typing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valid-typing
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple typing validator
 Home-page: https://gitlab.com/WilliamWCYoung/valid-typing
 Author: William Young
 Author-email: william.w.c.young@hotmail.com
 License: MIT
 Download-URL: https://gitlab.com/WilliamWCYoung/valid-typing/-/archive/0.1.0/valid-typing-0.1.0.tar.gz
 Platform: UNKNOWN
```

