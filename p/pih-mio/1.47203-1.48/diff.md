# Comparing `tmp/pih_mio-1.47203.tar.gz` & `tmp/pih_mio-1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.47203.tar", last modified: Fri Jul 28 08:40:35 2023, max compression
+gzip compressed data, was "pih_mio-1.48.tar", last modified: Fri Jul 28 09:14:52 2023, max compression
```

## Comparing `pih_mio-1.47203.tar` & `pih_mio-1.48.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 08:40:35.489890 pih_mio-1.47203/
-drwxrwxrwx   0        0        0        0 2023-07-28 08:40:35.756588 pih_mio-1.47203/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.47203/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165152 2023-07-28 07:22:07.000000 pih_mio-1.47203/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.47203/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.47203/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.47203/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 08:40:35.959709 pih_mio-1.47203/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 08:40:35.897238 pih_mio-1.47203/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 08:40:34.000000 pih_mio-1.47203/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-28 08:40:35.000000 pih_mio-1.47203/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 08:40:34.000000 pih_mio-1.47203/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 08:40:34.000000 pih_mio-1.47203/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 08:40:35.000000 pih_mio-1.47203/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1497 2023-07-28 08:36:59.000000 pih_mio-1.47203/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 08:40:35.959709 pih_mio-1.47203/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:51.509624 pih_mio-1.48/
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:51.853349 pih_mio-1.48/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165160 2023-07-28 09:13:23.000000 pih_mio-1.48/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      276 2023-07-28 09:14:52.259593 pih_mio-1.48/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:52.009607 pih_mio-1.48/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-28 09:14:51.000000 pih_mio-1.48/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:14:52.275218 pih_mio-1.48/setup.cfg
```

### Comparing `pih_mio-1.47203/MobileHelperCore/api.py` & `pih_mio-1.48/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from pih.collection import (User, Result, Workstation, 
                             RobocopyJobStatus, Mark, MarkGroup, 
                             FieldItem, FieldItemList, PolibasePerson, 
                             Note, ActionDescription, StorageValue, 
                             IntStorageValue, TimeStorageValue, BoolStorageValue,
                             CommandMenuItem)
 from MobileHelperContent.content import MEDIA_CONTENT
-from PolibaseDBCore.api import PolibaseDBApi
 from BackupCore.api import BackupApi
 import requests
 from io import BytesIO
 
 class InternalInterrupt(Exception):
 
     @property
@@ -1301,14 +1300,15 @@
         section_list = section_list or CheckableSections.all()
         self.console_apps_api.resources_and_indications_check(section_list, False, self.is_forced, all)
 
     def register_ct_indications_handler(self) -> None:
         self.console_apps_api.register_ct_indications()
 
     def create_polibase_db_backup_handler(self) -> None:
+        from PolibaseDBCore.api import PolibaseDBApi
         dump_name: str = PolibaseDBApi.get_default_name()
         answer: bool = self.input.yes_no(
             f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(dump_name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
         if A.A_P.DB.backup(self.input.answer if answer else dump_name):
             self.write_line(i(f"{self.user_given_name}, ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе {b('Backup Console')}"))
 
     def robocopy_job_run_handler(self) -> None:
```

### Comparing `pih_mio-1.47203/MobileHelperCore/service.py` & `pih_mio-1.48/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.47203/MobileHelperCore/service_api.py` & `pih_mio-1.48/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.47203/MobileHelperCore/tools.py` & `pih_mio-1.48/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.47203/pih_mio_setup.py` & `pih_mio-1.48/pih_mio_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
 setup(
     name=j((PIH.NAME, PIH.MIO.NAME), "_"),
-    version=PIH.VERSION.local(),
+    version=PIH.VERSION.MIO.local(),
     description="PIH Mobile Helper library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
```

