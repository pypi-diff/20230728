# Comparing `tmp/nonebot_plugin_majsoul-0.2.1.post1.tar.gz` & `tmp/nonebot_plugin_majsoul-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_majsoul-0.2.1.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_majsoul-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_majsoul-0.2.1.post1.tar` & `nonebot_plugin_majsoul-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.1.post1/LICENSE
--rw-r--r--   0        0        0      739 2023-06-17 15:15:01.368383 nonebot_plugin_majsoul-0.2.1.post1/pyproject.toml
--rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.1.post1/README.md
--rw-r--r--   0        0        0     1144 2023-05-29 13:21:52.045266 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/__init__.py
--rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/config.py
--rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/errors.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/__init__.py
--rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/handle_error.py
--rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/__init__.py
--rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/auto_retry.py
--rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/host_prober.py
--rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
--rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/api.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
--rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
--rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
--rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
--rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
--rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
--rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
--rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
--rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
--rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
--rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
--rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
--rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
--rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
--rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
--rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
--rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
--rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
--rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
--rw-r--r--   0        0        0     9721 2023-06-02 03:57:51.665919 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
--rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
--rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/__init__.py
--rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/downloader.py
--rw-r--r--   0        0        0     2729 2023-06-01 06:50:23.321782 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/query_paipu.py
--rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/__init__.py
--rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/decode_integer.py
--rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/my_executor.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/nonebot.py
--rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/percentile.py
--rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/rank.py
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.1.post1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.2/LICENSE
+-rw-r--r--   0        0        0      738 2023-07-28 14:59:31.096885 nonebot_plugin_majsoul-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-05-25 09:15:00.279006 nonebot_plugin_majsoul-0.2.2/README.md
+-rw-r--r--   0        0        0     1386 2023-07-28 14:58:53.767191 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/config.py
+-rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/errors.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/interceptors/__init__.py
+-rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/interceptors/handle_error.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/network/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-28 14:52:53.894450 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/network/auto_retry.py
+-rw-r--r--   0        0        0     2925 2023-07-28 14:58:53.757189 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/network/host_prober.py
+-rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
+-rw-r--r--   0        0        0     5179 2023-07-28 14:58:53.735120 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/api.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
+-rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
+-rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
+-rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
+-rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
+-rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
+-rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
+-rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
+-rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
+-rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
+-rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
+-rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
+-rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
+-rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
+-rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
+-rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
+-rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
+-rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
+-rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
+-rw-r--r--   0        0        0     9721 2023-06-02 03:57:51.665919 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
+-rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
+-rw-r--r--   0        0        0      103 2023-07-28 15:00:51.702408 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paipu/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-28 15:05:16.213071 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paipu/downloader.py
+-rw-r--r--   0        0        0     2702 2023-07-28 14:54:14.816176 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paipu/query_paipu.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/decode_integer.py
+-rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/my_executor.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/nonebot.py
+-rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/percentile.py
+-rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/rank.py
+-rw-r--r--   0        0        0     4433 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/LICENSE` & `nonebot_plugin_majsoul-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/README.md` & `nonebot_plugin_majsoul-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/__init__.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,33 +5,38 @@
 @License        : AGPLv3
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-majsoul
 """
 from nonebot import require
 
 require("nonebot_plugin_saa")
 
+from .config import Config
 from .utils.nonebot import default_cmd_start
 
-help_text = f"""
+__usage__ = f"""
 牌谱屋：
 - {default_cmd_start}雀魂(三麻)信息 <雀魂账号> [<房间类型>] [最近<数量>场] [最近<数量>{{天|周|个月|年}}]
 - {default_cmd_start}雀魂(三麻)对局 <雀魂账号> [<房间类型>]
 - {default_cmd_start}雀魂(三麻)PT图 <雀魂账号> [最近<数量>场] [最近<数量>{{天|周|个月|年}}]
 
 牌谱下载：
 - {default_cmd_start}下载雀魂牌谱 <牌谱链接或UUID>
 
 以上命令格式中，以<>包裹的表示一个参数，以[]包裹的表示一个可选项。
 
-详细说明：参见https://github.com/ssttkkl/nonebot-plugin-majsoul
+详细说明：参见https://github.com/bot-ssttkkl/nonebot-plugin-majsoul
 """.strip()
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name='雀魂查询',
     description='根据牌谱屋的数据查询雀魂账号信息',
