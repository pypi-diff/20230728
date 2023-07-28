# Comparing `tmp/taipy-templates-2.4.0.dev0.tar.gz` & `tmp/taipy-templates-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-templates-2.4.0.dev0.tar", last modified: Fri Jul 21 12:21:02 2023, max compression
+gzip compressed data, was "taipy-templates-3.0.0.dev0.tar", last modified: Fri Jun 23 10:12:23 2023, max compression
```

## Comparing `taipy-templates-2.4.0.dev0.tar` & `taipy-templates-3.0.0.dev0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.104243 taipy-templates-2.4.0.dev0/src/taipy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.108243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/page_1.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/page_1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/page_2.md
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/page_2.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/root.md
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/root.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
--rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 12:20:47.000000 taipy-templates-2.4.0.dev0/src/taipy/templates/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:21:02.112243 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-21 12:21:02.000000 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-21 12:21:02.000000 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:21:02.000000 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:20:54.000000 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 12:21:02.000000 taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.772085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/page_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_1/page_1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/page_2.md
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/page_2/page_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/root.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   411212 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/src/taipy/templates/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-23 10:12:23.000000 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-23 10:12:23.000000 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:12:23.000000 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:12:17.000000 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:12:23.000000 taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:12:23.776085 taipy-templates-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-23 10:12:10.000000 taipy-templates-3.0.0.dev0/tests/test_templates.py
```

### Comparing `taipy-templates-2.4.0.dev0/LICENSE` & `taipy-templates-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/PKG-INFO` & `taipy-templates-3.0.0.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-templates
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: An open-source package holding Taipy application templates.
 Home-page: https://github.com/avaiga/taipy-templates
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-templates
 Classifier: Intended Audience :: Developers
@@ -41,21 +41,19 @@
   - [Code of conduct](#code-of-conduct)
   - [Directory Structure](#directory-structure)
 
 ## What is Taipy templates
 
 Taipy is a Python library for creating Business Applications. More information on our [website](https://www.taipy.io).
 
-Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps
-users getting started with a simple and ready-to-go application.
+Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps users getting started with a simple and ready-to-go application.
 
 A more in depth documentation of taipy can be found [here](https://docs.taipy.io).
 
-To create a Taipy application using this template, first you need to install Taipy (>= 2.3). Then from a terminal,
-run the following command.
+To create a Taipy application using this template, first you need to install Taipy (> 2.2). Then from a terminal, run the following command.
 ```
 $ taipy create
 ```
 or
 ```
 $ taipy create --template "default"
 ```
@@ -68,12 +66,12 @@
 
 ## Code of conduct
 
 Want to be part of the _Taipy_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
-- `src/taipy/templates/`: Contains each template in a dedicated sub-folder.
+- `src/taipy/templates/`: Contains each template in a dedicated sub-folder with the following structure:
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy_.
 - `LICENSE`: The Apache 2.0 License.
 - `README.md`: Current file.
```

### Comparing `taipy-templates-2.4.0.dev0/README.md` & `taipy-templates-3.0.0.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,19 @@
   - [Code of conduct](#code-of-conduct)
   - [Directory Structure](#directory-structure)
 
 ## What is Taipy templates
 
 Taipy is a Python library for creating Business Applications. More information on our [website](https://www.taipy.io).
 
-Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps
-users getting started with a simple and ready-to-go application.
+Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps users getting started with a simple and ready-to-go application.
 
 A more in depth documentation of taipy can be found [here](https://docs.taipy.io).
 
-To create a Taipy application using this template, first you need to install Taipy (>= 2.3). Then from a terminal,
-run the following command.
+To create a Taipy application using this template, first you need to install Taipy (> 2.2). Then from a terminal, run the following command.
 ```
 $ taipy create
 ```
 or
 ```
 $ taipy create --template "default"
 ```
@@ -47,12 +45,12 @@
 
 ## Code of conduct
 
 Want to be part of the _Taipy_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
-- `src/taipy/templates/`: Contains each template in a dedicated sub-folder.
+- `src/taipy/templates/`: Contains each template in a dedicated sub-folder with the following structure:
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy_.
 - `LICENSE`: The Apache 2.0 License.
 - `README.md`: Current file.
```

### Comparing `taipy-templates-2.4.0.dev0/setup.py` & `taipy-templates-3.0.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/hooks/post_gen_project.py` & `taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}` & `taipy-templates-3.0.0.dev0/src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/hooks/post_gen_project.py` & `taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg` & `taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}` & `taipy-templates-3.0.0.dev0/src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}`

 * *Files identical despite different names*

### Comparing `taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/PKG-INFO` & `taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-templates
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: An open-source package holding Taipy application templates.
 Home-page: https://github.com/avaiga/taipy-templates
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-templates
 Classifier: Intended Audience :: Developers
@@ -41,21 +41,19 @@
   - [Code of conduct](#code-of-conduct)
   - [Directory Structure](#directory-structure)
 
 ## What is Taipy templates
 
 Taipy is a Python library for creating Business Applications. More information on our [website](https://www.taipy.io).
 
-Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps
-users getting started with a simple and ready-to-go application.
+Taipy templates is a repository that contains templates and scaffoldings created and maintained by Taipy. It helps users getting started with a simple and ready-to-go application.
 
 A more in depth documentation of taipy can be found [here](https://docs.taipy.io).
 
-To create a Taipy application using this template, first you need to install Taipy (>= 2.3). Then from a terminal,
-run the following command.
+To create a Taipy application using this template, first you need to install Taipy (> 2.2). Then from a terminal, run the following command.
 ```
 $ taipy create
 ```
 or
 ```
 $ taipy create --template "default"
 ```
@@ -68,12 +66,12 @@
 
 ## Code of conduct
 
 Want to be part of the _Taipy_ community? Check out our [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) file.
 
 ## Directory Structure
 
-- `src/taipy/templates/`: Contains each template in a dedicated sub-folder.
+- `src/taipy/templates/`: Contains each template in a dedicated sub-folder with the following structure:
 - `CODE_OF_CONDUCT.md`: Code of conduct for members and contributors of _taipy_.
 - `CONTRIBUTING.md`: Instructions to contribute to _taipy_.
 - `LICENSE`: The Apache 2.0 License.
 - `README.md`: Current file.
```

### Comparing `taipy-templates-2.4.0.dev0/src/taipy_templates.egg-info/SOURCES.txt` & `taipy-templates-3.0.0.dev0/src/taipy_templates.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+src/taipy/__init__.py
 src/taipy/templates/version.json
 src/taipy/templates/multi-page-gui/cookiecutter.json
 src/taipy/templates/multi-page-gui/hooks/post_gen_project.py
 src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/requirements.txt
 src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
 src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/__init__.py
 src/taipy/templates/multi-page-gui/{{cookiecutter.application_name}}/pages/root.md
@@ -22,8 +23,9 @@
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/requirements.txt
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/{{cookiecutter.application_main_file}}
 src/taipy/templates/taipy-default-template/{{cookiecutter.application_name}}/images/taipy_logo.jpg
 src/taipy_templates.egg-info/PKG-INFO
 src/taipy_templates.egg-info/SOURCES.txt
 src/taipy_templates.egg-info/dependency_links.txt
 src/taipy_templates.egg-info/not-zip-safe
-src/taipy_templates.egg-info/top_level.txt
+src/taipy_templates.egg-info/top_level.txt
+tests/test_templates.py
```

