# Comparing `tmp/wagtail-import-export-updated-0.1.4.tar.gz` & `tmp/wagtail-import-export-updated-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-import-export-updated-0.1.4.tar", last modified: Sun Jan 29 00:01:46 2023, max compression
+gzip compressed data, was "wagtail-import-export-updated-0.1.5.tar", last modified: Fri Jul 28 14:22:56 2023, max compression
```

## Comparing `wagtail-import-export-updated-0.1.4.tar` & `wagtail-import-export-updated-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.300737 wagtail-import-export-updated-0.1.4/
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      520 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/CHANGELOG.txt
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     1585 2022-06-12 21:39:00.000000 wagtail-import-export-updated-0.1.4/LICENSE
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      124 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.4/MANIFEST.in
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     4231 2023-01-29 00:01:46.300318 wagtail-import-export-updated-0.1.4/PKG-INFO
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     3504 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/README.md
--rw-r--r--   0 besarbertasholli   (501) staff       (20)       38 2023-01-29 00:01:46.300842 wagtail-import-export-updated-0.1.4/setup.cfg
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      935 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/setup.py
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.290533 wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     4231 2023-01-29 00:01:46.000000 wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/PKG-INFO
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      963 2023-01-29 00:01:46.000000 wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/SOURCES.txt
--rw-r--r--   0 besarbertasholli   (501) staff       (20)        1 2023-01-29 00:01:46.000000 wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/dependency_links.txt
--rw-r--r--   0 besarbertasholli   (501) staff       (20)       20 2023-01-29 00:01:46.000000 wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/top_level.txt
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.295872 wagtail-import-export-updated-0.1.4/wagtailimportexport/
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     6148 2022-06-12 21:40:04.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/.DS_Store
--rw-r--r--   0 besarbertasholli   (501) staff       (20)       77 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/__init__.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      425 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/admin_urls.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      370 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/apps.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      950 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/compat.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     1505 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/exporting.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     1295 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/forms.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     4113 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/importing.py
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.286097 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.298539 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      989 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/export_to_file.html
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      990 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/import_from_api.html
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     1021 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/import_from_file.html
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      945 2022-07-04 21:08:42.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/index.html
-drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-01-29 00:01:46.299795 wagtail-import-export-updated-0.1.4/wagtailimportexport/tests/
--rw-r--r--   0 besarbertasholli   (501) staff       (20)        0 2022-06-12 21:40:57.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/tests/__init__.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      319 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/tests/test_functions.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      513 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/urls.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)     5063 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/views.py
--rw-r--r--   0 besarbertasholli   (501) staff       (20)      768 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.4/wagtailimportexport/wagtail_hooks.py
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.656264 wagtail-import-export-updated-0.1.5/
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      610 2023-07-28 14:11:06.000000 wagtail-import-export-updated-0.1.5/CHANGELOG.txt
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     1577 2023-07-28 14:19:02.000000 wagtail-import-export-updated-0.1.5/LICENSE
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      118 2023-07-28 14:18:12.000000 wagtail-import-export-updated-0.1.5/MANIFEST.in
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     4051 2023-07-28 14:22:56.656526 wagtail-import-export-updated-0.1.5/PKG-INFO
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     3324 2023-07-28 13:46:23.000000 wagtail-import-export-updated-0.1.5/README.md
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)       79 2023-07-28 14:09:48.000000 wagtail-import-export-updated-0.1.5/pyproject.toml
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      186 2023-07-28 14:22:56.657218 wagtail-import-export-updated-0.1.5/setup.cfg
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      983 2023-07-28 11:10:42.000000 wagtail-import-export-updated-0.1.5/setup.py
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.636476 wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     4051 2023-07-28 14:22:56.000000 wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/PKG-INFO
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      988 2023-07-28 14:22:56.000000 wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)        1 2023-07-28 14:22:56.000000 wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)       20 2023-07-28 14:22:56.000000 wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/top_level.txt
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.649416 wagtail-import-export-updated-0.1.5/wagtailimportexport/
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     6148 2022-06-12 21:40:04.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/.DS_Store
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      175 2023-07-28 11:09:57.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/__init__.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      425 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/admin_urls.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      247 2023-07-28 11:05:26.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/apps.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     1105 2023-07-28 11:04:09.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/compat.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     1505 2023-07-28 11:11:26.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/exporting.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     1295 2023-07-28 11:06:11.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/forms.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     4113 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/importing.py
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.627705 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.654129 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      989 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/export_to_file.html
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      990 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/import_from_api.html
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     1021 2022-06-09 11:48:39.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/import_from_file.html
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      945 2022-07-04 21:08:42.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/index.html
+drwxr-xr-x   0 besarbertasholli   (501) staff       (20)        0 2023-07-28 14:22:56.655643 wagtail-import-export-updated-0.1.5/wagtailimportexport/tests/
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)        0 2022-06-12 21:40:57.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/tests/__init__.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      319 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/tests/test_functions.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      513 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/urls.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)     5063 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/views.py
+-rw-r--r--   0 besarbertasholli   (501) staff       (20)      768 2023-01-29 00:00:36.000000 wagtail-import-export-updated-0.1.5/wagtailimportexport/wagtail_hooks.py
```

### Comparing `wagtail-import-export-updated-0.1.4/CHANGELOG.txt` & `wagtail-import-export-updated-0.1.5/CHANGELOG.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+0.1.5 (28.07.2023)
+~~~~~~~~~~~~~~~~
+  * Updated Wagtail imports to work with Wagtail > 4
+
 0.1.4 (29.01.2023)
 ~~~~~~~~~~~~~~~~
   * Updated Django url imports to be constantly from django.urls
 
 0.1.3 (08.07.2022)
 ~~~~~~~~~~~~~~~~
   * Implemented cleaner solution of Django versions with compat
