# Comparing `tmp/tiledb_jupyter_bioimg-0.1.4a3.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.4a3.tar", last modified: Thu Jul 27 08:38:32 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.2.0.tar", last modified: Fri Jul 28 09:01:30 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.4a3.tar` & `tiledb_jupyter_bioimg-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-27 08:34:06.000000 tiledb_jupyter_bioimg-0.1.4a3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.624464 tiledb_jupyter_bioimg-0.1.4a3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/embed.ts
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.636464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
--rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 08:37:26.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    86073 2023-07-27 08:37:50.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:38:32.628464 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:35:59.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 08:38:32.000000 tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 08:29:52.000000 tiledb_jupyter_bioimg-0.1.4a3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.514762 tiledb_jupyter_bioimg-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-28 09:01:30.510762 tiledb_jupyter_bioimg-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-28 08:58:12.000000 tiledb_jupyter_bioimg-0.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:01:30.514762 tiledb_jupyter_bioimg-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.506762 tiledb_jupyter_bioimg-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/src/embed.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.506762 tiledb_jupyter_bioimg-0.2.0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.506762 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.506762 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.510762 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/744.dd52ff7cd343d8d95264.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)   790041 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   536613 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b8aecc8f2449f89407f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 09:00:41.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86065 2023-07-28 09:00:59.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:01:30.506762 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-28 09:01:30.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 09:01:30.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:01:30.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:59:37.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 09:01:30.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 09:01:30.000000 tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-28 08:55:10.000000 tiledb_jupyter_bioimg-0.2.0/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/LICENSE` & `tiledb_jupyter_bioimg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/PKG-INFO` & `tiledb_jupyter_bioimg-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.4a3
+Version: 0.2.0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/README.md` & `tiledb_jupyter_bioimg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/package.json` & `tiledb_jupyter_bioimg-0.2.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9708333333333332%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.6'}", "'version'": "'0.2.0'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3 || ^4",
-        "@tiledb-inc/bioimage-viewer": "^0.1.6-alpha.0"
+        "@tiledb-inc/bioimage-viewer": "^0.1.6"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3 || ^4",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.3"
+    "version": "0.2.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/setup.py` & `tiledb_jupyter_bioimg-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/src/index.ts` & `tiledb_jupyter_bioimg-0.2.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/src/version.ts` & `tiledb_jupyter_bioimg-0.2.0/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/src/widget.ts` & `tiledb_jupyter_bioimg-0.2.0/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9704166666666666%*

 * *Differences: {"'dependencies'": "{'@tiledb-inc/bioimage-viewer': '^0.1.6'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b8aecc8f2449f89407f2.js'}}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
         "@jupyterlab/application": "^3 || ^4",
-        "@tiledb-inc/bioimage-viewer": "^0.1.6-alpha.0"
+        "@tiledb-inc/bioimage-viewer": "^0.1.6"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3 || ^4",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
         "@typescript-eslint/parser": "^2.27.0",
         "eslint": "^7.5.0",
@@ -31,15 +31,15 @@
         "style/index.js",
         "dist/*.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.93be46de878c6c06707d.js",
+            "load": "static/remoteEntry.b8aecc8f2449f89407f2.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -106,9 +106,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4-alpha.3"
+    "version": "0.2.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/744.dd52ff7cd343d8d95264.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,32 @@
 "use strict";
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [744], {
         1744: (e, i, t) => {
             t.r(i), t.d(i, {
                 MODULE_NAME: () => o,
-                MODULE_VERSION: () => n,
+                MODULE_VERSION: () => a,
                 default: () => c
             });
             var l = {};
             t.r(l), t.d(l, {
                 BioImageViewerModel: () => u,
                 BioImageViewerView: () => p
             });
             var s = t(1395);
-            const a = t(4147),
-                n = a.version,
-                o = a.name;
-            var r = t(4633),
+            const n = t(4147),
+                a = n.version,
+                o = n.name;
+            var r = t(2041),
                 d = t.n(r);
             class u extends s.DOMWidgetModel {
                 static model_module = o;
-                static model_module_version = n;
+                static model_module_version = a;
                 static view_module = o;
-                static view_module_version = n;
+                static view_module_version = a;
                 static serializers = {
                     ...s.DOMWidgetModel.serializers
                 };
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: u.model_name,
@@ -57,18 +57,18 @@
             const c = {
                 id: "@tiledb-inc/jupyter-bioimage-viewer",
                 autoStart: !0,
                 requires: [s.IJupyterWidgetRegistry],
                 activate: function(e, i) {
                     i.registerWidget({
                         name: o,
-                        version: n,
+                        version: a,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.4-alpha.3","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6-alpha.0"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.2.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","tiledb","bioimaging","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js","dist/*.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension && jlpm run build:dist","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:dist":"NODE_OPTIONS=--max-old-space-size=4096 webpack --mode=production","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3 || ^4","@tiledb-inc/bioimage-viewer":"^0.1.6"},"devDependencies":{"@jupyterlab/builder":"^3 || ^4","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","ts-loader":"^9.2.5","typescript":"~5.1.6","webpack":"^5.88.1","webpack-cli":"^5.1.4"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12","capnp-ts":"0.4.0"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.lab.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b8aecc8f2449f89407f2.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, i, o, l, d, u, c, s, f, p, h, v, b, m, g, y = {
+    var e, r, t, n, i, o, a, l, u, d, c, s, f, p, h, v, b, m, g, y = {
             5290: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                i = t.S[n];
+                            if (i && i !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => i
+                    get: () => i,
+                    init: () => o
                 })
             }
         },
         w = {};
 
     function S(e) {
         var r = w[e];
@@ -46,22 +46,22 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "76d7c7825d9e5b8b9e5b",
+        744: "dd52ff7cd343d8d95264",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e] + ".js?v=" + {
         446: "3bf34f45c93ace9c0f28",
         468: "720ed03247c90f307866",
-        744: "76d7c7825d9e5b8b9e5b",
+        744: "dd52ff7cd343d8d95264",
         747: "6f54d04ff1f3fe09aea9",
         774: "a72cd7bed5a733f86080",
         995: "7e5a9c38e396a47c7d4a"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -69,67 +69,67 @@
             if ("object" == typeof window) return window
         }
     }(), S.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
-    }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, a, i) => {
+    }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var o, l;
-            if (void 0 !== a)
-                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
-                    var c = d[u];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + a) {
-                        o = c;
+            var a, l;
+            if (void 0 !== i)
+                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
+                    var c = u[d];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + i) {
+                        a = c;
                         break
                     }
                 }
-            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, S.nc && o.setAttribute("nonce", S.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
             var s = (r, n) => {
-                    o.onerror = o.onload = null, clearTimeout(f);
-                    var a = e[t];
-                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(n))), r) return r(n)
+                    a.onerror = a.onload = null, clearTimeout(f);
+                    var i = e[t];
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
                 f = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
