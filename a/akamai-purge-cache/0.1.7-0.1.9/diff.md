# Comparing `tmp/akamai_purge_cache-0.1.7.tar.gz` & `tmp/akamai_purge_cache-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-0.1.7.tar", max compression
+gzip compressed data, was "akamai_purge_cache-0.1.9.tar", max compression
```

## Comparing `akamai_purge_cache-0.1.7.tar` & `akamai_purge_cache-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0        0 2023-07-19 02:42:42.000000 akamai_purge_cache-0.1.7/README.md
--rwxr-xr-x   0        0        0        0 2023-07-22 07:11:33.000000 akamai_purge_cache-0.1.7/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      852 2023-07-22 08:16:41.000000 akamai_purge_cache-0.1.7/akamai_purge_cache/purge.py
--rwxr-xr-x   0        0        0      669 2023-07-25 00:36:49.307210 akamai_purge_cache-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-07-26 00:30:10.895312 akamai_purge_cache-0.1.9/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-25 14:00:09.217851 akamai_purge_cache-0.1.9/akamai_purge_cache/__init__.py
+-rwxr-xr-x   0        0        0      852 2023-07-25 19:52:16.805321 akamai_purge_cache-0.1.9/akamai_purge_cache/purge.py
+-rwxr-xr-x   0        0        0      669 2023-07-28 21:30:33.709997 akamai_purge_cache-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.9/PKG-INFO
```

### Comparing `akamai_purge_cache-0.1.7/akamai_purge_cache/purge.py` & `akamai_purge_cache-0.1.9/akamai_purge_cache/purge.py`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-0.1.7/pyproject.toml` & `akamai_purge_cache-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] 
 name = "akamai_purge_cache"
-version = "0.1.7" 
+version = "0.1.9" 
 description = "Marriott CDN Team Fastpurge POC script" 
 authors = ["Alan Janis <alan.janis@marriott.com>", "Raahi Chada <raahi.chada@marriott.com"]
 readme = "README.md"
 packages = [{include = "akamai_purge_cache"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

