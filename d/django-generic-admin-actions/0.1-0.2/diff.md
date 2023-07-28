# Comparing `tmp/django-generic-admin-actions-0.1.tar.gz` & `tmp/django-generic-admin-actions-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-generic-admin-actions-0.1.tar", last modified: Thu Jul 27 20:00:58 2023, max compression
+gzip compressed data, was "django-generic-admin-actions-0.2.tar", last modified: Fri Jul 28 20:28:11 2023, max compression
```

## Comparing `django-generic-admin-actions-0.1.tar` & `django-generic-admin-actions-0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-07-27 09:35:02.000000 django-generic-admin-actions-0.1/LICENCE
--rw-r--r--   0 thomas    (1000) thomas    (1000)      136 2023-07-27 11:11:22.000000 django-generic-admin-actions-0.1/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2091 2023-07-27 19:56:06.000000 django-generic-admin-actions-0.1/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.500338 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-27 20:00:58.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1086 2023-07-27 20:00:58.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-27 20:00:58.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2023-07-27 20:00:58.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       33 2023-07-27 20:00:58.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-27 19:30:57.000000 django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/zip-safe
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.500338 django-generic-admin-actions-0.1/generic_admin_actions/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.1/generic_admin_actions/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      660 2023-07-27 19:58:35.000000 django-generic-admin-actions-0.1/generic_admin_actions/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1618 2023-07-27 19:14:13.000000 django-generic-admin-actions-0.1/generic_admin_actions/admin.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      172 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.1/generic_admin_actions/apps.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      200 2023-07-27 13:31:59.000000 django-generic-admin-actions-0.1/generic_admin_actions/forms.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.500338 django-generic-admin-actions-0.1/generic_admin_actions/migrations/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.1/generic_admin_actions/migrations/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.496337 django-generic-admin-actions-0.1/generic_admin_actions/templates/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.500338 django-generic-admin-actions-0.1/generic_admin_actions/templates/admin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      454 2023-07-27 13:33:18.000000 django-generic-admin-actions-0.1/generic_admin_actions/templates/admin/change-list.html
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2192 2023-07-27 19:41:58.000000 django-generic-admin-actions-0.1/setup.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.496337 django-generic-admin-actions-0.1/tests/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.500338 django-generic-admin-actions-0.1/tests/testapp/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      215 2023-07-27 13:35:43.000000 django-generic-admin-actions-0.1/tests/testapp/actions.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      388 2023-07-27 13:40:59.000000 django-generic-admin-actions-0.1/tests/testapp/admin.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/apps.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/tests/testapp/management/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/management/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/tests/testapp/management/commands/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/management/commands/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1290 2023-07-27 19:52:51.000000 django-generic-admin-actions-0.1/tests/testapp/management/commands/testapp.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/tests/testapp/migrations/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      509 2023-07-27 12:32:31.000000 django-generic-admin-actions-0.1/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 12:32:29.000000 django-generic-admin-actions-0.1/tests/testapp/migrations/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      204 2023-07-27 13:41:08.000000 django-generic-admin-actions-0.1/tests/testapp/models.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3167 2023-07-27 12:43:08.000000 django-generic-admin-actions-0.1/tests/testapp/settings.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-27 20:00:58.504340 django-generic-admin-actions-0.1/tests/testapp/tests/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/tests/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1083 2023-07-27 14:04:55.000000 django-generic-admin-actions-0.1/tests/testapp/tests/test_generic_admin_actions.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      758 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/urls.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.1/tests/testapp/wsgi.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-07-27 09:35:02.000000 django-generic-admin-actions-0.2/LICENCE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      136 2023-07-27 11:11:22.000000 django-generic-admin-actions-0.2/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2091 2023-07-27 19:56:06.000000 django-generic-admin-actions-0.2/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3401 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1086 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       39 2023-07-28 20:28:11.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-27 19:30:57.000000 django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/zip-safe
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      660 2023-07-28 20:26:55.000000 django-generic-admin-actions-0.2/generic_admin_actions/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1603 2023-07-28 15:49:22.000000 django-generic-admin-actions-0.2/generic_admin_actions/admin.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      172 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/apps.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      200 2023-07-27 13:31:59.000000 django-generic-admin-actions-0.2/generic_admin_actions/forms.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/migrations/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:32:53.000000 django-generic-admin-actions-0.2/generic_admin_actions/migrations/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.484400 django-generic-admin-actions-0.2/generic_admin_actions/templates/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/generic_admin_actions/templates/admin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      454 2023-07-27 13:33:18.000000 django-generic-admin-actions-0.2/generic_admin_actions/templates/admin/change-list.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2192 2023-07-27 19:41:58.000000 django-generic-admin-actions-0.2/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.484400 django-generic-admin-actions-0.2/tests/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      215 2023-07-27 13:35:43.000000 django-generic-admin-actions-0.2/tests/testapp/actions.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      388 2023-07-27 13:40:59.000000 django-generic-admin-actions-0.2/tests/testapp/admin.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      114 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/apps.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/management/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/management/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/management/commands/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/management/commands/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1290 2023-07-27 19:52:51.000000 django-generic-admin-actions-0.2/tests/testapp/management/commands/testapp.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/migrations/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      509 2023-07-27 12:32:31.000000 django-generic-admin-actions-0.2/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 12:32:29.000000 django-generic-admin-actions-0.2/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      204 2023-07-27 13:41:08.000000 django-generic-admin-actions-0.2/tests/testapp/models.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3167 2023-07-27 12:43:08.000000 django-generic-admin-actions-0.2/tests/testapp/settings.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 20:28:11.488400 django-generic-admin-actions-0.2/tests/testapp/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/tests/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1083 2023-07-27 14:04:55.000000 django-generic-admin-actions-0.2/tests/testapp/tests/test_generic_admin_actions.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      758 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/urls.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      391 2023-07-27 09:35:33.000000 django-generic-admin-actions-0.2/tests/testapp/wsgi.py
```

### Comparing `django-generic-admin-actions-0.1/LICENCE` & `django-generic-admin-actions-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/PKG-INFO` & `django-generic-admin-actions-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-admin-actions
-Version: 0.1
+Version: 0.2
 Summary: TODO
 Home-page: https://github.com/thomst/django-generic-admin-actions
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-generic-admin-actions-0.1/README.rst` & `django-generic-admin-actions-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/PKG-INFO` & `django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-admin-actions
-Version: 0.1
+Version: 0.2
 Summary: TODO
 Home-page: https://github.com/thomst/django-generic-admin-actions
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-generic-admin-actions-0.1/django_generic_admin_actions.egg-info/SOURCES.txt` & `django-generic-admin-actions-0.2/django_generic_admin_actions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/generic_admin_actions/__version__.py` & `django-generic-admin-actions-0.2/generic_admin_actions/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "0.1"
+__version__ = "0.2"
```

### Comparing `django-generic-admin-actions-0.1/generic_admin_actions/admin.py` & `django-generic-admin-actions-0.2/generic_admin_actions/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,10 @@
         actions = dict()
         for action in self.generic_actions:
             name = getattr(action, '__name__', repr(action))
             actions[name] = action
         return actions
 
     def run_generic_action(self, request):
-        action = request.POST.get('generic_action', None)
+        action = request.POST['generic_action']
         actions = self.get_generic_actions()
-        actions[action](self, request)
-        return HttpResponseRedirect('../')
+        return actions[action](self, request) or HttpResponseRedirect('../')
```

### Comparing `django-generic-admin-actions-0.1/setup.py` & `django-generic-admin-actions-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/tests/testapp/management/commands/testapp.py` & `django-generic-admin-actions-0.2/tests/testapp/management/commands/testapp.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/tests/testapp/settings.py` & `django-generic-admin-actions-0.2/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/tests/testapp/tests/test_generic_admin_actions.py` & `django-generic-admin-actions-0.2/tests/testapp/tests/test_generic_admin_actions.py`

 * *Files identical despite different names*

### Comparing `django-generic-admin-actions-0.1/tests/testapp/urls.py` & `django-generic-admin-actions-0.2/tests/testapp/urls.py`

 * *Files identical despite different names*

