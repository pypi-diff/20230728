# Comparing `tmp/pminit-0.2.0.tar.gz` & `tmp/pminit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pminit-0.2.0.tar", max compression
+gzip compressed data, was "pminit-0.2.1.tar", max compression
```

## Comparing `pminit-0.2.0.tar` & `pminit-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       55 2023-07-20 15:39:35.976209 pminit-0.2.0/pminit/__init__.py
--rw-r--r--   0        0        0     1176 2023-07-20 15:39:35.976209 pminit-0.2.0/pminit/cli.py
--rw-r--r--   0        0        0      581 2023-07-20 15:39:35.976209 pminit-0.2.0/post-install-hook.py
--rw-r--r--   0        0        0     1006 2023-07-21 14:47:57.864107 pminit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    17097 2023-07-20 15:39:35.976209 pminit-0.2.0/pythonmonkey/package-lock.json
--rw-r--r--   0        0        0      653 2023-07-20 15:39:35.976209 pminit-0.2.0/pythonmonkey/package.json
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-28 19:28:06.865647 pminit-0.2.1/pminit/__init__.py
+-rw-r--r--   0        0        0     1216 2023-07-28 19:28:06.865647 pminit-0.2.1/pminit/cli.py
+-rw-r--r--   0        0        0     1231 2023-07-28 19:28:06.865647 pminit-0.2.1/post-install-hook.py
+-rw-r--r--   0        0        0     1006 2023-07-28 19:32:47.469717 pminit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    17531 2023-07-28 19:28:06.881443 pminit-0.2.1/pythonmonkey/package-lock.json
+-rw-r--r--   0        0        0      679 2023-07-28 19:28:06.881443 pminit-0.2.1/pythonmonkey/package.json
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.2.1/PKG-INFO
```

### Comparing `pminit-0.2.0/pyproject.toml` & `pminit-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pminit"
-version = "0.2.0"
+version = "0.2.1"
 description = "Post-install hook for PythonMonkey"
 authors = [
   "Tom Tang <xmader@distributive.network>",
   "Caleb Aikens <caleb@distributive.network>",
   "Wes Garland <wes@distributive.network>",
   "Hamada Gasmallah <hamada@distributive.network>"
 ]
```

### Comparing `pminit-0.2.0/pythonmonkey/package.json` & `pminit-0.2.1/pythonmonkey/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'dependencies'": "{'ctx-module': '^1.0.14'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Distributive Corp.",
     "bugs": {
         "url": "https://github.com/Distributive-Network/PythonMonkey/issues"
     },
     "dependencies": {
-        "ctx-module": "^1.0.13"
+        "ctx-module": "^1.0.14"
     },
     "description": "PythonMonkey - JS Components",
     "directories": {
         "doc": "docs",
         "test": "tests"
     },
     "homepage": "https://github.com/Distributive-Network/PythonMonkey#readme",
```

