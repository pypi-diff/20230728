# Comparing `tmp/hikari_core-0.9.0.1.tar.gz` & `tmp/hikari_core-0.9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.9.0.1.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.2.tar", max compression
```

## Comparing `hikari_core-0.9.0.1.tar` & `hikari_core-0.9.0.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     5066 2023-07-15 04:38:48.665919 hikari_core-0.9.0.1/hikari_core/__init__.py
--rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.1/hikari_core/analyze.py
--rw-r--r--   0        0        0     3510 2023-07-15 04:45:24.575490 hikari_core-0.9.0.1/hikari_core/command_select.py
--rw-r--r--   0        0        0     1506 2023-06-09 16:02:41.277675 hikari_core-0.9.0.1/hikari_core/config.py
--rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.1/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.1/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2598 2023-07-07 08:04:40.589860 hikari_core-0.9.0.1/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2324 2023-07-07 09:04:55.774201 hikari_core-0.9.0.1/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.1/hikari_core/game/help.py
--rw-r--r--   0        0        0     2122 2023-07-10 07:31:07.868469 hikari_core-0.9.0.1/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2311 2023-07-07 08:58:39.067755 hikari_core-0.9.0.1/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.1/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.1/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.1/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.1/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3152 2023-07-13 08:56:17.527001 hikari_core-0.9.0.1/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.1/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11581 2023-07-14 08:31:13.584765 hikari_core-0.9.0.1/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10567 2023-07-13 09:41:24.730553 hikari_core-0.9.0.1/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     2726 2023-07-13 06:28:59.408115 hikari_core-0.9.0.1/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     3553 2023-07-13 06:29:52.468436 hikari_core-0.9.0.1/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     4085 2023-07-13 08:58:03.235425 hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3998 2023-07-13 08:58:08.113156 hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6867 2023-07-13 08:58:13.299011 hikari_core-0.9.0.1/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-07-14 12:03:50.576415 hikari_core-0.9.0.1/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     3783 2023-07-14 12:03:51.005556 hikari_core-0.9.0.1/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5166 2023-07-14 12:03:51.031428 hikari_core-0.9.0.1/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-07-14 12:03:51.047079 hikari_core-0.9.0.1/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7310 2023-07-14 12:03:51.076856 hikari_core-0.9.0.1/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-07-14 12:03:51.120915 hikari_core-0.9.0.1/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-07-14 12:03:51.167932 hikari_core-0.9.0.1/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28156 2023-07-14 13:10:22.607915 hikari_core-0.9.0.1/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    28082 2023-07-14 13:16:23.660810 hikari_core-0.9.0.1/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-07-14 12:03:51.349020 hikari_core-0.9.0.1/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-07-14 12:03:51.375787 hikari_core-0.9.0.1/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21441 2023-07-14 13:18:45.676515 hikari_core-0.9.0.1/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-07-14 12:03:51.448109 hikari_core-0.9.0.1/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-07-14 12:03:51.476400 hikari_core-0.9.0.1/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4393 2023-06-09 16:04:19.214393 hikari_core-0.9.0.1/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.1/LICENSE
--rw-r--r--   0        0        0     1549 2023-07-15 04:51:04.294442 hikari_core-0.9.0.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.1/README.md
--rw-r--r--   0        0        0     9940 1970-01-01 00:00:00.000000 hikari_core-0.9.0.1/setup.py
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 hikari_core-0.9.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5109 2023-07-28 07:31:48.896307 hikari_core-0.9.0.2/hikari_core/__init__.py
+-rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.2/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3720 2023-07-28 07:42:02.336925 hikari_core-0.9.0.2/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1687 2023-07-28 07:28:53.238024 hikari_core-0.9.0.2/hikari_core/config.py
+-rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.2/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.2/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.2/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.2/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.2/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.2/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.2/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.2/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.2/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.2/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.2/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.2/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.2/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.2/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.2/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.2/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     8680 2023-07-28 07:58:37.367865 hikari_core-0.9.0.2/hikari_core/moudle/wws_real_game.py
+-rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.2/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.2/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-07-28 07:59:48.943041 hikari_core-0.9.0.2/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-07-28 07:59:49.206550 hikari_core-0.9.0.2/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-07-28 07:59:49.234283 hikari_core-0.9.0.2/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-07-28 07:59:49.253458 hikari_core-0.9.0.2/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-07-28 07:59:49.290337 hikari_core-0.9.0.2/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-07-28 07:59:49.327128 hikari_core-0.9.0.2/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-07-28 07:59:49.366917 hikari_core-0.9.0.2/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-07-28 07:59:49.415115 hikari_core-0.9.0.2/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28083 2023-07-28 07:59:49.535736 hikari_core-0.9.0.2/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-07-28 07:59:49.616548 hikari_core-0.9.0.2/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-07-28 07:59:49.648871 hikari_core-0.9.0.2/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-07-28 07:59:49.680252 hikari_core-0.9.0.2/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-07-28 07:59:49.712630 hikari_core-0.9.0.2/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-07-28 07:59:49.760899 hikari_core-0.9.0.2/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.2/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.2/LICENSE
+-rw-r--r--   0        0        0     1572 2023-07-28 08:00:25.413986 hikari_core-0.9.0.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.2/README.md
+-rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.2/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.2/PKG-INFO
```

### Comparing `hikari_core-0.9.0.1/hikari_core/__init__.py` & `hikari_core-0.9.0.2/hikari_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,28 @@
 )
 
 
 async def init_hikari(
     platform: str,
     PlatformId: str,
     command_text: str = None,
+    GroupId: str = None,
 ) -> Hikari_Model:
     """Hikari初始化
 
     Args:
         platform (str): 平台类型
         PlatformId (str): 平台ID
         command_text (str): 传入指令，不带wws
 
     Returns:
         Hikari_Model: 可通过Hikari.Status和Hikari.Output.Data内数据判断是否输出
     """
     try:
