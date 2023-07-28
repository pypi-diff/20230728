# Comparing `tmp/agentshell-0.0.2.tar.gz` & `tmp/agentshell-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentshell-0.0.2.tar", last modified: Fri Jul 28 01:28:23 2023, max compression
+gzip compressed data, was "agentshell-0.0.4.tar", last modified: Fri Jul 28 02:19:15 2023, max compression
```

## Comparing `agentshell-0.0.2.tar` & `agentshell-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.710068 agentshell-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 01:28:12.000000 agentshell-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 01:28:23.710068 agentshell-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 01:28:12.000000 agentshell-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.706068 agentshell-0.0.2/agentshell/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.706068 agentshell-0.0.2/agentshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:28:23.710068 agentshell-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-28 01:28:12.000000 agentshell-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 02:19:04.000000 agentshell-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 02:19:15.981243 agentshell-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 02:19:04.000000 agentshell-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/agentshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-28 02:19:04.000000 agentshell-0.0.4/agentshell/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:19:15.981243 agentshell-0.0.4/agentshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 02:19:15.000000 agentshell-0.0.4/agentshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:19:15.981243 agentshell-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 02:19:04.000000 agentshell-0.0.4/setup.py
```

### Comparing `agentshell-0.0.2/LICENSE` & `agentshell-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.2/PKG-INFO` & `agentshell-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.2
+Version: 0.0.4
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentshell-0.0.2/README.md` & `agentshell-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.2/agentshell/__init__.py` & `agentshell-0.0.4/agentshell/__init__.py`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.2/agentshell/action.py` & `agentshell-0.0.4/agentshell/action.py`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.2/agentshell/main.py` & `agentshell-0.0.4/agentshell/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Returns:
     str: The unique identifier of the current shell.
     """
 
     current_shell = get_memories("shell", "shell", filter_metadata={"current": "True"})
 
     if len(current_shell) == 0:
-        shell_id = create_memory("shell", "shell", metadata={"current": "True"})
+        shell_id = create_memory("shell", "shell", metadata={"current": "True", "cwd": os.getcwd()})
     else:
         current_shell = current_shell[0]
         shell_id = current_shell["id"]
 
     return shell_id
```

### Comparing `agentshell-0.0.2/agentshell.egg-info/PKG-INFO` & `agentshell-0.0.4/agentshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.2
+Version: 0.0.4
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentshell-0.0.2/setup.py` & `agentshell-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentshell",
-    version="0.0.2",
+    version="0.0.4",
     description="A shell for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentshell",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["agentshell"],
-    install_requires=["agentmemory"],
+    install_requires=["agentmemory", "easycompletion"],
     readme="README.md",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: POSIX :: Linux",
```

