# Comparing `tmp/hikari_core-0.9.0.2.tar.gz` & `tmp/hikari_core-0.9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.9.0.2.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.3.tar", max compression
```

## Comparing `hikari_core-0.9.0.2.tar` & `hikari_core-0.9.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     5109 2023-07-28 07:31:48.896307 hikari_core-0.9.0.2/hikari_core/__init__.py
--rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.2/hikari_core/analyze.py
--rw-r--r--   0        0        0     3720 2023-07-28 07:42:02.336925 hikari_core-0.9.0.2/hikari_core/command_select.py
--rw-r--r--   0        0        0     1687 2023-07-28 07:28:53.238024 hikari_core-0.9.0.2/hikari_core/config.py
--rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.2/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.2/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.2/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.2/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.2/hikari_core/game/help.py
--rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.2/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.2/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.2/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.2/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.2/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.2/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.2/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.2/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.2/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.2/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.2/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.2/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     8680 2023-07-28 07:58:37.367865 hikari_core-0.9.0.2/hikari_core/moudle/wws_real_game.py
--rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.2/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.2/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-07-28 07:59:48.943041 hikari_core-0.9.0.2/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     3783 2023-07-28 07:59:49.206550 hikari_core-0.9.0.2/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5166 2023-07-28 07:59:49.234283 hikari_core-0.9.0.2/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-07-28 07:59:49.253458 hikari_core-0.9.0.2/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7310 2023-07-28 07:59:49.290337 hikari_core-0.9.0.2/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-07-28 07:59:49.327128 hikari_core-0.9.0.2/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-07-28 07:59:49.366917 hikari_core-0.9.0.2/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28156 2023-07-28 07:59:49.415115 hikari_core-0.9.0.2/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    28083 2023-07-28 07:59:49.535736 hikari_core-0.9.0.2/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-07-28 07:59:49.616548 hikari_core-0.9.0.2/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-07-28 07:59:49.648871 hikari_core-0.9.0.2/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21441 2023-07-28 07:59:49.680252 hikari_core-0.9.0.2/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-07-28 07:59:49.712630 hikari_core-0.9.0.2/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-07-28 07:59:49.760899 hikari_core-0.9.0.2/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.2/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.2/LICENSE
--rw-r--r--   0        0        0     1572 2023-07-28 08:00:25.413986 hikari_core-0.9.0.2/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.2/README.md
--rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.2/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5109 2023-07-28 07:31:48.896307 hikari_core-0.9.0.3/hikari_core/__init__.py
+-rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.3/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3720 2023-07-28 07:42:02.336925 hikari_core-0.9.0.3/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1687 2023-07-28 08:11:43.676745 hikari_core-0.9.0.3/hikari_core/config.py
+-rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.3/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.3/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.3/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.3/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.3/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.3/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.3/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.3/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.3/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.3/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.3/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.3/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.3/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.3/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.3/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.3/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.3/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.3/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.3/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.3/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.3/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     9022 2023-07-28 08:16:59.730184 hikari_core-0.9.0.3/hikari_core/moudle/wws_real_game.py
+-rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.3/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.3/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.3/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.3/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-07-28 08:17:20.343610 hikari_core-0.9.0.3/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-07-28 08:17:20.587886 hikari_core-0.9.0.3/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-07-28 08:17:20.613615 hikari_core-0.9.0.3/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-07-28 08:17:20.629299 hikari_core-0.9.0.3/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-07-28 08:17:20.670812 hikari_core-0.9.0.3/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-07-28 08:17:20.853503 hikari_core-0.9.0.3/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-07-28 08:17:20.961319 hikari_core-0.9.0.3/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-07-28 08:17:21.048231 hikari_core-0.9.0.3/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28083 2023-07-28 08:17:21.078148 hikari_core-0.9.0.3/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-07-28 08:17:21.130303 hikari_core-0.9.0.3/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-07-28 08:17:21.187919 hikari_core-0.9.0.3/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-07-28 08:17:21.230947 hikari_core-0.9.0.3/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-07-28 08:17:21.259238 hikari_core-0.9.0.3/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-07-28 08:17:21.301324 hikari_core-0.9.0.3/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.3/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.3/LICENSE
+-rw-r--r--   0        0        0     1572 2023-07-28 08:17:41.767465 hikari_core-0.9.0.3/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.3/README.md
+-rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.3/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.3/PKG-INFO
```

### Comparing `hikari_core-0.9.0.2/hikari_core/__init__.py` & `hikari_core-0.9.0.3/hikari_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/analyze.py` & `hikari_core-0.9.0.3/hikari_core/analyze.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/command_select.py` & `hikari_core-0.9.0.3/hikari_core/command_select.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/config.py` & `hikari_core-0.9.0.3/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/data_source.py` & `hikari_core-0.9.0.3/hikari_core/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/game/ban_search.py` & `hikari_core-0.9.0.3/hikari_core/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/game/box_check.py` & `hikari_core-0.9.0.3/hikari_core/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/game/help.py` & `hikari_core-0.9.0.3/hikari_core/game/help.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/game/roll.py` & `hikari_core-0.9.0.3/hikari_core/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/game/sx.py` & `hikari_core-0.9.0.3/hikari_core/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0.3/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0.3/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0.3/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0.3/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0.3/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0.3/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0.3/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/model.py` & `hikari_core-0.9.0.3/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0.3/hikari_core/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_bind.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_real_game.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_real_game.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,14 @@
     'asia': 'https://api.worldofwarships.asia/wows/ships/stats/',
     'eu': 'https://api.worldofwarships.eu/wows/ships/stats/',
     'na': 'https://api.worldofwarships.com/wows/ships/stats/',
     'cn': 'https://vortex.wowsgame.cn/api/accounts/',
 }
 seach_ship_url = 'https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/info'
 
