# Comparing `tmp/agentcomlink-0.1.4.tar.gz` & `tmp/agentcomlink-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcomlink-0.1.4.tar", last modified: Fri Jul 28 16:00:31 2023, max compression
+gzip compressed data, was "agentcomlink-0.1.5.tar", last modified: Fri Jul 28 17:00:50 2023, max compression
```

## Comparing `agentcomlink-0.1.4.tar` & `agentcomlink-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/agentcomlink/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/agentcomlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:00:50.920958 agentcomlink-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 17:00:50.920958 agentcomlink-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:00:50.920958 agentcomlink-0.1.5/agentcomlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/agentcomlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/agentcomlink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/agentcomlink/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/agentcomlink/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/agentcomlink/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:00:50.920958 agentcomlink-0.1.5/agentcomlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 17:00:50.000000 agentcomlink-0.1.5/agentcomlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 17:00:50.000000 agentcomlink-0.1.5/agentcomlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:00:50.000000 agentcomlink-0.1.5/agentcomlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 17:00:50.000000 agentcomlink-0.1.5/agentcomlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:00:50.000000 agentcomlink-0.1.5/agentcomlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:00:50.920958 agentcomlink-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 17:00:40.000000 agentcomlink-0.1.5/setup.py
```

### Comparing `agentcomlink-0.1.4/LICENSE` & `agentcomlink-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.4/PKG-INFO` & `agentcomlink-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.4/README.md` & `agentcomlink-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.4/agentcomlink/__init__.py` & `agentcomlink-0.1.5/agentcomlink/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from .files import (
     get_storage_path,
     set_storage_path,
     add_file,
     remove_file,
     update_file,
     list_files,
+    list_files_formatted,
     get_file,
 )
-from .server import start_server, get_server, set_storage_path, send_message, register_message_handler, unregister_message_handler
+from .server import (
+    start_server,
+    get_server,
+    set_storage_path,
+    send_message,
+    register_message_handler,
+    unregister_message_handler,
+)
 
 __all__ = [
     "get_storage_path",
     "start_server",
     "send_message",
     "register_message_handler",
     "unregister_message_handler",
     "get_server",
     "set_storage_path",
     "add_file",
     "remove_file",
     "update_file",
     "list_files",
+    "list_files_formatted",
     "get_file",
 ]
```

### Comparing `agentcomlink-0.1.4/agentcomlink/files.py` & `agentcomlink-0.1.5/agentcomlink/files.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.4/agentcomlink/page.py` & `agentcomlink-0.1.5/agentcomlink/page.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.4/agentcomlink.egg-info/PKG-INFO` & `agentcomlink-0.1.5/agentcomlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.4/setup.py` & `agentcomlink-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentcomlink',
-    version='0.1.4',
+    version='0.1.5',
     description='Simple chat, debug and file management panel for agents',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentcomlink',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

