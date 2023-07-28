# Comparing `tmp/nonebot_plugin_aujob-0.0.5.tar.gz` & `tmp/nonebot_plugin_aujob-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.0.5.tar", last modified: Fri Jul 28 11:15:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.0.6.tar", last modified: Fri Jul 28 11:25:51 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.0.5.tar` & `nonebot_plugin_aujob-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.912872 nonebot_plugin_aujob-0.0.5/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:15:04.911873 nonebot_plugin_aujob-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.897872 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0    15661 2023-07-28 11:14:36.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:15:04.909876 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-28 11:15:04.000000 nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-28 11:14:41.000000 nonebot_plugin_aujob-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 11:15:04.913874 nonebot_plugin_aujob-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.519140 nonebot_plugin_aujob-0.0.6/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:25:51.517141 nonebot_plugin_aujob-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.503138 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0    15651 2023-07-28 11:25:23.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.515138 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-28 11:25:35.000000 nonebot_plugin_aujob-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:25:51.519140 nonebot_plugin_aujob-0.0.6/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.0.5/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from nonebot.plugin import PluginMetadata
 from nonebot import on_keyword
 from nonebot.adapters.onebot.v11 import Message
 
 __plugin_meta__ = PluginMetadata(
-    name="{Among US中的TOH模组职业介绍}",
-    description="{查询TOH模组里职业的玩法描述}",
-    usage="{输入.t加职业名可以查看职业的玩法}",
+    name="Among US中的TOH模组职业介绍",
+    description="查询TOH模组里职业的玩法描述",
+    usage="输入.t加职业名可以查看职业的玩法",
 
-    type="{application}",
+    type="application",
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
-    homepage="{https://github.com/qwqZYLqwq/nonebot-plugin-aujob}",
+    homepage="https://github.com/qwqZYLqwq/nonebot-plugin-aujob",
     # 发布必填。
 
 
     supported_adapters={"~onebot.v11", "~telegram"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
```

### Comparing `nonebot_plugin_aujob-0.0.5/pyproject.toml` & `nonebot_plugin_aujob-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