-        userinfo = UserInfo_Model(Platform=platform, PlatformId=PlatformId)
+        userinfo = UserInfo_Model(Platform=platform, PlatformId=PlatformId, GroupId=GroupId)
         input = Input_Model(Command_Text=command_text)
         hikari = Hikari_Model(UserInfo=userinfo, Input=input)
         hikari = await analyze_command(hikari)
         if not hikari.Status == 'init' or not hikari.Function:
             return hikari
         hikari: Hikari_Model = await hikari.Function(hikari)
         return await output_hikari(hikari)
```

### Comparing `hikari_core-0.9.0.1/hikari_core/analyze.py` & `hikari_core-0.9.0.2/hikari_core/analyze.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/command_select.py` & `hikari_core-0.9.0.2/hikari_core/command_select.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .game.roll import roll_ship
 from .game.sx import get_sx_info
 from .moudle.publicAPI import get_ship_name
 from .moudle.wws_bind import change_BindInfo, delete_BindInfo, get_BindInfo, set_BindInfo, set_special_BindInfo
 
 # from .moudle.wws_clan import get_ClanInfo
 from .moudle.wws_info import get_AccountInfo
+from .moudle.wws_real_game import get_diff_ship, get_listen_list
 from .moudle.wws_recent import get_RecentInfo
 
 # from .moudle.wws_record import get_record
 from .moudle.wws_ship_info import get_ShipInfo
 from .moudle.wws_ship_recent import get_ShipRecent
 from .moudle.wws_shiprank import get_ShipRank
 
@@ -50,14 +51,16 @@
     command(('sx', '扫雪'), get_sx_info),
     command(('ban', '封号记录'), get_BanInfo),
     command(('box', 'sd', '圣诞船池'), check_christmas_box),
     command(('搜船名', '查船名', '船名'), get_ship_name),
     command(('help', '帮助'), get_help),
     command(('check_version', '检查更新'), check_version),
     command(('更新样式',), async_update_template),
