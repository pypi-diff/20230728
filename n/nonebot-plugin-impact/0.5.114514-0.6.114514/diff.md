# Comparing `tmp/nonebot_plugin_impact-0.5.114514.tar.gz` & `tmp/nonebot_plugin_impact-0.6.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.5.114514.tar", last modified: Wed Jul 26 18:54:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.6.114514.tar", last modified: Fri Jul 28 16:38:32 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.5.114514.tar` & `nonebot_plugin_impact-0.6.114514.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.166345 nonebot_plugin_impact-0.5.114514/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.5.114514/LICENSE
--rw-rw-rw-   0        0        0      306 2023-07-26 18:54:58.165344 nonebot_plugin_impact-0.5.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.093484 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     2093 2023-07-26 18:53:36.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0     9180 2023-07-26 18:53:23.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/draw_img.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.100484 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/
--rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
--rw-rw-rw-   0        0        0    20206 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2205 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8628 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.098985 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      306 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 18:54:58.166844 nonebot_plugin_impact-0.5.114514/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-07-26 18:54:19.000000 nonebot_plugin_impact-0.5.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.777642 nonebot_plugin_impact-0.6.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.6.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-07-28 16:38:32.776641 nonebot_plugin_impact-0.6.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.759642 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2093 2023-07-28 16:37:24.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0     9180 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/draw_img.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.766642 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/
+-rw-rw-rw-   0        0        0  6700204 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
+-rw-rw-rw-   0        0        0    20206 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2205 2023-07-28 16:31:58.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8687 2023-07-28 16:35:21.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:38:32.765641 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-28 16:38:32.000000 nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 16:38:32.777642 nonebot_plugin_impact-0.6.114514/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-07-28 16:38:14.000000 nonebot_plugin_impact-0.6.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.5.114514/LICENSE` & `nonebot_plugin_impact-0.6.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,11 +85,11 @@
         description="让群友们眼前一黑的nonebot2淫趴插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_impact",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
-            "version": "0.05.114514",
+            "version": "0.06.114514",
             "priority": 20,
         },
     )
```

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/draw_img.py` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/draw_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.6.114514/nonebot_plugin_impact/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,18 @@
                 self.ejaculation_data = {}
                 self.write_ejaculation_data()  # 这种结构, 不想重构也不想新建json了，所以放宽了这么多{"user_id": {"date": {"ejaculation": 123}}}
         self.usage = """指令1: 嗦牛子 (给目标牛牛增加长度, 自己或者他人, 通过艾特选择对象, 没有at时目标是自己)
 指令2: 打胶 | 开导 (给自己牛牛增加长度)
 指令3: pk | 对决 (普通的pk,单纯的random实现输赢, 胜利方获取败方随机数/2的牛牛长度)
 指令4: 查询 (目标牛牛长度, 自己或者他人, 通过艾特选择对象, 没有at时目标是自己)
 指令5: jj排行榜 | jj排名 | jj榜单 | jjrank (字面意思, 输出倒数五位和前五位, 以及自己的排名)
-指令6: 开启淫趴|禁止淫趴 (由管理员 | 群主 | SUPERUSERS开启或者关闭淫趴)
-指令7: 日群友|透群友|日群主|透群主|日管理|透管理  (字面意思, 当使用透群友的时候如果at了人那么直接指定)
-指令8: 注入查询 | 摄入查询 (查询目标被透注入的量，后接(历史|全部), 可查看总被摄入的量, 无艾特的时候是自己, 有at的时候是目标)
-指令9: 淫趴介绍 | 淫趴说明| 淫趴帮助 (输出淫趴插件的命令列表)"""
+指令6: 开始银趴 | 关闭银趴 | 开启淫趴 | 禁止淫趴 | 开启银趴 | 禁止银趴 (由管理员 | 群主 | SUPERUSERS开启或者关闭淫趴)
+指令7: 日群友 | 透群友 | 日群主 | 透群主 | 日管理 | 透管理  (字面意思, 当使用透群友的时候如果at了人那么直接指定)
+指令8: 注入查询 | 摄入查询 | 射入查询 (查询目标被透注入的量，后接(历史|全部), 可查看总被摄入的量, 无艾特的时候是自己, 有at的时候是目标)
+指令9: 淫趴介绍  (输出淫趴插件的命令列表)"""
         self.not_allow = '群内还未开启淫趴游戏, 请管理员或群主发送"开启淫趴", "禁止淫趴"以开启/关闭该功能'  # 未开启该功能的send信息
         self.jj_variable = ["牛子", "牛牛", "丁丁", "JJ"]  # JJ变量
         self.cd_data = {}  # 冷却数据
         self.pk_cd_data = {}  # pk冷却数据
         self.suo_cd_data = {}  # 嗦牛子冷却数据
         self.ejaculation_cd = {}  # 射精CD
         config = nonebot.get_driver().config  # 获取配置
```

### Comparing `nonebot_plugin_impact-0.5.114514/setup.py` & `nonebot_plugin_impact-0.6.114514/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_impact",
-    version="0.05.114514",
+    version="0.06.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="让群友们眼前一黑的nonebot2淫趴插件",
     python_requires=">=3.8.0",
     packages=find_packages(),
     url="https://github.com/Special-Week/nonebot_plugin_impact",
     package_data={"nonebot_plugin_impact": ["fonts/*"]},
```

