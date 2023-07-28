# Comparing `tmp/django-safedelete-e2e-0.3.6.tar.gz` & `tmp/django-safedelete-e2e-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-safedelete-e2e-0.3.6.tar", last modified: Fri Jul 28 05:53:46 2023, max compression
+gzip compressed data, was "django-safedelete-e2e-0.3.7.tar", last modified: Fri Jul 28 06:14:37 2023, max compression
```

## Comparing `django-safedelete-e2e-0.3.6.tar` & `django-safedelete-e2e-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 05:53:46.450332 django-safedelete-e2e-0.3.6/
--rw-rw-r--   0 roniee007   (501) staff       (20)       59 2023-07-27 12:35:10.000000 django-safedelete-e2e-0.3.6/AUTHORS
--rw-rw-r--   0 roniee007   (501) staff       (20)     1430 2023-07-27 12:35:13.000000 django-safedelete-e2e-0.3.6/CHANGES
--rw-rw-r--   0 roniee007   (501) staff       (20)     1479 2023-07-27 12:36:03.000000 django-safedelete-e2e-0.3.6/LICENSE
--rw-rw-r--   0 roniee007   (501) staff       (20)       92 2023-07-27 12:36:05.000000 django-safedelete-e2e-0.3.6/MANIFEST.in
--rw-r--r--   0 roniee007   (501) staff       (20)     5559 2023-07-28 05:53:46.450414 django-safedelete-e2e-0.3.6/PKG-INFO
--rw-rw-r--   0 roniee007   (501) staff       (20)     2923 2023-07-27 12:36:17.000000 django-safedelete-e2e-0.3.6/README.rst
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 05:53:46.448343 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/
--rw-r--r--   0 roniee007   (501) staff       (20)     5559 2023-07-28 05:53:46.000000 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/PKG-INFO
--rw-r--r--   0 roniee007   (501) staff       (20)      531 2023-07-28 05:53:46.000000 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/SOURCES.txt
--rw-r--r--   0 roniee007   (501) staff       (20)        1 2023-07-28 05:53:46.000000 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/dependency_links.txt
--rw-r--r--   0 roniee007   (501) staff       (20)        7 2023-07-28 05:53:46.000000 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/requires.txt
--rw-r--r--   0 roniee007   (501) staff       (20)       11 2023-07-28 05:53:46.000000 django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/top_level.txt
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 05:53:46.449952 django-safedelete-e2e-0.3.6/safedelete/
--rw-rw-r--   0 roniee007   (501) staff       (20)      630 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/__init__.py
--rw-rw-r--   0 roniee007   (501) staff       (20)     5117 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/admin.py
--rw-rw-r--   0 roniee007   (501) staff       (20)     3240 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/managers.py
--rw-rw-r--   0 roniee007   (501) staff       (20)     6871 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/models.py
--rw-rw-r--   0 roniee007   (501) staff       (20)      840 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/settings.py
--rw-rw-r--   0 roniee007   (501) staff       (20)      226 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/shortcuts.py
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 05:53:46.446415 django-safedelete-e2e-0.3.6/safedelete/templates/
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 05:53:46.450147 django-safedelete-e2e-0.3.6/safedelete/templates/safedelete/
--rw-rw-r--   0 roniee007   (501) staff       (20)      658 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/templates/safedelete/undelete_selected_confirmation.html
--rw-rw-r--   0 roniee007   (501) staff       (20)    16838 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/tests.py
--rw-rw-r--   0 roniee007   (501) staff       (20)     1070 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.6/safedelete/utils.py
--rw-rw-r--   0 roniee007   (501) staff       (20)       80 2023-07-28 05:53:46.450623 django-safedelete-e2e-0.3.6/setup.cfg
--rw-rw-r--   0 roniee007   (501) staff       (20)     2157 2023-07-28 05:53:30.000000 django-safedelete-e2e-0.3.6/setup.py
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 06:14:37.250698 django-safedelete-e2e-0.3.7/
+-rw-rw-r--   0 roniee007   (501) staff       (20)       59 2023-07-27 12:35:10.000000 django-safedelete-e2e-0.3.7/AUTHORS
+-rw-rw-r--   0 roniee007   (501) staff       (20)     1430 2023-07-27 12:35:13.000000 django-safedelete-e2e-0.3.7/CHANGES
+-rw-rw-r--   0 roniee007   (501) staff       (20)     1479 2023-07-27 12:36:03.000000 django-safedelete-e2e-0.3.7/LICENSE
+-rw-rw-r--   0 roniee007   (501) staff       (20)       92 2023-07-27 12:36:05.000000 django-safedelete-e2e-0.3.7/MANIFEST.in
+-rw-r--r--   0 roniee007   (501) staff       (20)     5481 2023-07-28 06:14:37.250774 django-safedelete-e2e-0.3.7/PKG-INFO
+-rw-rw-r--   0 roniee007   (501) staff       (20)     2923 2023-07-27 12:36:17.000000 django-safedelete-e2e-0.3.7/README.rst
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 06:14:37.249237 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/
+-rw-r--r--   0 roniee007   (501) staff       (20)     5481 2023-07-28 06:14:37.000000 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/PKG-INFO
+-rw-r--r--   0 roniee007   (501) staff       (20)      531 2023-07-28 06:14:37.000000 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/SOURCES.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)        1 2023-07-28 06:14:37.000000 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/dependency_links.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)        7 2023-07-28 06:14:37.000000 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/requires.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)       11 2023-07-28 06:14:37.000000 django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/top_level.txt
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 06:14:37.250272 django-safedelete-e2e-0.3.7/safedelete/
+-rw-rw-r--   0 roniee007   (501) staff       (20)      630 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/__init__.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)     5115 2023-07-28 06:07:52.000000 django-safedelete-e2e-0.3.7/safedelete/admin.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)     3240 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/managers.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)     6871 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/models.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)      840 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/settings.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)      226 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/shortcuts.py
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 06:14:37.247459 django-safedelete-e2e-0.3.7/safedelete/templates/
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 06:14:37.250407 django-safedelete-e2e-0.3.7/safedelete/templates/safedelete/
+-rw-rw-r--   0 roniee007   (501) staff       (20)      658 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/templates/safedelete/undelete_selected_confirmation.html
+-rw-rw-r--   0 roniee007   (501) staff       (20)    16838 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/tests.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)     1070 2023-07-27 12:36:29.000000 django-safedelete-e2e-0.3.7/safedelete/utils.py
+-rw-rw-r--   0 roniee007   (501) staff       (20)       80 2023-07-28 06:14:37.250974 django-safedelete-e2e-0.3.7/setup.cfg
+-rw-rw-r--   0 roniee007   (501) staff       (20)     1557 2023-07-28 06:14:24.000000 django-safedelete-e2e-0.3.7/setup.py
```

### Comparing `django-safedelete-e2e-0.3.6/CHANGES` & `django-safedelete-e2e-0.3.7/CHANGES`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/LICENSE` & `django-safedelete-e2e-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/PKG-INFO` & `django-safedelete-e2e-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: django-safedelete-e2e
-Version: 0.3.6
+Version: 0.3.7
 Summary: Mask your objects instead of deleting them from your database.
 Home-page: https://github.com/Roniee007/django-safedelete-e2e
-Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/0.3.6
 Author: rounak kabra
 Author-email: rounak.kabra@e2enetworks.com
 License: BSD
 Keywords: django,delete,safedelete,softdelete
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django-safedelete-e2e-0.3.6/README.rst` & `django-safedelete-e2e-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/PKG-INFO` & `django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: django-safedelete-e2e
-Version: 0.3.6
+Version: 0.3.7
 Summary: Mask your objects instead of deleting them from your database.
 Home-page: https://github.com/Roniee007/django-safedelete-e2e
-Download-URL: https://github.com/makinacorpus/django-safedelete/tarball/0.3.6
 Author: rounak kabra
 Author-email: rounak.kabra@e2enetworks.com
 License: BSD
 Keywords: django,delete,safedelete,softdelete
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django-safedelete-e2e-0.3.6/django_safedelete_e2e.egg-info/SOURCES.txt` & `django-safedelete-e2e-0.3.7/django_safedelete_e2e.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/__init__.py` & `django-safedelete-e2e-0.3.7/safedelete/__init__.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/admin.py` & `django-safedelete-e2e-0.3.7/safedelete/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     # Django < 1.7
     from django.contrib.admin.util import model_ngettext
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import PermissionDenied
 from django.template.response import TemplateResponse
 try:
     # Django > 1.4.2
-    from django.utils.encoding import force_text
+    from django.utils.encoding import force_str
 except ImportError:
     # Django 1.4.2
     from django.utils.encoding import force_unicode as force_text
 from django.utils.html import conditional_escape
 from django.utils.six import text_type
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 def highlight_deleted(obj):
     """
         Display in red lines when object is deleted.
     """
     obj_str = conditional_escape(text_type(obj))
```

