# Comparing `tmp/django-datadog-logger-0.6.1.tar.gz` & `tmp/django-datadog-logger-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-datadog-logger-0.6.1.tar", last modified: Thu Apr 27 15:00:21 2023, max compression
+gzip compressed data, was "django-datadog-logger-0.6.2.tar", last modified: Fri Jul 28 09:55:22 2023, max compression
```

## Comparing `django-datadog-logger-0.6.1.tar` & `django-datadog-logger-0.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      155 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/AUTHORS.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     3699 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/CONTRIBUTING.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1965 2023-04-27 14:59:53.000000 django-datadog-logger-0.6.1/HISTORY.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1070 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/LICENSE
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      287 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/MANIFEST.in
--rw-rw-r--   0 lenno     (1000) lenno     (1000)    11053 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/PKG-INFO
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     8345 2021-08-27 08:13:56.000000 django-datadog-logger-0.6.1/README.rst
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-04-27 15:00:05.000000 django-datadog-logger-0.6.1/django_datadog_logger/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1001 2023-04-27 14:57:10.000000 django-datadog-logger-0.6.1/django_datadog_logger/celery.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      258 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.1/django_datadog_logger/encoders.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/formatters/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/formatters/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     7874 2023-04-27 14:22:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/formatters/datadog.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1608 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.1/django_datadog_logger/local.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/middleware/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      412 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/error_log.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      879 2020-11-04 07:40:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_id.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1861 2020-11-04 07:42:19.000000 django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_log.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      481 2021-06-14 11:41:52.000000 django-datadog-logger-0.6.1/django_datadog_logger/recursion.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     2395 2022-08-09 10:34:11.000000 django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/mixins.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      224 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.1/django_datadog_logger/wsgi.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.328127 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)    11053 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/PKG-INFO
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1176 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2020-02-17 12:25:46.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/not-zip-safe
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/requires.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-04-27 15:00:21.000000 django-datadog-logger-0.6.1/django_datadog_logger.egg-info/top_level.txt
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/docs/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      622 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/Makefile
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/authors.rst
--rwxrwxr-x   0 lenno     (1000) lenno     (1000)     4964 2023-04-27 14:32:31.000000 django-datadog-logger-0.6.1/docs/conf.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       33 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/contributing.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/history.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      318 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/index.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1242 2020-02-17 11:49:32.000000 django-datadog-logger-0.6.1/docs/installation.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      783 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/make.bat
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       27 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.1/docs/readme.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       97 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/docs/usage.rst
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      139 2020-02-17 12:15:03.000000 django-datadog-logger-0.6.1/pyproject.toml
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-04-27 12:59:29.000000 django-datadog-logger-0.6.1/requirements.txt
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      404 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/setup.cfg
--rw-rw-r--   0 lenno     (1000) lenno     (1000)     1731 2023-04-27 15:00:05.000000 django-datadog-logger-0.6.1/setup.py
-drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-04-27 15:00:21.332127 django-datadog-logger-0.6.1/tests/
--rw-rw-r--   0 lenno     (1000) lenno     (1000)       51 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.1/tests/__init__.py
--rw-rw-r--   0 lenno     (1000) lenno     (1000)      437 2020-02-17 11:54:33.000000 django-datadog-logger-0.6.1/tests/test_django_datadog_logger.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.219534 django-datadog-logger-0.6.2/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      155 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/AUTHORS.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     3699 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.2/CONTRIBUTING.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     2064 2023-07-28 09:55:10.000000 django-datadog-logger-0.6.2/HISTORY.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1070 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/LICENSE
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      287 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.2/MANIFEST.in
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)    11152 2023-07-28 09:55:22.219534 django-datadog-logger-0.6.2/PKG-INFO
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     8345 2021-08-27 08:13:56.000000 django-datadog-logger-0.6.2/README.rst
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.211534 django-datadog-logger-0.6.2/django_datadog_logger/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-07-28 09:54:18.000000 django-datadog-logger-0.6.2/django_datadog_logger/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1001 2023-04-27 14:57:10.000000 django-datadog-logger-0.6.2/django_datadog_logger/celery.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      258 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.2/django_datadog_logger/encoders.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.215534 django-datadog-logger-0.6.2/django_datadog_logger/formatters/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.2/django_datadog_logger/formatters/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     8000 2023-07-28 09:53:26.000000 django-datadog-logger-0.6.2/django_datadog_logger/formatters/datadog.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1608 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.2/django_datadog_logger/local.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.215534 django-datadog-logger-0.6.2/django_datadog_logger/middleware/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.2/django_datadog_logger/middleware/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      412 2019-12-16 08:08:58.000000 django-datadog-logger-0.6.2/django_datadog_logger/middleware/error_log.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      879 2020-11-04 07:40:11.000000 django-datadog-logger-0.6.2/django_datadog_logger/middleware/request_id.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1861 2020-11-04 07:42:19.000000 django-datadog-logger-0.6.2/django_datadog_logger/middleware/request_log.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      481 2021-06-14 11:41:52.000000 django-datadog-logger-0.6.2/django_datadog_logger/recursion.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.215534 django-datadog-logger-0.6.2/django_datadog_logger/rest_framework/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        0 2019-08-15 12:47:28.000000 django-datadog-logger-0.6.2/django_datadog_logger/rest_framework/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     2395 2022-08-09 10:34:11.000000 django-datadog-logger-0.6.2/django_datadog_logger/rest_framework/mixins.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      224 2021-06-14 11:05:07.000000 django-datadog-logger-0.6.2/django_datadog_logger/wsgi.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.215534 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)    11152 2023-07-28 09:55:22.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1176 2023-07-28 09:55:22.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2023-07-28 09:55:22.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)        1 2020-02-17 12:25:46.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/not-zip-safe
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-07-28 09:55:22.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/requires.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       22 2023-07-28 09:55:22.000000 django-datadog-logger-0.6.2/django_datadog_logger.egg-info/top_level.txt
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.219534 django-datadog-logger-0.6.2/docs/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      622 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/Makefile
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/authors.rst
+-rwxrwxr-x   0 lenno     (1000) lenno     (1000)     4964 2023-04-27 14:32:31.000000 django-datadog-logger-0.6.2/docs/conf.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       33 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/contributing.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       28 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/history.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      318 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/index.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1242 2020-02-17 11:49:32.000000 django-datadog-logger-0.6.2/docs/installation.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      783 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/make.bat
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       27 2020-11-27 12:01:54.000000 django-datadog-logger-0.6.2/docs/readme.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       97 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/docs/usage.rst
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      139 2020-02-17 12:15:03.000000 django-datadog-logger-0.6.2/pyproject.toml
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       46 2023-04-27 12:59:29.000000 django-datadog-logger-0.6.2/requirements.txt
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      404 2023-07-28 09:55:22.219534 django-datadog-logger-0.6.2/setup.cfg
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)     1731 2023-07-28 09:54:18.000000 django-datadog-logger-0.6.2/setup.py
+drwxrwxr-x   0 lenno     (1000) lenno     (1000)        0 2023-07-28 09:55:22.219534 django-datadog-logger-0.6.2/tests/
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)       51 2020-02-17 11:36:11.000000 django-datadog-logger-0.6.2/tests/__init__.py
+-rw-rw-r--   0 lenno     (1000) lenno     (1000)      437 2020-02-17 11:54:33.000000 django-datadog-logger-0.6.2/tests/test_django_datadog_logger.py
```

### Comparing `django-datadog-logger-0.6.1/CONTRIBUTING.rst` & `django-datadog-logger-0.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/HISTORY.rst` & `django-datadog-logger-0.6.2/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.6.2 (2023-04-27)
+------------------
+
+* Fixed case where accessing request.auth may raise errors
+
 0.6.1 (2023-04-27)
 ------------------
 
 * Removed dependency on Celery package, fixed import error
 
 0.6.0 (2023-04-27)
 ------------------