```

### Comparing `wagtail-import-export-updated-0.1.4/LICENSE` & `wagtail-import-export-updated-0.1.5/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 BSD 3-Clause License
 
-Copyright (c) 2022 Besarber Tasholli
-Copyright (c) 2018-present Torchbox Ltd and individual contributors.
+Copyright (c) 2023 Besarber Tasholli
+Copyright (c) 2018 Torchbox Ltd and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 - Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `wagtail-import-export-updated-0.1.4/PKG-INFO` & `wagtail-import-export-updated-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-import-export-updated
-Version: 0.1.4
+Version: 0.1.5
 Summary: Import/Export for Wagtail CMS pages, images and documents.
 Home-page: https://github.com/besarbertasholli/wagtail-import-export-updated
 Author: Besarber Tasholli
 Author-email: besarbertasholli@hotmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,14 @@
 License-File: LICENSE
 
 # wagtail-import-export-updated
 
 Import/Export for Wagtail CMS pages, images, and documents from CSV, JSON, and API. Forked and updated for usability with new versions of Django/Wagtail, as the original library from Torchbox has not been edited since Apr 2019.
 Improvements in functionality, performance, documentation, views, etc will be published time after time.
 
-For a more powerful solution (focused on allowing content to be transferred between multiple instances of a Wagtail project), consider https://github.com/wagtail/wagtail-transfer
-
 A published page and its published descendants can be exported via API or file from a source site and imported into a destination site under an existing page.
 
 The destination site should have the same page models as the source site, with compatible migrations.
 
 ## Installation
 
     pip install wagtail-import-export-updated
```

### Comparing `wagtail-import-export-updated-0.1.4/README.md` & `wagtail-import-export-updated-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # wagtail-import-export-updated
 
 Import/Export for Wagtail CMS pages, images, and documents from CSV, JSON, and API. Forked and updated for usability with new versions of Django/Wagtail, as the original library from Torchbox has not been edited since Apr 2019.
 Improvements in functionality, performance, documentation, views, etc will be published time after time.
 
-For a more powerful solution (focused on allowing content to be transferred between multiple instances of a Wagtail project), consider https://github.com/wagtail/wagtail-transfer
-
 A published page and its published descendants can be exported via API or file from a source site and imported into a destination site under an existing page.
 
 The destination site should have the same page models as the source site, with compatible migrations.
 
 ## Installation
 
     pip install wagtail-import-export-updated
