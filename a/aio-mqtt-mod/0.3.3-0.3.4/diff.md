# Comparing `tmp/aio-mqtt-mod-0.3.3.tar.gz` & `tmp/aio-mqtt-mod-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-mqtt-mod-0.3.3.tar", last modified: Wed Feb  1 15:06:21 2023, max compression
+gzip compressed data, was "aio-mqtt-mod-0.3.4.tar", last modified: Fri Jul 28 08:42:49 2023, max compression
```

## Comparing `aio-mqtt-mod-0.3.3.tar` & `aio-mqtt-mod-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-02-01 15:06:21.284428 aio-mqtt-mod-0.3.3/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11350 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/LICENSE
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5710 2023-02-01 15:06:21.284306 aio-mqtt-mod-0.3.3/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4646 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/README.rst
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-02-01 15:06:21.283411 aio-mqtt-mod-0.3.3/aio_mqtt/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      727 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/aio_mqtt/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    28997 2023-02-01 15:01:14.000000 aio-mqtt-mod-0.3.3/aio_mqtt/client.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1769 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/aio_mqtt/constants.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1565 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/aio_mqtt/enums.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1494 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/aio_mqtt/exceptions.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4147 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/aio_mqtt/utils.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      645 2023-02-01 15:04:28.000000 aio-mqtt-mod-0.3.3/aio_mqtt/version.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-02-01 15:06:21.284129 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5710 2023-02-01 15:06:21.000000 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      347 2023-02-01 15:06:21.000000 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-02-01 15:06:21.000000 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-02-01 15:00:57.000000 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/not-zip-safe
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-02-01 15:06:21.000000 aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/top_level.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       38 2023-02-01 15:06:21.284468 aio-mqtt-mod-0.3.3/setup.cfg
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1700 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.3/setup.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-07-28 08:42:49.023836 aio-mqtt-mod-0.3.4/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11350 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/LICENSE
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5710 2023-07-28 08:42:49.023699 aio-mqtt-mod-0.3.4/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4646 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/README.rst
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-07-28 08:42:49.022789 aio-mqtt-mod-0.3.4/aio_mqtt/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      727 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/aio_mqtt/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    29025 2023-07-28 08:36:09.000000 aio-mqtt-mod-0.3.4/aio_mqtt/client.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1769 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/aio_mqtt/constants.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1565 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/aio_mqtt/enums.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1494 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/aio_mqtt/exceptions.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4147 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/aio_mqtt/utils.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      645 2023-07-28 08:39:05.000000 aio-mqtt-mod-0.3.4/aio_mqtt/version.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-07-28 08:42:49.023501 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5710 2023-07-28 08:42:49.000000 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      347 2023-07-28 08:42:49.000000 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-07-28 08:42:49.000000 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-07-28 08:42:48.000000 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/not-zip-safe
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-07-28 08:42:49.000000 aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/top_level.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       38 2023-07-28 08:42:49.023885 aio-mqtt-mod-0.3.4/setup.cfg
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1700 2023-02-01 15:00:20.000000 aio-mqtt-mod-0.3.4/setup.py
```

### Comparing `aio-mqtt-mod-0.3.3/LICENSE` & `aio-mqtt-mod-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/PKG-INFO` & `aio-mqtt-mod-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-mqtt-mod
-Version: 0.3.3
+Version: 0.3.4
 Summary: Asynchronous MQTT client for 3.1.1 protocol version.
 Home-page: https://github.com/devbis/aio-mqtt
 Author: Not Just A Toy Corp.
 Author-email: dev@notjustatoy.com
 License: Apache License 2.0
 Keywords: mqtt asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aio-mqtt-mod-0.3.3/README.rst` & `aio-mqtt-mod-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/__init__.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/client.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 import datetime
 import enum
 import struct
 import sys
 import time
 import typing as ty
 import uuid
-from ssl import SSLContext
 
 from .constants import *
 from .enums import *
 from .exceptions import *
 from .utils import *
 
+if ty.TYPE_CHECKING:
+    from ssl import SSLContext
+
 __all__ = (
     'PublishableMessage',
     'DeliveredMessage',
     'ConnectResult',
     'Client',
 )
 
@@ -170,15 +172,15 @@
         self._consumer_queues: TopicMatcher[ty.Set[aio.Queue[DeliveredMessage]]] = TopicMatcher()
         self._disconnect_reason: ty.Optional[aio.Future] = None
 
     async def connect(
             self,
             host: str,
             port: int = 1883,
-            ssl: ty.Optional[ty.Union[bool, SSLContext]] = None,
+            ssl: ty.Optional[ty.Union[bool, 'SSLContext']] = None,
             keepalive: int = 60,
             client_id: ty.Optional[str] = None,
             clean_session: bool = True,
             will_message: ty.Optional[PublishableMessage] = None,
             username: ty.Optional[str] = None,
             password: ty.Optional[str] = None
     ) -> ConnectResult:
```

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/constants.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/constants.py`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/enums.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/enums.py`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/exceptions.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/utils.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt/version.py` & `aio-mqtt-mod-0.3.4/aio_mqtt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __all__ = (
     '__version__',
 )
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
```

### Comparing `aio-mqtt-mod-0.3.3/aio_mqtt_mod.egg-info/PKG-INFO` & `aio-mqtt-mod-0.3.4/aio_mqtt_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-mqtt-mod
-Version: 0.3.3
+Version: 0.3.4
 Summary: Asynchronous MQTT client for 3.1.1 protocol version.
 Home-page: https://github.com/devbis/aio-mqtt
 Author: Not Just A Toy Corp.
 Author-email: dev@notjustatoy.com
 License: Apache License 2.0
 Keywords: mqtt asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aio-mqtt-mod-0.3.3/setup.py` & `aio-mqtt-mod-0.3.4/setup.py`

 * *Files identical despite different names*

