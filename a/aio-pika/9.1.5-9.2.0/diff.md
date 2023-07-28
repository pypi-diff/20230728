# Comparing `tmp/aio_pika-9.1.5.tar.gz` & `tmp/aio_pika-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.1.5.tar", max compression
+gzip compressed data, was "aio_pika-9.2.0.tar", max compression
```

## Comparing `aio_pika-9.1.5.tar` & `aio_pika-9.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    15383 2023-07-24 18:31:14.983747 aio_pika-9.1.5/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.5/aio_pika/__init__.py
--rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.5/aio_pika/abc.py
--rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.5/aio_pika/channel.py
--rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.5/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.5/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.5/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.5/aio_pika/log.py
--rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.5/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.5/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.5/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.5/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.5/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.5/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.5/aio_pika/py.typed
--rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.5/aio_pika/queue.py
--rw-r--r--   0        0        0     8275 2023-07-24 18:23:35.142833 aio_pika-9.1.5/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.5/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.5/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.1.5/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.5/aio_pika/tools.py
--rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.5/aio_pika/transaction.py
--rw-r--r--   0        0        0     3269 2023-07-24 18:25:15.528884 aio_pika-9.1.5/pyproject.toml
--rw-r--r--   0        0        0    16986 1970-01-01 00:00:00.000000 aio_pika-9.1.5/PKG-INFO
+-rw-r--r--   0        0        0    15357 2023-07-24 18:32:09.544633 aio_pika-9.2.0/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.2.0/aio_pika/__init__.py
+-rw-r--r--   0        0        0    25283 2023-07-28 10:20:38.626427 aio_pika-9.2.0/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.2.0/aio_pika/channel.py
+-rw-r--r--   0        0        0    11373 2023-07-28 10:20:38.627934 aio_pika-9.2.0/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.2.0/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.2.0/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.2.0/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.2.0/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.2.0/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.2.0/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.2.0/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.2.0/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.2.0/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.2.0/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.2.0/aio_pika/queue.py
+-rw-r--r--   0        0        0     8275 2023-07-24 18:23:35.142833 aio_pika-9.2.0/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10677 2023-07-28 10:20:38.628792 aio_pika-9.2.0/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.2.0/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.2.0/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.2.0/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.2.0/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-07-28 10:25:54.710488 aio_pika-9.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16960 1970-01-01 00:00:00.000000 aio_pika-9.2.0/PKG-INFO
```

### Comparing `aio_pika-9.1.5/README.rst` & `aio_pika-9.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 A wrapper around `aiormq`_ for asyncio and humans.
 
 Check out the examples and the tutorial in the `documentation`_.
 
 If you are a newcomer to RabbitMQ, please start with the `adopted official RabbitMQ tutorial`_.
 
+.. _aiormq: http://github.com/mosquito/aiormq/
+
 .. note::
    Since version ``5.0.0`` this library doesn't use ``pika`` as AMQP connector.
    Versions below ``5.0.0`` contains or requires ``pika``'s source code.
 
 .. note::
    The version 7.0.0 has breaking API changes, see CHANGELOG.md
    for migration hints.
@@ -209,16 +211,16 @@
 
 
 There are more examples and the RabbitMQ tutorial in the `documentation`_.
 
 See also
 ==========
 
-`aiormq <https://github.com/mosquito/aiormq>`_
-----------------------------------------------
+`aiormq`_
+---------
 
 `aiormq` is a pure python AMQP client library. It is under the hood of **aio-pika** and might to be used when you really loving works with the protocol low level.
 Following examples demonstrates the user API.
 
 Simple consumer:
 
 .. code-block:: python
```

### Comparing `aio_pika-9.1.5/aio_pika/__init__.py` & `aio_pika-9.2.0/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/abc.py` & `aio_pika-9.2.0/aio_pika/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
 import dataclasses
 import sys
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from datetime import datetime, timedelta
 from enum import Enum, IntEnum, unique
 from functools import singledispatch
 from types import TracebackType
 from typing import (
     Any, AsyncContextManager, AsyncIterable, Awaitable, Callable, Dict,
-    Generator, Iterator, Optional, Type, TypeVar, Union, overload,
+    Generator, Iterator, Mapping, Optional, Tuple, Type, TypeVar, Union,
+    overload,
 )
 
 
 if sys.version_info >= (3, 8):
     from typing import Literal, TypedDict
 else:
     from typing_extensions import Literal, TypedDict
@@ -688,18 +690,37 @@
             return await self.connection.close(exc)
         except asyncio.CancelledError:
             raise
         finally:
             await self.close_callback.wait()
 
 
+@dataclass
+class ConnectionParameter:
+    name: str
+    parser: Callable[[str], Any]
+    default: Optional[str] = None
+    is_kwarg: bool = False
+
+    def parse(self, value: Optional[str]) -> Any:
+        if value is None:
+            return self.default
+        try:
+            return self.parser(value)
+        except ValueError:
+            return self.default
+
+
 class AbstractConnection(PoolInstance, ABC):
+    PARAMETERS: Tuple[ConnectionParameter, ...]
+
     close_callbacks: CallbackCollection
     connected: asyncio.Event
     transport: Optional[UnderlayConnection]
