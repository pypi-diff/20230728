# Comparing `tmp/qbwrap-1.0.0.tar.gz` & `tmp/qbwrap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbwrap-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qbwrap-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qbwrap-1.0.0.tar` & `qbwrap-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2129 2023-07-19 18:44:44.798173 qbwrap-1.0.0/README.md
--rw-r--r--   0        0        0      552 2023-07-12 20:08:48.342696 qbwrap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-04 19:23:02.823905 qbwrap-1.0.0/qbwrap/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 22:41:28.390993 qbwrap-1.0.0/qbwrap/action/__init__.py
--rw-r--r--   0        0        0     4593 2023-07-23 11:06:46.602283 qbwrap-1.0.0/qbwrap/action/main_action.py
--rw-r--r--   0        0        0     1636 2023-07-21 07:35:12.294168 qbwrap-1.0.0/qbwrap/action/run_action.py
--rw-r--r--   0        0        0     2022 2023-07-11 00:43:30.583631 qbwrap-1.0.0/qbwrap/action/setup_action.py
--rw-r--r--   0        0        0        0 2023-07-04 21:23:00.989319 qbwrap-1.0.0/qbwrap/dao/__init__.py
--rw-r--r--   0        0        0     5102 2023-07-23 21:20:21.218454 qbwrap-1.0.0/qbwrap/dao/argument_parser_dao.py
--rw-r--r--   0        0        0      769 2023-07-23 11:14:02.473225 qbwrap-1.0.0/qbwrap/dao/fields_dao.py
--rw-r--r--   0        0        0     6517 2023-07-24 13:40:02.276463 qbwrap-1.0.0/qbwrap/dao/qbwrap_options_dao.py
--rw-r--r--   0        0        0     3045 2023-07-21 08:28:04.666651 qbwrap-1.0.0/qbwrap/dao/qbwrap_setup_dao.py
--rw-r--r--   0        0        0      522 2023-07-24 13:41:08.279434 qbwrap-1.0.0/qbwrap/dao/qbwrap_stanza_delegate_dao.py
--rw-r--r--   0        0        0     1209 2023-07-23 11:12:21.237114 qbwrap-1.0.0/qbwrap/dao/reference_dao.py
--rw-r--r--   0        0        0        0 2023-07-04 21:36:14.821629 qbwrap-1.0.0/qbwrap/dto/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-13 17:07:04.073866 qbwrap-1.0.0/qbwrap/dto/bind_dto.py
--rw-r--r--   0        0        0      765 2023-07-13 17:07:08.383842 qbwrap-1.0.0/qbwrap/dto/field_dto.py
--rw-r--r--   0        0        0      817 2023-07-23 01:49:08.110059 qbwrap-1.0.0/qbwrap/dto/reference_dto.py
--rw-r--r--   0        0        0     1008 2023-07-13 17:07:11.890489 qbwrap-1.0.0/qbwrap/dto/tmpfs_device_dto.py
--rw-r--r--   0        0        0     1059 2023-07-24 13:28:23.293632 qbwrap-1.0.0/qbwrap/dto/tmpfs_device_options_dto.py
--rw-r--r--   0        0        0        0 2023-07-11 10:32:56.234833 qbwrap-1.0.0/qbwrap/helper/__init__.py
--rw-r--r--   0        0        0     1691 2023-07-23 11:07:30.042045 qbwrap-1.0.0/qbwrap/helper/bwrap_action_helper.py
--rw-r--r--   0        0        0     1959 2023-07-20 23:16:06.703247 qbwrap-1.0.0/qbwrap/helper/qbwrap_config_collection_helper.py
--rw-r--r--   0        0        0     1251 2023-07-13 20:44:21.880466 qbwrap-1.0.0/qbwrap/helper/qbwrap_config_file_helper.py
--rw-r--r--   0        0        0     2389 2023-07-21 11:40:42.029754 qbwrap-1.0.0/qbwrap/helper/qbwrap_config_finder_helper.py
--rw-r--r--   0        0        0        0 2023-07-04 20:27:26.207618 qbwrap-1.0.0/qbwrap/stanza/__init__.py
--rw-r--r--   0        0        0     2121 2023-07-24 13:29:50.396488 qbwrap-1.0.0/qbwrap/stanza/base_stanza.py
--rw-r--r--   0        0        0     1475 2023-07-24 13:36:38.734247 qbwrap-1.0.0/qbwrap/stanza/core_stanza.py
--rw-r--r--   0        0        0     1322 2023-07-24 13:33:06.038747 qbwrap-1.0.0/qbwrap/stanza/emulation_stanza.py
--rw-r--r--   0        0        0     2168 2023-07-24 12:56:56.367320 qbwrap-1.0.0/qbwrap/stanza/mount_stanza.py
--rw-r--r--   0        0        0     2385 2023-07-24 13:06:53.737375 qbwrap-1.0.0/qbwrap/stanza/setup_stanza.py
--rw-r--r--   0        0        0     1563 2023-07-07 01:05:34.247944 qbwrap-1.0.0/qbwrap/stanza/unshare_stanza.py
--rw-r--r--   0        0        0      815 2023-07-06 20:18:58.295366 qbwrap-1.0.0/qbwrap/stanza/user_stanza.py
--rw-r--r--   0        0        0        0 2023-07-04 19:16:35.899361 qbwrap-1.0.0/qbwrap/starter/__init__.py
--rw-r--r--   0        0        0      413 2023-07-13 15:13:43.384036 qbwrap-1.0.0/qbwrap/starter/main.py
--rw-r--r--   0        0        0        0 2023-07-04 22:58:43.887293 qbwrap-1.0.0/qbwrap/util/__init__.py
--rw-r--r--   0        0        0      537 2023-07-20 23:24:06.640614 qbwrap-1.0.0/qbwrap/util/bind_util.py
--rw-r--r--   0        0        0      884 2023-07-11 14:46:59.951725 qbwrap-1.0.0/qbwrap/util/device_util.py
--rw-r--r--   0        0        0      413 2023-07-24 13:26:15.660999 qbwrap-1.0.0/qbwrap/util/file_util.py
--rw-r--r--   0        0        0     1053 2023-07-13 15:19:04.832272 qbwrap-1.0.0/qbwrap/util/list_util.py
--rw-r--r--   0        0        0      593 2023-07-23 01:54:48.508191 qbwrap-1.0.0/qbwrap/util/reference_util.py
--rw-r--r--   0        0        0      575 2023-07-21 08:32:40.208472 qbwrap-1.0.0/qbwrap/util/sha_util.py
--rw-r--r--   0        0        0     1092 2023-07-24 13:42:17.742386 qbwrap-1.0.0/qbwrap/util/size_util.py
--rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 qbwrap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2658 2023-07-28 00:18:57.984019 qbwrap-1.1.0/README.md
+-rw-r--r--   0        0        0      719 2023-07-27 22:32:04.336530 qbwrap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-28 10:29:45.710678 qbwrap-1.1.0/qbwrap/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:41:28.390993 qbwrap-1.1.0/qbwrap/action/__init__.py
+-rw-r--r--   0        0        0     4593 2023-07-23 11:06:46.602283 qbwrap-1.1.0/qbwrap/action/main_action.py
+-rw-r--r--   0        0        0     1636 2023-07-21 07:35:12.294168 qbwrap-1.1.0/qbwrap/action/run_action.py
+-rw-r--r--   0        0        0     2022 2023-07-11 00:43:30.583631 qbwrap-1.1.0/qbwrap/action/setup_action.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:23:00.989319 qbwrap-1.1.0/qbwrap/dao/__init__.py
+-rw-r--r--   0        0        0     5102 2023-07-23 21:20:21.218454 qbwrap-1.1.0/qbwrap/dao/argument_parser_dao.py
+-rw-r--r--   0        0        0      769 2023-07-23 11:14:02.473225 qbwrap-1.1.0/qbwrap/dao/fields_dao.py
+-rw-r--r--   0        0        0     6517 2023-07-24 13:40:02.276463 qbwrap-1.1.0/qbwrap/dao/qbwrap_options_dao.py
+-rw-r--r--   0        0        0     3045 2023-07-21 08:28:04.666651 qbwrap-1.1.0/qbwrap/dao/qbwrap_setup_dao.py
+-rw-r--r--   0        0        0      522 2023-07-24 13:41:08.279434 qbwrap-1.1.0/qbwrap/dao/qbwrap_stanza_delegate_dao.py
+-rw-r--r--   0        0        0     1209 2023-07-23 11:12:21.237114 qbwrap-1.1.0/qbwrap/dao/reference_dao.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:36:14.821629 qbwrap-1.1.0/qbwrap/dto/__init__.py
+-rw-r--r--   0        0        0     1007 2023-07-13 17:07:04.073866 qbwrap-1.1.0/qbwrap/dto/bind_dto.py
+-rw-r--r--   0        0        0      765 2023-07-13 17:07:08.383842 qbwrap-1.1.0/qbwrap/dto/field_dto.py
+-rw-r--r--   0        0        0      817 2023-07-23 01:49:08.110059 qbwrap-1.1.0/qbwrap/dto/reference_dto.py
+-rw-r--r--   0        0        0     1008 2023-07-13 17:07:11.890489 qbwrap-1.1.0/qbwrap/dto/tmpfs_device_dto.py
+-rw-r--r--   0        0        0     1059 2023-07-24 13:28:23.293632 qbwrap-1.1.0/qbwrap/dto/tmpfs_device_options_dto.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:32:56.234833 qbwrap-1.1.0/qbwrap/helper/__init__.py
+-rw-r--r--   0        0        0     1691 2023-07-23 11:07:30.042045 qbwrap-1.1.0/qbwrap/helper/bwrap_action_helper.py
+-rw-r--r--   0        0        0     1959 2023-07-20 23:16:06.703247 qbwrap-1.1.0/qbwrap/helper/qbwrap_config_collection_helper.py
+-rw-r--r--   0        0        0     1251 2023-07-13 20:44:21.880466 qbwrap-1.1.0/qbwrap/helper/qbwrap_config_file_helper.py
+-rw-r--r--   0        0        0     2389 2023-07-21 11:40:42.029754 qbwrap-1.1.0/qbwrap/helper/qbwrap_config_finder_helper.py
+-rw-r--r--   0        0        0        0 2023-07-04 20:27:26.207618 qbwrap-1.1.0/qbwrap/stanza/__init__.py
+-rw-r--r--   0        0        0     2121 2023-07-24 13:29:50.396488 qbwrap-1.1.0/qbwrap/stanza/base_stanza.py
+-rw-r--r--   0        0        0     1475 2023-07-24 13:36:38.734247 qbwrap-1.1.0/qbwrap/stanza/core_stanza.py
+-rw-r--r--   0        0        0     1322 2023-07-24 13:33:06.038747 qbwrap-1.1.0/qbwrap/stanza/emulation_stanza.py
+-rw-r--r--   0        0        0     2168 2023-07-24 12:56:56.367320 qbwrap-1.1.0/qbwrap/stanza/mount_stanza.py
+-rw-r--r--   0        0        0     2319 2023-07-27 13:25:15.988754 qbwrap-1.1.0/qbwrap/stanza/setup_stanza.py
+-rw-r--r--   0        0        0     1563 2023-07-07 01:05:34.247944 qbwrap-1.1.0/qbwrap/stanza/unshare_stanza.py
+-rw-r--r--   0        0        0      815 2023-07-06 20:18:58.295366 qbwrap-1.1.0/qbwrap/stanza/user_stanza.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:16:35.899361 qbwrap-1.1.0/qbwrap/starter/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-13 15:13:43.384036 qbwrap-1.1.0/qbwrap/starter/main.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:58:43.887293 qbwrap-1.1.0/qbwrap/util/__init__.py
+-rw-r--r--   0        0        0      537 2023-07-20 23:24:06.640614 qbwrap-1.1.0/qbwrap/util/bind_util.py
+-rw-r--r--   0        0        0      884 2023-07-11 14:46:59.951725 qbwrap-1.1.0/qbwrap/util/device_util.py
+-rw-r--r--   0        0        0      413 2023-07-24 13:26:15.660999 qbwrap-1.1.0/qbwrap/util/file_util.py
+-rw-r--r--   0        0        0     1053 2023-07-13 15:19:04.832272 qbwrap-1.1.0/qbwrap/util/list_util.py
+-rw-r--r--   0        0        0      593 2023-07-23 01:54:48.508191 qbwrap-1.1.0/qbwrap/util/reference_util.py
+-rw-r--r--   0        0        0      575 2023-07-21 08:32:40.208472 qbwrap-1.1.0/qbwrap/util/sha_util.py
+-rw-r--r--   0        0        0     1092 2023-07-24 13:42:17.742386 qbwrap-1.1.0/qbwrap/util/size_util.py
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 qbwrap-1.1.0/PKG-INFO
```

### Comparing `qbwrap-1.0.0/README.md` & `qbwrap-1.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 ]
 tmpfs = [
     ["/dev/shm", {}],
     ["/tmp", {perms = "1777"}],
 ]
 ```
 
+## Documentation
+
+Documentation can either be built locally or browsed online on
+[GitLab pages](https://xgqt.gitlab.io/xgqt-python-app-qbwrap/).
+
 ## Command-line interface
 
 ### Usage
 
 ```text
 qbwrap [-h] [-V] [-q] [-f] [-r]
        [-R ROOT_METHOD] [-S DEV_SIZE] [-e EXECUTABLE] [-p PROCESS] [-m MERGE]
