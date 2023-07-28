# Comparing `tmp/vktoken-2.1.1.tar.gz` & `tmp/vktoken-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vktoken-2.1.1.tar", max compression
+gzip compressed data, was "vktoken-3.0.0.tar", last modified: Fri Jul 28 16:32:57 2023, max compression
```

## Comparing `vktoken-2.1.1.tar` & `vktoken-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,7 @@
--rw-r--r--   0        0        0     1063 2021-11-06 10:38:06.380079 vktoken-2.1.1/LICENSE
--rw-r--r--   0        0        0      599 2021-11-07 19:40:59.793317 vktoken-2.1.1/README.md
--rw-r--r--   0        0        0      761 2021-11-07 19:51:19.853313 vktoken-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      381 2021-11-07 19:48:59.189981 vktoken-2.1.1/vktoken/__init__.py
--rw-r--r--   0        0        0     2105 2021-11-07 19:53:02.643313 vktoken-2.1.1/vktoken/__main__.py
--rw-r--r--   0        0        0      149 2021-11-07 19:47:45.603314 vktoken-2.1.1/vktoken/app.py
--rw-r--r--   0        0        0        0 2021-11-06 21:20:09.616330 vktoken-2.1.1/vktoken/cli/__init__.py
--rw-r--r--   0        0        0     1134 2021-11-07 19:51:22.839980 vktoken-2.1.1/vktoken/cli/args.py
--rw-r--r--   0        0        0      215 2021-11-06 10:38:06.383412 vktoken-2.1.1/vktoken/cli/log.py
--rw-r--r--   0        0        0     1389 2021-11-07 19:58:00.120313 vktoken-2.1.1/setup.py
--rw-r--r--   0        0        0     1320 2021-11-07 19:58:00.120579 vktoken-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-28 15:46:42.727754 vktoken-3.0.0/LICENSE
+-rw-r--r--   0        0        0      600 2023-07-28 16:28:22.787795 vktoken-3.0.0/README.md
+-rw-r--r--   0        0        0      909 2023-07-28 16:32:57.017165 vktoken-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-28 16:28:49.972537 vktoken-3.0.0/vktoken/__init__.py
+-rw-r--r--   0        0        0     4053 2023-07-28 16:27:52.666187 vktoken-3.0.0/vktoken/__main__.py
+-rw-r--r--   0        0        0      239 2023-07-28 16:05:53.236320 vktoken-3.0.0/vktoken/app.py
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 vktoken-3.0.0/PKG-INFO
```

### Comparing `vktoken-2.1.1/LICENSE` & `vktoken-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vktoken-2.1.1/README.md` & `vktoken-3.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # vktoken
-Tool for getting VK access token.
+Tool for granting VK access token.
 [![preview](https://asciinema.org/a/nnP04X2a4jlKzCBIKHaN0HDVY.svg)](https://asciinema.org/a/nnP04X2a4jlKzCBIKHaN0HDVY)
 
 ## Installation
 `pip install --user vktoken`
 
 ## Usage
 `vktoken [--help] [--version] [--app] [--client-id] [--client-secret] login [password]`
```

### Comparing `vktoken-2.1.1/PKG-INFO` & `vktoken-3.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 Metadata-Version: 2.1
 Name: vktoken
-Version: 2.1.1
-Summary: Tool for getting VK access token
-Home-page: https://github.com/jieggii/vktoken
+Version: 3.0.0
+Summary: Tool for granting VK access token
+Keywords: vk vkontakte
+Author-Email: jieggii <jieggii@protonmail.com>
 License: MIT
-Keywords: vk,vkontakte
-Author: jieggii
-Author-email: jieggii.contact@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: requests (>=2.26.0,<3.0.0)
-Project-URL: Bug Tracker, https://github.com/jieggii/vktoken/issues
-Project-URL: Repository, https://github.com/jieggii/vktoken
+Requires-Python: >=3.8
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # vktoken
-Tool for getting VK access token.
+Tool for granting VK access token.
 [![preview](https://asciinema.org/a/nnP04X2a4jlKzCBIKHaN0HDVY.svg)](https://asciinema.org/a/nnP04X2a4jlKzCBIKHaN0HDVY)
 
 ## Installation
 `pip install --user vktoken`
 
 ## Usage
 `vktoken [--help] [--version] [--app] [--client-id] [--client-secret] login [password]`
@@ -31,8 +22,7 @@
 ## Examples
 * `vktoken +79652331167`  
 * `vktoken --app iphone +79523311167 mypassword`
 * `vktoken --client-id 3140623 --client-secret VeWdmVclDCtn6ihuP1nt +79523311167`
 
 ## Features
 * You can choose builtin VK app credentials from the list: `android`, `iphone`, `ipad` and `windows-phone`.
-
```

