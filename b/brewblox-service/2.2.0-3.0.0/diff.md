# Comparing `tmp/brewblox_service-2.2.0.tar.gz` & `tmp/brewblox_service-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-2.2.0.tar", max compression
+gzip compressed data, was "brewblox_service-3.0.0.tar", max compression
```

## Comparing `brewblox_service-2.2.0.tar` & `brewblox_service-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/LICENSE.md
--rw-r--r--   0        0        0     3464 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/README.md
--rw-r--r--   0        0        0     1147 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/cors.py
--rw-r--r--   0        0        0     9598 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/http.py
--rw-r--r--   0        0        0    14766 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5294 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5649 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7470 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/service.py
--rw-r--r--   0        0        0     2805 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/brewblox_service/testing.py
--rw-r--r--   0        0        0      664 2023-07-27 15:34:48.033140 brewblox_service-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 brewblox_service-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3551 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/README.md
+-rw-r--r--   0        0        0     1147 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9617 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/http.py
+-rw-r--r--   0        0        0      358 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/models.py
+-rw-r--r--   0        0        0    14606 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5378 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7652 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/service.py
+-rw-r--r--   0        0        0     2805 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/testing.py
+-rw-r--r--   0        0        0      681 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 brewblox_service-3.0.0/PKG-INFO
```

### Comparing `brewblox_service-2.2.0/LICENSE.md` & `brewblox_service-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.2.0/README.md` & `brewblox_service-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Scaffolding for Brewblox service applications
 
 In order to reduce code duplication between services, generic functionality is implemented here.
 
 For an example on how to implement your own service based on `brewblox-service`, see <https://github.com/brewblox/brewblox-boilerplate>.
 
-`brewblox-service` can technically be launched as a standalone application, but will not be very useful.
-
 ## [brewblox_service](./brewblox_service/__init__.py)
 
 Small generic tools are defined here.
 
 `brewblox_logger` can be used for creating module-specific loggers. It is not required, but will play a bit nicer with default formatting of the log.
 
 Example:
@@ -19,22 +17,21 @@
 
 LOGGER = brewblox_logger(__name__)
 LOGGER.info('hello')
 ```
 
 ## [service.py](./brewblox_service/service.py)
 
-Parses commandline arguments, creates an `aiohttp` app, and runs it.
+Parses commandline arguments, creates an `aiohttp` application object, and runs it.
 
 The shortest implementation is:
 
 ```python
 app = service.create_app(default_name='my_service')
-service.furnish(app)
-service.run(app)
+service.run_app(app)
 ```
 
 This will get you a working web application, but it will not have any endpoints.
 
 Applications can configure their own features, and add new commandline arguments.
 
 Example:
@@ -43,44 +40,45 @@
 # Separately creating the parser allows adding arguments to the default set
 parser = service.create_parser(default_name='my_service')
 parser.add_argument('--my-arg')
 
 # Now create the app
 app = service.create_app(parser=create_parser())
 
-# Add features for this service
-device.setup(app)
-api.setup(app)
-
-# Furnish and run
-service.furnish(app)
-service.run(app)
+async def setup():
+    # Add features for this service
+    # You can call async functions here
+    device.setup(app)
+    api.setup(app)
+
+# Run the app. It will await the setup() coroutine
+service.run_app(app, setup())
 ```
 
 ## [features.py](./brewblox_service/features.py)
 
 Many service features are application-scoped. Their lifecycle should span multiple requests, either because they are not request-driven, or because they manage asynchronous I/O operations (such as listening to AMQP messages).
 
 The `ServiceFeature` class offers an abstract base class for this behavior. Implementing classes should define `startup(app)` and `shutdown(app)` functions, and those will be automatically called when the application starts up and shuts down.
 
 Both `startup()` and `shutdown()` are called in an async context, making them the async counterparts of `__init__()` and `__del__()` functions.
 
-Features must be constructed after the app is created, but before it starts running. (`service.create_app()` and `service.run(app)`)
+Features must be constructed after the app is created, but before it starts running. (`service.create_app()` and `service.run_app(app)`).
+It is recommended but not required to add features in an async setup function.
 
 The `add()` and `get()` functions make it easy to centrally declare a feature, and then use it in any function that has a reference to the aiohttp app.
 
