# Comparing `tmp/michaelPanPrintLib-0.0.1.tar.gz` & `tmp/michaelPanPrintLib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michaelPanPrintLib-0.0.1.tar", last modified: Fri Jul 28 05:33:41 2023, max compression
+gzip compressed data, was "michaelPanPrintLib-0.0.2.tar", last modified: Fri Jul 28 06:10:17 2023, max compression
```

## Comparing `michaelPanPrintLib-0.0.1.tar` & `michaelPanPrintLib-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 05:33:41.114979 michaelPanPrintLib-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-28 02:35:25.000000 michaelPanPrintLib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1489 2023-07-28 05:33:41.113982 michaelPanPrintLib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-07-28 05:31:47.000000 michaelPanPrintLib-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 05:33:41.112985 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/
--rw-rw-rw-   0        0        0     1489 2023-07-28 05:33:41.000000 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-28 05:33:41.000000 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 05:33:41.000000 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 05:33:41.000000 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 05:33:41.000000 michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 05:33:41.114979 michaelPanPrintLib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-07-28 05:32:45.000000 michaelPanPrintLib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:10:17.307742 michaelPanPrintLib-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-28 02:35:25.000000 michaelPanPrintLib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1504 2023-07-28 06:10:17.306744 michaelPanPrintLib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-07-28 05:31:47.000000 michaelPanPrintLib-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 06:10:17.301758 michaelPanPrintLib-0.0.2/michaelPanPrintLib/
+-rw-rw-rw-   0        0        0      100 2023-07-28 06:09:42.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib/__init__.py
+-rw-rw-rw-   0        0        0     1799 2023-07-28 02:32:46.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib/change_print.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:10:17.305747 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/
+-rw-rw-rw-   0        0        0     1504 2023-07-28 06:10:17.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-28 06:10:17.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 06:10:17.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 06:10:17.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-28 06:10:17.000000 michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 06:10:17.307742 michaelPanPrintLib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      732 2023-07-28 06:10:07.000000 michaelPanPrintLib-0.0.2/setup.py
```

### Comparing `michaelPanPrintLib-0.0.1/LICENSE` & `michaelPanPrintLib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `michaelPanPrintLib-0.0.1/PKG-INFO` & `michaelPanPrintLib-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: michaelPanPrintLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: change output style
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
+Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Changing the console output style library
```

### Comparing `michaelPanPrintLib-0.0.1/README.md` & `michaelPanPrintLib-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `michaelPanPrintLib-0.0.1/michaelPanPrintLib.egg-info/PKG-INFO` & `michaelPanPrintLib-0.0.2/michaelPanPrintLib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: michaelPanPrintLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: change output style
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
+Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Changing the console output style library
```

### Comparing `michaelPanPrintLib-0.0.1/setup.py` & `michaelPanPrintLib-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="michaelPanPrintLib",  # 库的名称
-    version="0.0.1",  # 库的版本号
+    version="0.0.2",  # 库的版本号
     author="chuntong pan",  # 库的作者
     author_email="panzhang1314@gmail.com",  # 作者邮箱
     description="change output style",  # 库的简述
+    install_requires=['colorama'],  # 需要的依赖库
     long_description=long_description,
     long_description_content_type="text/markdown",
+    platforms=["all"],
     packages=setuptools.find_packages(),
     classifiers=["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
-    install_requires=['colorama']
 )
```

