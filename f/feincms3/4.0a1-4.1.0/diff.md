# Comparing `tmp/feincms3-4.0a1.tar.gz` & `tmp/feincms3-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feincms3-4.0a1.tar", last modified: Tue Sep 27 14:55:29 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `feincms3-4.0a1.tar` & `feincms3-4.1.0.tar`

### file list

```diff
@@ -1,71 +1,45 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.748573 feincms3-4.0a1/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1552 2022-03-23 06:34:04.000000 feincms3-4.0a1/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      166 2022-03-23 06:34:04.000000 feincms3-4.0a1/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1858 2022-09-27 14:55:29.748573 feincms3-4.0a1/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      787 2022-03-23 06:34:04.000000 feincms3-4.0a1/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.718573 feincms3-4.0a1/feincms3/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       63 2022-09-27 14:55:05.000000 feincms3-4.0a1/feincms3/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    17160 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/admin.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    22711 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/applications.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2980 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/cleanse.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2593 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/embedding.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4894 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/inline_ckeditor.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5362 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7195 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/en/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3/locale/en/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4923 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/fr/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4993 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     8276 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/it/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3/locale/it/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2295 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7000 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/locale/nb_NO/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3/locale/nb_NO/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4005 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7890 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10156 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/mixins.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9296 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/pages.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.718573 feincms3-4.0a1/feincms3/plugins/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4898 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/external.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1482 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/html.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1988 2022-09-27 14:52:22.000000 feincms3-4.0a1/feincms3/plugins/image.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2110 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/old_richtext.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      829 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/richtext.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2934 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/plugins/snippet.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5435 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/regions.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    12838 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/renderer.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.718573 feincms3-4.0a1/feincms3/root/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/root/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4442 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/root/middleware.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1411 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/root/passthru.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2666 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/shortcuts.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.708573 feincms3-4.0a1/feincms3/static/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.748573 feincms3-4.0a1/feincms3/static/feincms3/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      574 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/box-drawing.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1934 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/inline-ckeditor.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1174 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/inline-ckeditor.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1158 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/move-form.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      193 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/plugin-ckeditor.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      680 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/static/feincms3/static-path-style.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.718573 feincms3-4.0a1/feincms3/templatetags/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/templatetags/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5438 2022-09-21 20:30:58.000000 feincms3-4.0a1/feincms3/templatetags/feincms3.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2671 2022-09-27 14:52:22.000000 feincms3-4.0a1/feincms3/utils.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-09-27 14:55:29.738573 feincms3-4.0a1/feincms3.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1858 2022-09-27 14:55:29.000000 feincms3-4.0a1/feincms3.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2161 2022-09-27 14:55:29.000000 feincms3-4.0a1/feincms3.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-09-27 14:55:29.000000 feincms3-4.0a1/feincms3.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-03-23 06:34:19.000000 feincms3-4.0a1/feincms3.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2022-09-27 14:55:29.000000 feincms3-4.0a1/feincms3.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        9 2022-09-27 14:55:29.000000 feincms3-4.0a1/feincms3.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1455 2022-09-27 14:55:29.748573 feincms3-4.0a1/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-03-23 06:34:04.000000 feincms3-4.0a1/setup.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/__init__.py
+-rw-r--r--   0        0        0    17199 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/admin.py
+-rw-r--r--   0        0        0    24163 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/applications.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/cleanse.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/embedding.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/inline_ckeditor.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/mixins.py
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/pages.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/regions.py
+-rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/renderer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/shortcuts.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/utils.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/__init__.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/external.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/html.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/image.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/old_richtext.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/richtext.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/plugins/snippet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/root/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/root/middleware.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/root/passthru.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/box-drawing.css
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/inline-ckeditor.css
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/inline-ckeditor.js
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/move-form.css
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/plugin-ckeditor.css
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/static/feincms3/static-path-style.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/templatetags/__init__.py
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 feincms3-4.1.0/feincms3/templatetags/feincms3.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-4.1.0/.gitignore
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-4.1.0/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-4.1.0/README.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 feincms3-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 feincms3-4.1.0/PKG-INFO
```

### Comparing `feincms3-4.0a1/LICENSE` & `feincms3-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/PKG-INFO` & `feincms3-4.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: feincms3
-Version: 4.0a1
+Version: 4.1.0
 Summary: CMS-building toolkit for Django
-Home-page: https://github.com/matthiask/feincms3/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
-License: BSD-3-Clause
-Platform: OS Independent
+Project-URL: Homepage, https://github.com/matthiask/feincms3/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -18,18 +17,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Dist: django-content-editor>=6.0
+Requires-Dist: django-js-asset>=2.0
+Requires-Dist: django-tree-queries>=0.15.0
+Requires-Dist: django>=3.2
 Provides-Extra: all
+Requires-Dist: django-imagefield; extra == 'all'
+Requires-Dist: html-sanitizer>=1.1.1; extra == 'all'
+Requires-Dist: requests; extra == 'all'
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Requires-Dist: django-ckeditor; extra == 'tests'
+Requires-Dist: requests-mock; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 ========
 feincms3
 ========
 
 .. image:: https://github.com/matthiask/feincms3/workflows/Tests/badge.svg
     :target: https://github.com/matthiask/feincms3/
```

### Comparing `feincms3-4.0a1/README.rst` & `feincms3-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/admin.py` & `feincms3-4.1.0/feincms3/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,20 +120,20 @@
         """
 
         info = self.model._meta.app_label, self.model._meta.model_name
         return [
             re_path(
                 r"^(.+)/move/$",
                 action_form_view_decorator(self)(self.move_view),
-                name="%s_%s_move" % info,
+                name="{}_{}_move".format(*info),
             ),
             re_path(
                 r"^(.+)/clone/$",
                 action_form_view_decorator(self)(self.clone_view),
-                name="%s_%s_clone" % info,
+                name="{}_{}_clone".format(*info),
             ),
         ] + super().get_urls()
 
     def move_view(self, request, obj):
         return self.action_form_view(
             request, obj, form_class=MoveForm, title=_("Move %s") % obj
         )
@@ -147,31 +147,31 @@
         kw = {"request": request, "obj": obj, "modeladmin": self}
         form = form_class(request.POST if request.method == "POST" else None, **kw)
         if form.is_valid():
             return form.process()
         return self.render_action_form(request, form, title=title, obj=obj)
 
     def render_action_form(self, request, form, *, title, obj):
-        adminForm = helpers.AdminForm(
+        adminform = helpers.AdminForm(
             form,
             [
                 (None, {"fields": form.fields.keys()})
             ],  # list(self.get_fieldsets(request, obj)),
             {},  # self.get_prepopulated_fields(request, obj),
             (),  # self.get_readonly_fields(request, obj),
             model_admin=self,
         )
-        media = self.media + adminForm.media
+        media = self.media + adminform.media
 
         context = dict(
             self.admin_site.each_context(request),
             title=title,
             object_id=obj.pk,
             original=obj,
-            adminform=adminForm,
+            adminform=adminform,
             errors=helpers.AdminErrorList(form, ()),
             preserved_filters=self.get_preserved_filters(request),
             media=media,
             is_popup=False,
             inline_admin_formsets=[],
             save_as_new=False,
             show_save_and_add_another=False,
@@ -432,15 +432,15 @@
             )
 
         if self.cleaned_data.get("_set_content"):
             from django.forms.models import _get_foreign_key  # Since 2009.
 
             for inline in self.modeladmin.inlines:
                 fk = _get_foreign_key(
-                    self.modeladmin.model, inline.model, inline.fk_name, False
+                    self.modeladmin.model, inline.model, inline.fk_name, can_fail=False
                 )
 
                 # Remove all existing instances
                 inline.model._default_manager.filter(**{fk.name: target}).delete()
 
                 for obj in inline.model._default_manager.filter(
                     **{fk.name: self.instance}
@@ -493,11 +493,11 @@
             )
         ]
 
     def queryset(self, request, queryset):
         if self.value():
             try:
                 node = queryset.model._default_manager.get(pk=self.value())
-            except (TypeError, ValueError, queryset.model.DoesNotExist):
-                raise IncorrectLookupParameters()
+            except (TypeError, ValueError, queryset.model.DoesNotExist) as exc:
+                raise IncorrectLookupParameters() from exc
             return queryset.descendants(node, include_self=True)
         return queryset
```

### Comparing `feincms3-4.0a1/feincms3/applications.py` & `feincms3-4.1.0/feincms3/applications.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 import re
 import sys
 from collections import Counter, defaultdict
 from importlib import import_module
 from types import ModuleType
 
 from asgiref.local import Local
+from asgiref.sync import iscoroutinefunction
 from content_editor.models import Type
 from django.conf import settings
 from django.core.checks import Error, Info, Warning
 from django.core.exceptions import ValidationError
 from django.core.signals import request_finished
 from django.db import models
 from django.db.models import Q, signals
-from django.urls import NoReverseMatch, include, re_path, reverse
+from django.urls import NoReverseMatch, include, path, re_path, reverse
+from django.utils.decorators import sync_and_async_middleware
 from django.utils.translation import get_language, gettext_lazy as _
 
 from feincms3.mixins import ChoicesCharField
 
 
 __all__ = (
     "PageTypeMixin",
@@ -65,16 +67,16 @@
         try:
             return reverse(viewname, urlconf, args, kwargs, *fargs, **fkwargs)
         except NoReverseMatch:
             pass
     if fallback is not _sentinel:
         return fallback
     raise NoReverseMatch(
-        "Reverse for any of '%s' with arguments '%s' and keyword arguments"
-        " '%s' not found." % ("', '".join(viewnames), args or [], kwargs or {})
+        "Reverse for any of '{}' with arguments '{}' and keyword arguments"
+        " '{}' not found.".format("', '".join(viewnames), args or [], kwargs or {})
     )
 
 
 def reverse_app(namespaces, viewname, *args, languages=None, **kwargs):
     """
     Reverse app URLs, preferring the active language.
 
