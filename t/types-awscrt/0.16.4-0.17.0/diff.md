# Comparing `tmp/types_awscrt-0.16.4.tar.gz` & `tmp/types_awscrt-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_awscrt-0.16.4.tar", max compression
+gzip compressed data, was "types_awscrt-0.17.0.tar", max compression
```

## Comparing `types_awscrt-0.16.4.tar` & `types_awscrt-0.17.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/LICENSE
--rw-r--r--   0        0        0     1423 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/README.md
--rw-r--r--   0        0        0      289 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/__init__.pyi
--rw-r--r--   0        0        0      438 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/_test.pyi
--rw-r--r--   0        0        0     4673 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/auth.pyi
--rw-r--r--   0        0        0      128 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/checksums.pyi
--rw-r--r--   0        0        0       94 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/common.pyi
--rw-r--r--   0        0        0      594 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/crypto.pyi
--rw-r--r--   0        0        0     1707 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/eventstream/__init__.pyi
--rw-r--r--   0        0        0     3714 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/eventstream/rpc.pyi
--rw-r--r--   0        0        0      234 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/exceptions.pyi
--rw-r--r--   0        0        0     4713 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/http.pyi
--rw-r--r--   0        0        0     4721 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/io.pyi
--rw-r--r--   0        0        0     4090 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/mqtt.pyi
--rw-r--r--   0        0        0    11852 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/mqtt5.pyi
--rw-r--r--   0        0        0        0 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/py.typed
--rw-r--r--   0        0        0     3531 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/s3.pyi
--rw-r--r--   0        0        0     3414 2023-01-14 01:19:20.334530 types_awscrt-0.16.4/awscrt-stubs/websocket.pyi
--rw-r--r--   0        0        0     2411 2023-01-14 01:20:04.250548 types_awscrt-0.16.4/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 types_awscrt-0.16.4/setup.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 types_awscrt-0.16.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/LICENSE
+-rw-r--r--   0        0        0     1407 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/README.md
+-rw-r--r--   0        0        0      289 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/__init__.pyi
+-rw-r--r--   0        0        0      438 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/_test.pyi
+-rw-r--r--   0        0        0     4988 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/auth.pyi
+-rw-r--r--   0        0        0      128 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/checksums.pyi
+-rw-r--r--   0        0        0       94 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/common.pyi
+-rw-r--r--   0        0        0      594 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/crypto.pyi
+-rw-r--r--   0        0        0     1707 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/eventstream/__init__.pyi
+-rw-r--r--   0        0        0     3714 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/eventstream/rpc.pyi
+-rw-r--r--   0        0        0      234 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     4713 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/http.pyi
+-rw-r--r--   0        0        0     4722 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/io.pyi
+-rw-r--r--   0        0        0     4923 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/mqtt.pyi
+-rw-r--r--   0        0        0    11825 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/mqtt5.pyi
+-rw-r--r--   0        0        0        0 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/py.typed
+-rw-r--r--   0        0        0     4012 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/s3.pyi
+-rw-r--r--   0        0        0     3414 2023-07-28 01:14:31.174290 types_awscrt-0.17.0/awscrt-stubs/websocket.pyi
+-rw-r--r--   0        0        0     2551 2023-07-28 01:15:03.662634 types_awscrt-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 types_awscrt-0.17.0/PKG-INFO
```

### Comparing `types_awscrt-0.16.4/LICENSE` & `types_awscrt-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/README.md` & `types_awscrt-0.17.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # types-awscrt
 
 [![PyPI - types-awscrt](https://img.shields.io/pypi/v/types-awscrt.svg?color=blue&label=types-awscrt)](https://pypi.org/project/types-awscrt)
 [![PyPI - awscrt](https://img.shields.io/pypi/v/awscrt.svg?color=blue&label=awscrt)](https://pypi.org/project/awscrt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-awscrt.svg?color=blue)](https://pypi.org/project/types-awscrt)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-awscrt?color=blue)](https://pypistats.org/packages/types-awscrt)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-awscrt)](https://pepy.tech/project/types-awscrt)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations and code completion for [awscrt](https://pypi.org/project/awscrt/) package.
 This package is a part of [mypy_boto3_builder](https://github.com/youtype/mypy_boto3_builder) project.
 
 ## Installation
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/auth.pyi` & `types_awscrt-0.17.0/awscrt-stubs/auth.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -68,14 +68,25 @@
         identity: str,
         tls_ctx: ClientTlsContext,
         logins: Optional[Sequence[Tuple[str, str]]] = ...,
         custom_role_arn: Optional[str] = ...,
         client_bootstrap: Optional[ClientBootstrap] = ...,
         http_proxy_options: Optional[HttpProxyOptions] = ...,
     ) -> _R: ...
+    @classmethod
+    def new_x509(
+        cls: Type[_R],
+        *,
+        endpoint: str,
+        thing_name: str,
+        role_alias: str,
+        tls_ctx: ClientTlsContext,
+        client_bootstrap: Optional[ClientBootstrap] = ...,
+        http_proxy_options: Optional[HttpProxyOptions] = ...,
+    ) -> _R: ...
     def get_credentials(self) -> Future[AwsCredentials]: ...
 
 class AwsSigningAlgorithm(IntEnum):
     V4: int
     V4_ASYMMETRIC: int
 
 class AwsSignatureType(IntEnum):
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/crypto.pyi` & `types_awscrt-0.17.0/awscrt-stubs/crypto.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/awscrt-stubs/eventstream/__init__.pyi` & `types_awscrt-0.17.0/awscrt-stubs/eventstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/awscrt-stubs/eventstream/rpc.pyi` & `types_awscrt-0.17.0/awscrt-stubs/eventstream/rpc.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/awscrt-stubs/http.pyi` & `types_awscrt-0.17.0/awscrt-stubs/http.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/awscrt-stubs/io.pyi` & `types_awscrt-0.17.0/awscrt-stubs/io.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -142,10 +142,11 @@
     def wrap(cls: Type[_R], stream: IO[Any], allow_none: bool = ...) -> _R: ...
 
 class Pkcs11Lib(NativeResource):
     class InitializeFinalizeBehavior(IntEnum):
         DEFAULT: int
         OMIT: int
         STRICT: int
+
     def __init__(
         self, *, file: str, behavior: Optional[InitializeFinalizeBehavior] = ...
     ) -> None: ...
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/mqtt.pyi` & `types_awscrt-0.17.0/awscrt-stubs/mqtt.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from concurrent.futures import Future
+from dataclasses import dataclass
 from enum import IntEnum
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 from awscrt import NativeResource as NativeResource
 from awscrt.exceptions import AwsCrtError
 from awscrt.http import HttpProxyOptions as HttpProxyOptions
 from awscrt.http import HttpRequest as HttpRequest
@@ -26,20 +27,39 @@
 class Will:
     def __init__(self, topic: str, qos: QoS, payload: bytes, retain: bool) -> None:
         self.topic: str
         self.qos: QoS
         self.payload: bytes
         self.retain: bool
 
+@dataclass
+class OnConnectionSuccessData:
+    return_code: Optional[ConnectReturnCode] = ...
+    session_present: bool = ...
+
+@dataclass
+class OnConnectionFailureData:
+    error: Optional[AwsCrtError] = ...
+
+@dataclass
+class OnConnectionClosedData: ...
+
 class Client(NativeResource):
     def __init__(
         self, bootstrap: Optional[ClientBootstrap] = ..., tls_ctx: Optional[ClientTlsContext] = ...
     ) -> None:
         self.tls_ctx: ClientTlsContext
 
+@dataclass
+class OperationStatisticsData:
+    incomplete_operation_count: int = ...
+    incomplete_operation_size: int = ...
+    unacked_operation_count: int = ...
+    unacked_operation_size: int = ...
+
 class Connection(NativeResource):
     def __init__(
         self,
         client: Client,
         host_name: str,
         port: int,
         client_id: str,
@@ -59,14 +79,17 @@
         socket_options: Optional[SocketOptions] = ...,
         use_websockets: bool = ...,
         websocket_proxy_options: Optional[HttpProxyOptions] = ...,
         websocket_handshake_transform: Optional[
             Callable[[WebsocketHandshakeTransformArgs], None]
         ] = ...,
         proxy_options: Optional[HttpProxyOptions] = ...,
+        on_connection_success: Optional[Callable[[Connection], OnConnectionSuccessData]] = ...,
+        on_connection_failure: Optional[Callable[[Connection], OnConnectionFailureData]] = ...,
+        on_connection_closed: Optional[Callable[[Connection], OnConnectionClosedData]] = ...,
     ) -> None:
         self.client: Client
         self.client_id: str
         self.host_name: str
         self.port: int
         self.clean_session: bool
         self.reconnect_min_timeout_secs: int
@@ -90,14 +113,15 @@
     ) -> Tuple[Future[Optional[Dict[str, Any]]], int]: ...
     def on_message(self, callback: Callable[[str, bytes, bool, QoS, bool], None]) -> None: ...
     def unsubscribe(self, topic: str) -> Tuple[Future[Optional[Dict[str, Any]]], int]: ...
     def resubscribe_existing_topics(self) -> Tuple[Future[Optional[Dict[str, Any]]], int]: ...
     def publish(
         self, topic: str, payload: Union[str, bytes, bytearray], qos: QoS, retain: bool = ...
     ) -> Tuple[Future[Optional[Dict[str, Any]]], int]: ...
+    def get_stats(self) -> OperationStatisticsData: ...
 
 class WebsocketHandshakeTransformArgs:
     def __init__(
         self,
         mqtt_connection: Connection,
         http_request: HttpRequest,
         done_future: Future[Optional[BaseException]],
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/mqtt5.pyi` & `types_awscrt-0.17.0/awscrt-stubs/mqtt5.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from collections.abc import Sequence
 from concurrent.futures import Future
 from dataclasses import dataclass
 from enum import IntEnum
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Sequence
 
 from awscrt import NativeResource as NativeResource
 from awscrt import exceptions as exceptions
 from awscrt.http import HttpProxyOptions as HttpProxyOptions
 from awscrt.http import HttpRequest as HttpRequest
 from awscrt.io import ClientBootstrap as ClientBootstrap
 from awscrt.io import ClientTlsContext as ClientTlsContext
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/s3.pyi` & `types_awscrt-0.17.0/awscrt-stubs/s3.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from concurrent.futures import Future
 from enum import IntEnum
 from threading import Event
-from typing import Callable, List, Optional, Tuple
+from typing import Any, Callable, List, Optional, Tuple
 
 from awscrt import NativeResource as NativeResource
 from awscrt.auth import AwsCredentialsProvider as AwsCredentialsProvider
+from awscrt.auth import AwsSigningConfig
 from awscrt.http import HttpRequest as HttpRequest
 from awscrt.io import ClientBootstrap as ClientBootstrap
 from awscrt.io import TlsConnectionOptions as TlsConnectionOptions
 
 class S3RequestType(IntEnum):
     DEFAULT: int
     GET_OBJECT: int
@@ -22,24 +23,26 @@
     shutdown_event: Event
     def __init__(
         self,
         *,
         bootstrap: Optional[ClientBootstrap],
         region: str,
         tls_mode: Optional[S3RequestTlsMode] = ...,
+        signing_config: Optional[AwsSigningConfig] = ...,
         credential_provider: Optional[S3RequestTlsMode] = ...,
         tls_connection_options: Optional[TlsConnectionOptions] = ...,
         part_size: Optional[int] = ...,
         throughput_target_gbps: Optional[float] = ...,
     ) -> None: ...
     def make_request(
         self,
         *,
         request: HttpRequest,
         type: S3RequestType,
+        signing_config: Optional[AwsSigningConfig] = ...,
         credential_provider: Optional[AwsCredentialsProvider] = ...,
         recv_filepath: Optional[str] = ...,
         send_filepath: Optional[str] = ...,
         on_headers: Optional[Callable[[int, List[Tuple[str, str]]], None]] = ...,
         on_body: Optional[Callable[[bytes, int], None]] = ...,
         on_done: Optional[
             Callable[
@@ -53,14 +56,15 @@
     shutdown_event: Event
     def __init__(
         self,
         *,
         client: S3Client,
         request: HttpRequest,
         type: S3RequestType,
+        signing_config: Optional[AwsSigningConfig] = ...,
         credential_provider: Optional[AwsCredentialsProvider] = ...,
         recv_filepath: Optional[str] = ...,
         send_filepath: Optional[str] = ...,
         on_headers: Optional[Callable[[int, List[Tuple[str, str]]], None]] = ...,
         on_body: Optional[Callable[[bytes, int], None]] = ...,
         on_done: Optional[
             Callable[
@@ -75,26 +79,32 @@
     def cancel(self) -> None: ...
 
 class _S3ClientCore:
     def __init__(
         self,
         bootstrap: ClientBootstrap,
         credential_provider: Optional[AwsCredentialsProvider] = ...,
+        signing_config: Optional[AwsSigningConfig] = ...,
         tls_connection_options: Optional[TlsConnectionOptions] = ...,
     ) -> None: ...
 
 class _S3RequestCore:
     def __init__(
         self,
         request: HttpRequest,
         finish_future: Future[Optional[BaseException]],
         shutdown_event: Event,
+        signing_config: Optional[AwsSigningConfig] = ...,
         credential_provider: Optional[AwsCredentialsProvider] = ...,
         on_headers: Optional[Callable[[int, List[Tuple[str, str]]], None]] = ...,
         on_body: Optional[Callable[[bytes, int], None]] = ...,
         on_done: Optional[
             Callable[
                 [Optional[BaseException], Optional[List[Tuple[str, str]]], Optional[bytes]], None
             ]
         ] = ...,
         on_progress: Optional[Callable[[int], None]] = ...,
     ) -> None: ...
+
+def create_default_s3_signing_config(
+    *, region: str, credential_provider: AwsCredentialsProvider, **kwargs: Any
+) -> AwsSigningConfig: ...
```

### Comparing `types_awscrt-0.16.4/awscrt-stubs/websocket.pyi` & `types_awscrt-0.17.0/awscrt-stubs/websocket.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.16.4/pyproject.toml` & `types_awscrt-0.17.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "types-awscrt"
-version = "0.16.4"
+version = "0.17.0"
 description = "Type annotations and code completion for awscrt"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/types-awscrt"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
@@ -58,21 +58,19 @@
 "Bug Tracker" = "https://github.com/youtype/types-awscrt/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 awscrt = "*"
-isort = "*"
-black = "*"
-mypy = "*"
-flake8 = "*"
-twine = "*"
-pyyaml = "*"
-istub = "*"
+isort = { version = "*", python = ">=3.10" }
+black = { version = "*", python = ">=3.10" }
+mypy = { version = "*", python = ">=3.10" }
+flake8 = { version = "*", python = ">=3.10" }
+istub = { version = "*", python = ">=3.10" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = [
```

### Comparing `types_awscrt-0.16.4/PKG-INFO` & `types_awscrt-0.17.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-awscrt
-Version: 0.16.4
+Version: 0.17.0
 Summary: Type annotations and code completion for awscrt
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: awscrt,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,37 +15,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Stubs Only
 Project-URL: Bug Tracker, https://github.com/youtype/types-awscrt/issues
 Project-URL: Documentation, https://youtype.github.io/mypy_boto3_builder/
 Project-URL: Repository, https://github.com/youtype/types-awscrt
 Project-URL: Source, https://github.com/youtype/types-awscrt
 Description-Content-Type: text/markdown
 
 # types-awscrt
 
 [![PyPI - types-awscrt](https://img.shields.io/pypi/v/types-awscrt.svg?color=blue&label=types-awscrt)](https://pypi.org/project/types-awscrt)
 [![PyPI - awscrt](https://img.shields.io/pypi/v/awscrt.svg?color=blue&label=awscrt)](https://pypi.org/project/awscrt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-awscrt.svg?color=blue)](https://pypi.org/project/types-awscrt)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-awscrt?color=blue)](https://pypistats.org/packages/types-awscrt)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-awscrt)](https://pepy.tech/project/types-awscrt)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations and code completion for [awscrt](https://pypi.org/project/awscrt/) package.
 This package is a part of [mypy_boto3_builder](https://github.com/youtype/mypy_boto3_builder) project.
 
 ## Installation
```