-    usage=help_text
+    usage=__usage__,
+    type="application",
+    config=Config,
+    homepage="https://github.com/bot-ssttkkl/nonebot-plugin-majsoul",
+    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~telegram", "~kaiheila"}
 )
 
 from . import paifuya
 from . import paipu
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/interceptors/handle_error.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/auto_retry.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/network/auto_retry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from functools import wraps
-from typing import TypeVar, Callable
+from typing import TypeVar, Callable, Optional, Awaitable, Any, Union, Type, Sequence
 
-from httpx import HTTPError
 from nonebot import logger
 from typing_extensions import ParamSpec
 
 T = TypeVar('T')
 P = ParamSpec('P')
 
 
-def auto_retry(func: Callable[P, T]) -> Callable[P, T]:
-    @wraps(func)
-    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-        err = None
-
-        for i in range(10):
-            try:
-                return await func(*args, **kwargs)
-            except HTTPError as e:
-                logger.error(f"Retrying... {i + 1}/10")
-                logger.exception(e)
-                err = e
-            except Exception as e:
-                raise e
+def auto_retry(error: Union[Type[Exception], Sequence[Type[Exception]]],
+               before_retry: Optional[Callable[[], Awaitable[Any]]] = None):
+    def decorator(func: Callable[P, T]) -> Callable[P, T]:
+        @wraps(func)
+        async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+            err = None
+
+            for i in range(10):
+                try:
+                    return await func(*args, **kwargs)
+                except error as e:
+                    if before_retry:
+                        await before_retry()
+                    logger.error(f"Retrying... {i + 1}/10")
+                    logger.exception(e)
+                    err = e
+                except Exception as e:
+                    raise e
 
-        raise err
+            raise err
 
-    return wrapper
+        return wrapper
+
+    return decorator
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/network/host_prober.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/network/host_prober.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from asyncio import create_task, sleep, shield
-from functools import wraps
-from typing import AbstractSet, Optional, TypeVar, Union, Type, Tuple, Callable, Sequence
+from asyncio import create_task, sleep
+from typing import TypeVar, Sequence
 
 from icmplib import async_ping, NameLookupError, SocketAddressError, ICMPSocketError
 from nonebot import get_driver, logger
 from typing_extensions import ParamSpec
 
 from ..utils.percentile import percentile_str
 
@@ -27,19 +26,19 @@
     async def close(self):
         self._select_host_daemon_task.cancel()
 
     @property
     def host(self) -> str:
         return self._host
 
-    async def select_host(self, exclude: Optional[AbstractSet[str]] = None) -> bool:
+    async def select_host(self, exclude_current: bool = False) -> bool:
         logger.debug("paifuya host selecting...")
 
         ping_tasks = [create_task(async_ping(h))
-                      if not exclude or h not in exclude
+                      if not exclude_current or h == self._host
                       else None
                       for h in self._mirrors]
 
         selected = None
         selected_result = None
 
         for i, ping_task in enumerate(ping_tasks):
@@ -80,22 +79,7 @@
                 if await self.select_host():
                     await sleep(10 * 60)
                 else:
                     logger.error(f"all ping to paifuya host has failed. will retry after 60s...")
                     await sleep(60)
         except Exception as e:
             logger.exception(e)
-
-    def select_on_exception(self, exc_type: Union[Type[Exception], Tuple[Type[Exception], ...]]) -> \
-            Callable[[Callable[P, T]], Callable[P, T]]:
-        def decorator(func: Callable[P, T]) -> Callable[P, T]:
-            @wraps(func)
-            async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-                try:
-                    return await func(*args, **kwargs)
-                except exc_type as e:
-                    await shield(self.select_host(exclude={self._host}))
-                    raise e
-
-            return wrapper
-
-        return decorator
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/api.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime, timedelta
+from functools import partial
 from typing import List, AbstractSet, AsyncGenerator
 
 from httpx import AsyncClient, URL, HTTPError
 from nonebot import get_driver, logger
 
 from nonebot_plugin_majsoul.network.auto_retry import auto_retry
 from nonebot_plugin_majsoul.network.host_prober import HostProber
@@ -40,56 +41,52 @@
         )
 
         get_driver().on_shutdown(self.close)
 
     async def close(self):
         await self.client.aclose()
 
