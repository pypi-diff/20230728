# Comparing `tmp/agentloop-0.1.4.tar.gz` & `tmp/agentloop-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentloop-0.1.4.tar", last modified: Tue Jul 18 14:03:58 2023, max compression
+gzip compressed data, was "agentloop-0.1.5.tar", last modified: Fri Jul 28 11:10:45 2023, max compression
```

## Comparing `agentloop-0.1.4.tar` & `agentloop-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 14:03:46.000000 agentloop-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 14:03:58.948129 agentloop-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-18 14:03:46.000000 agentloop-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/agentloop/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-18 14:03:46.000000 agentloop-0.1.4/agentloop/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:03:58.948129 agentloop-0.1.4/agentloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 14:03:58.000000 agentloop-0.1.4/agentloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:03:58.948129 agentloop-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-18 14:03:46.000000 agentloop-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 11:10:35.000000 agentloop-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-28 11:10:45.307945 agentloop-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-28 11:10:35.000000 agentloop-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/agentloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/agentloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:10:45.307945 agentloop-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-28 11:10:35.000000 agentloop-0.1.5/setup.py
```

### Comparing `agentloop-0.1.4/LICENSE` & `agentloop-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentloop-0.1.4/PKG-INFO` & `agentloop-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -12,19 +12,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# agentloop
 
 A simple, lightweight loop for your agent. Start/stop, step-through, and more.
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentloop.svg)](https://badge.fury.io/py/agentloop)
+
 # Quickstart
 
 ```python
 from agentloop import start, stop
 
 def step_one(next_output, loop_data):
     print("step_one")
```

### Comparing `agentloop-0.1.4/README.md` & `agentloop-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-# agentloop
+# agentloop <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a>
 
 A simple, lightweight loop for your agent. Start/stop, step-through, and more.
 
 <img src="resources/image.jpg">
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentloop.svg)](https://badge.fury.io/py/agentloop)
+
 # Quickstart
 
 ```python
 from agentloop import start, stop
 
 def step_one(next_output, loop_data):
     print("step_one")
```

### Comparing `agentloop-0.1.4/agentloop/input.py` & `agentloop-0.1.5/agentloop/input.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-def step_with_input_key(loop_data, input_key=None):
+from .loop import stop
+
+def step_with_input_key(loop_data):
     """
     Listen for a specified key press, and when detected, step the loop
 
     Args:
         loop_data: loop data object, created by the start function
         input_key: The keyboard key which the listener will react to
             Defaults to keyboard.Key.space
@@ -15,19 +17,25 @@
         from pynput import keyboard as _keyboard
         keyboard = _keyboard
     except ImportError:
         raise ImportError(
             "pynput not installed. Please install it with `pip install pynput`"
         )
 
-    if input_key is None:
-        input_key = keyboard.Key.space
+    input_key = keyboard.Key.space
+
+    quit_key = "q"
 
     def on_press(key):
-        if key == input_key:
+        # check if key includes the quit key
+        if hasattr(key, "char") and key.char == quit_key:
+            print("Quitting...")
+            stop(loop_data)
+        elif key == input_key:
+            print("Stepping...")
             loop_data["step_event"].set()
 
     listener = None
     listener = keyboard.Listener(on_press=on_press)
     listener.start()
     loop_data["listener"] = listener
     return loop_data
```

### Comparing `agentloop-0.1.4/agentloop/loop.py` & `agentloop-0.1.5/agentloop/loop.py`

 * *Files identical despite different names*

### Comparing `agentloop-0.1.4/agentloop.egg-info/PKG-INFO` & `agentloop-0.1.5/agentloop.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -12,19 +12,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# agentloop
 
 A simple, lightweight loop for your agent. Start/stop, step-through, and more.
 
 
+[![Lint and Test](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml/badge.svg)](https://github.com/AutonomousResearchGroup/agentloop/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/agentloop.svg)](https://badge.fury.io/py/agentloop)
+
 # Quickstart
 
 ```python
 from agentloop import start, stop
 
 def step_one(next_output, loop_data):
     print("step_one")
```

### Comparing `agentloop-0.1.4/setup.py` & `agentloop-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentloop",
-    version="0.1.4",
+    version="0.1.5",
     description="A simple, lightweight loop for your agent.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentloop",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

