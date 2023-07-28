# Comparing `tmp/nanohelp-0.0.4.tar.gz` & `tmp/nanohelp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.0.4.tar", max compression
+gzip compressed data, was "nanohelp-0.0.5.tar", max compression
```

## Comparing `nanohelp-0.0.4.tar` & `nanohelp-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.4/LICENSE
--rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.4/README.md
--rw-r--r--   0        0        0      176 2023-07-28 02:56:09.128158 nanohelp-0.0.4/nanohelp/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-28 02:55:07.370199 nanohelp-0.0.4/nanohelp/wallet.py
--rw-r--r--   0        0        0      475 2023-07-28 02:56:03.457103 nanohelp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 nanohelp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.0.5/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-28 02:45:10.243651 nanohelp-0.0.5/README.md
+-rw-r--r--   0        0        0      176 2023-07-28 02:59:08.968017 nanohelp-0.0.5/nanohelp/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-28 02:55:07.370199 nanohelp-0.0.5/nanohelp/wallet.py
+-rw-r--r--   0        0        0      475 2023-07-28 02:59:13.588017 nanohelp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 nanohelp-0.0.5/PKG-INFO
```

### Comparing `nanohelp-0.0.4/LICENSE` & `nanohelp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.4/nanohelp/wallet.py` & `nanohelp-0.0.5/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.0.4/PKG-INFO` & `nanohelp-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.0.4
+Version: 0.0.5
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: basicnanoclient (>=0.0.5,<0.0.6)
```