@@ -76,7 +81,25 @@
   -P COLLECTION_PATH, --collection-path COLLECTION_PATH
                         overwrite path of the QBwrap collection
   -c {default,always,never}, --use-collection {default,always,never}
                         whether and how to use the QBwrap collection
   --no-setup            do not run setup (from the setup stanza) even if required
   --force-setup         force to run setup defined in the setup stanza
 ```
+
+## Installation
+
+### PyPi
+
+Available at [pypi.org/project/qbwrap](https://pypi.org/project/qbwrap/).
+
+```shell
+pip install --user --break-system-packages qbwrap
+```
+
+### Repository
+
+See instructions in the
+[xgqt-python-app-qbwrap](https://gitlab.com/xgqt/xgqt-python-app-qbwrap)
+repository's
+[README.md](https://gitlab.com/xgqt/xgqt-python-app-qbwrap/-/blob/master/README.md)
+file.
```

### Comparing `qbwrap-1.0.0/qbwrap/action/main_action.py` & `qbwrap-1.1.0/qbwrap/action/main_action.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/action/run_action.py` & `qbwrap-1.1.0/qbwrap/action/run_action.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/action/setup_action.py` & `qbwrap-1.1.0/qbwrap/action/setup_action.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/argument_parser_dao.py` & `qbwrap-1.1.0/qbwrap/dao/argument_parser_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/fields_dao.py` & `qbwrap-1.1.0/qbwrap/dao/fields_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/qbwrap_options_dao.py` & `qbwrap-1.1.0/qbwrap/dao/qbwrap_options_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/qbwrap_setup_dao.py` & `qbwrap-1.1.0/qbwrap/dao/qbwrap_setup_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/qbwrap_stanza_delegate_dao.py` & `qbwrap-1.1.0/qbwrap/dao/qbwrap_stanza_delegate_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dao/reference_dao.py` & `qbwrap-1.1.0/qbwrap/dao/reference_dao.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dto/bind_dto.py` & `qbwrap-1.1.0/qbwrap/dto/bind_dto.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dto/field_dto.py` & `qbwrap-1.1.0/qbwrap/dto/field_dto.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dto/reference_dto.py` & `qbwrap-1.1.0/qbwrap/dto/reference_dto.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dto/tmpfs_device_dto.py` & `qbwrap-1.1.0/qbwrap/dto/tmpfs_device_dto.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/dto/tmpfs_device_options_dto.py` & `qbwrap-1.1.0/qbwrap/dto/tmpfs_device_options_dto.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/helper/bwrap_action_helper.py` & `qbwrap-1.1.0/qbwrap/helper/bwrap_action_helper.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/helper/qbwrap_config_collection_helper.py` & `qbwrap-1.1.0/qbwrap/helper/qbwrap_config_collection_helper.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/helper/qbwrap_config_file_helper.py` & `qbwrap-1.1.0/qbwrap/helper/qbwrap_config_file_helper.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/helper/qbwrap_config_finder_helper.py` & `qbwrap-1.1.0/qbwrap/helper/qbwrap_config_finder_helper.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/base_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/base_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/core_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/core_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/emulation_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/emulation_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/mount_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/mount_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/setup_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/setup_stanza.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 class SetupStanza(BaseStanza):
     """! Setup stanza"""
 
     def __init__(self):
         super().__init__(stanza_name="setup")
 
         self.get_fields_dao().add_field(FieldDTO("url", str))
