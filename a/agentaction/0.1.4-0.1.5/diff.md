# Comparing `tmp/agentaction-0.1.4.tar.gz` & `tmp/agentaction-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentaction-0.1.4.tar", last modified: Fri Jul 28 02:58:45 2023, max compression
+gzip compressed data, was "agentaction-0.1.5.tar", last modified: Fri Jul 28 08:03:22 2023, max compression
```

## Comparing `agentaction-0.1.4.tar` & `agentaction-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 02:58:35.000000 agentaction-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 02:58:45.072158 agentaction-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-28 02:58:35.000000 agentaction-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/agentaction/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 02:58:35.000000 agentaction-0.1.4/agentaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-28 02:58:35.000000 agentaction-0.1.4/agentaction/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:58:45.072158 agentaction-0.1.4/agentaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 02:58:45.000000 agentaction-0.1.4/agentaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:58:45.072158 agentaction-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 02:58:35.000000 agentaction-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 08:03:12.000000 agentaction-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 08:03:22.773369 agentaction-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-28 08:03:12.000000 agentaction-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/agentaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 08:03:12.000000 agentaction-0.1.5/agentaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-28 08:03:12.000000 agentaction-0.1.5/agentaction/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:03:22.773369 agentaction-0.1.5/agentaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 08:03:22.000000 agentaction-0.1.5/agentaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:03:22.773369 agentaction-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 08:03:12.000000 agentaction-0.1.5/setup.py
```

### Comparing `agentaction-0.1.4/LICENSE` & `agentaction-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.4/PKG-INFO` & `agentaction-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.4
+Version: 0.1.5
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentaction-0.1.4/README.md` & `agentaction-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.4/agentaction/__init__.py` & `agentaction-0.1.5/agentaction/__init__.py`

 * *Files identical despite different names*

### Comparing `agentaction-0.1.4/agentaction/main.py` & `agentaction-0.1.5/agentaction/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             The builder is a function which injects data into the template
         values: A dictionary of values to insert into the prompt
 
     Returns:
         A string representing the composed prompt.
     """
     prompt = action["prompt"]
-    builder = action["builder"]
+    builder = action.get("builder", None)
     if builder is not None:
         prompt = builder(values)
     return prompt
 
 
 def get_actions():
     """
```

### Comparing `agentaction-0.1.4/agentaction.egg-info/PKG-INFO` & `agentaction-0.1.5/agentaction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentaction
-Version: 0.1.4
+Version: 0.1.5
 Summary: Action chaining and history for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentaction
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentaction-0.1.4/setup.py` & `agentaction-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentaction",
-    version="0.1.4",
+    version="0.1.5",
     description="Action chaining and history for agents",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentaction",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

