# Comparing `tmp/speakleash-0.2.1.tar.gz` & `tmp/speakleash-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.2.1.tar", last modified: Tue Jul  4 18:46:39 2023, max compression
+gzip compressed data, was "speakleash-0.2.3.tar", last modified: Fri Jul 28 08:46:27 2023, max compression
```

## Comparing `speakleash-0.2.1.tar` & `speakleash-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:46:39.605762 speakleash-0.2.1/
--rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.2.1/LICENSE
--rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-04 18:46:39.605464 speakleash-0.2.1/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)     1995 2023-06-09 19:57:52.000000 speakleash-0.2.1/README.md
--rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-07-04 18:46:39.605857 speakleash-0.2.1/setup.cfg
--rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-07-04 18:46:27.000000 speakleash-0.2.1/setup.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:46:39.602940 speakleash-0.2.1/speakleash/
--rw-r--r--   0 skondracki   (502) staff       (20)    10109 2023-07-04 18:45:49.000000 speakleash-0.2.1/speakleash/__init__.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:46:39.605031 speakleash-0.2.1/speakleash.egg-info/
--rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-04 18:46:39.000000 speakleash-0.2.1/speakleash.egg-info/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-07-04 18:46:39.000000 speakleash-0.2.1/speakleash.egg-info/SOURCES.txt
--rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-07-04 18:46:39.000000 speakleash-0.2.1/speakleash.egg-info/dependency_links.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-07-04 18:46:39.000000 speakleash-0.2.1/speakleash.egg-info/requires.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-07-04 18:46:39.000000 speakleash-0.2.1/speakleash.egg-info/top_level.txt
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-28 08:46:27.763456 speakleash-0.2.3/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.2.3/LICENSE
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-28 08:46:27.763143 speakleash-0.2.3/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)     1995 2023-06-09 19:57:52.000000 speakleash-0.2.3/README.md
+-rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-07-28 08:46:27.763556 speakleash-0.2.3/setup.cfg
+-rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-07-28 08:46:18.000000 speakleash-0.2.3/setup.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-28 08:46:27.760971 speakleash-0.2.3/speakleash/
+-rw-r--r--   0 skondracki   (502) staff       (20)    10236 2023-07-28 08:42:37.000000 speakleash-0.2.3/speakleash/__init__.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-28 08:46:27.762667 speakleash-0.2.3/speakleash.egg-info/
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-28 08:46:27.000000 speakleash-0.2.3/speakleash.egg-info/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-07-28 08:46:27.000000 speakleash-0.2.3/speakleash.egg-info/SOURCES.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-07-28 08:46:27.000000 speakleash-0.2.3/speakleash.egg-info/dependency_links.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-07-28 08:46:27.000000 speakleash-0.2.3/speakleash.egg-info/requires.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-07-28 08:46:27.000000 speakleash-0.2.3/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.2.1/LICENSE` & `speakleash-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.2.1/PKG-INFO` & `speakleash-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.2.1
+Version: 0.2.3
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `speakleash-0.2.1/README.md` & `speakleash-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `speakleash-0.2.1/setup.py` & `speakleash-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="speakleash",
-    version="0.2.1",
+    version="0.2.3",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages = ["speakleash"],
```

### Comparing `speakleash-0.2.1/speakleash/__init__.py` & `speakleash-0.2.3/speakleash/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,19 +180,23 @@
         names = StructureDownloader(replicate_dir).get_structure(url + structure_file)
 
         if names:      
             for item in names:
                 if "name" in item:
                     self.datasets.append(SpeakleashDataset(item["name"], url, self.replicate_dir))
 
-    def get(self, name):
-        for d in self.datasets:
-            if d.name == name:
-                return d
-        return None
+    def get(self, name, url = None):
+
+        if url:
+            return SpeakleashDataset(name, url, self.replicate_dir)
+        else:
+            for d in self.datasets:
+                if d.name == name:
+                    return d
+            return None
 
 class SpeakleashDataset(object):
 
     def __init__(self, name, url, replicate_dir):
         self.url = url
         self.name = name
         self.replicate_dir = replicate_dir
```

### Comparing `speakleash-0.2.1/speakleash.egg-info/PKG-INFO` & `speakleash-0.2.3/speakleash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.2.1
+Version: 0.2.3
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

