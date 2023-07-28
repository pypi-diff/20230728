# Comparing `tmp/django-lab-inventory-0.5.1.tar.gz` & `tmp/django-lab-inventory-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lab-inventory-0.5.1.tar", last modified: Sun Jul 23 12:19:31 2023, max compression
+gzip compressed data, was "django-lab-inventory-0.5.2.tar", last modified: Fri Jul 28 17:56:38 2023, max compression
```

## Comparing `django-lab-inventory-0.5.1.tar` & `django-lab-inventory-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.593927 django-lab-inventory-0.5.1/
--rw-r--r--   0 dmeliza    (503) staff       (20)       44 2014-05-14 21:02:10.000000 django-lab-inventory-0.5.1/.gitignore
--rw-r--r--   0 dmeliza    (503) staff       (20)     1461 2023-01-24 20:31:22.000000 django-lab-inventory-0.5.1/COPYING
--rw-r--r--   0 dmeliza    (503) staff       (20)      168 2023-07-23 12:18:34.000000 django-lab-inventory-0.5.1/MANIFEST.in
--rw-r--r--   0 dmeliza    (503) staff       (20)     2261 2023-07-23 12:19:31.594049 django-lab-inventory-0.5.1/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)     1484 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.574317 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2261 2023-07-23 12:19:31.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)     1515 2023-07-23 12:19:31.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-07-23 12:19:31.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-01-24 20:22:01.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)       49 2023-07-23 12:19:31.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/requires.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)       10 2023-07-23 12:19:31.000000 django-lab-inventory-0.5.1/django_lab_inventory.egg-info/top_level.txt
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.577238 django-lab-inventory-0.5.1/inventory/
--rw-r--r--   0 dmeliza    (503) staff       (20)       69 2023-07-23 12:19:07.000000 django-lab-inventory-0.5.1/inventory/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2302 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/admin.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1694 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/forms.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.586746 django-lab-inventory-0.5.1/inventory/migrations/
--rw-r--r--   0 dmeliza    (503) staff       (20)     7543 2019-01-19 00:40:08.000000 django-lab-inventory-0.5.1/inventory/migrations/0001_initial.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     7952 2019-01-19 00:42:07.000000 django-lab-inventory-0.5.1/inventory/migrations/0001_squashed_0003_auto_20150626_1807.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      701 2015-06-26 22:05:53.000000 django-lab-inventory-0.5.1/inventory/migrations/0002_auto_20150626_1805.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2024 2017-06-23 21:16:49.000000 django-lab-inventory-0.5.1/inventory/migrations/0002_auto_20170623_1716.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      660 2018-03-09 17:39:57.000000 django-lab-inventory-0.5.1/inventory/migrations/0003_add_vendor_email.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      663 2015-06-26 22:07:04.000000 django-lab-inventory-0.5.1/inventory/migrations/0003_auto_20150626_1807.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1589 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.1/inventory/migrations/0004_alter_category_id_alter_item_id_and_more.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      722 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/migrations/0005_rename_ptao_account_alter_account_options_and_more.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      395 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/migrations/0006_rename_ptao_order_account.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     2393 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/migrations/0007_remove_duplicates.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1434 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/migrations/0008_add_uniqueness_constraints.py
--rw-r--r--   0 dmeliza    (503) staff       (20)        0 2014-05-14 16:16:37.000000 django-lab-inventory-0.5.1/inventory/migrations/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     7055 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/models.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.587629 django-lab-inventory-0.5.1/inventory/templates/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2635 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.1/inventory/templates/base_view.html
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-23 12:19:31.593601 django-lab-inventory-0.5.1/inventory/templates/inventory/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2440 2023-07-20 17:27:51.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/base.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     1093 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/index.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     3545 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/item.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     1305 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/item_entry.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     2411 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/item_list.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     2742 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/order.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     1327 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/order_entry.html
--rw-r--r--   0 dmeliza    (503) staff       (20)     1764 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/order_list.html
--rw-r--r--   0 dmeliza    (503) staff       (20)        0 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/templates/inventory/order_table.html
--rw-r--r--   0 dmeliza    (503) staff       (20)       60 2023-07-20 17:28:57.000000 django-lab-inventory-0.5.1/inventory/tests.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      726 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.1/inventory/urls.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     4981 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.1/inventory/views.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1066 2023-07-23 12:19:31.597871 django-lab-inventory-0.5.1/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)       84 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.1/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.554487 django-lab-inventory-0.5.2/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       44 2014-05-14 21:02:10.000000 django-lab-inventory-0.5.2/.gitignore
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1461 2023-01-24 20:31:22.000000 django-lab-inventory-0.5.2/COPYING
+-rw-r--r--   0 dmeliza    (503) staff       (20)      168 2023-07-23 12:18:34.000000 django-lab-inventory-0.5.2/MANIFEST.in
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2261 2023-07-28 17:56:38.554585 django-lab-inventory-0.5.2/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1484 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/README.md
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.519306 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2261 2023-07-28 17:56:38.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1628 2023-07-28 17:56:38.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-07-28 17:56:38.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-01-24 20:22:01.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)       49 2023-07-28 17:56:38.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       10 2023-07-28 17:56:38.000000 django-lab-inventory-0.5.2/django_lab_inventory.egg-info/top_level.txt
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.526321 django-lab-inventory-0.5.2/inventory/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       69 2023-07-28 17:55:21.000000 django-lab-inventory-0.5.2/inventory/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2302 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/admin.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1694 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/forms.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.534723 django-lab-inventory-0.5.2/inventory/migrations/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7543 2019-01-19 00:40:08.000000 django-lab-inventory-0.5.2/inventory/migrations/0001_initial.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7952 2019-01-19 00:42:07.000000 django-lab-inventory-0.5.2/inventory/migrations/0001_squashed_0003_auto_20150626_1807.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      701 2015-06-26 22:05:53.000000 django-lab-inventory-0.5.2/inventory/migrations/0002_auto_20150626_1805.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2024 2017-06-23 21:16:49.000000 django-lab-inventory-0.5.2/inventory/migrations/0002_auto_20170623_1716.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      660 2018-03-09 17:39:57.000000 django-lab-inventory-0.5.2/inventory/migrations/0003_add_vendor_email.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      663 2015-06-26 22:07:04.000000 django-lab-inventory-0.5.2/inventory/migrations/0003_auto_20150626_1807.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1589 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.2/inventory/migrations/0004_alter_category_id_alter_item_id_and_more.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      722 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/migrations/0005_rename_ptao_account_alter_account_options_and_more.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      395 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/migrations/0006_rename_ptao_order_account.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2393 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/migrations/0007_remove_duplicates.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1434 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/migrations/0008_add_uniqueness_constraints.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)        0 2014-05-14 16:16:37.000000 django-lab-inventory-0.5.2/inventory/migrations/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7055 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/models.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.537670 django-lab-inventory-0.5.2/inventory/templates/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2635 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.2/inventory/templates/base_view.html
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-07-28 17:56:38.554173 django-lab-inventory-0.5.2/inventory/templates/inventory/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2440 2023-07-20 17:27:51.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/base.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1093 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/index.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     3545 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/item.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1305 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/item_entry.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2411 2023-07-23 12:07:10.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/item_list.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2910 2023-07-28 17:54:09.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/order.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1327 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/order_entry.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1764 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/order_list.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)      786 2023-07-28 17:41:15.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/order_mark_placed.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)        0 2023-07-21 18:56:23.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/order_table.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)      837 2023-07-28 17:35:10.000000 django-lab-inventory-0.5.2/inventory/templates/inventory/orderitem_confirm_delete.html
+-rw-r--r--   0 dmeliza    (503) staff       (20)       60 2023-07-20 17:28:57.000000 django-lab-inventory-0.5.2/inventory/tests.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1219 2023-07-28 17:53:56.000000 django-lab-inventory-0.5.2/inventory/urls.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     5566 2023-07-28 17:51:30.000000 django-lab-inventory-0.5.2/inventory/views.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1066 2023-07-28 17:56:38.556744 django-lab-inventory-0.5.2/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)       84 2023-01-24 20:21:36.000000 django-lab-inventory-0.5.2/setup.py
```

### Comparing `django-lab-inventory-0.5.1/COPYING` & `django-lab-inventory-0.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/PKG-INFO` & `django-lab-inventory-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lab-inventory
-Version: 0.5.1
+Version: 0.5.2
 Summary: A simple Django app for managing lab inventory
 Home-page: https://github.com/melizalab/django-lab-inventory
 Author: C Daniel Meliza
 Author-email: dan@meliza.org
 Maintainer: C Daniel Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `django-lab-inventory-0.5.1/README.md` & `django-lab-inventory-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/django_lab_inventory.egg-info/PKG-INFO` & `django-lab-inventory-0.5.2/django_lab_inventory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lab-inventory
-Version: 0.5.1
+Version: 0.5.2
 Summary: A simple Django app for managing lab inventory
 Home-page: https://github.com/melizalab/django-lab-inventory
 Author: C Daniel Meliza
 Author-email: dan@meliza.org
 Maintainer: C Daniel Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
```