+    kwargs: Mapping[str, Any]
 
     @abstractmethod
     def __init__(
         self, url: URL, loop: Optional[asyncio.AbstractEventLoop] = None,
         **kwargs: Any,
     ):
         raise NotImplementedError(
@@ -908,14 +929,15 @@
     "AbstractRobustExchange",
     "AbstractRobustQueue",
     "AbstractTransaction",
     "CallbackSetType",
     "CallbackType",
     "ChannelCloseCallback",
     "ConnectionCloseCallback",
+    "ConnectionParameter",
     "ConsumerTag",
     "DateType",
     "DeclarationResult",
     "DeliveryMode",
     "ExchangeParamType",
     "ExchangeType",
     "FieldValue",
```

### Comparing `aio_pika-9.1.5/aio_pika/channel.py` & `aio_pika-9.2.0/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/connection.py` & `aio_pika-9.2.0/aio_pika/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 from ssl import SSLContext
 from types import TracebackType
-from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union
 
 import aiormq.abc
+from aiormq.connection import parse_int
 from pamqp.common import FieldTable
 from yarl import URL
 
 from .abc import (
-    AbstractChannel, AbstractConnection, SSLOptions, TimeoutType,
-    UnderlayConnection,
+    AbstractChannel, AbstractConnection, ConnectionParameter, SSLOptions,
+    TimeoutType, UnderlayConnection,
 )
 from .channel import Channel
 from .exceptions import ConnectionClosed
 from .log import get_logger
 from .tools import CallbackCollection
 
 
@@ -21,15 +22,26 @@
 T = TypeVar("T")
 
 
 class Connection(AbstractConnection):
     """ Connection abstraction """
 
     CHANNEL_CLASS: Type[Channel] = Channel
-    KWARGS_TYPES: Tuple[Tuple[str, Callable[[str], Any], str], ...] = ()
+    PARAMETERS: Tuple[ConnectionParameter, ...] = (
+        ConnectionParameter(
+            name="interleave",
+            parser=parse_int,
+            is_kwarg=True,
+        ),
+        ConnectionParameter(
+            name="happy_eyeballs_delay",
+            parser=float,
+            is_kwarg=True,
+        ),
+    )
 
     _closed: bool
 
     @property
     def is_closed(self) -> bool:
         return self._closed
 
@@ -40,32 +52,38 @@
         self._close_called = True
         if not transport:
             return
         await transport.close(exc)
         self._closed = True
 
     @classmethod
-    def _parse_kwargs(cls, kwargs: Dict[str, Any]) -> Dict[str, Any]:
+    def _parse_parameters(cls, kwargs: Dict[str, Any]) -> Dict[str, Any]:
         result = {}
-        for key, parser, default in cls.KWARGS_TYPES:
-            result[key] = parser(kwargs.get(key, default))
+        for parameter in cls.PARAMETERS:
+            value = kwargs.get(parameter.name, parameter.default)
+
+            if parameter.is_kwarg and value is None:
+                # skip optional value
+                continue
+
+            result[parameter.name] = parameter.parse(value)
         return result
 
     def __init__(
         self, url: URL, loop: Optional[asyncio.AbstractEventLoop] = None,
         ssl_context: Optional[SSLContext] = None, **kwargs: Any,
     ):
         self.loop = loop or asyncio.get_event_loop()
         self.transport = None
         self._closed = False
         self._close_called = False
 
         self.url = URL(url)
 
-        self.kwargs: Dict[str, Any] = self._parse_kwargs(
+        self.kwargs: Dict[str, Any] = self._parse_parameters(
             kwargs or dict(self.url.query),
         )
         self.kwargs["context"] = ssl_context
         self.close_callbacks = CallbackCollection(self)
         self.connected: asyncio.Event = asyncio.Event()
 
     def __str__(self) -> str:
@@ -317,15 +335,15 @@
             }
         )
 
     .. note:
 
         ``client_properties`` argument requires ``aiormq>=2.9``
 
-    URL string might be contain ssl parameters e.g.
+    URL string might be containing ssl parameters e.g.
     `amqps://user:pass@host//?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
 
     :param client_properties: add custom client capability.
     :param url:
         RFC3986_ formatted broker address. When :class:`None`
         will be used keyword arguments.
     :param host: hostname of the broker
@@ -367,8 +385,8 @@
         **kwargs,
     )
 
     await connection.connect(timeout=timeout)
     return connection
 
 
-__all__ = ("connect", "Connection", "make_url")
+__all__ = ("Connection", "connect", "make_url")
```

