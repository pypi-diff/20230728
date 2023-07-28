# Comparing `tmp/goecharger-api-lite-1.5.0.tar.gz` & `tmp/goecharger-api-lite-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goecharger-api-lite-1.5.0.tar", last modified: Sun Jul 23 18:40:13 2023, max compression
+gzip compressed data, was "goecharger-api-lite-1.5.1.tar", last modified: Fri Jul 28 20:22:12 2023, max compression
```

## Comparing `goecharger-api-lite-1.5.0.tar` & `goecharger-api-lite-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:40:13.909985 goecharger-api-lite-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-23 18:40:13.909985 goecharger-api-lite-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:40:13.909985 goecharger-api-lite-1.5.0/goecharger_api_lite/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/goecharger_api_lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/goecharger_api_lite/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/goecharger_api_lite/goecharger_api_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:40:13.909985 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-23 18:40:13.000000 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-23 18:40:13.000000 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:40:13.000000 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-23 18:40:13.000000 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-23 18:40:13.000000 goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 18:40:13.909985 goecharger-api-lite-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-23 18:39:56.000000 goecharger-api-lite-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:12.093015 goecharger-api-lite-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-28 20:22:12.093015 goecharger-api-lite-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:12.093015 goecharger-api-lite-1.5.1/goecharger_api_lite/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/goecharger_api_lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/goecharger_api_lite/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/goecharger_api_lite/goecharger_api_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:12.093015 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-28 20:22:12.000000 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 20:22:12.000000 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:22:12.000000 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:22:12.000000 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:22:12.000000 goecharger-api-lite-1.5.1/goecharger_api_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:22:12.093015 goecharger-api-lite-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:00.000000 goecharger-api-lite-1.5.1/setup.py
```

### Comparing `goecharger-api-lite-1.5.0/LICENSE` & `goecharger-api-lite-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goecharger-api-lite-1.5.0/PKG-INFO` & `goecharger-api-lite-1.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: goecharger-api-lite
-Version: 1.5.0
-Summary: Lightweight Python API for accessing go-eCharger EV wallboxes using local HTTP API v2
-Home-page: https://github.com/bkogler/goecharger-api-lite
-Author: Bernhard Kogler
-Author-email: bernhard.kogler@supersonnig.org
-License: MIT
-Keywords: go-e EV wallbox electric charger Gemini flex HOMEfix HOME+ HTTP API v2
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [goecharger API (lite)](https://github.com/bkogler/goecharger-api-lite)
 Lightweight Python API for accessing modern go-eCharger EV wallboxes using local HTTP API v2
 
 [go-eCharger](https://go-e.com) models:
 * Gemini
 * Gemini flex
 * HOMEfix
@@ -98,14 +81,50 @@
 # set to 1 phase, 13 ampere
 charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.one)
 charger.set_ampere(13)
 
 # set to 3 phases, 16 ampere
 charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.three)
 charger.set_ampere(16)
+
+# set phase mode to auto
+charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.auto)
+
+# set maximum possible charge rate of the charger (ampere)
+# this will limit the maximum charge rate that can be set by the user, i.e. via the app
+charger.set_absolute_max_current(10)
+````
+
+### Set cable lock mode
+````python
+from goecharger_api_lite import GoeCharger
+
+charger = GoeCharger("192.168.1.150") # --> change to your IP
+
+# set to require unlocking the car first
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.unlockcarfirst)
+
+# set to automatically unlock after charging
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.automatic)
+
+# set to always lock the cable
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.locked)
+````
+
+### Set charge limit
+````python
+from goecharger_api_lite import GoeCharger
+
+charger = GoeCharger("192.168.1.150") # --> change to your IP
+
+# set charge limit to 2.5 kWh
+charger.set_charge_limit(2500)
+
+# Disable charge limit
+charger.set_charge_limit(None)
 ````
 
 ### Set Generic API Key
 ````python
 from goecharger_api_lite import GoeCharger
 
 charger = GoeCharger("192.168.1.150") # --> change to your IP
```

### Comparing `goecharger-api-lite-1.5.0/goecharger_api_lite/goecharger_api_lite.py` & `goecharger-api-lite-1.5.1/goecharger_api_lite/goecharger_api_lite.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,14 +69,20 @@
 
         __mappings_psm = {
             0: "auto",
             1: "one",
             2: "three"
         }
 
