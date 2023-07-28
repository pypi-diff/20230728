# Comparing `tmp/nanohelp-0.0.2.tar.gz` & `tmp/nanohelp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.0.2.tar", max compression
+gzip compressed data, was "nanohelp-0.0.3.tar", max compression
```

## Comparing `nanohelp-0.0.2.tar` & `nanohelp-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.2/LICENSE
--rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.2/README.md
--rw-r--r--   0        0        0      176 2023-07-28 02:51:53.596222 nanohelp-0.0.2/nanohelp/__init__.py
--rw-r--r--   0        0        0     3445 2023-07-28 02:31:03.365137 nanohelp-0.0.2/nanohelp/wallet.py
--rw-r--r--   0        0        0      448 2023-07-28 02:51:44.871067 nanohelp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.3/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.3/README.md
+-rw-r--r--   0        0        0      176 2023-07-28 02:53:49.647042 nanohelp-0.0.3/nanohelp/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-28 02:53:25.787075 nanohelp-0.0.3/nanohelp/wallet.py
+-rw-r--r--   0        0        0      448 2023-07-28 02:53:46.086629 nanohelp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.3/PKG-INFO
```

### Comparing `nanohelp-0.0.2/LICENSE` & `nanohelp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.2/nanohelp/wallet.py` & `nanohelp-0.0.3/nanohelp/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from basicnanoclient import BasicNanoClient
+from basicnanoclient.nano import BasicNanoClient
 import time
 
 class WalletManager:
     def __init__(self, node_address):
         self.client = BasicNanoClient(node_address)
         self.transaction_history = {}
```

### Comparing `nanohelp-0.0.2/PKG-INFO` & `nanohelp-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