-listen_config_path = f'{hikari_config.game_path}/listen_config.json'
-listen_data_path = f'{hikari_config.game_path}/account_data'
-
-if not os.path.exists(listen_config_path):
-    with open(listen_config_path, 'w') as f:
-        f.write(orjson.dumps({}).decode())
-
-if not os.path.exists(listen_data_path):
-    os.mkdir(listen_data_path)
-
 
 async def get_latest_info(server, account_id):
     try:
         if server != 'cn':
             client_wg = await get_client_wg()
             params = {
                 'application_id': '907d9c6bfc0d896a2c156e57194a97cf',
@@ -62,35 +52,48 @@
         await recreate_client_wg()
     except Exception:
         logger.error(traceback.format_exc())
 
 
 def get_last_info(account_id):
     try:
+        listen_data_path = f'{hikari_config.game_path}/account_data'
+        if not os.path.exists(listen_data_path):
+            os.mkdir(listen_data_path)
         with open(f'{listen_data_path}/{account_id}.json', 'rb') as f:
             last_info = orjson.loads(f.read())
         return last_info
     except Exception:
         print(traceback.format_exc())
 
 
 def write_latest_info(account_id, data):
     try:
+        listen_data_path = f'{hikari_config.game_path}/account_data'
+        if not os.path.exists(listen_data_path):
+            os.mkdir(listen_data_path)
         with open(f'{listen_data_path}/{account_id}.json', 'w', encoding='utf-8') as f:
             f.write(orjson.dumps(data).decode())
     except Exception:
         print(traceback.format_exc())
 
 
 def jsonDiff(a, b):
     result = json_tools.diff(a, b)
     return result
 
 
 def get_config():
+    listen_data_path = f'{hikari_config.game_path}/account_data'
+    if not os.path.exists(listen_data_path):
+        os.mkdir(listen_data_path)
+    listen_config_path = f'{hikari_config.game_path}/listen_config.json'
+    if not os.path.exists(listen_config_path):
+        with open(listen_config_path, 'w') as f:
+            f.write(orjson.dumps({}).decode())
     with open(listen_config_path, 'rb') as f:
         config = orjson.loads(f.read())
     return config
 
 
 async def get_diff_ship(hikari: Hikari_Model):  # noqa: PLR0915
     try:
```

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_info.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_ship_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_ship_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/moudle/wws_shiprank.py` & `hikari_core-0.9.0.3/hikari_core/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/bind-list.html` & `hikari_core-0.9.0.3/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0.3/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0.3/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0.3/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/hikari_core/utils.py` & `hikari_core-0.9.0.3/hikari_core/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/LICENSE` & `hikari_core-0.9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.2/pyproject.toml` & `hikari_core-0.9.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.9.0.2"
+version = "0.9.0.3"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
```

### Comparing `hikari_core-0.9.0.2/setup.py` & `hikari_core-0.9.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.9.0.2',
+    'version': '0.9.0.3',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-0.9.0.2/PKG-INFO` & `hikari_core-0.9.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.9.0.2
+Version: 0.9.0.3
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

