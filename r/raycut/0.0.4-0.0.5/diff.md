# Comparing `tmp/raycut-0.0.4.tar.gz` & `tmp/raycut-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raycut-0.0.4.tar", last modified: Fri Jul 28 06:16:48 2023, max compression
+gzip compressed data, was "raycut-0.0.5.tar", last modified: Fri Jul 28 06:35:03 2023, max compression
```

## Comparing `raycut-0.0.4.tar` & `raycut-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.916745 raycut-0.0.4/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:16:48.912743 raycut-0.0.4/PKG-INFO
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.912743 raycut-0.0.4/raycut/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2625 2023-07-28 06:16:15.000000 raycut-0.0.4/raycut/__init__.py
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.912743 raycut-0.0.4/raycut.egg-info/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/PKG-INFO
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/SOURCES.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/dependency_links.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/requires.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/top_level.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-28 06:16:48.916745 raycut-0.0.4/setup.cfg
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-28 06:16:26.000000 raycut-0.0.4/setup.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:35:03.912167 raycut-0.0.5/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:35:03.912167 raycut-0.0.5/PKG-INFO
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:35:03.912167 raycut-0.0.5/raycut/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2631 2023-07-28 06:34:16.000000 raycut-0.0.5/raycut/__init__.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:35:03.912167 raycut-0.0.5/raycut.egg-info/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:35:03.000000 raycut-0.0.5/raycut.egg-info/PKG-INFO
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-28 06:35:03.000000 raycut-0.0.5/raycut.egg-info/SOURCES.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-28 06:35:03.000000 raycut-0.0.5/raycut.egg-info/dependency_links.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-28 06:35:03.000000 raycut-0.0.5/raycut.egg-info/requires.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-28 06:35:03.000000 raycut-0.0.5/raycut.egg-info/top_level.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-28 06:35:03.912167 raycut-0.0.5/setup.cfg
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-28 06:34:29.000000 raycut-0.0.5/setup.py
```

### Comparing `raycut-0.0.4/PKG-INFO` & `raycut-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.4
+Version: 0.0.5
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.4/raycut/__init__.py` & `raycut-0.0.5/raycut/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         aws_secret_access_key = {aws_secret_access_key}
         ''')
 
     with open('example.yaml', 'w') as f:
         f.write(yaml)
 
     subprocess.check_call('ray up example.yaml --yes', shell=True)
-    p = subprocess.Popen('ray attach -p 10001 example.yaml', shell=True)
+    p = subprocess.Popen('nohup ray attach -p 10001 example.yaml', shell=True)
     ray.init(address='ray://localhost:10001')
 
     class cls:
         def run(self, f):
             return ray.get([f.remote()])
 
         def teardown(self):
```

### Comparing `raycut-0.0.4/raycut.egg-info/PKG-INFO` & `raycut-0.0.5/raycut.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.4
+Version: 0.0.5
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.4/setup.py` & `raycut-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 a remote instance with a single function call.
 '''
 
 from setuptools import setup
 
 setup(
     name='raycut',
-    version='0.0.4',
+    version='0.0.5',
     description=__doc__,
     long_description=long_description,
     url='http://github.com/d33tah/raycut',
     author='Jacek "d33tah" Wielemborek',
     author_email='d33tah@gmail.com',
     license='WTFPL',
     packages=['raycut'],
```

