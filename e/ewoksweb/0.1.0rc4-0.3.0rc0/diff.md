# Comparing `tmp/ewoksweb-0.1.0rc4.tar.gz` & `tmp/ewoksweb-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewoksweb-0.1.0rc4.tar", last modified: Wed May 24 09:24:58 2023, max compression
+gzip compressed data, was "ewoksweb-0.3.0rc0.tar", last modified: Fri Jul 28 05:17:43 2023, max compression
```

## Comparing `ewoksweb-0.1.0rc4.tar` & `ewoksweb-0.3.0rc0.tar`

### file list

```diff
@@ -1,32 +1,47 @@
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.647961 ewoksweb-0.1.0rc4/
--rw-rw-r--   0 huder     (1001) huder     (1001)     1102 2021-11-17 12:38:29.000000 ewoksweb-0.1.0rc4/LICENSE.md
--rw-rw-r--   0 huder     (1001) huder     (1001)     1736 2023-05-24 09:24:58.647961 ewoksweb-0.1.0rc4/PKG-INFO
--rw-rw-r--   0 huder     (1001) huder     (1001)     1021 2023-03-30 09:37:55.000000 ewoksweb-0.1.0rc4/README.md
--rw-rw-r--   0 huder     (1001) huder     (1001)      109 2022-10-26 14:51:49.000000 ewoksweb-0.1.0rc4/pyproject.toml
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/
--rw-rw-r--   0 huder     (1001) huder     (1001)       25 2023-05-24 09:23:57.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/__init__.py
--rw-rw-r--   0 huder     (1001) huder     (1001)      103 2022-10-26 14:51:49.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/serverutils.py
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/
--rw-rw-r--   0 huder     (1001) huder     (1001)      457 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/asset-manifest.json
--rw-rw-r--   0 huder     (1001) huder     (1001)     3870 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/favicon.ico
--rw-rw-r--   0 huder     (1001) huder     (1001)      635 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/index.html
--rw-rw-r--   0 huder     (1001) huder     (1001)       67 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/robots.txt
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/css/
--rw-rw-r--   0 huder     (1001) huder     (1001)    13629 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/css/main.fa9245a4.css
--rw-rw-r--   0 huder     (1001) huder     (1001)    28831 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/css/main.fa9245a4.css.map
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/js/
--rw-rw-r--   0 huder     (1001) huder     (1001)  1056213 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/js/main.1414d6ae.js
--rw-rw-r--   0 huder     (1001) huder     (1001)     3267 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/js/main.1414d6ae.js.LICENSE.txt
--rw-rw-r--   0 huder     (1001) huder     (1001)  4896772 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/js/main.1414d6ae.js.map
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.647961 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/media/
--rw-rw-r--   0 huder     (1001) huder     (1001)   157151 2023-05-24 09:24:44.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/media/ewoksUI.27496ca19b6f9d2adad4.png
-drwxrwxr-x   0 huder     (1001) huder     (1001)        0 2023-05-24 09:24:58.639961 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/
--rw-rw-r--   0 huder     (1001) huder     (1001)     1736 2023-05-24 09:24:58.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/PKG-INFO
--rw-rw-r--   0 huder     (1001) huder     (1001)      779 2023-05-24 09:24:58.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/SOURCES.txt
--rw-rw-r--   0 huder     (1001) huder     (1001)        1 2023-05-24 09:24:58.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/dependency_links.txt
--rw-rw-r--   0 huder     (1001) huder     (1001)       46 2023-05-24 09:24:58.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/requires.txt
--rw-rw-r--   0 huder     (1001) huder     (1001)        9 2023-05-24 09:24:58.000000 ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/top_level.txt
--rw-rw-r--   0 huder     (1001) huder     (1001)     1026 2023-05-24 09:24:58.647961 ewoksweb-0.1.0rc4/setup.cfg
--rw-rw-r--   0 huder     (1001) huder     (1001)      319 2022-05-24 08:27:41.000000 ewoksweb-0.1.0rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.074628 ewoksweb-0.3.0rc0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-28 05:17:43.074628 ewoksweb-0.3.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.046628 ewoksweb-0.3.0rc0/pysrc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.050628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/serverutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.054628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/index.html
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.050628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.054628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/css/
+-rw-r--r--   0 root         (0) root         (0)    20344 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/css/main.cf942d14.css
+-rw-r--r--   0 root         (0) root         (0)    40115 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/css/main.cf942d14.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.058628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/js/
+-rw-r--r--   0 root         (0) root         (0)  2467748 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/js/main.bddfef29.js
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/js/main.bddfef29.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  9125073 2023-07-28 05:17:42.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/js/main.bddfef29.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.070628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:28.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.070628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:28.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.070628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-28 05:15:18.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/icons/down.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.074628 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Adding-Tasks.json
+-rw-rw-rw-   0 root         (0) root         (0)    12150 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Buttons_Explanation.json
+-rw-rw-rw-   0 root         (0) root         (0)    26964 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Editing-Graph-Node-Link.json
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Ewoks-Tasks.json
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Styling-Nodes-Links.json
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/Subgraphs-Loops.json
+-rw-rw-rw-   0 root         (0) root         (0)    27687 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/WhatIsEwoks.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:28.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23112 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb/tests/resources/workflows/tutorial_Graph.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:17:43.054628 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-28 05:17:43.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-07-28 05:17:43.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:17:43.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-28 05:17:43.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 05:17:43.000000 ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-28 05:17:43.074628 ewoksweb-0.3.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-07-28 05:03:47.000000 ewoksweb-0.3.0rc0/setup.py
```

### Comparing `ewoksweb-0.1.0rc4/LICENSE.md` & `ewoksweb-0.3.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc4/PKG-INFO` & `ewoksweb-0.3.0rc0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksweb
-Version: 0.1.0rc4
+Version: 0.3.0rc0
 Summary: Web frontend for ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Author: ESRF
 Author-email: giannis.koumoutsos@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb
