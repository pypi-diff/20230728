# Comparing `tmp/pih-1.47204.tar.gz` & `tmp/pih-1.47205.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47204.tar", last modified: Fri Jul 28 13:13:36 2023, max compression
+gzip compressed data, was "pih-1.47205.tar", last modified: Fri Jul 28 13:42:35 2023, max compression
```

## Comparing `pih-1.47204.tar` & `pih-1.47205.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:13:34.901660 pih-1.47204/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:13:35.167901 pih-1.47204/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47204/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-1.47204/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-1.47204/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9217 2023-07-28 13:09:01.000000 pih-1.47204/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47204/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      261 2023-07-28 13:13:36.344014 pih-1.47204/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:13:36.060668 pih-1.47204/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47204/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47204/pih/collection.py
--rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47204/pih/console_api.py
--rw-rw-rw-   0        0        0   110449 2023-07-28 11:57:21.000000 pih-1.47204/pih/const.py
--rw-rw-rw-   0        0        0   309983 2023-07-28 13:13:20.000000 pih-1.47204/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47204/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47204/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47204/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47204/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47204/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47204/pih/service_example.py
--rw-rw-rw-   0        0        0    37996 2023-07-27 14:15:47.000000 pih-1.47204/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47204/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:13:36.297159 pih-1.47204/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-28 13:13:33.000000 pih-1.47204/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:13:33.000000 pih-1.47204/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-28 13:13:34.000000 pih-1.47204/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47204/pih_mio_setup.py
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47204/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:13:36.344014 pih-1.47204/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:34.173255 pih-1.47205/
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:34.471645 pih-1.47205/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47205/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-1.47205/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47205/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47205/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47205/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      261 2023-07-28 13:42:35.440373 pih-1.47205/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:35.206009 pih-1.47205/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47205/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47205/pih/collection.py
+-rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47205/pih/console_api.py
+-rw-rw-rw-   0        0        0   110449 2023-07-28 11:57:21.000000 pih-1.47205/pih/const.py
+-rw-rw-rw-   0        0        0   310256 2023-07-28 13:42:05.000000 pih-1.47205/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47205/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47205/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47205/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47205/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47205/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47205/pih/service_example.py
+-rw-rw-rw-   0        0        0    37996 2023-07-27 14:15:47.000000 pih-1.47205/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47205/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:35.409126 pih-1.47205/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47205/pih_mio_setup.py
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47205/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:42:35.518507 pih-1.47205/setup.cfg
```

### Comparing `pih-1.47204/MobileHelperCore/api.py` & `pih-1.47205/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/MobileHelperCore/service.py` & `pih-1.47205/MobileHelperCore/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 import importlib.util
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import A
 
-from MobileHelperCore.service_api import MobileHelperService as Service
+from MobileHelperCore.service_api import MobileHelperService as Service, as_developer
 
 host: str = A.OS.host()
 
-def as_developer() -> bool:
-    return A.SE.arg(1, "").lower() == "true"
-
 def checker(telephone_number: str) -> bool:
     if not A.D_C.empty(A.SRV.get_support_host_list(A.CT_SR.MOBILE_HELPER)):
         am_i_tester: bool = A.D.is_not_none(A.CT.TEST.USER) and A.D_TN.by_login(A.CT.TEST.USER) == telephone_number
         if as_developer() or A.D.contains(host, A.CT_H.DEVELOPER.NAME):
             return am_i_tester
         return not am_i_tester
     return True
```

### Comparing `pih-1.47204/MobileHelperCore/service_api.py` & `pih-1.47205/MobileHelperCore/service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 SR = A.CT_SR
 SC = A.CT_SC
 
 ROLE: SR = SR.MOBILE_HELPER
 
 #version 0.8
 
