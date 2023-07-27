# Comparing `tmp/sapphire_config-1.0.3.tar.gz` & `tmp/sapphire_config-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapphire_config-1.0.3.tar", last modified: Mon Jul 24 19:57:33 2023, max compression
+gzip compressed data, was "sapphire_config-1.0.4.tar", last modified: Thu Jul 27 21:50:52 2023, max compression
```

## Comparing `sapphire_config-1.0.3.tar` & `sapphire_config-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/README.md
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/components/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/components/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/examples/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/config/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/examples/config/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.3/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/src/sapphire_config/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5139 2023-07-05 19:42:10.000000 sapphire_config-1.0.3/src/sapphire_config/component.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-24 18:36:09.000000 sapphire_config-1.0.3/src/sapphire_config/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10027 2023-07-24 19:55:14.000000 sapphire_config-1.0.3/src/sapphire_config/parser.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      655 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/src/sapphire_config.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/tests/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-24 19:57:33.000000 sapphire_config-1.0.3/tests/__pycache__/
--rw-rw-r--   0 valentic   (500) valentic   (500)    84897 2023-07-24 19:55:12.000000 sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-311-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)    17175 2023-07-24 19:55:10.000000 sapphire_config-1.0.3/tests/test_sapphireconfig.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/README.md
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/examples/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/examples/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/examples/components/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/examples/components/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/examples/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/examples/config/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/examples/config/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.4/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.4/src/sapphire_config/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5206 2023-07-27 21:50:41.000000 sapphire_config-1.0.4/src/sapphire_config/component.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-26 01:19:42.000000 sapphire_config-1.0.4/src/sapphire_config/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10027 2023-07-24 19:55:14.000000 sapphire_config-1.0.4/src/sapphire_config/parser.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      655 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/src/sapphire_config.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 21:50:52.000000 sapphire_config-1.0.4/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    88114 2023-07-27 04:16:56.000000 sapphire_config-1.0.4/tests/__pycache__/test_sapphireconfig.cpython-311-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.4/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)    17975 2023-07-27 04:16:54.000000 sapphire_config-1.0.4/tests/test_sapphireconfig.py
```

### Comparing `sapphire_config-1.0.3/LICENSE` & `sapphire_config-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/PKG-INFO` & `sapphire_config-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire_config
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.3/examples/components/demo.conf` & `sapphire_config-1.0.4/examples/components/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/examples/components/demo.py` & `sapphire_config-1.0.4/examples/components/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/examples/config/demo.conf` & `sapphire_config-1.0.4/examples/config/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/examples/config/demo.py` & `sapphire_config-1.0.4/examples/config/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/pyproject.toml` & `sapphire_config-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/src/sapphire_config/component.py` & `sapphire_config-1.0.4/src/sapphire_config/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,16 +75,22 @@
 #   2023-06-26  Todd Valentic
 #               Initial implementation.
 #                   Complete rewrite with a new approach. Create a new
 #                   configparser filled in with entries specific for the
 #                   component. Allows for the reuse of features without
 #                   any new machinery.
 #
+#   2023-7-25   Todd Valentic
+#               Add set() and options() to config
+#               Remove get() mapping, use config
+#
 ##########################################################################
 
+from functools import partial
+
 from .parser import Parser
 
 # pylint: disable=too-few-public-methods, unused-argument
 
 class Component:
     """A component proxy from parent config"""
 
@@ -128,20 +134,16 @@
         proxy.update(self._get_values(parent, f"{prefix}.{name}."))
 
         # Add component meta options to section
 
         proxy["name"] = name
         proxy[prefix] = name
 
-        # Map the get*() methods onto object
-
-        for key in dir(proxy):
-            method = getattr(proxy, key)
-            if callable(method) and key.startswith("get"):
-                setattr(self, key, method)
+        proxy.set = partial(proxy.parser.set, proxy.name)
+        proxy.options = partial(proxy.parser.options, proxy.name) 
 
         return proxy
 
     def _get_values(self, parent, prefix):
         result = {}
 
         for key in parent:
```

### Comparing `sapphire_config-1.0.3/src/sapphire_config/parser.py` & `sapphire_config-1.0.4/src/sapphire_config/parser.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/src/sapphire_config.egg-info/PKG-INFO` & `sapphire_config-1.0.4/src/sapphire_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire-config
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.3/src/sapphire_config.egg-info/SOURCES.txt` & `sapphire_config-1.0.4/src/sapphire_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-311-pytest-7.4.0.pyc` & `sapphire_config-1.0.4/tests/__pycache__/test_sapphireconfig.cpython-311-pytest-7.4.0.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,36 +1,37 @@
 magic:    0xa70d0d0a
-moddate:  0x1ed7be64 (Mon Jul 24 19:55:10 2023 UTC)
-files sz: 17175
+moddate:  0xb6efc164 (Thu Jul 27 04:16:54 2023 UTC)
+files sz: 17975
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a02640164026c036d04630201006d055a
       060100640164026c075a07640164026c085a08640164026c095a09640164
       026c0a5a0a640164026c0b5a0b640164036c0c6d0d5a0d0100640164026c
       0e5a0f02004700640484006405650f6a100000000000000000a6030000ab
-      0300000000000000005a11640684005a12640784005a13640884005a1464
-      0984005a15640a84005a16640b84005a17640c84005a18640d84005a1964
-      0e84005a1a640f84005a1b641084005a1c641184005a1d641284005a1e64
-      1384005a1f641484005a20641584005a21641684005a22641784005a2364
-      1884005a24641984005a25641a84005a26641b84005a27641c84005a2864
-      1d84005a29641e84005a2a641f84005a2b642084005a2c642184005a2d64
-      2284005a2e642384005a2f642484005a30642584005a31642684005a3264
-      2784005a33642884005a34642984005a35642a84005a36642b84005a3764
-      2c84005a38642d84005a39642e84005a3a642f84005a3b643084005a3c64
-      3184005a3d643284005a3e643384005a3f643484005a40643584005a4164
-      3684005a42643784005a43643884005a44643984005a45643a84005a4664
-      3b84005a47643c84005a48643d84005a49643e84005a4a643f84005a4b64
-      4084005a4c644184005a4d644284005a4e644384005a4f644484005a5064
-      4584005a51644684005a52644784005a53644884005a54644984005a5564
-      4a84005a56644b84005a57644c84005a58644d84005a59644e84005a5a64
-      025300
+      0300000000000000005a1102004700640684006407650f6a100000000000
+      000000a6030000ab0300000000000000005a12640884005a13640984005a
+      14640a84005a15640b84005a16640c84005a17640d84005a18640e84005a
+      19640f84005a1a641084005a1b641184005a1c641284005a1d641384005a
+      1e641484005a1f641584005a20641684005a21641784005a22641884005a
+      23641984005a24641a84005a25641b84005a26641c84005a27641d84005a
+      28641e84005a29641f84005a2a642084005a2b642184005a2c642284005a
+      2d642384005a2e642484005a2f642584005a30642684005a31642784005a
+      32642884005a33642984005a34642a84005a35642b84005a36642c84005a
+      37642d84005a38642e84005a39642f84005a3a643084005a3b643184005a
+      3c643284005a3d643384005a3e643484005a3f643584005a40643684005a
+      41643784005a42643884005a43643984005a44643a84005a45643b84005a
+      46643c84005a47643d84005a48643e84005a49643f84005a4a644084005a
+      4b644184005a4c644284005a4d644384005a4e644484005a4f644584005a
+      50644684005a51644784005a52644884005a53644984005a54644a84005a
+      55644b84005a56644c84005a57644d84005a58644e84005a59644f84005a
+      5a645084005a5b645184005a5c645284005a5d64025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Sapphire Unit Tests')
                  4 STORE_NAME               0 (__doc__)
    
      5           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
@@ -89,307 +90,326 @@
                100 LOAD_CONST               5 ('Factory')
                102 LOAD_NAME               15 (sapphire)
                104 LOAD_ATTR               16 (Component)
                114 PRECALL                  3
                118 CALL                     3
                128 STORE_NAME              17 (Factory)
    
-    21         130 LOAD_CONST               6 (<code object test_get_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 21>)
-               132 MAKE_FUNCTION            0
-               134 STORE_NAME              18 (test_get_parser)
-   
-    29         136 LOAD_CONST               7 (<code object test_get_proxy_dict, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 29>)
-               138 MAKE_FUNCTION            0
-               140 STORE_NAME              19 (test_get_proxy_dict)
-   
-    37         142 LOAD_CONST               8 (<code object test_get_missing_section, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 37>)
-               144 MAKE_FUNCTION            0
-               146 STORE_NAME              20 (test_get_missing_section)
-   
-    43         148 LOAD_CONST               9 (<code object test_get_missing_option, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 43>)
-               150 MAKE_FUNCTION            0
-               152 STORE_NAME              21 (test_get_missing_option)
-   
-    50         154 LOAD_CONST              10 (<code object test_get_proxy_func, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 50>)
-               156 MAKE_FUNCTION            0
-               158 STORE_NAME              22 (test_get_proxy_func)
-   
-    58         160 LOAD_CONST              11 (<code object test_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 58>)
-               162 MAKE_FUNCTION            0
-               164 STORE_NAME              23 (test_int)
-   
-    66         166 LOAD_CONST              12 (<code object test_int_hex, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 66>)
-               168 MAKE_FUNCTION            0
-               170 STORE_NAME              24 (test_int_hex)
-   
-    74         172 LOAD_CONST              13 (<code object test_int_base, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 74>)
-               174 MAKE_FUNCTION            0
-               176 STORE_NAME              25 (test_int_base)
-   
-    82         178 LOAD_CONST              14 (<code object test_int_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 82>)
-               180 MAKE_FUNCTION            0
-               182 STORE_NAME              26 (test_int_fallback_none)
-   
-    89         184 LOAD_CONST              15 (<code object test_int_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 89>)
-               186 MAKE_FUNCTION            0
-               188 STORE_NAME              27 (test_int_fallback_str)
-   
-    96         190 LOAD_CONST              16 (<code object test_int_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 96>)
-               192 MAKE_FUNCTION            0
-               194 STORE_NAME              28 (test_int_fallback_int)
-   
-   103         196 LOAD_CONST              17 (<code object test_boolean, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 103>)
-               198 MAKE_FUNCTION            0
-               200 STORE_NAME              29 (test_boolean)
-   
-   111         202 LOAD_CONST              18 (<code object test_boolean_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 111>)
-               204 MAKE_FUNCTION            0
-               206 STORE_NAME              30 (test_boolean_fallback_none)
-   
-   118         208 LOAD_CONST              19 (<code object test_boolean_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 118>)
-               210 MAKE_FUNCTION            0
-               212 STORE_NAME              31 (test_boolean_fallback_str)
-   
-   125         214 LOAD_CONST              20 (<code object test_boolean_fallback_bool_t, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 125>)
-               216 MAKE_FUNCTION            0
-               218 STORE_NAME              32 (test_boolean_fallback_bool_t)
-   
-   132         220 LOAD_CONST              21 (<code object test_boolean_fallback_bool_f, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 132>)
-               222 MAKE_FUNCTION            0
-               224 STORE_NAME              33 (test_boolean_fallback_bool_f)
-   
-   139         226 LOAD_CONST              22 (<code object test_boolean_fallback_int_t, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 139>)
-               228 MAKE_FUNCTION            0
-               230 STORE_NAME              34 (test_boolean_fallback_int_t)
-   
-   146         232 LOAD_CONST              23 (<code object test_boolean_fallback_int_f, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 146>)
-               234 MAKE_FUNCTION            0
-               236 STORE_NAME              35 (test_boolean_fallback_int_f)
-   
-   153         238 LOAD_CONST              24 (<code object test_get_list_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 153>)
-               240 MAKE_FUNCTION            0
-               242 STORE_NAME              36 (test_get_list_parser)
-   
-   161         244 LOAD_CONST              25 (<code object test_get_list_proxy_func, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 161>)
-               246 MAKE_FUNCTION            0
-               248 STORE_NAME              37 (test_get_list_proxy_func)
-   
-   169         250 LOAD_CONST              26 (<code object test_get_list_conv_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 169>)
-               252 MAKE_FUNCTION            0
-               254 STORE_NAME              38 (test_get_list_conv_parser)
-   
-   177         256 LOAD_CONST              27 (<code object test_get_list_conv_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 177>)
-               258 MAKE_FUNCTION            0
-               260 STORE_NAME              39 (test_get_list_conv_proxy)
-   
-   185         262 LOAD_CONST              28 (<code object test_get_list_sep, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 185>)
-               264 MAKE_FUNCTION            0
-               266 STORE_NAME              40 (test_get_list_sep)
-   
-   193         268 LOAD_CONST              29 (<code object test_get_list_sep_conv, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 193>)
-               270 MAKE_FUNCTION            0
-               272 STORE_NAME              41 (test_get_list_sep_conv)
-   
-   201         274 LOAD_CONST              30 (<code object test_get_list_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 201>)
-               276 MAKE_FUNCTION            0
-               278 STORE_NAME              42 (test_get_list_fallback_none)
-   
-   209         280 LOAD_CONST              31 (<code object test_get_list_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 209>)
-               282 MAKE_FUNCTION            0
-               284 STORE_NAME              43 (test_get_list_fallback_str)
-   
-   216         286 LOAD_CONST              32 (<code object test_get_list_no_section, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 216>)
-               288 MAKE_FUNCTION            0
-               290 STORE_NAME              44 (test_get_list_no_section)
-   
-   222         292 LOAD_CONST              33 (<code object test_get_list_fallback_type_error, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 222>)
-               294 MAKE_FUNCTION            0
-               296 STORE_NAME              45 (test_get_list_fallback_type_error)
-   
-   229         298 LOAD_CONST              34 (<code object test_get_list_fallback_empty_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 229>)
-               300 MAKE_FUNCTION            0
-               302 STORE_NAME              46 (test_get_list_fallback_empty_str)
-   
-   236         304 LOAD_CONST              35 (<code object test_get_list_fallback_list, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 236>)
-               306 MAKE_FUNCTION            0
-               308 STORE_NAME              47 (test_get_list_fallback_list)
-   
-   243         310 LOAD_CONST              36 (<code object test_get_set_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 243>)
-               312 MAKE_FUNCTION            0
-               314 STORE_NAME              48 (test_get_set_parser)
-   
-   251         316 LOAD_CONST              37 (<code object test_get_set_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 251>)
-               318 MAKE_FUNCTION            0
-               320 STORE_NAME              49 (test_get_set_proxy)
-   
-   259         322 LOAD_CONST              38 (<code object test_get_set_conv_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 259>)
-               324 MAKE_FUNCTION            0
-               326 STORE_NAME              50 (test_get_set_conv_parser)
-   
-   267         328 LOAD_CONST              39 (<code object test_get_set_sep, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 267>)
-               330 MAKE_FUNCTION            0
-               332 STORE_NAME              51 (test_get_set_sep)
-   
-   275         334 LOAD_CONST              40 (<code object test_get_bytes, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 275>)
-               336 MAKE_FUNCTION            0
-               338 STORE_NAME              52 (test_get_bytes)
-   
-   283         340 LOAD_CONST              41 (<code object test_get_datetime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 283>)
-               342 MAKE_FUNCTION            0
-               344 STORE_NAME              53 (test_get_datetime)
-   
-   291         346 LOAD_CONST              42 (<code object test_get_datetime_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 291>)
-               348 MAKE_FUNCTION            0
-               350 STORE_NAME              54 (test_get_datetime_fallback_none)
-   
-   298         352 LOAD_CONST              43 (<code object test_get_datetime_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 298>)
-               354 MAKE_FUNCTION            0
-               356 STORE_NAME              55 (test_get_datetime_fallback_str)
-   
-   305         358 LOAD_CONST              44 (<code object test_get_datetime_fallback_datetime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 305>)
-               360 MAKE_FUNCTION            0
-               362 STORE_NAME              56 (test_get_datetime_fallback_datetime)
-   
-   313         364 LOAD_CONST              45 (<code object test_get_timedelta, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 313>)
-               366 MAKE_FUNCTION            0
-               368 STORE_NAME              57 (test_get_timedelta)
-   
-   321         370 LOAD_CONST              46 (<code object test_get_timedelta_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 321>)
-               372 MAKE_FUNCTION            0
-               374 STORE_NAME              58 (test_get_timedelta_fallback_none)
-   
-   328         376 LOAD_CONST              47 (<code object test_get_timedelta_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 328>)
-               378 MAKE_FUNCTION            0
-               380 STORE_NAME              59 (test_get_timedelta_fallback_str)
-   
-   335         382 LOAD_CONST              48 (<code object test_get_timedelta_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 335>)
-               384 MAKE_FUNCTION            0
-               386 STORE_NAME              60 (test_get_timedelta_fallback_int)
-   
-   342         388 LOAD_CONST              49 (<code object test_get_timeselta_fallback_td, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 342>)
-               390 MAKE_FUNCTION            0
-               392 STORE_NAME              61 (test_get_timeselta_fallback_td)
-   
-   350         394 LOAD_CONST              50 (<code object test_get_path, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 350>)
-               396 MAKE_FUNCTION            0
-               398 STORE_NAME              62 (test_get_path)
-   
-   358         400 LOAD_CONST              51 (<code object test_get_path_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 358>)
-               402 MAKE_FUNCTION            0
-               404 STORE_NAME              63 (test_get_path_fallback_none)
-   
-   365         406 LOAD_CONST              52 (<code object test_get_path_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 365>)
-               408 MAKE_FUNCTION            0
-               410 STORE_NAME              64 (test_get_path_fallback_str)
-   
-   372         412 LOAD_CONST              53 (<code object test_get_path_fallback_path, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 372>)
-               414 MAKE_FUNCTION            0
-               416 STORE_NAME              65 (test_get_path_fallback_path)
-   
-   380         418 LOAD_CONST              54 (<code object test_get_rate, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 380>)
-               420 MAKE_FUNCTION            0
-               422 STORE_NAME              66 (test_get_rate)
-   
-   391         424 LOAD_CONST              55 (<code object test_get_rate_all, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 391>)
-               426 MAKE_FUNCTION            0
-               428 STORE_NAME              67 (test_get_rate_all)
-   
-   406         430 LOAD_CONST              56 (<code object test_get_rate_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 406>)
-               432 MAKE_FUNCTION            0
-               434 STORE_NAME              68 (test_get_rate_fallback_none)
-   
-   414         436 LOAD_CONST              57 (<code object test_get_rate_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 414>)
-               438 MAKE_FUNCTION            0
-               440 STORE_NAME              69 (test_get_rate_fallback_str)
-   
-   424         442 LOAD_CONST              58 (<code object test_get_rate_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 424>)
-               444 MAKE_FUNCTION            0
-               446 STORE_NAME              70 (test_get_rate_fallback_int)
-   
-   434         448 LOAD_CONST              59 (<code object test_get_rate_fallback_rate, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 434>)
-               450 MAKE_FUNCTION            0
-               452 STORE_NAME              71 (test_get_rate_fallback_rate)
-   
-   444         454 LOAD_CONST              60 (<code object test_rate_init_default, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 444>)
-               456 MAKE_FUNCTION            0
-               458 STORE_NAME              72 (test_rate_init_default)
-   
-   454         460 LOAD_CONST              61 (<code object test_rate_init_timedelta, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 454>)
-               462 MAKE_FUNCTION            0
-               464 STORE_NAME              73 (test_rate_init_timedelta)
-   
-   464         466 LOAD_CONST              62 (<code object test_rate_nexttime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 464>)
-               468 MAKE_FUNCTION            0
-               470 STORE_NAME              74 (test_rate_nexttime)
-   
-   472         472 LOAD_CONST              63 (<code object test_rate_nexttime_sync, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 472>)
-               474 MAKE_FUNCTION            0
-               476 STORE_NAME              75 (test_rate_nexttime_sync)
-   
-   480         478 LOAD_CONST              64 (<code object test_rate_nexttime_offset, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 480>)
-               480 MAKE_FUNCTION            0
-               482 STORE_NAME              76 (test_rate_nexttime_offset)
-   
-   488         484 LOAD_CONST              65 (<code object test_rate_nexttime_offset_sync, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 488>)
-               486 MAKE_FUNCTION            0
-               488 STORE_NAME              77 (test_rate_nexttime_offset_sync)
-   
-   496         490 LOAD_CONST              66 (<code object test_rate_nexttime_offset_sync2, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 496>)
-               492 MAKE_FUNCTION            0
-               494 STORE_NAME              78 (test_rate_nexttime_offset_sync2)
-   
-   504         496 LOAD_CONST              67 (<code object test_get_components, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 504>)
-               498 MAKE_FUNCTION            0
-               500 STORE_NAME              79 (test_get_components)
-   
-   512         502 LOAD_CONST              68 (<code object test_get_components_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 512>)
-               504 MAKE_FUNCTION            0
-               506 STORE_NAME              80 (test_get_components_proxy)
-   
-   520         508 LOAD_CONST              69 (<code object test_get_callback, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 520>)
-               510 MAKE_FUNCTION            0
-               512 STORE_NAME              81 (test_get_callback)
-   
-   530         514 LOAD_CONST              70 (<code object test_get_interpolation, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 530>)
-               516 MAKE_FUNCTION            0
-               518 STORE_NAME              82 (test_get_interpolation)
-   
-   540         520 LOAD_CONST              71 (<code object test_get_interpolation_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 540>)
-               522 MAKE_FUNCTION            0
-               524 STORE_NAME              83 (test_get_interpolation_proxy)
-   
-   550         526 LOAD_CONST              72 (<code object test_get_interpolation_loop, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 550>)
-               528 MAKE_FUNCTION            0
-               530 STORE_NAME              84 (test_get_interpolation_loop)
-   
-   560         532 LOAD_CONST              73 (<code object test_component_mixin, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 560>)
-               534 MAKE_FUNCTION            0
-               536 STORE_NAME              85 (test_component_mixin)
-   
-   572         538 LOAD_CONST              74 (<code object test_component_mixin_default, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 572>)
-               540 MAKE_FUNCTION            0
-               542 STORE_NAME              86 (test_component_mixin_default)
-   
-   583         544 LOAD_CONST              75 (<code object test_timespan_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 583>)
-               546 MAKE_FUNCTION            0
-               548 STORE_NAME              87 (test_timespan_int)
-   
-   592         550 LOAD_CONST              76 (<code object test_timespan_td, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 592>)
-               552 MAKE_FUNCTION            0
-               554 STORE_NAME              88 (test_timespan_td)
-   
-   601         556 LOAD_CONST              77 (<code object test_timespan_rd, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 601>)
-               558 MAKE_FUNCTION            0
-               560 STORE_NAME              89 (test_timespan_rd)
-   
-   610         562 LOAD_CONST              78 (<code object test_escape, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 610>)
-               564 MAKE_FUNCTION            0
-               566 STORE_NAME              90 (test_escape)
-               568 LOAD_CONST               2 (None)
-               570 RETURN_VALUE
+    21         130 PUSH_NULL
+               132 LOAD_BUILD_CLASS
+               134 LOAD_CONST               6 (<code object FactorySet, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 21>)
+               136 MAKE_FUNCTION            0
+               138 LOAD_CONST               7 ('FactorySet')
+               140 LOAD_NAME               15 (sapphire)
+               142 LOAD_ATTR               16 (Component)
+               152 PRECALL                  3
+               156 CALL                     3
+               166 STORE_NAME              18 (FactorySet)
+   
+    30         168 LOAD_CONST               8 (<code object test_get_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 30>)
+               170 MAKE_FUNCTION            0
+               172 STORE_NAME              19 (test_get_parser)
+   
+    38         174 LOAD_CONST               9 (<code object test_get_proxy_dict, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 38>)
+               176 MAKE_FUNCTION            0
+               178 STORE_NAME              20 (test_get_proxy_dict)
+   
+    46         180 LOAD_CONST              10 (<code object test_get_missing_section, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 46>)
+               182 MAKE_FUNCTION            0
+               184 STORE_NAME              21 (test_get_missing_section)
+   
+    52         186 LOAD_CONST              11 (<code object test_get_missing_option, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 52>)
+               188 MAKE_FUNCTION            0
+               190 STORE_NAME              22 (test_get_missing_option)
+   
+    59         192 LOAD_CONST              12 (<code object test_get_proxy_func, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 59>)
+               194 MAKE_FUNCTION            0
+               196 STORE_NAME              23 (test_get_proxy_func)
+   
+    67         198 LOAD_CONST              13 (<code object test_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 67>)
+               200 MAKE_FUNCTION            0
+               202 STORE_NAME              24 (test_int)
+   
+    75         204 LOAD_CONST              14 (<code object test_int_hex, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 75>)
+               206 MAKE_FUNCTION            0
+               208 STORE_NAME              25 (test_int_hex)
+   
+    83         210 LOAD_CONST              15 (<code object test_int_base, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 83>)
+               212 MAKE_FUNCTION            0
+               214 STORE_NAME              26 (test_int_base)
+   
+    91         216 LOAD_CONST              16 (<code object test_int_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 91>)
+               218 MAKE_FUNCTION            0
+               220 STORE_NAME              27 (test_int_fallback_none)
+   
+    98         222 LOAD_CONST              17 (<code object test_int_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 98>)
+               224 MAKE_FUNCTION            0
+               226 STORE_NAME              28 (test_int_fallback_str)
+   
+   105         228 LOAD_CONST              18 (<code object test_int_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 105>)
+               230 MAKE_FUNCTION            0
+               232 STORE_NAME              29 (test_int_fallback_int)
+   
+   112         234 LOAD_CONST              19 (<code object test_boolean, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 112>)
+               236 MAKE_FUNCTION            0
+               238 STORE_NAME              30 (test_boolean)
+   
+   120         240 LOAD_CONST              20 (<code object test_boolean_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 120>)
+               242 MAKE_FUNCTION            0
+               244 STORE_NAME              31 (test_boolean_fallback_none)
+   
+   127         246 LOAD_CONST              21 (<code object test_boolean_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 127>)
+               248 MAKE_FUNCTION            0
+               250 STORE_NAME              32 (test_boolean_fallback_str)
+   
+   134         252 LOAD_CONST              22 (<code object test_boolean_fallback_bool_t, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 134>)
+               254 MAKE_FUNCTION            0
+               256 STORE_NAME              33 (test_boolean_fallback_bool_t)
+   
+   141         258 LOAD_CONST              23 (<code object test_boolean_fallback_bool_f, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 141>)
+               260 MAKE_FUNCTION            0
+               262 STORE_NAME              34 (test_boolean_fallback_bool_f)
+   
+   148         264 LOAD_CONST              24 (<code object test_boolean_fallback_int_t, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 148>)
+               266 MAKE_FUNCTION            0
+               268 STORE_NAME              35 (test_boolean_fallback_int_t)
+   
+   155         270 LOAD_CONST              25 (<code object test_boolean_fallback_int_f, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 155>)
+               272 MAKE_FUNCTION            0
+               274 STORE_NAME              36 (test_boolean_fallback_int_f)
+   
+   162         276 LOAD_CONST              26 (<code object test_get_list_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 162>)
+               278 MAKE_FUNCTION            0
+               280 STORE_NAME              37 (test_get_list_parser)
+   
+   170         282 LOAD_CONST              27 (<code object test_get_list_proxy_func, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 170>)
+               284 MAKE_FUNCTION            0
+               286 STORE_NAME              38 (test_get_list_proxy_func)
+   
+   178         288 LOAD_CONST              28 (<code object test_get_list_conv_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 178>)
+               290 MAKE_FUNCTION            0
+               292 STORE_NAME              39 (test_get_list_conv_parser)
+   
+   186         294 LOAD_CONST              29 (<code object test_get_list_conv_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 186>)
+               296 MAKE_FUNCTION            0
+               298 STORE_NAME              40 (test_get_list_conv_proxy)
+   
+   194         300 LOAD_CONST              30 (<code object test_get_list_sep, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 194>)
+               302 MAKE_FUNCTION            0
+               304 STORE_NAME              41 (test_get_list_sep)
+   
+   202         306 LOAD_CONST              31 (<code object test_get_list_sep_conv, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 202>)
+               308 MAKE_FUNCTION            0
+               310 STORE_NAME              42 (test_get_list_sep_conv)
+   
+   210         312 LOAD_CONST              32 (<code object test_get_list_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 210>)
+               314 MAKE_FUNCTION            0
+               316 STORE_NAME              43 (test_get_list_fallback_none)
+   
+   218         318 LOAD_CONST              33 (<code object test_get_list_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 218>)
+               320 MAKE_FUNCTION            0
+               322 STORE_NAME              44 (test_get_list_fallback_str)
+   
+   225         324 LOAD_CONST              34 (<code object test_get_list_no_section, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 225>)
+               326 MAKE_FUNCTION            0
+               328 STORE_NAME              45 (test_get_list_no_section)
+   
+   231         330 LOAD_CONST              35 (<code object test_get_list_fallback_type_error, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 231>)
+               332 MAKE_FUNCTION            0
+               334 STORE_NAME              46 (test_get_list_fallback_type_error)
+   
+   238         336 LOAD_CONST              36 (<code object test_get_list_fallback_empty_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 238>)
+               338 MAKE_FUNCTION            0
+               340 STORE_NAME              47 (test_get_list_fallback_empty_str)
+   
+   245         342 LOAD_CONST              37 (<code object test_get_list_fallback_list, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 245>)
+               344 MAKE_FUNCTION            0
+               346 STORE_NAME              48 (test_get_list_fallback_list)
+   
+   252         348 LOAD_CONST              38 (<code object test_get_set_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 252>)
+               350 MAKE_FUNCTION            0
+               352 STORE_NAME              49 (test_get_set_parser)
+   
+   260         354 LOAD_CONST              39 (<code object test_get_set_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 260>)
+               356 MAKE_FUNCTION            0
+               358 STORE_NAME              50 (test_get_set_proxy)
+   
+   268         360 LOAD_CONST              40 (<code object test_get_set_conv_parser, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 268>)
+               362 MAKE_FUNCTION            0
+               364 STORE_NAME              51 (test_get_set_conv_parser)
+   
+   276         366 LOAD_CONST              41 (<code object test_get_set_sep, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 276>)
+               368 MAKE_FUNCTION            0
+               370 STORE_NAME              52 (test_get_set_sep)
+   
+   284         372 LOAD_CONST              42 (<code object test_get_bytes, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 284>)
+               374 MAKE_FUNCTION            0
+               376 STORE_NAME              53 (test_get_bytes)
+   
+   292         378 LOAD_CONST              43 (<code object test_get_datetime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 292>)
+               380 MAKE_FUNCTION            0
+               382 STORE_NAME              54 (test_get_datetime)
+   
+   300         384 LOAD_CONST              44 (<code object test_get_datetime_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 300>)
+               386 MAKE_FUNCTION            0
+               388 STORE_NAME              55 (test_get_datetime_fallback_none)
+   
+   307         390 LOAD_CONST              45 (<code object test_get_datetime_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 307>)
+               392 MAKE_FUNCTION            0
+               394 STORE_NAME              56 (test_get_datetime_fallback_str)
+   
+   314         396 LOAD_CONST              46 (<code object test_get_datetime_fallback_datetime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 314>)
+               398 MAKE_FUNCTION            0
+               400 STORE_NAME              57 (test_get_datetime_fallback_datetime)
+   
+   322         402 LOAD_CONST              47 (<code object test_get_timedelta, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 322>)
+               404 MAKE_FUNCTION            0
+               406 STORE_NAME              58 (test_get_timedelta)
+   
+   330         408 LOAD_CONST              48 (<code object test_get_timedelta_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 330>)
+               410 MAKE_FUNCTION            0
+               412 STORE_NAME              59 (test_get_timedelta_fallback_none)
+   
+   337         414 LOAD_CONST              49 (<code object test_get_timedelta_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 337>)
+               416 MAKE_FUNCTION            0
+               418 STORE_NAME              60 (test_get_timedelta_fallback_str)
+   
+   344         420 LOAD_CONST              50 (<code object test_get_timedelta_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 344>)
+               422 MAKE_FUNCTION            0
+               424 STORE_NAME              61 (test_get_timedelta_fallback_int)
+   
+   351         426 LOAD_CONST              51 (<code object test_get_timeselta_fallback_td, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 351>)
+               428 MAKE_FUNCTION            0
+               430 STORE_NAME              62 (test_get_timeselta_fallback_td)
+   
+   359         432 LOAD_CONST              52 (<code object test_get_path, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 359>)
+               434 MAKE_FUNCTION            0
+               436 STORE_NAME              63 (test_get_path)
+   
+   367         438 LOAD_CONST              53 (<code object test_get_path_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 367>)
+               440 MAKE_FUNCTION            0
+               442 STORE_NAME              64 (test_get_path_fallback_none)
+   
+   374         444 LOAD_CONST              54 (<code object test_get_path_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 374>)
+               446 MAKE_FUNCTION            0
+               448 STORE_NAME              65 (test_get_path_fallback_str)
+   
+   381         450 LOAD_CONST              55 (<code object test_get_path_fallback_path, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 381>)
+               452 MAKE_FUNCTION            0
+               454 STORE_NAME              66 (test_get_path_fallback_path)
+   
+   389         456 LOAD_CONST              56 (<code object test_get_rate, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 389>)
+               458 MAKE_FUNCTION            0
+               460 STORE_NAME              67 (test_get_rate)
+   
+   400         462 LOAD_CONST              57 (<code object test_get_rate_all, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 400>)
+               464 MAKE_FUNCTION            0
+               466 STORE_NAME              68 (test_get_rate_all)
+   
+   415         468 LOAD_CONST              58 (<code object test_get_rate_fallback_none, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 415>)
+               470 MAKE_FUNCTION            0
+               472 STORE_NAME              69 (test_get_rate_fallback_none)
+   
+   423         474 LOAD_CONST              59 (<code object test_get_rate_fallback_str, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 423>)
+               476 MAKE_FUNCTION            0
+               478 STORE_NAME              70 (test_get_rate_fallback_str)
+   
+   433         480 LOAD_CONST              60 (<code object test_get_rate_fallback_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 433>)
+               482 MAKE_FUNCTION            0
+               484 STORE_NAME              71 (test_get_rate_fallback_int)
+   
+   443         486 LOAD_CONST              61 (<code object test_get_rate_fallback_rate, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 443>)
+               488 MAKE_FUNCTION            0
+               490 STORE_NAME              72 (test_get_rate_fallback_rate)
+   
+   453         492 LOAD_CONST              62 (<code object test_rate_init_default, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 453>)
+               494 MAKE_FUNCTION            0
+               496 STORE_NAME              73 (test_rate_init_default)
+   
+   463         498 LOAD_CONST              63 (<code object test_rate_init_timedelta, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 463>)
+               500 MAKE_FUNCTION            0
+               502 STORE_NAME              74 (test_rate_init_timedelta)
+   
+   473         504 LOAD_CONST              64 (<code object test_rate_nexttime, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 473>)
+               506 MAKE_FUNCTION            0
+               508 STORE_NAME              75 (test_rate_nexttime)
+   
+   481         510 LOAD_CONST              65 (<code object test_rate_nexttime_sync, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 481>)
+               512 MAKE_FUNCTION            0
+               514 STORE_NAME              76 (test_rate_nexttime_sync)
+   
+   489         516 LOAD_CONST              66 (<code object test_rate_nexttime_offset, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 489>)
+               518 MAKE_FUNCTION            0
+               520 STORE_NAME              77 (test_rate_nexttime_offset)
+   
+   497         522 LOAD_CONST              67 (<code object test_rate_nexttime_offset_sync, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 497>)
+               524 MAKE_FUNCTION            0
+               526 STORE_NAME              78 (test_rate_nexttime_offset_sync)
+   
+   505         528 LOAD_CONST              68 (<code object test_rate_nexttime_offset_sync2, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 505>)
+               530 MAKE_FUNCTION            0
+               532 STORE_NAME              79 (test_rate_nexttime_offset_sync2)
+   
+   513         534 LOAD_CONST              69 (<code object test_get_components, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 513>)
+               536 MAKE_FUNCTION            0
+               538 STORE_NAME              80 (test_get_components)
+   
+   521         540 LOAD_CONST              70 (<code object test_get_components_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 521>)
+               542 MAKE_FUNCTION            0
+               544 STORE_NAME              81 (test_get_components_proxy)
+   
+   529         546 LOAD_CONST              71 (<code object test_component_set, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 529>)
+               548 MAKE_FUNCTION            0
+               550 STORE_NAME              82 (test_component_set)
+   
+   537         552 LOAD_CONST              72 (<code object test_component_options, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 537>)
+               554 MAKE_FUNCTION            0
+               556 STORE_NAME              83 (test_component_options)
+   
+   547         558 LOAD_CONST              73 (<code object test_get_callback, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 547>)
+               560 MAKE_FUNCTION            0
+               562 STORE_NAME              84 (test_get_callback)
+   
+   557         564 LOAD_CONST              74 (<code object test_get_interpolation, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 557>)
+               566 MAKE_FUNCTION            0
+               568 STORE_NAME              85 (test_get_interpolation)
+   
+   567         570 LOAD_CONST              75 (<code object test_get_interpolation_proxy, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 567>)
+               572 MAKE_FUNCTION            0
+               574 STORE_NAME              86 (test_get_interpolation_proxy)
+   
+   577         576 LOAD_CONST              76 (<code object test_get_interpolation_loop, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 577>)
+               578 MAKE_FUNCTION            0
+               580 STORE_NAME              87 (test_get_interpolation_loop)
+   
+   587         582 LOAD_CONST              77 (<code object test_component_mixin, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 587>)
+               584 MAKE_FUNCTION            0
+               586 STORE_NAME              88 (test_component_mixin)
+   
+   599         588 LOAD_CONST              78 (<code object test_component_mixin_default, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 599>)
+               590 MAKE_FUNCTION            0
+               592 STORE_NAME              89 (test_component_mixin_default)
+   
+   610         594 LOAD_CONST              79 (<code object test_timespan_int, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 610>)
+               596 MAKE_FUNCTION            0
+               598 STORE_NAME              90 (test_timespan_int)
+   
+   619         600 LOAD_CONST              80 (<code object test_timespan_td, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 619>)
+               602 MAKE_FUNCTION            0
+               604 STORE_NAME              91 (test_timespan_td)
+   
+   628         606 LOAD_CONST              81 (<code object test_timespan_rd, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 628>)
+               608 MAKE_FUNCTION            0
+               610 STORE_NAME              92 (test_timespan_rd)
+   
+   637         612 LOAD_CONST              82 (<code object test_escape, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 637>)
+               614 MAKE_FUNCTION            0
+               616 STORE_NAME              93 (test_escape)
+               618 LOAD_CONST               2 (None)
+               620 RETURN_VALUE
    consts
       'Sapphire Unit Tests'
       0
       None
       ('relativedelta',)
       code
          argcount  : 0