-    @auto_retry
-    @prober.select_on_exception(HTTPError)
+    @auto_retry(HTTPError, before_retry=partial(prober.select_host, exclude_current=True))
     async def search_player(
             self, nickname: str,
             *, limit: int = 10
     ) -> List[PlayerInfo]:
         resp = await self.client.get(
             URL(f"https://{prober.host}/{self._baseurl}/search_player/{nickname}"),
             params={"limit": limit}
         )
         return [PlayerInfo.parse_obj(x) for x in resp.json()]
 
-    @auto_retry
-    @prober.select_on_exception(HTTPError)
+    @auto_retry(HTTPError, before_retry=partial(prober.select_host, exclude_current=True))
     async def player_stats(
             self, player_id: int, start_time: datetime, end_time: datetime, room_rank: AbstractSet[RoomRank]
     ) -> PlayerStats:
         start_timestamp = int(start_time.timestamp() * 1000)
         end_timestamp = int(end_time.timestamp() * 1000)
         mode = ".".join(map(lambda x: str(x.value), room_rank))
         resp = await self.client.get(
             URL(f"https://{prober.host}/{self._baseurl}/player_stats/{player_id}/{start_timestamp}/{end_timestamp}"),
             params={"mode": mode}
         )
         return PlayerStats.parse_obj(resp.json())
 
-    @auto_retry
-    @prober.select_on_exception(HTTPError)
+    @auto_retry(HTTPError, before_retry=partial(prober.select_host, exclude_current=True))
     async def player_extended_stats(
             self, player_id: int, start_time: datetime, end_time: datetime, room_rank: AbstractSet[RoomRank]
     ) -> PlayerExtendedStats:
         start_timestamp = int(start_time.timestamp() * 1000)
         end_timestamp = int(end_time.timestamp() * 1000)
         mode = ".".join(map(lambda x: str(x.value), room_rank))
         resp = await self.client.get(
             URL(f"https://{prober.host}/{self._baseurl}/player_extended_stats/{player_id}/{start_timestamp}/{end_timestamp}"),
             params={"mode": mode}
         )
         return PlayerExtendedStats.parse_obj(resp.json())
 
-    @auto_retry
-    @prober.select_on_exception(HTTPError)
+    @auto_retry(HTTPError, before_retry=partial(prober.select_host, exclude_current=True))
     async def player_records(
             self, player_id: int, start_time: datetime, end_time: datetime, room_rank: AbstractSet[RoomRank],
             *, limit: int, descending: bool = True
     ) -> List[GameRecord]:
         start_timestamp = int(start_time.timestamp() * 1000)
         end_timestamp = int(end_time.timestamp() * 1000)
         mode = ".".join(map(lambda x: str(x.value), room_rank))
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/downloader.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paipu/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 from typing import Optional
 
 from nonebot import get_driver, logger
 from tensoul import MajsoulPaipuDownloader
+from websockets.exceptions import ConnectionClosedError
 
 from ..config import conf
+from ..network.auto_retry import auto_retry
 
 _downloader: Optional[MajsoulPaipuDownloader] = None
 
 
 def get_downloader():
     if _downloader is None:
         raise RuntimeError("downloader is not ready")
     return _downloader
 
 
 @get_driver().on_startup
-async def init_downloader():
+async def restart_downloader():
     global _downloader
+
+    if _downloader is not None:
+        await _downloader.close()
+        _downloader = None
+
     if conf.majsoul_username:
         _downloader = MajsoulPaipuDownloader()
         await _downloader.start()
         await _downloader.login(conf.majsoul_username, conf.majsoul_password)
         logger.opt(colors=True).success(f"Logged in as <y>{conf.majsoul_username}</y>")
 
 
+@auto_retry(ConnectionClosedError, restart_downloader)
+async def download_paipu(uuid: str):
+    return await get_downloader().download(uuid)
+
+
 @get_driver().on_shutdown
-async def destroy_downloader():
+async def _destroy_downloader():
     global _downloader
 
     if _downloader is not None:
         await _downloader.close()
         _downloader = None
+
+
+__all__ = ("get_downloader", "restart_downloader", "download_paipu")
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/paipu/query_paipu.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/paipu/query_paipu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from nonebot import logger, get_driver
+from nonebot import logger
 
