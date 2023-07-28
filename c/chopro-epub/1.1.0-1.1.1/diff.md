# Comparing `tmp/chopro_epub-1.1.0.tar.gz` & `tmp/chopro_epub-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chopro_epub-1.1.0.tar", last modified: Fri Jul 28 06:28:55 2023, max compression
+gzip compressed data, was "chopro_epub-1.1.1.tar", last modified: Fri Jul 28 06:43:35 2023, max compression
```

## Comparing `chopro_epub-1.1.0.tar` & `chopro_epub-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:28:55.332696 chopro_epub-1.1.0/
--rw-r--r--   0 pferrand   (502) staff       (20)     1065 2023-07-28 06:27:08.000000 chopro_epub-1.1.0/LICENSE.md
--rw-r--r--   0 pferrand   (502) staff       (20)      501 2023-07-28 06:28:55.332964 chopro_epub-1.1.0/PKG-INFO
--rw-r--r--   0 pferrand   (502) staff       (20)     2274 2023-07-26 12:12:55.000000 chopro_epub-1.1.0/README.md
-drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:28:55.307813 chopro_epub-1.1.0/chopro_epub/
--rw-r--r--   0 pferrand   (502) staff       (20)       22 2023-07-28 06:10:00.000000 chopro_epub-1.1.0/chopro_epub/__init__.py
--rw-r--r--   0 pferrand   (502) staff       (20)      654 2023-07-27 13:24:38.000000 chopro_epub-1.1.0/chopro_epub/chopro-epub.css
-drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:28:55.332109 chopro_epub-1.1.0/chopro_epub/cli/
--rw-r--r--   0 pferrand   (502) staff       (20)        0 2023-07-28 06:10:00.000000 chopro_epub-1.1.0/chopro_epub/cli/__init__.py
--rw-r--r--   0 pferrand   (502) staff       (20)     4987 2023-07-28 06:10:00.000000 chopro_epub-1.1.0/chopro_epub/cli/epub.py
--rw-r--r--   0 pferrand   (502) staff       (20)     3004 2023-07-28 06:10:00.000000 chopro_epub-1.1.0/chopro_epub/cli/html.py
--rw-r--r--   0 pferrand   (502) staff       (20)     7382 2023-07-28 06:10:00.000000 chopro_epub-1.1.0/chopro_epub/parser.py
-drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:28:55.330609 chopro_epub-1.1.0/chopro_epub.egg-info/
--rw-r--r--   0 pferrand   (502) staff       (20)      501 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/PKG-INFO
--rw-r--r--   0 pferrand   (502) staff       (20)      407 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/SOURCES.txt
--rw-r--r--   0 pferrand   (502) staff       (20)        1 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/dependency_links.txt
--rw-r--r--   0 pferrand   (502) staff       (20)       98 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/entry_points.txt
--rw-r--r--   0 pferrand   (502) staff       (20)      105 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/requires.txt
--rw-r--r--   0 pferrand   (502) staff       (20)       12 2023-07-28 06:28:55.000000 chopro_epub-1.1.0/chopro_epub.egg-info/top_level.txt
--rw-r--r--   0 pferrand   (502) staff       (20)      187 2023-07-26 12:12:55.000000 chopro_epub-1.1.0/pyproject.toml
--rw-r--r--   0 pferrand   (502) staff       (20)      842 2023-07-28 06:28:55.333979 chopro_epub-1.1.0/setup.cfg
+drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:43:35.606401 chopro_epub-1.1.1/
+-rw-r--r--   0 pferrand   (502) staff       (20)     1065 2023-07-28 06:27:08.000000 chopro_epub-1.1.1/LICENSE.md
+-rw-r--r--   0 pferrand   (502) staff       (20)     2753 2023-07-28 06:43:35.606614 chopro_epub-1.1.1/PKG-INFO
+-rw-r--r--   0 pferrand   (502) staff       (20)     2274 2023-07-26 12:12:55.000000 chopro_epub-1.1.1/README.md
+drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:43:35.581491 chopro_epub-1.1.1/chopro_epub/
+-rw-r--r--   0 pferrand   (502) staff       (20)       22 2023-07-28 06:40:25.000000 chopro_epub-1.1.1/chopro_epub/__init__.py
+-rw-r--r--   0 pferrand   (502) staff       (20)      654 2023-07-27 13:24:38.000000 chopro_epub-1.1.1/chopro_epub/chopro-epub.css
+drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:43:35.605729 chopro_epub-1.1.1/chopro_epub/cli/
+-rw-r--r--   0 pferrand   (502) staff       (20)        0 2023-07-28 06:10:00.000000 chopro_epub-1.1.1/chopro_epub/cli/__init__.py
+-rw-r--r--   0 pferrand   (502) staff       (20)     4987 2023-07-28 06:10:00.000000 chopro_epub-1.1.1/chopro_epub/cli/epub.py
+-rw-r--r--   0 pferrand   (502) staff       (20)     3004 2023-07-28 06:10:00.000000 chopro_epub-1.1.1/chopro_epub/cli/html.py
+-rw-r--r--   0 pferrand   (502) staff       (20)     7382 2023-07-28 06:10:00.000000 chopro_epub-1.1.1/chopro_epub/parser.py
+drwxr-xr-x   0 pferrand   (502) staff       (20)        0 2023-07-28 06:43:35.604272 chopro_epub-1.1.1/chopro_epub.egg-info/
+-rw-r--r--   0 pferrand   (502) staff       (20)     2753 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/PKG-INFO
+-rw-r--r--   0 pferrand   (502) staff       (20)      407 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/SOURCES.txt
+-rw-r--r--   0 pferrand   (502) staff       (20)        1 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/dependency_links.txt
+-rw-r--r--   0 pferrand   (502) staff       (20)       98 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/entry_points.txt
+-rw-r--r--   0 pferrand   (502) staff       (20)      105 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/requires.txt
+-rw-r--r--   0 pferrand   (502) staff       (20)       12 2023-07-28 06:43:35.000000 chopro_epub-1.1.1/chopro_epub.egg-info/top_level.txt
+-rw-r--r--   0 pferrand   (502) staff       (20)      187 2023-07-26 12:12:55.000000 chopro_epub-1.1.1/pyproject.toml
+-rw-r--r--   0 pferrand   (502) staff       (20)      923 2023-07-28 06:43:35.607577 chopro_epub-1.1.1/setup.cfg
```

### Comparing `chopro_epub-1.1.0/LICENSE.md` & `chopro_epub-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chopro_epub-1.1.0/README.md` & `chopro_epub-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chopro_epub-1.1.0/chopro_epub/chopro-epub.css` & `chopro_epub-1.1.1/chopro_epub/chopro-epub.css`

 * *Files identical despite different names*

### Comparing `chopro_epub-1.1.0/chopro_epub/cli/epub.py` & `chopro_epub-1.1.1/chopro_epub/cli/epub.py`

 * *Files identical despite different names*

### Comparing `chopro_epub-1.1.0/chopro_epub/cli/html.py` & `chopro_epub-1.1.1/chopro_epub/cli/html.py`

 * *Files identical despite different names*

### Comparing `chopro_epub-1.1.0/chopro_epub/parser.py` & `chopro_epub-1.1.1/chopro_epub/parser.py`

 * *Files identical despite different names*

