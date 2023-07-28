# Comparing `tmp/alis_build_client-0.0.4.tar.gz` & `tmp/alis_build_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alis_build_client-0.0.4.tar", max compression
+gzip compressed data, was "alis_build_client-0.0.5.tar", max compression
```

## Comparing `alis_build_client-0.0.4.tar` & `alis_build_client-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-07-27 13:10:16.687154 alis_build_client-0.0.4/README.md
--rw-r--r--   0        0        0       75 2023-07-14 08:48:39.896818 alis_build_client-0.0.4/alis/build/client/__init__.py
--rw-r--r--   0        0        0     3025 2023-07-27 12:59:03.151904 alis_build_client-0.0.4/alis/build/client/grpc.py
--rw-r--r--   0        0        0      809 2023-07-27 13:05:18.746804 alis_build_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 alis_build_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      174 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/README.md
+-rw-r--r--   0        0        0       75 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/alis/build/client/__init__.py
+-rw-r--r--   0        0        0     2893 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/alis/build/client/grpc.py
+-rw-r--r--   0        0        0      809 2023-07-28 11:53:20.922167 alis_build_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 alis_build_client-0.0.5/PKG-INFO
```

### Comparing `alis_build_client-0.0.4/alis/build/client/grpc.py` & `alis_build_client-0.0.5/alis/build/client/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import logging
 from google.auth.transport.grpc import AuthMetadataPlugin
 from google.auth.transport.requests import Request
 from google.auth.exceptions import DefaultCredentialsError
 from google.oauth2 import id_token
 
+
 class InvalidArgumentError(Exception):
     def __init__(self, message):
         self.message = message
 
     def __str__(self):
         return f"Argument validation failed: {self.message}"
 
@@ -49,31 +50,26 @@
             self._token_expiry = id_token.verify_oauth2_token(token, request)['exp']
     
     validate_argument("host", host, r"^[a-zA-Z0-9.-]+:\d+$")
 
     if insecure:
         # Create an insecure Channel
         channel = grpc.insecure_channel(host)
-
-        logging.info(f"Established insecure channel to:{host}")
-
     else:
         # Make a secure Channel
         # The following URL will be used as the audience field in the JWT token authentication with the server.
         audience = f"https://{host.split(':')[0]}"
         try:
             # Create an AuthMetadataPlugin instance using the ID token credentials and the request
             auth = GrpcAuth(Request(), audience)
 
             # Create a set of grpc.CallCredentials using the AuthMetadataPlugin instance
             call_creds = grpc.metadata_call_credentials(auth)
 
             # Create a secure Channel using the call credentials
             channel = grpc.secure_channel(host, grpc.composite_channel_credentials(grpc.ssl_channel_credentials(), call_creds))
 
-            logging.info(f"Established secure channel to:{host}")
-
         except DefaultCredentialsError as e:
             logging.exception(f"Failed to fetch identity token credentials: {e}")
             return None
 
     return channel
```

### Comparing `alis_build_client-0.0.4/pyproject.toml` & `alis_build_client-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alis-build-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "A grpc client package for python applications."
 authors = ["Thomas Scholtz <tom.scholtz@alisx.com>"]
 readme = "README.md"
 homepage = "https://github.com/yourusername/grpc_client"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
```