-        self.get_fields_dao().add_field(FieldDTO("archive", str))
         self.get_fields_dao().add_field(FieldDTO("sha", str))
         self.get_fields_dao().add_field(FieldDTO("privileged", bool))
 
         self.bind_fields()
 
     def __get_url_archive(self) -> str:
         """! Return basename of setup.url."""
```

### Comparing `qbwrap-1.0.0/qbwrap/stanza/unshare_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/unshare_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/stanza/user_stanza.py` & `qbwrap-1.1.0/qbwrap/stanza/user_stanza.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/bind_util.py` & `qbwrap-1.1.0/qbwrap/util/bind_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/device_util.py` & `qbwrap-1.1.0/qbwrap/util/device_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/list_util.py` & `qbwrap-1.1.0/qbwrap/util/list_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/reference_util.py` & `qbwrap-1.1.0/qbwrap/util/reference_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/sha_util.py` & `qbwrap-1.1.0/qbwrap/util/sha_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/qbwrap/util/size_util.py` & `qbwrap-1.1.0/qbwrap/util/size_util.py`

 * *Files identical despite different names*

### Comparing `qbwrap-1.0.0/PKG-INFO` & `qbwrap-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbwrap
-Version: 1.0.0
+Version: 1.1.0
 Summary: This Source Code Form is subject to the terms of the Mozilla Public
 Author-email: Maciej Barć <xgqt@riseup.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -45,14 +45,19 @@
 ]
 tmpfs = [
     ["/dev/shm", {}],
     ["/tmp", {perms = "1777"}],
 ]
 ```
 
+## Documentation
+
+Documentation can either be built locally or browsed online on
+[GitLab pages](https://xgqt.gitlab.io/xgqt-python-app-qbwrap/).
+
 ## Command-line interface
 
 ### Usage
 
 ```text
 qbwrap [-h] [-V] [-q] [-f] [-r]
        [-R ROOT_METHOD] [-S DEV_SIZE] [-e EXECUTABLE] [-p PROCESS] [-m MERGE]
@@ -90,7 +95,25 @@
                         overwrite path of the QBwrap collection
   -c {default,always,never}, --use-collection {default,always,never}
                         whether and how to use the QBwrap collection
   --no-setup            do not run setup (from the setup stanza) even if required
   --force-setup         force to run setup defined in the setup stanza
 ```
 
+## Installation
+
+### PyPi
+
+Available at [pypi.org/project/qbwrap](https://pypi.org/project/qbwrap/).
+
+```shell
+pip install --user --break-system-packages qbwrap
+```
+
+### Repository
+
+See instructions in the
+[xgqt-python-app-qbwrap](https://gitlab.com/xgqt/xgqt-python-app-qbwrap)
+repository's
+[README.md](https://gitlab.com/xgqt/xgqt-python-app-qbwrap/-/blob/master/README.md)
+file.
+
```

