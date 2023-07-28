# Comparing `tmp/pyhyypapihawkmod-1.2.0b1.tar.gz` & `tmp/pyhyypapihawkmod-1.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.2.0b1.tar", last modified: Fri Jul 28 13:52:50 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.2.0b2.tar", last modified: Fri Jul 28 17:50:47 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.2.0b1.tar` & `pyhyypapihawkmod-1.2.0b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:52:50.004219 pyhyypapihawkmod-1.2.0b1/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-28 13:52:50.003207 pyhyypapihawkmod-1.2.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2317 2023-07-28 13:52:00.000000 pyhyypapihawkmod-1.2.0b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 13:52:49.987983 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-07-28 13:50:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    11035 2023-07-28 13:50:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29480 2023-07-28 13:50:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4026 2023-07-28 13:50:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-07-28 13:50:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:52:50.000171 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-28 13:52:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-28 13:52:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:52:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-28 13:52:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 13:52:49.000000 pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 13:52:50.004219 pyhyypapihawkmod-1.2.0b1/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-28 13:52:03.000000 pyhyypapihawkmod-1.2.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.713806 pyhyypapihawkmod-1.2.0b2/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-28 17:50:47.712798 pyhyypapihawkmod-1.2.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2415 2023-07-28 17:49:31.000000 pyhyypapihawkmod-1.2.0b2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.697681 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    11363 2023-07-28 17:47:18.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29480 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4026 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.711310 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:50:47.714311 pyhyypapihawkmod-1.2.0b2/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-28 17:11:42.000000 pyhyypapihawkmod-1.2.0b2/setup.py
```

### Comparing `pyhyypapihawkmod-1.2.0b1/LICENSE.md` & `pyhyypapihawkmod-1.2.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/PKG-INFO` & `pyhyypapihawkmod-1.2.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b1
+Version: 1.2.0b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b1/README.md` & `pyhyypapihawkmod-1.2.0b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.2.0b2
+- Added additional checks for openviolated and tampered information when not received
+
 1.2.0b1
 - Version bump for semantic versioning 
 
 1.1.7b3
 - Revert 1.1.7b2
 
 1.1.7b2
```

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/alarm_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
-SLEEP_DELAY = 0.5
+SLEEP_DELAY = 0.6
 
 class HyypAlarmInfos:
     """Initialize Hyyp alarm objects."""
 
     def __init__(self, client: HyypClient) -> None:
         """init."""
         self._client = client
@@ -39,22 +39,27 @@
             time.sleep(SLEEP_DELAY)
             entry = {siteid : self._client.get_zone_state_info(site_id=siteid)}
             self._zone_state_info.append(entry)
 
             
         
     def get_zone_state_info_for_site(self, site):
-        current_siteinfo = {}
+        current_siteinfo = None
         for siteinfo in self._zone_state_info:
-            if site not in siteinfo:
-                continue
-            current_siteinfo = siteinfo[site]
+            if site in siteinfo:
+                current_siteinfo = siteinfo[site]
+                if "status" not in current_siteinfo:
+                    return None
+                if current_siteinfo["status"] != "SUCCESS":
+                    return None
         return current_siteinfo
+    
             
 
+
         
     def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
         """Fetch and cache site notifications."""
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
@@ -143,15 +148,14 @@
         
         for site in site_ids:
             
             self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
             zone_states = self.get_zone_state_info_for_site(site=site)
 
-
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["update"] = str(datetime.fromtimestamp(time.time()))
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
@@ -189,14 +193,18 @@
                         "bypassed"
                     ] = bool(zone in self._state_info["bypassedZoneIds"])
 
 
 
                 # New zone information from IDS servers
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
+                    if zone_states is None:
+                        continue
+                    if "zones" not in zone_states:
+                        continue
                     for zone_state in zone_states["zones"]:
                         if site_ids[site]["partitions"][partition]["zones"][zone][
                             "number"] != zone_state["number"]:
                             continue
                         site_ids[site]["partitions"][partition]["zones"][zone][
                             "bypassed"] = bool(zone_state["bypassed"])
                         site_ids[site]["partitions"][partition]["zones"][zone][
```

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b1
+Version: 1.2.0b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b1/setup.py` & `pyhyypapihawkmod-1.2.0b2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.2.0b1",
+    version="1.2.0b2",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