@@ -470,14 +490,112 @@
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'Factory'
          firstlineno 15
          lnotab 0x0c010402
       'Factory'
       code
          argcount  : 0
+         nlocals   : 0
+         stacksize : 2
+         flags     : 0
+         code
+            0x8700970065005a0164005a0264015a0388006601640284085a04880078
+            015a055300
+                       0 MAKE_CELL                0 (__class__)
+         
+          21           2 RESUME                   0
+                       4 LOAD_NAME                0 (__name__)
+                       6 STORE_NAME               1 (__module__)
+                       8 LOAD_CONST               0 ('FactorySet')
+                      10 STORE_NAME               2 (__qualname__)
+         
+          22          12 LOAD_CONST               1 ('Test component set')
+                      14 STORE_NAME               3 (__doc__)
+         
+          24          16 LOAD_CLOSURE             0 (__class__)
+                      18 BUILD_TUPLE              1
+                      20 LOAD_CONST               2 (<code object __init__, file "/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py", line 24>)
+                      22 MAKE_FUNCTION            8 (closure)
+                      24 STORE_NAME               4 (__init__)
+                      26 LOAD_CLOSURE             0 (__class__)
+                      28 COPY                     1
+                      30 STORE_NAME               5 (__classcell__)
+                      32 RETURN_VALUE
+         consts
+            'FactorySet'
+            'Test component set'
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x950197000200740100000000000000000000a6000000ab000000000000
+                  0000006a010000000000000000640167017c01a201520069007c02a4018e
+                  0101007c006a020000000000000000a00300000000000000000000000000
+                  00000000000000640264037c006a0400000000000000009b009d02a60200
+                  00ab020000000000000000010064005300
+                             0 COPY_FREE_VARS           1
+               
+                24           2 RESUME                   0
+               
+                25           4 PUSH_NULL
+                             6 LOAD_GLOBAL              1 (NULL + super)
+                            18 PRECALL                  0
+                            22 CALL                     0
+                            32 LOAD_ATTR                1 (__init__)
+                            42 LOAD_CONST               1 ('component')
+                            44 BUILD_LIST               1
+                            46 LOAD_FAST                1 (p)
+                            48 LIST_EXTEND              1
+                            50 LIST_TO_TUPLE
+                            52 BUILD_MAP                0
+                            54 LOAD_FAST                2 (kw)
+                            56 DICT_MERGE               1
+                            58 CALL_FUNCTION_EX         1
+                            60 POP_TOP
+               
+                27          62 LOAD_FAST                0 (self)
+                            64 LOAD_ATTR                2 (config)
+                            74 LOAD_METHOD              3 (set)
+                            96 LOAD_CONST               2 ('setname')
+                            98 LOAD_CONST               3 ('setname.')
+                           100 LOAD_FAST                0 (self)
+                           102 LOAD_ATTR                4 (name)
+                           112 FORMAT_VALUE             0
+                           114 BUILD_STRING             2
+                           116 PRECALL                  2
+                           120 CALL                     2
+                           130 POP_TOP
+                           132 LOAD_CONST               0 (None)
+                           134 RETURN_VALUE
+               consts
+                  None
+                  'component'
+                  'setname'
+                  'setname.'
+               names      ('super', '__init__', 'config', 'set', 'name')
+               varnames   ('self', 'p', 'kw')
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
+               name       '__init__'
+               firstlineno 24
+               lnotab 0x04013a02
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__classcell__')
+         varnames   ()
+         freevars   ()
+         cellvars   ('__class__',)
+         filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
+         name       'FactorySet'
+         firstlineno 21
+         lnotab 0x0c010402
+      'FactorySet'
+      code
+         argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d0069007c0064013c00000064027c006401190000
             0000000000000064033c0000007c00a00200000000000000000000000000
@@ -490,43 +608,43 @@
             07000000000000000000006a0800000000000000007c01a6010000ab0100
             000000000000006e0164067407000000000000000000006a080000000000
             0000007c02a6010000ab01000000000000000064079c027a0600007d0464
             0864097c0469017a0600007d057413000000000000000000007407000000
             000000000000006a0a00000000000000007c05a6010000ab010000000000
             000000a6010000ab0100000000000000008201640078017d037d02640053
             00
-          21           0 RESUME                   0
+          30           0 RESUME                   0
          
-          22           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          31           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          23          40 BUILD_MAP                0
+          32          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          24          50 LOAD_CONST               2 ('value')
+          33          50 LOAD_CONST               2 ('value')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('option')
                       68 STORE_SUBSCR
          
-          26          72 LOAD_FAST                0 (config)
+          35          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('option')
                      100 PRECALL                  2
                      104 CALL                     2
                      114 STORE_FAST               1 (result)
          
-          27         116 LOAD_CONST               2 ('value')
+          36         116 LOAD_CONST               2 ('value')
                      118 STORE_FAST               2 (@py_assert2)
                      120 LOAD_FAST                1 (result)
                      122 LOAD_FAST                2 (@py_assert2)
                      124 COMPARE_OP               2 (==)
                      130 STORE_FAST               3 (@py_assert1)
                      132 LOAD_FAST                3 (@py_assert1)
                      134 POP_JUMP_FORWARD_IF_TRUE   151 (to 438)
@@ -604,15 +722,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_parser'
-         firstlineno 21
+         firstlineno 30
          lnotab 0x020126010a0116022c01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -627,42 +745,42 @@
             00ab01000000000000000072147405000000000000000000006a07000000
             00000000007c01a6010000ab0100000000000000006e0164067405000000
             000000000000006a0700000000000000007c02a6010000ab010000000000
             00000064079c027a0600007d04640864097c0469017a0600007d05741100
             0000000000000000007405000000000000000000006a0900000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-          29           0 RESUME                   0
+          38           0 RESUME                   0
          
-          30           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          39           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          31          40 BUILD_MAP                0
+          40          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          32          50 LOAD_CONST               2 ('value')
+          41          50 LOAD_CONST               2 ('value')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('option')
                       68 STORE_SUBSCR
          
-          34          72 LOAD_FAST                0 (config)
+          43          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_CONST               3 ('option')
                       88 BINARY_SUBSCR
                       98 STORE_FAST               1 (result)
          
-          35         100 LOAD_CONST               2 ('value')
+          44         100 LOAD_CONST               2 ('value')
                      102 STORE_FAST               2 (@py_assert2)
                      104 LOAD_FAST                1 (result)
                      106 LOAD_FAST                2 (@py_assert2)
                      108 COMPARE_OP               2 (==)
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -740,15 +858,15 @@
             'py5'
          names      ('sapphire', 'Parser', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_proxy_dict'
-         firstlineno 29
+         firstlineno 38
          lnotab 0x020126010a0116021c01
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
@@ -756,43 +874,43 @@
             0000000000000000007d007405000000000000000000006a030000000000
             0000007408000000000000000000006a050000000000000000a6010000ab
             010000000000000000350001007c00a00600000000000000000000000000
             00000000000000640164027400000000000000000000006a070000000000
             000000ac03a6030000ab0300000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-          37           0 RESUME                   0
+          46           0 RESUME                   0
          
-          38           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          47           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          40          40 LOAD_GLOBAL              5 (NULL + pytest)
+          49          40 LOAD_GLOBAL              5 (NULL + pytest)
                       52 LOAD_ATTR                3 (raises)
                       62 LOAD_GLOBAL              8 (configparser)
                       74 LOAD_ATTR                5 (NoSectionError)
                       84 PRECALL                  1
                       88 CALL                     1
                       98 BEFORE_WITH
                      100 POP_TOP
          
-          41         102 LOAD_FAST                0 (config)
+          50         102 LOAD_FAST                0 (config)
                      104 LOAD_METHOD              6 (get)
                      126 LOAD_CONST               1 ('section')
                      128 LOAD_CONST               2 ('missing')
                      130 LOAD_GLOBAL              0 (sapphire)
                      142 LOAD_ATTR                7 (UNSET)
                      152 KW_NAMES                 3
                      154 PRECALL                  3
                      158 CALL                     3
                      168 POP_TOP
          
-          40         170 LOAD_CONST               0 (None)
+          49         170 LOAD_CONST               0 (None)
                      172 LOAD_CONST               0 (None)
                      174 LOAD_CONST               0 (None)
                      176 PRECALL                  2
                      180 CALL                     2
                      190 POP_TOP
                      192 LOAD_CONST               0 (None)
                      194 RETURN_VALUE
@@ -820,15 +938,15 @@
             ('fallback',)
          names      ('sapphire', 'Parser', 'pytest', 'raises', 'configparser', 'NoSectionError', 'get', 'UNSET')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_missing_section'
-         firstlineno 37
+         firstlineno 46
          lnotab 0x020126023e0144ff
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
@@ -836,48 +954,48 @@
             0000000000000000007d0069007c0064013c000000740500000000000000
             0000006a0300000000000000007408000000000000000000006a05000000
             0000000000a6010000ab010000000000000000350001007c00a006000000
             000000000000000000000000000000000064016402740000000000000000
             0000006a070000000000000000ac03a6030000ab03000000000000000001
             00640064006400a6020000ab020000000000000000010064005300230031
             0073047702780359007701010059000100010064005300
-          43           0 RESUME                   0
+          52           0 RESUME                   0
          
-          44           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          53           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          45          40 BUILD_MAP                0
+          54          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          47          50 LOAD_GLOBAL              5 (NULL + pytest)
+          56          50 LOAD_GLOBAL              5 (NULL + pytest)
                       62 LOAD_ATTR                3 (raises)
                       72 LOAD_GLOBAL              8 (configparser)
                       84 LOAD_ATTR                5 (NoOptionError)
                       94 PRECALL                  1
                       98 CALL                     1
                      108 BEFORE_WITH
                      110 POP_TOP
          
-          48         112 LOAD_FAST                0 (config)
+          57         112 LOAD_FAST                0 (config)
                      114 LOAD_METHOD              6 (get)
                      136 LOAD_CONST               1 ('section')
                      138 LOAD_CONST               2 ('missing')
                      140 LOAD_GLOBAL              0 (sapphire)
                      152 LOAD_ATTR                7 (UNSET)
                      162 KW_NAMES                 3
                      164 PRECALL                  3
                      168 CALL                     3
                      178 POP_TOP
          
-          47         180 LOAD_CONST               0 (None)
+          56         180 LOAD_CONST               0 (None)
                      182 LOAD_CONST               0 (None)
                      184 LOAD_CONST               0 (None)
                      186 PRECALL                  2
                      190 CALL                     2
                      200 POP_TOP
                      202 LOAD_CONST               0 (None)
                      204 RETURN_VALUE
@@ -905,15 +1023,15 @@
             ('fallback',)
          names      ('sapphire', 'Parser', 'pytest', 'raises', 'configparser', 'NoOptionError', 'get', 'UNSET')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_missing_option'
-         firstlineno 43
+         firstlineno 52
          lnotab 0x020126010a023e0144ff
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -929,44 +1047,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016406740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             079c027a0600007d04640864097c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-          50           0 RESUME                   0
+          59           0 RESUME                   0
          
-          51           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          60           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          52          40 BUILD_MAP                0
+          61          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          53          50 LOAD_CONST               2 ('value')
+          62          50 LOAD_CONST               2 ('value')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('option')
                       68 STORE_SUBSCR
          
-          55          72 LOAD_FAST                0 (config)
+          64          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get)
                      108 LOAD_CONST               3 ('option')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-          56         126 LOAD_CONST               2 ('value')
