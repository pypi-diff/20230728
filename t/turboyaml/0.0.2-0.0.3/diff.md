# Comparing `tmp/turboyaml-0.0.2.tar.gz` & `tmp/turboyaml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboyaml-0.0.2.tar", last modified: Fri Jul 28 02:54:25 2023, max compression
+gzip compressed data, was "turboyaml-0.0.3.tar", last modified: Fri Jul 28 03:03:40 2023, max compression
```

## Comparing `turboyaml-0.0.2.tar` & `turboyaml-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.099517 turboyaml-0.0.2/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.2/LICENSE
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5689 2023-07-28 02:54:25.099332 turboyaml-0.0.2/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5116 2023-07-28 02:27:59.000000 turboyaml-0.0.2/README.md
--rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-07-28 02:54:25.099587 turboyaml-0.0.2/setup.cfg
--rw-r--r--   0 fredbrowne   (501) staff       (20)      914 2023-07-28 02:09:59.000000 turboyaml-0.0.2/setup.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.098470 turboyaml-0.0.2/turboyaml/
--rw-r--r--   0 fredbrowne   (501) staff       (20)       22 2023-07-28 02:21:13.000000 turboyaml-0.0.2/turboyaml/__init__.py
--rw-r--r--   0 fredbrowne   (501) staff       (20)     9193 2023-07-28 02:27:09.000000 turboyaml-0.0.2/turboyaml/cli.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 02:54:25.099159 turboyaml-0.0.2/turboyaml.egg-info/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5689 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)      265 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/entry_points.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       15 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/requires.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-07-28 02:54:25.000000 turboyaml-0.0.2/turboyaml.egg-info/top_level.txt
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.374927 turboyaml-0.0.3/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.3/LICENSE
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5970 2023-07-28 03:03:40.374802 turboyaml-0.0.3/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5397 2023-07-28 02:57:28.000000 turboyaml-0.0.3/README.md
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-07-28 03:03:40.374967 turboyaml-0.0.3/setup.cfg
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      939 2023-07-28 03:02:30.000000 turboyaml-0.0.3/setup.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.373439 turboyaml-0.0.3/turboyaml/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       22 2023-07-28 02:21:13.000000 turboyaml-0.0.3/turboyaml/__init__.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     9193 2023-07-28 02:27:09.000000 turboyaml-0.0.3/turboyaml/cli.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.374611 turboyaml-0.0.3/turboyaml.egg-info/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5970 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      265 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/entry_points.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       29 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/requires.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/top_level.txt
```

### Comparing `turboyaml-0.0.2/LICENSE` & `turboyaml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turboyaml-0.0.2/PKG-INFO` & `turboyaml-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboyaml
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.
 Home-page: https://github.com/fredbrowne/turboyaml
 Author: Fred Setra
 Author-email: fred.setra@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -104,14 +104,17 @@
 
 turboyaml is open-source software licensed under the MIT License.
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
+- 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
+
+
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
 
 ## Disclaimer
```

### Comparing `turboyaml-0.0.2/README.md` & `turboyaml-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 
 turboyaml is open-source software licensed under the MIT License.
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
+- 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
+
+
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
 
 ## Disclaimer
```

### Comparing `turboyaml-0.0.2/setup.py` & `turboyaml-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="turboyaml",
-    version="0.0.2",
+    version="0.0.3",
     author="Fred Setra",
     author_email="fred.setra@gmail.com",
     description="An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredbrowne/turboyaml",
     packages=find_packages(),
     install_requires=[
         "openai==0.27.8",
+        "pyyaml==6.0.1",
     ],
     entry_points={
         "console_scripts": [
             "turboyaml=turboyaml.cli:main",
         ],
     },
     classifiers=[
```

### Comparing `turboyaml-0.0.2/turboyaml/cli.py` & `turboyaml-0.0.3/turboyaml/cli.py`

 * *Files identical despite different names*

### Comparing `turboyaml-0.0.2/turboyaml.egg-info/PKG-INFO` & `turboyaml-0.0.3/turboyaml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboyaml
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.
 Home-page: https://github.com/fredbrowne/turboyaml
 Author: Fred Setra
 Author-email: fred.setra@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -104,14 +104,17 @@
 
 turboyaml is open-source software licensed under the MIT License.
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
+- 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
+
+
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
 
 ## Disclaimer
```