-                    target: o
+                    target: a
                 }), 12e4);
-            o.onerror = s.bind(null, o.onerror), o.onload = s.bind(null, o.onload), l && document.head.appendChild(o)
+            a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         S.S = {};
         var e = {},
             r = {};
         S.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var i = r[t];
+            if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
+                if (n.push(i), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var i = S.S[t],
-                    o = "@tiledb-inc/jupyter-bioimage-viewer",
+                var o = S.S[t],
+                    a = "@tiledb-inc/jupyter-bioimage-viewer",
                     l = (e, r, t, n) => {
-                        var a = i[e] = i[e] || {},
-                            l = a[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : o > l.from)) && (a[r] = {
+                        var i = o[e] = o[e] || {},
+                            l = i[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (i[r] = {
                             get: t,
-                            from: o,
+                            from: a,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6-alpha.0", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.1.4-alpha.3", (() => S.e(744).then((() => () => S(1744)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    u = [];
+                return "default" === t && (l("@tiledb-inc/bioimage-viewer", "0.1.6", (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))), l("@tiledb-inc/jupyter-bioimage-viewer", "0.2.0", (() => S.e(744).then((() => () => S(1744)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -144,162 +144,162 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                i = (typeof a)[0];
-            if (n >= r.length) return "u" == i;
-            var o = r[n],
-                l = (typeof o)[0];
-            if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
-            if ("o" != i && "u" != i && a != o) return a < o;
+            var i = e[n],
+                o = (typeof i)[0];
+            if (n >= r.length) return "u" == o;
+            var a = r[n],
+                l = (typeof a)[0];
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+            if ("o" != o && "u" != o && i != a) return i < a;
             n++
         }
-    }, a = e => {
+    }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
-        var o = [];
-        for (i = 1; i < e.length; i++) {
-            var l = e[i];
-            o.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
+        var a = [];
+        for (o = 1; o < e.length; o++) {
+            var l = e[o];
+            a.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
         }
-        return d();
+        return u();
 
-        function d() {
-            return o.pop().replace(/^\((.+)\)$/, "$1")
+        function u() {
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
-            for (var o = 0, l = 1, d = !0;; l++, o++) {
-                var u, c, s = l < e.length ? (typeof e[l])[0] : "";
-                if (o >= r.length || "o" == (c = (typeof(u = r[o]))[0])) return !d || ("u" == s ? l > n && !a : "" == s != a);
+                i = n < 0;
+            i && (n = -n - 1);
+            for (var a = 0, l = 1, u = !0;; l++, a++) {
+                var d, c, s = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (c = (typeof(d = r[a]))[0])) return !u || ("u" == s ? l > n && !i : "" == s != i);
                 if ("u" == c) {
-                    if (!d || "u" != s) return !1
-                } else if (d)
+                    if (!u || "u" != s) return !1
+                } else if (u)
                     if (s == c)
                         if (l <= n) {
-                            if (u != e[l]) return !1
+                            if (d != e[l]) return !1
                         } else {
-                            if (a ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (d = !1)
+                            if (i ? d > e[l] : d < e[l]) return !1;
+                            d != e[l] && (u = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (a || l <= n) return !1;
-                    d = !1, l--
+                    if (i || l <= n) return !1;
+                    u = !1, l--
                 } else {
-                    if (l <= n || c < s != a) return !1;
-                    d = !1
-                } else "s" != s && "n" != s && (d = !1, l--)
+                    if (l <= n || c < s != i) return !1;
+                    u = !1
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var f = [],
             p = f.pop.bind(f);
-        for (o = 1; o < e.length; o++) {
-            var h = e[o];
-            f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", u = (e, r, t, n) => {
-        var a = l(e, t);
-        return i(n, a) || s(d(e, t, a, n)), f(e[t][a])
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", d = (e, r, t, n) => {
+        var i = l(e, t);
+        return o(n, i) || s(u(e, t, i, n)), f(e[t][i])
     }, c = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+        var i = e[r];
+        return (r = Object.keys(i).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && i[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
-        var i = S.I(r);
-        return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
-    })(((e, r, t, n) => (o(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, a) => {
-        var i = r && S.o(r, t) && c(r, t, n);
-        return i ? f(i) : a()
+    }, f = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
+        var o = S.I(r);
+        return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, i)) : e(r, S.S[r], t, n, i)
+    })(((e, r, t, n) => (a(e, t), d(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
+        var o = r && S.o(r, t) && c(r, t, n);
+        return o ? f(o) : i()
     })), b = {}, m = {
         1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ]),
-        4633: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 6, , "alpha", 0], (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))),
+        2041: () => v("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 6], (() => Promise.all([S.e(995), S.e(774), S.e(446)]).then((() => () => S(3774))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         6271: () => h("default", "react", [1, 17, 0, 1])
     }, g = {
         446: [4456, 6271],
-        744: [1395, 4633]
+        744: [1395, 2041]
     }, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
             if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete b[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
             try {
-                var a = m[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var i = m[e]();
+                i.then ? r.push(b[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         S.b = document.baseURI || self.location.href;
         var e = {
             448: 0
         };
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var i = S.p + S.u(r),
-                        o = new Error;
-                    S.l(i, (t => {
+                    var i = new Promise(((t, i) => n = e[r] = [t, i]));
+                    t.push(n[2] = i);
+                    var o = S.p + S.u(r),
+                        a = new Error;
+                    S.l(o, (t => {
                         if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                i = t && t.target && t.target.src;
-                            o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
+                            var i = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [i, o, l] = t,
-                    d = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in o) S.o(o, n) && (S.m[n] = o[n]);
+                var n, i, [o, a, l] = t,
+                    u = 0;
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in a) S.o(a, n) && (S.m[n] = a[n]);
                     l && l(S)
                 }
-                for (r && r(t); d < i.length; d++) a = i[d], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < o.length; u++) i = o[u], S.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var j = S(5290);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = j
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989224137931034%*

 * *Differences: {"'packages'": "{23: {'versionInfo': '0.1.6'}}"}*

```diff
@@ -138,15 +138,15 @@
             "name": "@probe.gl/stats",
             "versionInfo": "3.6.0"
         },
         {
             "extractedText": "",
             "licenseId": "MIT",
             "name": "@tiledb-inc/bioimage-viewer",
-            "versionInfo": "0.1.6-alpha.0"
+            "versionInfo": "0.1.6"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2020 TileDB, Inc.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@tiledb-inc/tiledb-cloud",
             "versionInfo": "1.0.13"
         },
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.4a3
+Version: 0.2.0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.2.0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4.svg
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/468.720ed03247c90f307866.js
-tiledb_jupyter_bioimg/labextension/static/744.76d7c7825d9e5b8b9e5b.js
+tiledb_jupyter_bioimg/labextension/static/744.dd52ff7cd343d8d95264.js
 tiledb_jupyter_bioimg/labextension/static/747.6f54d04ff1f3fe09aea9.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js
 tiledb_jupyter_bioimg/labextension/static/774.a72cd7bed5a733f86080.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js
 tiledb_jupyter_bioimg/labextension/static/995.7e5a9c38e396a47c7d4a.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.93be46de878c6c06707d.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.b8aecc8f2449f89407f2.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.4a3/tsconfig.json` & `tiledb_jupyter_bioimg-0.2.0/tsconfig.json`

 * *Files identical despite different names*

