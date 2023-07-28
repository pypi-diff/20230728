# Comparing `tmp/agentaction-0.1.3.tar.gz` & `tmp/agentaction-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.3.tar", last modified: Thu Jul 20 11:26:25 2023, max compression
+gzip compressed data, was "agentaction-0.1.4.tar", last modified: Fri Jul 28 02:58:45 2023, max compression
```

## Comparing `agentaction-0.1.3.tar` & `agentaction-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 11:26:05.000000 agentaction-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:26:25.853547 agentaction-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-20 11:26:05.000000 agentaction-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 11:26:05.000000 agentaction-0.1.3/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-20 11:26:05.000000 agentaction-0.1.3/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:26:25.853547 agentaction-0.1.3/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 11:26:25.000000 agentaction-0.1.3/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:26:25.853547 agentaction-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 11:26:05.000000 agentaction-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 02:58:35.000000 agentaction-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 02:58:45.072158 agentaction-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-28 02:58:35.000000 agentaction-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 02:58:35.000000 agentaction-0.1.4/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-28 02:58:35.000000 agentaction-0.1.4/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:58:45.072158 agentaction-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 02:58:35.000000 agentaction-0.1.4/setup.py
```

### Comparing `agentaction-0.1.3/LICENSE` & `agentaction-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.3/PKG-INFO` & `agentaction-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.3
+Version: 0.1.4
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# agentaction
 
 Action chaining and history for agents
 
 
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
 
@@ -135,14 +134,16 @@
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
 ### `get_formatted_actions(search_text: str) -> list`
 Retrieve a dict containing the available actions in several formats
 
+### `get_action_from_memory(action_name) -> dict or None`
+Retrieve an action from memory based on the action's name.
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.3/README.md` & `agentaction-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# agentaction
+# agentaction <a href="https://discord.gg/qetWd7J9De"><img style="float: right" src="https://dcbadge.vercel.app/api/server/qetWd7J9De" alt=""></a>
 
 Action chaining and history for agents
 
 <img src="resources/image.jpg">
 
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
@@ -118,14 +118,16 @@
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
 ### `get_formatted_actions(search_text: str) -> list`
 Retrieve a dict containing the available actions in several formats
 
+### `get_action_from_memory(action_name) -> dict or None`
+Retrieve an action from memory based on the action's name.
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.3/agentaction/__init__.py` & `agentaction-0.1.4/agentaction/__init__.py`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.3/agentaction/main.py` & `agentaction-0.1.4/agentaction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,25 +109,24 @@
         ignored_actions = actions[last_action]["never_after_actions"]
         ignored_action_objects = []
         for action in ignored_actions:
             ignored_action_objects.append(get_action_from_memory(action))
         # check if available_actions contains recommended actions, if not, add them
         for action in recommended_action_objects:
             if action not in available_actions:
-                print("action")
-                print(action)
                 action["recommended"] = True
                 available_actions.append(action)
         # for each action in ignored, delete from available
         for action in ignored_action_objects:
             if action in available_actions:
                 available_actions.remove(action)
 
     return available_actions
 
+
 def get_action_from_memory(action_name):
     """
     Retrieve an action from memory based on the action's name.
 
     Args:
         action_name: The name of the action to retrieve.
 
@@ -240,15 +239,14 @@
     The actions returned are then added to the 'actions' dictionary.
 
     Returns:
     None
     """
 
     actions_dir = os.path.abspath(actions_dir)
-    print("actiond_dir", actions_dir)
     sys.path.insert(0, actions_dir)
 
     for filename in os.listdir(actions_dir):
         if filename.endswith(".py"):
             module_name = filename[:-3]  # filename without .py
             module = importlib.import_module(module_name)
 
@@ -284,15 +282,14 @@
     Returns:
         {
         "available_actions": a list of available actions in memory format
         "formatted_actions": a list of actions as a string
         "short_actions": a list of actions names as a string, comma separated
     }
     """
-    # check if context['summary'] exists
     header_text = "Available actions for me to choose from:"
     available_actions = get_available_actions(search_text, n_results=5)
 
     # sort available_actions so that recommended are first
     # recommended are action["metadata"].get("recommended", None)
     available_actions = sorted(
         available_actions,
```

### Comparing `agentaction-0.1.3/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.4/agentaction.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.3
+Version: 0.1.4
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# agentaction
 
 Action chaining and history for agents
 
 
 # Why Use This?
 This package helps manage and simplify the task of handling actions for an agent, especially a looping agent with chained functions. Actions can be anything, but the intended purpose is to work with openai function calling or other JSON/function calling LLM completion paradigms.
 
@@ -135,14 +134,16 @@
 
 ### `get_available_actions(search_text: str) -> list`
 Retrieves the available actions based on relevance and last action.
 
 ### `get_formatted_actions(search_text: str) -> list`
 Retrieve a dict containing the available actions in several formats
 
+### `get_action_from_memory(action_name) -> dict or None`
+Retrieve an action from memory based on the action's name.
 ### `search_actions(search_text: str, n_results: int=5) -> list`
 Searches for actions based on a query text.
 
 ### `use_action(function_name: str, arguments: dict) -> dict`
 Executes a specific action by its function name.
 
 ### `add_action(name: str, action: dict)`
```

### Comparing `agentaction-0.1.3/setup.py` & `agentaction-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.3",
+    version="0.1.4",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