@@ -23,68 +23,24 @@
 _ewoksweb_ is a frontend to create, visualize and execute
 [ewoks](https://ewoks.readthedocs.io/) workflows in the web.
 
 ## Demo
 
 https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb/
 
-## From source
+## Local installation
 
-Required system packages
-
-```bash
-apt-get install npm
-npm install -g pnpm
-```
-
-Start the frontend
-
-```bash
-pnpm start
-```
-
-Build the package for deployment on pypi
-
-```bash
-npx -y browserslist@latest --update-db  # optional
-pnpm install
-pnpm build
-python setup.py sdist
-```
-
-## From pypi
-
-Install REST server only (`ewoksserver` is another package)
-
-```bash
-pip install ewoksserver
-```
-
-Install REST server with frontend (`ewoksserver` has `ewoksweb` as optional
-dependency)
+Install the [ewoksserver](https://ewoksserver.readthedocs.io) python package
 
 ```bash
 pip install ewoksserver[frontend]
 ```
 
-or alternatively
-
-```bash
-pip install ewoksserver
-pip install ewoksweb
-```
-
-Start the server that serves the frontend
+Start the server and open the frontend in a web browser
 
 ```bash
 ewoks-server
 ```
 
-or for an installation with the system python
-
-```bash
-python3 -m ewoksserver.server
-```
-
 ## Documentation
 
 https://ewoksweb.readthedocs.io/
```

### Comparing `ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/favicon.ico` & `ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/index.html` & `ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><title>Ewoks-web</title><meta name="description" content="Visualizer for Ewoks task graphs"/><link rel="icon" href="./favicon.ico"/><link rel="apple-touch-icon" href="./favicon192.png"/><script src="https://polyfill.io/v3/polyfill.min.js?features=default"></script><script defer="defer" src="./static/js/main.1414d6ae.js"></script><link href="./static/css/main.fa9245a4.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><title>Ewoks-web</title><meta name="description" content="Visualizer for Ewoks task graphs"/><link rel="icon" href="./favicon.ico"/><link rel="apple-touch-icon" href="./favicon192.png"/><script src="https://polyfill.io/v3/polyfill.min.js?features=default"></script><script defer="defer" src="./static/js/main.bddfef29.js"></script><link href="./static/css/main.cf942d14.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `ewoksweb-0.1.0rc4/pysrc/ewoksweb/static/static/js/main.1414d6ae.js.LICENSE.txt` & `ewoksweb-0.3.0rc0/pysrc/ewoksweb/static/static/js/main.bddfef29.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc4/pysrc/ewoksweb.egg-info/PKG-INFO` & `ewoksweb-0.3.0rc0/pysrc/ewoksweb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksweb
-Version: 0.1.0rc4
+Version: 0.3.0rc0
 Summary: Web frontend for ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Author: ESRF
 Author-email: giannis.koumoutsos@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb
@@ -23,68 +23,24 @@
 _ewoksweb_ is a frontend to create, visualize and execute
 [ewoks](https://ewoks.readthedocs.io/) workflows in the web.
 
 ## Demo
 
 https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb/
 
-## From source
+## Local installation
 
-Required system packages
-
-```bash
-apt-get install npm
-npm install -g pnpm
-```
-
-Start the frontend
-
-```bash
-pnpm start
-```
-
-Build the package for deployment on pypi
-
-```bash
-npx -y browserslist@latest --update-db  # optional
-pnpm install
-pnpm build
-python setup.py sdist
-```
-
-## From pypi
-
-Install REST server only (`ewoksserver` is another package)
-
-```bash
-pip install ewoksserver
-```
-
-Install REST server with frontend (`ewoksserver` has `ewoksweb` as optional
-dependency)
+Install the [ewoksserver](https://ewoksserver.readthedocs.io) python package
 
 ```bash
 pip install ewoksserver[frontend]
 ```
 
-or alternatively
-
-```bash
-pip install ewoksserver
-pip install ewoksweb
-```
-
-Start the server that serves the frontend
+Start the server and open the frontend in a web browser
 
 ```bash
 ewoks-server
 ```
 
-or for an installation with the system python
-
-```bash
-python3 -m ewoksserver.server
-```
-
 ## Documentation
 
 https://ewoksweb.readthedocs.io/
```

### Comparing `ewoksweb-0.1.0rc4/setup.cfg` & `ewoksweb-0.3.0rc0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 where = pysrc
 
 [options.package_data]
 ewoksweb = 
 	static/*
 	static/*/*.*
 	static/*/*/*.*
+	tests/resources/icons/*
+	tests/resources/workflows/*
 
 [options.extras_require]
 dev = 
 	black >=22
 	flake8 >=4
 doc = 
 	sphinx >=4.5
```