+          65         126 LOAD_CONST               2 ('value')
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -1044,15 +1162,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_proxy_func'
-         firstlineno 50
+         firstlineno 59
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1068,44 +1186,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016407740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             089c027a0600007d046409640a7c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-          58           0 RESUME                   0
+          67           0 RESUME                   0
          
-          59           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          68           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          60          40 BUILD_MAP                0
+          69          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          61          50 LOAD_CONST               2 ('1')
+          70          50 LOAD_CONST               2 ('1')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('int')
                       68 STORE_SUBSCR
          
-          63          72 LOAD_FAST                0 (config)
+          72          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_int)
                      108 LOAD_CONST               3 ('int')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-          64         126 LOAD_CONST               4 (1)
+          73         126 LOAD_CONST               4 (1)
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -1184,15 +1302,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int'
-         firstlineno 58
+         firstlineno 67
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1208,44 +1326,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016407740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             089c027a0600007d046409640a7c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-          66           0 RESUME                   0
+          75           0 RESUME                   0
          
-          67           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          76           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          68          40 BUILD_MAP                0
+          77          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          69          50 LOAD_CONST               2 ('0x10')
+          78          50 LOAD_CONST               2 ('0x10')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('int')
                       68 STORE_SUBSCR
          
-          71          72 LOAD_FAST                0 (config)
+          80          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_int)
                      108 LOAD_CONST               3 ('int')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-          72         126 LOAD_CONST               4 (16)
+          81         126 LOAD_CONST               4 (16)
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -1324,15 +1442,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int_hex'
-         firstlineno 66
+         firstlineno 75
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1348,46 +1466,46 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164097407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             000000640a9c027a0600007d04640b640c7c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-          74           0 RESUME                   0
+          83           0 RESUME                   0
          
-          75           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          84           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          76          40 BUILD_MAP                0
+          85          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          77          50 LOAD_CONST               2 ('044')
+          86          50 LOAD_CONST               2 ('044')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('int')
                       68 STORE_SUBSCR
          
-          79          72 LOAD_FAST                0 (config)
+          88          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_int)
                      108 LOAD_CONST               3 ('int')
                      110 LOAD_CONST               4 (8)
                      112 KW_NAMES                 5
                      114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (result)
          
-          80         130 LOAD_CONST               6 (36)
+          89         130 LOAD_CONST               6 (36)
                      132 STORE_FAST               2 (@py_assert2)
                      134 LOAD_FAST                1 (result)
                      136 LOAD_FAST                2 (@py_assert2)
                      138 COMPARE_OP               2 (==)
                      144 STORE_FAST               3 (@py_assert1)
                      146 LOAD_FAST                3 (@py_assert1)
                      148 POP_JUMP_FORWARD_IF_TRUE   151 (to 452)
@@ -1468,15 +1586,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int_base'
-         firstlineno 74
+         firstlineno 83
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1491,37 +1609,37 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164057407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064069c027a0600007d04640764087c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-          82           0 RESUME                   0
+          91           0 RESUME                   0
          
-          83           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          92           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          84          40 BUILD_MAP                0
+          93          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          86          50 LOAD_FAST                0 (config)
+          95          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_int)
                       86 LOAD_CONST               2 ('missing')
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (result)
          
-          87         104 LOAD_CONST               0 (None)
+          96         104 LOAD_CONST               0 (None)
                      106 STORE_FAST               2 (@py_assert2)
                      108 LOAD_FAST                1 (result)
                      110 LOAD_FAST                2 (@py_assert2)
                      112 IS_OP                    0
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -1598,15 +1716,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int_fallback_none'
-         firstlineno 82
+         firstlineno 91
          lnotab 0x020126010a023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1621,39 +1739,39 @@
             0000007c01a6010000ab0100000000000000007214740700000000000000
             0000006a0800000000000000007c01a6010000ab0100000000000000006e
             0164087407000000000000000000006a0800000000000000007c02a60100
             00ab01000000000000000064099c027a0600007d04640a640b7c0469017a
             0600007d057413000000000000000000007407000000000000000000006a
             0a00000000000000007c05a6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d037d0264005300
-          89           0 RESUME                   0
+          98           0 RESUME                   0
          
-          90           2 LOAD_GLOBAL              1 (NULL + sapphire)
+          99           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          91          40 BUILD_MAP                0
+         100          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-          93          50 LOAD_FAST                0 (config)
+         102          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_int)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('1')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-          94         108 LOAD_CONST               5 (1)
+         103         108 LOAD_CONST               5 (1)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 COMPARE_OP               2 (==)
                      122 STORE_FAST               3 (@py_assert1)
                      124 LOAD_FAST                3 (@py_assert1)
                      126 POP_JUMP_FORWARD_IF_TRUE   151 (to 430)
@@ -1733,15 +1851,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int_fallback_str'
-         firstlineno 89
+         firstlineno 98
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1756,39 +1874,39 @@
             0000007c01a6010000ab0100000000000000007214740700000000000000
             0000006a0800000000000000007c01a6010000ab0100000000000000006e
             0164077407000000000000000000006a0800000000000000007c02a60100
             00ab01000000000000000064089c027a0600007d046409640a7c0469017a
             0600007d057413000000000000000000007407000000000000000000006a
             0a00000000000000007c05a6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d037d0264005300
-          96           0 RESUME                   0
+         105           0 RESUME                   0
          
-          97           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         106           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-          98          40 BUILD_MAP                0
+         107          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         100          50 LOAD_FAST                0 (config)
+         109          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_int)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (1)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         101         108 LOAD_CONST               3 (1)
+         110         108 LOAD_CONST               3 (1)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 COMPARE_OP               2 (==)
                      122 STORE_FAST               3 (@py_assert1)
                      124 LOAD_FAST                3 (@py_assert1)
                      126 POP_JUMP_FORWARD_IF_TRUE   151 (to 430)
@@ -1867,15 +1985,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_int_fallback_int'
-         firstlineno 96
+         firstlineno 105
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -1891,44 +2009,44 @@
             00000072147407000000000000000000006a0800000000000000007c01a6
             010000ab0100000000000000006e0164077407000000000000000000006a
             0800000000000000007c02a6010000ab01000000000000000064089c027a
             0600007d046409640a7c0469017a0600007d057413000000000000000000
             007407000000000000000000006a0a00000000000000007c05a6010000ab
             010000000000000000a6010000ab0100000000000000008201640078017d
             037d0264005300
-         103           0 RESUME                   0
+         112           0 RESUME                   0
          
-         104           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         113           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         105          40 BUILD_MAP                0
+         114          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         106          50 LOAD_CONST               2 ('true')
+         115          50 LOAD_CONST               2 ('true')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('boolean')
                       68 STORE_SUBSCR
          
-         108          72 LOAD_FAST                0 (config)
+         117          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_boolean)
                      108 LOAD_CONST               3 ('boolean')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         109         126 LOAD_CONST               4 (True)
+         118         126 LOAD_CONST               4 (True)
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 IS_OP                    0
                      136 STORE_FAST               3 (@py_assert1)
                      138 LOAD_FAST                3 (@py_assert1)
                      140 POP_JUMP_FORWARD_IF_TRUE   151 (to 444)
@@ -2007,15 +2125,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean'
-         firstlineno 103
+         firstlineno 112
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2030,37 +2148,37 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164057407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064069c027a0600007d04640764087c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         111           0 RESUME                   0
+         120           0 RESUME                   0
          
-         112           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         121           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         113          40 BUILD_MAP                0
+         122          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         115          50 LOAD_FAST                0 (config)
+         124          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (result)
          
-         116         104 LOAD_CONST               0 (None)
+         125         104 LOAD_CONST               0 (None)
                      106 STORE_FAST               2 (@py_assert2)
                      108 LOAD_FAST                1 (result)
                      110 LOAD_FAST                2 (@py_assert2)
                      112 IS_OP                    0
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -2137,15 +2255,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_none'
-         firstlineno 111
+         firstlineno 120
          lnotab 0x020126010a023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2160,39 +2278,39 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640874
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             0000000000000064099c027a0600007d04640a640b7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         118           0 RESUME                   0
+         127           0 RESUME                   0
          
-         119           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         128           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         120          40 BUILD_MAP                0
+         129          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         122          50 LOAD_FAST                0 (config)
+         131          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('true')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         123         108 LOAD_CONST               5 (True)
+         132         108 LOAD_CONST               5 (True)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 IS_OP                    0
                      118 STORE_FAST               3 (@py_assert1)
                      120 LOAD_FAST                3 (@py_assert1)
                      122 POP_JUMP_FORWARD_IF_TRUE   151 (to 426)
@@ -2272,15 +2390,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_str'
-         firstlineno 118
+         firstlineno 127
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2295,39 +2413,39 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640774
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             0000000000000064089c027a0600007d046409640a7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         125           0 RESUME                   0
+         134           0 RESUME                   0
          
-         126           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         135           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         127          40 BUILD_MAP                0
+         136          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         129          50 LOAD_FAST                0 (config)
+         138          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (True)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         130         108 LOAD_CONST               3 (True)
+         139         108 LOAD_CONST               3 (True)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 IS_OP                    0
                      118 STORE_FAST               3 (@py_assert1)
                      120 LOAD_FAST                3 (@py_assert1)
                      122 POP_JUMP_FORWARD_IF_TRUE   151 (to 426)
@@ -2406,15 +2524,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_bool_t'
-         firstlineno 125
+         firstlineno 134
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2429,39 +2547,39 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640774
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             0000000000000064089c027a0600007d046409640a7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         132           0 RESUME                   0
+         141           0 RESUME                   0
          
-         133           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         142           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         134          40 BUILD_MAP                0
+         143          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         136          50 LOAD_FAST                0 (config)
+         145          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (False)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         137         108 LOAD_CONST               3 (False)
+         146         108 LOAD_CONST               3 (False)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 IS_OP                    0
                      118 STORE_FAST               3 (@py_assert1)
                      120 LOAD_FAST                3 (@py_assert1)
                      122 POP_JUMP_FORWARD_IF_TRUE   151 (to 426)
@@ -2540,15 +2658,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_bool_f'
-         firstlineno 132
+         firstlineno 141
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2563,39 +2681,39 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640874
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             0000000000000064099c027a0600007d04640a640b7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         139           0 RESUME                   0
+         148           0 RESUME                   0
          
-         140           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         149           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         141          40 BUILD_MAP                0
+         150          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         143          50 LOAD_FAST                0 (config)
+         152          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (1)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         144         108 LOAD_CONST               5 (True)
+         153         108 LOAD_CONST               5 (True)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 IS_OP                    0
                      118 STORE_FAST               3 (@py_assert1)
                      120 LOAD_FAST                3 (@py_assert1)
                      122 POP_JUMP_FORWARD_IF_TRUE   151 (to 426)
@@ -2675,15 +2793,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_int_t'
-         firstlineno 139
+         firstlineno 148
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2698,39 +2816,39 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640874
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             0000000000000064099c027a0600007d04640a640b7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         146           0 RESUME                   0
+         155           0 RESUME                   0
          
-         147           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         156           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         148          40 BUILD_MAP                0
+         157          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         150          50 LOAD_FAST                0 (config)
+         159          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_boolean)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (0)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         151         108 LOAD_CONST               5 (False)
+         160         108 LOAD_CONST               5 (False)
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 IS_OP                    0
                      118 STORE_FAST               3 (@py_assert1)
                      120 LOAD_FAST                3 (@py_assert1)
                      122 POP_JUMP_FORWARD_IF_TRUE   151 (to 426)
@@ -2810,15 +2928,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_boolean', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_boolean_fallback_int_f'
-         firstlineno 146
+         firstlineno 155
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2834,43 +2952,43 @@
             0072147407000000000000000000006a0800000000000000007c01a60100
             00ab0100000000000000006e0164077407000000000000000000006a0800
             000000000000007c02a6010000ab01000000000000000064089c027a0600
             007d046409640a7c0469017a0600007d0574130000000000000000000074
             07000000000000000000006a0a00000000000000007c05a6010000ab0100
             00000000000000a6010000ab0100000000000000008201640078017d037d
             0264005300
-         153           0 RESUME                   0
+         162           0 RESUME                   0
          
-         154           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         163           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         155          40 BUILD_MAP                0
+         164          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         156          50 LOAD_CONST               2 ('a b c')
+         165          50 LOAD_CONST               2 ('a b c')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         158          72 LOAD_FAST                0 (config)
+         167          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get_list)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('list')
                      100 PRECALL                  2
                      104 CALL                     2
                      114 STORE_FAST               1 (result)
          
-         159         116 BUILD_LIST               0
+         168         116 BUILD_LIST               0
                      118 LOAD_CONST               4 (('a', 'b', 'c'))
                      120 LIST_EXTEND              1
                      122 STORE_FAST               2 (@py_assert2)
                      124 LOAD_FAST                1 (result)
                      126 LOAD_FAST                2 (@py_assert2)
                      128 COMPARE_OP               2 (==)
                      134 STORE_FAST               3 (@py_assert1)
@@ -2951,15 +3069,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_parser'
-         firstlineno 153
+         firstlineno 162
          lnotab 0x020126010a0116022c01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2975,44 +3093,44 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164077407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064089c027a0600007d046409640a7c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         161           0 RESUME                   0
+         170           0 RESUME                   0
          
-         162           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         171           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         163          40 BUILD_MAP                0
+         172          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         164          50 LOAD_CONST               2 ('a b c')
+         173          50 LOAD_CONST               2 ('a b c')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         166          72 LOAD_FAST                0 (config)
+         175          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_list)
                      108 LOAD_CONST               3 ('list')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         167         126 BUILD_LIST               0
+         176         126 BUILD_LIST               0
                      128 LOAD_CONST               4 (('a', 'b', 'c'))
                      130 LIST_EXTEND              1
                      132 STORE_FAST               2 (@py_assert2)
                      134 LOAD_FAST                1 (result)
                      136 LOAD_FAST                2 (@py_assert2)
                      138 COMPARE_OP               2 (==)
                      144 STORE_FAST               3 (@py_assert1)
@@ -3093,15 +3211,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_proxy_func'
-         firstlineno 161
+         firstlineno 170
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3117,45 +3235,45 @@
             01a6010000ab01000000000000000072147409000000000000000000006a
             0900000000000000007c01a6010000ab0100000000000000006e01640874
             09000000000000000000006a0900000000000000007c02a6010000ab0100
             0000000000000064099c027a0600007d04640a640b7c0469017a0600007d
             057415000000000000000000007409000000000000000000006a0b000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         169           0 RESUME                   0
+         178           0 RESUME                   0
          
-         170           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         179           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         171          40 BUILD_MAP                0
+         180          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         172          50 LOAD_CONST               2 ('1 2 3')
+         181          50 LOAD_CONST               2 ('1 2 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         174          72 LOAD_FAST                0 (config)
+         183          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get_list)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('list')
                      100 LOAD_GLOBAL              6 (int)
                      112 KW_NAMES                 4
                      114 PRECALL                  3
                      118 CALL                     3
                      128 STORE_FAST               1 (result)
          
-         175         130 BUILD_LIST               0
+         184         130 BUILD_LIST               0
                      132 LOAD_CONST               5 ((1, 2, 3))
                      134 LIST_EXTEND              1
                      136 STORE_FAST               2 (@py_assert2)
                      138 LOAD_FAST                1 (result)
                      140 LOAD_FAST                2 (@py_assert2)
                      142 COMPARE_OP               2 (==)
                      148 STORE_FAST               3 (@py_assert1)
@@ -3237,15 +3355,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', 'int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_conv_parser'
-         firstlineno 169
+         firstlineno 178
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3261,46 +3379,46 @@
             0800000000000000007c01a6010000ab0100000000000000007214740900
             0000000000000000006a0900000000000000007c01a6010000ab01000000
             00000000006e0164087409000000000000000000006a0900000000000000
             007c02a6010000ab01000000000000000064099c027a0600007d04640a64
             0b7c0469017a0600007d0574150000000000000000000074090000000000
             00000000006a0b00000000000000007c05a6010000ab0100000000000000
             00a6010000ab0100000000000000008201640078017d037d0264005300
-         177           0 RESUME                   0
+         186           0 RESUME                   0
          
-         178           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         187           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         179          40 BUILD_MAP                0
+         188          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         180          50 LOAD_CONST               2 ('1 2 3')
+         189          50 LOAD_CONST               2 ('1 2 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         182          72 LOAD_FAST                0 (config)
+         191          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_list)
                      108 LOAD_CONST               3 ('list')
                      110 LOAD_GLOBAL              6 (int)
                      122 KW_NAMES                 4
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_FAST               1 (result)
          
-         183         140 BUILD_LIST               0
+         192         140 BUILD_LIST               0
                      142 LOAD_CONST               5 ((1, 2, 3))
                      144 LIST_EXTEND              1
                      146 STORE_FAST               2 (@py_assert2)
                      148 LOAD_FAST                1 (result)
                      150 LOAD_FAST                2 (@py_assert2)
                      152 COMPARE_OP               2 (==)
                      158 STORE_FAST               3 (@py_assert1)
@@ -3382,15 +3500,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', 'int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_conv_proxy'
-         firstlineno 177
+         firstlineno 186
          lnotab 0x020126010a0116024401
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3406,46 +3524,46 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640974
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             00000000000000640a9c027a0600007d04640b640c7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         185           0 RESUME                   0
+         194           0 RESUME                   0
          
-         186           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         195           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         187          40 BUILD_MAP                0
+         196          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         188          50 LOAD_CONST               2 ('1, 2, 3')
+         197          50 LOAD_CONST               2 ('1, 2, 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         190          72 LOAD_FAST                0 (config)
+         199          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_list)
                      108 LOAD_CONST               3 ('list')
                      110 LOAD_CONST               4 (',')
                      112 KW_NAMES                 5
                      114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (result)
          
-         191         130 BUILD_LIST               0
+         200         130 BUILD_LIST               0
                      132 LOAD_CONST               6 (('1', '2', '3'))
                      134 LIST_EXTEND              1
                      136 STORE_FAST               2 (@py_assert2)
                      138 LOAD_FAST                1 (result)
                      140 LOAD_FAST                2 (@py_assert2)
                      142 COMPARE_OP               2 (==)
                      148 STORE_FAST               3 (@py_assert1)
@@ -3528,15 +3646,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_sep'
-         firstlineno 185
+         firstlineno 194
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3553,47 +3671,47 @@
             09000000000000000000006a0900000000000000007c01a6010000ab0100
             000000000000006e0164097409000000000000000000006a090000000000
             0000007c02a6010000ab010000000000000000640a9c027a0600007d0464
             0b640c7c0469017a0600007d057415000000000000000000007409000000
             000000000000006a0b00000000000000007c05a6010000ab010000000000
             000000a6010000ab0100000000000000008201640078017d037d02640053
             00
-         193           0 RESUME                   0
+         202           0 RESUME                   0
          
-         194           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         203           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         195          40 BUILD_MAP                0
+         204          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         196          50 LOAD_CONST               2 ('1, 2, 3')
+         205          50 LOAD_CONST               2 ('1, 2, 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         198          72 LOAD_FAST                0 (config)
+         207          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_list)
                      108 LOAD_CONST               3 ('list')
                      110 LOAD_CONST               4 (',')
                      112 LOAD_GLOBAL              6 (int)
                      124 KW_NAMES                 5
                      126 PRECALL                  3
                      130 CALL                     3
                      140 STORE_FAST               1 (result)
          
-         199         142 BUILD_LIST               0
+         208         142 BUILD_LIST               0
                      144 LOAD_CONST               6 ((1, 2, 3))
                      146 LIST_EXTEND              1
                      148 STORE_FAST               2 (@py_assert2)
                      150 LOAD_FAST                1 (result)
                      152 LOAD_FAST                2 (@py_assert2)
                      154 COMPARE_OP               2 (==)
                      160 STORE_FAST               3 (@py_assert1)
@@ -3676,15 +3794,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', 'int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_sep_conv'
-         firstlineno 193
+         firstlineno 202
          lnotab 0x020126010a0116024601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3700,44 +3818,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016407740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             089c027a0600007d046409640a7c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-         201           0 RESUME                   0
+         210           0 RESUME                   0
          
-         202           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         211           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         203          40 BUILD_MAP                0
+         212          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         204          50 LOAD_CONST               2 ('1, 2, 3')
+         213          50 LOAD_CONST               2 ('1, 2, 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('list')
                       68 STORE_SUBSCR
          
-         206          72 LOAD_FAST                0 (config)
+         215          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_list)
                      108 LOAD_CONST               4 ('missing')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         207         126 BUILD_LIST               0
+         216         126 BUILD_LIST               0
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -3816,15 +3934,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_fallback_none'
-         firstlineno 201
+         firstlineno 210
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -3839,39 +3957,39 @@
             000000000000007c01a6010000ab01000000000000000072147407000000
             000000000000006a0800000000000000007c01a6010000ab010000000000
             0000006e0164087407000000000000000000006a0800000000000000007c
             02a6010000ab01000000000000000064099c027a0600007d04640a640b7c
             0469017a0600007d05741300000000000000000000740700000000000000
             0000006a0a00000000000000007c05a6010000ab010000000000000000a6
             010000ab0100000000000000008201640078017d037d0264005300
-         209           0 RESUME                   0
+         218           0 RESUME                   0
          
-         210           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         219           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         211          40 BUILD_MAP                0
+         220          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         213          50 LOAD_FAST                0 (config)
+         222          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_list)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('a b c')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         214         108 BUILD_LIST               0
+         223         108 BUILD_LIST               0
                      110 LOAD_CONST               5 (('a', 'b', 'c'))
                      112 LIST_EXTEND              1
                      114 STORE_FAST               2 (@py_assert2)
                      116 LOAD_FAST                1 (result)
                      118 LOAD_FAST                2 (@py_assert2)
                      120 COMPARE_OP               2 (==)
                      126 STORE_FAST               3 (@py_assert1)
@@ -3953,55 +4071,55 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_fallback_str'
-         firstlineno 209
+         firstlineno 218
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d007405000000000000000000006a030000000000
             000000740800000000000000000000a6010000ab01000000000000000035
             0001007c00640119000000000000000000a0050000000000000000000000
             0000000000000000006402a6010000ab0100000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         216           0 RESUME                   0
+         225           0 RESUME                   0
          
-         217           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         226           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         219          40 LOAD_GLOBAL              5 (NULL + pytest)
+         228          40 LOAD_GLOBAL              5 (NULL + pytest)
                       52 LOAD_ATTR                3 (raises)
                       62 LOAD_GLOBAL              8 (KeyError)
                       74 PRECALL                  1
                       78 CALL                     1
                       88 BEFORE_WITH
                       90 POP_TOP
          
-         220          92 LOAD_FAST                0 (config)
+         229          92 LOAD_FAST                0 (config)
                       94 LOAD_CONST               1 ('section')
                       96 BINARY_SUBSCR
                      106 LOAD_METHOD              5 (get_list)
                      128 LOAD_CONST               2 ('missing')
                      130 PRECALL                  1
                      134 CALL                     1
                      144 POP_TOP
          
-         219         146 LOAD_CONST               0 (None)
+         228         146 LOAD_CONST               0 (None)
                      148 LOAD_CONST               0 (None)
                      150 LOAD_CONST               0 (None)
                      152 PRECALL                  2
                      156 CALL                     2
                      166 POP_TOP
                      168 LOAD_CONST               0 (None)
                      170 RETURN_VALUE
@@ -4028,15 +4146,15 @@
             'missing'
          names      ('sapphire', 'Parser', 'pytest', 'raises', 'KeyError', 'get_list')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_no_section'
-         firstlineno 216
+         firstlineno 225
          lnotab 0x02012602340136ff
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
@@ -4044,47 +4162,47 @@
             0000000000000000007d0069007c0064013c000000740500000000000000
             0000006a030000000000000000740800000000000000000000a6010000ab
             010000000000000000350001007c00640119000000000000000000a00500
             0000000000000000000000000000000000000064026403ac04a6020000ab
             0200000000000000000100640064006400a6020000ab0200000000000000
             000100640053002300310073047702780359007701010059000100010064
             005300