+        __mappings_ust = {
+            0 : "unlock car first",
+            1 : "automatic",
+            2 : "locked"
+        }
+
         __mappings_var = {
             11: "11KW/16A",
             22: "22KW/32A"
         }
 
         def __init__(self, response: Dict[str, Any]):
             self.__response = response
@@ -137,14 +143,17 @@
                 case "amp":
                     return "ampere_allowed", value
 
                 # car state
                 case "car":
                     return "car_state", cls.__mappings_car[value]
 
+                case "dwo":
+                    return "charge_limit", value
+
                 # error code
                 case "err":
                     return "error", cls.__mappings_err[value]
 
                 # forced state
                 case "frc":
                     return "charging_mode", cls.__mappings_frc[value]
@@ -181,14 +190,18 @@
                 case "psm":
                     return "phase_mode", cls.__mappings_psm[value]
 
                 # device temperature
                 case "tma":
                     return "temperature", sum(value)/len(value) if len(value) > 0 else None
 
+                # cable_lock_mode
+                case "ust":
+                    return "cable_lock_mode", cls.__mappings_ust[value]
+
                 # device model (11KW / 22KW)
                 case "var":
                     return "device_model", cls.__mappings_var[value]
 
                 # no mapping specified, return unchanged value
                 case _:
                     return name, value
@@ -202,37 +215,46 @@
         "err",  # error_code
         "frc",  # charging_mode
     )
 
     # default status
     STATUS_DEFAULT = (
         "acu",  # ampere
+        "ama",  # ampere_max_limit
         "car",  # car_state
+        "dwo",  # charge_limit
         "err",  # error_code
         "frc",  # charging_mode
         "nrg",  # energy
         "psm",  # phase_mode
         "tma",  # temperature
+        "ust",  # cable_lock_mode
         "var",  # device_model
     )
 
     class SettableValueEnum:
         """
         Predefined parameters which can be set on GoeCharger device
         """
 
         class ChargingMode(Enum):
             neutral = 0
             off = 1
             on = 2
 
         class PhaseMode(Enum):
+            auto = 0
             one = 1
             three = 2
 
+        class CableLockMode(Enum):
+            unlockcarfirst = 0
+            automatic = 1
+            locked = 2
+
     def __init__(self, host: str, timeout: Optional[float] = 3.0) -> None:
         """
         Initialises GoeCharger connection
 
         :param host: hostname of GoeCharger device
         :param timeout: timeout to wait for a response from device in seconds
         """
@@ -399,14 +421,35 @@
 
     def get_phase_mode(self) -> Dict[str, SettableValueEnum.PhaseMode]:
         """
         Returns phase mode of GoeCharger device (1 phase / 3 phases / neutral)
         """
         return self.__get_status("psm")
 
+    def get_absolute_max_current(self) -> Dict[str, int]:
+        """
+        Returns absolute maximum current setting for the device in Ampere
+        :return:
+        """
+        return self.__get_status("ama")
+
+    def get_cable_lock_mode(self) -> Dict[str, SettableValueEnum.CableLockMode]:
+        """
+        Returns cable lock mode
+        :return:
+        """
+        return self.__get_status("ust")
+
+    def get_charge_limit(self) -> Dict[str, float | None]:
+        """
+        Returns charge limit in Wh or null if disabled
+        :return:
+        """
+        return self.__get_status("dwo")
+
     def set_key(self, key: str, value: Any) -> None:
         """
         Generic (low-level) function for setting a GoeCharger key to a value.
         For possible keys see official API documentation for device
 
         :param key: name of key to set
         :param value: value for key to set
@@ -447,13 +490,66 @@
         :param value: charging_mode to set
         :return:
         """
         self.__set_key("frc", value.value)
 
     def set_phase_mode(self, value: SettableValueEnum.PhaseMode) -> None:
         """
-        Sets phase mode to 1 or 3 phase(s)
+        Sets phase mode to auto, 1 or 3 phase(s)
 
         :param value: phase mode to set
         :return:
         """
         self.__set_key("psm", value.value)