-## [mqtt.py](./brewblox_service/mqtt.py)
+## [repeater.py](./brewblox_service/repeater.py)
 
-The replacement for the AMQP-based `events` module.
+A very common use case for features is to have the equivalent of a `while True` loop.
+The `RepeaterFeature` class handles the boilerplate involved in setting this up in an async context.
 
-The major advantages over AMQP is that the protocol is simpler, and supports websocket transport.
-This allows for it to be used outside a Brewblox network.
-
-Messages have a /-separated *topic* and a JSON-serialized body.
+## [mqtt.py](./brewblox_service/mqtt.py)
 
+Basic MQTT messaging: publish and listen to events.
 To publish data, all you need is the `publish(topic, message)` function.
 
 To listen to incoming messages, you can combine `subscribe(topic)` with one or more calls to `listen(topic, callback)`.
 The subscribe/listen functions allow for + and # wildcards to be used.
 
 For a detailed explanation of how to use MQTT topics, see <http://www.steves-internet-guide.com/understanding-mqtt-topics/>.
```

### Comparing `brewblox_service-2.2.0/brewblox_service/__init__.py` & `brewblox_service-3.0.0/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.2.0/brewblox_service/cors.py` & `brewblox_service-3.0.0/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.2.0/brewblox_service/features.py` & `brewblox_service-3.0.0/brewblox_service/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,19 +154,19 @@
                         'Could you come over here?',
                     ]))
 
     Example use:
 
         app = service.create_app(default_name='example')
 
-        scheduler.setup(app)
-        greeter = MyFeature(app)
+        async def setup():
+            scheduler.setup(app)
+            greeter = MyFeature(app)
 
-        service.furnish(app)
-        service.run(app)
+        service.run_app(app, setup())
         # greeter.startup(app) is called now
 
         # Press Ctrl+C to quit
         # greeter.before_shutdown(app) will be called
         # greeter.shutdown(app) will be called
     """
```

### Comparing `brewblox_service-2.2.0/brewblox_service/http.py` & `brewblox_service-3.0.0/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.2.0/brewblox_service/mqtt.py` & `brewblox_service-3.0.0/brewblox_service/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     await mqtt.publish('app', 'brewcast/state/a', json.dumps({'example': True}))
 """
 
 import asyncio
 from contextlib import suppress
 from dataclasses import dataclass, field
 from ssl import CERT_NONE
-from typing import Awaitable, Callable, Literal, Optional
+from typing import Awaitable, Callable, Optional
 
 from aiohttp import web
 from aiomqtt import Client, Message, MqttError, TLSParameters, Will
 from aiomqtt.types import PayloadType
 
-from brewblox_service import brewblox_logger, features, repeater, strex
+from brewblox_service import brewblox_logger, features, models, repeater, strex
 
 LOGGER = brewblox_logger(__name__)
 MQTT_LOGGER = brewblox_logger('aiomqtt')
 
 ListenerCallback_ = Callable[[str, str], Awaitable[None]]
 
 RECONNECT_INTERVAL_S = 2
@@ -78,14 +78,39 @@
         if not self.port:
             self.port = DEFAULT_PORTS[self.protocol]
 
     def __str__(self):
         return f'{self.protocol}://{self.host}:{self.port}{self.path}'
 
 
+def _make_client(config: MQTTConfig) -> Client:
+    secure_protocol = config.protocol in ['mqtts', 'wss']
+    tls_params = None
+    will = None
+
+    if secure_protocol:
+        tls_params = TLSParameters(cert_reqs=CERT_NONE)
+
+    if config.client_will:
+        will = Will(**config.client_will)
+
+    client = Client(hostname=config.host,
+                    port=config.port,
+                    transport=config.transport,
+                    websocket_path=config.path,
+                    tls_params=tls_params,
+                    will=will,
+                    logger=MQTT_LOGGER)
+
+    if secure_protocol:
+        client._client.tls_insecure_set(True)
+
+    return client
+
+
 class EventHandler(repeater.RepeaterFeature):
     """
     Connection handler class for MQTT events.
     Handles both TCP and Websocket connections.
 
     Automatically reconnects and resubscribes when connection is lost.
 
@@ -129,82 +154,56 @@
             Examples: (formatted as <protocol>://<host>:<port><path>)
                 ws://eventbus:15675/eventbus
                 wss://BREWBLOX_HOST:443/eventbus
     """
 
     def __init__(self,
                  app: web.Application,
-                 protocol: Literal['ws', 'wss', 'mqtt', 'mqtts'] = None,
+                 protocol: models.MqttProtocol = None,
                  host: str = None,
                  port: int = None,
                  path: str = None,
                  **kwargs):
         super().__init__(app, **kwargs)
 