-         222           0 RESUME                   0
+         231           0 RESUME                   0
          
-         223           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         232           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         224          40 BUILD_MAP                0
+         233          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         226          50 LOAD_GLOBAL              5 (NULL + pytest)
+         235          50 LOAD_GLOBAL              5 (NULL + pytest)
                       62 LOAD_ATTR                3 (raises)
                       72 LOAD_GLOBAL              8 (AttributeError)
                       84 PRECALL                  1
                       88 CALL                     1
                       98 BEFORE_WITH
                      100 POP_TOP
          
-         227         102 LOAD_FAST                0 (config)
+         236         102 LOAD_FAST                0 (config)
                      104 LOAD_CONST               1 ('section')
                      106 BINARY_SUBSCR
                      116 LOAD_METHOD              5 (get_list)
                      138 LOAD_CONST               2 ('missing')
                      140 LOAD_CONST               3 (1)
                      142 KW_NAMES                 4
                      144 PRECALL                  2
                      148 CALL                     2
                      158 POP_TOP
          
-         226         160 LOAD_CONST               0 (None)
+         235         160 LOAD_CONST               0 (None)
                      162 LOAD_CONST               0 (None)
                      164 LOAD_CONST               0 (None)
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_TOP
                      182 LOAD_CONST               0 (None)
                      184 RETURN_VALUE
@@ -4113,15 +4231,15 @@
             ('fallback',)
          names      ('sapphire', 'Parser', 'pytest', 'raises', 'AttributeError', 'get_list')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_fallback_type_error'
-         firstlineno 222
+         firstlineno 231
          lnotab 0x020126010a0234013aff
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4136,39 +4254,39 @@
             0000007c01a6010000ab0100000000000000007214740700000000000000
             0000006a0800000000000000007c01a6010000ab0100000000000000006e
             0164077407000000000000000000006a0800000000000000007c02a60100
             00ab01000000000000000064089c027a0600007d046409640a7c0469017a
             0600007d057413000000000000000000007407000000000000000000006a
             0a00000000000000007c05a6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d037d0264005300
-         229           0 RESUME                   0
+         238           0 RESUME                   0
          
-         230           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         239           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         231          40 BUILD_MAP                0
+         240          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         233          50 LOAD_FAST                0 (config)
+         242          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_list)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         234         108 BUILD_LIST               0
+         243         108 BUILD_LIST               0
                      110 STORE_FAST               2 (@py_assert2)
                      112 LOAD_FAST                1 (result)
                      114 LOAD_FAST                2 (@py_assert2)
                      116 COMPARE_OP               2 (==)
                      122 STORE_FAST               3 (@py_assert1)
                      124 LOAD_FAST                3 (@py_assert1)
                      126 POP_JUMP_FORWARD_IF_TRUE   151 (to 430)
@@ -4247,15 +4365,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_fallback_empty_str'
-         firstlineno 229
+         firstlineno 238
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4271,41 +4389,41 @@
             07000000000000000000006a0800000000000000007c01a6010000ab0100
             000000000000006e0164077407000000000000000000006a080000000000
             0000007c02a6010000ab01000000000000000064089c027a0600007d0464
             09640a7c0469017a0600007d057413000000000000000000007407000000
             000000000000006a0a00000000000000007c05a6010000ab010000000000
             000000a6010000ab0100000000000000008201640078017d037d02640053
             00
-         236           0 RESUME                   0
+         245           0 RESUME                   0
          
-         237           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         246           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         238          40 BUILD_MAP                0
+         247          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         240          50 LOAD_FAST                0 (config)
+         249          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_list)
                       86 LOAD_CONST               2 ('missing')
                       88 BUILD_LIST               0
                       90 LOAD_CONST               3 ((1, 2, 3))
                       92 LIST_EXTEND              1
                       94 KW_NAMES                 4
                       96 PRECALL                  2
                      100 CALL                     2
                      110 STORE_FAST               1 (result)
          
-         241         112 BUILD_LIST               0
+         250         112 BUILD_LIST               0
                      114 LOAD_CONST               3 ((1, 2, 3))
                      116 LIST_EXTEND              1
                      118 STORE_FAST               2 (@py_assert2)
                      120 LOAD_FAST                1 (result)
                      122 LOAD_FAST                2 (@py_assert2)
                      124 COMPARE_OP               2 (==)
                      130 STORE_FAST               3 (@py_assert1)
@@ -4386,15 +4504,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_list', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_list_fallback_list'
-         firstlineno 236
+         firstlineno 245
          lnotab 0x020126010a023e01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4410,43 +4528,43 @@
             0072147407000000000000000000006a0800000000000000007c01a60100
             00ab0100000000000000006e0164077407000000000000000000006a0800
             000000000000007c02a6010000ab01000000000000000064089c027a0600
             007d046409640a7c0469017a0600007d0574130000000000000000000074
             07000000000000000000006a0a00000000000000007c05a6010000ab0100
             00000000000000a6010000ab0100000000000000008201640078017d037d
             0264005300
-         243           0 RESUME                   0
+         252           0 RESUME                   0
          
-         244           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         253           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         245          40 BUILD_MAP                0
+         254          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         246          50 LOAD_CONST               2 ('a b c c')
+         255          50 LOAD_CONST               2 ('a b c c')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('set')
                       68 STORE_SUBSCR
          
-         248          72 LOAD_FAST                0 (config)
+         257          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get_set)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('set')
                      100 PRECALL                  2
                      104 CALL                     2
                      114 STORE_FAST               1 (result)
          
-         249         116 BUILD_SET                0
+         258         116 BUILD_SET                0
                      118 LOAD_CONST               4 (frozenset({'c', 'a', 'b'}))
                      120 SET_UPDATE               1
                      122 STORE_FAST               2 (@py_assert2)
                      124 LOAD_FAST                1 (result)
                      126 LOAD_FAST                2 (@py_assert2)
                      128 COMPARE_OP               2 (==)
                      134 STORE_FAST               3 (@py_assert1)
@@ -4527,15 +4645,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_set', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_set_parser'
-         firstlineno 243
+         firstlineno 252
          lnotab 0x020126010a0116022c01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4551,44 +4669,44 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164077407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064089c027a0600007d046409640a7c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         251           0 RESUME                   0
+         260           0 RESUME                   0
          
-         252           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         261           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         253          40 BUILD_MAP                0
+         262          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         254          50 LOAD_CONST               2 ('a b c c')
+         263          50 LOAD_CONST               2 ('a b c c')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('set')
                       68 STORE_SUBSCR
          
-         256          72 LOAD_FAST                0 (config)
+         265          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_set)
                      108 LOAD_CONST               3 ('set')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         257         126 BUILD_SET                0
+         266         126 BUILD_SET                0
                      128 LOAD_CONST               4 (frozenset({'c', 'a', 'b'}))
                      130 SET_UPDATE               1
                      132 STORE_FAST               2 (@py_assert2)
                      134 LOAD_FAST                1 (result)
                      136 LOAD_FAST                2 (@py_assert2)
                      138 COMPARE_OP               2 (==)
                      144 STORE_FAST               3 (@py_assert1)
@@ -4669,15 +4787,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_set', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_set_proxy'
-         firstlineno 251
+         firstlineno 260
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4693,45 +4811,45 @@
             01a6010000ab01000000000000000072147409000000000000000000006a
             0900000000000000007c01a6010000ab0100000000000000006e01640874
             09000000000000000000006a0900000000000000007c02a6010000ab0100
             0000000000000064099c027a0600007d04640a640b7c0469017a0600007d
             057415000000000000000000007409000000000000000000006a0b000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         259           0 RESUME                   0
+         268           0 RESUME                   0
          
-         260           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         269           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         261          40 BUILD_MAP                0
+         270          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         262          50 LOAD_CONST               2 ('1 2 3')
+         271          50 LOAD_CONST               2 ('1 2 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('set')
                       68 STORE_SUBSCR
          
-         264          72 LOAD_FAST                0 (config)
+         273          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get_set)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('set')
                      100 LOAD_GLOBAL              6 (int)
                      112 KW_NAMES                 4
                      114 PRECALL                  3
                      118 CALL                     3
                      128 STORE_FAST               1 (result)
          
-         265         130 BUILD_SET                0
+         274         130 BUILD_SET                0
                      132 LOAD_CONST               5 (frozenset({1, 2, 3}))
                      134 SET_UPDATE               1
                      136 STORE_FAST               2 (@py_assert2)
                      138 LOAD_FAST                1 (result)
                      140 LOAD_FAST                2 (@py_assert2)
                      142 COMPARE_OP               2 (==)
                      148 STORE_FAST               3 (@py_assert1)
@@ -4813,15 +4931,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_set', 'int', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_set_conv_parser'
-         firstlineno 259
+         firstlineno 268
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4837,46 +4955,46 @@
             01a6010000ab01000000000000000072147407000000000000000000006a
             0800000000000000007c01a6010000ab0100000000000000006e01640974
             07000000000000000000006a0800000000000000007c02a6010000ab0100
             00000000000000640a9c027a0600007d04640b640c7c0469017a0600007d
             057413000000000000000000007407000000000000000000006a0a000000
             00000000007c05a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d037d0264005300
-         267           0 RESUME                   0
+         276           0 RESUME                   0
          
-         268           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         277           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         269          40 BUILD_MAP                0
+         278          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         270          50 LOAD_CONST               2 ('1, 2, 3')
+         279          50 LOAD_CONST               2 ('1, 2, 3')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('set')
                       68 STORE_SUBSCR
          
-         272          72 LOAD_FAST                0 (config)
+         281          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_set)
                      108 LOAD_CONST               3 ('set')
                      110 LOAD_CONST               4 (',')
                      112 KW_NAMES                 5
                      114 PRECALL                  2
                      118 CALL                     2
                      128 STORE_FAST               1 (result)
          
-         273         130 BUILD_SET                0
+         282         130 BUILD_SET                0
                      132 LOAD_CONST               6 (frozenset({'2', '1', '3'}))
                      134 SET_UPDATE               1
                      136 STORE_FAST               2 (@py_assert2)
                      138 LOAD_FAST                1 (result)
                      140 LOAD_FAST                2 (@py_assert2)
                      142 COMPARE_OP               2 (==)
                      148 STORE_FAST               3 (@py_assert1)
@@ -4959,15 +5077,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_set', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_set_sep'
-         firstlineno 267
+         firstlineno 276
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -4983,44 +5101,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016407740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             089c027a0600007d046409640a7c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-         275           0 RESUME                   0
+         284           0 RESUME                   0
          
-         276           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         285           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         277          40 BUILD_MAP                0
+         286          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         278          50 LOAD_CONST               2 ('100 MiB')
+         287          50 LOAD_CONST               2 ('100 MiB')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('bytes')
                       68 STORE_SUBSCR
          
-         280          72 LOAD_FAST                0 (config)
+         289          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_bytes)
                      108 LOAD_CONST               3 ('bytes')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         281         126 LOAD_CONST               4 (104857600)
+         290         126 LOAD_CONST               4 (104857600)
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -5099,15 +5217,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_bytes', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_bytes'
-         firstlineno 275
+         firstlineno 284
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 10
          stacksize : 10
          flags     : 3
          code
@@ -5135,44 +5253,44 @@
             0100000000000000007409000000000000000000006a0900000000000000
             007c05a6010000ab0100000000000000007409000000000000000000006a
             0900000000000000007c06a6010000ab010000000000000000640a9c077a
             0600007d08640b640c7c0869017a0600007d097415000000000000000000
             007409000000000000000000006a0b00000000000000007c09a6010000ab
             010000000000000000a6010000ab0100000000000000008201640078017d
             0778017d0278017d0378017d0478017d057d0664005300
-         283           0 RESUME                   0
+         292           0 RESUME                   0
          
-         284           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         293           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         285          40 BUILD_MAP                0
+         294          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         286          50 LOAD_CONST               2 ('2023-06-01')
+         295          50 LOAD_CONST               2 ('2023-06-01')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('datetime')
                       68 STORE_SUBSCR
          
-         288          72 LOAD_FAST                0 (config)
+         297          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_datetime)
                      108 LOAD_CONST               3 ('datetime')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         289         126 LOAD_GLOBAL              6 (datetime)
+         298         126 LOAD_GLOBAL              6 (datetime)
                      138 LOAD_ATTR                3 (datetime)
                      148 STORE_FAST               2 (@py_assert3)
                      150 LOAD_CONST               4 (2023)
                      152 STORE_FAST               3 (@py_assert5)
                      154 LOAD_CONST               5 (6)
                      156 STORE_FAST               4 (@py_assert7)
                      158 LOAD_CONST               6 (1)
@@ -5317,15 +5435,15 @@
             'py14'
          names      ('sapphire', 'Parser', 'get_datetime', 'datetime', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert1', '@py_format13', '@py_format15')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_datetime'
-         firstlineno 283
+         firstlineno 292
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -5340,37 +5458,37 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164057407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064069c027a0600007d04640764087c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         291           0 RESUME                   0
+         300           0 RESUME                   0
          
-         292           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         301           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         293          40 BUILD_MAP                0
+         302          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         295          50 LOAD_FAST                0 (config)
+         304          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_datetime)
                       86 LOAD_CONST               2 ('missing')
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (result)
          
-         296         104 LOAD_CONST               0 (None)
+         305         104 LOAD_CONST               0 (None)
                      106 STORE_FAST               2 (@py_assert2)
                      108 LOAD_FAST                1 (result)
                      110 LOAD_FAST                2 (@py_assert2)
                      112 IS_OP                    0
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -5447,15 +5565,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_datetime', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_datetime_fallback_none'
-         firstlineno 291
+         firstlineno 300
          lnotab 0x020126010a023601
       code
          argcount  : 0
          nlocals   : 10
          stacksize : 10
          flags     : 3
          code
@@ -5483,39 +5601,39 @@
             0000006a0900000000000000007c05a6010000ab01000000000000000074
             09000000000000000000006a0900000000000000007c06a6010000ab0100
             00000000000000640c9c077a0600007d08640d640e7c0869017a0600007d
             097415000000000000000000007409000000000000000000006a0b000000
             00000000007c09a6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d0778017d0278017d0378017d0478017d057d
             0664005300
-         298           0 RESUME                   0
+         307           0 RESUME                   0
          
-         299           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         308           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         300          40 BUILD_MAP                0
+         309          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         302          50 LOAD_FAST                0 (config)
+         311          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_datetime)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('2023-06-01')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         303         108 LOAD_GLOBAL              6 (datetime)
+         312         108 LOAD_GLOBAL              6 (datetime)
                      120 LOAD_ATTR                3 (datetime)
                      130 STORE_FAST               2 (@py_assert3)
                      132 LOAD_CONST               5 (2023)
                      134 STORE_FAST               3 (@py_assert5)
                      136 LOAD_CONST               6 (6)
                      138 STORE_FAST               4 (@py_assert7)
                      140 LOAD_CONST               7 (1)
@@ -5662,15 +5780,15 @@
             'py14'
          names      ('sapphire', 'Parser', 'get_datetime', 'datetime', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert1', '@py_format13', '@py_format15')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_datetime_fallback_str'
-         firstlineno 298
+         firstlineno 307
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 11
          stacksize : 10
          flags     : 3
          code
@@ -5699,48 +5817,48 @@
             00000000007409000000000000000000006a0900000000000000007c06a6
             010000ab0100000000000000007409000000000000000000006a09000000
             00000000007c07a6010000ab010000000000000000640b9c077a0600007d
             09640c640d7c0969017a0600007d0a741500000000000000000000740900
             0000000000000000006a0b00000000000000007c0aa6010000ab01000000
             0000000000a6010000ab0100000000000000008201640078017d0878017d
             0378017d0478017d0578017d067d0764005300
-         305           0 RESUME                   0
+         314           0 RESUME                   0
          
-         306           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         315           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         307          40 BUILD_MAP                0
+         316          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         309          50 LOAD_GLOBAL              5 (NULL + datetime)
+         318          50 LOAD_GLOBAL              5 (NULL + datetime)
                       62 LOAD_ATTR                2 (datetime)
                       72 LOAD_CONST               2 (2023)
                       74 LOAD_CONST               3 (6)
                       76 LOAD_CONST               4 (1)
                       78 PRECALL                  3
                       82 CALL                     3
                       92 STORE_FAST               1 (dt)
          
-         310          94 LOAD_FAST                0 (config)
+         319          94 LOAD_FAST                0 (config)
                       96 LOAD_CONST               1 ('section')
                       98 BINARY_SUBSCR
                      108 LOAD_METHOD              3 (get_datetime)
                      130 LOAD_CONST               5 ('missing')
                      132 LOAD_FAST                1 (dt)
                      134 KW_NAMES                 6
                      136 PRECALL                  2
                      140 CALL                     2
                      150 STORE_FAST               2 (result)
          
-         311         152 LOAD_GLOBAL              4 (datetime)
+         320         152 LOAD_GLOBAL              4 (datetime)
                      164 LOAD_ATTR                2 (datetime)
                      174 STORE_FAST               3 (@py_assert3)
                      176 LOAD_CONST               2 (2023)
                      178 STORE_FAST               4 (@py_assert5)
                      180 LOAD_CONST               3 (6)
                      182 STORE_FAST               5 (@py_assert7)
                      184 LOAD_CONST               4 (1)
@@ -5886,15 +6004,15 @@
             'py14'
          names      ('sapphire', 'Parser', 'datetime', 'get_datetime', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'dt', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert9', '@py_assert11', '@py_assert1', '@py_format13', '@py_format15')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_datetime_fallback_datetime'
-         firstlineno 305
+         firstlineno 314
          lnotab 0x020126010a022c013a01
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 8
          flags     : 3
          code
@@ -5919,44 +6037,44 @@
             010000ab010000000000000000740b000000000000000000006a0a000000
             00000000007c03a6010000ab010000000000000000740b00000000000000
             0000006a0a00000000000000007c04a6010000ab01000000000000000064
             0a9c057a0600007d06640b640c7c0669017a0600007d0774170000000000
             0000000000740b000000000000000000006a0c00000000000000007c07a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d0578017d0278017d037d0464005300
-         313           0 RESUME                   0
+         322           0 RESUME                   0
          
-         314           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         323           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         315          40 BUILD_MAP                0
+         324          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         316          50 LOAD_CONST               2 ('10s')
+         325          50 LOAD_CONST               2 ('10s')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('timedelta')
                       68 STORE_SUBSCR
          
-         318          72 LOAD_FAST                0 (config)
+         327          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_timedelta)
                      108 LOAD_CONST               3 ('timedelta')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         319         126 LOAD_GLOBAL              6 (datetime)
+         328         126 LOAD_GLOBAL              6 (datetime)
                      138 LOAD_ATTR                4 (timedelta)
                      148 STORE_FAST               2 (@py_assert3)
                      150 LOAD_CONST               4 (10)
                      152 STORE_FAST               3 (@py_assert5)
                      154 PUSH_NULL
                      156 LOAD_FAST                2 (@py_assert3)
                      158 LOAD_FAST                3 (@py_assert5)
@@ -6082,15 +6200,15 @@
             'py10'
          names      ('sapphire', 'Parser', 'get_timedelta', 'datetime', 'timedelta', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_format9', '@py_format11')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_timedelta'
-         firstlineno 313
+         firstlineno 322
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -6105,37 +6223,37 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164057407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064069c027a0600007d04640764087c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         321           0 RESUME                   0
+         330           0 RESUME                   0
          
-         322           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         331           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         323          40 BUILD_MAP                0
+         332          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         325          50 LOAD_FAST                0 (config)
+         334          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_timedelta)
                       86 LOAD_CONST               2 ('missing')
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (result)
          
-         326         104 LOAD_CONST               0 (None)
+         335         104 LOAD_CONST               0 (None)
                      106 STORE_FAST               2 (@py_assert2)
                      108 LOAD_FAST                1 (result)
                      110 LOAD_FAST                2 (@py_assert2)
                      112 IS_OP                    0
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -6212,15 +6330,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_timedelta', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_timedelta_fallback_none'
-         firstlineno 321
+         firstlineno 330
          lnotab 0x020126010a023601
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 8
          flags     : 3
          code
@@ -6245,39 +6363,39 @@
             000000000000006a0a00000000000000007c03a6010000ab010000000000
             000000740b000000000000000000006a0a00000000000000007c04a60100
             00ab010000000000000000640b9c057a0600007d06640c640d7c0669017a
             0600007d07741700000000000000000000740b000000000000000000006a
             0c00000000000000007c07a6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d0578017d0278017d037d04640053
             00
-         328           0 RESUME                   0
+         337           0 RESUME                   0
          
-         329           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         338           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         330          40 BUILD_MAP                0
+         339          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         332          50 LOAD_FAST                0 (config)
+         341          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_timedelta)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('10s')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         333         108 LOAD_GLOBAL              6 (datetime)
+         342         108 LOAD_GLOBAL              6 (datetime)
                      120 LOAD_ATTR                4 (timedelta)
                      130 STORE_FAST               2 (@py_assert3)
                      132 LOAD_CONST               5 (10)
                      134 STORE_FAST               3 (@py_assert5)
                      136 PUSH_NULL
                      138 LOAD_FAST                2 (@py_assert3)
                      140 LOAD_FAST                3 (@py_assert5)
@@ -6404,15 +6522,15 @@
             'py10'
          names      ('sapphire', 'Parser', 'get_timedelta', 'datetime', 'timedelta', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_format9', '@py_format11')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_timedelta_fallback_str'
-         firstlineno 328
+         firstlineno 337
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 8
          flags     : 3
          code
@@ -6437,39 +6555,39 @@
             000000000000006a0a00000000000000007c03a6010000ab010000000000
             000000740b000000000000000000006a0a00000000000000007c04a60100
             00ab010000000000000000640a9c057a0600007d06640b640c7c0669017a
             0600007d07741700000000000000000000740b000000000000000000006a
             0c00000000000000007c07a6010000ab010000000000000000a6010000ab
             0100000000000000008201640078017d0578017d0278017d037d04640053
             00
-         335           0 RESUME                   0
+         344           0 RESUME                   0
          
-         336           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         345           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         337          40 BUILD_MAP                0
+         346          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         339          50 LOAD_FAST                0 (config)
+         348          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_timedelta)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 (10)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         340         108 LOAD_GLOBAL              6 (datetime)
+         349         108 LOAD_GLOBAL              6 (datetime)
                      120 LOAD_ATTR                4 (timedelta)
                      130 STORE_FAST               2 (@py_assert3)
                      132 LOAD_CONST               3 (10)
                      134 STORE_FAST               3 (@py_assert5)
                      136 PUSH_NULL
                      138 LOAD_FAST                2 (@py_assert3)
                      140 LOAD_FAST                3 (@py_assert5)
@@ -6595,15 +6713,15 @@
             'py10'
          names      ('sapphire', 'Parser', 'get_timedelta', 'datetime', 'timedelta', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_format9', '@py_format11')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_timedelta_fallback_int'
-         firstlineno 335
+         firstlineno 344
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -6622,47 +6740,47 @@
             0000000000a6000000ab00000000000000000076007314740b0000000000
             00000000006a0900000000000000007c01a6010000ab0100000000000000
             007214740b000000000000000000006a0a00000000000000007c01a60100
             00ab0100000000000000006e016409640a9c027a0600007d04640b640c7c
             0469017a0600007d05741700000000000000000000740b00000000000000
             0000006a0c00000000000000007c05a6010000ab010000000000000000a6
             010000ab010000000000000000820164007d0364005300
-         342           0 RESUME                   0
+         351           0 RESUME                   0
          
-         343           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         352           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         344          40 BUILD_MAP                0
+         353          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         346          50 LOAD_GLOBAL              5 (NULL + datetime)
+         355          50 LOAD_GLOBAL              5 (NULL + datetime)
                       62 LOAD_ATTR                3 (timedelta)
                       72 LOAD_CONST               2 (10)
                       74 KW_NAMES                 3
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               1 (td)
          
-         347          92 LOAD_FAST                0 (config)
+         356          92 LOAD_FAST                0 (config)
                       94 LOAD_CONST               1 ('section')
                       96 BINARY_SUBSCR
                      106 LOAD_METHOD              4 (get_path)
                      128 LOAD_CONST               4 ('missing')
                      130 LOAD_FAST                1 (td)
                      132 KW_NAMES                 5
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_FAST               2 (result)
          
-         348         150 LOAD_FAST                2 (result)
+         357         150 LOAD_FAST                2 (result)
                      152 LOAD_FAST                1 (td)
                      154 COMPARE_OP               2 (==)
                      160 STORE_FAST               3 (@py_assert1)
                      162 LOAD_FAST                3 (@py_assert1)
                      164 POP_JUMP_FORWARD_IF_TRUE   194 (to 554)
                      166 LOAD_GLOBAL             11 (NULL + @pytest_ar)
                      178 LOAD_ATTR                6 (_call_reprcompare)
@@ -6754,15 +6872,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'get_path', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'td', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_timeselta_fallback_td'
-         firstlineno 342
+         firstlineno 351
          lnotab 0x020126010a022a013a01
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 8
          flags     : 3
          code
@@ -6787,44 +6905,44 @@
             00ab010000000000000000740b000000000000000000006a0a0000000000
             0000007c03a6010000ab010000000000000000740b000000000000000000
             006a0a00000000000000007c04a6010000ab01000000000000000064089c
             057a0600007d066409640a7c0669017a0600007d07741700000000000000
             000000740b000000000000000000006a0c00000000000000007c07a60100
             00ab010000000000000000a6010000ab0100000000000000008201640078
             017d0578017d0278017d037d0464005300
-         350           0 RESUME                   0
+         359           0 RESUME                   0
          
-         351           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         360           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         352          40 BUILD_MAP                0
+         361          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         353          50 LOAD_CONST               2 ('/home/test')
+         362          50 LOAD_CONST               2 ('/home/test')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('path')
                       68 STORE_SUBSCR
          
-         355          72 LOAD_FAST                0 (config)
+         364          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_path)
                      108 LOAD_CONST               3 ('path')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         356         126 LOAD_GLOBAL              6 (pathlib)
