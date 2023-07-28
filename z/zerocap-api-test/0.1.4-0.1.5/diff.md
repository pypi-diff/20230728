# Comparing `tmp/zerocap_api_test-0.1.4.tar.gz` & `tmp/zerocap_api_test-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerocap_api_test-0.1.4.tar", last modified: Wed Jul 26 08:02:23 2023, max compression
+gzip compressed data, was "zerocap_api_test-0.1.5.tar", last modified: Fri Jul 28 05:27:19 2023, max compression
```

## Comparing `zerocap_api_test-0.1.4.tar` & `zerocap_api_test-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/
--rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.4/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1454 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1074 2023-07-26 07:10:20.000000 zerocap_api_test-0.1.4/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      792 2023-07-26 08:02:15.000000 zerocap_api_test-0.1.4/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test/
--rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.4/zerocap_api_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6928 2023-07-26 07:42:11.000000 zerocap_api_test-0.1.4/zerocap_api_test/main.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1454 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      284 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.606649 zerocap_api_test-0.1.5/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.5/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)     1620 2023-07-28 05:27:19.606205 zerocap_api_test-0.1.5/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)     1240 2023-07-28 05:26:50.000000 zerocap_api_test-0.1.5/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-28 05:27:19.606772 zerocap_api_test-0.1.5/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      792 2023-07-28 05:24:45.000000 zerocap_api_test-0.1.5/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.604151 zerocap_api_test-0.1.5/zerocap_api_test/
+-rw-r--r--   0 gao        (501) staff       (20)      121 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.5/zerocap_api_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     7467 2023-07-28 05:18:21.000000 zerocap_api_test-0.1.5/zerocap_api_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-28 05:27:19.605719 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)     1620 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      284 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       17 2023-07-28 05:27:19.000000 zerocap_api_test-0.1.5/zerocap_api_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_test-0.1.4/LICENSE.txt` & `zerocap_api_test-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.4/PKG-INFO` & `zerocap_api_test-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_api_test
-Version: 0.1.4
+Version: 0.1.5
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,19 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note=None, third_identity_id=None)
+    result = client.fetch_order(id, note="", third_identity_id="")
 
-    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
+    result = client.fetch_orders(symbol = '', start_datetime = '', end_datetime = 0, page = '', limit = '', ids = "",
+                                status = "", sort_order = "", order_type = "", side = "", third_identity_id = "",
+                                note = "")
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

### Comparing `zerocap_api_test-0.1.4/README.rst` & `zerocap_api_test-0.1.5/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note=None, third_identity_id=None)
+    result = client.fetch_order(id, note="", third_identity_id="")
 
-    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
+    result = client.fetch_orders(symbol = '', start_datetime = '', end_datetime = 0, page = '', limit = '', ids = "",
+                                status = "", sort_order = "", order_type = "", side = "", third_identity_id = "",
+                                note = "")
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

### Comparing `zerocap_api_test-0.1.4/setup.py` & `zerocap_api_test-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_api_test',  # 包名
-      version='0.1.4',  # 版本号
+      version='0.1.5',  # 版本号
       description='zerocap_api',
       long_description=long_description,
       author='jiayu.gao',
       author_email='jiayu.gao@eigen.capital',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_api_test-0.1.4/zerocap_api_test/main.py` & `zerocap_api_test-0.1.5/zerocap_api_test/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,16 @@
             self.api_secret.encode("utf-8"), self.api_key.encode("utf-8"), hashlib.sha256
         ).hexdigest()
 
     def encryption_api_key(self):
         signature = self.hashing()
         return signature
 
-    def create_order(self, symbol, side, type, amount, price, client_order_id, note, third_identity_id):
+    def create_order(self, symbol: str, side: str, type: str, amount: str, price: str, client_order_id: str,
+                     note: str, third_identity_id: str):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Create Order Api Key error"
 
         url = f"{self.base_url}/create_order"
         headers = {
             'Content-Type': 'application/json',
@@ -145,15 +146,15 @@
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
         else:
             raise Exception(response.text)
 
-    def fetch_order(self, id, note='', third_identity_id=''):
+    def fetch_order(self, id: str, note: str = '', third_identity_id: str = ''):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Order Api Key error"
 
         url = f"{self.base_url}/fetch_order"
         headers = {
             'Content-Type': 'application/json',
@@ -170,26 +171,36 @@
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
         else:
             raise Exception(response.text)
 
-    def fetch_orders(self, symbol: str='', since: int='', limit: int=0, note: str='', third_identity_id:str=''):
+    def fetch_orders(self, symbol: str = '', start_datetime: int = '', end_datetime: int = 0, page: int = '',
+                     limit: int = '', ids: str = "", status: str = "", sort_order: str = "", order_type: str = "",
+                     side: str = "", third_identity_id: str = "", note: str = ""
+                     ):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Orders Api Key error"
 
         url = f"{self.base_url}/fetch_orders"
         headers = {
             'Content-Type': 'application/json',
         }
         data = {
             "symbol": symbol,
-            "since": since,
+            "start_datetime": start_datetime,
+            "end_datetime": end_datetime,
+            "page": page,
+            "ids": ids,
+            "status": status,
+            "sort_order": sort_order,
+            "order_type": order_type,
+            "side": side,
             "limit": limit,
             "account_vault": {
                 "third_identity_id": third_identity_id,
                 "api_key": self.api_key,
                 "signature": signature,
                 "note": note,
             }
```

### Comparing `zerocap_api_test-0.1.4/zerocap_api_test.egg-info/PKG-INFO` & `zerocap_api_test-0.1.5/zerocap_api_test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-api-test
-Version: 0.1.4
+Version: 0.1.5
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,19 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note=None, third_identity_id=None)
+    result = client.fetch_order(id, note="", third_identity_id="")
 
-    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
+    result = client.fetch_orders(symbol = '', start_datetime = '', end_datetime = 0, page = '', limit = '', ids = "",
+                                status = "", sort_order = "", order_type = "", side = "", third_identity_id = "",
+                                note = "")
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

