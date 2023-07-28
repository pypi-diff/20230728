# Comparing `tmp/uni-sdk-0.2.0.tar.gz` & `tmp/uni-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uni-sdk-0.2.0.tar", last modified: Sat Dec 17 04:46:14 2022, max compression
+gzip compressed data, was "uni-sdk-0.3.0.tar", last modified: Fri Jul 28 10:26:54 2023, max compression
```

## Comparing `uni-sdk-0.2.0.tar` & `uni-sdk-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 acathur    (501) staff       (20)        0 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/
--rw-r--r--   0 acathur    (501) staff       (20)     3655 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 acathur    (501) staff       (20)     1066 2022-12-14 14:59:06.000000 uni-sdk-0.2.0/LICENSE
--rw-r--r--   0 acathur    (501) staff       (20)       26 2021-05-24 10:59:16.000000 uni-sdk-0.2.0/MANIFEST.in
--rw-r--r--   0 acathur    (501) staff       (20)     2262 2022-12-16 10:36:33.000000 uni-sdk-0.2.0/README.md
--rw-r--r--   0 acathur    (501) staff       (20)     2926 2022-12-16 17:57:35.000000 uni-sdk-0.2.0/setup.py
-drwxr-xr-x   0 acathur    (501) staff       (20)        0 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni/
--rw-r--r--   0 acathur    (501) staff       (20)      243 2022-12-16 09:29:42.000000 uni-sdk-0.2.0/uni/exception.py
--rw-r--r--   0 acathur    (501) staff       (20)     1998 2022-12-17 04:44:01.000000 uni-sdk-0.2.0/uni/client.py
--rw-r--r--   0 acathur    (501) staff       (20)       93 2022-12-16 09:55:02.000000 uni-sdk-0.2.0/uni/__init__.py
--rw-r--r--   0 acathur    (501) staff       (20)      769 2022-12-16 09:29:43.000000 uni-sdk-0.2.0/uni/response.py
--rw-r--r--   0 acathur    (501) staff       (20)       63 2022-12-16 09:24:03.000000 uni-sdk-0.2.0/uni/__version__.py
-drwxr-xr-x   0 acathur    (501) staff       (20)        0 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni/services/
--rw-r--r--   0 acathur    (501) staff       (20)       37 2022-12-16 09:42:41.000000 uni-sdk-0.2.0/uni/services/__init__.py
--rw-r--r--   0 acathur    (501) staff       (20)      172 2022-12-16 10:15:09.000000 uni-sdk-0.2.0/uni/services/messages.py
--rw-r--r--   0 acathur    (501) staff       (20)       38 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/setup.cfg
-drwxr-xr-x   0 acathur    (501) staff       (20)        0 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni_sdk.egg-info/
--rw-r--r--   0 acathur    (501) staff       (20)     3655 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni_sdk.egg-info/PKG-INFO
--rw-r--r--   0 acathur    (501) staff       (20)      294 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 acathur    (501) staff       (20)        4 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni_sdk.egg-info/top_level.txt
--rw-r--r--   0 acathur    (501) staff       (20)        1 2022-12-17 04:46:14.000000 uni-sdk-0.2.0/uni_sdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 acathur    (501) staff       (20)        0 2023-07-28 10:26:54.403378 uni-sdk-0.3.0/
+-rw-r--r--   0 acathur    (501) staff       (20)     1066 2022-12-14 14:59:06.000000 uni-sdk-0.3.0/LICENSE
+-rw-r--r--   0 acathur    (501) staff       (20)       26 2021-05-24 10:59:16.000000 uni-sdk-0.3.0/MANIFEST.in
+-rw-r--r--   0 acathur    (501) staff       (20)     4268 2023-07-28 10:26:54.402763 uni-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 acathur    (501) staff       (20)     3401 2023-07-27 13:17:57.000000 uni-sdk-0.3.0/README.md
+-rw-r--r--   0 acathur    (501) staff       (20)       38 2023-07-28 10:26:54.403540 uni-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 acathur    (501) staff       (20)     2943 2023-07-28 10:24:59.000000 uni-sdk-0.3.0/setup.py
+drwxr-xr-x   0 acathur    (501) staff       (20)        0 2023-07-28 10:26:54.395970 uni-sdk-0.3.0/uni/
+-rw-r--r--   0 acathur    (501) staff       (20)       93 2022-12-16 09:55:02.000000 uni-sdk-0.3.0/uni/__init__.py
+-rw-r--r--   0 acathur    (501) staff       (20)       63 2023-07-27 12:54:59.000000 uni-sdk-0.3.0/uni/__version__.py
+-rw-r--r--   0 acathur    (501) staff       (20)     2182 2023-07-27 13:02:53.000000 uni-sdk-0.3.0/uni/client.py
+-rw-r--r--   0 acathur    (501) staff       (20)      243 2022-12-16 09:29:42.000000 uni-sdk-0.3.0/uni/exception.py
+-rw-r--r--   0 acathur    (501) staff       (20)      794 2023-07-27 13:07:36.000000 uni-sdk-0.3.0/uni/response.py
+drwxr-xr-x   0 acathur    (501) staff       (20)        0 2023-07-28 10:26:54.398964 uni-sdk-0.3.0/uni/services/
+-rw-r--r--   0 acathur    (501) staff       (20)       65 2023-07-27 12:55:56.000000 uni-sdk-0.3.0/uni/services/__init__.py
+-rw-r--r--   0 acathur    (501) staff       (20)      172 2022-12-17 13:50:18.000000 uni-sdk-0.3.0/uni/services/messages.py
+-rw-r--r--   0 acathur    (501) staff       (20)      311 2023-07-27 13:08:45.000000 uni-sdk-0.3.0/uni/services/otp.py
+drwxr-xr-x   0 acathur    (501) staff       (20)        0 2023-07-28 10:26:54.402028 uni-sdk-0.3.0/uni_sdk.egg-info/
+-rw-r--r--   0 acathur    (501) staff       (20)     4268 2023-07-28 10:26:54.000000 uni-sdk-0.3.0/uni_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 acathur    (501) staff       (20)      314 2023-07-28 10:26:54.000000 uni-sdk-0.3.0/uni_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 acathur    (501) staff       (20)        1 2023-07-28 10:26:54.000000 uni-sdk-0.3.0/uni_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 acathur    (501) staff       (20)        4 2023-07-28 10:26:54.000000 uni-sdk-0.3.0/uni_sdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `uni-sdk-0.2.0/PKG-INFO` & `uni-sdk-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,118 @@
-Metadata-Version: 2.1
-Name: uni-sdk
-Version: 0.2.0
-Summary: The official Unimatrix SDK for Python.
-Home-page: https://github.com/unimtx/uni-python-sdk
-Author: Unimatrix
-Author-email: dev@unimtx.com
-License: MIT
-Project-URL: Documentation, https://www.unimtx.com/docs
-Project-URL: Homepage, https://unimtx.com
-Project-URL: Repository, https://github.com/unimtx/uni-python-sdk
-Description: 
-        # Unimatrix Python SDK
-        
-        [![PyPI](https://img.shields.io/pypi/v/uni-sdk.svg)](https://pypi.python.org/pypi/uni-sdk) [![Release](https://img.shields.io/github/release/unimtx/uni-python-sdk.svg)](https://github.com/unimtx/uni-python-sdk/releases/latest) [![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/unimtx/uni-python-sdk/blob/main/LICENSE)
-        
-        The Unimatrix Python SDK provides convenient access to integrate communication capabilities into your Python applications using the Unimatrix HTTP API. The SDK provides support for sending SMS, 2FA verification, and phone number lookup.
-        
-        ## Getting started
-        
-        Before you begin, you need an [Unimatrix](https://www.unimtx.com/) account. If you don't have one yet, you can [sign up](https://www.unimtx.com/signup?s=python.sdk.gh) for an Unimatrix account and get free credits to get you started.
-        
-        ## Documentation
-        
-        Check out the documentation at [unimtx.com/docs](https://www.unimtx.com/docs) for a quick overview.
-        
-        ## Installation
-        
-        Using pip is the recommended way to install the Unimatrix SDK for Python, which is available on [PyPI](https://pypi.org/project/uni-sdk/).
-        
-        Run the following command to add `uni-sdk` as a dependency to your project:
-        
-        ```bash
-        pip install uni-sdk
-        ```
-        
-        ## Usage
-        
-        The following example shows how to use the Unimatrix Python SDK to interact with Unimatrix services.
-        
-        ### Send SMS
-        
-        Send a text message to a single recipient.
-        
-        ```py
-        
-        from uni.client import UniClient
-        from uni.exception import UniException
-        
-        client = UniClient("your access key id", "your access key secret")
-        
-        try:
-          res = client.messages.send({
-            "to": "your phone number", # in E.164 format
-            "signature": "your sender name",
-            "content": "Your verification code is 2048."
-          })
-          print(res.data)
-        except UniException as e:
-          print(e)
-        
-        ```
-        
-        ## Reference
-        
-        ### Other Unimatrix SDKs
-        
-        To find Unimatrix SDKs in other programming languages, check out the list below:
-        
-        - [Java](https://github.com/unimtx/uni-java-sdk)
-        - [Go](https://github.com/unimtx/uni-go-sdk)
-        - [Node.js](https://github.com/unimtx/uni-node-sdk)
-        - [PHP](https://github.com/unimtx/uni-php-sdk)
-        
-        ## License
-        
-        This library is released under the [MIT License](https://github.com/unimtx/uni-python-sdk/blob/main/LICENSE).
-        
-Keywords: unimatrix,sms,messaging,2fa,verification,sdk,api
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
+# Unimatrix Python SDK
+
+[![PyPI](https://img.shields.io/pypi/v/uni-sdk.svg)](https://pypi.python.org/pypi/uni-sdk) [![Release](https://img.shields.io/github/release/unimtx/uni-python-sdk.svg)](https://github.com/unimtx/uni-python-sdk/releases/latest) [![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/unimtx/uni-python-sdk/blob/main/LICENSE)
+
+The Unimatrix Python SDK provides convenient access to integrate communication capabilities into your Python applications using the Unimatrix HTTP API. The SDK provides support for sending SMS, 2FA verification, and phone number lookup.
+
+## Getting started
+
+Before you begin, you need an [Unimatrix](https://www.unimtx.com/) account. If you don't have one yet, you can [sign up](https://www.unimtx.com/signup?s=python.sdk.gh) for an Unimatrix account and get free credits to get you started.
+
+## Documentation
+
+Check out the documentation at [unimtx.com/docs](https://www.unimtx.com/docs) for a quick overview.
+
+## Installation
+
+Using pip is the recommended way to install the Unimatrix SDK for Python, which is available on [PyPI](https://pypi.org/project/uni-sdk/).
+
+Run the following command to add `uni-sdk` as a dependency to your project:
+
+```bash
+pip install uni-sdk
+```
+
+## Usage
+
+The following example shows how to use the Unimatrix Python SDK to interact with Unimatrix services.
+
+### Initialize a client
+
+```py
+from uni.client import UniClient
+
+client = UniClient("your access key id", "your access key secret")
+```
+
+or you can configure your credentials by environment variables:
+
+```sh
+export UNIMTX_ACCESS_KEY_ID=your_access_key_id
+export UNIMTX_ACCESS_KEY_SECRET=your_access_key_secret
+```
+
+### Send SMS
+
+Send a text message to a single recipient.
+
+```py
+from uni.client import UniClient
+from uni.exception import UniException
+
+client = UniClient()
+
+try:
+  res = client.messages.send({
+    "to": "+1206880xxxx", # in E.164 format
+    "text": "Your verification code is 2048."
+  })
+  print(res.data)
+except UniException as e:
+  print(e)
+```
+
+### Send verification code
+
+Send a one-time passcode (OTP) to a recipient. The following example will automatically generate a verification code.
+
+```py
+from uni.client import UniClient
+from uni.exception import UniException
+
+client = UniClient()
+
+try:
+  res = client.otp.send({
+    "to": "+1206880xxxx"
+  })
+  print(res.data)
+except UniException as e:
+  print(e)
+```
+
+### Check verification code
+
+Verify the one-time passcode (OTP) that a user provided. The following example will check whether the user-provided verification code is correct.
+
+```py
+from uni.client import UniClient
+from uni.exception import UniException
+
+client = UniClient()
+
+try:
+  res = client.otp.verify({
+    "to": "+1206880xxxx",
+    "code": "123456" # the code user provided
+  })
+  print(res.valid)
+except UniException as e:
+  print(e)
+```
+
+## Reference
+
+### Other Unimatrix SDKs
+
+To find Unimatrix SDKs in other programming languages, check out the list below:
+
+- [Java](https://github.com/unimtx/uni-java-sdk)
+- [Go](https://github.com/unimtx/uni-go-sdk)
+- [Node.js](https://github.com/unimtx/uni-node-sdk)
+- [PHP](https://github.com/unimtx/uni-php-sdk)
+- [Ruby](https://github.com/unimtx/uni-ruby-sdk)
+- [.NET](https://github.com/unimtx/uni-dotnet-sdk)
+
+## License
+
+This library is released under the [MIT License](https://github.com/unimtx/uni-python-sdk/blob/main/LICENSE).
```