+
+    def set_absolute_max_current(self, value: int | str) -> None:
+        """
+        Sets absolute maximum current setting for the device in Ampere
+
+        :param value: integer value between 0 and ampere_device_maximum (16 / 32)
+        :return:
+        """
+
+        # check data type of parameter
+        if not isinstance(value, int):
+            try:
+                value = int(value)
+            except ValueError:
+                raise GoeChargerError("Ampere value needs to be an integer")
+
+        if not self.__device_model:
+            self.__device_model = self.get_status("var")["device_model"]
+
+        # check for 32A values on 16A devices
+        if self.__device_model.find("11") != -1 and value > 16:
+            raise GoeChargerError(
+                f"Ampere value of '{value}' too big for charger device_model '{self.__device_model}'")
+
+        # set value
+        self.__set_key("ama", value)
+
+    def set_cable_lock_mode(self, value: SettableValueEnum.CableLockMode) -> None:
+        """
+        Sets cable lock mode
+
+        :param value: cable lock mode to set
+        :return:
+        """
+        self.__set_key("ust", value.value)
+
+    def set_charge_limit(self, chargeLimit: float | str | None) -> None:
+        """
+        Sets charge limit in Wh or null to disable charge limit
+
+        :param value: charge limit to set in Wh
+        :return:
+        """
+
+        # check data type of parameter
+        if not isinstance(chargeLimit, float):
+            if chargeLimit is not None:
+                try:
+                    chargeLimit = float(chargeLimit)
+                except ValueError:
+                    raise GoeChargerError("Wh needs to be an integer")
+
+        self.__set_key("dwo", chargeLimit)
```

### Comparing `goecharger-api-lite-1.5.0/goecharger_api_lite.egg-info/PKG-INFO` & `goecharger-api-lite-1.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goecharger-api-lite
-Version: 1.5.0
+Version: 1.5.1
 Summary: Lightweight Python API for accessing go-eCharger EV wallboxes using local HTTP API v2
 Home-page: https://github.com/bkogler/goecharger-api-lite
 Author: Bernhard Kogler
 Author-email: bernhard.kogler@supersonnig.org
 License: MIT
 Keywords: go-e EV wallbox electric charger Gemini flex HOMEfix HOME+ HTTP API v2
 Classifier: Development Status :: 5 - Production/Stable
@@ -98,14 +98,50 @@
 # set to 1 phase, 13 ampere
 charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.one)
 charger.set_ampere(13)
 
 # set to 3 phases, 16 ampere
 charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.three)
 charger.set_ampere(16)
+
+# set phase mode to auto
+charger.set_phase_mode(charger.SettableValueEnum.PhaseMode.auto)
+
+# set maximum possible charge rate of the charger (ampere)
+# this will limit the maximum charge rate that can be set by the user, i.e. via the app
+charger.set_absolute_max_current(10)
+````
+
+### Set cable lock mode
+````python
+from goecharger_api_lite import GoeCharger
+
+charger = GoeCharger("192.168.1.150") # --> change to your IP
+
+# set to require unlocking the car first
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.unlockcarfirst)
+
+# set to automatically unlock after charging
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.automatic)
+
+# set to always lock the cable
+charger.set_cable_lock_mode(charger.SettableValueEnum.CableLockMode.locked)
+````
+
+### Set charge limit
+````python
+from goecharger_api_lite import GoeCharger
+
+charger = GoeCharger("192.168.1.150") # --> change to your IP
+
+# set charge limit to 2.5 kWh
+charger.set_charge_limit(2500)
+
+# Disable charge limit
+charger.set_charge_limit(None)
 ````
 
 ### Set Generic API Key
 ````python
 from goecharger_api_lite import GoeCharger
 
 charger = GoeCharger("192.168.1.150") # --> change to your IP
```

### Comparing `goecharger-api-lite-1.5.0/setup.py` & `goecharger-api-lite-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='goecharger-api-lite',
-    version='1.5.0',
+    version='1.5.1',
     packages=['goecharger_api_lite'],
     url='https://github.com/bkogler/goecharger-api-lite',
     license='MIT',
     author='Bernhard Kogler',
     author_email='bernhard.kogler@supersonnig.org',
     description='Lightweight Python API for accessing go-eCharger EV wallboxes using local HTTP API v2',
     long_description=long_description,
```