### Comparing `django-safedelete-e2e-0.3.6/safedelete/managers.py` & `django-safedelete-e2e-0.3.7/safedelete/managers.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/models.py` & `django-safedelete-e2e-0.3.7/safedelete/models.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/settings.py` & `django-safedelete-e2e-0.3.7/safedelete/settings.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/templates/safedelete/undelete_selected_confirmation.html` & `django-safedelete-e2e-0.3.7/safedelete/templates/safedelete/undelete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/tests.py` & `django-safedelete-e2e-0.3.7/safedelete/tests.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/safedelete/utils.py` & `django-safedelete-e2e-0.3.7/safedelete/utils.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.6/setup.py` & `django-safedelete-e2e-0.3.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,37 +7,23 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open('README.rst', 'r') as f_readme:
     with open('CHANGES', 'r') as f_changes:
         long_description = f_readme.read() + '\n\n' + f_changes.read()
 
 
-def get_version(package_name):
-    version_re = re.compile(r"^__version__ = [\"']([\w_.-]+)[\"']$")
-    package_components = package_name.split('.')
-    init_path = os.path.join(here, *(package_components + ['__init__.py']))
-    with codecs.open(init_path, 'r', 'utf-8') as f:
-        for line in f:
-            match = version_re.match(line.strip())
-            if match:
-                return match.groups()[0]
-    raise RuntimeError("Unable to find version string.")
-
-version = get_version('safedelete')
-
 setup(
     name='django-safedelete-e2e',
     packages=find_packages(),
-    version=version,
+    version='0.3.7',
     description='Mask your objects instead of deleting them from your database.',
     long_description=long_description,
     author='rounak kabra',
     author_email='rounak.kabra@e2enetworks.com',
     url='https://github.com/Roniee007/django-safedelete-e2e',
-    download_url='https://github.com/makinacorpus/django-safedelete/tarball/%s' % version,
     keywords=['django', 'delete', 'safedelete', 'softdelete'],
     classifiers=[
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
```

