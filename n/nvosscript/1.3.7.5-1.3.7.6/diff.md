# Comparing `tmp/nvosscript-1.3.7.5.tar.gz` & `tmp/nvosscript-1.3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.7.5.tar", last modified: Mon Jul 17 08:14:14 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.6.tar", last modified: Fri Jul 28 08:11:59 2023, max compression
```

## Comparing `nvosscript-1.3.7.5.tar` & `nvosscript-1.3.7.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.902410 nvosscript-1.3.7.5/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.5/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-17 08:14:14.902037 nvosscript-1.3.7.5/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.5/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.877526 nvosscript-1.3.7.5/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.5/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.5/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.5/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.5/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.886992 nvosscript-1.3.7.5/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-17 08:14:14.000000 nvosscript-1.3.7.5/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-17 08:14:14.902466 nvosscript-1.3.7.5/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-17 08:13:24.000000 nvosscript-1.3.7.5/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.890119 nvosscript-1.3.7.5/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.5/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.5/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      748 2023-07-17 07:08:02.000000 nvosscript-1.3.7.5/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3083 2023-07-17 08:12:44.000000 nvosscript-1.3.7.5/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.900531 nvosscript-1.3.7.5/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.5/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.5/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-17 08:13:33.000000 nvosscript-1.3.7.5/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.5/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-17 08:14:14.901351 nvosscript-1.3.7.5/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.5/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.725454 nvosscript-1.3.7.6/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.6/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-28 08:11:59.725060 nvosscript-1.3.7.6/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.6/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.712880 nvosscript-1.3.7.6/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.6/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.6/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8854 2023-07-28 08:11:34.000000 nvosscript-1.3.7.6/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.6/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.716845 nvosscript-1.3.7.6/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-28 08:11:59.000000 nvosscript-1.3.7.6/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-28 08:11:59.725516 nvosscript-1.3.7.6/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-28 08:11:57.000000 nvosscript-1.3.7.6/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.719899 nvosscript-1.3.7.6/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.6/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.6/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      748 2023-07-17 07:08:02.000000 nvosscript-1.3.7.6/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3083 2023-07-17 08:12:44.000000 nvosscript-1.3.7.6/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.723513 nvosscript-1.3.7.6/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.6/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.6/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-28 08:11:54.000000 nvosscript-1.3.7.6/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.6/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-28 08:11:59.724348 nvosscript-1.3.7.6/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.6/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.7.5/LICENSE` & `nvosscript-1.3.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/nvos/file.py` & `nvosscript-1.3.7.6/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/nvos/remote.py` & `nvosscript-1.3.7.6/nvos/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,14 @@
         while True:
             time.sleep(1)
             time_count += 1
             progress.update(global_var - addition)
             addition = global_var
             if (global_var == len(upload_list) or global_var >= len(upload_list) - 20):
                 break
-            if time_count == 60:
-                break
 
 
 def uploading_file(workspace_path, file):
 
     global global_var
 
     get_current_env()
```

### Comparing `nvosscript-1.3.7.5/nvos/run.py` & `nvosscript-1.3.7.6/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/setup.py` & `nvosscript-1.3.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.7.05',
+    version='1.3.7.06',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.7.5/skyeye/loghandler.py` & `nvosscript-1.3.7.6/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/skyeye/remote.py` & `nvosscript-1.3.7.6/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/start/login.py` & `nvosscript-1.3.7.6/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/start/main.py` & `nvosscript-1.3.7.6/start/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.7.05")
+        print("1.3.7.06")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.7.5/start/utils.py` & `nvosscript-1.3.7.6/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.5/win/win_auto_script.py` & `nvosscript-1.3.7.6/win/win_auto_script.py`

 * *Files identical despite different names*