### Comparing `aio_pika-9.1.5/aio_pika/exceptions.py` & `aio_pika-9.2.0/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/exchange.py` & `aio_pika-9.2.0/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/message.py` & `aio_pika-9.2.0/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/patterns/base.py` & `aio_pika-9.2.0/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/patterns/master.py` & `aio_pika-9.2.0/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/patterns/rpc.py` & `aio_pika-9.2.0/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/pool.py` & `aio_pika-9.2.0/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/queue.py` & `aio_pika-9.2.0/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/robust_channel.py` & `aio_pika-9.2.0/aio_pika/robust_channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/robust_connection.py` & `aio_pika-9.2.0/aio_pika/robust_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 from ssl import SSLContext
-from typing import Any, Optional, Type, Union
+from typing import Any, Optional, Tuple, Type, Union
 from weakref import WeakSet
 
 import aiormq.abc
 from aiormq.connection import parse_bool, parse_timeout
 from pamqp.common import FieldTable
 from yarl import URL
 
 from .abc import (
-    AbstractRobustChannel, AbstractRobustConnection, SSLOptions, TimeoutType,
+    AbstractRobustChannel, AbstractRobustConnection, ConnectionParameter,
+    SSLOptions, TimeoutType,
 )
 from .connection import Connection, make_url
 from .exceptions import CONNECTION_EXCEPTIONS
 from .log import get_logger
 from .robust_channel import RobustChannel
 from .tools import CallbackCollection
 
@@ -22,17 +23,23 @@
 
 
 class RobustConnection(Connection, AbstractRobustConnection):
     """Robust connection"""
 
     CHANNEL_REOPEN_PAUSE = 1
     CHANNEL_CLASS: Type[RobustChannel] = RobustChannel
-    KWARGS_TYPES = (
-        ("reconnect_interval", parse_timeout, "5"),
-        ("fail_fast", parse_bool, "1"),
+    PARAMETERS: Tuple[ConnectionParameter, ...] = Connection.PARAMETERS + (
+        ConnectionParameter(
+            name="reconnect_interval",
+            parser=parse_timeout, default="5",
+        ),
+        ConnectionParameter(
+            name="fail_fast",
+            parser=parse_bool, default="1",
+        ),
     )
 
     def __init__(
         self,
         url: URL,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         **kwargs: Any,
@@ -280,15 +287,15 @@
             }
         )
 
     .. note:
 
         ``client_properties`` argument requires ``aiormq>=2.9``
 
-    URL string might be contain ssl parameters e.g.
+    URL string might contain ssl parameters e.g.
     `amqps://user:pass@host//?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
 
     :param client_properties: add custom client capability.
     :param url:
         RFC3986_ formatted broker address. When :class:`None`
         will be used keyword arguments.
     :param host: hostname of the broker
```

### Comparing `aio_pika-9.1.5/aio_pika/robust_exchange.py` & `aio_pika-9.2.0/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/robust_queue.py` & `aio_pika-9.2.0/aio_pika/robust_queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/tools.py` & `aio_pika-9.2.0/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/aio_pika/transaction.py` & `aio_pika-9.2.0/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.5/pyproject.toml` & `aio_pika-9.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.1.5"
+version = "9.2.0"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
@@ -33,15 +33,15 @@
 [tool.poetry.urls]
 "Source" = "https://github.com/mosquito/aio-pika"
 "Tracker" = "https://github.com/mosquito/aio-pika/issues"
 "Documentation" = "https://aio-pika.readthedocs.org/"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aiormq = "~6.7.5"
+aiormq = "~6.7.7"
 yarl = [{ version = '*'}]
 typing_extensions = [{ version = '*', python = "< 3.8" }]
 # for pkg_resources
 setuptools = [{ version = '*', python = "< 3.8" }]
 
 [tool.poetry.group.dev.dependencies]
 aiomisc = "^17.2"
```

### Comparing `aio_pika-9.1.5/PKG-INFO` & `aio_pika-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.1.5
+Version: 9.2.0
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: aiormq (>=6.7.5,<6.8.0)
+Requires-Dist: aiormq (>=6.7.7,<6.8.0)
 Requires-Dist: setuptools ; python_version < "3.8"
 Requires-Dist: typing_extensions ; python_version < "3.8"
 Requires-Dist: yarl
 Project-URL: Documentation, https://aio-pika.readthedocs.org/
 Project-URL: Source, https://github.com/mosquito/aio-pika
 Project-URL: Tracker, https://github.com/mosquito/aio-pika/issues
 Description-Content-Type: text/x-rst
@@ -71,14 +71,16 @@
 
 A wrapper around `aiormq`_ for asyncio and humans.
 
 Check out the examples and the tutorial in the `documentation`_.
 
 If you are a newcomer to RabbitMQ, please start with the `adopted official RabbitMQ tutorial`_.
 
+.. _aiormq: http://github.com/mosquito/aiormq/
+
 .. note::
    Since version ``5.0.0`` this library doesn't use ``pika`` as AMQP connector.
    Versions below ``5.0.0`` contains or requires ``pika``'s source code.
 
 .. note::
    The version 7.0.0 has breaking API changes, see CHANGELOG.md
    for migration hints.
@@ -247,16 +249,16 @@
 
 
 There are more examples and the RabbitMQ tutorial in the `documentation`_.
 
 See also
 ==========
 
-`aiormq <https://github.com/mosquito/aiormq>`_
-----------------------------------------------
+`aiormq`_
+---------
 
 `aiormq` is a pure python AMQP client library. It is under the hood of **aio-pika** and might to be used when you really loving works with the protocol low level.
 Following examples demonstrates the user API.
 
 Simple consumer:
 
 .. code-block:: python
```