-        config = app['config']
-        protocol = protocol or config['mqtt_protocol']
-        host = host or config['mqtt_host']
-        port = port or config['mqtt_port']
-        path = path or config['mqtt_path']
+        config: models.ServiceConfig = app['config']
+        protocol = protocol or config.mqtt_protocol
+        host = host or config.mqtt_host
+        port = port or config.mqtt_port
+        path = path or config.mqtt_path
         self.config = MQTTConfig(protocol, host, port, path)
         self.client: Client = None
 
-        self._ready_ev: asyncio.Event = None
+        self._ready_ev = asyncio.Event()
         self._connect_delay: int = 0
         self._subscribed_topics: list[str] = []
         self._listeners: list[tuple[str, ListenerCallback_]] = []
 
     def __str__(self):
         return f'<{type(self).__name__} for {self.config}>'
 
     @property
-    def ready(self) -> Optional[asyncio.Event]:
+    def ready(self) -> asyncio.Event:
         return self._ready_ev
 
     def set_client_will(self, topic: str, message: PayloadType, **kwargs):
         if self.client:
             raise RuntimeError('Client will must be set before startup')
         self.config.client_will = dict(topic=topic,
                                        payload=message,
                                        **kwargs)
 
-    @staticmethod
-    def create_client(config: MQTTConfig) -> Client:
-        secure_protocol = config.protocol in ['mqtts', 'wss']
-        tls_params = None
-        will = None
-
-        if secure_protocol:
-            tls_params = TLSParameters(cert_reqs=CERT_NONE)
-
-        if config.client_will:
-            will = Will(**config.client_will)
-
-        client = Client(hostname=config.host,
-                        port=config.port,
-                        transport=config.transport,
-                        websocket_path=config.path,
-                        tls_params=tls_params,
-                        will=will,
-                        logger=MQTT_LOGGER)
-
-        if secure_protocol:
-            client._client.tls_insecure_set(True)
-
-        return client
-
     async def _handle_callback(self, cb: ListenerCallback_, message: Message):
         try:
             await cb(str(message.topic), decoded(message.payload))
         except Exception as ex:
             LOGGER.error(f'Exception handling MQTT callback for {message.topic}: {strex(ex)}')
 
     async def startup(self, app: web.Application):
-        self._ready_ev = asyncio.Event()
-        self.client = self.create_client(self.config)
+        self.client = _make_client(self.config)
 
     async def run(self):
         await asyncio.sleep(self._connect_delay)
         self._connect_delay = RECONNECT_INTERVAL_S
 
         try:
             async with self.client:
```

### Comparing `brewblox_service-2.2.0/brewblox_service/repeater.py` & `brewblox_service-3.0.0/brewblox_service/repeater.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 import asyncio
 from abc import abstractmethod
 from typing import Optional
 
 from aiohttp import web
 
-from brewblox_service import brewblox_logger, features, scheduler, strex
+from brewblox_service import (brewblox_logger, features, models, scheduler,
+                              strex)
 
 LOGGER = brewblox_logger(__name__, dedupe=True)
 
 
 class RepeaterCancelled(Exception):
     """
     This can be raised during either setup() or run() to permanently cancel execution.
@@ -64,17 +65,19 @@
     - `run()` [repeated until shutdown]
     - `before_shutdown()`
     - `shutdown()`
     """
 
     def __init__(self, app: web.Application, autostart=True, **kwargs):
         super().__init__(app, **kwargs)
+        config: models.ServiceConfig = app['config']
+
         self._autostart: bool = autostart
         self._task: Optional[asyncio.Task] = None
