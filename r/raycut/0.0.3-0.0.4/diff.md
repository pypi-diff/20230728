# Comparing `tmp/raycut-0.0.3.tar.gz` & `tmp/raycut-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raycut-0.0.3.tar", last modified: Fri Jul 28 05:56:11 2023, max compression
+gzip compressed data, was "raycut-0.0.4.tar", last modified: Fri Jul 28 06:16:48 2023, max compression
```

## Comparing `raycut-0.0.3.tar` & `raycut-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 05:56:11.743009 raycut-0.0.3/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 05:56:11.743009 raycut-0.0.3/PKG-INFO
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 05:56:11.739009 raycut-0.0.3/raycut/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2500 2023-07-28 05:55:42.000000 raycut-0.0.3/raycut/__init__.py
-drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 05:56:11.743009 raycut-0.0.3/raycut.egg-info/
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 05:56:11.000000 raycut-0.0.3/raycut.egg-info/PKG-INFO
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-28 05:56:11.000000 raycut-0.0.3/raycut.egg-info/SOURCES.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-28 05:56:11.000000 raycut-0.0.3/raycut.egg-info/dependency_links.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-28 05:56:11.000000 raycut-0.0.3/raycut.egg-info/requires.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-28 05:56:11.000000 raycut-0.0.3/raycut.egg-info/top_level.txt
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-28 05:56:11.743009 raycut-0.0.3/setup.cfg
--rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-28 05:55:31.000000 raycut-0.0.3/setup.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.916745 raycut-0.0.4/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:16:48.912743 raycut-0.0.4/PKG-INFO
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.912743 raycut-0.0.4/raycut/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)     2625 2023-07-28 06:16:15.000000 raycut-0.0.4/raycut/__init__.py
+drwxrwxr-x   0 d33tah    (1000) d33tah    (1000)        0 2023-07-28 06:16:48.912743 raycut-0.0.4/raycut.egg-info/
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      533 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/PKG-INFO
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      176 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/SOURCES.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        1 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/dependency_links.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       10 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/requires.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)        7 2023-07-28 06:16:48.000000 raycut-0.0.4/raycut.egg-info/top_level.txt
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)       38 2023-07-28 06:16:48.916745 raycut-0.0.4/setup.cfg
+-rw-rw-r--   0 d33tah    (1000) d33tah    (1000)      689 2023-07-28 06:16:26.000000 raycut-0.0.4/setup.py
```

### Comparing `raycut-0.0.3/PKG-INFO` & `raycut-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.3
+Version: 0.0.4
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.3/raycut/__init__.py` & `raycut-0.0.4/raycut/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,38 +52,44 @@
     - ray stop
     - ray start --head --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml --dashboard-host=0.0.0.0
 worker_start_ray_commands:
     - ray stop
     - ray start --address=$RAY_HEAD_IP:6379 --object-manager-port=8076
 '''
 
+
 def init(aws_access_key_id, aws_secret_access_key):
-    subprocess.check_call('mkdir -p ~/.aws && pip install boto3 ray && apt update && apt install rsync -y', shell=True)
+    subprocess.check_call(
+        'mkdir -p ~/.aws', shell=True)
+    subprocess.check_call('pip install boto3 ray', shell=True)
+    subprocess.check_call('apt update && apt install rsync -y', shell=True)
 
     p = pathlib.Path('~/.aws/').expanduser()
     try:
-        (p / 'credentials').rename( p / f'credentials_backup_{time.time()}')
+        (p / 'credentials').rename(p / f'credentials_backup_{time.time()}')
     except FileNotFoundError:
         pass
     with open(p / 'credentials', 'w') as f:
         f.write(f'''
         # added by raycut
         [default]
         aws_access_key_id = {aws_access_key_id}
         aws_secret_access_key = {aws_secret_access_key}
         ''')
 
     with open('example.yaml', 'w') as f:
         f.write(yaml)
 
     subprocess.check_call('ray up example.yaml --yes', shell=True)
-    subprocess.check_call('ray attach -p 10001 example.yaml', shell=True)
-    ray.init(address=f'ray://localhost:10001')
+    p = subprocess.Popen('ray attach -p 10001 example.yaml', shell=True)
+    ray.init(address='ray://localhost:10001')
 
     class cls:
         def run(self, f):
             return ray.get([f.remote()])
 
         def teardown(self):
+            p.kill()
+            p.wait()
             subprocess.check_call('ray down example.yaml --yes', shell=True)
 
     return cls()
```

### Comparing `raycut-0.0.3/raycut.egg-info/PKG-INFO` & `raycut-0.0.4/raycut.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raycut
-Version: 0.0.3
+Version: 0.0.4
 Summary: A convenience library for Ray that allows you to run a function on a remote
 Home-page: http://github.com/d33tah/raycut
 Author: Jacek "d33tah" Wielemborek
 Author-email: d33tah@gmail.com
 License: WTFPL
 
 A convenience library for Ray that allows you to run a function on a remote
```

### Comparing `raycut-0.0.3/setup.py` & `raycut-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 a remote instance with a single function call.
 '''
 
 from setuptools import setup
 
 setup(
     name='raycut',
-    version='0.0.3',
+    version='0.0.4',
     description=__doc__,
     long_description=long_description,
     url='http://github.com/d33tah/raycut',
     author='Jacek "d33tah" Wielemborek',
     author_email='d33tah@gmail.com',
     license='WTFPL',
     packages=['raycut'],
```

