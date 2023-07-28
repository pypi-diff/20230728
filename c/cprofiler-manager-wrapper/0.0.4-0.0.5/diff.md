# Comparing `tmp/cprofiler_manager_wrapper-0.0.4.tar.gz` & `tmp/cprofiler_manager_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cprofiler_manager_wrapper-0.0.4.tar", last modified: Fri Feb 17 18:40:26 2023, max compression
+gzip compressed data, was "cprofiler_manager_wrapper-0.0.5.tar", last modified: Fri Jul 28 17:40:18 2023, max compression
```

## Comparing `cprofiler_manager_wrapper-0.0.4.tar` & `cprofiler_manager_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/
--rw-r--r--   0 aleksejsosov   (501) staff       (20)     1663 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/PKG-INFO
--rw-r--r--   0 aleksejsosov   (501) staff       (20)      664 2023-02-17 18:39:06.000000 cprofiler_manager_wrapper-0.0.4/README.md
--rw-r--r--   0 aleksejsosov   (501) staff       (20)      116 2023-02-17 18:39:37.000000 cprofiler_manager_wrapper-0.0.4/setup.py
-drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/
--rw-r--r--   0 aleksejsosov   (501) staff       (20)     1663 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 aleksejsosov   (501) staff       (20)      348 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 aleksejsosov   (501) staff       (20)       18 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/requires.txt
--rw-r--r--   0 aleksejsosov   (501) staff       (20)       26 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/top_level.txt
--rw-r--r--   0 aleksejsosov   (501) staff       (20)        1 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 aleksejsosov   (501) staff       (20)      774 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/setup.cfg
-drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-02-17 18:40:25.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper/
--rw-r--r--   0 aleksejsosov   (501) staff       (20)       30 2023-02-17 18:00:36.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper/__init__.py
--rw-r--r--   0 aleksejsosov   (501) staff       (20)     1551 2023-02-17 17:46:01.000000 cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper/profiler.py
+drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-07-28 17:40:18.441067 cprofiler_manager_wrapper-0.0.5/
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)     1391 2023-07-28 17:40:18.441136 cprofiler_manager_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)      664 2023-07-28 17:38:51.000000 cprofiler_manager_wrapper-0.0.5/README.md
+drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-07-28 17:40:18.440233 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper/
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)       30 2023-07-28 17:38:51.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper/__init__.py
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)     1551 2023-07-28 17:38:51.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper/profiler.py
+drwxr-xr-x   0 aleksejsosov   (501) staff       (20)        0 2023-07-28 17:40:18.440918 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)     1391 2023-07-28 17:40:18.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)      363 2023-07-28 17:40:18.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)        1 2023-07-28 17:40:18.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)       18 2023-07-28 17:40:18.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/requires.txt
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)       26 2023-07-28 17:40:18.000000 cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)       98 2023-07-28 17:38:51.000000 cprofiler_manager_wrapper-0.0.5/pyproject.toml
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)      774 2023-07-28 17:40:18.441371 cprofiler_manager_wrapper-0.0.5/setup.cfg
+-rw-r--r--   0 aleksejsosov   (501) staff       (20)      116 2023-07-28 17:38:51.000000 cprofiler_manager_wrapper-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cprofiler_manager_wrapper-0.0.4/PKG-INFO` & `cprofiler_manager_wrapper-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: cprofiler_manager_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: simple_profiler
 Home-page: https://github.com/Rwwwrl/SimpleProfiler
 Author: Alexey Sosov
 Author-email: lesh.solowiew@yandex.ru
 License: BSD-3-Clause
-Description: ### Install
-        
-        `pip install cprofiler-manager-wrapper`
-        
-        ### Usage
-        
-        ```python
-        from cprofiler_manager_wrapper import Profiler
-        
-        
-        def func_to_profile():
-            from time import sleep
-        
-            result = []
-            for i in range(10):
-                result.append(i)
-            sleep(1)
-        
-            a = 10
-        
-            return 'hello world'
-        
-        
-        with Profiler(func_about_string='func', disable=False):
-            func_to_profile()
-        ```
-        
-        По итогу будет создана, если ее не было, папка _prof_folder_, внутри которой будет лежат файл _<some>.prof_
-        
-        Для открытия .prof файла используется **snakeviz** - `snakeviz prof_folder/<some>.prof`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+### Install
+
+`pip install cprofiler-manager-wrapper`
+
+### Usage
+
+```python
+from cprofiler_manager_wrapper import Profiler
+
+
+def func_to_profile():
+    from time import sleep
+
+    result = []
+    for i in range(10):
+        result.append(i)
+    sleep(1)
+
+    a = 10
+
+    return 'hello world'
+
+
+with Profiler(func_about_string='func', disable=False):
+    func_to_profile()
+```
+
+По итогу будет создана, если ее не было, папка _prof_folder_, внутри которой будет лежат файл _<some>.prof_
+
+Для открытия .prof файла используется **snakeviz** - `snakeviz prof_folder/<some>.prof`
```

### Comparing `cprofiler_manager_wrapper-0.0.4/README.md` & `cprofiler_manager_wrapper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper.egg-info/PKG-INFO` & `cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: cprofiler-manager-wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: simple_profiler
 Home-page: https://github.com/Rwwwrl/SimpleProfiler
 Author: Alexey Sosov
 Author-email: lesh.solowiew@yandex.ru
 License: BSD-3-Clause
-Description: ### Install
-        
-        `pip install cprofiler-manager-wrapper`
-        
-        ### Usage
-        
-        ```python
-        from cprofiler_manager_wrapper import Profiler
-        
-        
-        def func_to_profile():
-            from time import sleep
-        
-            result = []
-            for i in range(10):
-                result.append(i)
-            sleep(1)
-        
-            a = 10
-        
-            return 'hello world'
-        
-        
-        with Profiler(func_about_string='func', disable=False):
-            func_to_profile()
-        ```
-        
-        По итогу будет создана, если ее не было, папка _prof_folder_, внутри которой будет лежат файл _<some>.prof_
-        
-        Для открытия .prof файла используется **snakeviz** - `snakeviz prof_folder/<some>.prof`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+### Install
+
+`pip install cprofiler-manager-wrapper`
+
+### Usage
+
+```python
+from cprofiler_manager_wrapper import Profiler
+
+
+def func_to_profile():
+    from time import sleep
+
+    result = []
+    for i in range(10):
+        result.append(i)
+    sleep(1)
+
+    a = 10
+
+    return 'hello world'
+
+
+with Profiler(func_about_string='func', disable=False):
+    func_to_profile()
+```
+
+По итогу будет создана, если ее не было, папка _prof_folder_, внутри которой будет лежат файл _<some>.prof_
+
+Для открытия .prof файла используется **snakeviz** - `snakeviz prof_folder/<some>.prof`
```

### Comparing `cprofiler_manager_wrapper-0.0.4/setup.cfg` & `cprofiler_manager_wrapper-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cprofiler_manager_wrapper
-version = 0.0.4
+version = 0.0.5
 description = simple_profiler
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Rwwwrl/SimpleProfiler
 author = Alexey Sosov
 author_email = lesh.solowiew@yandex.ru
 license = BSD-3-Clause
```

### Comparing `cprofiler_manager_wrapper-0.0.4/cprofiler_manager_wrapper/profiler.py` & `cprofiler_manager_wrapper-0.0.5/cprofiler_manager_wrapper/profiler.py`

 * *Files identical despite different names*