@@ -169,14 +171,15 @@
     """
     try:
         return fn(*args, **kwargs)
     except NoReverseMatch:
         return fallback
 
 
+# Used in feincms3-sites
 def _del_apps_urlconf_cache(**kwargs):
     try:
         del _apps_urlconf_cache.cache
     except AttributeError:
         pass
 
 
@@ -218,54 +221,83 @@
     if apps is None:
         apps = getattr(_apps_urlconf_cache, "cache", None)
 
         if apps is None:
             fields = ("path", "page_type", "app_namespace", "language_code")
             apps = list(
                 _APPS_MODEL._default_manager.active()
-                .with_tree_fields(False)
+                .without_tree_fields()
                 .exclude(app_namespace="")
                 .values_list(*fields)
                 .order_by(*fields)
             )
             # NOTE! We *could* cache the module_name instead but we'd still
             # have to check if the module actually exists in the local Python
             # process.
             _apps_urlconf_cache.cache = apps
 
     if not apps:
         # No point wrapping ROOT_URLCONF if there are no additional URLs
         return settings.ROOT_URLCONF
 
+    return _build_apps_urlconf(apps)
+
+
+async def apps_urlconf_async(*, apps=None):
+    if apps is None:
+        apps = getattr(_apps_urlconf_cache, "cache", None)
+
+        if apps is None:
+            fields = ("path", "page_type", "app_namespace", "language_code")
+            apps = [
+                row
+                async for row in _APPS_MODEL._default_manager.active()
+                .without_tree_fields()
+                .exclude(app_namespace="")
+                .values_list(*fields)
+                .order_by(*fields)
+            ]
+            # NOTE! We *could* cache the module_name instead but we'd still
+            # have to check if the module actually exists in the local Python
+            # process.
+            _apps_urlconf_cache.cache = apps
+
+    if not apps:
+        # No point wrapping ROOT_URLCONF if there are no additional URLs
+        return settings.ROOT_URLCONF
+
+    return _build_apps_urlconf(apps)
+
+
+def _build_apps_urlconf(apps):
     key = ",".join(itertools.chain.from_iterable(apps))
     module_name = "urlconf_%s" % hashlib.md5(key.encode("utf-8")).hexdigest()
 
     if module_name not in sys.modules:
         types = {app.key: app for app in _APPS_MODEL.TYPES if app.get("urlconf")}
 
         m = ModuleType(module_name)
 
         mapping = defaultdict(list)
-        for path, page_type, app_namespace, language_code in apps:
+        for app_path, page_type, app_namespace, language_code in apps:
             if page_type not in types:
                 continue
             mapping[language_code].append(
                 re_path(
-                    r"^%s" % re.escape(path.lstrip("/")),
+                    r"^%s" % re.escape(app_path.lstrip("/")),
                     include(types[page_type]["urlconf"], namespace=app_namespace),
                 )
             )
 
         m.urlpatterns = [
-            re_path(
-                r"",
+            path(
+                "",
                 include(
                     (instances, _APPS_MODEL.LANGUAGE_CODES_NAMESPACE),
-                    namespace="%s-%s"
-                    % (_APPS_MODEL.LANGUAGE_CODES_NAMESPACE, language_code),
+                    namespace=f"{_APPS_MODEL.LANGUAGE_CODES_NAMESPACE}-{language_code}",
                 ),
             )
             for language_code, instances in mapping.items()
         ]
 
         # Append patterns from ROOT_URLCONF instead of including them because
         # i18n_patterns only work in the root URLconf.
@@ -313,25 +345,34 @@
         language_code=request.resolver_match.namespaces[0][
             len(_APPS_MODEL.LANGUAGE_CODES_NAMESPACE) + 1 :
         ],
         app_namespace=request.resolver_match.namespaces[1],
     )
 
 
+@sync_and_async_middleware
 def apps_middleware(get_response):
     """
     This middleware must be put in ``MIDDLEWARE``; it simply assigns
     the return value of :func:`~feincms3.applications.apps_urlconf` to
     ``request.urlconf``. This middleware should probably be one of the first
     since it has to run before any resolving happens.
     """
 
-    def middleware(request):
-        request.urlconf = apps_urlconf()
-        return get_response(request)
+    if iscoroutinefunction(get_response):
+
+        async def middleware(request):
+            request.urlconf = await apps_urlconf_async()
+            return await get_response(request)
+
+    else:
+
+        def middleware(request):
+            request.urlconf = apps_urlconf()
+            return get_response(request)
 
     return middleware
 
 
 class TemplateType(Type):
     """
     Template page type
@@ -493,36 +534,36 @@
     app_namespace = models.CharField(
         ("app instance namespace"), max_length=100, blank=True, editable=False
     )
 
     class Meta:
         abstract = True
 
+    def save(self, *args, **kwargs):
+        """
+        Updates ``app_namespace``.
+        """
+        self.app_namespace = self.type.app_namespace(self)
+        super().save(*args, **kwargs)
+
+    save.alters_data = True
+
     @property
     def type(self):
         """
         Returns the appropriate page type instance, either the selected type or
         the first type in the list of ``TYPES`` if no type is selected or if
         the type does not exist anymore.
         """
         return self.TYPES_DICT.get(self.page_type, self.TYPES[0])
 
     @property
     def regions(self):
         return self.type.regions
 
-    def save(self, *args, **kwargs):
-        """
-        Updates ``app_namespace``.
-        """
-        self.app_namespace = self.type.app_namespace(self)
-        super().save(*args, **kwargs)
-
-    save.alters_data = True
-
     def clean_fields(self, exclude=None):
         """
         Checks that required fields are given and that an app namespace only
         exists once per site and language.
         """
         exclude = [] if exclude is None else exclude
         super().clean_fields(exclude)
@@ -551,15 +592,17 @@
                 Q(language_code=self.language_code),
                 ~Q(pk=self.pk),
             ).exists():
                 fields = ["__all__", "page_type"]
                 fields.extend(type.get("required_fields", ()))
                 raise ValidationError(
                     {
-                        field: _("This exact app already exists.")
+                        field: _(
+                            'The page type "{page_type}" with the specified configuration exists already.'
+                        ).format(page_type=type.title)
                         for field in fields
                         if field not in exclude
                     }
                 )
 
     @staticmethod
     def fill_page_type_choices(sender, **kwargs):
