# Comparing `tmp/nonebot_plugin_aujob-0.0.4.tar.gz` & `tmp/nonebot_plugin_aujob-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.0.4.tar", last modified: Fri Jul 28 11:07:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.0.5.tar", last modified: Fri Jul 28 11:15:04 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.0.4.tar` & `nonebot_plugin_aujob-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.445945 nonebot_plugin_aujob-0.0.4/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:07:04.444949 nonebot_plugin_aujob-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.431947 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0    15688 2023-07-27 13:53:51.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:07:04.442944 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-28 11:07:04.000000 nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-28 11:06:48.000000 nonebot_plugin_aujob-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 11:07:04.445945 nonebot_plugin_aujob-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.912872 nonebot_plugin_aujob-0.0.5/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:15:04.911873 nonebot_plugin_aujob-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.897872 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0    15661 2023-07-28 11:14:36.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.909876 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-28 11:14:41.000000 nonebot_plugin_aujob-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:15:04.913874 nonebot_plugin_aujob-0.0.5/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.0.4/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from nonebot.plugin import PluginMetadata
 from nonebot import on_keyword
 from nonebot.adapters.onebot.v11 import Message
-from .config import Config
 
 __plugin_meta__ = PluginMetadata(
     name="{Among US中的TOH模组职业介绍}",
     description="{查询TOH模组里职业的玩法描述}",
     usage="{输入.t加职业名可以查看职业的玩法}",
 
     type="{application}",
```

### Comparing `nonebot_plugin_aujob-0.0.4/pyproject.toml` & `nonebot_plugin_aujob-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

