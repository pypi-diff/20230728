# Comparing `tmp/pih_mio-1.48001.tar.gz` & `tmp/pih_mio-1.48002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48001.tar", last modified: Fri Jul 28 09:16:20 2023, max compression
+gzip compressed data, was "pih_mio-1.48002.tar", last modified: Fri Jul 28 09:21:24 2023, max compression
```

## Comparing `pih_mio-1.48001.tar` & `pih_mio-1.48002.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.504282 pih_mio-1.48001/
-drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.535545 pih_mio-1.48001/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48001/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165160 2023-07-28 09:13:23.000000 pih_mio-1.48001/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48001/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48001/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48001/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 09:16:20.958198 pih_mio-1.48001/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.895689 pih_mio-1.48001/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 09:16:19.000000 pih_mio-1.48001/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:16:19.000000 pih_mio-1.48001/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48001/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 09:16:20.958198 pih_mio-1.48001/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.585389 pih_mio-1.48002/
+drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.929136 pih_mio-1.48002/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48002/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165168 2023-07-28 09:19:10.000000 pih_mio-1.48002/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48002/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48002/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48002/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:21:24.335509 pih_mio-1.48002/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 09:21:23.991636 pih_mio-1.48002/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:21:22.000000 pih_mio-1.48002/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:21:22.000000 pih_mio-1.48002/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 09:21:23.000000 pih_mio-1.48002/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48002/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:21:24.335509 pih_mio-1.48002/setup.cfg
```

### Comparing `pih_mio-1.48001/MobileHelperCore/api.py` & `pih_mio-1.48002/MobileHelperCore/api.py`

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
-from BackupCore.api import BackupApi
 import requests
 from io import BytesIO
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
@@ -1308,14 +1307,15 @@
         dump_name: str = PolibaseDBApi.get_default_name()
         answer: bool = self.input.yes_no(
             f"Изменить имя файла дампа базы данных", False, b("Отправьте имя"), f"Использовать имя: {b(dump_name)} - отправьте {A.CT.VISUAL.NUMBER_SYMBOLS[0]}")
         if A.A_P.DB.backup(self.input.answer if answer else dump_name):
             self.write_line(i(f"{self.user_given_name}, ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе {b('Backup Console')}"))
 
     def robocopy_job_run_handler(self) -> None:
+        from BackupCore.api import BackupApi
         forced: bool = self.is_forced
         source_job_name: str | None = self.first_arg()
         if not A.D_C.empty(source_job_name):
             source_job_name = source_job_name.lower()
         job_name_set: set = set()
         job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = defaultdict(list)
         job_status_list: list[RobocopyJobStatus] = A.R_B.robocopy_job_status_list().data
```

### Comparing `pih_mio-1.48001/MobileHelperCore/service.py` & `pih_mio-1.48002/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48001/MobileHelperCore/service_api.py` & `pih_mio-1.48002/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48001/MobileHelperCore/tools.py` & `pih_mio-1.48002/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48001/pih_mio_setup.py` & `pih_mio-1.48002/pih_mio_setup.py`

 * *Files identical despite different names*

