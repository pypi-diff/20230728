# Comparing `tmp/pih-1.47203.tar.gz` & `tmp/pih-1.47204.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47203.tar", last modified: Fri Jul 28 05:46:11 2023, max compression
+gzip compressed data, was "pih-1.47204.tar", last modified: Fri Jul 28 13:13:36 2023, max compression
```

## Comparing `pih-1.47203.tar` & `pih-1.47204.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 05:46:11.845119 pih-1.47203/
--rw-rw-rw-   0        0        0      261 2023-07-28 05:46:11.845119 pih-1.47203/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 05:46:11.579319 pih-1.47203/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47203/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47203/pih/collection.py
--rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47203/pih/console_api.py
--rw-rw-rw-   0        0        0   110191 2023-07-27 06:39:11.000000 pih-1.47203/pih/const.py
--rw-rw-rw-   0        0        0   309822 2023-07-28 05:45:52.000000 pih-1.47203/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47203/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47203/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47203/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47203/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47203/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47203/pih/service_example.py
--rw-rw-rw-   0        0        0    37996 2023-07-27 14:15:47.000000 pih-1.47203/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47203/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-28 05:46:11.798036 pih-1.47203/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-28 05:46:09.000000 pih-1.47203/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-28 05:46:10.000000 pih-1.47203/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 05:46:09.000000 pih-1.47203/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-28 05:46:10.000000 pih-1.47203/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-28 05:46:10.000000 pih-1.47203/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47203/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 05:46:11.860532 pih-1.47203/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 13:13:34.901660 pih-1.47204/
+drwxrwxrwx   0        0        0        0 2023-07-28 13:13:35.167901 pih-1.47204/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47204/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-1.47204/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-1.47204/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9217 2023-07-28 13:09:01.000000 pih-1.47204/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47204/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      261 2023-07-28 13:13:36.344014 pih-1.47204/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:13:36.060668 pih-1.47204/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47204/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47204/pih/collection.py
+-rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47204/pih/console_api.py
+-rw-rw-rw-   0        0        0   110449 2023-07-28 11:57:21.000000 pih-1.47204/pih/const.py
+-rw-rw-rw-   0        0        0   309983 2023-07-28 13:13:20.000000 pih-1.47204/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47204/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47204/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47204/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47204/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47204/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47204/pih/service_example.py
+-rw-rw-rw-   0        0        0    37996 2023-07-27 14:15:47.000000 pih-1.47204/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47204/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:13:36.297159 pih-1.47204/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-28 13:13:33.000000 pih-1.47204/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:13:33.000000 pih-1.47204/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47204/pih_mio_setup.py
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47204/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:13:36.344014 pih-1.47204/setup.cfg
```

### Comparing `pih-1.47203/pih/collection.py` & `pih-1.47204/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/console_api.py` & `pih-1.47204/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/const.py` & `pih-1.47204/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,20 @@
         PYTHON: str = "py"
         BASE64: str = "base64"
         EXE: str = "exe"
         TRUE_TYPE_FONT: str = "ttf"
 
 class HOSTS:
 
+    class SVSHOST:
+
+        NAME: str = "svshost"
+        ALIAS: str = "zabbix"
+        IP: str = "192.168.100.95"
+
     class BACKUP_WORKER:
     
         NAME: str = "backup_worker"
         ALIAS: str = "backup_worker"
         IP: str = "192.168.100.11"
 
     class WS255:
@@ -1730,14 +1736,16 @@
 
     WS_735: ServiceDescription = ServiceDescription(
         name="ws_735",
         description="ws-735 service",
         host=CONST.HOST.WS735.NAME,
         login="nak",
         password="Soad7623!",
+        pyton_executor_path=r"C:\Users\nak\AppData\Local\Programs\Python\Python310\python.exe",
+        run_from_system_account=True,
         commands=[ServiceCommands.print_image],
         modules=["pywin32", "Pillow"]
     )
 
     RECOGNIZE: ServiceDescription = ServiceDescription(
         name="Recognize",
         description="Recognize service",
```

### Comparing `pih-1.47203/pih/pih.py` & `pih-1.47204/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1595,14 +1595,16 @@
             self.input: Input = input
         if session is None: 
             PIH.session: Session = Session(input, output)
         else:
             self.session: Session = session
         
     class MIO:
+
+        NAME: str = "mio"
     
         ANSWER: dict[str, list[str]] = defaultdict(list)
 
         @staticmethod
         def create_output(recipient: str | Enum, say_hello: bool = True) -> Output:
             from MobileHelperCore.api import MobileOutput, MobileSession, Flags, format_given_name
             recipient = recipient if isinstance(recipient, str) else EnumTool.get(recipient)
@@ -1626,17 +1628,23 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
+        class MIO:
+            
+            @staticmethod
+            def local() -> str:
+                return "1.48012"  
+
         @staticmethod
         def local() -> str:
-            return "1.47203"
+            return "1.47204"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.47203/pih/rpc.py` & `pih-1.47204/pih/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 from pih import A
             else:
                 A = sys.modules["pih.pih"].A
             max_workers = max_workers or RPC.Service.MAX_WORKERS
             service_description: ServiceDescription = role_or_information if isinstance(
                 role_or_information, ServiceInformationBase) else A.CT_SR.description(role_or_information)
             self.description = service_description
-            isolate_arg: str | None = A.SE.arg(1, None)
+            isolate_arg: str | None = A.SE.arg(0, None)
             if A.D.is_not_none(isolate_arg):
                 self.description.isolated = isolate_arg.lower() in [
                     "true", "1", "yes"]
             self.description.pih_version = A.V.local()
             self.description.host = A.SRV.create_host(self.description)
             self.description.port = A.SRV.create_port(self.description)
             self.information = A.D.fill_data_from_source(ServiceInformation(), self.description)
```

### Comparing `pih-1.47203/pih/rpcCommandCall_pb2.py` & `pih-1.47204/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47204/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/rpc_collection.py` & `pih-1.47204/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/rpc_const.py` & `pih-1.47204/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/service_example.py` & `pih-1.47204/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/tools.py` & `pih-1.47204/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih/widgets.py` & `pih-1.47204/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47203/pih_setup.py` & `pih-1.47204/pih_setup.py`

 * *Files identical despite different names*