```

### Comparing `wagtail-import-export-updated-0.1.4/setup.py` & `wagtail-import-export-updated-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
+from wagtailimportexport import __version__
 
 setup(
     name="wagtail-import-export-updated",
-    version="0.1.4",
+    version=__version__,
     description="Import/Export for Wagtail CMS pages, images and documents.",
     author="Besarber Tasholli",
     author_email="besarbertasholli@hotmail.com",
     url="https://github.com/besarbertasholli/wagtail-import-export-updated",
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
```

### Comparing `wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/PKG-INFO` & `wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-import-export-updated
-Version: 0.1.4
+Version: 0.1.5
 Summary: Import/Export for Wagtail CMS pages, images and documents.
 Home-page: https://github.com/besarbertasholli/wagtail-import-export-updated
 Author: Besarber Tasholli
 Author-email: besarbertasholli@hotmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,14 @@
 License-File: LICENSE
 
 # wagtail-import-export-updated
 
 Import/Export for Wagtail CMS pages, images, and documents from CSV, JSON, and API. Forked and updated for usability with new versions of Django/Wagtail, as the original library from Torchbox has not been edited since Apr 2019.
 Improvements in functionality, performance, documentation, views, etc will be published time after time.
 
-For a more powerful solution (focused on allowing content to be transferred between multiple instances of a Wagtail project), consider https://github.com/wagtail/wagtail-transfer
-
 A published page and its published descendants can be exported via API or file from a source site and imported into a destination site under an existing page.
 
 The destination site should have the same page models as the source site, with compatible migrations.
 
 ## Installation
 
     pip install wagtail-import-export-updated
```

### Comparing `wagtail-import-export-updated-0.1.4/wagtail_import_export_updated.egg-info/SOURCES.txt` & `wagtail-import-export-updated-0.1.5/wagtail_import_export_updated.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 CHANGELOG.txt
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 wagtail_import_export_updated.egg-info/PKG-INFO
 wagtail_import_export_updated.egg-info/SOURCES.txt
 wagtail_import_export_updated.egg-info/dependency_links.txt
 wagtail_import_export_updated.egg-info/top_level.txt
 wagtailimportexport/.DS_Store
 wagtailimportexport/__init__.py
```

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/.DS_Store` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/compat.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/compat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 try:
+    from wagtail import hooks
+    from wagtail.models import Page
+except ImportError:  # fallback for Wagtail < 4.0
+    from wagtail.core import hooks
+    from wagtail.core.models import Page
+except Exception:  # last resort
+    from wagtail.wagtailcore import hooks
+    from wagtail.wagtailcore.models import Page
+
+try:
     from wagtail.admin import messages
     from wagtail.admin.menu import MenuItem
     from wagtail.admin.widgets import AdminPageChooser
-    from wagtail.core import hooks
-    from wagtail.core.models import Page
 
     WAGTAIL_VERSION_2_OR_GREATER = True
 except ImportError:  # fallback for Wagtail < 2.0
     from wagtail.wagtailadmin import messages
     from wagtail.wagtailadmin.menu import MenuItem
     from wagtail.wagtailadmin.widgets import AdminPageChooser
-    from wagtail.wagtailcore import hooks
-    from wagtail.wagtailcore.models import Page
 
     WAGTAIL_VERSION_2_OR_GREATER = False
 
 try:
     from django.utils.translation import (
         ngettext as ngettext,
         gettext as gettext,
```

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/exporting.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/exporting.py`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/forms.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/importing.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/importing.py`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/export_to_file.html` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/export_to_file.html`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/import_from_api.html` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/import_from_api.html`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/import_from_file.html` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/import_from_file.html`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/templates/wagtailimportexport/index.html` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/templates/wagtailimportexport/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/urls.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/views.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-import-export-updated-0.1.4/wagtailimportexport/wagtail_hooks.py` & `wagtail-import-export-updated-0.1.5/wagtailimportexport/wagtail_hooks.py`

 * *Files identical despite different names*

