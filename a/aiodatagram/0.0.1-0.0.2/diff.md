# Comparing `tmp/aiodatagram-0.0.1.tar.gz` & `tmp/aiodatagram-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodatagram-0.0.1.tar", last modified: Fri Dec  9 20:26:49 2022, max compression
+gzip compressed data, was "aiodatagram-0.0.2.tar", last modified: Fri Jul 28 19:46:42 2023, max compression
```

## Comparing `aiodatagram-0.0.1.tar` & `aiodatagram-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2022-12-09 20:26:49.707727 aiodatagram-0.0.1/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2022-12-09 20:26:49.707592 aiodatagram-0.0.1/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2022-12-09 20:20:10.000000 aiodatagram-0.0.1/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2022-12-09 20:26:49.706796 aiodatagram-0.0.1/aiodatagram/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      128 2022-12-09 20:09:07.000000 aiodatagram-0.0.1/aiodatagram/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2385 2022-12-09 20:15:05.000000 aiodatagram-0.0.1/aiodatagram/broadcast.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2198 2022-12-09 20:09:07.000000 aiodatagram-0.0.1/aiodatagram/client.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2458 2022-12-09 20:16:39.000000 aiodatagram-0.0.1/aiodatagram/endpoint.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)       73 2022-12-09 20:24:07.000000 aiodatagram-0.0.1/aiodatagram/types.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2022-12-09 20:26:49.707353 aiodatagram-0.0.1/aiodatagram.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2022-12-09 20:26:49.000000 aiodatagram-0.0.1/aiodatagram.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      284 2022-12-09 20:26:49.000000 aiodatagram-0.0.1/aiodatagram.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2022-12-09 20:26:49.000000 aiodatagram-0.0.1/aiodatagram.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       12 2022-12-09 20:26:49.000000 aiodatagram-0.0.1/aiodatagram.egg-info/top_level.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2022-12-09 20:26:49.707769 aiodatagram-0.0.1/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2022-12-09 20:24:30.000000 aiodatagram-0.0.1/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 19:46:42.678691 aiodatagram-0.0.2/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-07-28 19:46:42.678535 aiodatagram-0.0.2/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      134 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 19:46:42.677786 aiodatagram-0.0.2/aiodatagram/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      128 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/aiodatagram/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2397 2023-07-28 19:45:37.000000 aiodatagram-0.0.2/aiodatagram/broadcast.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2198 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/aiodatagram/client.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2458 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/aiodatagram/endpoint.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       73 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/aiodatagram/types.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-28 19:46:42.678337 aiodatagram-0.0.2/aiodatagram.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-07-28 19:46:42.000000 aiodatagram-0.0.2/aiodatagram.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      284 2023-07-28 19:46:42.000000 aiodatagram-0.0.2/aiodatagram.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-28 19:46:42.000000 aiodatagram-0.0.2/aiodatagram.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       12 2023-07-28 19:46:42.000000 aiodatagram-0.0.2/aiodatagram.egg-info/top_level.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-28 19:46:42.678742 aiodatagram-0.0.2/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      693 2023-07-28 19:40:38.000000 aiodatagram-0.0.2/setup.py
```

### Comparing `aiodatagram-0.0.1/aiodatagram/broadcast.py` & `aiodatagram-0.0.2/aiodatagram/broadcast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Provide high-level UDP broadcast for asyncio"""
 
 from asyncio import (
     DatagramProtocol,
     DatagramTransport,
     get_event_loop,
     wait,
+    create_task,
     sleep,
     FIRST_COMPLETED
 )
 from typing import Union, Text
-from socket import socket, SOL_SOCKET, SO_BROADCAST
+from socket import SOL_SOCKET, SO_BROADCAST
 from .client import DatagramClient
 from .types import Address
 
 class Broadcast(DatagramClient):
     """High-level UDP broadcaster"""
 
     def read_queue(self):
@@ -28,17 +29,17 @@
     async def receive(self, timeout=1.0, count=0):
         """
         Wait for an incoming datagram for time (in seconds) and return it.
         This method is a coroutine.
         """
         if self._queue.empty() and self._closed:
             raise IOError("Enpoint is closed")
-        exit_conditions = [sleep(timeout)]
+        exit_conditions = [create_task(sleep(timeout))]
         if count != 0:
-            exit_conditions.append(self._wait_for_count(count))
+            exit_conditions.append(create_task(self._wait_for_count(count)))
         await wait(exit_conditions, return_when=FIRST_COMPLETED)
         if self._closed:
             raise IOError("Enpoint is closed")
         return self.read_queue()
 
     async def _wait_for_count(self, count: int) -> None:
         while True:
@@ -52,15 +53,15 @@
 
     def __init__(self, broadcast: Broadcast):
         self._broadcast = broadcast
         self._transport = None
 
     def connection_made(self, transport: DatagramTransport):
         self._transport = transport
-        sock = transport.get_extra_info("socket")  # type: socket.socket
+        sock = transport.get_extra_info("socket")
         sock.setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
         self._broadcast._transport = transport
 
     def datagram_received(self, data: Union[bytes, Text], addr: Address):
         self._broadcast.feed_datagram(data, addr)
 
 async def open_broadcast(addr: Address) -> Broadcast:
```

### Comparing `aiodatagram-0.0.1/aiodatagram/client.py` & `aiodatagram-0.0.2/aiodatagram/client.py`

 * *Files identical despite different names*

### Comparing `aiodatagram-0.0.1/aiodatagram/endpoint.py` & `aiodatagram-0.0.2/aiodatagram/endpoint.py`

 * *Files identical despite different names*

### Comparing `aiodatagram-0.0.1/setup.py` & `aiodatagram-0.0.2/setup.py`

 * *Files identical despite different names*

