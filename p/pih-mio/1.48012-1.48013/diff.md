# Comparing `tmp/pih-mio-1.48012.tar.gz` & `tmp/pih-mio-1.48013.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48012.tar", last modified: Fri Jul 28 13:14:07 2023, max compression
+gzip compressed data, was "pih-mio-1.48013.tar", last modified: Fri Jul 28 13:42:14 2023, max compression
```

## Comparing `pih-mio-1.48012.tar` & `pih-mio-1.48013.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:14:06.977972 pih-mio-1.48012/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:14:07.307916 pih-mio-1.48012/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48012/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      236 2023-07-28 13:12:31.000000 pih-mio-1.48012/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48012/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48012/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9217 2023-07-28 13:09:01.000000 pih-mio-1.48012/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48012/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 13:14:07.698558 pih-mio-1.48012/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:14:07.604825 pih-mio-1.48012/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48012/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:14:07.745486 pih-mio-1.48012/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.467316 pih-mio-1.48013/
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.498580 pih-mio-1.48013/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48013/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48013/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48013/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48013/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48013/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48013/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:42:14.967321 pih-mio-1.48013/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:42:14.936080 pih-mio-1.48013/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 13:42:14.000000 pih-mio-1.48013/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 13:42:13.000000 pih-mio-1.48013/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48013/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:42:14.982966 pih-mio-1.48013/setup.cfg
```

### Comparing `pih-mio-1.48012/MobileHelperCore/api.py` & `pih-mio-1.48013/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48012/MobileHelperCore/service.py` & `pih-mio-1.48013/MobileHelperCore/service.py`

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

### Comparing `pih-mio-1.48012/MobileHelperCore/service_api.py` & `pih-mio-1.48013/MobileHelperCore/service_api.py`

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

### Comparing `pih-mio-1.48012/MobileHelperCore/tools.py` & `pih-mio-1.48013/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48012/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48013/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48012/pih_mio_setup.py` & `pih-mio-1.48013/pih_mio_setup.py`

 * *Files identical despite different names*

