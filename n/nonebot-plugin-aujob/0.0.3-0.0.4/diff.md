# Comparing `tmp/nonebot_plugin_aujob-0.0.3.tar.gz` & `tmp/nonebot_plugin_aujob-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.0.3.tar", last modified: Fri Jul 28 10:38:45 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.0.4.tar", last modified: Fri Jul 28 11:07:04 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.0.3.tar` & `nonebot_plugin_aujob-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:38:45.535001 nonebot_plugin_aujob-0.0.3/
--rw-rw-rw-   0        0        0      511 2023-07-28 10:38:45.534002 nonebot_plugin_aujob-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 10:38:45.519001 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0    15688 2023-07-27 13:53:51.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 10:38:45.532003 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-28 10:38:45.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-28 10:38:45.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:38:45.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-28 10:38:45.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-28 10:38:45.000000 nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      702 2023-07-28 10:38:29.000000 nonebot_plugin_aujob-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 10:38:45.536004 nonebot_plugin_aujob-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.445945 nonebot_plugin_aujob-0.0.4/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:07:04.444949 nonebot_plugin_aujob-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.431947 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0    15688 2023-07-27 13:53:51.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.442944 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-28 11:06:48.000000 nonebot_plugin_aujob-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:07:04.445945 nonebot_plugin_aujob-0.0.4/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.0.3/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.0.3/pyproject.toml` & `nonebot_plugin_aujob-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "nonebot2>=2.0.0",
-    "nonebot-plugin-apscheduler>=0.2.0"
+    "nonebot-adapter-onebot>=2.0.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