+def as_developer() -> bool:
+    return A.SE.arg(1, "").lower() == "true"
+
 class MobileHelperService():
 
     INIT: bool = False
     INSTANCE: Any | None = None
     NAME: str = "MobileHelper"
    
     sender_profile_id: A.CT_ME_WH_W.PROFILE = A.ME_WH_W.get_profile_id(A.D_TN.it_administrator())
@@ -44,16 +47,17 @@
         self.allow_send_to_next_service_in_chain: dict[str, bool] = defaultdict(bool)
         MobileHelperService.INSTANCE = self  
            
     def start(self) -> bool:
         if MobileHelperService.INIT:
             service_role_desctiption: self.ServiceRoleDescription | None = A.SRV_A.create_support_service_or_master_service_description(A.CT_SR.description(self.service_role))
             if not A.D_C.empty(service_role_desctiption):
-                A.SRV_A.serve(service_role_desctiption, self.service_call_handler,
-                            MobileHelperService.service_starts_handler)
+                with A.ER.detect_interruption("Выход"):
+                    A.SRV_A.serve(service_role_desctiption, self.service_call_handler,
+                                MobileHelperService.service_starts_handler)
                 return True
         return False
 
     def create_mobile_helper(self, telephone_number: str, flags: int | None = None, recipient: str | None = None) -> Api:
         stdin: self.Stdin = self.Stdin()
         session: self.MobileSession = self.MobileSession(telephone_number, flags)
         output: self.MobileOutput = self.MobileOutput(session)
@@ -159,8 +163,10 @@
         if sc == A.CT_SC.send_mobile_helper_message:
             self.receive_message_handler(
                 " ".join((self.root, parameter_list.next())), parameter_list.next(), parameter_list.next())
         return None
 
     @staticmethod
     def service_starts_handler() -> None:
+        if as_developer():
+            A.O.blue("For developer")
         A.SRV_A.subscribe_on(A.CT_SC.send_event, A.CT_SubT.ON_RESULT_SEQUENTIALLY, MobileHelperService.NAME)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pih-1.47204/MobileHelperCore/tools.py` & `pih-1.47205/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/collection.py` & `pih-1.47205/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/console_api.py` & `pih-1.47205/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/const.py` & `pih-1.47205/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/pih.py` & `pih-1.47205/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1632,19 +1632,19 @@
 
     class VERSION:
 
         class MIO:
             
             @staticmethod
             def local() -> str:
-                return "1.48012"  
+                return "1.48013"  
 
         @staticmethod
         def local() -> str:
-            return "1.47204"
+            return "1.47205"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1684,14 +1684,21 @@
 
         @contextmanager
         def detect() -> bool:
             try:
                 yield True
             except Exception as error:
                 PIH.ERROR.global_except_hook(type(error), error, error.__traceback__)
+
+        @contextmanager
+        def detect_interruption(message: str | None = None) -> bool:
+            try:
+                yield True
+            except KeyboardInterrupt as error:
+               if_else(DataTool.is_none(message), None, PIH.output.red(message))
         
         @staticmethod
         def rpc_error_handler(details: str, code: tuple, description: ServiceRoles, command: ServiceCommands) -> None:
             if isinstance(command, ServiceCommands):
                 if code == StatusCode.UNAVAILABLE:
                     if PIH.ERROR.notify_about_error:
                         PIH.output.error(f"Error: {details}")
```

### Comparing `pih-1.47204/pih/rpc.py` & `pih-1.47205/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/rpcCommandCall_pb2.py` & `pih-1.47205/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47205/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/rpc_collection.py` & `pih-1.47205/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/rpc_const.py` & `pih-1.47205/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/service_example.py` & `pih-1.47205/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/tools.py` & `pih-1.47205/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih/widgets.py` & `pih-1.47205/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih.egg-info/SOURCES.txt` & `pih-1.47205/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih_mio_setup.py` & `pih-1.47205/pih_mio_setup.py`

 * *Files identical despite different names*

### Comparing `pih-1.47204/pih_setup.py` & `pih-1.47205/pih_setup.py`

 * *Files identical despite different names*

