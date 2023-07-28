# Comparing `tmp/nuregi-0.2.0.dev2.tar.gz` & `tmp/nuregi-0.2.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuregi-0.2.0.dev2.tar", last modified: Fri Jul 28 12:05:34 2023, max compression
+gzip compressed data, was "nuregi-0.2.0.dev3.tar", last modified: Fri Jul 28 12:20:53 2023, max compression
```

## Comparing `nuregi-0.2.0.dev2.tar` & `nuregi-0.2.0.dev3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.393742 nuregi-0.2.0.dev2/
--rw-rw-rw-   0        0        0    35821 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/LICENSE.txt
--rw-rw-rw-   0        0        0     3421 2023-07-28 12:05:34.393742 nuregi-0.2.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     2398 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.372210 nuregi-0.2.0.dev2/nuregi/
--rw-rw-rw-   0        0        0       68 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.388235 nuregi-0.2.0.dev2/nuregi/api/
--rw-rw-rw-   0        0        0      184 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/api/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-07-28 11:55:55.000000 nuregi-0.2.0.dev2/nuregi/api/api.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.390235 nuregi-0.2.0.dev2/nuregi/exceptions/
--rw-rw-rw-   0        0        0       27 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/exceptions/__init__.py
--rw-rw-rw-   0        0        0      359 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.391236 nuregi-0.2.0.dev2/nuregi/scraper/
--rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.392737 nuregi-0.2.0.dev2/nuregi/scraper/pdf/
--rw-rw-rw-   0        0        0       69 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/pdf/__init__.py
--rw-rw-rw-   0        0        0     4483 2023-07-28 11:59:45.000000 nuregi-0.2.0.dev2/nuregi/scraper/pdf/pdf.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.392737 nuregi-0.2.0.dev2/nuregi/scraper/web/
--rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/nuregi/scraper/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 12:05:34.387230 nuregi-0.2.0.dev2/nuregi.egg-info/
--rw-rw-rw-   0        0        0     3421 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 12:05:34.000000 nuregi-0.2.0.dev2/nuregi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-07-28 12:05:34.396742 nuregi-0.2.0.dev2/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-07-28 12:02:20.000000 nuregi-0.2.0.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.819144 nuregi-0.2.0.dev3/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3421 2023-07-28 12:20:53.819144 nuregi-0.2.0.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     2398 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.792805 nuregi-0.2.0.dev3/nuregi/
+-rw-rw-rw-   0        0        0       68 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.813833 nuregi-0.2.0.dev3/nuregi/api/
+-rw-rw-rw-   0        0        0      184 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/api/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-07-28 11:55:55.000000 nuregi-0.2.0.dev3/nuregi/api/api.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.815142 nuregi-0.2.0.dev3/nuregi/exceptions/
+-rw-rw-rw-   0        0        0       27 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      359 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.816142 nuregi-0.2.0.dev3/nuregi/scraper/
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.818143 nuregi-0.2.0.dev3/nuregi/scraper/pdf/
+-rw-rw-rw-   0        0        0       69 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/scraper/pdf/__init__.py
+-rw-rw-rw-   0        0        0     4483 2023-07-28 11:59:45.000000 nuregi-0.2.0.dev3/nuregi/scraper/pdf/pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.819144 nuregi-0.2.0.dev3/nuregi/scraper/web/
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/nuregi/scraper/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:20:53.811832 nuregi-0.2.0.dev3/nuregi.egg-info/
+-rw-rw-rw-   0        0        0     3421 2023-07-28 12:20:53.000000 nuregi-0.2.0.dev3/nuregi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-07-28 12:20:53.000000 nuregi-0.2.0.dev3/nuregi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:20:53.000000 nuregi-0.2.0.dev3/nuregi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-28 12:20:53.000000 nuregi-0.2.0.dev3/nuregi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 12:20:53.000000 nuregi-0.2.0.dev3/nuregi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2023-07-26 21:23:48.000000 nuregi-0.2.0.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-28 12:20:53.821143 nuregi-0.2.0.dev3/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-07-28 12:20:19.000000 nuregi-0.2.0.dev3/setup.py
```

### Comparing `nuregi-0.2.0.dev2/LICENSE.txt` & `nuregi-0.2.0.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev2/PKG-INFO` & `nuregi-0.2.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuregi
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: A basic Python-based API client library for registrar.nu.edu.kz
 Home-page: https://github.com/aldan/nuregi
 Author: aldan
 Author-email: gitaldan@gmail.com
 Project-URL: Source, https://github.com/aldan/nuregi
 Project-URL: Tracker, https://github.com/aldan/nuregi/issues
 Keywords: api library registrar.nu.edu.kz scraper
```

### Comparing `nuregi-0.2.0.dev2/README.md` & `nuregi-0.2.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev2/nuregi/api/api.py` & `nuregi-0.2.0.dev3/nuregi/api/api.py`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev2/nuregi/scraper/pdf/pdf.py` & `nuregi-0.2.0.dev3/nuregi/scraper/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `nuregi-0.2.0.dev2/nuregi.egg-info/PKG-INFO` & `nuregi-0.2.0.dev3/nuregi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuregi
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: A basic Python-based API client library for registrar.nu.edu.kz
 Home-page: https://github.com/aldan/nuregi
 Author: aldan
 Author-email: gitaldan@gmail.com
 Project-URL: Source, https://github.com/aldan/nuregi
 Project-URL: Tracker, https://github.com/aldan/nuregi/issues
 Keywords: api library registrar.nu.edu.kz scraper
```

### Comparing `nuregi-0.2.0.dev2/setup.py` & `nuregi-0.2.0.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 base_dir = pathlib.Path(__file__).parent.resolve()
 long_description = (base_dir / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='nuregi',
-    version='0.2.0.dev2',
+    version='0.2.0.dev3',
     description='A basic Python-based API client library for registrar.nu.edu.kz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aldan/nuregi',
     author='aldan',
     author_email='gitaldan@gmail.com',
 
@@ -33,15 +33,15 @@
         'Source': 'https://github.com/aldan/nuregi',
         'Tracker': 'https://github.com/aldan/nuregi/issues',
     },
 
     packages=find_packages(),
 
     install_requires=[
-        'requests==2.31.0',
-        'numpy==1.25.1',
-        'pandas==2.0.3',
-        'tabula-py==2.7.0',
+        'requests==2.28.1',
+        'numpy==1.23.1',
+        'pandas==1.4.3',
+        'tabula-py==2.4.0',
     ],
 
     python_requires='>=3.8',
 )
```