+    command(('查询监控', '监控列表', '查询监听', '监听列表'), get_listen_list),
+    command(('测试监控'), get_diff_ship),
 ]
 
 second_command_list = [
     command(('recent', '近期'), get_ShipRecent),
     command(('ship', '单船'), get_ShipRecent),
     # command(("clan", "军团", "公会", "工会"), get_record),
     # command(("record", "历史记录"), get_record),
```

### Comparing `hikari_core-0.9.0.1/hikari_core/config.py` & `hikari_core-0.9.0.2/hikari_core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from typing import Optional
 
 from loguru import logger
 from pydantic import BaseModel
 
+from .data_source import dir_path
+
 
 class Config_Model(BaseModel):
     proxy: Optional[str]
     http2: bool = True
     token: Optional[str] = '123456:111111111111'
     auto_rendering: bool = True
     auto_image: bool = True
     use_broswer: Optional[str] = 'chromium'
+    game_path: Optional[str] = f'{dir_path}/game'
 
 
 hikari_config = Config_Model()
 
 
 def set_hikari_config(  # noqa: PLR0913
     proxy: Optional[str],
     http2: bool = True,
     token: Optional[str] = '123456:111111111111',
     auto_rendering: bool = True,
     auto_image: bool = True,
     use_broswer: Optional[str] = 'chromium',
+    game_path: Optional[str] = f'{dir_path}/game',
 ):
     """配置Hikari-core
 
     Args:
         proxy (str): 访问WG使用的代理，格式http://localhost:7890
         http2 (bool): 是否开启http2，默认启用
         token (str): #请加群联系雨季获取api_key和token Q群:967546463
@@ -38,8 +42,9 @@
     global hikari_config  # noqa: PLW0602
     hikari_config.proxy = proxy
     hikari_config.http2 = http2
     hikari_config.token = token
     hikari_config.auto_rendering = auto_rendering
     hikari_config.auto_image = auto_image
     hikari_config.use_broswer = use_broswer
+    hikari_config.game_path = game_path
     logger.info(f'当前hikari-core配置\n{hikari_config}')
```

### Comparing `hikari_core-0.9.0.1/hikari_core/data_source.py` & `hikari_core-0.9.0.2/hikari_core/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/game/ban_search.py` & `hikari_core-0.9.0.2/hikari_core/game/ban_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                         return hikari.error('目前仅支持国服查询')
                 else:
                     return hikari.error('未查询到该用户绑定信息，请使用wws 查询绑定 进行检查')
         else:
             return hikari.error('当前请求状态错误')
         url = 'https://api.wows.shinoaki.com/public/wows/ban/cn/user'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.post(url, json={'accountId': hikari.Input.AccountId}, timeout=None)
+        resp = await client_yuyuko.post(url, json={'accountId': hikari.Input.AccountId}, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
         if result['code'] == 200 and result['data']:
             hikari = hikari.set_template_info('wws-ban.html', 900, 100)
             return hikari.success(result['data'])
         elif result['code'] == 404 and result['data']:
             hikari = hikari.set_template_info('wws-unban.html', 900, 100)
```

### Comparing `hikari_core-0.9.0.1/hikari_core/game/box_check.py` & `hikari_core-0.9.0.2/hikari_core/game/box_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             return hikari.error('当前请求状态错误')
         url = 'https://api.wows.shinoaki.com/public/wows/christmas/ship/box'
         if hikari.Input.Search_Type == 3:
             params = {'server': hikari.Input.Server, 'accountId': hikari.Input.AccountId}
         else:
             params = {'server': hikari.Input.Platform, 'accountId': hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
         if result['code'] == 200 and result['data']:
             hikari = hikari.set_template_info('wws-box-christmas.html', 920, 1000)
             return hikari.success(result['data'])
         elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
```

### Comparing `hikari_core-0.9.0.1/hikari_core/game/help.py` & `hikari_core-0.9.0.2/hikari_core/game/help.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/game/roll.py` & `hikari_core-0.9.0.2/hikari_core/game/roll.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             'county': hikari.Input.ShipInfo.Ship_Nation,
             'level': hikari.Input.ShipInfo.Ship_Tier,
             'shipName': '',
             'shipType': hikari.Input.ShipInfo.Ship_Type,
         }
         url = 'https://api.wows.shinoaki.com/public/wows/roll/ship/roll'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.post(url, json=params, timeout=None)
+        resp = await client_yuyuko.post(url, json=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             return hikari.success(f"本次roll到了{result['data']['shipNameCn']}")
         elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
         elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
```

### Comparing `hikari_core-0.9.0.1/hikari_core/game/sx.py` & `hikari_core-0.9.0.2/hikari_core/game/sx.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             return hikari.error('当前请求状态错误')
         url = 'https://api.wows.shinoaki.com/public/wows/christmas/ship/christmas'
         if hikari.Input.Search_Type == 3:
             params = {'server': hikari.Input.Server, 'accountId': hikari.Input.AccountId}
         else:
             params = {'server': hikari.Input.Platform, 'accountId': hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
         if result['code'] == 200 and result['data']:
             hikari = hikari.set_template_info('wws-sx.html', 920, 1000)
             return hikari.success(result['data'])
         elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
```

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0.2/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0.2/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0.2/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0.2/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/model.py` & `hikari_core-0.9.0.2/hikari_core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     async def __call__(self, **kwargs):
         ...
 
 
 class UserInfo_Model(BaseModel):
     Platform: str = 'QQ'
     PlatformId: str = '1119809439'
+    GroupId: str = None
 
 
 class Ship_Model(BaseModel):
     Ship_Nation: Optional[str]
     Ship_Tier: Optional[int]
     Ship_Type: Optional[str]
     Ship_Name_Cn: Optional[str]
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0.2/hikari_core/moudle/publicAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 async def get_nation_list():
     try:
         msg = ''
         url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/nation/list'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, timeout=None)
+        resp = await client_yuyuko.get(url, timeout=10)
         result = orjson.loads(resp.content)
         for nation in result['data']:
             msg: str = msg + f"{nation['cn']}：{nation['nation']}\n"
         return msg
     except PoolTimeout:
         await recreate_client_yuyuko()
         return
@@ -47,15 +47,15 @@
             'level': hikari.Input.ShipInfo.Ship_Tier,
             'shipName': '',
             'shipType': hikari.Input.ShipInfo.Ship_Type,
             'groupType': 'default',
         }
         url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['data']:
             for ship in result['data']:
                 msg += f"{ship['nameCn']}：{ship['nameEnglish']}\n"
             return hikari.success(msg)
         else:
             return hikari.failed('没有符合的船只')
@@ -76,15 +76,15 @@
         result = shipname.split('.')
         if len(result) == 2 and result[1].isdigit():
             shipname = result[0]
             shipname_select_index = int(result[1])
         url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
         params = {'country': '', 'level': '', 'shipName': shipname, 'shipType': '', 'groupType': 'default'}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         List, select_List = [], []
         if result['code'] == 200 and result['data']:
             for each in result['data']:
                 List.append(
                     Ship_Model(
                         Ship_Nation=each['country'],
@@ -114,15 +114,15 @@
 
 
 async def get_all_shipList():
     try:
         url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
         params = {'country': '', 'level': '', 'shipName': '', 'shipType': '', 'groupType': 'default'}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             return result['data']
         else:
             return None
     except PoolTimeout:
         await recreate_client_yuyuko()
@@ -132,15 +132,15 @@
 
 
 async def get_AccountIdByName(server: str, name: str) -> str:
     try:
         url = 'https://api.wows.shinoaki.com/public/wows/account/search/user'
         params = {'server': server, 'userName': name}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             return int(result['data']['accountId'])
         else:
             return result['message']
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
@@ -154,15 +154,15 @@
 
 
 async def get_ClanIdByName(server: str, tag: str):
     try:
         url = 'https://api.wows.shinoaki.com/public/wows/clan/search'
         params = {'server': server, 'tag': tag, 'type': 1}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             # for each in result['data']:
             #    List.append([each['clanId'],each['name'],each['serverName'],each['tag']])
             return result['data']
         else:
             return None
@@ -226,15 +226,15 @@
         return
 
 
 async def get_MyShipRank_yuyuko(params) -> int:
     try:
         url = 'https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             if result['data']['ranking']:
                 return result['data']['ranking']
             elif not result['data']['ranking'] and not result['data']['serverId'] == 'cn':
                 ranking = await get_MyShipRank_Numbers(result['data']['httpUrl'], result['data']['serverId'])
                 if ranking:
@@ -288,15 +288,15 @@
         post_data = {
             'accountId': int(accountId),
             'ranking': int(ranking),
             'serverId': serverId,
             'shipId': int(shipId),
         }
         client_yuyuko = await get_client_yuyuko()
-        await client_yuyuko.post(url, json=post_data, timeout=None)
+        await client_yuyuko.post(url, json=post_data, timeout=10)
         return
     except PoolTimeout:
         await recreate_client_yuyuko()
         return
     except Exception:
         logger.error(traceback.format_exc())
         return
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_bind.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_bind.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 async def get_BindInfo(hikari: Hikari_Model) -> Hikari_Model:
     try:
         if hikari.Status != 'init':
             return hikari.error('当前请求状态错误')
         url = 'https://v3-api.wows.shinoaki.com/api/user/platform/bind/list'
         params = {'platformType': hikari.Input.Platform, 'platformId': hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['message'] == 'success':
             if result['data']:
                 hikari = hikari.set_template_info('bind-list.html', 900, 440)
                 return hikari.success(result['data'])
             else:
                 return hikari.failed('该用户似乎还没绑定窝窝屎账号')
@@ -48,15 +48,15 @@
                 if not isinstance(hikari.Input.AccountId, int):
                     return hikari.error(f'{hikari.Input.AccountId}')
         else:
             return hikari.error('当前请求状态错误')
         url = 'https://api.wows.shinoaki.com/api/wows/bind/account/platform/bind/put'
         params = {'platformType': hikari.Input.Platform, 'platformId': hikari.Input.PlatformId, 'accountId': hikari.Input.AccountId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['message'] == 'success':
             return hikari.success('绑定成功')
         elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
@@ -75,15 +75,15 @@
 async def set_special_BindInfo(hikari: Hikari_Model) -> Hikari_Model:
     try:
         if hikari.Status != 'init':
             return hikari.error('当前请求状态错误')
         url = 'https://api.wows.shinoaki.com/api/wows/bind/account/platform/bind/put'
         params = {'platformType': hikari.Input.Platform, 'platformId': hikari.Input.PlatformId, 'accountId': hikari.Input.AccountId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['message'] == 'success':
             return hikari.success('绑定成功')
         elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
@@ -160,15 +160,15 @@
                 hikari.Input.Select_Data = hikari.Output.Data
             if hikari.Input.Select_Index > len(hikari.Input.Select_Data):
                 return hikari.error('请选择正确的序号')
             hikari.Input.AccountId = hikari.Input.Select_Data[hikari.Input.Select_Index - 1]['accountId']
             url = 'https://api.wows.shinoaki.com/api/wows/bind/account/platform/bind/remove'
             params = {'platformType': hikari.Input.Platform, 'platformId': hikari.Input.PlatformId, 'accountId': hikari.Input.AccountId}
             client_yuyuko = await get_client_yuyuko()
-            resp = await client_yuyuko.get(url, params=params, timeout=None)
+            resp = await client_yuyuko.get(url, params=params, timeout=10)
             result = orjson.loads(resp.content)
             if result['code'] == 200 and result['message'] == 'success':
                 return hikari.success(
                     f"删除绑定成功，删除的账号为{hikari.Input.Select_Data[hikari.Input.Select_Index - 1]['server']}：{hikari.Input.Select_Data[hikari.Input.Select_Index - 1]['userName']}"
                 )
             elif result['code'] == 500:
                 return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
@@ -190,15 +190,15 @@
     try:
         url = 'https://api.wows.shinoaki.com/public/wows/bind/account/platform/bind/list'
         params = {
             'platformType': platformType,
             'platformId': platformId,
         }
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['message'] == 'success':
             if result['data']:
                 for each in result['data']:
                     if each['defaultId']:
                         return each
             else:
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             logger.success('跳过上报数据，直接请求')
         url = 'https://v3-api.wows.shinoaki.com/public/wows/account/user/info'
         if hikari.Input.Search_Type == 3:
             params = {'server': hikari.Input.Server, 'accountId': hikari.Input.AccountId}
         else:
             params = {'server': hikari.Input.Platform, 'accountId': hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
         if result['code'] == 200 and result['data']:
             hikari = hikari.set_template_info('wws-info.html', 920, 1000)
             return hikari.success(result['data'])
         elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 'accountId': hikari.Input.PlatformId,
                 'dateTime': hikari.Input.Recent_Date,
                 'day': hikari.Input.Recent_Day,
                 'shipId': 0,
             }
         print(params)
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
         if result['code'] == 200:
             if result['data']['battleTypeInfo']['PVP']['battle'] or result['data']['battleTypeInfo']['RANK_SOLO']['battle']:
                 hikari = hikari.set_template_info('wws-info-recent.html', 1200, 100)
                 return hikari.success(result['data'])
             else:
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_info.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if hikari.Input.Search_Type == 3:
             params = {'server': hikari.Input.Server, 'accountId': hikari.Input.AccountId, 'shipId': hikari.Input.ShipInfo.Ship_Id}
         else:
             params = {'server': hikari.Input.Platform, 'accountId': hikari.Input.PlatformId, 'shipId': hikari.Input.ShipInfo.Ship_Id}
 
         ranking = await get_MyShipRank_yuyuko(params)
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
 
         if result['code'] == 200 and result['data']:
             if result['data']['typeInfo']['PVP']['battle'] or result['data']['typeInfo']['RANK_SOLO']['battle']:
                 hikari.set_template_info('wws-ship.html', 800, 100)
                 result['data']['shipRank'] = ranking
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 'server': hikari.Input.Platform,
                 'accountId': hikari.Input.PlatformId,
                 'shipId': hikari.Input.ShipInfo.Ship_Id,
                 'day': hikari.Input.Recent_Day,
             }
 
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         hikari.Output.Yuyuko_Code = result['code']
 
         if result['code'] == 200 and result['data']:
             hikari.set_template_info('wws-ship-recent.html', 800, 100)
             return hikari.success(result['data'])
         elif result['code'] == 403:
```

### Comparing `hikari_core-0.9.0.1/hikari_core/moudle/wws_shiprank.py` & `hikari_core-0.9.0.2/hikari_core/moudle/wws_shiprank.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 async def search_ShipRank_Yuyuko(hikari: Hikari_Model):
     try:
         url = 'https://api.wows.shinoaki.com/upload/numbers/data/v2/upload/ship/rank'
         params = {'server': hikari.Input.Server, 'shipId': int(hikari.Input.ShipInfo.Ship_Id)}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             hikari.set_template_info('ship-rank.html', 1300, 100)
             result_data = {'data': result['data'], 'shipInfo': hikari.Input.ShipInfo.dict()}
             return hikari.success(result_data)
         else:
             return hikari
@@ -79,15 +79,15 @@
         return hikari.error('wuwuwu出了点问题，请联系麻麻解决')
 
 
 async def search_ShipRank_Numbers(hikari: Hikari_Model):
     try:
         client_default = await get_client_default()
         number_url = f'{number_url_homes[hikari.Input.Server]}/ship/{hikari.Input.ShipInfo.Ship_Id},{hikari.Input.ShipInfo.ship_Name_Numbers}'
-        resp = await client_default.get(number_url, timeout=None)
+        resp = await client_default.get(number_url, timeout=10)
         soup = BeautifulSoup(resp.content, 'html.parser')
         data = soup.select('tr[class="cells-middle"]')
         infoList = await set_ShipRank_Numbers(data, hikari.Input.Server, hikari.Input.ShipInfo.Ship_Id)
         if infoList:
             hikari.set_template_info('ship-rank.html', 1300, 100)
             result_data = {'data': infoList, 'shipInfo': hikari.Input.ShipInfo.dict()}
             return hikari.success(result_data), infoList
@@ -104,15 +104,15 @@
         return hikari.error('wuwuwu出了点问题，请联系麻麻解决'), None
 
 
 async def post_ShipRank(data):
     try:
         url = 'https://api.wows.shinoaki.com/upload/numbers/data/v2/upload/ship/rank'
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.post(url, json=data, timeout=None)
+        resp = await client_yuyuko.post(url, json=data, timeout=10)
         result = orjson.loads(resp.content)
         logger.success(result)
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
     except PoolTimeout:
         await recreate_client_yuyuko()
     except Exception:
@@ -120,15 +120,15 @@
 
 
 async def search_cn_rank(hikari: Hikari_Model):
     try:
         url = 'https://api.wows.shinoaki.com/wows/rank/ship/server'
         params = {'server': hikari.Input.Server, 'shipId': int(hikari.Input.ShipInfo.Ship_Id), 'page': 1}
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        resp = await client_yuyuko.get(url, params=params, timeout=10)
         result = orjson.loads(resp.content)
         if result['code'] == 200 and result['data']:
             hikari.set_template_info('ship-rank.html', 1300, 100)
             result_data = {'data': result['data'], 'shipInfo': hikari.Input.ShipInfo.dict()}
             return hikari.success(result_data)
         else:
             return hikari.failed(f"{result['message']}")
```

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/bind-list.html` & `hikari_core-0.9.0.2/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0.2/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0.2/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-info.html`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
 						<span class="pr-number">{{ data['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span
 								class="pr-text"></span></span>
 						<div class="pr-bar"></div>
 					</div>
 				</div>
 
 				<div class="recnet-time">
-					<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d%H:%M:%S',time.localtime(abs(data['lastBattleTime'])))}}</span>
+					<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['lastBattleTime'])))}}</span>
 				</div>
 
 				<div class="overview-change">
 					<div class="overview-change-item left-item">
 						<div class="left-item-top item-top">
 							<div class="overview-count-title item-top-top">场次</div>
 							<div class="overview-count item-top-bottom">{{
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% if data['userInfo']['clanInfo']['tag'] %}
 [{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
 {{ data['userInfo']['userName'] }}
 {{ data['userInfo']['serverCn'] }}
 {{ data['prInfo']['value'] }}    
-æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d%H:%M:%S',time.localtime(abs
+æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs
 (data['lastBattleTime'])))}}
 åºæ¬¡
 {{ data['battleTypeInfo']['PVP']['shipInfo']['battleInfo']['battle'] }}
 PR
 è¾ä¸æ¬¡
 {{ '%+d' | format(data['dwpData']['pr']) }}
 èç
```

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0.2/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/hikari_core/utils.py` & `hikari_core-0.9.0.2/hikari_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     def reset(self, key):
         self.count[key] = 0
 
 
 async def download(url, path, proxy=None):
     async with httpx.AsyncClient(proxies=proxy) as client:
-        resp = await client.get(url, timeout=None)
+        resp = await client.get(url, timeout=10)
         content = resp.read()
         content = content.replace(b'\n', b'\r\n')
         with open(path, 'wb') as f:
             f.write(content)
 
 
 async def byte2md5(bytes) -> str:
```

### Comparing `hikari_core-0.9.0.1/LICENSE` & `hikari_core-0.9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.1/pyproject.toml` & `hikari_core-0.9.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.9.0.1"
+version = "0.9.0.2"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
@@ -17,14 +17,15 @@
 APScheduler = "^3.10.1"
 jinja2 = "^3.0.0"
 pydantic = "^1.10.7"
 playwright = ">=1.17.2"
 aiofiles = ">=0.8.0"
 beautifulsoup4 = "^4.12.2"
 loguru = "^0.7.0"
+json_tools = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "tsinghua"
```

### Comparing `hikari_core-0.9.0.1/setup.py` & `hikari_core-0.9.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,22 +210,23 @@
 install_requires = \
 ['APScheduler>=3.10.1,<4.0.0',
  'aiofiles>=0.8.0',
  'asyncio>=3.4.3,<4.0.0',
  'beautifulsoup4>=4.12.2,<5.0.0',
  'httpx[http2]>=0.24.0',
  'jinja2>=3.0.0,<4.0.0',
+ 'json_tools>=0.4.1,<0.5.0',
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.9.0.1',
+    'version': '0.9.0.2',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-0.9.0.1/PKG-INFO` & `hikari_core-0.9.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.9.0.1
+Version: 0.9.0.2
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: APScheduler (>=3.10.1,<4.0.0)
 Requires-Dist: aiofiles (>=0.8.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: httpx[http2] (>=0.24.0)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
+Requires-Dist: json_tools (>=0.4.1,<0.5.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: orjson (>=3.8.11,<4.0.0)
 Requires-Dist: playwright (>=1.17.2)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Project-URL: Repository, https://github.com/wows-yuyuko/Hikari-core
 Description-Content-Type: text/markdown
```

