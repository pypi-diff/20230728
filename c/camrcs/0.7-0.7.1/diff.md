# Comparing `tmp/camrcs-0.7.tar.gz` & `tmp/camrcs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camrcs-0.7.tar", last modified: Thu Jul 27 13:08:46 2023, max compression
+gzip compressed data, was "camrcs-0.7.1.tar", last modified: Fri Jul 28 10:33:05 2023, max compression
```

## Comparing `camrcs-0.7.tar` & `camrcs-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.612685 camrcs-0.7/
--rw-rw-r--   0 niek      (1000) niek      (1000)     1524 2023-07-27 13:08:46.608685 camrcs-0.7/PKG-INFO
--rw-rw-r--   0 niek      (1000) niek      (1000)      895 2023-07-25 07:38:12.000000 camrcs-0.7/README.md
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.608685 camrcs-0.7/camrcs.egg-info/
--rw-rw-r--   0 niek      (1000) niek      (1000)     1524 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/PKG-INFO
--rw-rw-r--   0 niek      (1000) niek      (1000)      362 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/SOURCES.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/dependency_links.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/entry_points.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       19 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/requires.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        7 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/top_level.txt
--rw-r--r--   0 niek      (1000) niek      (1000)     9764 2023-07-27 13:01:35.000000 camrcs-0.7/camrcs.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.608685 camrcs-0.7/docs/
--rw-rw-r--   0 niek      (1000) niek      (1000)      634 2023-07-20 06:51:26.000000 camrcs-0.7/docs/Makefile
--rw-rw-r--   0 niek      (1000) niek      (1000)     1195 2023-07-24 12:10:28.000000 camrcs-0.7/docs/about.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     2696 2023-07-26 10:04:11.000000 camrcs-0.7/docs/archiving.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     1930 2023-07-26 09:59:43.000000 camrcs-0.7/docs/conf.py
--rw-rw-r--   0 niek      (1000) niek      (1000)      296 2023-07-26 10:03:30.000000 camrcs-0.7/docs/data_pre.csv
--rw-rw-r--   0 niek      (1000) niek      (1000)      585 2023-07-26 09:56:52.000000 camrcs-0.7/docs/index.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     1051 2023-07-26 10:07:35.000000 camrcs-0.7/docs/installation.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)      795 2023-07-20 06:51:26.000000 camrcs-0.7/docs/make.bat
--rw-rw-r--   0 niek      (1000) niek      (1000)      272 2023-07-26 10:02:35.000000 camrcs-0.7/docs/requirements.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-27 13:08:46.612685 camrcs-0.7/setup.cfg
--rw-r--r--   0 niek      (1000) niek      (1000)     1196 2023-07-27 13:03:59.000000 camrcs-0.7/setup.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-28 10:33:05.851755 camrcs-0.7.1/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1547 2023-07-28 10:33:05.851755 camrcs-0.7.1/PKG-INFO
+-rw-rw-r--   0 niek      (1000) niek      (1000)      916 2023-07-27 13:21:36.000000 camrcs-0.7.1/README.md
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-28 10:33:05.851755 camrcs-0.7.1/camrcs.egg-info/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1547 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/PKG-INFO
+-rw-rw-r--   0 niek      (1000) niek      (1000)      362 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/entry_points.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       19 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/requires.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        7 2023-07-28 10:33:05.000000 camrcs-0.7.1/camrcs.egg-info/top_level.txt
+-rw-r--r--   0 niek      (1000) niek      (1000)    10809 2023-07-28 10:20:51.000000 camrcs-0.7.1/camrcs.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-28 10:33:05.851755 camrcs-0.7.1/docs/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      634 2023-07-20 06:51:26.000000 camrcs-0.7.1/docs/Makefile
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1195 2023-07-24 12:10:28.000000 camrcs-0.7.1/docs/about.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     2696 2023-07-26 10:04:11.000000 camrcs-0.7.1/docs/archiving.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1932 2023-07-28 10:12:52.000000 camrcs-0.7.1/docs/conf.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)      296 2023-07-26 10:03:30.000000 camrcs-0.7.1/docs/data_pre.csv
+-rw-rw-r--   0 niek      (1000) niek      (1000)      585 2023-07-26 09:56:52.000000 camrcs-0.7.1/docs/index.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1171 2023-07-28 10:32:02.000000 camrcs-0.7.1/docs/installation.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)      795 2023-07-20 06:51:26.000000 camrcs-0.7.1/docs/make.bat
+-rw-rw-r--   0 niek      (1000) niek      (1000)      272 2023-07-26 10:02:35.000000 camrcs-0.7.1/docs/requirements.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-28 10:33:05.855754 camrcs-0.7.1/setup.cfg
+-rw-r--r--   0 niek      (1000) niek      (1000)     1198 2023-07-28 10:12:48.000000 camrcs-0.7.1/setup.py
```

### Comparing `camrcs-0.7/PKG-INFO` & `camrcs-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camrcs
-Version: 0.7
+Version: 0.7.1
 Summary: A package for management of Cambridge Research Cold Storage backups
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: MIT
 Project-URL: Documentation, https://camrcs.readthedocs.io
 Project-URL: Source, https://github.com/niekwit/camrcs
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Topic :: System :: Archiving :: Backup
 Description-Content-Type: text/markdown
 
 # CAMRCS
 
 `camrcs` is a Python package that manages data backups to Cambridge University Research Cold Storage (RCS).
 
