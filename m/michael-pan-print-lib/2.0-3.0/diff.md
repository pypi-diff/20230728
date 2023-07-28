# Comparing `tmp/michael-pan-print-lib-2.0.tar.gz` & `tmp/michael-pan-print-lib-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michael-pan-print-lib-2.0.tar", last modified: Fri Jul 28 03:07:28 2023, max compression
+gzip compressed data, was "michael-pan-print-lib-3.0.tar", last modified: Fri Jul 28 03:18:43 2023, max compression
```

## Comparing `michael-pan-print-lib-2.0.tar` & `michael-pan-print-lib-3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 03:07:28.119882 michael-pan-print-lib-2.0/
--rw-rw-rw-   0        0        0     1092 2023-07-28 02:35:25.000000 michael-pan-print-lib-2.0/LICENSE
--rw-rw-rw-   0        0        0     2067 2023-07-28 03:07:28.119882 michael-pan-print-lib-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1621 2023-07-28 02:32:58.000000 michael-pan-print-lib-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 03:07:28.118886 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/
--rw-rw-rw-   0        0        0     2067 2023-07-28 03:07:28.000000 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-28 03:07:28.000000 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 03:07:28.000000 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 03:07:28.000000 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 03:07:28.000000 michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 03:07:28.120880 michael-pan-print-lib-2.0/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-07-28 03:07:15.000000 michael-pan-print-lib-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:18:43.776778 michael-pan-print-lib-3.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-28 02:35:25.000000 michael-pan-print-lib-3.0/LICENSE
+-rw-rw-rw-   0        0        0     1992 2023-07-28 03:18:43.776778 michael-pan-print-lib-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1621 2023-07-28 02:32:58.000000 michael-pan-print-lib-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 03:18:43.775781 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/
+-rw-rw-rw-   0        0        0     1992 2023-07-28 03:18:43.000000 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-28 03:18:43.000000 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:18:43.000000 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 03:18:43.000000 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:18:43.000000 michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 03:18:43.776778 michael-pan-print-lib-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      711 2023-07-28 03:18:32.000000 michael-pan-print-lib-3.0/setup.py
```

### Comparing `michael-pan-print-lib-2.0/LICENSE` & `michael-pan-print-lib-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `michael-pan-print-lib-2.0/PKG-INFO` & `michael-pan-print-lib-3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: michael-pan-print-lib
-Version: 2.0
+Version: 3.0
 Summary: change output style
-Home-page: https://github.com/p110120p1/Logistics
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 改变控制台输出样式库(Changing the console output style library)
 
 ## 1.简介(Introduction)
```

### Comparing `michael-pan-print-lib-2.0/README.md` & `michael-pan-print-lib-3.0/README.md`

 * *Files identical despite different names*

### Comparing `michael-pan-print-lib-2.0/michael_pan_print_lib.egg-info/PKG-INFO` & `michael-pan-print-lib-3.0/michael_pan_print_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: michael-pan-print-lib
-Version: 2.0
+Version: 3.0
 Summary: change output style
-Home-page: https://github.com/p110120p1/Logistics
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 改变控制台输出样式库(Changing the console output style library)
 
 ## 1.简介(Introduction)
```

### Comparing `michael-pan-print-lib-2.0/setup.py` & `michael-pan-print-lib-3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import setuptools
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="michael-pan-print-lib",  # 库的名称
-    version="2.0",  # 库的版本号
+    version="3.0",  # 库的版本号
     author="chuntong pan",  # 库的作者
     author_email="panzhang1314@gmail.com",  # 作者邮箱
     description="change output style",  # 库的简述
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/p110120p1/Logistics",  # 这个字段好像没在用，可以随意写
     packages=setuptools.find_packages(),
-    python_requires='>=3.8',
     classifiers=["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
     install_requires=['colorama==0.4.6']
 )
```