```

### Comparing `django-datadog-logger-0.6.1/LICENSE` & `django-datadog-logger-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/PKG-INFO` & `django-datadog-logger-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datadog-logger
-Version: 0.6.1
+Version: 0.6.2
 Summary: Django DataDog Logger integration package.
 Home-page: https://github.com/namespace-ee/django-datadog-logger
 Author: Lenno Nagel
 Author-email: lenno@namespace.ee
 License: MIT license
 Keywords: django_datadog_logger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -233,14 +233,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.6.2 (2023-04-27)
+------------------
+
+* Fixed case where accessing request.auth may raise errors
+
 0.6.1 (2023-04-27)
 ------------------
 
 * Removed dependency on Celery package, fixed import error
 
 0.6.0 (2023-04-27)
 ------------------
```

### Comparing `django-datadog-logger-0.6.1/README.rst` & `django-datadog-logger-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/celery.py` & `django-datadog-logger-0.6.2/django_datadog_logger/celery.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/formatters/datadog.py` & `django-datadog-logger-0.6.2/django_datadog_logger/formatters/datadog.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pytz
 import json_log_formatter
 from django.conf import settings
 from django.core.exceptions import DisallowedHost
 from django.http.request import split_domain_port
 from django.urls import resolve, NoReverseMatch, Resolver404
 from rest_framework.compat import unicode_http_header