-        self._debug: bool = app['config']['debug']
+        self._debug: bool = config.debug
 
     async def _startup(self, app: web.Application):
         """
         Overrides the private ServiceFeature startup hook.
         This avoids a gotcha where subclasses have to call `super().startup(app)`
         for RepeaterFeature, but not for ServiceFeature.
         """
```

### Comparing `brewblox_service-2.2.0/brewblox_service/scheduler.py` & `brewblox_service-3.0.0/brewblox_service/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,19 +133,19 @@
 
         async def start(app):
             await scheduler.create(app, current_time(interval=2))
 
 
         app = service.create_app(default_name='example')
 
-        scheduler.setup(app)
-        app.on_startup.append(start)
+        async def setup():
+            scheduler.setup(app)
+            app.on_startup.append(start)
 
-        service.furnish(app)
-        service.run(app)
+        service.run_app(app, setup())
     """
     return await fget(app).create(coro, name=name)
 
 
 async def cancel(app: web.Application,
                  task: asyncio.Task,
                  wait_for: bool = True,
@@ -193,14 +193,14 @@
 
             # Start second task to stop the first
             await scheduler.create(app, stop_after(app, task, duration=10))
 
 
         app = service.create_app(default_name='example')
 
-        scheduler.setup(app)
-        app.on_startup.append(start)
+        async def setup():
+            scheduler.setup(app)
+            app.on_startup.append(start)
 
-        service.furnish(app)
-        service.run(app)
+        service.run_app(app, setup())
     """
     return await fget(app).cancel(task, wait_for=wait_for)
```

### Comparing `brewblox_service-2.2.0/brewblox_service/service.py` & `brewblox_service-3.0.0/brewblox_service/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,39 @@
 This module provides the framework to which service implementations can attach their features.
 
 Example:
     # Uses the default argument parser
     # To add new commandline arguments, use create_parser()
     app = service.create_app(default_name='my_service')
 
-    # (Placeholder names)
-    # All features (endpoints and async handlers) must be created and added to the app here
-    # The Aiohttp Application will freeze functionality once it has been started
-    feature_one.setup(app)
-    feature_two.setup(app)
-
-    # Modify added resources to conform to standards
-    service.furnish(app)
+    async def setup():
+        # (Placeholder names)
+        # All features (endpoints and async handlers) must be created and added to the app here
+        # The Aiohttp Application will freeze functionality once it has been started
+        feature_one.setup(app)
+        feature_two.setup(app)
 
     # Run the application
     # This function blocks until the application is shut down
-    service.run(app)
+    service.run_app(app, setup())
 """
 
 import argparse
 import logging
 # The argumentparser can't fall back to the default sys.argv if sys is not imported
 import sys  # noqa
 import tempfile
-from os import getenv
-from typing import Optional
+from typing import Awaitable, Optional
 
 from aiohttp import web
 from aiohttp_pydantic import oas
 
-from brewblox_service import brewblox_logger, cors, features
+from brewblox_service import brewblox_logger, cors, features, models
 
 LOGGER = brewblox_logger(__name__)
-routes = web.RouteTableDef()
 
 
 def _init_logging(args: argparse.Namespace):
     level = logging.DEBUG if args.debug else logging.INFO
     format = '%(asctime)s %(levelname)-8s %(name)-30s  %(message)s'
     datefmt = '%Y/%m/%d %H:%M:%S'
 
@@ -104,15 +100,16 @@
                        default='brewcast/state')
     return parser
 
 
 def create_app(
         default_name: str = None,
         parser: argparse.ArgumentParser = None,
-        raw_args: Optional[list[str]] = None
+        raw_args: Optional[list[str]] = None,
+        config_cls: type[models.ServiceConfig] = models.ServiceConfig,
 ) -> web.Application:
     """
     Creates and configures an Aiohttp application.
 
     Args:
         default_name (str, optional):
             Default value for the --name commandline argument.
@@ -123,87 +120,88 @@
             Application-specific parser.
             If not provided, the return value of `create_parser()` will be used.
 
         raw_args (list of str, optional):
             Explicit commandline arguments.
             Defaults to sys.argv[1:]
 
