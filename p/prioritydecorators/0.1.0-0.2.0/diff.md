# Comparing `tmp/prioritydecorators-0.1.0.tar.gz` & `tmp/prioritydecorators-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prioritydecorators-0.1.0.tar", last modified: Fri Jul 28 14:26:20 2023, max compression
+gzip compressed data, was "prioritydecorators-0.2.0.tar", last modified: Fri Jul 28 14:38:51 2023, max compression
```

## Comparing `prioritydecorators-0.1.0.tar` & `prioritydecorators-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 14:26:20.122333 prioritydecorators-0.1.0/
--rw-rw-rw-   0        0        0     1077 2023-07-28 14:25:29.000000 prioritydecorators-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      267 2023-07-28 14:26:20.122333 prioritydecorators-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3955 2023-07-28 14:01:42.000000 prioritydecorators-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 14:26:20.101187 prioritydecorators-0.1.0/prioritydecorators/
--rw-rw-rw-   0        0        0        0 2023-07-28 12:58:38.000000 prioritydecorators-0.1.0/prioritydecorators/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-07-28 13:26:38.000000 prioritydecorators-0.1.0/prioritydecorators/prioritydecorators.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:26:20.121335 prioritydecorators-0.1.0/prioritydecorators.egg-info/
--rw-rw-rw-   0        0        0      267 2023-07-28 14:26:19.000000 prioritydecorators-0.1.0/prioritydecorators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-07-28 14:26:19.000000 prioritydecorators-0.1.0/prioritydecorators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 14:26:19.000000 prioritydecorators-0.1.0/prioritydecorators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-28 14:26:19.000000 prioritydecorators-0.1.0/prioritydecorators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-28 14:26:19.000000 prioritydecorators-0.1.0/prioritydecorators.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-28 14:26:20.124333 prioritydecorators-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-07-28 13:36:23.000000 prioritydecorators-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:38:51.456645 prioritydecorators-0.2.0/
+-rw-rw-rw-   0        0        0     1077 2023-07-28 14:25:29.000000 prioritydecorators-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4256 2023-07-28 14:38:51.456645 prioritydecorators-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3955 2023-07-28 14:28:36.000000 prioritydecorators-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 14:38:51.448646 prioritydecorators-0.2.0/prioritydecorators/
+-rw-rw-rw-   0        0        0        0 2023-07-28 12:58:38.000000 prioritydecorators-0.2.0/prioritydecorators/__init__.py
+-rw-rw-rw-   0        0        0     6568 2023-07-28 13:26:38.000000 prioritydecorators-0.2.0/prioritydecorators/prioritydecorators.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:38:51.455646 prioritydecorators-0.2.0/prioritydecorators.egg-info/
+-rw-rw-rw-   0        0        0     4256 2023-07-28 14:38:51.000000 prioritydecorators-0.2.0/prioritydecorators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-28 14:38:51.000000 prioritydecorators-0.2.0/prioritydecorators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:38:51.000000 prioritydecorators-0.2.0/prioritydecorators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-28 14:38:51.000000 prioritydecorators-0.2.0/prioritydecorators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-28 14:38:51.000000 prioritydecorators-0.2.0/prioritydecorators.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-28 14:38:51.458645 prioritydecorators-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-07-28 14:37:17.000000 prioritydecorators-0.2.0/setup.py
```

### Comparing `prioritydecorators-0.1.0/LICENSE.txt` & `prioritydecorators-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prioritydecorators-0.1.0/README.md` & `prioritydecorators-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prioritydecorators-0.1.0/prioritydecorators/prioritydecorators.py` & `prioritydecorators-0.2.0/prioritydecorators/prioritydecorators.py`

 * *Files identical despite different names*

