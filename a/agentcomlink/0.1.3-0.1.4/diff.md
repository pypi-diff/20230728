# Comparing `tmp/agentcomlink-0.1.3.tar.gz` & `tmp/agentcomlink-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcomlink-0.1.3.tar", last modified: Fri Jul 28 08:49:48 2023, max compression
+gzip compressed data, was "agentcomlink-0.1.4.tar", last modified: Fri Jul 28 16:00:31 2023, max compression
```

## Comparing `agentcomlink-0.1.3.tar` & `agentcomlink-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:49:48.263963 agentcomlink-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 08:49:48.263963 agentcomlink-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:49:48.263963 agentcomlink-0.1.3/agentcomlink/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/agentcomlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/agentcomlink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/agentcomlink/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/agentcomlink/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/agentcomlink/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:49:48.263963 agentcomlink-0.1.3/agentcomlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 08:49:48.000000 agentcomlink-0.1.3/agentcomlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 08:49:48.000000 agentcomlink-0.1.3/agentcomlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:49:48.000000 agentcomlink-0.1.3/agentcomlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 08:49:48.000000 agentcomlink-0.1.3/agentcomlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 08:49:48.000000 agentcomlink-0.1.3/agentcomlink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:49:48.263963 agentcomlink-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 08:49:38.000000 agentcomlink-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/agentcomlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/agentcomlink/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/agentcomlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 16:00:31.000000 agentcomlink-0.1.4/agentcomlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:00:31.145665 agentcomlink-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 16:00:18.000000 agentcomlink-0.1.4/setup.py
```

### Comparing `agentcomlink-0.1.3/LICENSE` & `agentcomlink-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.3/PKG-INFO` & `agentcomlink-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-Metadata-Version: 2.1
-Name: agentcomlink
-Version: 0.1.3
-Summary: Simple chat, debug and file management panel for agents
-Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
-Author: Moon
-Author-email: shawmakesmagic@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+# agentcomlink <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a>
 
 Simple file management and serving for agents
 
+<img src="resources/image.jpg">
+
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentcomlink/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentcomlink/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentcomlink.svg)](https://badge.fury.io/py/agentcomlink)
 
 # Installation
 
 ```bash
 pip install agentcomlink
 ```
 
 ## Quickstart
 
 1. **Start the server**:
-You can start the server with uvicorn like this:
+   You can start the server with uvicorn like this:
+
 ```python
 import os
 
 if __name__ == "__main__":
     import uvicorn
     uvicorn.run("agentcomlink:start_server", host="0.0.0.0", port=int(os.getenv("PORT", 8000)))
 ```
+
 This will start the server at `http://localhost:8000`.
 
 2. **Get a file**:
    Once the server is up and running, you can retrieve file content by sending a GET request to `/file/{path}` endpoint, where `{path}` is the path to the file relative to the server's current storage directory.
 
 ```python
 from agentcomlink import get_file
@@ -203,14 +192,34 @@
 
 ```python
 from agentcomlink import list_files
 
 files = list_files()
 ```
 
+### `list_files_formatted(path='.')`
+
+Lists all files in the specified directory as a formatted string. Convenient!
+
+**Arguments**:
+
+- `path` (str, optional): The path to the directory. Defaults to `'.'` (current directory).
+
+**Returns**:
+
+- A string containing a list of file names in the specified directory.
+
+**Example**:
+
+```python
+from agentcomlink import list_files
+
+files = list_files()
+```
+
 ### `get_file(path)`
 
 Returns the content of the file at the specified path.
 
 **Arguments**:
 
 - `path` (str): The path to the file.
@@ -227,7 +236,8 @@
 content = get_file("test.txt")
 ```
 
 # Contributions Welcome
 
 If you like this library and want to contribute in any way, please feel free to submit a PR and I will review it. Please note that the goal here is simplicity and accesibility, using common language and few dependencies.
 
+<img src="resources/youcreatethefuture.jpg">
```

### Comparing `agentcomlink-0.1.3/agentcomlink/__init__.py` & `agentcomlink-0.1.4/agentcomlink/__init__.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.3/agentcomlink/files.py` & `agentcomlink-0.1.4/agentcomlink/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,13 +39,23 @@
     return True
 
 
 def list_files(path="."):
     check_files()
     return os.listdir(os.path.join(storage_path, path))  # Returns the list of files
 
+def list_files_formatted(path="."):
+    check_files()
+    files = os.listdir(os.path.join(storage_path, path))
+    files_formatted = []
+    for file in files:
+        if os.path.isdir(os.path.join(storage_path, path, file)):
+            files_formatted.append(file + "/")
+        else:
+            files_formatted.append(file)
+    return "User's Files:\n" + "\n".join(files_formatted)
 
 def get_file(path):
     check_files()
     with open(os.path.join(storage_path, path), "r") as f:  # 'r' for reading
         content = f.read()
     return content
```

### Comparing `agentcomlink-0.1.3/agentcomlink/page.py` & `agentcomlink-0.1.4/agentcomlink/page.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.3/agentcomlink/server.py` & `agentcomlink-0.1.4/agentcomlink/server.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.3/agentcomlink.egg-info/PKG-INFO` & `agentcomlink-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,31 +16,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Simple file management and serving for agents
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentcomlink/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentcomlink/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentcomlink.svg)](https://badge.fury.io/py/agentcomlink)
+
 # Installation
 
 ```bash
 pip install agentcomlink
 ```
 
 ## Quickstart
 
 1. **Start the server**:
-You can start the server with uvicorn like this:
+   You can start the server with uvicorn like this:
+
 ```python
 import os
 
 if __name__ == "__main__":
     import uvicorn
     uvicorn.run("agentcomlink:start_server", host="0.0.0.0", port=int(os.getenv("PORT", 8000)))
 ```
+
 This will start the server at `http://localhost:8000`.
 
 2. **Get a file**:
    Once the server is up and running, you can retrieve file content by sending a GET request to `/file/{path}` endpoint, where `{path}` is the path to the file relative to the server's current storage directory.
 
 ```python
 from agentcomlink import get_file
@@ -201,14 +206,34 @@
 
 **Example**:
 
 ```python
 from agentcomlink import list_files
 
 files = list_files()
+```
+
+### `list_files_formatted(path='.')`
+
+Lists all files in the specified directory as a formatted string. Convenient!
+
+**Arguments**:
+
+- `path` (str, optional): The path to the directory. Defaults to `'.'` (current directory).
+
+**Returns**:
+
+- A string containing a list of file names in the specified directory.
+
+**Example**:
+
+```python
+from agentcomlink import list_files
+
+files = list_files()
 ```
 
 ### `get_file(path)`
 
 Returns the content of the file at the specified path.
 
 **Arguments**:
```

### Comparing `agentcomlink-0.1.3/setup.py` & `agentcomlink-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentcomlink',
-    version='0.1.3',
+    version='0.1.4',
     description='Simple chat, debug and file management panel for agents',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentcomlink',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

