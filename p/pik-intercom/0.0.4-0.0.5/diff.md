# Comparing `tmp/pik_intercom-0.0.4.tar.gz` & `tmp/pik_intercom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pik_intercom-0.0.4.tar", last modified: Fri Jul  7 03:59:37 2023, max compression
+gzip compressed data, was "pik_intercom-0.0.5.tar", last modified: Fri Jul 28 08:19:41 2023, max compression
```

## Comparing `pik_intercom-0.0.4.tar` & `pik_intercom-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/pik_intercom/
--rw-r--r--   0 runner    (1001) docker     (123)    30170 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/icm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pik_intercom/iot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/pik_intercom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 03:59:37.000000 pik_intercom-0.0.4/pik_intercom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 03:59:37.109711 pik_intercom-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-07 03:59:27.000000 pik_intercom-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:19:41.899354 pik_intercom-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 08:19:41.899354 pik_intercom-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:19:41.899354 pik_intercom-0.0.5/pik_intercom/
+-rw-r--r--   0 runner    (1001) docker     (123)    30356 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pik_intercom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pik_intercom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pik_intercom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pik_intercom/icm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pik_intercom/iot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:19:41.899354 pik_intercom-0.0.5/pik_intercom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 08:19:41.000000 pik_intercom-0.0.5/pik_intercom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-28 08:19:41.000000 pik_intercom-0.0.5/pik_intercom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:19:41.000000 pik_intercom-0.0.5/pik_intercom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 08:19:41.000000 pik_intercom-0.0.5/pik_intercom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 08:19:41.899354 pik_intercom-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-28 08:19:32.000000 pik_intercom-0.0.5/setup.py
```

### Comparing `pik_intercom-0.0.4/LICENSE` & `pik_intercom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.4/PKG-INFO` & `pik_intercom-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik_intercom
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.4/pik_intercom/__init__.py` & `pik_intercom-0.0.5/pik_intercom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Pik Intercom API"""
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 import json
 import random
 import string
 from typing import (
     TypeVar,
     ClassVar,
@@ -355,15 +355,19 @@
         """
         params = {} if params is None else dict(params)
         page_number = 0
 
         while max_pages is None or (page_number < max_pages):
             page_number += 1
             params["page"] = page_number
-            (resp_data, headers, request_counter,) = await self.make_request(
+            (
+                resp_data,
+                headers,
+                request_counter,
+            ) = await self.make_request(
                 method,
                 url,
                 title=title,
                 params=params,
                 **kwargs,
             )
 
@@ -506,24 +510,32 @@
 
         _LOGGER.debug(f"[{request_counter}] Authentication successful")
 
     async def update_customer_device(self) -> Any:
         if not (device_id := self.device_id):
             raise PikIntercomException("device ID not set")
         try:
-            (resp_data, headers, request_counter,) = await self.make_request(
+            (
+                resp_data,
+                headers,
+                request_counter,
+            ) = await self.make_request(
                 aiohttp.hdrs.METH_GET,
                 f"{self.BASE_ICM_URL}/api/customers/devices/lookup",
                 title="customer device lookup",
                 params={"customer_device[uid]": device_id},
             )
         except aiohttp.ClientResponseError as exc:
             if exc.status != 404:
                 raise
-            (resp_data, headers, request_counter,) = await self.make_request(
+            (
+                resp_data,
+                headers,
+                request_counter,
+            ) = await self.make_request(
                 aiohttp.hdrs.METH_POST,
                 f"{self.BASE_ICM_URL}/api/customers/devices",
                 title="customer device initialization",
                 params={
                     "customer_device[model]": self.device_model,
                     "customer_device[kind]": "mobile",
                     "customer_device[uid]": device_id,
```

### Comparing `pik_intercom-0.0.4/pik_intercom/base.py` & `pik_intercom-0.0.5/pik_intercom/base.py`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.4/pik_intercom/icm.py` & `pik_intercom-0.0.5/pik_intercom/icm.py`

 * *Files identical despite different names*

### Comparing `pik_intercom-0.0.4/pik_intercom/iot.py` & `pik_intercom-0.0.5/pik_intercom/iot.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,18 @@
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         BaseIotCameraWithRTSP.update_from_dict(self, data)
         ObjectWithUnlocker.update_from_dict(self, data)
 
         if property_geo_units := data.get("property_geo_units"):
             units = {}
             for geo_unit_data in property_geo_units:
-                units[geo_unit_data["id"]] = (geo_unit_data["post_name"], geo_unit_data["type"])
+                units[geo_unit_data["id"]] = (
+                    geo_unit_data["post_name"],
+                    geo_unit_data["type"],
+                )
             self.property_geo_units = MappingProxyType(units)
         else:
             self.property_geo_units = None
 
         # Parse geo_unit parameter
         geo_unit_data = data.get("geo_unit") or {}
         self.geo_unit_id = geo_unit_data.get("id") or None
@@ -256,15 +259,18 @@
         relay_settings_data = data.get("user_settings") or {}
         self.custom_name = relay_settings_data.get("custom_name") or None
         self.is_favorite = bool(relay_settings_data.get("is_favorite"))
         self.is_hidden = bool(relay_settings_data.get("is_hidden"))
 
     @property
     def property_geo_unit(self) -> Optional[Tuple[int, str, str]]:
-        for geo_unit_id, (geo_unit_name, geo_unit_type) in self.property_geo_units.items():
+        for geo_unit_id, (
+            geo_unit_name,
+            geo_unit_type,
+        ) in self.property_geo_units.items():
             return geo_unit_id, geo_unit_name, geo_unit_type
 
     @property
     def intercoms(self) -> List["IotIntercom"]:
         """Retrieve list of related intercoms."""
         relay_id = self.id
         return [
@@ -335,15 +341,15 @@
     def update_from_dict(self, data: Mapping[str, Any]) -> None:
         IotCallSession.update_from_dict(self, data)
 
         self.intercom_name = data.get("intercom_name") or None
         self.property_name = data.get("property_name") or None
         self.sip_proxy = data.get("proxy") or None
         self.target_relay_ids = (
-            (
+            tuple(
                 int(relay_data["id"])
                 for relay_data in data["target_relays"]
                 if relay_data
             )
             if data.get("target_relays")
             else ()
         )
```

### Comparing `pik_intercom-0.0.4/pik_intercom.egg-info/PKG-INFO` & `pik_intercom-0.0.5/pik_intercom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pik-intercom
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pik Intercom API for Python
 Home-page: https://github.com/alryaz/pik-intercom-python
 Author: Alexander Ryazanov
 Author-email: alryaz@alryaz.com
 Project-URL: Documentation, https://github.com/alryaz/pik-intercom-python
 Project-URL: Bug Reports, https://github.com/alryaz/pik-intercom-python/issues
 Project-URL: Source Code, https://github.com/alryaz/pik-intercom-python
```

### Comparing `pik_intercom-0.0.4/setup.py` & `pik_intercom-0.0.5/setup.py`

 * *Files identical despite different names*

