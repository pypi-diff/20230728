# Comparing `tmp/cadcutils-1.5.1.1.tar.gz` & `tmp/cadcutils-1.5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadcutils-1.5.1.1.tar", last modified: Fri Dec 16 22:22:03 2022, max compression
+gzip compressed data, was "cadcutils-1.5.1.2.tar", last modified: Fri Jul 28 15:47:13 2023, max compression
```

## Comparing `cadcutils-1.5.1.1.tar` & `cadcutils-1.5.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.596522 cadcutils-1.5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-16 22:22:03.596522 cadcutils-1.5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.584522 cadcutils-1.5.1.1/cadcutils/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.588522 cadcutils-1.5.1.1/cadcutils/net/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14480 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9055 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.592522 cadcutils-1.5.1.1/cadcutils/net/group_xml/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/group_property_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/group_property_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/group_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/group_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/groups_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/groups_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.592522 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_group_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_user_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/user_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/group_xml/user_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24635 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/groups_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/netutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.592522 cadcutils-1.5.1.1/cadcutils/net/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    18202 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_groups_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_int_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_netutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64617 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/tests/test_wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55249 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/ws.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12263 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/net/wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8457 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/old_get_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.596522 cadcutils-1.5.1.1/cadcutils/util/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/cadcutils/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-16 22:22:02.000000 cadcutils-1.5.1.1/cadcutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 22:22:03.584522 cadcutils-1.5.1.1/cadcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-16 22:22:03.000000 cadcutils-1.5.1.1/cadcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-16 22:22:03.596522 cadcutils-1.5.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3093 2022-12-16 22:21:53.000000 cadcutils-1.5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.284331 cadcutils-1.5.1.2/cadcutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.292331 cadcutils-1.5.1.2/cadcutils/net/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14480 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9055 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/group_xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/user_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/user_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29291 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/netutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20910 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_int_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_netutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64620 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55249 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/ws.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12263 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8457 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/old_get_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 15:47:11.000000 cadcutils-1.5.1.2/cadcutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.288331 cadcutils-1.5.1.2/cadcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.300331 cadcutils-1.5.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3093 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/setup.py
```

### Comparing `cadcutils-1.5.1.1/LICENSE` & `cadcutils-1.5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/PKG-INFO` & `cadcutils-1.5.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.1.1
+Version: 1.5.1.2
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.1.1/README.rst` & `cadcutils-1.5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/exceptions.py` & `cadcutils-1.5.1.2/cadcutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/__init__.py` & `cadcutils-1.5.1.2/cadcutils/net/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/auth.py` & `cadcutils-1.5.1.2/cadcutils/net/auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group.py` & `cadcutils-1.5.1.2/cadcutils/net/group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/__init__.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/group_property_reader.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/group_property_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/group_reader.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/group_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/groups_reader.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/groups_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_group_reader_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-# (c) 2021.                            (c) 2021.
+# (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -162,7 +162,46 @@
     assert(actual.last_modified == expected.last_modified)
 
     assert(actual.properties == expected.properties)
     assert(actual.group_members == expected.group_members)
     assert(actual.user_members == expected.user_members)
     assert(actual.group_admins == expected.group_admins)
     assert(actual.user_admins == expected.user_admins)
