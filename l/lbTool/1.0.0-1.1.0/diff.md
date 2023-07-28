# Comparing `tmp/lbTool-1.0.0.tar.gz` & `tmp/lbTool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbTool-1.0.0.tar", last modified: Tue Jul 25 08:44:59 2023, max compression
+gzip compressed data, was "lbTool-1.1.0.tar", last modified: Fri Jul 28 01:52:26 2023, max compression
```

## Comparing `lbTool-1.0.0.tar` & `lbTool-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:44:59.703057 lbTool-1.0.0/
--rw-rw-rw-   0        0        0      111 2023-07-25 08:44:59.702060 lbTool-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 08:44:59.693084 lbTool-1.0.0/lbTool/
--rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbTool-1.0.0/lbTool/EnCipher.py
--rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbTool-1.0.0/lbTool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:44:59.701063 lbTool-1.0.0/lbTool.egg-info/
--rw-rw-rw-   0        0        0      111 2023-07-25 08:44:59.000000 lbTool-1.0.0/lbTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-25 08:44:59.000000 lbTool-1.0.0/lbTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:44:59.000000 lbTool-1.0.0/lbTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-25 08:44:59.000000 lbTool-1.0.0/lbTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 08:44:59.000000 lbTool-1.0.0/lbTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 08:44:59.703057 lbTool-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-07-25 08:43:49.000000 lbTool-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:52:26.921280 lbTool-1.1.0/
+-rw-rw-rw-   0        0        0      111 2023-07-28 01:52:26.920283 lbTool-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 01:52:26.911307 lbTool-1.1.0/lbTool/
+-rw-rw-rw-   0        0        0     1234 2023-07-27 08:26:52.000000 lbTool-1.1.0/lbTool/Common.py
+-rw-rw-rw-   0        0        0     2981 2023-07-27 01:05:47.000000 lbTool-1.1.0/lbTool/Db.py
+-rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbTool-1.1.0/lbTool/EnCipher.py
+-rw-rw-rw-   0        0        0     2143 2023-07-26 10:00:46.000000 lbTool-1.1.0/lbTool/FileUtil.py
+-rw-rw-rw-   0        0        0      804 2023-07-27 08:09:45.000000 lbTool-1.1.0/lbTool/Logging.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbTool-1.1.0/lbTool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 01:52:26.919286 lbTool-1.1.0/lbTool.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-07-28 01:52:26.000000 lbTool-1.1.0/lbTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-28 01:52:26.000000 lbTool-1.1.0/lbTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 01:52:26.000000 lbTool-1.1.0/lbTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-28 01:52:26.000000 lbTool-1.1.0/lbTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 01:52:26.000000 lbTool-1.1.0/lbTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 01:52:26.921280 lbTool-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-27 01:05:47.000000 lbTool-1.1.0/setup.py
```

### Comparing `lbTool-1.0.0/lbTool/EnCipher.py` & `lbTool-1.1.0/lbTool/EnCipher.py`

 * *Files identical despite different names*

