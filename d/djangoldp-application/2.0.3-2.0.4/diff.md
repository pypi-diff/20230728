# Comparing `tmp/djangoldp_application-2.0.3.tar.gz` & `tmp/djangoldp_application-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_application-2.0.3.tar", last modified: Fri Jul 28 13:57:57 2023, max compression
+gzip compressed data, was "djangoldp_application-2.0.4.tar", last modified: Fri Jul 28 13:58:38 2023, max compression
```

## Comparing `djangoldp_application-2.0.3.tar` & `djangoldp_application-2.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.047298 djangoldp_application-2.0.3/
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:57:57.047298 djangoldp_application-2.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.043298 djangoldp_application-2.0.3/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-28 13:57:54.000000 djangoldp_application-2.0.3/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.047298 djangoldp_application-2.0.3/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0006_applicationservice.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21594 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.043298 djangoldp_application-2.0.3/djangoldp_application/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.047298 djangoldp_application-2.0.3/djangoldp_application/templates/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/templates/djangoldp_application/email.html
--rw-rw-rw-   0 root         (0) root         (0)    26529 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/djangoldp_application/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:57:57.043298 djangoldp_application-2.0.3/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:57:56.000000 djangoldp_application-2.0.3/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1425 2023-07-28 13:57:57.000000 djangoldp_application-2.0.3/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:57:56.000000 djangoldp_application-2.0.3/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-28 13:57:56.000000 djangoldp_application-2.0.3/djangoldp_application.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 13:57:56.000000 djangoldp_application-2.0.3/djangoldp_application.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-28 13:57:57.047298 djangoldp_application-2.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-28 13:57:38.000000 djangoldp_application-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-28 13:58:35.000000 djangoldp_application-2.0.4/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0006_applicationservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21594 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.524931 djangoldp_application-2.0.4/djangoldp_application/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/email.html
+-rw-rw-rw-   0 root         (0) root         (0)    26529 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/setup.py
```

### Comparing `djangoldp_application-2.0.3/README.md` & `djangoldp_application-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/admin.py` & `djangoldp_application-2.0.4/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-2.0.4/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-2.0.4/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/models.py` & `djangoldp_application-2.0.4/djangoldp_application/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/templates/djangoldp_application/email.html` & `djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application/views.py` & `djangoldp_application-2.0.4/djangoldp_application/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-2.0.4/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.3/setup.cfg` & `djangoldp_application-2.0.4/setup.cfg`

 * *Files identical despite different names*