+
+
+def test_external_users():
+    # external users are users that do not have a CADC internal Identity
+    owner = User()
+    owner.identities['HTTP'] = Identity('foo', 'HTTP')
+
+    expected = Group('groupID')
+    expected.owner = owner
+    expected.description = 'description'
+    expected.last_modified = datetime(2014, 1, 20, 19, 45, 37, 0)
+
+    member = User()
+    owner.identities['X500'] = Identity('cn=tom,c=ca', 'X500')
+    admin = User()
+    admin.identities['X500'] = Identity('cn=jerry,c=ca', 'X500')
+    expected.user_members.add(member)
+    expected.user_admins.add(admin)
+
+    writer = GroupWriter()
+    xml_string = writer.write(expected, True)
+
+    assert(xml_string)
+    assert(len(xml_string) > 0)
+
+    reader = GroupReader()
+    actual = reader.read(xml_string)
+
+    assert expected.group_id
+    assert actual.group_id
+    assert(actual.group_id == expected.group_id)
+
+    assert(actual.owner.internal_id == expected.owner.internal_id)
+    assert(actual.owner.identities == expected.owner.identities)
+    assert(actual.description == expected.description)
+    assert(actual.last_modified == expected.last_modified)
+
+    assert(actual.user_members == expected.user_members)
+    assert(actual.user_admins == expected.user_admins)
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_groups_reader_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/tests/test_user_reader_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/user_reader.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/user_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-# (c) 2021.                            (c) 2021.
+# (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -81,26 +81,24 @@
         return : a User object
         """
         root = etree.fromstring(xml_string)
         return self.get_user(root)
 
     def get_user(self, user_element):
         internal_id_element = user_element.find('internalID')
-        if internal_id_element is None:
-            raise UserParsingException(
-                'internalID element not found in user element')
-
-        uri_element = internal_id_element.find('uri')
-        if uri_element is None:
-            raise UserParsingException(
-                'uri element not found in internalID element')
-
-        uri = uri_element.text
-        if not uri:
-            raise UserParsingException('uri element has no text value')
+        uri = None
+        if internal_id_element is not None:
+            uri_element = internal_id_element.find('uri')
+            if uri_element is None:
+                raise UserParsingException(
+                    'uri element not found in internalID element')
+
+            uri = uri_element.text
+            if not uri:
+                raise UserParsingException('uri element has no text value')
 
         user = User(uri)
 
         identities_element = user_element.findall('./identities/identity')
         for identity_element in identities_element:
             identity_type = identity_element.get('type')
             name = identity_element.text
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/group_xml/user_writer.py` & `cadcutils-1.5.1.2/cadcutils/net/group_xml/user_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2021.                            (c) 2021.
+#  (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -80,17 +80,18 @@
         return etree.tostring(self.get_user_element(user),
                               xml_declaration=declaration,
                               encoding='UTF-8',
                               pretty_print=True)
 
     def get_user_element(self, user):
         user_element = etree.Element('user')
-        internalid_element = etree.SubElement(user_element, 'internalID')
-        uri_element = etree.SubElement(internalid_element, 'uri')
-        uri_element.text = user.internal_id
+        if user.internal_id:
+            internalid_element = etree.SubElement(user_element, 'internalID')
+            uri_element = etree.SubElement(internalid_element, 'uri')
+            uri_element.text = user.internal_id
         if user.identities:
             identities_element = etree.SubElement(user_element, 'identities')
             for identity in user.identities.values():
                 identity_element = etree.SubElement(identities_element,
                                                     'identity')
                 identity_element.set('type', identity.type)
                 identity_element.text = identity.name
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/groups_client.py` & `cadcutils-1.5.1.2/cadcutils/net/groups_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2022.                            (c) 2022.
+#  (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -74,15 +74,15 @@
 import traceback
 import logging
 from urllib.parse import urlparse, urlencode
 
 
 from cadcutils import version  # TODO should it be application version instead?
 from cadcutils import util, exceptions
-from . import BaseWsClient, Subject
+from . import BaseWsClient, Subject, User
 from .auth import SECURITY_METHODS_IDS, CookieInfo
 from . import Role, Group, Identity
 from .group_xml import GroupWriter, GroupReader, GroupsReader
 
 
 CADC_LOGIN_CAPABILITY = 'ivo://ivoa.net/std/UMS#login-0.1'
 CADC_SSO_COOKIE_NAME = 'CADC_SSO'
@@ -387,14 +387,75 @@
         ['{} ({})'.format(
             m.identities['HTTP'].name,
             m.identities['X500'].name) for m in group.user_members])))
     print('  Group Members: {}'.format(
         (',\n'+' '*17).join([gr.group_id for gr in group.group_members])))
 
 
+def print_group_admins(group):
+    print('   User Administrators: {}'.format((',\n'+' '*17).join(
+        ['{} ({})'.format(
+            m.identities['HTTP'].name,
+            m.identities['X500'].name) for m in group.user_admins])))
+    print('  Group Administrators: {}'.format(
+        (',\n'+' '*17).join([gr.group_id for gr in group.group_admins])))
+
+
+def _add_admin_user(group, user):
+    if user.strip().lower().startswith('cn='):
+        id_type = 'X500'
+    else:
+        id_type = 'HTTP'
+    for admin_user in group.user_admins:
+        if (id_type in admin_user.identities) and admin_user.identities[id_type].name.lower() == user.strip().lower():
+            raise ValueError("User " + user.strip().lower() + " already in the admins group")
+    admin = User()
+    admin.identities[id_type] = Identity(user.strip().lower(), id_type)
+    group.add_user_admin(admin)
+
+
+def _remove_admin_users(group, users):
+    # removes user from group's admins or raises ValueError if not found
+    # Note: users are matched on HTTP or X500 identities and not on the CADC internal identity
+    for ru in users:
+        if not group.user_admins:
+            raise ValueError("Nothing to remove - admins list empty")
+        rm_user = ru.strip().lower()
+        if rm_user.startswith('cn='):
+            id_type = 'X500'
+        else:
+            id_type = 'HTTP'
+        rm_user_found = False
+        for eu in group.user_admins:
+            if (id_type in eu.identities) and (eu.identities[id_type].name.lower() == rm_user):
+                group.user_admins.remove(eu)
+                rm_user_found = True
+                break
+        if not rm_user_found:
+            raise ValueError("User " + rm_user + " not found in the admins list")
+
+
+def _add_admin_groups(group, add_groups):
+    for ag in add_groups:
+        add_group = Group(ag)
+        if add_group not in group.group_admins:
+            group.group_admins.add(add_group)
+        else:
+            raise ValueError("Group " + ag + " already in the admins group")
+
+
+def _remove_admin_groups(group, rm_groups):
+    for rg in rm_groups:
+        rm_group = Group(rg)
+        if rm_group in group.group_admins:
+            group.group_admins.remove(Group(rg))
+        else:
+            raise ValueError("Group " + rg + " not in admins groups")
+
+
 def main_app():
     parser = util.get_base_parser(version=version.version, auth_required=True,
                                   default_resource_id=CADC_AC_SERVICE_ID)
 
     parser.description = (
         'Client for accessing the User Group Management System (GMS) at the '
         'Canadian Astronomy Data Centre')
@@ -444,16 +505,16 @@
     create_parser.epilog = (
         'Examples:\n'
         '        cadc-groups create --cert ~/.ssl/cadcproxy.pem -d "My first '
         'group" -m "cn=abc" foo\n')
 
     members_parser = subparsers.add_parser(
         'members',
-        description='Display, sets or deletes group membership information',
-        help='Display, sets or deletes group membership information')
+        description='Displays, sets or deletes group membership information',
+        help='Displays, sets or deletes group membership information')
     cmd_group = members_parser.add_mutually_exclusive_group()
     cmd_group.add_argument('-clear', '--clear', action='store_true',
                            help='Clear group and user membership')
     cmd_group.add_argument('--remove-group', action='append',
                            help='Remove member group with provided ID')
     cmd_group.add_argument('--add-group', action='append',
                            help='Add member group with provided ID')
@@ -464,14 +525,36 @@
                            help='Add member user with with given CADC username'
                                 ' or distinguished name (DN)')
     members_parser.add_argument('groupid', help='ID of the group')
     members_parser.epilog = (
         'Examples:\n'
         '        cadc-groups members --erase GEMINI foo\n')
 
+    admins_parser = subparsers.add_parser(
+        'admins',
+        description='Displays, sets or deletes group adminstrator information',
+        help='Displays, sets or deletes group adminstrators information')
+    cmd_group = admins_parser.add_mutually_exclusive_group()
+    cmd_group.add_argument('-clear', '--clear', action='store_true',
+                           help='Clear group and user admins')
+    cmd_group.add_argument('--remove-group', action='append',
+                           help='Remove admin group with provided ID')
+    cmd_group.add_argument('--add-group', action='append',
+                           help='Add admin group with provided ID')
+    cmd_group.add_argument('--remove-user', action='append',
+                           help='Remove admin user with CADC username or '
+                                'distinguished name (DN)')
+    cmd_group.add_argument('--add-user', action='append',
+                           help='Add admin user with with given CADC username'
+                                ' or distinguished name (DN)')
+    admins_parser.add_argument('groupid', help='ID of the group')
+    members_parser.epilog = (
+        'Examples:\n'
+        '        cadc-groups admins --erase GEMINI foo\n')
+
     remove_parser = subparsers.add_parser(
         'remove',
         description='Remove a CADC group.',
         help='Remove a CADC group')
     remove_parser.add_argument('groupid', help='ID of the group',
                                nargs='+')
 
@@ -564,14 +647,40 @@
                         identity=Identity(name=ru, identity_type=id_type))
             elif args.remove_group:
                 for rg in args.remove_group:
                     client.remove_group_member(group_id=group.group_id,
                                                member_group_id=rg)
             else:
                 print_group_members(group)
+        elif args.cmd == 'admins':
+            logger.info('admins')
+            group = client.get_group(args.groupid)
+            if args.clear:
+                group.group_admins.clear()
+                group.user_admins.clear()
+                client.update_group(group)
+            elif args.add_user:
+                # Note: admin users need to be added one-by-one in order for the
+                # server to provide the internal CADC ID which is the user primary
+                # key
+                for admin in args.add_user:
+                    _add_admin_user(group, admin)
+                    client.update_group(group)
+            elif args.add_group:
+                _add_admin_groups(group, args.add_group)
+                client.update_group(group)
+            elif args.remove_user:
+                _remove_admin_users(group, args.remove_user)
+                client.update_group(group)
+            elif args.remove_group:
+                _remove_admin_groups(group, args.remove_group)
+                client.update_group(group)
+            else:
+                print_group_admins(group)
+
         elif args.cmd == 'remove':
             logger.info('remove')
             for gi in args.groupid:
                 client.remove_group(group_id=gi)
         else:
             raise RuntimeError('Unknown command option: ' + args.cmd)
     except Exception as ex:
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/netutils.py` & `cadcutils-1.5.1.2/cadcutils/net/netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_auth.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2022.                            (c) 2022.
+#  (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -66,15 +66,15 @@
 # ***********************************************************************
 
 import os
 import sys
 import re
 import unittest
 
-from mock import Mock, patch, mock_open
+from unittest.mock import Mock, patch, mock_open
 from io import StringIO
 
 from cadcutils.net import auth
 from cadcutils.util import get_base_parser
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 TESTDATA_DIR = os.path.join(THIS_DIR, 'data')
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_group.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-# (c) 2021.                            (c) 2021.
+# (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_groups_client.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_groups_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-# (c) 2021.                            (c) 2021.
+# (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -63,19 +63,21 @@
 #                                       <http://www.gnu.org/licenses/>.
 #
 # ***********************************************************************
 
 import sys
 import pytest
 import os
-from mock import Mock, patch, call
+from unittest.mock import Mock, patch, call
 
 from cadcutils.net import Subject, GroupsClient, Group, Identity, Role
 from cadcutils.net.groups_client import main_app
 from cadcutils.net.group_xml import GroupWriter, GroupsWriter
+from cadcutils.net.groups_client import _add_admin_groups, _add_admin_user, \
+    _remove_admin_groups, _remove_admin_users
 
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 TESTDATA_DIR = os.path.join(THIS_DIR, 'data')
 
 
 class MyExitError(Exception):
@@ -432,7 +434,81 @@
     add_user_member_mock.reset_mock()
     sys.argv = 'cadc-groups members --cert cert.pem ' \
                '--remove-user CN=abc,OU=org GrID'.split()
     main_app()
     remove_user_member_mock.assert_called_with(
         group_id=target_grid,
         identity=Identity(name='CN=abc,OU=org', identity_type='X500'))
+
+
+def test_user_admins():
+    target_group = Group('target')
+    _add_admin_user(target_group, 'user1')
+    assert 1 == len(target_group.user_admins)
+    for admin in target_group.user_admins:
+        assert admin.internal_id is None
+        assert admin.identities['HTTP'].name == 'user1'
+    # mimic the server updating the internal_id
+    admin.internal_id = '007'
+    target_group.user_admins.clear()
+    target_group.user_admins.add(admin)
+
+    _add_admin_user(target_group, 'cn=user2')
+    assert 2 == len(target_group.user_admins)
+    for admin in target_group.user_admins:
+        if 'HTTP' in admin.identities:
+            assert admin.internal_id == '007'
+            assert admin.identities['HTTP'].name == 'user1'
+        if 'X500' in admin.identities:
+            assert None is admin.internal_id
+            assert admin.identities['X500'].name == 'cn=user2'
+
+    with pytest.raises(ValueError):
+        _add_admin_user(target_group, 'user1')
+
+    with pytest.raises(ValueError):
+        _add_admin_user(target_group, 'cn=user2')
+
+    with pytest.raises(ValueError):
+        _remove_admin_users(target_group, 'user_not_found')
+
+    _remove_admin_users(target_group, ['user1'])
+    assert 1 == len(target_group.user_admins)
+    for admin in target_group.user_admins:
+        assert admin.internal_id is None
+        assert admin.identities['X500'].name == 'cn=user2'
+
+    _remove_admin_users(target_group, ["cn=user2"])
+    assert 0 == len(target_group.user_admins)
+
+    with pytest.raises(ValueError):
+        _remove_admin_users(target_group, ['cn=user2'])
+
+
+def test_group_admins():
+    target_group = Group('target')
+    _add_admin_groups(target_group, ['group1'])
+    assert 1 == len(target_group.group_admins)
+    for admin in target_group.group_admins:
+        assert 'group1' == admin.group_id
+
+    _add_admin_groups(target_group, ['group2'])
+    assert 2 == len(target_group.group_admins)
+    for admin in target_group.group_admins:
+        assert admin.group_id in ['group1', 'group2']
+
+    with pytest.raises(ValueError):
+        _add_admin_groups(target_group, ['group1'])
+
+    with pytest.raises(ValueError):
+        _remove_admin_groups(target_group, ['group_not_found'])
+
+    _remove_admin_groups(target_group, ['group1'])
+    assert 1 == len(target_group.group_admins)
+    for admin in target_group.group_admins:
+        assert 'group2' == admin.group_id
+
+    _remove_admin_groups(target_group, ['group2'])
+    assert 0 == len(target_group.group_admins)
+
+    with pytest.raises(ValueError):
+        _remove_admin_groups(target_group, ['group2'])
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_int_groups.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_int_groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ************************************************************************
 # *******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # **************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 # *
-# *  (c) 2021.                            (c) 2021.
+# *  (c) 2023.                            (c) 2023.
 # *  Government of Canada                 Gouvernement du Canada
 # *  National Research Council            Conseil national de recherches
 # *  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 # *  All rights reserved                  Tous droits réservés
 # *
 # *  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 # *  expressed, implied, or               énoncée, implicite ou légale,
@@ -64,15 +64,15 @@
 # *
 # ************************************************************************
 
 import pytest
 import os
 import sys
 
-from cadcutils.net import Subject, GroupsClient, Group
+from cadcutils.net import Subject, GroupsClient
 from cadcutils.net.groups_client import main_app
 
 REG_HOST = 'ws.cadc-ccda.hia-iha.nrc-cnrc.gc.ca'
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 TESTDATA_DIR = os.path.join(THIS_DIR, 'data')
 
@@ -148,26 +148,32 @@
     test_group = client.get_group(TEST_GROUP_ID)
 
     assert not test_group.group_members
     assert not test_group.user_members
     assert not test_group.group_admins
     assert not test_group.user_admins
 
-    test_group.group_admins.add(Group(group_id=TEST_MEMBER_GROUP_ID))
-    # TODO currently not supported. Need to retrieve user info first
-    # test_group.user_admins.add(
-    #     User(internal_id=
-    #          'ivo://cadc.nrc.ca/gms?00000000-0000-0000-0000-000000000005'))
+    # test user and group administrators
+    sys.argv = 'cadc-groups admins --cert {} --add-user {} {}'.format(
+        CADC_TESTCERT, TEST_MEMBER_USER_ID, TEST_GROUP_ID).split()
+    main_app()
+
+    sys.argv = 'cadc-groups admins --cert {} --add-group {} {}'.format(
+        CADC_TESTCERT, TEST_MEMBER_GROUP_ID, TEST_GROUP_ID).split()
+    main_app()
 
-    client.update_group(group=test_group)
     test_group = client.get_group(TEST_GROUP_ID)
+
     assert len(test_group.group_admins) == 1
-    # assert len(test_group.user_admins) == 1
+    assert len(test_group.user_admins) == 1
+    assert not test_group.group_members
+    assert not test_group.user_members
 
-    test_group.user_admins.clear()
-    test_group.group_admins.clear()
-    client.update_group(group=test_group)
+    sys.argv = 'cadc-groups admins --cert {} --clear {}'.format(
+        CADC_TESTCERT, TEST_GROUP_ID).split()
+    main_app()
     test_group = client.get_group(TEST_GROUP_ID)
 
     assert not test_group.group_members
     assert not test_group.user_members
     assert not test_group.group_admins
+    assert not test_group.user_admins
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_netutils.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_netutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2022.                            (c) 2022.
+#  (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -62,15 +62,15 @@
 #  <http://www.gnu.org/licenses/>.      pas le cas, consultez :
 #                                       <http://www.gnu.org/licenses/>.
 #
 #
 # ***********************************************************************
 
 import pytest
-from mock import patch, Mock, MagicMock, call
+from unittest.mock import patch, Mock, MagicMock, call
 from requests.utils import CaseInsensitiveDict
 import base64
 
 from cadcutils.net import get_header_filename, extract_md5, Transfer, \
     add_md5_header
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_ws.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # ***********************************************************************
 # ******************  CANADIAN ASTRONOMY DATA CENTRE  *******************
 # *************  CENTRE CANADIEN DE DONNÉES ASTRONOMIQUES  **************
 #
-#  (c) 2022.                            (c) 2022.
+#  (c) 2023.                            (c) 2023.
 #  Government of Canada                 Gouvernement du Canada
 #  National Research Council            Conseil national de recherches
 #  Ottawa, Canada, K1A 0R6              Ottawa, Canada, K1A 0R6
 #  All rights reserved                  Tous droits réservés
 #
 #  NRC disclaims any warranties,        Le CNRC dénie toute garantie
 #  expressed, implied, or               énoncée, implicite ou légale,
@@ -65,15 +65,15 @@
 #
 # ***********************************************************************
 
 import os
 import unittest
 
 import requests
-from mock import Mock, patch, call, ANY
+from unittest.mock import Mock, patch, call, ANY
 from io import StringIO
 from urllib.parse import urlparse
 import tempfile
 import pytest
 import hashlib
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 
@@ -735,15 +735,15 @@
             put_mock.put_num = 0
             client.upload_file(url=target_url, src=src.name,
                                headers=caller_header)
             # check all puts were called
             assert len(put_responses) == put_mock.put_num
 
             # permanent Transfer error
-            session.put = Mock(Mock(headers=start_txn_headers),
+            session.put = Mock(headers=start_txn_headers,
                                side_effect=[exceptions.TransferException] * 3)
             with pytest.raises(exceptions.TransferException):
                 client.upload_file(url=target_url, src=src.name)
 
             # permanent Transfer error including in HEAD
             session.put = Mock(side_effect=[Mock(headers=start_txn_headers),
                                             exceptions.TransferException])
```

### Comparing `cadcutils-1.5.1.1/cadcutils/net/tests/test_wscapabilities.py` & `cadcutils-1.5.1.2/cadcutils/net/tests/test_wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/ws.py` & `cadcutils-1.5.1.2/cadcutils/net/ws.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/net/wscapabilities.py` & `cadcutils-1.5.1.2/cadcutils/net/wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/old_get_cert.py` & `cadcutils-1.5.1.2/cadcutils/old_get_cert.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/util/__init__.py` & `cadcutils-1.5.1.2/cadcutils/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/util/config.py` & `cadcutils-1.5.1.2/cadcutils/util/config.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils/util/utils.py` & `cadcutils-1.5.1.2/cadcutils/util/utils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/cadcutils.egg-info/PKG-INFO` & `cadcutils-1.5.1.2/cadcutils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.1.1
+Version: 1.5.1.2
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.1.1/cadcutils.egg-info/SOURCES.txt` & `cadcutils-1.5.1.2/cadcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.1/setup.cfg` & `cadcutils-1.5.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 long_description = Library of utilities. It includes generic utilities for logging and command line parsing, networking utilities, etc.
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 edit_on_github = False
 github_project = opencadc/cadctools
-version = 1.5.1.1
+version = 1.5.1.2
 
 [options]
 install_requires = 
 	setuptools>=36.0
 	requests>=2.8
 	lxml>=3.7.0
 	html2text
```

### Comparing `cadcutils-1.5.1.1/setup.py` & `cadcutils-1.5.1.2/setup.py`

 * *Files identical despite different names*

