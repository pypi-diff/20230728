# Comparing `tmp/nest_asyncio-1.5.6.tar.gz` & `tmp/nest_asyncio-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nest_asyncio-1.5.6.tar", last modified: Fri Sep 30 07:09:13 2022, max compression
+gzip compressed data, was "nest_asyncio-1.5.7.tar", last modified: Fri Jul 28 09:32:50 2023, max compression
```

## Comparing `nest_asyncio-1.5.6.tar` & `nest_asyncio-1.5.7.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2022-09-30 07:09:13.925886 nest_asyncio-1.5.6/
-drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2022-09-30 07:09:13.924886 nest_asyncio-1.5.6/.github/
--rw-r--r--   0 ewald     (1000) ewald     (1000)       45 2022-09-30 06:46:34.000000 nest_asyncio-1.5.6/.github/FUNDING.yml
-drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2022-09-30 07:09:13.924886 nest_asyncio-1.5.6/.github/workflows/
--rw-r--r--   0 ewald     (1000) ewald     (1000)      905 2022-09-30 07:02:48.000000 nest_asyncio-1.5.6/.github/workflows/test.yml
--rw-rw-r--   0 ewald     (1000) ewald     (1000)     1206 2018-09-28 21:35:37.000000 nest_asyncio-1.5.6/.gitignore
--rw-rw-r--   0 ewald     (1000) ewald     (1000)      169 2020-11-03 11:29:33.000000 nest_asyncio-1.5.6/.travis.yml
--rw-rw-r--   0 ewald     (1000) ewald     (1000)     1322 2020-03-29 14:34:24.000000 nest_asyncio-1.5.6/LICENSE
--rw-rw-r--   0 ewald     (1000) ewald     (1000)       45 2020-01-28 12:13:04.000000 nest_asyncio-1.5.6/MANIFEST.in
--rw-r--r--   0 ewald     (1000) ewald     (1000)     2730 2022-09-30 07:09:13.925886 nest_asyncio-1.5.6/PKG-INFO
--rw-rw-r--   0 ewald     (1000) ewald     (1000)     1788 2021-01-24 17:32:43.000000 nest_asyncio-1.5.6/README.rst
--rwxrwxr-x   0 ewald     (1000) ewald     (1000)      113 2018-09-07 15:13:20.000000 nest_asyncio-1.5.6/dist.sh
-drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2022-09-30 07:09:13.925886 nest_asyncio-1.5.6/nest_asyncio.egg-info/
--rw-r--r--   0 ewald     (1000) ewald     (1000)     2730 2022-09-30 07:09:13.000000 nest_asyncio-1.5.6/nest_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 ewald     (1000) ewald     (1000)      339 2022-09-30 07:09:13.000000 nest_asyncio-1.5.6/nest_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 ewald     (1000) ewald     (1000)        1 2022-09-30 07:09:13.000000 nest_asyncio-1.5.6/nest_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 ewald     (1000) ewald     (1000)       13 2022-09-30 07:09:13.000000 nest_asyncio-1.5.6/nest_asyncio.egg-info/top_level.txt
--rw-r--r--   0 ewald     (1000) ewald     (1000)     7779 2022-09-30 06:44:18.000000 nest_asyncio-1.5.6/nest_asyncio.py
--rw-rw-r--   0 ewald     (1000) ewald     (1000)      148 2020-07-16 10:39:43.000000 nest_asyncio-1.5.6/pyproject.toml
--rw-rw-r--   0 ewald     (1000) ewald     (1000)      976 2022-09-30 07:09:13.925886 nest_asyncio-1.5.6/setup.cfg
--rw-rw-r--   0 ewald     (1000) ewald     (1000)       70 2020-07-16 10:39:56.000000 nest_asyncio-1.5.6/setup.py
-drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2022-09-30 07:09:13.925886 nest_asyncio-1.5.6/tests/
--rw-rw-r--   0 ewald     (1000) ewald     (1000)        0 2019-03-05 21:28:45.000000 nest_asyncio-1.5.6/tests/__init__.py
--rw-r--r--   0 ewald     (1000) ewald     (1000)     2974 2022-04-02 13:24:51.000000 nest_asyncio-1.5.6/tests/nest_test.py
+drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2023-07-28 09:32:50.693442 nest_asyncio-1.5.7/
+drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2023-07-28 09:32:50.692442 nest_asyncio-1.5.7/.github/
+-rw-r--r--   0 ewald     (1000) ewald     (1000)       45 2022-09-30 06:46:34.000000 nest_asyncio-1.5.7/.github/FUNDING.yml
+drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2023-07-28 09:32:50.692442 nest_asyncio-1.5.7/.github/workflows/
+-rw-r--r--   0 ewald     (1000) ewald     (1000)     1153 2023-07-27 14:29:57.000000 nest_asyncio-1.5.7/.github/workflows/test.yml
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)     1206 2018-09-28 21:35:37.000000 nest_asyncio-1.5.7/.gitignore
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)     1322 2020-03-29 14:34:24.000000 nest_asyncio-1.5.7/LICENSE
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)       45 2020-01-28 12:13:04.000000 nest_asyncio-1.5.7/MANIFEST.in
+-rw-r--r--   0 ewald     (1000) ewald     (1000)     2730 2023-07-28 09:32:50.693442 nest_asyncio-1.5.7/PKG-INFO
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)     1788 2021-01-24 17:32:43.000000 nest_asyncio-1.5.7/README.rst
+-rwxrwxr-x   0 ewald     (1000) ewald     (1000)      113 2018-09-07 15:13:20.000000 nest_asyncio-1.5.7/dist.sh
+drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2023-07-28 09:32:50.693442 nest_asyncio-1.5.7/nest_asyncio.egg-info/
+-rw-r--r--   0 ewald     (1000) ewald     (1000)     2730 2023-07-28 09:32:50.000000 nest_asyncio-1.5.7/nest_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 ewald     (1000) ewald     (1000)      327 2023-07-28 09:32:50.000000 nest_asyncio-1.5.7/nest_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 ewald     (1000) ewald     (1000)        1 2023-07-28 09:32:50.000000 nest_asyncio-1.5.7/nest_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 ewald     (1000) ewald     (1000)       13 2023-07-28 09:32:50.000000 nest_asyncio-1.5.7/nest_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 ewald     (1000) ewald     (1000)     8006 2023-07-28 09:21:33.000000 nest_asyncio-1.5.7/nest_asyncio.py
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)      148 2020-07-16 10:39:43.000000 nest_asyncio-1.5.7/pyproject.toml
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)      976 2023-07-28 09:32:50.694442 nest_asyncio-1.5.7/setup.cfg
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)       70 2020-07-16 10:39:56.000000 nest_asyncio-1.5.7/setup.py
+drwxr-xr-x   0 ewald     (1000) ewald     (1000)        0 2023-07-28 09:32:50.693442 nest_asyncio-1.5.7/tests/
+-rw-rw-r--   0 ewald     (1000) ewald     (1000)        0 2019-03-05 21:28:45.000000 nest_asyncio-1.5.7/tests/__init__.py
+-rw-r--r--   0 ewald     (1000) ewald     (1000)     2974 2022-04-02 13:24:51.000000 nest_asyncio-1.5.7/tests/nest_test.py
```

### Comparing `nest_asyncio-1.5.6/.gitignore` & `nest_asyncio-1.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nest_asyncio-1.5.6/LICENSE` & `nest_asyncio-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nest_asyncio-1.5.6/PKG-INFO` & `nest_asyncio-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nest_asyncio
-Version: 1.5.6
+Version: 1.5.7
 Summary: Patch asyncio to allow nested event loops
 Home-page: https://github.com/erdewit/nest_asyncio
 Author: Ewald R. de Wit
 Author-email: ewald.de.wit@gmail.com
 License: BSD
 Keywords: asyncio,nested,eventloop
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nest_asyncio-1.5.6/README.rst` & `nest_asyncio-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `nest_asyncio-1.5.6/nest_asyncio.egg-info/PKG-INFO` & `nest_asyncio-1.5.7/nest_asyncio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nest-asyncio
-Version: 1.5.6
+Version: 1.5.7
 Summary: Patch asyncio to allow nested event loops
 Home-page: https://github.com/erdewit/nest_asyncio
 Author: Ewald R. de Wit
 Author-email: ewald.de.wit@gmail.com
 License: BSD
 Keywords: asyncio,nested,eventloop
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nest_asyncio-1.5.6/nest_asyncio.py` & `nest_asyncio-1.5.7/nest_asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,27 @@
 from contextlib import contextmanager, suppress
 from heapq import heappop
 
 
 def apply(loop=None):
     """Patch asyncio to make its event loop reentrant."""
     _patch_asyncio()
+    _patch_policy()
     _patch_task()
     _patch_tornado()
 
     loop = loop or asyncio.get_event_loop()
     _patch_loop(loop)
 
 
 def _patch_asyncio():
     """Patch asyncio module to use pure Python tasks and futures."""
 
     def run(main, *, debug=False):
-        try:
-            loop = asyncio.get_event_loop()
-        except RuntimeError:
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-            _patch_loop(loop)
+        loop = asyncio.get_event_loop()
         loop.set_debug(debug)
         task = asyncio.ensure_future(main)
         try:
             return loop.run_until_complete(task)
         finally:
             if not task.done():
                 task.cancel()
@@ -55,19 +51,32 @@
             asyncio.futures._PyFuture
     if sys.version_info < (3, 7, 0):
         asyncio.tasks._current_tasks = asyncio.tasks.Task._current_tasks
         asyncio.all_tasks = asyncio.tasks.Task.all_tasks
     if sys.version_info >= (3, 9, 0):
         events._get_event_loop = events.get_event_loop = \
             asyncio.get_event_loop = _get_event_loop
-        _get_event_loop
     asyncio.run = run
     asyncio._nest_patched = True
 
 
+def _patch_policy():
+    """Patch the policy to always return a patched loop."""
+
+    def get_event_loop(self):
+        if self._local._loop is None:
+            loop = self.new_event_loop()
+            _patch_loop(loop)
+            self.set_event_loop(loop)
+        return self._local._loop
+
+    policy = events.get_event_loop_policy()
+    policy.__class__.get_event_loop = get_event_loop
+
+
 def _patch_loop(loop):
     """Patch loop to make it reentrant."""
 
     def run_forever(self):
         with manage_run(self), manage_asyncgens(self):
             while True:
                 self._run_once()
```

### Comparing `nest_asyncio-1.5.6/setup.cfg` & `nest_asyncio-1.5.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nest_asyncio
-version = 1.5.6
+version = 1.5.7
 author = Ewald R. de Wit
 author_email = ewald.de.wit@gmail.com
 license = BSD
 license_files = LICENSE
 description = Patch asyncio to allow nested event loops
 keywords = asyncio, nested, eventloop
 url = https://github.com/erdewit/nest_asyncio
```

### Comparing `nest_asyncio-1.5.6/tests/nest_test.py` & `nest_asyncio-1.5.7/tests/nest_test.py`

 * *Files identical despite different names*