### Comparing `uni-sdk-0.2.0/LICENSE` & `uni-sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uni-sdk-0.2.0/setup.py` & `uni-sdk-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 PACKAGE = 'uni'
 NAME = 'uni-sdk'
 DESCRIPTION = 'The official Unimatrix SDK for Python.'
 URL = 'https://github.com/unimtx/uni-python-sdk'
 AUTHOR = 'Unimatrix'
 EMAIL = 'dev@unimtx.com'
-KEYWORDS = ['unimatrix', 'sms', 'messaging', '2fa', 'verification', 'sdk', 'api']
+KEYWORDS = ['unimatrix', 'unisdk', 'sms', 'messaging', '2fa', 'otp', 'verification', 'sdk', 'api']
 REQUIRES_PYTHON = '>=3.6.0'
 VERSION = None
 
 REQUIRED = []
 
 EXTRAS = {}
```

### Comparing `uni-sdk-0.2.0/uni/client.py` & `uni-sdk-0.3.0/uni/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 import http.client
 import urllib.parse
 import time
 import hmac
 import json
 from urllib.parse import urlparse
 from uni.response import UniResponse
-from uni.services import (MessageService)
+from uni.services import (MessageService, OtpService)
 from uni.__version__ import __version__
 
 DEFAULT_ENDPOINT = "https://api.unimtx.com"
 DEFAULT_SIGNING_ALGORITHM = "hmac-sha256"
 
 class UniClient:
   name = "uni-python-sdk"
   version = __version__
 