+        config_cls (type[models.ServiceConfig], optional):
+            The Pydantic model to load the parsed args.
+            This model should inherit from ServiceConfig.
+
     Returns:
         web.Application: A configured Aiohttp Application object.
-            This Application must be furnished, and is not yet running.
+            This Application is not yet running.
 
     """
 
     if parser is None:
         assert default_name, 'Default service name is required'
         parser = create_parser(default_name)
 
     args, unknown_args = parser.parse_known_args(raw_args)
     _init_logging(args)
 
     if unknown_args:
         LOGGER.error(f'Unknown arguments detected: {unknown_args}')
 
+    config: models.ServiceConfig = config_cls(**vars(args))
     app = web.Application()
-    app['config'] = vars(args)
+    app['config'] = config
 
     app.middlewares.append(cors.cors_middleware)
-    oas.setup(app, url_prefix='/api/doc', title_spec=args.name)
+    oas.setup(app, url_prefix='/api/doc', title_spec=config.name)
 
     return app
 
 
-def furnish(app: web.Application):
-    """
-    Configures Application routes, readying it for running.
-
-    This function modifies routes and resources that were added by calling code,
-    and must be called immediately prior to `run(app)`.
-
-    Args:
-        app (web.Application):
-            The Aiohttp Application as created by `create_app()`
-    """
-    config = app['config']
-    name = config['name']
-    prefix = '/' + name.lstrip('/')
-
-    app.router.add_routes(routes)
-    for resource in app.router.resources():
-        resource.add_prefix(prefix)
-
-    LOGGER.info(f'Service name: {name}')
-    LOGGER.info(f'Service info: {getenv("SERVICE_INFO")}')
-    LOGGER.info(f'Service config: {config}')
-
-    for route in app.router.routes():
-        LOGGER.debug(f'Endpoint [{route.method}] {route.resource.canonical}')
-
-    for name, impl in app.get(features.FEATURES_KEY, {}).items():
-        LOGGER.debug(f'Feature [{name}] {impl}')
-
-
-def run(app: web.Application, listen_http: bool = True):
+def run_app(app: web.Application,
+            setup: Awaitable = None,
+            listen_http: bool = True):
     """
     Runs the application in an async context.
     This function will block indefinitely until the application is shut down.
 
     Args:
         app (web.Application):
             The Aiohttp Application as created by `create_app()`
 
