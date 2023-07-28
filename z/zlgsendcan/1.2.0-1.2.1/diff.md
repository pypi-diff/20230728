# Comparing `tmp/zlgsendcan-1.2.0.tar.gz` & `tmp/zlgsendcan-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.2.0.tar", last modified: Thu Jul 27 05:06:45 2023, max compression
+gzip compressed data, was "zlgsendcan-1.2.1.tar", last modified: Fri Jul 28 03:12:49 2023, max compression
```

## Comparing `zlgsendcan-1.2.0.tar` & `zlgsendcan-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.093339 zlgsendcan-1.2.0/
--rw-rw-rw-   0        0        0      221 2023-07-27 05:06:45.092338 zlgsendcan-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 05:06:45.093339 zlgsendcan-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-07-27 05:06:39.000000 zlgsendcan-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.085337 zlgsendcan-1.2.0/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.2.0/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0     2076 2023-07-27 04:16:37.000000 zlgsendcan-1.2.0/zlgsendcan/example_test.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.2.0/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.2.0/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.2.0/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.2.0/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25707 2023-07-27 05:06:39.000000 zlgsendcan-1.2.0/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    19391 2023-07-27 03:26:06.000000 zlgsendcan-1.2.0/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.091340 zlgsendcan-1.2.0/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      221 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-07-27 05:06:45.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.332455 zlgsendcan-1.2.1/
+-rw-rw-rw-   0        0        0      221 2023-07-28 03:12:49.331460 zlgsendcan-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 03:12:49.332455 zlgsendcan-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      438 2023-07-28 03:12:39.000000 zlgsendcan-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.321457 zlgsendcan-1.2.1/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.2.1/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0     2076 2023-07-27 04:16:37.000000 zlgsendcan-1.2.1/zlgsendcan/example_test.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.2.1/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.2.1/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.2.1/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.2.1/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25707 2023-07-27 05:06:39.000000 zlgsendcan-1.2.1/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19479 2023-07-28 03:12:11.000000 zlgsendcan-1.2.1/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:12:49.329458 zlgsendcan-1.2.1/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 03:12:49.000000 zlgsendcan-1.2.1/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.2.0/zlgsendcan/example_test.py` & `zlgsendcan-1.2.1/zlgsendcan/example_test.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.0/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.2.1/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.0/zlgsendcan/parseDBC.py` & `zlgsendcan-1.2.1/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.0/zlgsendcan/yaml_util.py` & `zlgsendcan-1.2.1/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.0/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.2.1/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.2.0/zlgsendcan/zlgserver.py` & `zlgsendcan-1.2.1/zlgsendcan/zlgserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import importlib
 import time
-from PyQt5.QtWidgets import QMessageBox
+# from PyQt5.QtWidgets import QMessageBox
 from zlgsendcan.parseDBC import GlobleValue, DbcInit, get_signal_data1
 from zlgsendcan.zlgcan1 import *
 import threading
 
 
 # 获取dbc文件解析的db对象做成全局变量调用
 def get_dbc_db(dbc_path):
@@ -26,18 +26,19 @@
         GlobleValue.can_conf['can_type'] = can_type
         GlobleValue.can_conf['sjy'] = brate['sjy']
 
         self.zcanlib = ZCAN()
         # self.testcantype = 1  # 0:CAN; 1:canfd
         self.handle = self.zcanlib.OpenDevice(ZCAN_USBCANFD_200U, 0, 0)
         if self.handle == INVALID_DEVICE_HANDLE:
-            msgbox = QMessageBox(QMessageBox.Critical, '错误', "请检查周立功是否连接或重复开启！")
-            msgbox.adjustSize()
-            msgbox.show()
-            msgbox.exec_()
+            # msgbox = QMessageBox(QMessageBox.Critical, '错误', "请检查周立功是否连接或重复开启！")
+            # msgbox.adjustSize()
+            # msgbox.show()
+            # msgbox.exec_()
+            print('"请检查周立功是否连接或重复开启！')
             print("Open CANFD Device failed!")
             # exit(0)
         print("device handle:%d." % (self.handle))
         info = self.zcanlib.GetDeviceInf(self.handle)
         print("Device Information:\n%s" % (info))
 
         # Start CAN
@@ -182,17 +183,17 @@
                             result = my_module.crc_check(pro_name, k, v)
                         else:
                             # ob.crc = True if is_crc == '1' else False
                             # ob.pro_name = pro_name
                             # dbc解析出来的数据
                             result = ob.dbc_parser()
                         if isinstance(result, str):
-                            msgbox = QMessageBox(QMessageBox.Critical, '错误', result)
-                            msgbox.adjustSize()
-                            msgbox.exec_()
+                            # msgbox = QMessageBox(QMessageBox.Critical, '错误', result)
+                            # msgbox.adjustSize()
+                            # msgbox.exec_()
                             return
                         # 数据对象
 
                         data_obj, data_len = canfd_msg(ob, result)
                         msg_th = ThreadStep(data_obj, ctime, sendnum, data_len)
                         msg_th.flag = True
                         th = threading.Thread(target=msg_th.runn, args=[handle],
```