-  def __init__(self, access_key_id, access_key_secret=None, endpoint=DEFAULT_ENDPOINT, signing_algorithm=DEFAULT_SIGNING_ALGORITHM):
-    self.access_key_id = access_key_id
-    self.access_key_secret = access_key_secret
-    self.endpoint = endpoint
+  def __init__(self, access_key_id = None, access_key_secret=None, endpoint=None, signing_algorithm=DEFAULT_SIGNING_ALGORITHM):
+    self.access_key_id = access_key_id or os.environ.get("UNIMTX_ACCESS_KEY_ID")
+    self.access_key_secret = access_key_secret or os.environ.get("UNIMTX_ACCESS_KEY_SECRET")
+    self.endpoint = endpoint or os.environ.get("UNIMTX_ENDPOINT") or DEFAULT_ENDPOINT
     self.signing_algorithm = signing_algorithm
     self.hmac_algorithm = signing_algorithm.split("-")[1]
 
     self.messages = MessageService(self)
+    self.otp = OtpService(self)
 
   def __sign(self, query):
     if (self.access_key_secret != None):
       query["algorithm"] = self.signing_algorithm
       query["timestamp"] = int(time.time())
       query["nonce"] = os.urandom(8).hex()
```

### Comparing `uni-sdk-0.2.0/uni/response.py` & `uni-sdk-0.3.0/uni/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,9 +20,10 @@
       else:
         self.code = code
         self.message = message
         self.data = body["data"]
     else:
       raise UniException(status_text, -1, request_id=request_id)
 
+    self.status = status
     self.raw = res
     self.request_id = request_id
```