+from rest_framework.exceptions import AuthenticationFailed
 
 from django_datadog_logger.encoders import SafeJsonEncoder
 from django_datadog_logger.celery import get_task_name, get_celery_request
 import django_datadog_logger.celery
 import django_datadog_logger.wsgi
 
 # those fields are excluded from extra dict
@@ -50,16 +51,19 @@
             if t.params.get("version") is not None:
                 return unicode_http_header(t.params.get("version"))
     return None
 
 
 @not_recursive
 def get_wsgi_request_auth(wsgi_request):
-    if getattr(wsgi_request, "auth", None) is not None and isinstance(wsgi_request.auth, dict):
-        return wsgi_request.auth
+    try:
+        if getattr(wsgi_request, "auth", None) is not None and isinstance(wsgi_request.auth, dict):
+            return wsgi_request.auth
+    except Exception:  # NOQA
+        return None
 
 
 @not_recursive
 def get_wsgi_request_user(wsgi_request):
     if getattr(wsgi_request, "user", None) is not None:
         if getattr(wsgi_request.user, "is_authenticated", False):
             return wsgi_request.user
```

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/local.py` & `django-datadog-logger-0.6.2/django_datadog_logger/local.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_id.py` & `django-datadog-logger-0.6.2/django_datadog_logger/middleware/request_id.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/middleware/request_log.py` & `django-datadog-logger-0.6.2/django_datadog_logger/middleware/request_log.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger/rest_framework/mixins.py` & `django-datadog-logger-0.6.2/django_datadog_logger/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger.egg-info/PKG-INFO` & `django-datadog-logger-0.6.2/django_datadog_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datadog-logger
-Version: 0.6.1
+Version: 0.6.2
 Summary: Django DataDog Logger integration package.
 Home-page: https://github.com/namespace-ee/django-datadog-logger
 Author: Lenno Nagel
 Author-email: lenno@namespace.ee
 License: MIT license
 Keywords: django_datadog_logger
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -233,14 +233,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+0.6.2 (2023-04-27)
+------------------
+
+* Fixed case where accessing request.auth may raise errors
+
 0.6.1 (2023-04-27)
 ------------------
 
 * Removed dependency on Celery package, fixed import error
 
 0.6.0 (2023-04-27)
 ------------------
```

### Comparing `django-datadog-logger-0.6.1/django_datadog_logger.egg-info/SOURCES.txt` & `django-datadog-logger-0.6.2/django_datadog_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/docs/Makefile` & `django-datadog-logger-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/docs/conf.py` & `django-datadog-logger-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/docs/installation.rst` & `django-datadog-logger-0.6.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/docs/make.bat` & `django-datadog-logger-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-datadog-logger-0.6.1/setup.py` & `django-datadog-logger-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="django_datadog_logger",
     name="django-datadog-logger",
     packages=find_packages(include=["django_datadog_logger", "django_datadog_logger.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/namespace-ee/django-datadog-logger",
-    version="0.6.1",
+    version="0.6.2",
     zip_safe=False,
 )
```

