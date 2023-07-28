# Comparing `tmp/hyd-0.1.4.tar.gz` & `tmp/hyd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyd-0.1.4.tar", max compression
+gzip compressed data, was "hyd-0.1.5.tar", max compression
```

## Comparing `hyd-0.1.4.tar` & `hyd-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.4/LICENSE
--rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.4/README.md
--rw-r--r--   0        0        0     3866 2023-05-11 08:37:42.319477 hyd-0.1.4/hyd/HaukursYouTubeDownloader.py
--rw-r--r--   0        0        0      385 2023-05-11 08:38:00.313976 hyd-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 hyd-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.5/LICENSE
+-rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.5/README.md
+-rw-r--r--   0        0        0     4467 2023-07-28 18:26:56.948007 hyd-0.1.5/hyd/HaukursYouTubeDownloader.py
+-rw-r--r--   0        0        0      457 2023-07-28 18:40:09.865965 hyd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 hyd-0.1.5/PKG-INFO
```

### Comparing `hyd-0.1.4/LICENSE` & `hyd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyd-0.1.4/PKG-INFO` & `hyd-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hyd
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: A basic python youtube downloader made using tkinter, moviepy and pytube.
 License: MIT
 Author: haukurlogi
 Author-email: haukurlogi2008@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
-Requires-Dist: pytube (>=12.1.0,<13.0.0)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Description-Content-Type: text/markdown
 
 ### Install
 
 ```
 pip install hyd
 ```
```

