# Comparing `tmp/nanohelp-0.0.5.tar.gz` & `tmp/nanohelp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.0.5.tar", max compression
+gzip compressed data, was "nanohelp-0.0.6.tar", max compression
```

## Comparing `nanohelp-0.0.5.tar` & `nanohelp-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.5/LICENSE
--rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.5/README.md
--rw-r--r--   0        0        0      176 2023-07-28 02:59:08.968017 nanohelp-0.0.5/nanohelp/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-28 02:55:07.370199 nanohelp-0.0.5/nanohelp/wallet.py
--rw-r--r--   0        0        0      475 2023-07-28 02:59:13.588017 nanohelp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 nanohelp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.6/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.6/README.md
+-rw-r--r--   0        0        0      176 2023-07-28 03:14:29.634894 nanohelp-0.0.6/nanohelp/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-28 02:55:07.370199 nanohelp-0.0.6/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-28 03:14:24.428041 nanohelp-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 nanohelp-0.0.6/PKG-INFO
```

### Comparing `nanohelp-0.0.5/LICENSE` & `nanohelp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.5/nanohelp/wallet.py` & `nanohelp-0.0.6/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.5/PKG-INFO` & `nanohelp-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: basicnanoclient (>=0.0.5,<0.0.6)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: py-multicodec (>=0.2.1,<0.3.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # nanohelp
```