+from .downloader import download_paipu
 from ..config import conf
 
 if not conf.majsoul_username:
     logger.warning("majsoul_paipu is disabled because majsoul_username is not configured")
 else:
     import json
     import re
     from asyncio import wait_for
 
     from nonebot import on_command, logger, require
     from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
     from nonebot.params import CommandArg
     from tensoul.downloader import MajsoulDownloadError
 
-    from .downloader import get_downloader
     from ..errors import BadRequestError
     from ..interceptors.handle_error import handle_error
     from ..utils.nonebot import default_cmd_start
 
     uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
 
     require("nonebot_plugin_gocqhttp_cross_machine_upload_file")
@@ -36,15 +36,15 @@
         if not mat:
             raise BadRequestError(f"使用方式：{default_cmd_start}下载雀魂牌谱 <牌谱网址>")
 
         uuid = mat.group(0)
 
         logger.opt(colors=True).info(f"Downloading paipu <y>{uuid}</y>")
         try:
-            coro = get_downloader().download(uuid)
+            coro = download_paipu(uuid)
             if conf.majsoul_query_timeout:
                 record = await wait_for(coro, timeout=conf.majsoul_query_timeout)
             else:
                 record = await coro
         except MajsoulDownloadError as e:
             logger.opt(colors=True).warning(f"Failed to download paipu <y>{uuid}</y>, code: {e.code}")
             if e.code == 1203:
```

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/src/nonebot_plugin_majsoul/utils/decode_integer.py` & `nonebot_plugin_majsoul-0.2.2/src/nonebot_plugin_majsoul/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.2.1.post1/PKG-INFO` & `nonebot_plugin_majsoul-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-majsoul
-Version: 0.2.1.post1
+Version: 0.2.2
 Summary: NoneBot2 雀魂信息查询插件
 License: AGPL-3.0
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: icmplib (>=3.0.3,<4.0.0)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: monthdelta (>=0.9.1,<0.10.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: icmplib (>=3.0.3)
+Requires-Dist: matplotlib (>=3.6.2)
+Requires-Dist: monthdelta (>=0.9.1)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.4)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1)
 Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
-Requires-Dist: tensoul (>=0.1.0,<0.2.0)
+Requires-Dist: tensoul (>=0.1.0)
 Requires-Dist: tzlocal (>=4.2)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.1.post1
-Summary: NoneBot2 éé­ä¿¡æ¯æ¥è¯¢æä»¶ License: AGPL-3.0 Author: ssttkkl
-Author-email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: icmplib
-(>=3.0.3,<4.0.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist:
-monthdelta (>=0.9.1,<0.10.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-
-file (>=0.1.4) Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1)
-Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0) Requires-Dist: tensoul
-(>=0.1.0,<0.2.0) Requires-Dist: tzlocal (>=4.2) Description-Content-Type: text/
-markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.2 Summary:
+NoneBot2 éé­ä¿¡æ¯æ¥è¯¢æä»¶ License: AGPL-3.0 Author: ssttkkl Author-
+email: huang.wen.long@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: icmplib (>=3.0.3)
+Requires-Dist: matplotlib (>=3.6.2) Requires-Dist: monthdelta (>=0.9.1)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3) Requires-Dist: nonebot-plugin-
+gocqhttp-cross-machine-upload-file (>=0.1.4) Requires-Dist: nonebot-plugin-
+send-anything-anywhere (>=0.2.1) Requires-Dist: nonebot2[httpx]
+(>=2.0.0,<3.0.0) Requires-Dist: tensoul (>=0.1.0) Requires-Dist: tzlocal
+(>=4.2) Description-Content-Type: text/markdown
                                    [nonebot]
     nonebot-plugin-majsoul ============ _â¨ éé­ä¿¡æ¯æ¥è¯¢æä»¶ â¨_
                            [license] [pypi] [python]
 å[DaiShengSheng/Majsoul_bot](https://github.com/DaiShengSheng/
 Majsoul_bot)å¯åèåçéé­ä¿¡æ¯æ¥è¯¢ Bot æä»¶ã
 æ¯æééå¨ï¼Onebot V11 ## åè½ ### éé­çè°±å± ####
 æ¥è¯¢ä¸ªäººæ°æ®ï¼å¯æç§æ¶é´ãæç§åºæ°ãæç§æ¿é´ç±»åæ¥è¯¢ï¼
```

