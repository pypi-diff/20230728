# Comparing `tmp/ifunnygifmaker-0.2.2.tar.gz` & `tmp/ifunnygifmaker-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.2.2.tar", last modified: Sat Apr 22 19:16:45 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.2.3.tar", last modified: Fri Jul 28 04:38:14 2023, max compression
```

## Comparing `ifunnygifmaker-0.2.2.tar` & `ifunnygifmaker-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.2.2/README.md
--rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.2.2/ifunnygifmaker/.DS_Store
--rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.2.2/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.2.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
--rw-r--r--   0        0        0     4935 2023-04-22 19:16:27.890457 ifunnygifmaker-0.2.2/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      459 2023-04-22 19:16:38.456853 ifunnygifmaker-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-07-11 21:32:07.857910 ifunnygifmaker-0.2.3/README.md
+-rw-r--r--   0        0        0       39 2023-07-11 21:32:07.857910 ifunnygifmaker-0.2.3/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0    25492 2023-07-11 21:32:07.857910 ifunnygifmaker-0.2.3/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0     5198 2023-07-28 04:37:08.491632 ifunnygifmaker-0.2.3/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      578 2023-07-28 03:31:44.122022 ifunnygifmaker-0.2.3/ifunnygifmaker/utils/image_utils.py
+-rw-r--r--   0        0        0      447 2023-07-28 04:37:58.451627 ifunnygifmaker-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 ifunnygifmaker-0.2.3/PKG-INFO
```

### Comparing `ifunnygifmaker-0.2.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf` & `ifunnygifmaker-0.2.3/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf`

 * *Files identical despite different names*