+        setup (Awaitable):
+            If you have setup that should happen async before app start,
+            you can provide an awaitable here.
+            It will be awaited before application startup.
+
         listen_http (bool):
             Whether to open a port for the REST API.
             Set to False to disable all REST endpoints.
             This can be useful for services that use communication protocols
             other than REST (such as MQTT), or only have active functionality.
     """
-    config = app['config']
+    config: models.ServiceConfig = app['config']
+
+    async def _factory() -> web.Application:
+        if setup is not None:
+            await setup
+
+        prefix = '/' + config.name.lstrip('/')
+        for resource in app.router.resources():
+            resource.add_prefix(prefix)
+
+        LOGGER.info(f'Service name: {config.name}')
+        LOGGER.info(f'Service config: {config}')
+
+        for route in app.router.routes():
+            LOGGER.debug(f'Endpoint [{route.method}] {route.resource.canonical}')
+
+        for name, impl in app.get(features.FEATURES_KEY, {}).items():
+            LOGGER.debug(f'Feature [{name}] {impl}')
+
+        return app
 
     if listen_http:
-        web.run_app(app, host=config['host'], port=config['port'])
+        web.run_app(_factory(), host=config.host, port=config.port)
     else:
         # Listen to a dummy UNIX socket
         # The service still runs, but is not bound to any port
         # This is useful for services without a meaningful REST API
         with tempfile.TemporaryDirectory() as tmpdir:
-            web.run_app(app, path=f'{tmpdir}/dummy.sock')
+            web.run_app(_factory(), path=f'{tmpdir}/dummy.sock')
```

### Comparing `brewblox_service-2.2.0/brewblox_service/testing.py` & `brewblox_service-3.0.0/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-2.2.0/PKG-INFO` & `brewblox_service-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 2.2.0
+Version: 3.0.0
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.7)
-Requires-Dist: aiohttp-pydantic (>=1.12)
-Requires-Dist: aiomqtt (>=1.0.0,<2.0.0)
+Requires-Dist: aiohttp (==3.*)
+Requires-Dist: aiohttp-pydantic (==1.*)
+Requires-Dist: aiomqtt (==1.*)
+Requires-Dist: pydantic (==1.*)
 Description-Content-Type: text/markdown
 
 # Scaffolding for Brewblox service applications
 
 In order to reduce code duplication between services, generic functionality is implemented here.
 
 For an example on how to implement your own service based on `brewblox-service`, see <https://github.com/brewblox/brewblox-boilerplate>.
 
-`brewblox-service` can technically be launched as a standalone application, but will not be very useful.
-
 ## [brewblox_service](./brewblox_service/__init__.py)
 
 Small generic tools are defined here.
 
 `brewblox_logger` can be used for creating module-specific loggers. It is not required, but will play a bit nicer with default formatting of the log.
 
 Example:
@@ -37,22 +36,21 @@
 
 LOGGER = brewblox_logger(__name__)
 LOGGER.info('hello')
 ```
 
 ## [service.py](./brewblox_service/service.py)
 
-Parses commandline arguments, creates an `aiohttp` app, and runs it.
+Parses commandline arguments, creates an `aiohttp` application object, and runs it.
 
 The shortest implementation is:
 
 ```python
 app = service.create_app(default_name='my_service')
-service.furnish(app)
-service.run(app)
+service.run_app(app)
 ```
 
 This will get you a working web application, but it will not have any endpoints.
 
 Applications can configure their own features, and add new commandline arguments.
 
 Example:
@@ -61,44 +59,45 @@
 # Separately creating the parser allows adding arguments to the default set
 parser = service.create_parser(default_name='my_service')
 parser.add_argument('--my-arg')
 
 # Now create the app
 app = service.create_app(parser=create_parser())
 
-# Add features for this service
-device.setup(app)
-api.setup(app)
-
-# Furnish and run
-service.furnish(app)
-service.run(app)
+async def setup():
+    # Add features for this service
+    # You can call async functions here
+    device.setup(app)
+    api.setup(app)
+
+# Run the app. It will await the setup() coroutine
+service.run_app(app, setup())
 ```
 
 ## [features.py](./brewblox_service/features.py)
 
 Many service features are application-scoped. Their lifecycle should span multiple requests, either because they are not request-driven, or because they manage asynchronous I/O operations (such as listening to AMQP messages).
 
 The `ServiceFeature` class offers an abstract base class for this behavior. Implementing classes should define `startup(app)` and `shutdown(app)` functions, and those will be automatically called when the application starts up and shuts down.
 
 Both `startup()` and `shutdown()` are called in an async context, making them the async counterparts of `__init__()` and `__del__()` functions.
 
-Features must be constructed after the app is created, but before it starts running. (`service.create_app()` and `service.run(app)`)
+Features must be constructed after the app is created, but before it starts running. (`service.create_app()` and `service.run_app(app)`).
+It is recommended but not required to add features in an async setup function.
 
 The `add()` and `get()` functions make it easy to centrally declare a feature, and then use it in any function that has a reference to the aiohttp app.
 
-## [mqtt.py](./brewblox_service/mqtt.py)
+## [repeater.py](./brewblox_service/repeater.py)
 
-The replacement for the AMQP-based `events` module.
+A very common use case for features is to have the equivalent of a `while True` loop.
+The `RepeaterFeature` class handles the boilerplate involved in setting this up in an async context.
 
-The major advantages over AMQP is that the protocol is simpler, and supports websocket transport.
-This allows for it to be used outside a Brewblox network.
-
-Messages have a /-separated *topic* and a JSON-serialized body.
+## [mqtt.py](./brewblox_service/mqtt.py)
 
+Basic MQTT messaging: publish and listen to events.
 To publish data, all you need is the `publish(topic, message)` function.
 
 To listen to incoming messages, you can combine `subscribe(topic)` with one or more calls to `listen(topic, callback)`.
 The subscribe/listen functions allow for + and # wildcards to be used.
 
 For a detailed explanation of how to use MQTT topics, see <http://www.steves-internet-guide.com/understanding-mqtt-topics/>.
```