```

### Comparing `feincms3-4.0a1/feincms3/cleanse.py` & `feincms3-4.1.0/feincms3/cleanse.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/embedding.py` & `feincms3-4.1.0/feincms3/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/inline_ckeditor.py` & `feincms3-4.1.0/feincms3/inline_ckeditor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 
+import django
 from django import forms
 from django.conf import settings
 from django.db import models
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 from html_sanitizer.django import get_sanitizer
 from js_asset import JS
 
 
 __all__ = ["InlineCKEditorField"]
 
 
 CKEDITOR_JS_URL = JS(
-    "https://cdn.ckeditor.com/4.19.1/full/ckeditor.js",
+    "https://cdn.ckeditor.com/4.20.1/full/ckeditor.js",
     {
         # "integrity": "sha384-qdzSU+GzmtYP2hzdmYowu+mz86DPHVROVcDAPdT/ePp1E8ke2z0gy7ITERtHzPmJ",  # noqa
         "crossorigin": "anonymous",
         "defer": "defer",
     },
 )
 CKEDITOR_CONFIG = {
@@ -120,14 +121,16 @@
 class InlineCKEditorWidget(forms.Textarea):
     def __init__(self, *args, **kwargs):
         self.ckeditor = kwargs.pop("ckeditor") or CKEDITOR_JS_URL
         self.config = kwargs.pop("config") or CKEDITOR_CONFIG["default"]
 
         attrs = kwargs.setdefault("attrs", {})
         attrs["data-inline-cke"] = id(self.config)
+        if django.VERSION < (4, 2):
+            attrs["data-inline-cke-dj41"] = True
         super().__init__(*args, **kwargs)
 
     @property
     def media(self):
         return forms.Media(
             css={"all": ["feincms3/inline-ckeditor.css"]},
             js=[
```

### Comparing `feincms3-4.0a1/feincms3/locale/de/LC_MESSAGES/django.mo` & `feincms3-4.1.0/feincms3/locale/de/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -68,18 +68,14 @@
 
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Objekte in der primären Sprache können nicht eine Übersetzung eines anderen "
 "Objektes sein."
 
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-"Objekte können nur Übersetzungen sein von Objekten in der primären Sprache."
-
 msgid "Only set one redirect value."
 msgstr "Bitte nur einen Weiterleitungs-Wert setzen."
 
 msgid "Path must start and end with a slash (/)."
 msgstr "Pfad muss mit einem Slash (/) starten und enden."
 
 msgid "Position is expected to be greater than zero."
@@ -109,16 +105,20 @@
 
 msgid "The node %(node)s has been moved to the new position."
 msgstr "%(node)s wurde zur neuen Position verschoben."
 
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr "Der Pfad %(path)s der Seite %(page)s würde nicht eindeutig sein."
 
-msgid "This exact app already exists."
-msgstr "Diese exakte Anwendung existiert bereits."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
+"Der Seitentyp \"{page_type}\" mit der spezifizierten Konfiguration existiert "
+"schon."
 
 msgid "This field is required for the page type \"%s\"."
 msgstr "Dieses Feld wird für den Seitentyp \"%s\" benötigt."
 
 msgid "URL"
 msgstr "URL"
```

### Comparing `feincms3-4.0a1/feincms3/locale/de/LC_MESSAGES/django.po` & `feincms3-4.1.0/feincms3/locale/de/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -5,296 +5,305 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-03-16 10:34+0100\n"
+"POT-Creation-Date: 2023-02-02 17:10+0100\n"
 "PO-Revision-Date: 2020-12-04 09:43+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/feincms3/feincms3/"
 "de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:97 pages.py:60
+#: admin.py:98 pages.py:69
 msgid "title"
 msgstr "Titel"
 
-#: admin.py:111
+#: admin.py:112
 msgid "move"
 msgstr "verschieben"
 
-#: admin.py:137
+#: admin.py:138
 #, python-format
 msgid "Move %s"
 msgstr "%s verschieben"
 
-#: admin.py:142
+#: admin.py:143
 #, python-format
 msgid "Clone %s"
 msgstr "%s klonen"
 
-#: admin.py:211
+#: admin.py:212
 msgid "New location"
 msgstr "Neuer Ort"
 
-#: admin.py:219
+#: admin.py:220
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
 "Verschieben ist nicht möglich weil es keine gültigen Zielorte gibt. "
 "Vielleicht den einzigen Wurzelknoten gewählt?"
 
-#: admin.py:265 admin.py:276 admin.py:286
+#: admin.py:266 admin.py:277 admin.py:287
 msgid "move here"
 msgstr "hierhin verschieben"
 
-#: admin.py:344
+#: admin.py:345
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr "%(node)s wurde zur neuen Position verschoben."
 
-#: admin.py:362
+#: admin.py:363
 msgid "target"
 msgstr "Ziel"
 
-#: admin.py:372
+#: admin.py:373
 msgid "Replace target's content"
 msgstr "Inhalt des Ziels ersetzen"
 
-#: admin.py:374
+#: admin.py:375
 #, python-format
 msgid "Affects the following models: %s."
 msgstr "Betrifft die folgenden Inhalte: %s."
 
-#: admin.py:396
+#: admin.py:397
 #, python-format
 msgid "Current: \"%s\""
 msgstr "Aktuell: „%s“"
 
-#: admin.py:406
+#: admin.py:407
 msgid "Cannot clone node to itself."
 msgstr "Kann Knoten nicht zu sich selbst klonen."
 
-#: admin.py:429
+#: admin.py:430
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr "Aktualisierte Felder von %(node)s: %(fields)s"
 
-#: admin.py:453
+#: admin.py:454
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr "Ersetzte den Inhalt von %(target)s mit dem Inhalt von %(source)s."
 
-#: admin.py:482
+#: admin.py:481
 msgid "subtree"
 msgstr "Unterbaum"
 
-#: applications.py:389
+#: applications.py:492
 msgid "page type"
 msgstr "Seitentyp"
 
-#: applications.py:436
+#: applications.py:536
 #, python-format
 msgid "This field is required for the page type \"%s\"."
 msgstr "Dieses Feld wird für den Seitentyp \"%s\" benötigt."
 
-#: applications.py:460
-msgid "This exact app already exists."
-msgstr "Diese exakte Anwendung existiert bereits."
+#: applications.py:558
+#, python-brace-format
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
+"Der Seitentyp \"{page_type}\" mit der spezifizierten Konfiguration existiert "
+"schon."
 
-#: mixins.py:18
+#: mixins.py:20
 msgid "menu"
 msgstr "Menü"
 
-#: mixins.py:51 plugins/snippet.py:32
+#: mixins.py:72 plugins/snippet.py:33
 msgid "template"
 msgstr "Vorlage"
 
-#: mixins.py:97
+#: mixins.py:123
 msgid "language"
 msgstr "Sprache"
 
-#: mixins.py:127
+#: mixins.py:153
 msgid "translation of"
 msgstr "Übersetzung von"
 
-#: mixins.py:168
+#: mixins.py:214
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Objekte in der primären Sprache können nicht eine Übersetzung eines anderen "
 "Objektes sein."
 
-#: mixins.py:181
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-"Objekte können nur Übersetzungen sein von Objekten in der primären Sprache."
-
-#: mixins.py:194
+#: mixins.py:228
 msgid "Redirect to URL"
 msgstr "Weiterleiten zu URL"
 
-#: mixins.py:201
+#: mixins.py:236
 msgid "Redirect to page"
 msgstr "Weiterleiten zu Seite"
 
-#: mixins.py:224
+#: mixins.py:259
 msgid "Only set one redirect value."
 msgstr "Bitte nur einen Weiterleitungs-Wert setzen."
 
-#: mixins.py:232
+#: mixins.py:267
 msgid "Cannot redirect to self."
 msgstr "Kann nicht zu sich selbst weiterleiten."
 
-#: mixins.py:243
+#: mixins.py:278
 #, python-format
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
 "Die gewählte Seite „%(title)s“ leitet schon weiter auf „%(path)s“ weiter, "
 "bitte Verkettungen von Weiterleitungen vermeiden."
 
-#: mixins.py:260
+#: mixins.py:295
 #, python-format
 msgid ""
 "Do not chain redirects. The following pages already redirect to this page: "
 "%(pages)s"
 msgstr ""
 "Verkettung von Weiterleitungen nicht erlaubt. Die folgenden Seiten leiten "
 "schon auf diese Seite weiter: %(pages)s"
 
-#: pages.py:59
+#: pages.py:68
 msgid "is active"
 msgstr "ist aktiv"
 
-#: pages.py:61
+#: pages.py:70
 msgid "slug"
 msgstr "Slug"
 
-#: pages.py:68
+#: pages.py:77
 msgid "Position is expected to be greater than zero."
 msgstr "Position sollte grösser als Null sein."
 
-#: pages.py:75
+#: pages.py:84
 msgid "path"
 msgstr "Pfad"
 
-#: pages.py:80
+#: pages.py:89
 msgid ""
 "Automatically generated by concatenating the parent's path and the slug "
 "unless the path is defined manually."
 msgstr ""
 "Wird automatisch generiert durch das Aneinananderhängen des Pfades der "
 "übergeordneten Seite und des Slugs, ausser wenn der Pfad manuell definiert "
 "wird."
 
-#: pages.py:86
+#: pages.py:95
 msgid "Path must start and end with a slash (/)."
 msgstr "Pfad muss mit einem Slash (/) starten und enden."
 
-#: pages.py:90
+#: pages.py:99
 msgid "manually define the path"
 msgstr "Pfad manuell definieren"
 
-#: pages.py:97
+#: pages.py:106
 msgid "page"
 msgstr "Seite"
 
-#: pages.py:98
+#: pages.py:107
 msgid "pages"
 msgstr "Seiten"
 
-#: pages.py:140
+#: pages.py:149
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr "Statische Pfade können nicht leer sein. Meinten Sie „/“?"
 
-#: pages.py:160
+#: pages.py:171
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr "Der Pfad %(path)s der Seite %(page)s würde nicht eindeutig sein."
 
-#: plugins/external.py:108
+#: plugins/external.py:113
 msgid "URL"
 msgstr "URL"
 
-#: plugins/external.py:110 plugins/image.py:40
+#: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
 msgstr "alternativer Text"
 
-#: plugins/external.py:111 plugins/image.py:41
+#: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
 msgstr "Beschreibung der Bildinhalte, zB für Screenreader."
 
-#: plugins/external.py:115 plugins/image.py:45
+#: plugins/external.py:120 plugins/image.py:47
 msgid "caption"
 msgstr "Legende"
 
-#: plugins/external.py:119
+#: plugins/external.py:124
 msgid "external content"
 msgstr "externer Inhalt"
 
-#: plugins/external.py:135
+#: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr "Kann das HTML für diese URL nicht laden, tut mir leid!"
 
 #: plugins/html.py:26
 msgid ""
 "The content will be inserted directly into the page. It is VERY important "
 "that the HTML snippet is well-formed!"
 msgstr ""
 "Der Inhalt wird direkt in die Seite eingefügt. Es ist SEHR wichtig, dass das "
 "HTML gültig ist!"
 
-#: plugins/image.py:24 plugins/image.py:49
+#: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr "Bild"
 
-#: plugins/image.py:33
+#: plugins/image.py:35
 msgid "image width"
 msgstr "Bildbreite"
 
-#: plugins/image.py:36
+#: plugins/image.py:38
 msgid "image height"
 msgstr "Bildhöhe"
 
-#: plugins/image.py:38
+#: plugins/image.py:40
 msgid "primary point of interest"
 msgstr "Fokuspunkt"
 
-#: plugins/image.py:50
+#: plugins/image.py:52
 msgid "images"
 msgstr "Bilder"
 
-#: plugins/richtext.py:30
+#: plugins/old_richtext.py:40 plugins/richtext.py:20
 msgid "text"
 msgstr "Text"
 
-#: plugins/richtext.py:34
+#: plugins/old_richtext.py:44 plugins/richtext.py:24
 msgid "rich text"
 msgstr "Text"
 
-#: plugins/richtext.py:35
+#: plugins/old_richtext.py:45 plugins/richtext.py:25
 msgid "rich texts"
 msgstr "Texte"
 
-#: plugins/snippet.py:39
+#: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr "vordefinierter Baustein"
 
-#: plugins/snippet.py:40
+#: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr "vordefinierte Bausteine"
 
+#~ msgid "This exact app already exists."
+#~ msgstr "Diese exakte Anwendung existiert bereits."
+
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Objekte können nur Übersetzungen sein von Objekten in der primären "
+#~ "Sprache."
+
 #~ msgid "Generated automatically if 'static path' is unset."
 #~ msgstr "Automatisch generiert falls „statischer Pfad“ nicht gesetzt ist."
 
 #~ msgid "static path"
 #~ msgstr "statischer Pfad"
```

### Comparing `feincms3-4.0a1/feincms3/locale/en/LC_MESSAGES/django.po` & `feincms3-4.1.0/feincms3/locale/en/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,274 +4,273 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-03-16 10:34+0100\n"
+"POT-Creation-Date: 2023-02-02 17:10+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:97 pages.py:60
+#: admin.py:98 pages.py:69
 msgid "title"
 msgstr ""
 
-#: admin.py:111
+#: admin.py:112
 msgid "move"
 msgstr ""
 
-#: admin.py:137
+#: admin.py:138
 #, python-format
 msgid "Move %s"
 msgstr ""
 
-#: admin.py:142
+#: admin.py:143
 #, python-format
 msgid "Clone %s"
 msgstr ""
 
-#: admin.py:211
+#: admin.py:212
 msgid "New location"
 msgstr ""
 
-#: admin.py:219
+#: admin.py:220
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
 
-#: admin.py:265 admin.py:276 admin.py:286
+#: admin.py:266 admin.py:277 admin.py:287
 msgid "move here"
 msgstr ""
 
-#: admin.py:344
+#: admin.py:345
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 msgid "target"
 msgstr ""
 
-#: admin.py:372
+#: admin.py:373
 msgid "Replace target's content"
 msgstr ""
 
-#: admin.py:374
+#: admin.py:375
 #, python-format
 msgid "Affects the following models: %s."
 msgstr ""
 
-#: admin.py:396
+#: admin.py:397
 #, python-format
 msgid "Current: \"%s\""
 msgstr ""
 
-#: admin.py:406
+#: admin.py:407
 msgid "Cannot clone node to itself."
 msgstr ""
 
-#: admin.py:429
+#: admin.py:430
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr ""
 
-#: admin.py:453
+#: admin.py:454
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr ""
 
-#: admin.py:482
+#: admin.py:481
 msgid "subtree"
 msgstr ""
 
-#: applications.py:389
+#: applications.py:492
 msgid "page type"
 msgstr ""
 
-#: applications.py:436
+#: applications.py:536
 #, python-format
 msgid "This field is required for the page type \"%s\"."
 msgstr ""
 
-#: applications.py:460
-msgid "This exact app already exists."
+#: applications.py:558
+#, python-brace-format
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
 msgstr ""
 
-#: mixins.py:18
+#: mixins.py:20
 msgid "menu"
 msgstr ""
 
-#: mixins.py:51 plugins/snippet.py:32
+#: mixins.py:72 plugins/snippet.py:33
 msgid "template"
 msgstr ""
 
-#: mixins.py:97
+#: mixins.py:123
 msgid "language"
 msgstr ""
 
-#: mixins.py:127
+#: mixins.py:153
 msgid "translation of"
 msgstr ""
 
-#: mixins.py:168
+#: mixins.py:214
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 
-#: mixins.py:181
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-
-#: mixins.py:194
+#: mixins.py:228
 msgid "Redirect to URL"
 msgstr ""
 
-#: mixins.py:201
+#: mixins.py:236
 msgid "Redirect to page"
 msgstr ""
 
-#: mixins.py:224
+#: mixins.py:259
 msgid "Only set one redirect value."
 msgstr ""
 
-#: mixins.py:232
+#: mixins.py:267
 msgid "Cannot redirect to self."
 msgstr ""
 
-#: mixins.py:243
+#: mixins.py:278
 #, python-format
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
 
-#: mixins.py:260
+#: mixins.py:295
 #, python-format
 msgid ""
 "Do not chain redirects. The following pages already redirect to this page: "
 "%(pages)s"
 msgstr ""
 
-#: pages.py:59
+#: pages.py:68
 msgid "is active"
 msgstr ""
 
-#: pages.py:61
+#: pages.py:70
 msgid "slug"
 msgstr ""
 
-#: pages.py:68
+#: pages.py:77
 msgid "Position is expected to be greater than zero."
 msgstr ""
 
-#: pages.py:75
+#: pages.py:84
 msgid "path"
 msgstr ""
 
-#: pages.py:80
+#: pages.py:89
 msgid ""
 "Automatically generated by concatenating the parent's path and the slug "
 "unless the path is defined manually."
 msgstr ""
 
-#: pages.py:86
+#: pages.py:95
 msgid "Path must start and end with a slash (/)."
 msgstr ""
 
-#: pages.py:90
+#: pages.py:99
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:97
+#: pages.py:106
 msgid "page"
 msgstr ""
 
-#: pages.py:98
+#: pages.py:107
 msgid "pages"
 msgstr ""
 
-#: pages.py:140
+#: pages.py:149
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr ""
 
-#: pages.py:160
+#: pages.py:171
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr ""
 
-#: plugins/external.py:108
+#: plugins/external.py:113
 msgid "URL"
 msgstr ""
 
-#: plugins/external.py:110 plugins/image.py:40
+#: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
 msgstr ""
 
-#: plugins/external.py:111 plugins/image.py:41
+#: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
 msgstr ""
 
-#: plugins/external.py:115 plugins/image.py:45
+#: plugins/external.py:120 plugins/image.py:47
 msgid "caption"
 msgstr ""
 
-#: plugins/external.py:119
+#: plugins/external.py:124
 msgid "external content"
 msgstr ""
 
-#: plugins/external.py:135
+#: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr ""
 
 #: plugins/html.py:26
 msgid ""
 "The content will be inserted directly into the page. It is VERY important "
 "that the HTML snippet is well-formed!"
 msgstr ""
 
-#: plugins/image.py:24 plugins/image.py:49
+#: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr ""
 
-#: plugins/image.py:33
+#: plugins/image.py:35
 msgid "image width"
 msgstr ""
 
-#: plugins/image.py:36
+#: plugins/image.py:38
 msgid "image height"
 msgstr ""
 
-#: plugins/image.py:38
+#: plugins/image.py:40
 msgid "primary point of interest"
 msgstr ""
 
-#: plugins/image.py:50
+#: plugins/image.py:52
 msgid "images"
 msgstr ""
 
-#: plugins/richtext.py:30
+#: plugins/old_richtext.py:40 plugins/richtext.py:20
 msgid "text"
 msgstr ""
 
-#: plugins/richtext.py:34
+#: plugins/old_richtext.py:44 plugins/richtext.py:24
 msgid "rich text"
 msgstr ""
 
-#: plugins/richtext.py:35
+#: plugins/old_richtext.py:45 plugins/richtext.py:25
 msgid "rich texts"
 msgstr ""
 
-#: plugins/snippet.py:39
+#: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
-#: plugins/snippet.py:40
+#: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
```

### Comparing `feincms3-4.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo` & `feincms3-4.1.0/feincms3/locale/fr/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -60,19 +60,14 @@
 
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Les objets dans la langue principale ne peuvent pas être la traduction d’un "
 "autre objet."
 
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-"Les objets peuvent seulement être la traduction d’objets dans la langue "
-"principale."
-
 msgid "Only set one redirect value."
 msgstr "Définissez une seule valeur de redirection."
 
 msgid "Path must start and end with a slash (/)."
 msgstr "Le chemin doit commencer et se terminer par une barre oblique (/)."
 
 msgid "Position is expected to be greater than zero."
@@ -103,17 +98,14 @@
 
 msgid "The node %(node)s has been moved to the new position."
 msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
 
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr "Le nouveau chemin %(path)s de la page %(page)s ne serait pas unique."
 
-msgid "This exact app already exists."
-msgstr "Cette application exacte existe déjà."
-
 msgid "This field is required for the page type \"%s\"."
 msgstr "Ce champ est obligatoire pour le type de page \"%s\"."
 
 msgid "URL"
 msgstr "URL"
 
 msgid "Unable to fetch HTML for this URL, sorry!"
```

### Comparing `feincms3-4.0a1/feincms3/locale/fr/LC_MESSAGES/django.po` & `feincms3-4.1.0/feincms3/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -5,318 +5,324 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-03-16 10:34+0100\n"
-"PO-Revision-Date: 2020-12-04 09:43+0000\n"
-"Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
-"Language-Team: French <https://hosted.weblate.org/projects/feincms3/feincms3/"
-"fr/>\n"
-"Language: fr\n"
+"POT-Creation-Date: 2023-02-02 17:10+0100\n"
+"PO-Revision-Date: 2020-12-04 09:46+0000\n"
+"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
+"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
+"feincms3/feincms3/nb_NO/>\n"
+"Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:97 pages.py:60
+#: admin.py:98 pages.py:69
 msgid "title"
-msgstr "titre"
+msgstr "tittel"
 
-#: admin.py:111
+#: admin.py:112
 msgid "move"
-msgstr "déplacer"
+msgstr "flytt"
 
-#: admin.py:137
+#: admin.py:138
 #, python-format
 msgid "Move %s"
-msgstr "Déplacer %s"
+msgstr "Flytt %s"
 
-#: admin.py:142
+#: admin.py:143
 #, python-format
 msgid "Clone %s"
-msgstr "Cloner %s"
+msgstr "Klon %s"
 
-#: admin.py:211
+#: admin.py:212
 msgid "New location"
-msgstr "Nouvel emplacement"
+msgstr "Ny plassering"
 
-#: admin.py:219
+#: admin.py:220
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
-"Le déplacement n’est pas possible car il n’y a pas de cibles valides. Peut-"
-"être avez-vous sélectionné le seul nœud racine ?"
+"Flytting er ikke mulig fordi det ikke er noen gyldige mål. Kanskje du valgte "
+"den eneste rotnoden?"
 
-#: admin.py:265 admin.py:276 admin.py:286
+#: admin.py:266 admin.py:277 admin.py:287
 msgid "move here"
-msgstr "déplacer ici"
+msgstr "flytt hit"
 
-#: admin.py:344
+#: admin.py:345
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
-msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
+msgstr "Noden %(node)s har blitt flyttet til ny plassering"
 
-#: admin.py:362
+#: admin.py:363
 msgid "target"
-msgstr "cible"
+msgstr "mål"
 
-#: admin.py:372
+#: admin.py:373
 msgid "Replace target's content"
-msgstr "Remplacer le contenu de la cible"
+msgstr "Erstatt målets innhold"
 
-#: admin.py:374
+#: admin.py:375
 #, python-format
 msgid "Affects the following models: %s."
-msgstr "Affecte les modèles suivants : %s."
+msgstr "Har innvirkning på følgende moduler: %s."
 
-#: admin.py:396
+#: admin.py:397
 #, python-format
 msgid "Current: \"%s\""
-msgstr "Actuel : « %s »"
+msgstr "Nåværende: «%s»"
 
-#: admin.py:406
+#: admin.py:407
 msgid "Cannot clone node to itself."
-msgstr "Impossible de cloner le nœud sur lui-même."
+msgstr "Kan ikke klone node til seg selv."
 
-#: admin.py:429
+#: admin.py:430
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
-msgstr "Champs mis à jour de %(node)s : %(fields)s"
+msgstr "Oppdaterte felter tilhørende %(node)s: %(fields)s"
 
-#: admin.py:453
+#: admin.py:454
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
-msgstr "Remplacement du contenu de %(target)s par le contenu de %(source)s."
+msgstr "Erstattet innholdet i %(target)s med innholdet i %(source)s."
 
-#: admin.py:482
+#: admin.py:481
 msgid "subtree"
 msgstr ""
 
-#: applications.py:389
+#: applications.py:492
+#, fuzzy
+#| msgid "page"
 msgid "page type"
-msgstr "type de page"
+msgstr "side"
 
-#: applications.py:436
-#, python-format
+#: applications.py:536
+#, fuzzy, python-format
+#| msgid "This field is required for the application %s."
 msgid "This field is required for the page type \"%s\"."
-msgstr "Ce champ est obligatoire pour le type de page \"%s\"."
+msgstr "Dette feltet kreves for programmet %s."
 
-#: applications.py:460
-msgid "This exact app already exists."
-msgstr "Cette application exacte existe déjà."
+#: applications.py:558
+#, python-brace-format
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
 
-#: mixins.py:18
+#: mixins.py:20
 msgid "menu"
-msgstr "menu"
+msgstr "meny"
 
-#: mixins.py:51 plugins/snippet.py:32
+#: mixins.py:72 plugins/snippet.py:33
 msgid "template"
-msgstr "modèle"
+msgstr "mal"
 
-#: mixins.py:97
+#: mixins.py:123
 msgid "language"
-msgstr "langue"
+msgstr "språk"
 
-#: mixins.py:127
+#: mixins.py:153
 msgid "translation of"
-msgstr "traduction de"
+msgstr "oversettelse av"
 
-#: mixins.py:168
+#: mixins.py:214
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
-"Les objets dans la langue principale ne peuvent pas être la traduction d’un "
-"autre objet."
-
-#: mixins.py:181
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-"Les objets peuvent seulement être la traduction d’objets dans la langue "
-"principale."
+"Objekter i primærspråket kan ikke være oversettelsen av et annet objekt."
 
-#: mixins.py:194
+#: mixins.py:228
 msgid "Redirect to URL"
-msgstr "Rediriger vers l’URL"
+msgstr "Videresendt til nettadresse"
 
-#: mixins.py:201
+#: mixins.py:236
 msgid "Redirect to page"
-msgstr "Rediriger vers la page"
+msgstr "Videresendt til side"
 
-#: mixins.py:224
+#: mixins.py:259
 msgid "Only set one redirect value."
-msgstr "Définissez une seule valeur de redirection."
+msgstr "Kun sett én videresendingsverdi."
 
-#: mixins.py:232
+#: mixins.py:267
 msgid "Cannot redirect to self."
-msgstr "Impossible de rediriger vers soi."
+msgstr "Kan ikke videresende til seg selv."
 
-#: mixins.py:243
+#: mixins.py:278
 #, python-format
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
-"Ne pas enchaîner les redirections. La page sélectionnée « %(title)s » "
-"redirige vers « %(path)s »."
+"Kan ikke opprette videresendelser i stafett. Valgt side «%(title)s» "
+"videresender til «%(path)s»."
 
-#: mixins.py:260
+#: mixins.py:295
 #, python-format
 msgid ""
 "Do not chain redirects. The following pages already redirect to this page: "
 "%(pages)s"
 msgstr ""
-"Ne pas enchaîner les redirections. Les pages suivantes redirigent déjà vers "
-"cette page : %(pages)s"
+"Ikke opprett videresendelser i stafett. Følgende sider videresender til "
+"denne siden: %(pages)s"
 
-#: pages.py:59
+#: pages.py:68
 msgid "is active"
-msgstr "est actif"
+msgstr "er aktiv"
 
-#: pages.py:61
+#: pages.py:70
 msgid "slug"
-msgstr "slug"
+msgstr ""
 
-#: pages.py:68
+#: pages.py:77
 msgid "Position is expected to be greater than zero."
-msgstr "La position devrait être supérieure à zéro."
+msgstr "Posisjonen forventes å være større enn null."
 
-#: pages.py:75
+#: pages.py:84
 msgid "path"
-msgstr "chemin"
+msgstr "sti"
 
-#: pages.py:80
+#: pages.py:89
 msgid ""
 "Automatically generated by concatenating the parent's path and the slug "
 "unless the path is defined manually."
 msgstr ""
 
-#: pages.py:86
+#: pages.py:95
 msgid "Path must start and end with a slash (/)."
-msgstr "Le chemin doit commencer et se terminer par une barre oblique (/)."
+msgstr "Sti må starte og slutt med skråstrek (/)."
 
-#: pages.py:90
+#: pages.py:99
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:97
+#: pages.py:106
 msgid "page"
-msgstr "page"
+msgstr "side"
 
-#: pages.py:98
+#: pages.py:107
 msgid "pages"
-msgstr "pages"
+msgstr "sider"
 
-#: pages.py:140
+#: pages.py:149
 msgid "Static paths cannot be empty. Did you mean '/'?"
-msgstr ""
-"Les chemins statiques ne peuvent pas être vides. Vouliez-vous dire « / » ?"
+msgstr "Statiske stier må fylles ut. Mente du «/»?"
 
-#: pages.py:160
+#: pages.py:171
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
-msgstr "Le nouveau chemin %(path)s de la page %(page)s ne serait pas unique."
+msgstr "Siden «%(page)s» sin nye sti %(path)s finnes allerede."
 
-#: plugins/external.py:108
+#: plugins/external.py:113
 msgid "URL"
-msgstr "URL"
+msgstr "Nettadresse"
 
-#: plugins/external.py:110 plugins/image.py:40
+#: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
-msgstr "texte alternatif"
+msgstr ""
 
-#: plugins/external.py:111 plugins/image.py:41
+#: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
-msgstr "Décrit les contenus de l’image, par ex. pour un lecteur d’écran."
+msgstr ""
 
-#: plugins/external.py:115 plugins/image.py:45
+#: plugins/external.py:120 plugins/image.py:47
+#, fuzzy
 #| msgid "application"
 msgid "caption"
-msgstr "légende"
+msgstr "program"
 
-#: plugins/external.py:119
+#: plugins/external.py:124
 msgid "external content"
-msgstr "contenu externe"
+msgstr "eksternt innhold"
 
-#: plugins/external.py:135
+#: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
-msgstr "Impossible de récupérer le HTML pour cette URL, désolé !"
+msgstr "Klarte ikke å hente HTML for denne nettadressen."
 
 #: plugins/html.py:26
 msgid ""
 "The content will be inserted directly into the page. It is VERY important "
 "that the HTML snippet is well-formed!"
 msgstr ""
-"Le contenu sera inséré directement dans la page. Il est TRÈS important que "
-"l’extrait de code HTML soit bien formé !"
 
-#: plugins/image.py:24 plugins/image.py:49
+#: plugins/image.py:26 plugins/image.py:51
 msgid "image"
-msgstr "image"
+msgstr "bilde"
 
-#: plugins/image.py:33
+#: plugins/image.py:35
 msgid "image width"
-msgstr "Largeur de l’image"
+msgstr "bildebredde"
 
-#: plugins/image.py:36
+#: plugins/image.py:38
 msgid "image height"
-msgstr "hauteur de l’image"
+msgstr "bildehøyde"
 
-#: plugins/image.py:38
+#: plugins/image.py:40
 msgid "primary point of interest"
-msgstr "principal point d’intérêt"
+msgstr "hoved-interessepunkt"
 
-#: plugins/image.py:50
+#: plugins/image.py:52
 msgid "images"
-msgstr "images"
+msgstr "bilder"
 
-#: plugins/richtext.py:30
+#: plugins/old_richtext.py:40 plugins/richtext.py:20
 msgid "text"
-msgstr "texte"
+msgstr "tekst"
 
-#: plugins/richtext.py:34
+#: plugins/old_richtext.py:44 plugins/richtext.py:24
+#, fuzzy
 msgid "rich text"
-msgstr "texte riche"
+msgstr "rikholdig tekst"
 
-#: plugins/richtext.py:35
+#: plugins/old_richtext.py:45 plugins/richtext.py:25
+#, fuzzy
 msgid "rich texts"
-msgstr "textes riches"
+msgstr "rikholdige tekster"
 
-#: plugins/snippet.py:39
+#: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
-#: plugins/snippet.py:40
+#: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
+#~ msgid "This exact app already exists."
+#~ msgstr "Akkurat dette programmet finnes allerede."
+
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr "Objekter kan kun være oversettelser av objekter i primærspråk."
+
 #~ msgid "Generated automatically if 'static path' is unset."
-#~ msgstr "Généré automatiquement si le « chemin statique » n’est pas défini."
+#~ msgstr "Generert automatisk hvis «statisk sti» ikke er valgt."
 
 #~ msgid "static path"
-#~ msgstr "chemin statique"
+#~ msgstr "statisk sti"
 
 #~ msgid "snippet"
-#~ msgstr "extrait"
+#~ msgstr "tekstsnutt"
 
 #~ msgid "snippets"
-#~ msgstr "extraits"
+#~ msgstr "tekstsnutter"
 
 #~ msgid "template name"
-#~ msgstr "nom du modèle"
+#~ msgstr "malnavn"
 
 #~ msgid "ancestor"
-#~ msgstr "ancêtre"
+#~ msgstr "opphav"
 
 #~ msgid "app instance namespace"
-#~ msgstr "espace de noms d’instance d’application"
+#~ msgstr "programinstans-navnerom"
 
 #~ msgid "move to"
 #~ msgstr "verschieben nach"
 
 #~ msgid "left sibling"
 #~ msgstr "linkes Geschwister"
```

### Comparing `feincms3-4.0a1/feincms3/locale/it/LC_MESSAGES/django.po` & `feincms3-4.1.0/feincms3/locale/it/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -5,297 +5,303 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-03-16 10:34+0100\n"
+"POT-Creation-Date: 2023-02-02 17:10+0100\n"
 "PO-Revision-Date: 2020-12-04 09:43+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/feincms3/"
 "feincms3/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:97 pages.py:60
+#: admin.py:98 pages.py:69
 msgid "title"
 msgstr "titolo"
 
-#: admin.py:111
+#: admin.py:112
 msgid "move"
 msgstr "sposta"
 
-#: admin.py:137
+#: admin.py:138
 #, python-format
 msgid "Move %s"
 msgstr "Sposta %s"
 
-#: admin.py:142
+#: admin.py:143
 #, python-format
 msgid "Clone %s"
 msgstr "Clona %s"
 
-#: admin.py:211
+#: admin.py:212
 msgid "New location"
 msgstr "Nuova posizione"
 
-#: admin.py:219
+#: admin.py:220
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
 "Lo spostamento non è possibile perché non ci sono bersagli validi. Forse hai "
 "selezionato l'unico nodo radice?"
 
-#: admin.py:265 admin.py:276 admin.py:286
+#: admin.py:266 admin.py:277 admin.py:287
 msgid "move here"
 msgstr "sposta qui"
 
-#: admin.py:344
+#: admin.py:345
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr ""
 
-#: admin.py:362
+#: admin.py:363
 msgid "target"
 msgstr ""
 
-#: admin.py:372
+#: admin.py:373
 msgid "Replace target's content"
 msgstr ""
 
-#: admin.py:374
+#: admin.py:375
 #, python-format
 msgid "Affects the following models: %s."
 msgstr ""
 
-#: admin.py:396
+#: admin.py:397
 #, python-format
 msgid "Current: \"%s\""
 msgstr "Attuale: «%s»"
 
-#: admin.py:406
+#: admin.py:407
 msgid "Cannot clone node to itself."
 msgstr ""
 
-#: admin.py:429
+#: admin.py:430
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr ""
 
-#: admin.py:453
+#: admin.py:454
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr ""
 
-#: admin.py:482
+#: admin.py:481
 msgid "subtree"
 msgstr ""
 
-#: applications.py:389
+#: applications.py:492
 #, fuzzy
 #| msgid "page"
 msgid "page type"
 msgstr "pagina"
 
-#: applications.py:436
+#: applications.py:536
 #, fuzzy, python-format
 #| msgid "This field is required for the application %s."
 msgid "This field is required for the page type \"%s\"."
 msgstr "Questo campo è obbligatorio per l’applicazione %s."
 
-#: applications.py:460
-msgid "This exact app already exists."
-msgstr "Questa applicazione esatta esiste già."
+#: applications.py:558
+#, python-brace-format
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
 
-#: mixins.py:18
+#: mixins.py:20
 msgid "menu"
 msgstr "menù"
 
-#: mixins.py:51 plugins/snippet.py:32
+#: mixins.py:72 plugins/snippet.py:33
 msgid "template"
 msgstr "modello"
 
-#: mixins.py:97
+#: mixins.py:123
 msgid "language"
 msgstr "lingua"
 
-#: mixins.py:127
+#: mixins.py:153
 msgid "translation of"
 msgstr "traduzione di"
 
-#: mixins.py:168
+#: mixins.py:214
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Gli oggetti nella lingua principale non possono essere la traduzione di un "
 "altro oggetto."
 
-#: mixins.py:181
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr ""
-"Gli oggetti possono essere solo la traduzione di oggetti nella lingua "
-"principale."
-
-#: mixins.py:194
+#: mixins.py:228
 msgid "Redirect to URL"
 msgstr "Reindirizza all’URL"
 
-#: mixins.py:201
+#: mixins.py:236
 msgid "Redirect to page"
 msgstr "Reindirizza alla pagina"
 
-#: mixins.py:224
+#: mixins.py:259
 msgid "Only set one redirect value."
 msgstr ""
 
-#: mixins.py:232
+#: mixins.py:267
 msgid "Cannot redirect to self."
 msgstr ""
 
-#: mixins.py:243
+#: mixins.py:278
 #, python-format
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
 
-#: mixins.py:260
+#: mixins.py:295
 #, python-format
 msgid ""
 "Do not chain redirects. The following pages already redirect to this page: "
 "%(pages)s"
 msgstr ""
 
-#: pages.py:59
+#: pages.py:68
 msgid "is active"
 msgstr "è attivo"
 
-#: pages.py:61
+#: pages.py:70
 msgid "slug"
 msgstr ""
 
-#: pages.py:68
+#: pages.py:77
 msgid "Position is expected to be greater than zero."
 msgstr ""
 
-#: pages.py:75
+#: pages.py:84
 msgid "path"
 msgstr ""
 
-#: pages.py:80
+#: pages.py:89
 msgid ""
 "Automatically generated by concatenating the parent's path and the slug "
 "unless the path is defined manually."
 msgstr ""
 
-#: pages.py:86
+#: pages.py:95
 msgid "Path must start and end with a slash (/)."
 msgstr ""
 
-#: pages.py:90
+#: pages.py:99
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:97
+#: pages.py:106
 msgid "page"
 msgstr "pagina"
 
-#: pages.py:98
+#: pages.py:107
 msgid "pages"
 msgstr "pagine"
 
-#: pages.py:140
+#: pages.py:149
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr ""
 
-#: pages.py:160
+#: pages.py:171
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr ""
 
-#: plugins/external.py:108
+#: plugins/external.py:113
 msgid "URL"
 msgstr "URL"
 
-#: plugins/external.py:110 plugins/image.py:40
+#: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
 msgstr ""
 
-#: plugins/external.py:111 plugins/image.py:41
+#: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
 msgstr ""
 
-#: plugins/external.py:115 plugins/image.py:45
+#: plugins/external.py:120 plugins/image.py:47
 #, fuzzy
 #| msgid "application"
 msgid "caption"
 msgstr "applicazione"
 
-#: plugins/external.py:119
+#: plugins/external.py:124
 msgid "external content"
 msgstr ""
 
-#: plugins/external.py:135
+#: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr ""
 
 #: plugins/html.py:26
 msgid ""
 "The content will be inserted directly into the page. It is VERY important "
 "that the HTML snippet is well-formed!"
 msgstr ""
 "Il contenuto verrà inserito direttamente nella pagina. È MOLTO importante "
 "che il frammento HTML sia ben formato!"
 
-#: plugins/image.py:24 plugins/image.py:49
+#: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr "imagine"
 
-#: plugins/image.py:33
+#: plugins/image.py:35
 msgid "image width"
 msgstr "larghezza immagine"
 
-#: plugins/image.py:36
+#: plugins/image.py:38
 msgid "image height"
 msgstr "altezza immagine"
 
-#: plugins/image.py:38
+#: plugins/image.py:40
 msgid "primary point of interest"
 msgstr ""
 
-#: plugins/image.py:50
+#: plugins/image.py:52
 msgid "images"
 msgstr "imagini"
 
-#: plugins/richtext.py:30
+#: plugins/old_richtext.py:40 plugins/richtext.py:20
 msgid "text"
 msgstr "testo"
 
-#: plugins/richtext.py:34
+#: plugins/old_richtext.py:44 plugins/richtext.py:24
 msgid "rich text"
 msgstr ""
 
-#: plugins/richtext.py:35
+#: plugins/old_richtext.py:45 plugins/richtext.py:25
 msgid "rich texts"
 msgstr ""
 
-#: plugins/snippet.py:39
+#: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
-#: plugins/snippet.py:40
+#: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
+#~ msgid "This exact app already exists."
+#~ msgstr "Questa applicazione esatta esiste già."
+
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Gli oggetti possono essere solo la traduzione di oggetti nella lingua "
+#~ "principale."
+
 #~ msgid "snippet"
 #~ msgstr "frammento"
 
 #~ msgid "snippets"
 #~ msgstr "frammenti"
 
 #~ msgid "template name"
```

### Comparing `feincms3-4.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo` & `feincms3-4.1.0/feincms3/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -56,17 +56,14 @@
 msgstr "Ny plassering"
 
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Objekter i primærspråket kan ikke være oversettelsen av et annet objekt."
 
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr "Objekter kan kun være oversettelser av objekter i primærspråk."
-
 msgid "Only set one redirect value."
 msgstr "Kun sett én videresendingsverdi."
 
 msgid "Path must start and end with a slash (/)."
 msgstr "Sti må starte og slutt med skråstrek (/)."
 
 msgid "Position is expected to be greater than zero."
@@ -89,17 +86,14 @@
 
 msgid "The node %(node)s has been moved to the new position."
 msgstr "Noden %(node)s har blitt flyttet til ny plassering"
 
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr "Siden «%(page)s» sin nye sti %(path)s finnes allerede."
 
-msgid "This exact app already exists."
-msgstr "Akkurat dette programmet finnes allerede."
-
 msgid "URL"
 msgstr "Nettadresse"
 
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr "Klarte ikke å hente HTML for denne nettadressen."
 
 msgid "Updated fields of %(node)s: %(fields)s"
```

### Comparing `feincms3-4.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po` & `feincms3-4.1.0/feincms3/locale/fr/LC_MESSAGES/django.po`

 * *Files 18% similar despite different names*

```diff
@@ -5,318 +5,323 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-03-16 10:34+0100\n"
-"PO-Revision-Date: 2020-12-04 09:46+0000\n"
-"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
-"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
-"feincms3/feincms3/nb_NO/>\n"
-"Language: nb_NO\n"
+"POT-Creation-Date: 2023-02-02 17:10+0100\n"
+"PO-Revision-Date: 2020-12-04 09:43+0000\n"
+"Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
+"Language-Team: French <https://hosted.weblate.org/projects/feincms3/feincms3/"
+"fr/>\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:97 pages.py:60
+#: admin.py:98 pages.py:69
 msgid "title"
-msgstr "tittel"
+msgstr "titre"
 
-#: admin.py:111
+#: admin.py:112
 msgid "move"
-msgstr "flytt"
+msgstr "déplacer"
 
-#: admin.py:137
+#: admin.py:138
 #, python-format
 msgid "Move %s"
-msgstr "Flytt %s"
+msgstr "Déplacer %s"
 
-#: admin.py:142
+#: admin.py:143
 #, python-format
 msgid "Clone %s"
-msgstr "Klon %s"
+msgstr "Cloner %s"
 
-#: admin.py:211
+#: admin.py:212
 msgid "New location"
-msgstr "Ny plassering"
+msgstr "Nouvel emplacement"
 
-#: admin.py:219
+#: admin.py:220
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
-"Flytting er ikke mulig fordi det ikke er noen gyldige mål. Kanskje du valgte "
-"den eneste rotnoden?"
+"Le déplacement n’est pas possible car il n’y a pas de cibles valides. Peut-"
+"être avez-vous sélectionné le seul nœud racine ?"
 
-#: admin.py:265 admin.py:276 admin.py:286
+#: admin.py:266 admin.py:277 admin.py:287
 msgid "move here"
-msgstr "flytt hit"
+msgstr "déplacer ici"
 
-#: admin.py:344
+#: admin.py:345
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
-msgstr "Noden %(node)s har blitt flyttet til ny plassering"
+msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
 
-#: admin.py:362
+#: admin.py:363
 msgid "target"
-msgstr "mål"
+msgstr "cible"
 
-#: admin.py:372
+#: admin.py:373
 msgid "Replace target's content"
-msgstr "Erstatt målets innhold"
+msgstr "Remplacer le contenu de la cible"
 
-#: admin.py:374
+#: admin.py:375
 #, python-format
 msgid "Affects the following models: %s."
-msgstr "Har innvirkning på følgende moduler: %s."
+msgstr "Affecte les modèles suivants : %s."
 
-#: admin.py:396
+#: admin.py:397
 #, python-format
 msgid "Current: \"%s\""
-msgstr "Nåværende: «%s»"
+msgstr "Actuel : « %s »"
 
-#: admin.py:406
+#: admin.py:407
 msgid "Cannot clone node to itself."
-msgstr "Kan ikke klone node til seg selv."
+msgstr "Impossible de cloner le nœud sur lui-même."
 
-#: admin.py:429
+#: admin.py:430
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
-msgstr "Oppdaterte felter tilhørende %(node)s: %(fields)s"
+msgstr "Champs mis à jour de %(node)s : %(fields)s"
 
-#: admin.py:453
+#: admin.py:454
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
-msgstr "Erstattet innholdet i %(target)s med innholdet i %(source)s."
+msgstr "Remplacement du contenu de %(target)s par le contenu de %(source)s."
 
-#: admin.py:482
+#: admin.py:481
 msgid "subtree"
 msgstr ""
 
-#: applications.py:389
-#, fuzzy
-#| msgid "page"
+#: applications.py:492
 msgid "page type"
-msgstr "side"
+msgstr "type de page"
 
-#: applications.py:436
-#, fuzzy, python-format
-#| msgid "This field is required for the application %s."
+#: applications.py:536
+#, python-format
 msgid "This field is required for the page type \"%s\"."
-msgstr "Dette feltet kreves for programmet %s."
+msgstr "Ce champ est obligatoire pour le type de page \"%s\"."
 
-#: applications.py:460
-msgid "This exact app already exists."
-msgstr "Akkurat dette programmet finnes allerede."
+#: applications.py:558
+#, python-brace-format
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
 
-#: mixins.py:18
+#: mixins.py:20
 msgid "menu"
-msgstr "meny"
+msgstr "menu"
 
-#: mixins.py:51 plugins/snippet.py:32
+#: mixins.py:72 plugins/snippet.py:33
 msgid "template"
-msgstr "mal"
+msgstr "modèle"
 
-#: mixins.py:97
+#: mixins.py:123
 msgid "language"
-msgstr "språk"
+msgstr "langue"
 
-#: mixins.py:127
+#: mixins.py:153
 msgid "translation of"
-msgstr "oversettelse av"
+msgstr "traduction de"
 
-#: mixins.py:168
+#: mixins.py:214
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
-"Objekter i primærspråket kan ikke være oversettelsen av et annet objekt."
-
-#: mixins.py:181
-msgid "Objects may only be the translation of objects in the primary language."
-msgstr "Objekter kan kun være oversettelser av objekter i primærspråk."
+"Les objets dans la langue principale ne peuvent pas être la traduction d’un "
+"autre objet."
 
-#: mixins.py:194
+#: mixins.py:228
 msgid "Redirect to URL"
-msgstr "Videresendt til nettadresse"
+msgstr "Rediriger vers l’URL"
 
-#: mixins.py:201
+#: mixins.py:236
 msgid "Redirect to page"
-msgstr "Videresendt til side"
+msgstr "Rediriger vers la page"
 
-#: mixins.py:224
+#: mixins.py:259
 msgid "Only set one redirect value."
-msgstr "Kun sett én videresendingsverdi."
+msgstr "Définissez une seule valeur de redirection."
 
-#: mixins.py:232
+#: mixins.py:267
 msgid "Cannot redirect to self."
-msgstr "Kan ikke videresende til seg selv."
+msgstr "Impossible de rediriger vers soi."
 
-#: mixins.py:243
+#: mixins.py:278
 #, python-format
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
-"Kan ikke opprette videresendelser i stafett. Valgt side «%(title)s» "
-"videresender til «%(path)s»."
+"Ne pas enchaîner les redirections. La page sélectionnée « %(title)s » "
+"redirige vers « %(path)s »."
 
-#: mixins.py:260
+#: mixins.py:295
 #, python-format
 msgid ""
 "Do not chain redirects. The following pages already redirect to this page: "
 "%(pages)s"
 msgstr ""
-"Ikke opprett videresendelser i stafett. Følgende sider videresender til "
-"denne siden: %(pages)s"
+"Ne pas enchaîner les redirections. Les pages suivantes redirigent déjà vers "
+"cette page : %(pages)s"
 
-#: pages.py:59
+#: pages.py:68
 msgid "is active"
-msgstr "er aktiv"
+msgstr "est actif"
 
-#: pages.py:61
+#: pages.py:70
 msgid "slug"
-msgstr ""
+msgstr "slug"
 
-#: pages.py:68
+#: pages.py:77
 msgid "Position is expected to be greater than zero."
-msgstr "Posisjonen forventes å være større enn null."
+msgstr "La position devrait être supérieure à zéro."
 
-#: pages.py:75
+#: pages.py:84
 msgid "path"
-msgstr "sti"
+msgstr "chemin"
 
-#: pages.py:80
+#: pages.py:89
 msgid ""
 "Automatically generated by concatenating the parent's path and the slug "
 "unless the path is defined manually."
 msgstr ""
 
-#: pages.py:86
+#: pages.py:95
 msgid "Path must start and end with a slash (/)."
-msgstr "Sti må starte og slutt med skråstrek (/)."
+msgstr "Le chemin doit commencer et se terminer par une barre oblique (/)."
 
-#: pages.py:90
+#: pages.py:99
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:97
+#: pages.py:106
 msgid "page"
-msgstr "side"
+msgstr "page"
 
-#: pages.py:98
+#: pages.py:107
 msgid "pages"
-msgstr "sider"
+msgstr "pages"
 
-#: pages.py:140
+#: pages.py:149
 msgid "Static paths cannot be empty. Did you mean '/'?"
-msgstr "Statiske stier må fylles ut. Mente du «/»?"
+msgstr ""
+"Les chemins statiques ne peuvent pas être vides. Vouliez-vous dire « / » ?"
 
-#: pages.py:160
+#: pages.py:171
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
-msgstr "Siden «%(page)s» sin nye sti %(path)s finnes allerede."
+msgstr "Le nouveau chemin %(path)s de la page %(page)s ne serait pas unique."
 
-#: plugins/external.py:108
+#: plugins/external.py:113
 msgid "URL"
-msgstr "Nettadresse"
+msgstr "URL"
 
-#: plugins/external.py:110 plugins/image.py:40
+#: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
-msgstr ""
+msgstr "texte alternatif"
 
-#: plugins/external.py:111 plugins/image.py:41
+#: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
-msgstr ""
+msgstr "Décrit les contenus de l’image, par ex. pour un lecteur d’écran."
 
-#: plugins/external.py:115 plugins/image.py:45
-#, fuzzy
-#| msgid "application"
+#: plugins/external.py:120 plugins/image.py:47
 msgid "caption"
-msgstr "program"
+msgstr "légende"
 
-#: plugins/external.py:119
+#: plugins/external.py:124
 msgid "external content"
-msgstr "eksternt innhold"
+msgstr "contenu externe"
 
-#: plugins/external.py:135
+#: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
-msgstr "Klarte ikke å hente HTML for denne nettadressen."
+msgstr "Impossible de récupérer le HTML pour cette URL, désolé !"
 
 #: plugins/html.py:26
 msgid ""
 "The content will be inserted directly into the page. It is VERY important "
 "that the HTML snippet is well-formed!"
 msgstr ""
+"Le contenu sera inséré directement dans la page. Il est TRÈS important que "
+"l’extrait de code HTML soit bien formé !"
 
-#: plugins/image.py:24 plugins/image.py:49
+#: plugins/image.py:26 plugins/image.py:51
 msgid "image"
-msgstr "bilde"
+msgstr "image"
 
-#: plugins/image.py:33
+#: plugins/image.py:35
 msgid "image width"
-msgstr "bildebredde"
+msgstr "Largeur de l’image"
 
-#: plugins/image.py:36
+#: plugins/image.py:38
 msgid "image height"
-msgstr "bildehøyde"
+msgstr "hauteur de l’image"
 
-#: plugins/image.py:38
+#: plugins/image.py:40
 msgid "primary point of interest"
-msgstr "hoved-interessepunkt"
+msgstr "principal point d’intérêt"
 
-#: plugins/image.py:50
+#: plugins/image.py:52
 msgid "images"
-msgstr "bilder"
+msgstr "images"
 
-#: plugins/richtext.py:30
+#: plugins/old_richtext.py:40 plugins/richtext.py:20
 msgid "text"
-msgstr "tekst"
+msgstr "texte"
 
-#: plugins/richtext.py:34
-#, fuzzy
+#: plugins/old_richtext.py:44 plugins/richtext.py:24
 msgid "rich text"
-msgstr "rikholdig tekst"
+msgstr "texte riche"
 
-#: plugins/richtext.py:35
-#, fuzzy
+#: plugins/old_richtext.py:45 plugins/richtext.py:25
 msgid "rich texts"
-msgstr "rikholdige tekster"
+msgstr "textes riches"
 
-#: plugins/snippet.py:39
+#: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
-#: plugins/snippet.py:40
+#: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
+#~ msgid "This exact app already exists."
+#~ msgstr "Cette application exacte existe déjà."
+
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Les objets peuvent seulement être la traduction d’objets dans la langue "
+#~ "principale."
+
 #~ msgid "Generated automatically if 'static path' is unset."
-#~ msgstr "Generert automatisk hvis «statisk sti» ikke er valgt."
+#~ msgstr "Généré automatiquement si le « chemin statique » n’est pas défini."
 
 #~ msgid "static path"
-#~ msgstr "statisk sti"
+#~ msgstr "chemin statique"
 
 #~ msgid "snippet"
-#~ msgstr "tekstsnutt"
+#~ msgstr "extrait"
 
 #~ msgid "snippets"
-#~ msgstr "tekstsnutter"
+#~ msgstr "extraits"
 
 #~ msgid "template name"
-#~ msgstr "malnavn"
+#~ msgstr "nom du modèle"
 
 #~ msgid "ancestor"
-#~ msgstr "opphav"
+#~ msgstr "ancêtre"
 
 #~ msgid "app instance namespace"
-#~ msgstr "programinstans-navnerom"
+#~ msgstr "espace de noms d’instance d’application"
 
 #~ msgid "move to"
 #~ msgstr "verschieben nach"
 
 #~ msgid "left sibling"
 #~ msgstr "linkes Geschwister"
```

### Comparing `feincms3-4.0a1/feincms3/mixins.py` & `feincms3-4.1.0/feincms3/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         errors.extend(cls._check_feincms3_menu_mixin(**kwargs))
         return errors
 
     @classmethod
     def _check_feincms3_menu_mixin(cls, **kwargs):
         if invalid := [
             value
-            for value, label in cls.MENUS
+            for value, _label in cls.MENUS
             if value and (value.startswith("_") or not value.isidentifier())
         ]:
             yield Warning(
                 "MenuMixin menus should only use valid public Python identifiers"
                 f" as keys. Invalid: {sorted(invalid)!r}.",
                 obj=cls,
                 id="feincms3.W005",
@@ -104,14 +104,15 @@
 
             warnings.warn(
                 f"{sender._meta.label} uses the TemplateMixin."
                 " It is recommended to use the PageTypeMixin and TemplateType"
                 " from feincms3.applications even if you're not planning to use"
                 " any apps.",
                 DeprecationWarning,
+                stacklevel=1,
             )
 
 
 signals.class_prepared.connect(TemplateMixin.fill_template_key_choices)
 
 
 class LanguageMixin(models.Model):
```

### Comparing `feincms3-4.0a1/feincms3/pages.py` & `feincms3-4.1.0/feincms3/pages.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/plugins/external.py` & `feincms3-4.1.0/feincms3/plugins/external.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/plugins/html.py` & `feincms3-4.1.0/feincms3/plugins/html.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/plugins/image.py` & `feincms3-4.1.0/feincms3/plugins/image.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/plugins/old_richtext.py` & `feincms3-4.1.0/feincms3/plugins/old_richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/plugins/richtext.py` & `feincms3-4.1.0/feincms3/plugins/richtext.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from feincms3.inline_ckeditor import InlineCKEditorField
 
 
 __all__ = ("RichText", "RichTextInline", "render_richtext")
 
 
 class RichText(models.Model):
+    """
+    Rich text plugin.
+
+    :class:`feincms3.inline_ckeditor.InlineCKEditorField` does all the heavy
+    lifting.
+    """
+
     text = InlineCKEditorField(_("text"))
 
     class Meta:
         abstract = True
         verbose_name = _("rich text")
         verbose_name_plural = _("rich texts")
```

### Comparing `feincms3-4.0a1/feincms3/plugins/snippet.py` & `feincms3-4.1.0/feincms3/plugins/snippet.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/regions.py` & `feincms3-4.1.0/feincms3/regions.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/renderer.py` & `feincms3-4.1.0/feincms3/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+import inspect
 import warnings
 from collections import deque
 
 from content_editor.contents import contents_for_item
 from django.core.cache import cache
+from django.core.exceptions import ImproperlyConfigured
 from django.template import Context, Engine
 from django.utils.functional import SimpleLazyObject
 from django.utils.html import mark_safe
 
 
 __all__ = (
-    "PluginNotRegistered",
+    "PluginNotRegisteredError",
     "default_context",
     "render_in_context",
     "template_renderer",
     "RegionRenderer",
     "TemplatePluginRenderer",
 )
 
 
-class PluginNotRegistered(Exception):
+class PluginNotRegisteredError(Exception):
     """
     Exception raised when encountering a plugin which isn't known to the
     renderer.
     """
 
-    pass
+
+# Backwards compatibility
+PluginNotRegistered = PluginNotRegisteredError
 
 
 def default_context(plugin, context):
     """
     Return the default context for plugins rendered with a template, which
     simply is a single variable named ``plugin`` containing the plugin
     instance.
@@ -113,48 +117,58 @@
           renderer instance or rendering **will** crash loudly.
         - ``marks: Set[str] = {"default"}``: The marks of this plugin. Marks
           only have the meaning you assign to them. Marks are preferrable to
           running ``isinstance`` on plugin instances especially when using the
           same region renderer class for different content types (e.g. pages
           and blog articles).
         """
+        if plugin in self._renderers:
+            warnings.warn(
+                f"The plugin {plugin} has already been registered with {self.__class__} before.",
+                stacklevel=2,
+            )
         self._renderers[plugin] = renderer
         self._subregions[plugin] = subregion
         self._marks[plugin] = marks
 
+        if callable(renderer) and len(inspect.signature(renderer).parameters) < 2:
+            raise ImproperlyConfigured(
+                f"The renderer function {renderer} has less than the two required arguments."
+            )
+
     def plugins(self):
         """
         Return a list of all registered plugin classes
         """
         return list(self._renderers)
 
     def render_plugin(self, plugin, context):
         """
         Render a single plugin using the registered renderer
         """
         try:
             renderer = self._renderers[plugin.__class__]
-        except KeyError:
-            raise PluginNotRegistered(
+        except KeyError as exc:
+            raise PluginNotRegisteredError(
                 f"Plugin {plugin._meta.label_lower} is not registered"
-            )
+            ) from exc
         if callable(renderer):
             return renderer(plugin, context)
         return renderer
 
     def subregion(self, plugin):
         """
         Return the subregion of a plugin instance
         """
         try:
             subregion = self._subregions[plugin.__class__]
-        except KeyError:
-            raise PluginNotRegistered(
+        except KeyError as exc:
+            raise PluginNotRegisteredError(
                 f"Plugin {plugin._meta.label_lower} is not registered"
-            )
+            ) from exc
         if callable(subregion):
             return subregion(plugin)
         return subregion
 
     def takewhile_subregion(self, plugins, subregion):
         """
         Yield all plugins from the head of the ``plugins`` deque as long as
@@ -165,18 +179,18 @@
 
     def marks(self, plugin):
         """
         Return the marks of a plugin instance
         """
         try:
             marks = self._marks[plugin.__class__]
-        except KeyError:
-            raise PluginNotRegistered(
+        except KeyError as exc:
+            raise PluginNotRegisteredError(
                 f"Plugin {plugin._meta.label_lower} is not registered"
-            )
+            ) from exc
         if callable(marks):
             return marks(plugin)
         return marks
 
     def takewhile_mark(self, plugins, mark):
         """
         Yield all plugins from the head of the ``plugins`` deque as long as
```

### Comparing `feincms3-4.0a1/feincms3/root/middleware.py` & `feincms3-4.1.0/feincms3/root/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,14 @@
     HttpResponseRedirect,
 )
 
 
 class _UseRootMiddlewareResponse(HttpResponseNotFound):
     """Used by feincms3.root.passthru to tell the middleware to do its thing"""
 
-    pass
-
 
 def create_page_if_404_middleware(*, queryset, handler, language_code_redirect=False):
     """
     Create a middleware for handling pages
 
     This utility is there for your convenience, you do not have to use it. The
     returned middleware already handles returning non-404 responses as-is,
```

### Comparing `feincms3-4.0a1/feincms3/root/passthru.py` & `feincms3-4.1.0/feincms3/root/passthru.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     # Fallback
     reverse_passthru("imprint", fallback="/en/imprint/")
 
     # Outside the request-response cycle
     reverse_passthru("imprint", urlconf=apps_urlconf())
 """
 
+from functools import partial
+
 from django.urls import path
+from django.utils.functional import lazy
 
 from feincms3.applications import reverse_app
 from feincms3.root.middleware import _UseRootMiddlewareResponse
 
 
 app_name = "passthru"
 urlpatterns = [path("", lambda request: _UseRootMiddlewareResponse(), name="passthru")]
@@ -49,7 +52,11 @@
 def reverse_passthru(namespace, **kwargs):
     """
     Reverse a passthru app URL
 
     Raises ``NoReverseMatch`` if page could not be found.
     """
     return reverse_app(namespace, "passthru", **kwargs)
+
+
+def reverse_passthru_lazy(namespace, **kwargs):
+    return lazy(partial(reverse_passthru, namespace, **kwargs), str)()
```

### Comparing `feincms3-4.0a1/feincms3/shortcuts.py` & `feincms3-4.1.0/feincms3/shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def render_list(
     request,
     queryset,
     context=None,
     *,
     model=None,
     paginate_by=None,
-    template_name_suffix="_list"
+    template_name_suffix="_list",
 ):
     """
     Render a list of items
 
     Usage example::
 
         def article_list(request, ...):
```

### Comparing `feincms3-4.0a1/feincms3/static/feincms3/box-drawing.css` & `feincms3-4.1.0/feincms3/static/feincms3/box-drawing.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/static/feincms3/inline-ckeditor.css` & `feincms3-4.1.0/feincms3/static/feincms3/inline-ckeditor.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 .change-form .cke_textarea_inline {
-  margin-left: 170px;
   max-width: 80ch;
   border: 1px solid var(--border-color);
   border-radius: 4px;
   padding: 5px 6px;
 }
 
+.change-form [data-inline-cke-dj41] + .cke_textarea_inline {
+  margin-left: 170px;
+}
+
 @media (max-width: 767px) {
   .change-form .cke_textarea_inline {
     margin: 0;
     width: calc(100%);
     max-width: none;
     padding: 6px 8px;
   }
 }
 
-.cke_textarea_inline *:not(hr) {
+.inline-group[data-inline-type="tabular"] .cke_textarea_inline {
+  margin: 0;
+}
+
+.cke_textarea_inline *:not(hr, table, tr, th, td) {
   background: none !important;
   color: inherit !important;
   border: none !important;
   padding: 0 !important;
   margin: 0 !important;
 }
```

### Comparing `feincms3-4.0a1/feincms3/static/feincms3/inline-ckeditor.js` & `feincms3-4.1.0/feincms3/static/feincms3/inline-ckeditor.js`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/static/feincms3/move-form.css` & `feincms3-4.1.0/feincms3/static/feincms3/move-form.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/static/feincms3/static-path-style.js` & `feincms3-4.1.0/feincms3/static/feincms3/static-path-style.js`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/templatetags/feincms3.py` & `feincms3-4.1.0/feincms3/templatetags/feincms3.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.0a1/feincms3/utils.py` & `feincms3-4.1.0/feincms3/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,16 +72,24 @@
 def upload_to(instance, filename):
     """
     Standard ``upload_to`` callable for feincms3 file fields
 
     The generated path consists of:
 
     - The instance's lowercased model label
-    - The year and the day of the year
+    - A part of the proleptic Gregorian ordinal of the date
     - The original filename
+
+    The ordinal changes each day which means that filename collisions only
+    happen when uploading to the same model (or one with the same name in a
+    different app) and on the same day. This is much better than the previous
+    default of using ``images/%Y/%m`` where you had to wait up to a full month
+    to avoid collisions.
     """
 
+    ordinal = str(dt.date.today().toordinal())
     return posixpath.join(
-        instance._meta.label_lower,
-        dt.date.today().strftime("%y/%j"),
+        instance._meta.model_name,
+        ordinal[1:3],  # cut the first digit, it will only reach 800000 in 2191.
+        ordinal[3:],
         filename,
     )
```

### Comparing `feincms3-4.0a1/setup.cfg` & `feincms3-4.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,72 @@
-[metadata]
-name = feincms3
-version = attr: feincms3.__version__
-description = CMS-building toolkit for Django
-long_description = file: README.rst
-long_description_content_type = text/x-rst
-url = https://github.com/matthiask/feincms3/
-author = Matthias Kestenholz
-author_email = mk@feinheit.ch
-license = BSD-3-Clause
-license_file = LICENSE
-platforms = OS Independent
-classifiers = 
-	Environment :: Web Environment
-	Framework :: Django
-	Intended Audience :: Developers
-	License :: OSI Approved :: BSD License
-	Operating System :: OS Independent
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Topic :: Internet :: WWW/HTTP :: Dynamic Content
-	Topic :: Software Development
-	Topic :: Software Development :: Libraries :: Application Frameworks
-
-[options]
-packages = find:
-install_requires = 
-	Django>=3.2
-	django-content-editor>=6.0
-	django-js-asset>=2.0
-	django-tree-queries>=0.6.0
-python_requires = >=3.8
-include_package_data = True
-zip_safe = False
-
-[options.extras_require]
-all = 
-	django-imagefield
-	html-sanitizer>=1.1.1
-	requests
-tests = 
-	coverage
-	django-ckeditor
-	requests-mock
-
-[options.packages.find]
-exclude = 
-	tests
-	tests.*
-
-[coverage:run]
-branch = True
-include = 
-	*feincms3*
-	*testapp*
-omit = 
-	*migrations*
-	*.tox*
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "feincms3"
+dynamic = ["version"]
+description = "CMS-building toolkit for Django"
+readme = "README.rst"
+license = "BSD-3-Clause"
+requires-python = ">=3.8"
+authors = [
+    { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
+]
+classifiers = [
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+]
+dependencies = [
+    "django-content-editor>=6.0",
+    "django-js-asset>=2.0",
+    "django-tree-queries>=0.15.0",
+    "Django>=3.2",
+]
+
+[project.optional-dependencies]
+all = [
+    "django-imagefield",
+    "html-sanitizer>=1.1.1",
+    "requests",
+]
+tests = [
+    "coverage",
+    "django-ckeditor",
+    "requests-mock",
+]
+
+[project.urls]
+Homepage = "https://github.com/matthiask/feincms3/"
+
+[tool.hatch.build]
+include = ["feincms3/"]
+
+[tool.hatch.version]
+path = "feincms3/__init__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/feincms3",
+]
+
+[tool.ruff]
+extend-select = ["B", "E", "F", "W", "C90", "I", "N", "UP", "FBT", "C4", "DJ", "PIE"]
+extend-ignore = ["E501"]
+fix = true
+target-version = "py38"
+
+[tool.ruff.isort]
+combine-as-imports = true
+lines-after-imports = 2
```