+         365         126 LOAD_GLOBAL              6 (pathlib)
                      138 LOAD_ATTR                4 (Path)
                      148 STORE_FAST               2 (@py_assert3)
                      150 LOAD_CONST               2 ('/home/test')
                      152 STORE_FAST               3 (@py_assert5)
                      154 PUSH_NULL
                      156 LOAD_FAST                2 (@py_assert3)
                      158 LOAD_FAST                3 (@py_assert5)
@@ -6947,15 +7065,15 @@
             'py10'
          names      ('sapphire', 'Parser', 'get_path', 'pathlib', 'Path', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_format9', '@py_format11')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_path'
-         firstlineno 350
+         firstlineno 359
          lnotab 0x020126010a0116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -6970,37 +7088,37 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e0164057407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             00000064069c027a0600007d04640764087c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         358           0 RESUME                   0
+         367           0 RESUME                   0
          
-         359           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         368           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         360          40 BUILD_MAP                0
+         369          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         362          50 LOAD_FAST                0 (config)
+         371          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_path)
                       86 LOAD_CONST               2 ('missing')
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (result)
          
-         363         104 LOAD_CONST               0 (None)
+         372         104 LOAD_CONST               0 (None)
                      106 STORE_FAST               2 (@py_assert2)
                      108 LOAD_FAST                1 (result)
                      110 LOAD_FAST                2 (@py_assert2)
                      112 IS_OP                    0
                      114 STORE_FAST               3 (@py_assert1)
                      116 LOAD_FAST                3 (@py_assert1)
                      118 POP_JUMP_FORWARD_IF_TRUE   151 (to 422)
@@ -7077,15 +7195,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_path', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_path_fallback_none'
-         firstlineno 358
+         firstlineno 367
          lnotab 0x020126010a023601
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 8
          flags     : 3
          code
@@ -7109,39 +7227,39 @@
             000000000000007c02a6010000ab010000000000000000740b0000000000
             00000000006a0a00000000000000007c03a6010000ab0100000000000000
             00740b000000000000000000006a0a00000000000000007c04a6010000ab
             01000000000000000064099c057a0600007d06640a640b7c0669017a0600
             007d07741700000000000000000000740b000000000000000000006a0c00
             000000000000007c07a6010000ab010000000000000000a6010000ab0100
             000000000000008201640078017d0578017d0278017d037d0464005300
-         365           0 RESUME                   0
+         374           0 RESUME                   0
          
-         366           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         375           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         367          40 BUILD_MAP                0
+         376          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         369          50 LOAD_FAST                0 (config)
+         378          50 LOAD_FAST                0 (config)
                       52 LOAD_CONST               1 ('section')
                       54 BINARY_SUBSCR
                       64 LOAD_METHOD              2 (get_path)
                       86 LOAD_CONST               2 ('missing')
                       88 LOAD_CONST               3 ('/home/test')
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_FAST               1 (result)
          
-         370         108 LOAD_GLOBAL              6 (pathlib)
+         379         108 LOAD_GLOBAL              6 (pathlib)
                      120 LOAD_ATTR                4 (Path)
                      130 STORE_FAST               2 (@py_assert3)
                      132 LOAD_CONST               3 ('/home/test')
                      134 STORE_FAST               3 (@py_assert5)
                      136 PUSH_NULL
                      138 LOAD_FAST                2 (@py_assert3)
                      140 LOAD_FAST                3 (@py_assert5)
