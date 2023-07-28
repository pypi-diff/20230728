# Comparing `tmp/django-webstack-1.4.0.tar.gz` & `tmp/django-webstack-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.4.0.tar", last modified: Thu Jul 27 11:20:01 2023, max compression
+gzip compressed data, was "django-webstack-1.4.1.tar", last modified: Fri Jul 28 04:06:25 2023, max compression
```

## Comparing `django-webstack-1.4.0.tar` & `django-webstack-1.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.103463 django-webstack-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 11:19:50.000000 django-webstack-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 11:19:50.000000 django-webstack-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-27 11:20:01.103463 django-webstack-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 11:19:50.000000 django-webstack-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.095463 django-webstack-1.4.0/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-27 11:20:01.000000 django-webstack-1.4.0/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-27 11:20:01.000000 django-webstack-1.4.0/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:20:01.000000 django-webstack-1.4.0/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 11:20:01.000000 django-webstack-1.4.0/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 11:20:01.000000 django-webstack-1.4.0/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:20:01.103463 django-webstack-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-27 11:19:59.000000 django-webstack-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.099463 django-webstack-1.4.0/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.099463 django-webstack-1.4.0/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/migrations/0003_auto_20230725_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.095463 django-webstack-1.4.0/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.095463 django-webstack-1.4.0/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.095463 django-webstack-1.4.0/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.099463 django-webstack-1.4.0/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.099463 django-webstack-1.4.0/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.103463 django-webstack-1.4.0/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.095463 django-webstack-1.4.0/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:20:01.103463 django-webstack-1.4.0/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 11:19:50.000000 django-webstack-1.4.0/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 04:06:16.000000 django-webstack-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 04:06:16.000000 django-webstack-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:06:25.200587 django-webstack-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 04:06:16.000000 django-webstack-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 04:06:25.000000 django-webstack-1.4.1/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 04:06:25.200587 django-webstack-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-28 04:06:23.000000 django-webstack-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.196587 django-webstack-1.4.1/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.196587 django-webstack-1.4.1/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.192587 django-webstack-1.4.1/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:06:25.200587 django-webstack-1.4.1/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 04:06:16.000000 django-webstack-1.4.1/webstack/views.py
```

### Comparing `django-webstack-1.4.0/LICENSE` & `django-webstack-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/PKG-INFO` & `django-webstack-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.4.0
+Version: 1.4.1
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.4.0/README.md` & `django-webstack-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.4.1/django_webstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.4.0
+Version: 1.4.1
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.4.0/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.4.1/django_webstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/setup.py` & `django-webstack-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
 # 这里的版本号根据tag去动态设置
-VERSION = '1.4.0'
+VERSION = '1.4.1'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

### Comparing `django-webstack-1.4.0/webstack/admin.py` & `django-webstack-1.4.1/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/migrations/0001_initial.py` & `django-webstack-1.4.1/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.4.1/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/migrations/0003_auto_20230725_1401.py` & `django-webstack-1.4.1/webstack/migrations/0003_auto_20230725_1401.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/models.py` & `django-webstack-1.4.1/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.4.1/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.4.1/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.4.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.4.1/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.4.1/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.4.1/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.4.0/webstack/templates/webstack/base.html` & `django-webstack-1.4.1/webstack/templates/webstack/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 <html lang="zh">
 
 <head>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
     <title>{% block title %}{% endblock %}</title>
-    <meta name="keywords"
-          content="UI设计,UI设计素材,设计导航,网址导航,设计资源,创意导航,创意网站导航,设计师网址大全,设计素材大全,设计师导航,UI设计资源,优秀UI设计欣赏,设计师导航,设计师网址大全,设计师网址导航,产品经理网址导航,交互设计师网址导航,www.webstack.cc">
-    <meta name="description" content="WebStack - 收集国内外优秀设计网站、UI设计资源网站、灵感创意网站、素材资源网站，定时更新分享优质产品设计书签。www.webstack.cc">
     {% block meta %}{% endblock %}
     <link href="https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
     <link href="https://cdn.bootcss.com/twitter-bootstrap/3.0.2/css/bootstrap.min.css" rel="stylesheet">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-core.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-components.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/xenon-skins.css' %}">
     <link rel="stylesheet" href="{% static 'webstack/assets/css/nav.css' %}">
```

### Comparing `django-webstack-1.4.0/webstack/templates/webstack/index.html` & `django-webstack-1.4.1/webstack/templates/webstack/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% extends 'webstack/base.html' %}
 {% load static %}
 
-{% block title %}我的导航网站{% endblock %}
+{% block title %}导航网站{% endblock %}
 
 {% block meta %}
     <link rel="shortcut icon" href="{% static 'webstack/assets/images/favicon.png' %}">
+    <meta name="keywords" content="网址导航">
+    <meta name="description" content="常用网址导航聚合站">
 {% endblock %}
 
 {% block top-file %}{% endblock %}
 
 {% block logo %}
     <div class="logo">
         <a href="#" class="logo-expanded">
@@ -25,16 +27,16 @@
 {% endblock %}
 
 {% block main-menu %}{% endblock %}
 
 {% block footer %}
     <div class="footer-text">
         &copy; 2023
-        <a href="https://github.com/WebStackPage/WebStackPage.github.io" target="_blank">
-            <strong>WebStack</strong>
+        <a href="https://github.com/Hopetree/django-webstack" target="_blank">
+            <strong>django-webstack</strong>
         </a>
         design by
-        <a href="https://github.com/Hopetree/django-webstack" target="_blank">
-            <strong>Hopetree</strong>
+        <a href="https://github.com/WebStackPage/WebStackPage.github.io" target="_blank">
+            <strong>WebStack</strong>
         </a>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'webstack/base.html' %} {% load static %} {% block title
-%}æçå¯¼èªç½ç«{% endblock %} {% block meta %}
+%}å¯¼èªç½ç«{% endblock %} {% block meta %}
+
+
  {% endblock %} {% block top-file %}{% endblock %} {% block logo %}
 
 {% endblock %} {% block navbar-list %}
 é¦é¡µ
 {% endblock %} {% block main-menu %}{% endblock %} {% block footer %}
-© 2023 WebStack design by Hopetree
+© 2023 django-webstack design by WebStack
 {% endblock %}
```