### Comparing `django-lab-inventory-0.5.1/django_lab_inventory.egg-info/SOURCES.txt` & `django-lab-inventory-0.5.2/django_lab_inventory.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,10 @@
 inventory/templates/inventory/index.html
 inventory/templates/inventory/item.html
 inventory/templates/inventory/item_entry.html
 inventory/templates/inventory/item_list.html
 inventory/templates/inventory/order.html
 inventory/templates/inventory/order_entry.html
 inventory/templates/inventory/order_list.html
-inventory/templates/inventory/order_table.html
+inventory/templates/inventory/order_mark_placed.html
+inventory/templates/inventory/order_table.html
+inventory/templates/inventory/orderitem_confirm_delete.html
```

### Comparing `django-lab-inventory-0.5.1/inventory/admin.py` & `django-lab-inventory-0.5.2/inventory/admin.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/forms.py` & `django-lab-inventory-0.5.2/inventory/forms.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0001_initial.py` & `django-lab-inventory-0.5.2/inventory/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0001_squashed_0003_auto_20150626_1807.py` & `django-lab-inventory-0.5.2/inventory/migrations/0001_squashed_0003_auto_20150626_1807.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0002_auto_20150626_1805.py` & `django-lab-inventory-0.5.2/inventory/migrations/0002_auto_20150626_1805.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0002_auto_20170623_1716.py` & `django-lab-inventory-0.5.2/inventory/migrations/0002_auto_20170623_1716.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0003_add_vendor_email.py` & `django-lab-inventory-0.5.2/inventory/migrations/0003_add_vendor_email.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0003_auto_20150626_1807.py` & `django-lab-inventory-0.5.2/inventory/migrations/0003_auto_20150626_1807.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0004_alter_category_id_alter_item_id_and_more.py` & `django-lab-inventory-0.5.2/inventory/migrations/0004_alter_category_id_alter_item_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0005_rename_ptao_account_alter_account_options_and_more.py` & `django-lab-inventory-0.5.2/inventory/migrations/0005_rename_ptao_account_alter_account_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0007_remove_duplicates.py` & `django-lab-inventory-0.5.2/inventory/migrations/0007_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/migrations/0008_add_uniqueness_constraints.py` & `django-lab-inventory-0.5.2/inventory/migrations/0008_add_uniqueness_constraints.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/models.py` & `django-lab-inventory-0.5.2/inventory/models.py`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/base_view.html` & `django-lab-inventory-0.5.2/inventory/templates/base_view.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/base.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/base.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/index.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/index.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/item.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/item.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/item_entry.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/item_entry.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/item_list.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/item_list.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/order.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/order.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 {% block content %}
 
 <h2>order: {{ order.name }}</h2>
 <hr>
 
 <dl class="dl-horizontal">
-  <dt>created on</dt><dd>{{ order.order_date }}</dd>
+  <dt>{{order.ordered|yesno:"ordered on,created on"}}</dt><dd>{{ order.order_date }}</dd>
   <dt>created by<dt><dd>{{ order.ordered_by.username}}</dd>
   <dt>account</dt><dd>{{ order.account }}</dd>
   <dt>status</dt><dd>{{ order.ordered|yesno:"ordered,in progress" }}</dd>
 </dl>
 
 <h3>items</h3>
 
@@ -52,23 +52,24 @@
           <td>{{ oit.total_price }}</td>
 	  {% if order.ordered %}
 	  <td>{{ oit.date_arrived|default:"no" }}</td>
 	  {% endif %}
           <td><a href="{% url 'admin:inventory_orderitem_change' oit.id %}"
                  class="glyphicon glyphicon-edit" alt="[edit]" aria-label="Edit"></a></td>
 	  {% if not order.ordered %}
-          <td><a href="{% url 'admin:inventory_orderitem_delete' oit.id %}"
+          <td><a href="{% url 'inventory:remove_item_from_order' oit.id %}"
                  class="glyphicon glyphicon-trash" alt="[delete]" aria-label="Delete"></a></td>
 	  {% endif %}
         </tr>
     {% endfor %}
   </tbody>
 </table>
 
 
 <hr>
 
 <p>To update information about an item after it has been received, click the <span class="glyphicon glyphicon-edit" alt="[edit]".  aria-label="Edit"></span> icon. {% if not order.ordered %} To add items to this order, search the <a href="{% url 'inventory:items' %}">items list</a> or <a href="{% url 'inventory:new_item' %}">add a new item</a>. To remove an item from the order, click the <span class="glyphicon glyphicon-trash" alt="[delete]" aria-label="Delete"></span> icon. {% endif %} </p>
 <a href="{% url 'inventory:orders' %}">back to order list</a><br/>
+{% if not order.ordered %}<a href="{% url 'inventory:mark_order_placed' order.id %}">mark this order as placed</a><br/>{% endif %}
 <a href="{% url 'admin:inventory_order_change' order.id %}">edit order (advanced users only)</a><br/>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "base_view.html" %} {% load widget_tweaks %} {% block title %}
 meliza-lab : order : {{ order.name }} {% endblock %} {% block content %}
 ***** order: {{ order.name }} *****
 ===============================================================================
-  created on
+  {{order.ordered|yesno:"ordered on,created on"}}
       {{ order.order_date }}
   created by
       {{ order.ordered_by.username}}
   account
       {{ order.account }}
   status
       {{ order.ordered|yesno:"ordered,in progress" }}
@@ -20,9 +20,10 @@
               }}{% endif %}       }}{% endif %}
 ===============================================================================
 To update information about an item after it has been received, click the
 aria-label="Edit"> icon. {% if not order.ordered %} To add items to this order,
 search the items_list or add_a_new_item. To remove an item from the order,
 click the  icon. {% endif %}
 back_to_order_list
-edit_order_(advanced_users_only)
+{% if not order.ordered %}mark_this_order_as_placed
+{% endif %} edit_order_(advanced_users_only)
 {% endblock %}
```

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/order_entry.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/order_entry.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/templates/inventory/order_list.html` & `django-lab-inventory-0.5.2/inventory/templates/inventory/order_list.html`

 * *Files identical despite different names*

### Comparing `django-lab-inventory-0.5.1/inventory/views.py` & `django-lab-inventory-0.5.2/inventory/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
+import datetime
+
 from django.shortcuts import get_object_or_404, redirect
 import django_filters as filters
 from django.db.models import Q
 from django.shortcuts import render
 from django.views import generic
 from django_filters.views import FilterView
 
