# Comparing `tmp/agentshell-0.0.1.tar.gz` & `tmp/agentshell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentshell-0.0.1.tar", last modified: Fri Jul 28 01:15:03 2023, max compression
+gzip compressed data, was "agentshell-0.0.2.tar", last modified: Fri Jul 28 01:28:23 2023, max compression
```

## Comparing `agentshell-0.0.1.tar` & `agentshell-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:15:03.803925 agentshell-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 01:14:52.000000 agentshell-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-28 01:15:03.803925 agentshell-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-28 01:14:52.000000 agentshell-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:15:03.803925 agentshell-0.0.1/agentshell/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 01:14:52.000000 agentshell-0.0.1/agentshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-28 01:14:52.000000 agentshell-0.0.1/agentshell/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-28 01:14:52.000000 agentshell-0.0.1/agentshell/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:15:03.803925 agentshell-0.0.1/agentshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-28 01:15:03.000000 agentshell-0.0.1/agentshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 01:15:03.000000 agentshell-0.0.1/agentshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:15:03.000000 agentshell-0.0.1/agentshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 01:15:03.000000 agentshell-0.0.1/agentshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 01:15:03.000000 agentshell-0.0.1/agentshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:15:03.803925 agentshell-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-28 01:14:52.000000 agentshell-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.710068 agentshell-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 01:28:12.000000 agentshell-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 01:28:23.710068 agentshell-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-28 01:28:12.000000 agentshell-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.706068 agentshell-0.0.2/agentshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-28 01:28:12.000000 agentshell-0.0.2/agentshell/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:28:23.706068 agentshell-0.0.2/agentshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 01:28:23.000000 agentshell-0.0.2/agentshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:28:23.710068 agentshell-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-28 01:28:12.000000 agentshell-0.0.2/setup.py
```

### Comparing `agentshell-0.0.1/LICENSE` & `agentshell-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentshell-0.0.1/PKG-INFO` & `agentshell-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.1
+Version: 0.0.2
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 
 ```bash
 pip install agentshell
 ```
 
 # Documentation
 
-## `get_files_in_current_directory(shell_id=None)`
+## `get_files_in_cwd(shell_id=None)`
 
 Returns a list of files in the current directory of a specific shell. If `shell_id` is not specified, uses the current shell.
 
 **Parameters:**
 
 - `shell_id`: The unique identifier of the shell.
```

### Comparing `agentshell-0.0.1/README.md` & `agentshell-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```bash
 pip install agentshell
 ```
 
 # Documentation
 
-## `get_files_in_current_directory(shell_id=None)`
+## `get_files_in_cwd(shell_id=None)`
 
 Returns a list of files in the current directory of a specific shell. If `shell_id` is not specified, uses the current shell.
 
 **Parameters:**
 
 - `shell_id`: The unique identifier of the shell.
```

### Comparing `agentshell-0.0.1/agentshell/action.py` & `agentshell-0.0.2/agentshell/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from easycompletion import compose_function, compose_prompt
 
-from agentshell.main import get_files_in_current_directory, run_command
+from agentshell.main import get_files_in_cwd, run_command
 
 
 use_shell_prompt = """TIME: {{current_time}}
 DATE: {{current_date}}
 PLATFORM: {{platform}}
 PROJECT DIRECTORY: {{cwd}}
 PWD: {{cwd}}
@@ -21,15 +21,15 @@
 """
 
 
 def compose_use_shell_prompt(context):
     context["files_in_current_directory"] = (
         "\n" + "Files in the current directory (ls -alh):\n"
         "============================================\n"
-        "" + ("\n".join(get_files_in_current_directory())) + "\n"
+        "" + ("\n".join(get_files_in_cwd())) + "\n"
         "============================================\n"
     )
 
     return compose_prompt(use_shell_prompt, context)
 
 
 def use_shell(arguments):
```

### Comparing `agentshell-0.0.1/agentshell/main.py` & `agentshell-0.0.2/agentshell/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     get_memories,
     get_memory,
     update_memory,
     wipe_category,
 )
 
 
-def get_files_in_current_directory(shell_id=None):
+def get_files_in_cwd(shell_id=None):
     """
     Returns a list of files in the current directory of a specific shell.
-    
+
     Parameters:
     shell_id (str): The unique identifier of the shell. If not specified, uses the current shell.
-    
+
     Returns:
     list: A list of filenames in the current directory.
     """
 
     if shell_id is None:
         shell_id = get_current_shell()
     shell = get_memory("shell", shell_id)
@@ -37,19 +37,19 @@
     # result_decoded = result_decoded[:-1]
     return result_decoded
 
 
 def get_current_shell():
     """
     Returns the unique identifier of the current shell. If no shell is currently active, creates a new shell and returns its identifier.
-    
+
     Returns:
     str: The unique identifier of the current shell.
     """
-     
+
     current_shell = get_memories("shell", "shell", filter_metadata={"current": "True"})
 
     if len(current_shell) == 0:
         shell_id = create_memory("shell", "shell", metadata={"current": "True"})
     else:
         current_shell = current_shell[0]
         shell_id = current_shell["id"]
@@ -149,17 +149,25 @@
     command (str): The command that was executed.
     success (bool): Whether the command was successful.
     output (str): The output of the command.
     error (str): Any error messages produced by the command.
     """
 
     timestamp = time.time()
+
+    formatted_memory = """\
+    Command: {command}
+    Timestamp: {timestamp}
+    Success: {success}
+    Output: {output}
+    Error: {error}"""
+
     create_memory(
         "shell_history",
-        shell_id,
+        formatted_memory,
         metadata={
             "shell_id": shell_id,
             "command": command,
             "success": success,
             "output": output or "",
             "error": error or "",
             "timestamp": timestamp,
@@ -249,15 +257,15 @@
     Parameters:
     command (str): The command to execute.
     shell_id (str): The unique identifier of the shell. If not specified, uses the current shell.
 
     Returns:
     bool: True if the command was successful, False otherwise.
     """
-    
+
     if shell_id is None:
         shell_id = get_current_shell()
     shell = get_memory("shell", shell_id)
     cwd = shell["metadata"]["cwd"]
     # Execute command in the current working directory
     command_to_run = f"cd {cwd} && {command}"
     process = subprocess.run(command_to_run, shell=True, text=True, capture_output=True)
```

### Comparing `agentshell-0.0.1/agentshell.egg-info/PKG-INFO` & `agentshell-0.0.2/agentshell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentshell
-Version: 0.0.1
+Version: 0.0.2
 Summary: A shell for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentshell
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 
 ```bash
 pip install agentshell
 ```
 
 # Documentation
 
-## `get_files_in_current_directory(shell_id=None)`
+## `get_files_in_cwd(shell_id=None)`
 
 Returns a list of files in the current directory of a specific shell. If `shell_id` is not specified, uses the current shell.
 
 **Parameters:**
 
 - `shell_id`: The unique identifier of the shell.
```

### Comparing `agentshell-0.0.1/setup.py` & `agentshell-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentshell",
-    version="0.0.1",
+    version="0.0.2",
     description="A shell for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentshell",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