-Complete documentation can be found [here](https://camrcs.readthedocs.io).
+Complete documentation can be found [here](https://camrcs.readthedocs.io/en/stable/index.html).
 
 ## QUICKSTART
 
 ### Installation
 
 Install `pigz` first:
```

### Comparing `camrcs-0.7/README.md` & `camrcs-0.7.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # CAMRCS
 
 `camrcs` is a Python package that manages data backups to Cambridge University Research Cold Storage (RCS).
 
-Complete documentation can be found [here](https://camrcs.readthedocs.io).
+Complete documentation can be found [here](https://camrcs.readthedocs.io/en/stable/index.html).
 
 ## QUICKSTART
 
 ### Installation
 
 Install `pigz` first:
```

### Comparing `camrcs-0.7/camrcs.egg-info/PKG-INFO` & `camrcs-0.7.1/camrcs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camrcs
-Version: 0.7
+Version: 0.7.1
 Summary: A package for management of Cambridge Research Cold Storage backups
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: MIT
 Project-URL: Documentation, https://camrcs.readthedocs.io
 Project-URL: Source, https://github.com/niekwit/camrcs
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Topic :: System :: Archiving :: Backup
 Description-Content-Type: text/markdown
 
 # CAMRCS
 
 `camrcs` is a Python package that manages data backups to Cambridge University Research Cold Storage (RCS).
 
-Complete documentation can be found [here](https://camrcs.readthedocs.io).
+Complete documentation can be found [here](https://camrcs.readthedocs.io/en/stable/index.html).
 
 ## QUICKSTART
 
 ### Installation
 
 Install `pigz` first:
```

### Comparing `camrcs-0.7/camrcs.py` & `camrcs-0.7.1/camrcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import numpy as np
 import subprocess
 import hashlib
 from pathlib import Path
 from datetime import datetime
 import time
 import timeit
+import glob
 
-VERSION = 0.7
+VERSION = "0.7.1"
 
 #get current working dir
 cdir = os.getcwd()
  
 
 ####Python functions####
 
@@ -74,14 +75,40 @@
     #format time
     ty_res = time.gmtime(total_time)
     res = time.strftime("%H:%M:%S",ty_res)
     
     click.echo(f"Total run time: {res}")
 
 
+#adapted from https://stackoverflow.com/questions/2104080/how-do-i-check-file-size-in-python#2104083
+def convert_bytes(num):
+    '''this function will convert bytes to MB.... GB... etc
+    '''
+    
+    for x in ['bytes', 'KB', 'MB', 'GB', 'TB']:
+        
+        if num < 1024.0:
+            
+            return f'{num:.1f} {x}'
+        
+        num /= 1024.0
+
+
+def file_size(archive):
+    '''calculates total size of split archive files
+    '''
+    
+    #calculate total size of list of files
+    file_list = glob.glob(f"{archive}.part-*")
+    size =  sum(os.path.getsize(f) for f in file_list if os.path.isfile(f))
+    
+    return convert_bytes(size)
+
+
+
 ####command line parser####
 @click.group()
 
 def cli():
     '''Management of data backups to/from Cambridge University Research Cold Storage (RCS)
     '''
 
@@ -107,15 +134,15 @@
     start = timeit.default_timer()
     
     #create empty data.csv if requested        
     if csv:
         
         click.secho("Creating new data.csv", fg="green")
         
-        header = "id,crsid,project_dir,date_up,date_down,temp_path,target_dir,remote_dest_dir,chunk_size,exclude_dir,md5sum_up,md5sum_down,download_dir,version"
+        header = "id,crsid,project_dir,date_up,date_down,temp_path,target_dir,remote_dest_dir,chunk_size,exclude_dir,md5sum_up,md5sum_down,archive_size,download_dir,version"
 
         #write to file
         with open(os.path.join(cdir,"data.csv"), "w") as text_file:
             
             print(header, file=text_file)
             
         return
@@ -187,15 +214,15 @@
             #get md5sum from text file
             if run(tar):
                 
                 Path(os.path.join(f"{archive}.split.done")).touch()
                 
                 with open(md5sum_file) as f:
                     md5sum_up = f.readline().split("  ")[0]
-                    
+                
                 #remove md5sum file
                 os.remove(md5sum_file)
                     
         else:
             
             click.echo(f"{archive} has been created and split before...")
             
@@ -207,19 +234,27 @@
         rsync = f"rsync -v -h --progress $(ls {archive}.part-*) {crsid}@rcs.uis.cam.ac.uk:{project_dir}/{remote_dest_dir}" 
                
         if run(rsync):
             
             #update csv
             csv.at[index,"md5sum_up"] = md5sum_up
             csv.at[index,"date_up"] = str(datetime.now().astimezone())
-            csv.at[index,"version"] = VERSION
+            
+            try: #these columns might not exist if data.csv was created with older version of camrcs
+                
+                csv.at[index,"version"] = VERSION
+                csv.at[index,"archive_size"] = file_size(archive)
+            
+            except KeyError: #just print to console
+                
+                click.echo(f"Total archive size is {file_size(archive)}")
                       
         
-    #update csv with md5sum hash/date
-    update_csv(csv)
+        #update csv with md5sum hash/date
+        update_csv(csv)
                 
     #remove archive and split archive files
     if not keep:
     
         click.echo("Removing all archive files...")
         remove = f"rm -r {archive}*"
     
@@ -363,8 +398,7 @@
 cli.add_command(version)
 
 
 
 
 
 
-
```

### Comparing `camrcs-0.7/docs/Makefile` & `camrcs-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `camrcs-0.7/docs/about.rst` & `camrcs-0.7.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `camrcs-0.7/docs/archiving.rst` & `camrcs-0.7.1/docs/archiving.rst`

 * *Files identical despite different names*

### Comparing `camrcs-0.7/docs/conf.py` & `camrcs-0.7.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'camrcs'
 copyright = '2023, Niek Wit'
 author = 'Niek Wit'
 
 # The full version, including alpha/beta/rc tags
-release = '0.7'
+release = '0.7.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `camrcs-0.7/docs/index.rst` & `camrcs-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `camrcs-0.7/docs/installation.rst` & `camrcs-0.7.1/docs/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,22 @@
    
    $ pip install camrcs
 
 
 This will install the most recent stable version of `camrcs`.
 
 
+To update ``camrcs`` to the latest stable version:
+
+.. code-block:: console
+   
+   $ pip install camrcs --upgrade
+   
+
+
 pigz
 =======================
 
 ``camrcs`` uses ``pigz`` for data compression
 
 Debian-based GNU/Linux
 -----------------------
```

### Comparing `camrcs-0.7/docs/make.bat` & `camrcs-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `camrcs-0.7/setup.py` & `camrcs-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='camrcs',
-    version='0.7',
+    version='0.7.1',
     py_modules=['camrcs'], 
     description='A package for management of Cambridge Research Cold Storage backups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls={
         'Documentation': 'https://camrcs.readthedocs.io',
         'Source': 'https://github.com/niekwit/camrcs',
```