-from inventory.models import Item, Order
+from inventory.models import Item, Order, OrderItem
 from inventory.forms import NewOrderForm, NewItemForm, NewOrderItemForm
 
 
 def index(request):
     return render(request, "inventory/index.html")
 
 
@@ -115,14 +117,28 @@
     def form_valid(self, form):
         order = form.save(commit=False)
         order.ordered = False
         order.save()
         return redirect("inventory:order", pk=order.id)
 
 
+class OrderMarkPlaced(generic.UpdateView):
+    model = Order
+    fields = ["ordered"]
+    template_name = "inventory/order_mark_placed.html"
+
+    def post(self, request, *args, **kwargs):
+        order_id = kwargs["pk"]
+        order = get_object_or_404(Order, id=order_id)
+        order.order_date = datetime.date.today()
+        order.ordered = True
+        order.save()
+        return redirect("inventory:order", pk=order_id)
+
+
 class ItemList(PaginatedFilterView):
     model = Item
     filterset_class = ItemFilter
     template_name = "inventory/item_list.html"
     context_object_name = "item_list"
 
     def get_queryset(self):
@@ -151,16 +167,21 @@
         item = form.save()
         return redirect("inventory:item", pk=item.id)
 
 
 class OrderItemEntry(generic.FormView):
     """Order an item (associate it with an order)"""
 
-    template_name = "inventory/orderitem_entry.html"
     form_class = NewOrderItemForm
 
     def form_valid(self, form):
         item_id = self.kwargs["pk"]
         form.instance.item = get_object_or_404(Item, pk=item_id)
         form.instance.reconciled = False
         oitem = form.save()
         return redirect("inventory:order", pk=oitem.order.id)
+
+
+class OrderItemDelete(generic.DeleteView):
+    model = OrderItem
+    template_name = "inventory/orderitem_confirm_delete.html"
+    success_url = "/inventory/orders/{order_id}/"
```

### Comparing `django-lab-inventory-0.5.1/setup.cfg` & `django-lab-inventory-0.5.2/setup.cfg`

 * *Files identical despite different names*

