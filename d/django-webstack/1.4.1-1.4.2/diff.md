# Comparing `tmp/django-webstack-1.4.1.tar.gz` & `tmp/django-webstack-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.4.1.tar", last modified: Fri Jul 28 04:06:25 2023, max compression
+gzip compressed data, was "django-webstack-1.4.2.tar", last modified: Fri Jul 28 04:15:14 2023, max compression
```

## Comparing `django-webstack-1.4.1.tar` & `django-webstack-1.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 04:06:16.000000 django-webstack-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 04:06:16.000000 django-webstack-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:06:25.200587 django-webstack-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 04:06:16.000000 django-webstack-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:06:25.200587 django-webstack-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-28 04:06:23.000000 django-webstack-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0003_auto_20230725_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.196587 django-webstack-1.4.1/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.196587 django-webstack-1.4.1/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.602132 django-webstack-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 04:15:04.000000 django-webstack-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 04:15:04.000000 django-webstack-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:15:14.602132 django-webstack-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 04:15:04.000000 django-webstack-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:15:14.000000 django-webstack-1.4.2/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-28 04:15:14.000000 django-webstack-1.4.2/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:15:14.000000 django-webstack-1.4.2/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 04:15:14.000000 django-webstack-1.4.2/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:15:14.000000 django-webstack-1.4.2/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:15:14.602132 django-webstack-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-28 04:15:13.000000 django-webstack-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.598132 django-webstack-1.4.2/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.598132 django-webstack-1.4.2/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.602132 django-webstack-1.4.2/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.594132 django-webstack-1.4.2/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:15:14.602132 django-webstack-1.4.2/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 04:15:04.000000 django-webstack-1.4.2/webstack/views.py
```

### Comparing `django-webstack-1.4.1/LICENSE` & `django-webstack-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/PKG-INFO` & `django-webstack-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.4.1
+Version: 1.4.2
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.4.1/README.md` & `django-webstack-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.4.2/django_webstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.4.1
+Version: 1.4.2
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.4.1/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.4.2/django_webstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/setup.py` & `django-webstack-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
 # 这里的版本号根据tag去动态设置
-VERSION = '1.4.1'
+VERSION = '1.4.2'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.4.1/webstack/admin.py` & `django-webstack-1.4.2/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/migrations/0001_initial.py` & `django-webstack-1.4.2/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.4.2/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/migrations/0003_auto_20230725_1401.py` & `django-webstack-1.4.2/webstack/migrations/0003_auto_20230725_1401.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/models.py` & `django-webstack-1.4.2/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.4.2/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.4.2/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.4.2/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.4.2/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.4.2/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.4.2/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.1/webstack/templates/webstack/base.html` & `django-webstack-1.4.2/webstack/templates/webstack/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,29 @@
     <link href="https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
     <link href="https://cdn.bootcss.com/twitter-bootstrap/3.0.2/css/bootstrap.min.css" rel="stylesheet">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-core.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-components.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-skins.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/nav.css' %}">
     <script src="https://cdn.bootcss.com/jquery/1.11.1/jquery.min.js"></script>
+    <style>
+        .sidebar-menu .main-menu a {
+            padding: 14px 4px;
+        }
+
+        .sidebar-menu .main-menu a > i {
+            margin-right: 8px;
+            width: 18px;
+            max-height: 18px;
+        }
+
+        .sidebar-menu .main-menu ul li a {
+            padding-left: 34px;
+        }
+    </style>
     {% block top-file %}{% endblock %}
 </head>
 
 <body class="page-body">
 <!-- skin-white -->
 <div class="page-container">
     <div class="sidebar-menu toggle-others fixed">
```

### Comparing `django-webstack-1.4.1/webstack/templates/webstack/index.html` & `django-webstack-1.4.2/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