@@ -7265,15 +7383,15 @@
             'py10'
          names      ('sapphire', 'Parser', 'get_path', 'pathlib', 'Path', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert5', '@py_assert7', '@py_assert1', '@py_format9', '@py_format11')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_path_fallback_str'
-         firstlineno 365
+         firstlineno 374
          lnotab 0x020126010a023a01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -7292,46 +7410,46 @@
             000000a6000000ab00000000000000000076007314740b00000000000000
             0000006a0900000000000000007c01a6010000ab01000000000000000072
             14740b000000000000000000006a0a00000000000000007c01a6010000ab
             0100000000000000006e01640864099c027a0600007d04640a640b7c0469
             017a0600007d05741700000000000000000000740b000000000000000000
             006a0c00000000000000007c05a6010000ab010000000000000000a60100
             00ab010000000000000000820164007d0364005300
-         372           0 RESUME                   0
+         381           0 RESUME                   0
          
-         373           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         382           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         374          40 BUILD_MAP                0
+         383          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         376          50 LOAD_GLOBAL              5 (NULL + pathlib)
+         385          50 LOAD_GLOBAL              5 (NULL + pathlib)
                       62 LOAD_ATTR                3 (Path)
                       72 LOAD_CONST               2 ('/home/test')
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               1 (pt)
          
-         377          90 LOAD_FAST                0 (config)
+         386          90 LOAD_FAST                0 (config)
                       92 LOAD_CONST               1 ('section')
                       94 BINARY_SUBSCR
                      104 LOAD_METHOD              4 (get_path)
                      126 LOAD_CONST               3 ('missing')
                      128 LOAD_FAST                1 (pt)
                      130 KW_NAMES                 4
                      132 PRECALL                  2
                      136 CALL                     2
                      146 STORE_FAST               2 (result)
          
-         378         148 LOAD_FAST                2 (result)
+         387         148 LOAD_FAST                2 (result)
                      150 LOAD_FAST                1 (pt)
                      152 COMPARE_OP               2 (==)
                      158 STORE_FAST               3 (@py_assert1)
                      160 LOAD_FAST                3 (@py_assert1)
                      162 POP_JUMP_FORWARD_IF_TRUE   194 (to 552)
                      164 LOAD_GLOBAL             11 (NULL + @pytest_ar)
                      176 LOAD_ATTR                6 (_call_reprcompare)
@@ -7422,15 +7540,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'pathlib', 'Path', 'get_path', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'pt', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_path_fallback_path'
-         firstlineno 372
+         firstlineno 381
          lnotab 0x020126010a0228013a01
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -7451,59 +7569,59 @@
             000000a6000000ab00000000000000000076007314740d00000000000000
             0000006a0a00000000000000007c02a6010000ab01000000000000000072
             14740d000000000000000000006a0b00000000000000007c02a6010000ab
             0100000000000000006e01640364099c027a0600007d05640a640b7c0569
             017a0600007d06741900000000000000000000740d000000000000000000
             006a0d00000000000000007c06a6010000ab010000000000000000a60100
             00ab010000000000000000820164007d0464005300
-         380           0 RESUME                   0
+         389           0 RESUME                   0
          
-         381           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         390           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         382          40 BUILD_MAP                0
+         391          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         383          50 LOAD_CONST               2 ('60')
+         392          50 LOAD_CONST               2 ('60')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('rate')
                       68 STORE_SUBSCR
          
-         385          72 LOAD_GLOBAL              5 (NULL + datetime)
+         394          72 LOAD_GLOBAL              5 (NULL + datetime)
                       84 LOAD_ATTR                3 (timedelta)
                       94 LOAD_CONST               4 (60)
                       96 KW_NAMES                 5
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               1 (period)
          
-         386         114 LOAD_GLOBAL              1 (NULL + sapphire)
+         395         114 LOAD_GLOBAL              1 (NULL + sapphire)
                      126 LOAD_ATTR                4 (Rate)
                      136 LOAD_FAST                1 (period)
                      138 PRECALL                  1
                      142 CALL                     1
                      152 STORE_FAST               2 (rate)
          
-         388         154 LOAD_FAST                0 (config)
+         397         154 LOAD_FAST                0 (config)
                      156 LOAD_CONST               1 ('section')
                      158 BINARY_SUBSCR
                      168 LOAD_METHOD              5 (get_rate)
                      190 LOAD_CONST               3 ('rate')
                      192 PRECALL                  1
                      196 CALL                     1
                      206 STORE_FAST               3 (result)
          
-         389         208 LOAD_FAST                3 (result)
+         398         208 LOAD_FAST                3 (result)
                      210 LOAD_FAST                2 (rate)
                      212 COMPARE_OP               2 (==)
                      218 STORE_FAST               4 (@py_assert1)
                      220 LOAD_FAST                4 (@py_assert1)
                      222 POP_JUMP_FORWARD_IF_TRUE   194 (to 612)
                      224 LOAD_GLOBAL             13 (NULL + @pytest_ar)
                      236 LOAD_ATTR                7 (_call_reprcompare)
@@ -7594,15 +7712,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'Rate', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'period', 'rate', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate'
-         firstlineno 380
+         firstlineno 389
          lnotab 0x020126010a0116022a0128023601
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -7627,92 +7745,92 @@
             000000ab00000000000000000076007314740d000000000000000000006a
             0a00000000000000007c03a6010000ab0100000000000000007214740d00
             0000000000000000006a0b00000000000000007c03a6010000ab01000000
             00000000006e01640e64129c027a0600007d06641364147c0669017a0600
             007d07741900000000000000000000740d000000000000000000006a0d00
             000000000000007c07a6010000ab010000000000000000a6010000ab0100
             00000000000000820164007d0564005300
-         391           0 RESUME                   0
+         400           0 RESUME                   0
          
-         392           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         401           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         393          40 BUILD_MAP                0
+         402          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         394          50 LOAD_CONST               2 ('60')
+         403          50 LOAD_CONST               2 ('60')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('rate.period')
                       68 STORE_SUBSCR
          
-         395          72 LOAD_CONST               4 ('true')
+         404          72 LOAD_CONST               4 ('true')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('rate.sync')
                       90 STORE_SUBSCR
          
-         396          94 LOAD_CONST               6 ('10s')
+         405          94 LOAD_CONST               6 ('10s')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('rate.offset')
                      112 STORE_SUBSCR
          
-         397         116 LOAD_CONST               4 ('true')
+         406         116 LOAD_CONST               4 ('true')
                      118 LOAD_FAST                0 (config)
                      120 LOAD_CONST               1 ('section')
                      122 BINARY_SUBSCR
                      132 LOAD_CONST               8 ('rate.at_start')
                      134 STORE_SUBSCR
          
-         399         138 LOAD_GLOBAL              5 (NULL + datetime)
+         408         138 LOAD_GLOBAL              5 (NULL + datetime)
                      150 LOAD_ATTR                3 (timedelta)
                      160 LOAD_CONST               9 (60)
                      162 KW_NAMES                10
                      164 PRECALL                  1
                      168 CALL                     1
                      178 STORE_FAST               1 (period)
          
-         400         180 LOAD_GLOBAL              5 (NULL + datetime)
+         409         180 LOAD_GLOBAL              5 (NULL + datetime)
                      192 LOAD_ATTR                3 (timedelta)
                      202 LOAD_CONST              11 (10)
                      204 KW_NAMES                10
                      206 PRECALL                  1
                      210 CALL                     1
                      220 STORE_FAST               2 (offset)
          
-         401         222 LOAD_GLOBAL              1 (NULL + sapphire)
+         410         222 LOAD_GLOBAL              1 (NULL + sapphire)
                      234 LOAD_ATTR                4 (Rate)
                      244 LOAD_FAST                1 (period)
                      246 LOAD_CONST              12 (True)
                      248 LOAD_FAST                2 (offset)
                      250 LOAD_CONST              12 (True)
                      252 KW_NAMES                13
                      254 PRECALL                  4
                      258 CALL                     4
                      268 STORE_FAST               3 (rate)
          
-         403         270 LOAD_FAST                0 (config)
+         412         270 LOAD_FAST                0 (config)
                      272 LOAD_CONST               1 ('section')
                      274 BINARY_SUBSCR
                      284 LOAD_METHOD              5 (get_rate)
                      306 LOAD_CONST              14 ('rate')
                      308 PRECALL                  1
                      312 CALL                     1
                      322 STORE_FAST               4 (result)
          
-         404         324 LOAD_FAST                4 (result)
+         413         324 LOAD_FAST                4 (result)
                      326 LOAD_FAST                3 (rate)
                      328 COMPARE_OP               2 (==)
                      334 STORE_FAST               5 (@py_assert1)
                      336 LOAD_FAST                5 (@py_assert1)
                      338 POP_JUMP_FORWARD_IF_TRUE   194 (to 728)
                      340 LOAD_GLOBAL             13 (NULL + @pytest_ar)
                      352 LOAD_ATTR                7 (_call_reprcompare)
@@ -7812,15 +7930,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'Rate', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'period', 'offset', 'rate', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate_all'
-         firstlineno 391
+         firstlineno 400
          lnotab 0x020126010a0116011601160116022a012a0130023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -7835,36 +7953,36 @@
             0072147407000000000000000000006a0800000000000000007c01a60100
             00ab0100000000000000006e0164057407000000000000000000006a0800
             000000000000007c02a6010000ab01000000000000000064069c027a0600
             007d04640764087c0469017a0600007d0574130000000000000000000074
             07000000000000000000006a0a00000000000000007c05a6010000ab0100
             00000000000000a6010000ab0100000000000000008201640078017d037d
             0264005300
-         406           0 RESUME                   0
+         415           0 RESUME                   0
          
-         407           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         416           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         408          40 BUILD_MAP                0
+         417          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         411          50 LOAD_FAST                0 (config)
+         420          50 LOAD_FAST                0 (config)
                       52 LOAD_METHOD              2 (get_rate)
                       74 LOAD_CONST               1 ('section')
                       76 LOAD_CONST               2 ('missing')
                       78 PRECALL                  2
                       82 CALL                     2
                       92 STORE_FAST               1 (result)
          
-         412          94 LOAD_CONST               0 (None)
+         421          94 LOAD_CONST               0 (None)
                       96 STORE_FAST               2 (@py_assert2)
                       98 LOAD_FAST                1 (result)
                      100 LOAD_FAST                2 (@py_assert2)
                      102 IS_OP                    0
                      104 STORE_FAST               3 (@py_assert1)
                      106 LOAD_FAST                3 (@py_assert1)
                      108 POP_JUMP_FORWARD_IF_TRUE   151 (to 412)
@@ -7941,15 +8059,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate_fallback_none'
-         firstlineno 406
+         firstlineno 415
          lnotab 0x020126010a032c01
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -7970,54 +8088,54 @@
             007314740d000000000000000000006a0a00000000000000007c02a60100
             00ab0100000000000000007214740d000000000000000000006a0b000000
             00000000007c02a6010000ab0100000000000000006e01640a640b9c027a
             0600007d05640c640d7c0569017a0600007d067419000000000000000000
             00740d000000000000000000006a0d00000000000000007c06a6010000ab
             010000000000000000a6010000ab010000000000000000820164007d0464
             005300
-         414           0 RESUME                   0
+         423           0 RESUME                   0
          
-         415           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         424           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         416          40 BUILD_MAP                0
+         425          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         418          50 LOAD_GLOBAL              5 (NULL + datetime)
+         427          50 LOAD_GLOBAL              5 (NULL + datetime)
                       62 LOAD_ATTR                3 (timedelta)
                       72 LOAD_CONST               2 (60)
                       74 KW_NAMES                 3
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               1 (period)
          
-         419          92 LOAD_GLOBAL              1 (NULL + sapphire)
+         428          92 LOAD_GLOBAL              1 (NULL + sapphire)
                      104 LOAD_ATTR                4 (Rate)
                      114 LOAD_FAST                1 (period)
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               2 (rate)
          
-         421         132 LOAD_FAST                0 (config)
+         430         132 LOAD_FAST                0 (config)
                      134 LOAD_CONST               1 ('section')
                      136 BINARY_SUBSCR
                      146 LOAD_METHOD              5 (get_rate)
                      168 LOAD_CONST               4 ('missing')
                      170 LOAD_CONST               5 ('60s')
                      172 KW_NAMES                 6
                      174 PRECALL                  2
                      178 CALL                     2
                      188 STORE_FAST               3 (result)
          
-         422         190 LOAD_FAST                3 (result)
+         431         190 LOAD_FAST                3 (result)
                      192 LOAD_FAST                2 (rate)
                      194 COMPARE_OP               2 (==)
                      200 STORE_FAST               4 (@py_assert1)
                      202 LOAD_FAST                4 (@py_assert1)
                      204 POP_JUMP_FORWARD_IF_TRUE   194 (to 594)
                      206 LOAD_GLOBAL             13 (NULL + @pytest_ar)
                      218 LOAD_ATTR                7 (_call_reprcompare)
@@ -8110,15 +8228,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'Rate', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'period', 'rate', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate_fallback_str'
-         firstlineno 414
+         firstlineno 423
          lnotab 0x020126010a022a0128023a01
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -8139,54 +8257,54 @@
             007314740d000000000000000000006a0a00000000000000007c02a60100
             00ab0100000000000000007214740d000000000000000000006a0b000000
             00000000007c02a6010000ab0100000000000000006e016409640a9c027a
             0600007d05640b640c7c0569017a0600007d067419000000000000000000
             00740d000000000000000000006a0d00000000000000007c06a6010000ab
             010000000000000000a6010000ab010000000000000000820164007d0464
             005300
-         424           0 RESUME                   0
+         433           0 RESUME                   0
          
-         425           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         434           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         426          40 BUILD_MAP                0
+         435          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         428          50 LOAD_GLOBAL              5 (NULL + datetime)
+         437          50 LOAD_GLOBAL              5 (NULL + datetime)
                       62 LOAD_ATTR                3 (timedelta)
                       72 LOAD_CONST               2 (60)
                       74 KW_NAMES                 3
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               1 (period)
          
-         429          92 LOAD_GLOBAL              1 (NULL + sapphire)
+         438          92 LOAD_GLOBAL              1 (NULL + sapphire)
                      104 LOAD_ATTR                4 (Rate)
                      114 LOAD_FAST                1 (period)
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               2 (rate)
          
-         431         132 LOAD_FAST                0 (config)
+         440         132 LOAD_FAST                0 (config)
                      134 LOAD_CONST               1 ('section')
                      136 BINARY_SUBSCR
                      146 LOAD_METHOD              5 (get_rate)
                      168 LOAD_CONST               4 ('missing')
                      170 LOAD_CONST               2 (60)
                      172 KW_NAMES                 5
                      174 PRECALL                  2
                      178 CALL                     2
                      188 STORE_FAST               3 (result)
          
-         432         190 LOAD_FAST                3 (result)
+         441         190 LOAD_FAST                3 (result)
                      192 LOAD_FAST                2 (rate)
                      194 COMPARE_OP               2 (==)
                      200 STORE_FAST               4 (@py_assert1)
                      202 LOAD_FAST                4 (@py_assert1)
                      204 POP_JUMP_FORWARD_IF_TRUE   194 (to 594)
                      206 LOAD_GLOBAL             13 (NULL + @pytest_ar)
                      218 LOAD_ATTR                7 (_call_reprcompare)
@@ -8278,15 +8396,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'Rate', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'period', 'rate', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate_fallback_int'
-         firstlineno 424
+         firstlineno 433
          lnotab 0x020126010a022a0128023a01
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -8307,54 +8425,54 @@
             007314740d000000000000000000006a0a00000000000000007c02a60100
             00ab0100000000000000007214740d000000000000000000006a0b000000
             00000000007c02a6010000ab0100000000000000006e016409640a9c027a
             0600007d05640b640c7c0569017a0600007d067419000000000000000000
             00740d000000000000000000006a0d00000000000000007c06a6010000ab
             010000000000000000a6010000ab010000000000000000820164007d0464
             005300
-         434           0 RESUME                   0
+         443           0 RESUME                   0
          
-         435           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         444           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         436          40 BUILD_MAP                0
+         445          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         438          50 LOAD_GLOBAL              5 (NULL + datetime)
+         447          50 LOAD_GLOBAL              5 (NULL + datetime)
                       62 LOAD_ATTR                3 (timedelta)
                       72 LOAD_CONST               2 (60)
                       74 KW_NAMES                 3
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               1 (period)
          
-         439          92 LOAD_GLOBAL              1 (NULL + sapphire)
+         448          92 LOAD_GLOBAL              1 (NULL + sapphire)
                      104 LOAD_ATTR                4 (Rate)
                      114 LOAD_FAST                1 (period)
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               2 (rate)
          
-         441         132 LOAD_FAST                0 (config)
+         450         132 LOAD_FAST                0 (config)
                      134 LOAD_CONST               1 ('section')
                      136 BINARY_SUBSCR
                      146 LOAD_METHOD              5 (get_rate)
                      168 LOAD_CONST               4 ('missing')
                      170 LOAD_FAST                2 (rate)
                      172 KW_NAMES                 5
                      174 PRECALL                  2
                      178 CALL                     2
                      188 STORE_FAST               3 (result)
          
-         442         190 LOAD_FAST                3 (result)
+         451         190 LOAD_FAST                3 (result)
                      192 LOAD_FAST                2 (rate)
                      194 COMPARE_OP               2 (==)
                      200 STORE_FAST               4 (@py_assert1)
                      202 LOAD_FAST                4 (@py_assert1)
                      204 POP_JUMP_FORWARD_IF_TRUE   194 (to 594)
                      206 LOAD_GLOBAL             13 (NULL + @pytest_ar)
                      218 LOAD_ATTR                7 (_call_reprcompare)
@@ -8446,15 +8564,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'datetime', 'timedelta', 'Rate', 'get_rate', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'period', 'rate', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_rate_fallback_rate'
-         firstlineno 434
+         firstlineno 443
          lnotab 0x020126010a022a0128023a01
       code
          argcount  : 0
          nlocals   : 13
          stacksize : 9
          flags     : 3
          code
@@ -8562,24 +8680,24 @@
             11000000000000000000006a0a00000000000000007c05a6010000ab0100
             000000000000007411000000000000000000006a0a00000000000000007c
             0aa6010000ab01000000000000000064109c037a0600007d0b641164127c
             0b69017a0600007d0c741700000000000000000000741100000000000000
             0000006a0c00000000000000007c0ca6010000ab010000000000000000a6
             010000ab0100000000000000008201640078017d0578017d067d0a640053
             00
-         444           0 RESUME                   0
+         453           0 RESUME                   0
          
-         445           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         454           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (0)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               0 (rate)
          
-         447          42 LOAD_FAST                0 (rate)
+         456          42 LOAD_FAST                0 (rate)
                       44 LOAD_ATTR                2 (period)
                       54 STORE_FAST               1 (@py_assert2)
                       56 LOAD_GLOBAL              6 (datetime)
                       68 LOAD_ATTR                4 (timedelta)
                       78 STORE_FAST               2 (@py_assert5)
                       80 LOAD_GLOBAL             11 (NULL + isinstance)
                       92 LOAD_FAST                1 (@py_assert2)
@@ -8682,15 +8800,15 @@
                  >>  722 LOAD_CONST               0 (None)
                      724 COPY                     1
                      726 STORE_FAST               1 (@py_assert2)
                      728 COPY                     1
                      730 STORE_FAST               2 (@py_assert5)
                      732 STORE_FAST               3 (@py_assert7)
          
-         448         734 LOAD_FAST                0 (rate)
+         457         734 LOAD_FAST                0 (rate)
                      736 LOAD_ATTR               13 (offset)
                      746 STORE_FAST               1 (@py_assert2)
                      748 LOAD_GLOBAL              6 (datetime)
                      760 LOAD_ATTR                4 (timedelta)
                      770 STORE_FAST               2 (@py_assert5)
                      772 LOAD_GLOBAL             11 (NULL + isinstance)
                      784 LOAD_FAST                1 (@py_assert2)
@@ -8793,15 +8911,15 @@
                  >> 1414 LOAD_CONST               0 (None)
                     1416 COPY                     1
                     1418 STORE_FAST               1 (@py_assert2)
                     1420 COPY                     1
                     1422 STORE_FAST               2 (@py_assert5)
                     1424 STORE_FAST               3 (@py_assert7)
          
-         449        1426 LOAD_FAST                0 (rate)
+         458        1426 LOAD_FAST                0 (rate)
                     1428 LOAD_ATTR                2 (period)
                     1438 STORE_FAST               5 (@py_assert1)
                     1440 LOAD_FAST                5 (@py_assert1)
                     1442 LOAD_ATTR               14 (total_seconds)
                     1452 STORE_FAST               6 (@py_assert3)
                     1454 PUSH_NULL
                     1456 LOAD_FAST                6 (@py_assert3)
@@ -8893,15 +9011,15 @@
                     1918 STORE_FAST               6 (@py_assert3)
                     1920 COPY                     1
                     1922 STORE_FAST               2 (@py_assert5)
                     1924 COPY                     1
                     1926 STORE_FAST               3 (@py_assert7)
                     1928 STORE_FAST               7 (@py_assert8)
          
-         450        1930 LOAD_FAST                0 (rate)
+         459        1930 LOAD_FAST                0 (rate)
                     1932 LOAD_ATTR               13 (offset)
                     1942 STORE_FAST               5 (@py_assert1)
                     1944 LOAD_FAST                5 (@py_assert1)
                     1946 LOAD_ATTR               14 (total_seconds)
                     1956 STORE_FAST               6 (@py_assert3)
                     1958 PUSH_NULL
                     1960 LOAD_FAST                6 (@py_assert3)
@@ -8993,15 +9111,15 @@
                     2422 STORE_FAST               6 (@py_assert3)
                     2424 COPY                     1
                     2426 STORE_FAST               2 (@py_assert5)
                     2428 COPY                     1
                     2430 STORE_FAST               3 (@py_assert7)
                     2432 STORE_FAST               7 (@py_assert8)
          
-         451        2434 LOAD_FAST                0 (rate)
+         460        2434 LOAD_FAST                0 (rate)
                     2436 LOAD_ATTR               16 (sync)
                     2446 STORE_FAST               5 (@py_assert1)
                     2448 LOAD_CONST              14 (False)
                     2450 STORE_FAST              10 (@py_assert4)
                     2452 LOAD_FAST                5 (@py_assert1)
                     2454 LOAD_FAST               10 (@py_assert4)
                     2456 COMPARE_OP               2 (==)
@@ -9071,15 +9189,15 @@
                  >> 2808 LOAD_CONST               0 (None)
                     2810 COPY                     1
                     2812 STORE_FAST               5 (@py_assert1)
                     2814 COPY                     1
                     2816 STORE_FAST               6 (@py_assert3)
                     2818 STORE_FAST              10 (@py_assert4)
          
-         452        2820 LOAD_FAST                0 (rate)
+         461        2820 LOAD_FAST                0 (rate)
                     2822 LOAD_ATTR               17 (at_start)
                     2832 STORE_FAST               5 (@py_assert1)
                     2834 LOAD_CONST              14 (False)
                     2836 STORE_FAST              10 (@py_assert4)
                     2838 LOAD_FAST                5 (@py_assert1)
                     2840 LOAD_FAST               10 (@py_assert4)
                     2842 COMPARE_OP               2 (==)
@@ -9177,15 +9295,15 @@
             ('%(py2)s\n{%(py2)s = %(py0)s.at_start\n} == %(py5)s',)
          names      ('sapphire', 'Rate', 'period', 'datetime', 'timedelta', 'isinstance', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'offset', 'total_seconds', '_call_reprcompare', 'sync', 'at_start')
          varnames   ('rate', '@py_assert2', '@py_assert5', '@py_assert7', '@py_format9', '@py_assert1', '@py_assert3', '@py_assert8', '@py_format10', '@py_format12', '@py_assert4', '@py_format6', '@py_format8')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_init_default'
-         firstlineno 444
+         firstlineno 453
          lnotab 0x02012802ff00ff00b601ff00ff00b601ff00f901ff00f901ff008301
       code
          argcount  : 0
          nlocals   : 12
          stacksize : 9
          flags     : 3
          code
@@ -9270,39 +9388,39 @@
             0000006a0a00000000000000007c04a6010000ab01000000000000000074
             11000000000000000000006a0a00000000000000007c09a6010000ab0100
             00000000000000640a9c057a0600007d0a640b640c7c0a69017a0600007d
             0b7417000000000000000000007411000000000000000000006a0c000000
             00000000007c0ba6010000ab010000000000000000a6010000ab01000000
             00000000008201640078017d0778017d0878017d0478017d057d09640053
             00
-         454           0 RESUME                   0
+         463           0 RESUME                   0
          
-         455           2 LOAD_GLOBAL              1 (NULL + datetime)
+         464           2 LOAD_GLOBAL              1 (NULL + datetime)
                       14 LOAD_ATTR                1 (timedelta)
                       24 LOAD_CONST               1 (0)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               0 (period)
          
-         456          42 LOAD_GLOBAL              1 (NULL + datetime)
+         465          42 LOAD_GLOBAL              1 (NULL + datetime)
                       54 LOAD_ATTR                1 (timedelta)
                       64 LOAD_CONST               1 (0)
                       66 PRECALL                  1
                       70 CALL                     1
                       80 STORE_FAST               1 (offset)
          
-         457          82 LOAD_GLOBAL              5 (NULL + sapphire)
+         466          82 LOAD_GLOBAL              5 (NULL + sapphire)
                       94 LOAD_ATTR                3 (Rate)
                      104 LOAD_FAST                0 (period)
                      106 LOAD_FAST                1 (offset)
                      108 PRECALL                  2
                      112 CALL                     2
                      122 STORE_FAST               2 (rate)
          
-         459         124 LOAD_FAST                2 (rate)
+         468         124 LOAD_FAST                2 (rate)
                      126 LOAD_ATTR                4 (period)
                      136 STORE_FAST               3 (@py_assert2)
                      138 LOAD_GLOBAL              0 (datetime)
                      150 LOAD_ATTR                1 (timedelta)
                      160 STORE_FAST               4 (@py_assert5)
                      162 LOAD_GLOBAL             11 (NULL + isinstance)
                      174 LOAD_FAST                3 (@py_assert2)
@@ -9405,15 +9523,15 @@
                  >>  804 LOAD_CONST               0 (None)
                      806 COPY                     1
                      808 STORE_FAST               3 (@py_assert2)
                      810 COPY                     1
                      812 STORE_FAST               4 (@py_assert5)
                      814 STORE_FAST               5 (@py_assert7)
          
-         460         816 LOAD_FAST                2 (rate)
+         469         816 LOAD_FAST                2 (rate)
                      818 LOAD_ATTR               13 (offset)
                      828 STORE_FAST               3 (@py_assert2)
                      830 LOAD_GLOBAL              0 (datetime)
                      842 LOAD_ATTR                1 (timedelta)
                      852 STORE_FAST               4 (@py_assert5)
                      854 LOAD_GLOBAL             11 (NULL + isinstance)
                      866 LOAD_FAST                3 (@py_assert2)
@@ -9516,15 +9634,15 @@
                  >> 1496 LOAD_CONST               0 (None)
                     1498 COPY                     1
                     1500 STORE_FAST               3 (@py_assert2)
                     1502 COPY                     1
                     1504 STORE_FAST               4 (@py_assert5)
                     1506 STORE_FAST               5 (@py_assert7)
          
-         461        1508 LOAD_FAST                2 (rate)
+         470        1508 LOAD_FAST                2 (rate)
                     1510 LOAD_ATTR                4 (period)
                     1520 STORE_FAST               7 (@py_assert1)
                     1522 LOAD_FAST                7 (@py_assert1)
                     1524 LOAD_ATTR               14 (total_seconds)
                     1534 STORE_FAST               8 (@py_assert3)
                     1536 PUSH_NULL
                     1538 LOAD_FAST                8 (@py_assert3)
@@ -9616,15 +9734,15 @@
                     2000 STORE_FAST               8 (@py_assert3)
                     2002 COPY                     1
                     2004 STORE_FAST               4 (@py_assert5)
                     2006 COPY                     1
                     2008 STORE_FAST               5 (@py_assert7)
                     2010 STORE_FAST               9 (@py_assert8)
          
-         462        2012 LOAD_FAST                2 (rate)
+         471        2012 LOAD_FAST                2 (rate)
                     2014 LOAD_ATTR               13 (offset)
                     2024 STORE_FAST               7 (@py_assert1)
                     2026 LOAD_FAST                7 (@py_assert1)
                     2028 LOAD_ATTR               14 (total_seconds)
                     2038 STORE_FAST               8 (@py_assert3)
                     2040 PUSH_NULL
                     2042 LOAD_FAST                8 (@py_assert3)
@@ -9738,15 +9856,15 @@
             ('%(py6)s\n{%(py6)s = %(py4)s\n{%(py4)s = %(py2)s\n{%(py2)s = %(py0)s.offset\n}.total_seconds\n}()\n} == %(py9)s',)
          names      ('datetime', 'timedelta', 'sapphire', 'Rate', 'period', 'isinstance', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation', 'offset', 'total_seconds', '_call_reprcompare')
          varnames   ('period', 'offset', 'rate', '@py_assert2', '@py_assert5', '@py_assert7', '@py_format9', '@py_assert1', '@py_assert3', '@py_assert8', '@py_format10', '@py_format12')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_init_timedelta'
-         firstlineno 454
+         firstlineno 463
          lnotab 0x0201280128012a02ff00ff00b601ff00ff00b601ff00f901
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 8
          flags     : 3
          code
@@ -9766,45 +9884,45 @@
             03a6010000ab010000000000000000740b000000000000000000006a0a00
             000000000000007c04a6010000ab010000000000000000740b0000000000
             00000000006a0a00000000000000007c05a6010000ab0100000000000000
             00640b9c047a0600007d07640c640d7c0769017a0600007d087417000000
             00000000000000740b000000000000000000006a0c00000000000000007c
             08a6010000ab010000000000000000a6010000ab01000000000000000082
             01640078017d0378017d0478017d067d0564005300
-         464           0 RESUME                   0
+         473           0 RESUME                   0
          
-         465           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         474           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (60)
                       26 LOAD_CONST               2 (False)
                       28 KW_NAMES                 3
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               0 (rate)
          
-         467          46 LOAD_GLOBAL              5 (NULL + datetime)
+         476          46 LOAD_GLOBAL              5 (NULL + datetime)
                       58 LOAD_ATTR                2 (datetime)
                       68 LOAD_CONST               4 (2001)
                       70 LOAD_CONST               5 (1)
                       72 LOAD_CONST               5 (1)
                       74 LOAD_CONST               6 (0)
                       76 LOAD_CONST               6 (0)
                       78 LOAD_CONST               7 (5)
                       80 PRECALL                  6
                       84 CALL                     6
                       94 STORE_FAST               1 (curtime)
          
-         469          96 LOAD_FAST                0 (rate)
+         478          96 LOAD_FAST                0 (rate)
                       98 LOAD_METHOD              3 (nexttime)
                      120 LOAD_FAST                1 (curtime)
                      122 PRECALL                  1
                      126 CALL                     1
                      136 STORE_FAST               2 (wait)
          
-         470         138 LOAD_FAST                2 (wait)
+         479         138 LOAD_FAST                2 (wait)
                      140 LOAD_ATTR                4 (total_seconds)
                      150 STORE_FAST               3 (@py_assert1)
                      152 PUSH_NULL
                      154 LOAD_FAST                3 (@py_assert1)
                      156 PRECALL                  0
                      160 CALL                     0
                      170 STORE_FAST               4 (@py_assert3)
@@ -9908,15 +10026,15 @@
             'py9'
          names      ('sapphire', 'Rate', 'datetime', 'nexttime', 'total_seconds', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('rate', 'curtime', 'wait', '@py_assert1', '@py_assert3', '@py_assert6', '@py_assert5', '@py_format8', '@py_format10')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_nexttime'
-         firstlineno 464
+         firstlineno 473
          lnotab 0x02012c0232022a01
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 8
          flags     : 3
          code
@@ -9936,45 +10054,45 @@
             03a6010000ab010000000000000000740b000000000000000000006a0a00
             000000000000007c04a6010000ab010000000000000000740b0000000000
             00000000006a0a00000000000000007c05a6010000ab0100000000000000
             00640c9c047a0600007d07640d640e7c0769017a0600007d087417000000
             00000000000000740b000000000000000000006a0c00000000000000007c
             08a6010000ab010000000000000000a6010000ab01000000000000000082
             01640078017d0378017d0478017d067d0564005300
-         472           0 RESUME                   0
+         481           0 RESUME                   0
          
-         473           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         482           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (60)
                       26 LOAD_CONST               2 (True)
                       28 KW_NAMES                 3
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               0 (rate)
          
-         475          46 LOAD_GLOBAL              5 (NULL + datetime)
+         484          46 LOAD_GLOBAL              5 (NULL + datetime)
                       58 LOAD_ATTR                2 (datetime)
                       68 LOAD_CONST               4 (2001)
                       70 LOAD_CONST               5 (1)
                       72 LOAD_CONST               5 (1)
                       74 LOAD_CONST               6 (0)
                       76 LOAD_CONST               6 (0)
                       78 LOAD_CONST               7 (5)
                       80 PRECALL                  6
                       84 CALL                     6
                       94 STORE_FAST               1 (curtime)
          
-         477          96 LOAD_FAST                0 (rate)
+         486          96 LOAD_FAST                0 (rate)
                       98 LOAD_METHOD              3 (nexttime)
                      120 LOAD_FAST                1 (curtime)
                      122 PRECALL                  1
                      126 CALL                     1
                      136 STORE_FAST               2 (wait)
          
-         478         138 LOAD_FAST                2 (wait)
+         487         138 LOAD_FAST                2 (wait)
                      140 LOAD_ATTR                4 (total_seconds)
                      150 STORE_FAST               3 (@py_assert1)
                      152 PUSH_NULL
                      154 LOAD_FAST                3 (@py_assert1)
                      156 PRECALL                  0
                      160 CALL                     0
                      170 STORE_FAST               4 (@py_assert3)
@@ -10079,15 +10197,15 @@
             'py9'
          names      ('sapphire', 'Rate', 'datetime', 'nexttime', 'total_seconds', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('rate', 'curtime', 'wait', '@py_assert1', '@py_assert3', '@py_assert6', '@py_assert5', '@py_format8', '@py_format10')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_nexttime_sync'
-         firstlineno 472
+         firstlineno 481
          lnotab 0x02012c0232022a01
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 8
          flags     : 3
          code
@@ -10107,45 +10225,45 @@
             03a6010000ab010000000000000000740b000000000000000000006a0a00
             000000000000007c04a6010000ab010000000000000000740b0000000000
             00000000006a0a00000000000000007c05a6010000ab0100000000000000
             00640b9c047a0600007d07640c640d7c0769017a0600007d087417000000
             00000000000000740b000000000000000000006a0c00000000000000007c
             08a6010000ab010000000000000000a6010000ab01000000000000000082
             01640078017d0378017d0478017d067d0564005300
-         480           0 RESUME                   0
+         489           0 RESUME                   0
          
-         481           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         490           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (60)
                       26 LOAD_CONST               2 (10)
                       28 KW_NAMES                 3
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               0 (rate)
          
-         483          46 LOAD_GLOBAL              5 (NULL + datetime)
+         492          46 LOAD_GLOBAL              5 (NULL + datetime)
                       58 LOAD_ATTR                2 (datetime)
                       68 LOAD_CONST               4 (2001)
                       70 LOAD_CONST               5 (1)
                       72 LOAD_CONST               5 (1)
                       74 LOAD_CONST               6 (0)
                       76 LOAD_CONST               6 (0)
                       78 LOAD_CONST               7 (5)
                       80 PRECALL                  6
                       84 CALL                     6
                       94 STORE_FAST               1 (curtime)
          
-         485          96 LOAD_FAST                0 (rate)
+         494          96 LOAD_FAST                0 (rate)
                       98 LOAD_METHOD              3 (nexttime)
                      120 LOAD_FAST                1 (curtime)
                      122 PRECALL                  1
                      126 CALL                     1
                      136 STORE_FAST               2 (wait)
          
-         486         138 LOAD_FAST                2 (wait)
+         495         138 LOAD_FAST                2 (wait)
                      140 LOAD_ATTR                4 (total_seconds)
                      150 STORE_FAST               3 (@py_assert1)
                      152 PUSH_NULL
                      154 LOAD_FAST                3 (@py_assert1)
                      156 PRECALL                  0
                      160 CALL                     0
                      170 STORE_FAST               4 (@py_assert3)
@@ -10249,15 +10367,15 @@
             'py9'
          names      ('sapphire', 'Rate', 'datetime', 'nexttime', 'total_seconds', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('rate', 'curtime', 'wait', '@py_assert1', '@py_assert3', '@py_assert6', '@py_assert5', '@py_format8', '@py_format10')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_nexttime_offset'
-         firstlineno 480
+         firstlineno 489
          lnotab 0x02012c0232022a01
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 8
          flags     : 3
          code
@@ -10277,46 +10395,46 @@
             007c03a6010000ab010000000000000000740b000000000000000000006a
             0a00000000000000007c04a6010000ab010000000000000000740b000000
             000000000000006a0a00000000000000007c05a6010000ab010000000000
             000000640c9c047a0600007d07640d640e7c0769017a0600007d08741700
             000000000000000000740b000000000000000000006a0c00000000000000
             007c08a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d0378017d0478017d067d0564005300
-         488           0 RESUME                   0
+         497           0 RESUME                   0
          
-         489           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         498           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (60)
                       26 LOAD_CONST               2 (10)
                       28 LOAD_CONST               3 (True)
                       30 KW_NAMES                 4
                       32 PRECALL                  3
                       36 CALL                     3
                       46 STORE_FAST               0 (rate)
          
-         491          48 LOAD_GLOBAL              5 (NULL + datetime)
+         500          48 LOAD_GLOBAL              5 (NULL + datetime)
                       60 LOAD_ATTR                2 (datetime)
                       70 LOAD_CONST               5 (2001)
                       72 LOAD_CONST               6 (1)
                       74 LOAD_CONST               6 (1)
                       76 LOAD_CONST               7 (0)
                       78 LOAD_CONST               7 (0)
                       80 LOAD_CONST               8 (5)
                       82 PRECALL                  6
                       86 CALL                     6
                       96 STORE_FAST               1 (curtime)
          
-         493          98 LOAD_FAST                0 (rate)
+         502          98 LOAD_FAST                0 (rate)
                      100 LOAD_METHOD              3 (nexttime)
                      122 LOAD_FAST                1 (curtime)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_FAST               2 (wait)
          
-         494         140 LOAD_FAST                2 (wait)
+         503         140 LOAD_FAST                2 (wait)
                      142 LOAD_ATTR                4 (total_seconds)
                      152 STORE_FAST               3 (@py_assert1)
                      154 PUSH_NULL
                      156 LOAD_FAST                3 (@py_assert1)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 STORE_FAST               4 (@py_assert3)
@@ -10421,15 +10539,15 @@
             'py9'
          names      ('sapphire', 'Rate', 'datetime', 'nexttime', 'total_seconds', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('rate', 'curtime', 'wait', '@py_assert1', '@py_assert3', '@py_assert6', '@py_assert5', '@py_format8', '@py_format10')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_nexttime_offset_sync'
-         firstlineno 488
+         firstlineno 497
          lnotab 0x02012e0232022a01
       code
          argcount  : 0
          nlocals   : 9
          stacksize : 8
          flags     : 3
          code
@@ -10449,46 +10567,46 @@
             007c03a6010000ab010000000000000000740b000000000000000000006a
             0a00000000000000007c04a6010000ab010000000000000000740b000000
             000000000000006a0a00000000000000007c05a6010000ab010000000000
             000000640d9c047a0600007d07640e640f7c0769017a0600007d08741700
             000000000000000000740b000000000000000000006a0c00000000000000
             007c08a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d0378017d0478017d067d0564005300
-         496           0 RESUME                   0
+         505           0 RESUME                   0
          
-         497           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         506           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Rate)
                       24 LOAD_CONST               1 (60)
                       26 LOAD_CONST               2 (10)
                       28 LOAD_CONST               3 (True)
                       30 KW_NAMES                 4
                       32 PRECALL                  3
                       36 CALL                     3
                       46 STORE_FAST               0 (rate)
          
-         499          48 LOAD_GLOBAL              5 (NULL + datetime)
+         508          48 LOAD_GLOBAL              5 (NULL + datetime)
                       60 LOAD_ATTR                2 (datetime)
                       70 LOAD_CONST               5 (2001)
                       72 LOAD_CONST               6 (1)
                       74 LOAD_CONST               6 (1)
                       76 LOAD_CONST               7 (0)
                       78 LOAD_CONST               7 (0)
                       80 LOAD_CONST               8 (15)
                       82 PRECALL                  6
                       86 CALL                     6
                       96 STORE_FAST               1 (curtime)
          
-         501          98 LOAD_FAST                0 (rate)
+         510          98 LOAD_FAST                0 (rate)
                      100 LOAD_METHOD              3 (nexttime)
                      122 LOAD_FAST                1 (curtime)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_FAST               2 (wait)
          
-         502         140 LOAD_FAST                2 (wait)
+         511         140 LOAD_FAST                2 (wait)
                      142 LOAD_ATTR                4 (total_seconds)
                      152 STORE_FAST               3 (@py_assert1)
                      154 PUSH_NULL
                      156 LOAD_FAST                3 (@py_assert1)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 STORE_FAST               4 (@py_assert3)
@@ -10594,15 +10712,15 @@
             'py9'
          names      ('sapphire', 'Rate', 'datetime', 'nexttime', 'total_seconds', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('rate', 'curtime', 'wait', '@py_assert1', '@py_assert3', '@py_assert6', '@py_assert5', '@py_format8', '@py_format10')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_rate_nexttime_offset_sync2'
-         firstlineno 496
+         firstlineno 505
          lnotab 0x02012e0232022a01
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
@@ -10626,45 +10744,45 @@
             000000740a00000000000000000000a6010000ab01000000000000000072
             197411000000000000000000006a0a0000000000000000740a0000000000
             0000000000a6010000ab0100000000000000006e01640874110000000000
             00000000006a0a00000000000000007c02a6010000ab0100000000000000
             0064099c047a0600007d0374170000000000000000000074110000000000
             00000000006a0c00000000000000007c03a6010000ab0100000000000000
             00a6010000ab010000000000000000820164007d0264005300
-         504           0 RESUME                   0
+         513           0 RESUME                   0
          
-         505           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         514           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         506          40 BUILD_MAP                0
+         515          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         507          50 LOAD_CONST               2 ('a b')
+         516          50 LOAD_CONST               2 ('a b')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('components')
                       68 STORE_SUBSCR
          
-         509          72 LOAD_FAST                0 (config)
+         518          72 LOAD_FAST                0 (config)
                       74 LOAD_METHOD              2 (get_components)
                       96 LOAD_CONST               1 ('section')
                       98 LOAD_CONST               3 ('components')
                      100 LOAD_GLOBAL              6 (Factory)
                      112 KW_NAMES                 4
                      114 PRECALL                  3
                      118 CALL                     3
                      128 STORE_FAST               1 (result)
          
-         510         130 LOAD_GLOBAL              9 (NULL + isinstance)
+         519         130 LOAD_GLOBAL              9 (NULL + isinstance)
                      142 LOAD_FAST                1 (result)
                      144 LOAD_GLOBAL             10 (dict)
                      156 PRECALL                  2
                      160 CALL                     2
                      170 STORE_FAST               2 (@py_assert3)
                      172 LOAD_FAST                2 (@py_assert3)
                      174 EXTENDED_ARG             1
@@ -10765,15 +10883,15 @@
             ('py0', 'py1', 'py2', 'py4')
          names      ('sapphire', 'Parser', 'get_components', 'Factory', 'isinstance', 'dict', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_components'
-         firstlineno 504
+         firstlineno 513
          lnotab 0x020126010a0116023a01
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
@@ -10798,46 +10916,46 @@
             01000000000000000072197411000000000000000000006a0a0000000000
             000000740a00000000000000000000a6010000ab0100000000000000006e
             0164087411000000000000000000006a0a00000000000000007c02a60100
             00ab01000000000000000064099c047a0600007d03741700000000000000
             0000007411000000000000000000006a0c00000000000000007c03a60100
             00ab010000000000000000a6010000ab010000000000000000820164007d
             0264005300
-         512           0 RESUME                   0
+         521           0 RESUME                   0
          
-         513           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         522           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         514          40 BUILD_MAP                0
+         523          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         515          50 LOAD_CONST               2 ('a b')
+         524          50 LOAD_CONST               2 ('a b')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('components')
                       68 STORE_SUBSCR
          
-         517          72 LOAD_FAST                0 (config)
+         526          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get_components)
                      108 LOAD_CONST               3 ('components')
                      110 LOAD_GLOBAL              6 (Factory)
                      122 KW_NAMES                 4
                      124 PRECALL                  2
                      128 CALL                     2
                      138 STORE_FAST               1 (result)
          
-         518         140 LOAD_GLOBAL              9 (NULL + isinstance)
+         527         140 LOAD_GLOBAL              9 (NULL + isinstance)
                      152 LOAD_FAST                1 (result)
                      154 LOAD_GLOBAL             10 (dict)
                      166 PRECALL                  2
                      170 CALL                     2
                      180 STORE_FAST               2 (@py_assert3)
                      182 LOAD_FAST                2 (@py_assert3)
                      184 EXTENDED_ARG             1
@@ -10938,18 +11056,354 @@
             ('py0', 'py1', 'py2', 'py4')
          names      ('sapphire', 'Parser', 'get_components', 'Factory', 'isinstance', 'dict', '@py_builtins', 'locals', '@pytest_ar', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_components_proxy'
-         firstlineno 512
+         firstlineno 521
          lnotab 0x020126010a0116024401
       code
          argcount  : 0
+         nlocals   : 11
+         stacksize : 9
+         flags     : 3
+         code
+            0x97007401000000000000000000006a010000000000000000a6000000ab
+            0000000000000000007d0069007c0064013c00000064027c006401190000
+            0000000000000064033c0000007c00a00200000000000000000000000000
+            0000000000000064016403740600000000000000000000ac04a6030000ab
+            0300000000000000007d017c016405190000000000000000007d027c026a
+            0400000000000000007d037c036a0500000000000000007d0464067d0502
+            007c047c05a6010000ab0100000000000000007d0664077d077c067c076b
+            02000000007d087c0873b8740d000000000000000000006a070000000000
+            00000064087c08660164097c067c076602a6040000ab0400000000000000
+            00740d000000000000000000006a0800000000000000007c02a6010000ab
+            010000000000000000740d000000000000000000006a0800000000000000
+            007c03a6010000ab010000000000000000740d000000000000000000006a
+            0800000000000000007c04a6010000ab010000000000000000740d000000
+            000000000000006a0800000000000000007c05a6010000ab010000000000
+            000000740d000000000000000000006a0800000000000000007c06a60100
+            00ab010000000000000000740d000000000000000000006a080000000000
+            0000007c07a6010000ab010000000000000000640a9c067a0600007d0964
+            0b640c7c0969017a0600007d0a741300000000000000000000740d000000
+            000000000000006a0a00000000000000007c0aa6010000ab010000000000
+            000000a6010000ab0100000000000000008201640078017d0278017d0378
+            017d0478017d0578017d0678017d087d0764005300
+         529           0 RESUME                   0
+         
+         530           2 LOAD_GLOBAL              1 (NULL + sapphire)
+                      14 LOAD_ATTR                1 (Parser)
+                      24 PRECALL                  0
+                      28 CALL                     0
+                      38 STORE_FAST               0 (config)
+         
+         531          40 BUILD_MAP                0
+                      42 LOAD_FAST                0 (config)
+                      44 LOAD_CONST               1 ('section')
+                      46 STORE_SUBSCR
+         
+         532          50 LOAD_CONST               2 ('a b')
+                      52 LOAD_FAST                0 (config)
+                      54 LOAD_CONST               1 ('section')
+                      56 BINARY_SUBSCR
+                      66 LOAD_CONST               3 ('components')
+                      68 STORE_SUBSCR
+         
+         534          72 LOAD_FAST                0 (config)
+                      74 LOAD_METHOD              2 (get_components)
+                      96 LOAD_CONST               1 ('section')
+                      98 LOAD_CONST               3 ('components')
+                     100 LOAD_GLOBAL              6 (FactorySet)
+                     112 KW_NAMES                 4
+                     114 PRECALL                  3
+                     118 CALL                     3
+                     128 STORE_FAST               1 (result)
+         
+         535         130 LOAD_FAST                1 (result)
+                     132 LOAD_CONST               5 ('a')
+                     134 BINARY_SUBSCR
+                     144 STORE_FAST               2 (@py_assert0)
+                     146 LOAD_FAST                2 (@py_assert0)
+                     148 LOAD_ATTR                4 (config)
+                     158 STORE_FAST               3 (@py_assert2)
+                     160 LOAD_FAST                3 (@py_assert2)
+                     162 LOAD_ATTR                5 (get)
+                     172 STORE_FAST               4 (@py_assert4)
+                     174 LOAD_CONST               6 ('setname')
+                     176 STORE_FAST               5 (@py_assert6)
+                     178 PUSH_NULL
+                     180 LOAD_FAST                4 (@py_assert4)
+                     182 LOAD_FAST                5 (@py_assert6)
+                     184 PRECALL                  1
+                     188 CALL                     1
+                     198 STORE_FAST               6 (@py_assert8)
+                     200 LOAD_CONST               7 ('setname.a')
+                     202 STORE_FAST               7 (@py_assert11)
+                     204 LOAD_FAST                6 (@py_assert8)
+                     206 LOAD_FAST                7 (@py_assert11)
+                     208 COMPARE_OP               2 (==)
+                     214 STORE_FAST               8 (@py_assert10)
+                     216 LOAD_FAST                8 (@py_assert10)
+                     218 POP_JUMP_FORWARD_IF_TRUE   184 (to 588)
+                     220 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     232 LOAD_ATTR                7 (_call_reprcompare)
+                     242 LOAD_CONST               8 (('==',))
+                     244 LOAD_FAST                8 (@py_assert10)
+                     246 BUILD_TUPLE              1
+                     248 LOAD_CONST               9 (('%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s\n{%(py3)s = %(py1)s.config\n}.get\n}(%(py7)s)\n} == %(py12)s',))
+                     250 LOAD_FAST                6 (@py_assert8)
+                     252 LOAD_FAST                7 (@py_assert11)
+                     254 BUILD_TUPLE              2
+                     256 PRECALL                  4
+                     260 CALL                     4
+                     270 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     282 LOAD_ATTR                8 (_saferepr)
+                     292 LOAD_FAST                2 (@py_assert0)
+                     294 PRECALL                  1
+                     298 CALL                     1
+                     308 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     320 LOAD_ATTR                8 (_saferepr)
+                     330 LOAD_FAST                3 (@py_assert2)
+                     332 PRECALL                  1
+                     336 CALL                     1
+                     346 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     358 LOAD_ATTR                8 (_saferepr)
+                     368 LOAD_FAST                4 (@py_assert4)
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     396 LOAD_ATTR                8 (_saferepr)
+                     406 LOAD_FAST                5 (@py_assert6)
+                     408 PRECALL                  1
+                     412 CALL                     1
+                     422 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     434 LOAD_ATTR                8 (_saferepr)
+                     444 LOAD_FAST                6 (@py_assert8)
+                     446 PRECALL                  1
+                     450 CALL                     1
+                     460 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     472 LOAD_ATTR                8 (_saferepr)
+                     482 LOAD_FAST                7 (@py_assert11)
+                     484 PRECALL                  1
+                     488 CALL                     1
+                     498 LOAD_CONST              10 (('py1', 'py3', 'py5', 'py7', 'py9', 'py12'))
+                     500 BUILD_CONST_KEY_MAP      6
+                     502 BINARY_OP                6 (%)
+                     506 STORE_FAST               9 (@py_format13)
+                     508 LOAD_CONST              11 ('assert %(py14)s')
+                     510 LOAD_CONST              12 ('py14')
+                     512 LOAD_FAST                9 (@py_format13)
+                     514 BUILD_MAP                1
+                     516 BINARY_OP                6 (%)
+                     520 STORE_FAST              10 (@py_format15)
+                     522 LOAD_GLOBAL             19 (NULL + AssertionError)
+                     534 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     546 LOAD_ATTR               10 (_format_explanation)
+                     556 LOAD_FAST               10 (@py_format15)
+                     558 PRECALL                  1
+                     562 CALL                     1
+                     572 PRECALL                  1
+                     576 CALL                     1
+                     586 RAISE_VARARGS            1
+                 >>  588 LOAD_CONST               0 (None)
+                     590 COPY                     1
+                     592 STORE_FAST               2 (@py_assert0)
+                     594 COPY                     1
+                     596 STORE_FAST               3 (@py_assert2)
+                     598 COPY                     1
+                     600 STORE_FAST               4 (@py_assert4)
+                     602 COPY                     1
+                     604 STORE_FAST               5 (@py_assert6)
+                     606 COPY                     1
+                     608 STORE_FAST               6 (@py_assert8)
+                     610 COPY                     1
+                     612 STORE_FAST               8 (@py_assert10)
+                     614 STORE_FAST               7 (@py_assert11)
+                     616 LOAD_CONST               0 (None)
+                     618 RETURN_VALUE
+         consts
+            None
+            'section'
+            'a b'
+            'components'
+            ('factory',)
+            'a'
+            'setname'
+            'setname.a'
+            ('==',)
+            ('%(py9)s\n{%(py9)s = %(py5)s\n{%(py5)s = %(py3)s\n{%(py3)s = %(py1)s.config\n}.get\n}(%(py7)s)\n} == %(py12)s',)
+            ('py1', 'py3', 'py5', 'py7', 'py9', 'py12')
+            'assert %(py14)s'
+            'py14'
+         names      ('sapphire', 'Parser', 'get_components', 'FactorySet', 'config', 'get', '@pytest_ar', '_call_reprcompare', '_saferepr', 'AssertionError', '_format_explanation')
+         varnames   ('config', 'result', '@py_assert0', '@py_assert2', '@py_assert4', '@py_assert6', '@py_assert8', '@py_assert11', '@py_assert10', '@py_format13', '@py_format15')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
+         name       'test_component_set'
+         firstlineno 529
+         lnotab 0x020126010a0116023a01
+      code
+         argcount  : 0
+         nlocals   : 7
+         stacksize : 7
+         flags     : 3
+         code
+            0x97007401000000000000000000006a010000000000000000a6000000ab
+            0000000000000000007d0069007c0064013c00000064027c006401190000
+            0000000000000064033c0000007c00a00200000000000000000000000000
+            0000000000000064016403740600000000000000000000ac04a6030000ab
+            0300000000000000007d017c016402190000000000000000006a04000000
+            0000000000a0050000000000000000000000000000000000000000a60000
+            00ab0000000000000000007d0267006405a2017d037c027c036b02000000
+            007d047c047397740d000000000000000000006a07000000000000000064
+            067c04660164077c027c036602a6040000ab040000000000000000640874
+            11000000000000000000006a090000000000000000a6000000ab00000000
+            000000000076007314740d000000000000000000006a0a00000000000000
+            007c02a6010000ab0100000000000000007214740d000000000000000000
+            006a0b00000000000000007c02a6010000ab0100000000000000006e0164
+            08740d000000000000000000006a0b00000000000000007c03a6010000ab
+            01000000000000000064099c027a0600007d05640a640b7c0569017a0600
+            007d06741900000000000000000000740d000000000000000000006a0d00
+            000000000000007c06a6010000ab010000000000000000a6010000ab0100
+            000000000000008201640078017d047d0364005300
+         537           0 RESUME                   0
+         
+         538           2 LOAD_GLOBAL              1 (NULL + sapphire)
+                      14 LOAD_ATTR                1 (Parser)
+                      24 PRECALL                  0
+                      28 CALL                     0
+                      38 STORE_FAST               0 (config)
+         
+         539          40 BUILD_MAP                0
+                      42 LOAD_FAST                0 (config)
+                      44 LOAD_CONST               1 ('section')
+                      46 STORE_SUBSCR
+         
+         540          50 LOAD_CONST               2 ('a')
+                      52 LOAD_FAST                0 (config)
+                      54 LOAD_CONST               1 ('section')
+                      56 BINARY_SUBSCR
+                      66 LOAD_CONST               3 ('components')
+                      68 STORE_SUBSCR
+         
+         542          72 LOAD_FAST                0 (config)
+                      74 LOAD_METHOD              2 (get_components)
+                      96 LOAD_CONST               1 ('section')
+                      98 LOAD_CONST               3 ('components')
+                     100 LOAD_GLOBAL              6 (FactorySet)
+                     112 KW_NAMES                 4
+                     114 PRECALL                  3
+                     118 CALL                     3
+                     128 STORE_FAST               1 (c)
+         
+         543         130 LOAD_FAST                1 (c)
+                     132 LOAD_CONST               2 ('a')
+                     134 BINARY_SUBSCR
+                     144 LOAD_ATTR                4 (config)
+                     154 LOAD_METHOD              5 (options)
+                     176 PRECALL                  0
+                     180 CALL                     0
+                     190 STORE_FAST               2 (options)
+         
+         545         192 BUILD_LIST               0
+                     194 LOAD_CONST               5 (('name', 'component', 'setname', 'components'))
+                     196 LIST_EXTEND              1
+                     198 STORE_FAST               3 (@py_assert2)
+                     200 LOAD_FAST                2 (options)
+                     202 LOAD_FAST                3 (@py_assert2)
+                     204 COMPARE_OP               2 (==)
+                     210 STORE_FAST               4 (@py_assert1)
+                     212 LOAD_FAST                4 (@py_assert1)
+                     214 POP_JUMP_FORWARD_IF_TRUE   151 (to 518)
+                     216 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     228 LOAD_ATTR                7 (_call_reprcompare)
+                     238 LOAD_CONST               6 (('==',))
+                     240 LOAD_FAST                4 (@py_assert1)
+                     242 BUILD_TUPLE              1
+                     244 LOAD_CONST               7 (('%(py0)s == %(py3)s',))
+                     246 LOAD_FAST                2 (options)
+                     248 LOAD_FAST                3 (@py_assert2)
+                     250 BUILD_TUPLE              2
+                     252 PRECALL                  4
+                     256 CALL                     4
+                     266 LOAD_CONST               8 ('options')
+                     268 LOAD_GLOBAL             17 (NULL + @py_builtins)
+                     280 LOAD_ATTR                9 (locals)
+                     290 PRECALL                  0
+                     294 CALL                     0
+                     304 CONTAINS_OP              0
+                     306 POP_JUMP_FORWARD_IF_TRUE    20 (to 348)
+                     308 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     320 LOAD_ATTR               10 (_should_repr_global_name)
+                     330 LOAD_FAST                2 (options)
+                     332 PRECALL                  1
+                     336 CALL                     1
+                     346 POP_JUMP_FORWARD_IF_FALSE    20 (to 388)
+                 >>  348 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     360 LOAD_ATTR               11 (_saferepr)
+                     370 LOAD_FAST                2 (options)
+                     372 PRECALL                  1
+                     376 CALL                     1
+                     386 JUMP_FORWARD             1 (to 390)
+                 >>  388 LOAD_CONST               8 ('options')
+                 >>  390 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     402 LOAD_ATTR               11 (_saferepr)
+                     412 LOAD_FAST                3 (@py_assert2)
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 LOAD_CONST               9 (('py0', 'py3'))
+                     430 BUILD_CONST_KEY_MAP      2
+                     432 BINARY_OP                6 (%)
+                     436 STORE_FAST               5 (@py_format4)
+                     438 LOAD_CONST              10 ('assert %(py5)s')
+                     440 LOAD_CONST              11 ('py5')
+                     442 LOAD_FAST                5 (@py_format4)
+                     444 BUILD_MAP                1
+                     446 BINARY_OP                6 (%)
+                     450 STORE_FAST               6 (@py_format6)
+                     452 LOAD_GLOBAL             25 (NULL + AssertionError)
+                     464 LOAD_GLOBAL             13 (NULL + @pytest_ar)
+                     476 LOAD_ATTR               13 (_format_explanation)
+                     486 LOAD_FAST                6 (@py_format6)
+                     488 PRECALL                  1
+                     492 CALL                     1
+                     502 PRECALL                  1
+                     506 CALL                     1
+                     516 RAISE_VARARGS            1
+                 >>  518 LOAD_CONST               0 (None)
+                     520 COPY                     1
+                     522 STORE_FAST               4 (@py_assert1)
+                     524 STORE_FAST               3 (@py_assert2)
+                     526 LOAD_CONST               0 (None)
+                     528 RETURN_VALUE
+         consts
+            None
+            'section'
+            'a'
+            'components'
+            ('factory',)
+            ('name', 'component', 'setname', 'components')
+            ('==',)
+            ('%(py0)s == %(py3)s',)
+            'options'
+            ('py0', 'py3')
+            'assert %(py5)s'
+            'py5'
+         names      ('sapphire', 'Parser', 'get_components', 'FactorySet', 'config', 'options', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
+         varnames   ('config', 'c', 'options', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
+         name       'test_component_options'
+         firstlineno 537
+         lnotab 0x020126010a0116023a013e02
+      code
+         argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d0069007c0064013c00000064027c006401190000
             0000000000000064033c00000064047c0064011900000000000000000064
@@ -10969,58 +11423,58 @@
             00000000006a0a0000000000000000740600000000000000000000a60100
             00ab0100000000000000006e016402740b000000000000000000006a0a00
             000000000000007c02a6010000ab010000000000000000640b9c037a0600
             007d04640c640d7c0469017a0600007d0574170000000000000000000074
             0b000000000000000000006a0c00000000000000007c05a6010000ab0100
             00000000000000a6010000ab0100000000000000008201640078017d037d
             0264005300
-         520           0 RESUME                   0
+         547           0 RESUME                   0
          
-         521           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         548           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         522          40 BUILD_MAP                0
+         549          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         523          50 LOAD_CONST               2 ('os')
+         550          50 LOAD_CONST               2 ('os')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('callback.module')
                       68 STORE_SUBSCR
          
-         524          72 LOAD_CONST               4 ('cpu_count')
+         551          72 LOAD_CONST               4 ('cpu_count')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('callback.function')
                       90 STORE_SUBSCR
          
-         525          94 LOAD_CONST               4 ('cpu_count')
+         552          94 LOAD_CONST               4 ('cpu_count')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               6 ('callback.init')
                      112 STORE_SUBSCR
          
-         527         116 LOAD_FAST                0 (config)
+         554         116 LOAD_FAST                0 (config)
                      118 LOAD_CONST               1 ('section')
                      120 BINARY_SUBSCR
                      130 LOAD_METHOD              2 (get_callback)
                      152 LOAD_CONST               7 ('callback')
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               1 (result)
          
-         528         170 LOAD_GLOBAL              6 (os)
+         555         170 LOAD_GLOBAL              6 (os)
                      182 LOAD_ATTR                4 (cpu_count)
                      192 STORE_FAST               2 (@py_assert3)
                      194 LOAD_FAST                1 (result)
                      196 LOAD_FAST                2 (@py_assert3)
                      198 IS_OP                    0
                      200 STORE_FAST               3 (@py_assert1)
                      202 LOAD_FAST                3 (@py_assert1)
@@ -11123,15 +11577,15 @@
             'py6'
          names      ('sapphire', 'Parser', 'get_callback', 'os', 'cpu_count', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert3', '@py_assert1', '@py_format5', '@py_format7')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_callback'
-         firstlineno 520
+         firstlineno 547
          lnotab 0x020126010a011601160116023601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -11148,57 +11602,57 @@
             00ab01000000000000000072147407000000000000000000006a08000000
             00000000007c01a6010000ab0100000000000000006e01640a7407000000
             000000000000006a0800000000000000007c02a6010000ab010000000000
             000000640b9c027a0600007d04640c640d7c0469017a0600007d05741300
             0000000000000000007407000000000000000000006a0a00000000000000
             007c05a6010000ab010000000000000000a6010000ab0100000000000000
             008201640078017d037d0264005300
-         530           0 RESUME                   0
+         557           0 RESUME                   0
          
-         531           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         558           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         532          40 BUILD_MAP                0
+         559          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         533          50 LOAD_CONST               2 ('a')
+         560          50 LOAD_CONST               2 ('a')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('base.name')
                       68 STORE_SUBSCR
          
-         534          72 LOAD_CONST               4 ('name')
+         561          72 LOAD_CONST               4 ('name')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('opt')
                       90 STORE_SUBSCR
          
-         535          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
+         562          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('path')
                      112 STORE_SUBSCR
          
-         537         116 LOAD_FAST                0 (config)
+         564         116 LOAD_FAST                0 (config)
                      118 LOAD_METHOD              2 (get)
                      140 LOAD_CONST               1 ('section')
                      142 LOAD_CONST               7 ('path')
                      144 PRECALL                  2
                      148 CALL                     2
                      158 STORE_FAST               1 (result)
          
-         538         160 LOAD_CONST               2 ('a')
+         565         160 LOAD_CONST               2 ('a')
                      162 STORE_FAST               2 (@py_assert2)
                      164 LOAD_FAST                1 (result)
                      166 LOAD_FAST                2 (@py_assert2)
                      168 COMPARE_OP               2 (==)
                      174 STORE_FAST               3 (@py_assert1)
                      176 LOAD_FAST                3 (@py_assert1)
                      178 POP_JUMP_FORWARD_IF_TRUE   151 (to 482)
@@ -11280,15 +11734,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_interpolation'
-         firstlineno 530
+         firstlineno 557
          lnotab 0x020126010a011601160116022c01
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -11304,56 +11758,56 @@
             0600000000000000007c01a6010000ab0100000000000000007214740500
             0000000000000000006a0700000000000000007c01a6010000ab01000000
             00000000006e01640a7405000000000000000000006a0700000000000000
             007c02a6010000ab010000000000000000640b9c027a0600007d04640c64
             0d7c0469017a0600007d0574110000000000000000000074050000000000
             00000000006a0900000000000000007c05a6010000ab0100000000000000
             00a6010000ab0100000000000000008201640078017d037d0264005300
-         540           0 RESUME                   0
+         567           0 RESUME                   0
          
-         541           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         568           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         542          40 BUILD_MAP                0
+         569          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         543          50 LOAD_CONST               2 ('a')
+         570          50 LOAD_CONST               2 ('a')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('base.name')
                       68 STORE_SUBSCR
          
-         544          72 LOAD_CONST               4 ('name')
+         571          72 LOAD_CONST               4 ('name')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('opt')
                       90 STORE_SUBSCR
          
-         545          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
+         572          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('path')
                      112 STORE_SUBSCR
          
-         547         116 LOAD_FAST                0 (config)
+         574         116 LOAD_FAST                0 (config)
                      118 LOAD_CONST               1 ('section')
                      120 BINARY_SUBSCR
                      130 LOAD_CONST               7 ('path')
                      132 BINARY_SUBSCR
                      142 STORE_FAST               1 (result)
          
-         548         144 LOAD_CONST               2 ('a')
+         575         144 LOAD_CONST               2 ('a')
                      146 STORE_FAST               2 (@py_assert2)
                      148 LOAD_FAST                1 (result)
                      150 LOAD_FAST                2 (@py_assert2)
                      152 COMPARE_OP               2 (==)
                      158 STORE_FAST               3 (@py_assert1)
                      160 LOAD_FAST                3 (@py_assert1)
                      162 POP_JUMP_FORWARD_IF_TRUE   151 (to 466)
@@ -11435,15 +11889,15 @@
             'py5'
          names      ('sapphire', 'Parser', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_interpolation_proxy'
-         firstlineno 540
+         firstlineno 567
          lnotab 0x020126010a011601160116021c01
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -11452,65 +11906,65 @@
             0000000000000064033c00000064047c0064011900000000000000000064
             053c00000064067c0064011900000000000000000064073c000000740500
             0000000000000000006a0300000000000000007408000000000000000000
             006a050000000000000000a6010000ab010000000000000000350001007c
             006401190000000000000000006407190000000000000000007d01640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         550           0 RESUME                   0
+         577           0 RESUME                   0
          
-         551           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         578           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         552          40 BUILD_MAP                0
+         579          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         553          50 LOAD_CONST               2 ('%(path)')
+         580          50 LOAD_CONST               2 ('%(path)')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('base.name')
                       68 STORE_SUBSCR
          
-         554          72 LOAD_CONST               4 ('name')
+         581          72 LOAD_CONST               4 ('name')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('opt')
                       90 STORE_SUBSCR
          
-         555          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
+         582          94 LOAD_CONST               6 ('%(base.%(opt)s)s')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('path')
                      112 STORE_SUBSCR
          
-         557         116 LOAD_GLOBAL              5 (NULL + pytest)
+         584         116 LOAD_GLOBAL              5 (NULL + pytest)
                      128 LOAD_ATTR                3 (raises)
                      138 LOAD_GLOBAL              8 (configparser)
                      150 LOAD_ATTR                5 (InterpolationDepthError)
                      160 PRECALL                  1
                      164 CALL                     1
                      174 BEFORE_WITH
                      176 POP_TOP
          
-         558         178 LOAD_FAST                0 (config)
+         585         178 LOAD_FAST                0 (config)
                      180 LOAD_CONST               1 ('section')
                      182 BINARY_SUBSCR
                      192 LOAD_CONST               7 ('path')
                      194 BINARY_SUBSCR
                      204 STORE_FAST               1 (_result)
          
-         557         206 LOAD_CONST               0 (None)
+         584         206 LOAD_CONST               0 (None)
                      208 LOAD_CONST               0 (None)
                      210 LOAD_CONST               0 (None)
                      212 PRECALL                  2
                      216 CALL                     2
                      226 POP_TOP
                      228 LOAD_CONST               0 (None)
                      230 RETURN_VALUE
@@ -11542,15 +11996,15 @@
             'path'
          names      ('sapphire', 'Parser', 'pytest', 'raises', 'configparser', 'InterpolationDepthError')
          varnames   ('config', '_result')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_get_interpolation_loop'
-         firstlineno 550
+         firstlineno 577
          lnotab 0x020126010a011601160116023e011cff
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -11571,77 +12025,77 @@
             007214740d000000000000000000006a0b00000000000000007c02a60100
             00ab0100000000000000006e01640f740d000000000000000000006a0b00
             000000000000007c03a6010000ab01000000000000000064109c027a0600
             007d05641164127c0569017a0600007d0674190000000000000000000074
             0d000000000000000000006a0d00000000000000007c06a6010000ab0100
             00000000000000a6010000ab0100000000000000008201640078017d047d
             0364005300
-         560           0 RESUME                   0
+         587           0 RESUME                   0
          
-         561           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         588           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         562          40 BUILD_MAP                0
+         589          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         563          50 LOAD_CONST               2 ('base key1')
+         590          50 LOAD_CONST               2 ('base key1')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('base.mixin.key1')
                       68 STORE_SUBSCR
          
-         564          72 LOAD_CONST               4 ('a b')
+         591          72 LOAD_CONST               4 ('a b')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('components')
                       90 STORE_SUBSCR
          
-         565          94 LOAD_CONST               6 ('base.mixin')
+         592          94 LOAD_CONST               6 ('base.mixin')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('component.a.mixin')
                      112 STORE_SUBSCR
          
-         566         116 LOAD_CONST               8 ('a key1')
+         593         116 LOAD_CONST               8 ('a key1')
                      118 LOAD_FAST                0 (config)
                      120 LOAD_CONST               1 ('section')
                      122 BINARY_SUBSCR
                      132 LOAD_CONST               9 ('component.a.key1')
                      134 STORE_SUBSCR
          
-         568         138 LOAD_FAST                0 (config)
+         595         138 LOAD_FAST                0 (config)
                      140 LOAD_CONST               1 ('section')
                      142 BINARY_SUBSCR
                      152 LOAD_METHOD              2 (get_components)
                      174 LOAD_CONST               5 ('components')
                      176 LOAD_GLOBAL              6 (Factory)
                      188 KW_NAMES                10
                      190 PRECALL                  2
                      194 CALL                     2
                      204 STORE_FAST               1 (components)
          
-         569         206 LOAD_FAST                1 (components)
+         596         206 LOAD_FAST                1 (components)
                      208 LOAD_CONST              11 ('a')
                      210 BINARY_SUBSCR
                      220 LOAD_ATTR                4 (config)
                      230 LOAD_METHOD              5 (get)
                      252 LOAD_CONST              12 ('key1')
                      254 PRECALL                  1
                      258 CALL                     1
                      268 STORE_FAST               2 (result)
          
-         570         270 LOAD_CONST               8 ('a key1')
+         597         270 LOAD_CONST               8 ('a key1')
                      272 STORE_FAST               3 (@py_assert2)
                      274 LOAD_FAST                2 (result)
                      276 LOAD_FAST                3 (@py_assert2)
                      278 COMPARE_OP               2 (==)
                      284 STORE_FAST               4 (@py_assert1)
                      286 LOAD_FAST                4 (@py_assert1)
                      288 POP_JUMP_FORWARD_IF_TRUE   151 (to 592)
@@ -11728,15 +12182,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_components', 'Factory', 'config', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'components', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_component_mixin'
-         firstlineno 560
+         firstlineno 587
          lnotab 0x020126010a01160116011601160244014001
       code
          argcount  : 0
          nlocals   : 7
          stacksize : 7
          flags     : 3
          code
@@ -11756,70 +12210,70 @@
             0100000000000000007214740d000000000000000000006a0b0000000000
             0000007c02a6010000ab0100000000000000006e01640d740d0000000000
             00000000006a0b00000000000000007c03a6010000ab0100000000000000
             00640e9c027a0600007d05640f64107c0569017a0600007d067419000000
             00000000000000740d000000000000000000006a0d00000000000000007c
             06a6010000ab010000000000000000a6010000ab01000000000000000082
             01640078017d047d0364005300
-         572           0 RESUME                   0
+         599           0 RESUME                   0
          
-         573           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         600           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         574          40 BUILD_MAP                0
+         601          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         575          50 LOAD_CONST               2 ('base key1')
+         602          50 LOAD_CONST               2 ('base key1')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('base.mixin.key1')
                       68 STORE_SUBSCR
          
-         576          72 LOAD_CONST               4 ('a b')
+         603          72 LOAD_CONST               4 ('a b')
                       74 LOAD_FAST                0 (config)
                       76 LOAD_CONST               1 ('section')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               5 ('components')
                       90 STORE_SUBSCR
          
-         577          94 LOAD_CONST               6 ('base.mixin')
+         604          94 LOAD_CONST               6 ('base.mixin')
                       96 LOAD_FAST                0 (config)
                       98 LOAD_CONST               1 ('section')
                      100 BINARY_SUBSCR
                      110 LOAD_CONST               7 ('component.a.mixin')
                      112 STORE_SUBSCR
          
-         579         116 LOAD_FAST                0 (config)
+         606         116 LOAD_FAST                0 (config)
                      118 LOAD_CONST               1 ('section')
                      120 BINARY_SUBSCR
                      130 LOAD_METHOD              2 (get_components)
                      152 LOAD_CONST               5 ('components')
                      154 LOAD_GLOBAL              6 (Factory)
                      166 KW_NAMES                 8
                      168 PRECALL                  2
                      172 CALL                     2
                      182 STORE_FAST               1 (components)
          
-         580         184 LOAD_FAST                1 (components)
+         607         184 LOAD_FAST                1 (components)
                      186 LOAD_CONST               9 ('a')
                      188 BINARY_SUBSCR
                      198 LOAD_ATTR                4 (config)
                      208 LOAD_METHOD              5 (get)
                      230 LOAD_CONST              10 ('key1')
                      232 PRECALL                  1
                      236 CALL                     1
                      246 STORE_FAST               2 (result)
          
-         581         248 LOAD_CONST               2 ('base key1')
+         608         248 LOAD_CONST               2 ('base key1')
                      250 STORE_FAST               3 (@py_assert2)
                      252 LOAD_FAST                2 (result)
                      254 LOAD_FAST                3 (@py_assert2)
                      256 COMPARE_OP               2 (==)
                      262 STORE_FAST               4 (@py_assert1)
                      264 LOAD_FAST                4 (@py_assert1)
                      266 POP_JUMP_FORWARD_IF_TRUE   151 (to 570)
@@ -11904,15 +12358,15 @@
             'py5'
          names      ('sapphire', 'Parser', 'get_components', 'Factory', 'config', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'components', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_component_mixin_default'
-         firstlineno 572
+         firstlineno 599
          lnotab 0x020126010a0116011601160244014001
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -11932,51 +12386,51 @@
             147409000000000000000000006a0800000000000000007c01a6010000ab
             01000000000000000072147409000000000000000000006a090000000000
             0000007c01a6010000ab0100000000000000006e016409640a9c027a0600
             007d04640b640c7c0469017a0600007d0574150000000000000000000074
             09000000000000000000006a0b00000000000000007c05a6010000ab0100
             00000000000000a6010000ab010000000000000000820164007d03640053
             00
-         583           0 RESUME                   0
+         610           0 RESUME                   0
          
-         584           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         611           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         585          40 BUILD_MAP                0
+         612          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         586          50 LOAD_CONST               2 ('10')
+         613          50 LOAD_CONST               2 ('10')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('timespan')
                       68 STORE_SUBSCR
          
-         588          72 LOAD_GLOBAL              5 (NULL + relativedelta)
+         615          72 LOAD_GLOBAL              5 (NULL + relativedelta)
                       84 LOAD_CONST               4 (10)
                       86 KW_NAMES                 5
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (rd)
          
-         589         104 LOAD_FAST                0 (config)
+         616         104 LOAD_FAST                0 (config)
                      106 LOAD_CONST               1 ('section')
                      108 BINARY_SUBSCR
                      118 LOAD_METHOD              3 (get_timespan)
                      140 LOAD_CONST               3 ('timespan')
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (result)
          
-         590         158 LOAD_FAST                2 (result)
+         617         158 LOAD_FAST                2 (result)
                      160 LOAD_FAST                1 (rd)
                      162 COMPARE_OP               2 (==)
                      168 STORE_FAST               3 (@py_assert1)
                      170 LOAD_FAST                3 (@py_assert1)
                      172 POP_JUMP_FORWARD_IF_TRUE   194 (to 562)
                      174 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      186 LOAD_ATTR                5 (_call_reprcompare)
@@ -12068,15 +12522,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'relativedelta', 'get_timespan', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'rd', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_timespan_int'
-         firstlineno 583
+         firstlineno 610
          lnotab 0x020126010a01160220013601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -12096,51 +12550,51 @@
             147409000000000000000000006a0800000000000000007c01a6010000ab
             01000000000000000072147409000000000000000000006a090000000000
             0000007c01a6010000ab0100000000000000006e016409640a9c027a0600
             007d04640b640c7c0469017a0600007d0574150000000000000000000074
             09000000000000000000006a0b00000000000000007c05a6010000ab0100
             00000000000000a6010000ab010000000000000000820164007d03640053
             00
-         592           0 RESUME                   0
+         619           0 RESUME                   0
          
-         593           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         620           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         594          40 BUILD_MAP                0
+         621          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         595          50 LOAD_CONST               2 ('10s')
+         622          50 LOAD_CONST               2 ('10s')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('timespan')
                       68 STORE_SUBSCR
          
-         597          72 LOAD_GLOBAL              5 (NULL + relativedelta)
+         624          72 LOAD_GLOBAL              5 (NULL + relativedelta)
                       84 LOAD_CONST               4 (10)
                       86 KW_NAMES                 5
                       88 PRECALL                  1
                       92 CALL                     1
                      102 STORE_FAST               1 (rd)
          
-         598         104 LOAD_FAST                0 (config)
+         625         104 LOAD_FAST                0 (config)
                      106 LOAD_CONST               1 ('section')
                      108 BINARY_SUBSCR
                      118 LOAD_METHOD              3 (get_timespan)
                      140 LOAD_CONST               3 ('timespan')
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               2 (result)
          
-         599         158 LOAD_FAST                2 (result)
+         626         158 LOAD_FAST                2 (result)
                      160 LOAD_FAST                1 (rd)
                      162 COMPARE_OP               2 (==)
                      168 STORE_FAST               3 (@py_assert1)
                      170 LOAD_FAST                3 (@py_assert1)
                      172 POP_JUMP_FORWARD_IF_TRUE   194 (to 562)
                      174 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      186 LOAD_ATTR                5 (_call_reprcompare)
@@ -12232,15 +12686,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'relativedelta', 'get_timespan', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'rd', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_timespan_td'
-         firstlineno 592
+         firstlineno 619
          lnotab 0x020126010a01160220013601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -12260,52 +12714,52 @@
             0073147409000000000000000000006a0800000000000000007c01a60100
             00ab01000000000000000072147409000000000000000000006a09000000
             00000000007c01a6010000ab0100000000000000006e01640a640b9c027a
             0600007d04640c640d7c0469017a0600007d057415000000000000000000
             007409000000000000000000006a0b00000000000000007c05a6010000ab
             010000000000000000a6010000ab010000000000000000820164007d0364
             005300
-         601           0 RESUME                   0
+         628           0 RESUME                   0
          
-         602           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         629           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         603          40 BUILD_MAP                0
+         630          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         604          50 LOAD_CONST               2 ('days=1, seconds=10')
+         631          50 LOAD_CONST               2 ('days=1, seconds=10')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('timespan')
                       68 STORE_SUBSCR
          
-         606          72 LOAD_GLOBAL              5 (NULL + relativedelta)
+         633          72 LOAD_GLOBAL              5 (NULL + relativedelta)
                       84 LOAD_CONST               4 (1)
                       86 LOAD_CONST               5 (10)
                       88 KW_NAMES                 6
                       90 PRECALL                  2
                       94 CALL                     2
                      104 STORE_FAST               1 (rd)
          
-         607         106 LOAD_FAST                0 (config)
+         634         106 LOAD_FAST                0 (config)
                      108 LOAD_CONST               1 ('section')
                      110 BINARY_SUBSCR
                      120 LOAD_METHOD              3 (get_timespan)
                      142 LOAD_CONST               3 ('timespan')
                      144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               2 (result)
          
-         608         160 LOAD_FAST                2 (result)
+         635         160 LOAD_FAST                2 (result)
                      162 LOAD_FAST                1 (rd)
                      164 COMPARE_OP               2 (==)
                      170 STORE_FAST               3 (@py_assert1)
                      172 LOAD_FAST                3 (@py_assert1)
                      174 POP_JUMP_FORWARD_IF_TRUE   194 (to 564)
                      176 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      188 LOAD_ATTR                5 (_call_reprcompare)
@@ -12398,15 +12852,15 @@
             'py4'
          names      ('sapphire', 'Parser', 'relativedelta', 'get_timespan', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'rd', 'result', '@py_assert1', '@py_format3', '@py_format5')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_timespan_rd'
-         firstlineno 601
+         firstlineno 628
          lnotab 0x020126010a01160222013601
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -12422,44 +12876,44 @@
             0000000000000072147407000000000000000000006a0800000000000000
             007c01a6010000ab0100000000000000006e016407740700000000000000
             0000006a0800000000000000007c02a6010000ab01000000000000000064
             089c027a0600007d046409640a7c0469017a0600007d0574130000000000
             00000000007407000000000000000000006a0a00000000000000007c05a6
             010000ab010000000000000000a6010000ab010000000000000000820164
             0078017d037d0264005300
-         610           0 RESUME                   0
+         637           0 RESUME                   0
          
-         611           2 LOAD_GLOBAL              1 (NULL + sapphire)
+         638           2 LOAD_GLOBAL              1 (NULL + sapphire)
                       14 LOAD_ATTR                1 (Parser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (config)
          
-         612          40 BUILD_MAP                0
+         639          40 BUILD_MAP                0
                       42 LOAD_FAST                0 (config)
                       44 LOAD_CONST               1 ('section')
                       46 STORE_SUBSCR
          
-         613          50 LOAD_CONST               2 ('%%Y')
+         640          50 LOAD_CONST               2 ('%%Y')
                       52 LOAD_FAST                0 (config)
                       54 LOAD_CONST               1 ('section')
                       56 BINARY_SUBSCR
                       66 LOAD_CONST               3 ('value')
                       68 STORE_SUBSCR
          
-         615          72 LOAD_FAST                0 (config)
+         642          72 LOAD_FAST                0 (config)
                       74 LOAD_CONST               1 ('section')
                       76 BINARY_SUBSCR
                       86 LOAD_METHOD              2 (get)
                      108 LOAD_CONST               3 ('value')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               1 (result)
          
-         616         126 LOAD_CONST               4 ('%Y')
+         643         126 LOAD_CONST               4 ('%Y')
                      128 STORE_FAST               2 (@py_assert2)
                      130 LOAD_FAST                1 (result)
                      132 LOAD_FAST                2 (@py_assert2)
                      134 COMPARE_OP               2 (==)
                      140 STORE_FAST               3 (@py_assert1)
                      142 LOAD_FAST                3 (@py_assert1)
                      144 POP_JUMP_FORWARD_IF_TRUE   151 (to 448)
@@ -12538,23 +12992,23 @@
             'py5'
          names      ('sapphire', 'Parser', 'get', '@pytest_ar', '_call_reprcompare', '@py_builtins', 'locals', '_should_repr_global_name', '_saferepr', 'AssertionError', '_format_explanation')
          varnames   ('config', 'result', '@py_assert2', '@py_assert1', '@py_format4', '@py_format6')
          freevars   ()
          cellvars   ()
          filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
          name       'test_escape'
-         firstlineno 610
+         firstlineno 637
          lnotab 0x020126010a0116023601
-   names      ('__doc__', 'builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'configparser', 'datetime', 'os', 'pathlib', 'pytest', 'dateutil.relativedelta', 'relativedelta', 'sapphire_config', 'sapphire', 'Component', 'Factory', 'test_get_parser', 'test_get_proxy_dict', 'test_get_missing_section', 'test_get_missing_option', 'test_get_proxy_func', 'test_int', 'test_int_hex', 'test_int_base', 'test_int_fallback_none', 'test_int_fallback_str', 'test_int_fallback_int', 'test_boolean', 'test_boolean_fallback_none', 'test_boolean_fallback_str', 'test_boolean_fallback_bool_t', 'test_boolean_fallback_bool_f', 'test_boolean_fallback_int_t', 'test_boolean_fallback_int_f', 'test_get_list_parser', 'test_get_list_proxy_func', 'test_get_list_conv_parser', 'test_get_list_conv_proxy', 'test_get_list_sep', 'test_get_list_sep_conv', 'test_get_list_fallback_none', 'test_get_list_fallback_str', 'test_get_list_no_section', 'test_get_list_fallback_type_error', 'test_get_list_fallback_empty_str', 'test_get_list_fallback_list', 'test_get_set_parser', 'test_get_set_proxy', 'test_get_set_conv_parser', 'test_get_set_sep', 'test_get_bytes', 'test_get_datetime', 'test_get_datetime_fallback_none', 'test_get_datetime_fallback_str', 'test_get_datetime_fallback_datetime', 'test_get_timedelta', 'test_get_timedelta_fallback_none', 'test_get_timedelta_fallback_str', 'test_get_timedelta_fallback_int', 'test_get_timeselta_fallback_td', 'test_get_path', 'test_get_path_fallback_none', 'test_get_path_fallback_str', 'test_get_path_fallback_path', 'test_get_rate', 'test_get_rate_all', 'test_get_rate_fallback_none', 'test_get_rate_fallback_str', 'test_get_rate_fallback_int', 'test_get_rate_fallback_rate', 'test_rate_init_default', 'test_rate_init_timedelta', 'test_rate_nexttime', 'test_rate_nexttime_sync', 'test_rate_nexttime_offset', 'test_rate_nexttime_offset_sync', 'test_rate_nexttime_offset_sync2', 'test_get_components', 'test_get_components_proxy', 'test_get_callback', 'test_get_interpolation', 'test_get_interpolation_proxy', 'test_get_interpolation_loop', 'test_component_mixin', 'test_component_mixin_default', 'test_timespan_int', 'test_timespan_td', 'test_timespan_rd', 'test_escape')
+   names      ('__doc__', 'builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'configparser', 'datetime', 'os', 'pathlib', 'pytest', 'dateutil.relativedelta', 'relativedelta', 'sapphire_config', 'sapphire', 'Component', 'Factory', 'FactorySet', 'test_get_parser', 'test_get_proxy_dict', 'test_get_missing_section', 'test_get_missing_option', 'test_get_proxy_func', 'test_int', 'test_int_hex', 'test_int_base', 'test_int_fallback_none', 'test_int_fallback_str', 'test_int_fallback_int', 'test_boolean', 'test_boolean_fallback_none', 'test_boolean_fallback_str', 'test_boolean_fallback_bool_t', 'test_boolean_fallback_bool_f', 'test_boolean_fallback_int_t', 'test_boolean_fallback_int_f', 'test_get_list_parser', 'test_get_list_proxy_func', 'test_get_list_conv_parser', 'test_get_list_conv_proxy', 'test_get_list_sep', 'test_get_list_sep_conv', 'test_get_list_fallback_none', 'test_get_list_fallback_str', 'test_get_list_no_section', 'test_get_list_fallback_type_error', 'test_get_list_fallback_empty_str', 'test_get_list_fallback_list', 'test_get_set_parser', 'test_get_set_proxy', 'test_get_set_conv_parser', 'test_get_set_sep', 'test_get_bytes', 'test_get_datetime', 'test_get_datetime_fallback_none', 'test_get_datetime_fallback_str', 'test_get_datetime_fallback_datetime', 'test_get_timedelta', 'test_get_timedelta_fallback_none', 'test_get_timedelta_fallback_str', 'test_get_timedelta_fallback_int', 'test_get_timeselta_fallback_td', 'test_get_path', 'test_get_path_fallback_none', 'test_get_path_fallback_str', 'test_get_path_fallback_path', 'test_get_rate', 'test_get_rate_all', 'test_get_rate_fallback_none', 'test_get_rate_fallback_str', 'test_get_rate_fallback_int', 'test_get_rate_fallback_rate', 'test_rate_init_default', 'test_rate_init_timedelta', 'test_rate_nexttime', 'test_rate_nexttime_sync', 'test_rate_nexttime_offset', 'test_rate_nexttime_offset_sync', 'test_rate_nexttime_offset_sync2', 'test_get_components', 'test_get_components_proxy', 'test_component_set', 'test_component_options', 'test_get_callback', 'test_get_interpolation', 'test_get_interpolation_proxy', 'test_get_interpolation_loop', 'test_component_mixin', 'test_component_mixin_default', 'test_timespan_int', 'test_timespan_td', 'test_timespan_rd', 'test_escape')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/valentic/Dropbox/Software/sapphire-config/tests/test_sapphireconfig.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010404220108010801080108020c020802260606080608060606
-      070608060806080608060706070607060806070607060706070607060706
-      080608060806080608060806080607060606070607060706080608060806
-      080608060806070607060806080607060706070608060806070607060806
-      0b060f0608060a060a060a060a060a060806080608060806080608060806
-      0a060a060a060a060c060b060906090609
+      0x00ff02010404220108010801080108020c020802260626090608060806
+      060607060806080608060806070607060706080607060706070607060706
+      070608060806080608060806080608060706060607060706070608060806
+      080608060806080607060706080608060706070607060806080607060706
+      08060b060f0608060a060a060a060a060a06080608060806080608060806
+      080608060a060a060a060a060a060c060b060906090609
```

### Comparing `sapphire_config-1.0.3/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc` & `sapphire_config-1.0.4/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.3/tests/test_sapphireconfig.py` & `sapphire_config-1.0.4/tests/test_sapphireconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 
 class Factory(sapphire.Component):
     """Example Component class"""
 
     def __init__(self, *p, **kw):
         super().__init__('component', *p, **kw)
 
+class FactorySet(sapphire.Component):
+    """Test component set"""
+
+    def __init__(self, *p, **kw):
+        super().__init__("component", *p, **kw)
+
+        self.config.set("setname", f"setname.{self.name}") 
+
+
 def test_get_parser():
     config = sapphire.Parser()
     config['section'] = {}
     config['section']['option'] = 'value'
 
     result = config.get('section', 'option')
     assert result == 'value'
@@ -513,14 +522,32 @@
     config = sapphire.Parser()
     config['section'] = {}
     config['section']['components'] = 'a b'
 
     result = config['section'].get_components('components', factory=Factory)
     assert isinstance(result, dict)
 
+def test_component_set():
+    config = sapphire.Parser()
+    config['section'] = {}
+    config['section']['components'] = 'a b'
+
+    result = config.get_components('section', 'components', factory=FactorySet)
+    assert result['a'].config.get('setname') == "setname.a" 
+
+def test_component_options():
+    config = sapphire.Parser()
+    config['section'] = {}
+    config['section']['components'] = 'a'
+
+    c = config.get_components('section', 'components', factory=FactorySet)
+    options = c['a'].config.options()
+
+    assert options == ['name', 'component', 'setname', 'components'] 
+
 def test_get_callback():
     config = sapphire.Parser()
     config['section'] = {}
     config['section']['callback.module'] = 'os'
     config['section']['callback.function'] = 'cpu_count'
     config['section']['callback.init'] = 'cpu_count'
```

