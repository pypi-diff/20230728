# Comparing `tmp/hikari_core-0.9.0.4.tar.gz` & `tmp/hikari_core-0.9.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.9.0.4.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.5.tar", max compression
```

## Comparing `hikari_core-0.9.0.4.tar` & `hikari_core-0.9.0.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     5109 2023-07-28 07:31:48.896307 hikari_core-0.9.0.4/hikari_core/__init__.py
--rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.4/hikari_core/analyze.py
--rw-r--r--   0        0        0     3720 2023-07-28 07:42:02.336925 hikari_core-0.9.0.4/hikari_core/command_select.py
--rw-r--r--   0        0        0     1687 2023-07-28 08:11:43.676745 hikari_core-0.9.0.4/hikari_core/config.py
--rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.4/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.4/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.4/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.4/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.4/hikari_core/game/help.py
--rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.4/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.4/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.4/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.4/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.4/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.4/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.4/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.4/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.4/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.4/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.4/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.4/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.4/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.4/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.4/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.4/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     9092 2023-07-28 08:21:37.959850 hikari_core-0.9.0.4/hikari_core/moudle/wws_real_game.py
--rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.4/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.4/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.4/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.4/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-07-28 08:17:20.343610 hikari_core-0.9.0.4/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     3783 2023-07-28 08:17:20.587886 hikari_core-0.9.0.4/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5166 2023-07-28 08:17:20.613615 hikari_core-0.9.0.4/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-07-28 08:17:20.629299 hikari_core-0.9.0.4/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7310 2023-07-28 08:17:20.670812 hikari_core-0.9.0.4/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-07-28 08:17:20.853503 hikari_core-0.9.0.4/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-07-28 08:17:20.961319 hikari_core-0.9.0.4/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28156 2023-07-28 08:17:21.048231 hikari_core-0.9.0.4/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    28083 2023-07-28 08:17:21.078148 hikari_core-0.9.0.4/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-07-28 08:17:21.130303 hikari_core-0.9.0.4/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-07-28 08:17:21.187919 hikari_core-0.9.0.4/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21441 2023-07-28 08:17:21.230947 hikari_core-0.9.0.4/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-07-28 08:17:21.259238 hikari_core-0.9.0.4/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-07-28 08:17:21.301324 hikari_core-0.9.0.4/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.4/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.4/LICENSE
--rw-r--r--   0        0        0     1572 2023-07-28 08:22:17.798452 hikari_core-0.9.0.4/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.4/README.md
--rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.4/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5109 2023-07-28 07:31:48.896307 hikari_core-0.9.0.5/hikari_core/__init__.py
+-rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.5/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3720 2023-07-28 07:42:02.336925 hikari_core-0.9.0.5/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1687 2023-07-28 08:11:43.676745 hikari_core-0.9.0.5/hikari_core/config.py
+-rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.5/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.5/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2596 2023-07-27 08:41:51.618680 hikari_core-0.9.0.5/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2322 2023-07-27 08:41:54.883058 hikari_core-0.9.0.5/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.5/hikari_core/game/help.py
+-rw-r--r--   0        0        0        2 2023-07-28 08:35:12.065554 hikari_core-0.9.0.5/hikari_core/game/listen_config.json
+-rw-r--r--   0        0        0     2120 2023-07-27 08:42:02.060038 hikari_core-0.9.0.5/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2309 2023-07-27 08:41:58.810270 hikari_core-0.9.0.5/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.5/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.5/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.5/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.5/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.5/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.5/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.5/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.5/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.5/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3177 2023-07-28 07:21:03.627231 hikari_core-0.9.0.5/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.5/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11565 2023-07-27 08:42:33.417281 hikari_core-0.9.0.5/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10557 2023-07-27 08:42:38.327361 hikari_core-0.9.0.5/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2724 2023-07-27 08:42:41.165778 hikari_core-0.9.0.5/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     9091 2023-07-28 08:27:08.082798 hikari_core-0.9.0.5/hikari_core/moudle/wws_real_game.py
+-rw-r--r--   0        0        0     3551 2023-07-27 08:42:43.695971 hikari_core-0.9.0.5/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     4083 2023-07-27 08:42:46.702994 hikari_core-0.9.0.5/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3996 2023-07-27 08:42:48.787811 hikari_core-0.9.0.5/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6859 2023-07-27 08:42:56.242021 hikari_core-0.9.0.5/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-07-28 08:35:11.074545 hikari_core-0.9.0.5/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-07-28 08:35:11.435773 hikari_core-0.9.0.5/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-07-28 08:35:11.523017 hikari_core-0.9.0.5/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-07-28 08:35:11.540758 hikari_core-0.9.0.5/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-07-28 08:35:11.585298 hikari_core-0.9.0.5/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-07-28 08:35:11.640437 hikari_core-0.9.0.5/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-07-28 08:35:11.683589 hikari_core-0.9.0.5/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-07-28 08:35:11.722574 hikari_core-0.9.0.5/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28083 2023-07-28 08:35:11.758452 hikari_core-0.9.0.5/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-07-28 08:35:11.827208 hikari_core-0.9.0.5/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-07-28 08:35:11.860192 hikari_core-0.9.0.5/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-07-28 08:35:11.893502 hikari_core-0.9.0.5/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-07-28 08:35:11.926477 hikari_core-0.9.0.5/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-07-28 08:35:11.970911 hikari_core-0.9.0.5/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4391 2023-07-27 08:41:46.196862 hikari_core-0.9.0.5/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.5/LICENSE
+-rw-r--r--   0        0        0     1572 2023-07-28 08:35:40.460016 hikari_core-0.9.0.5/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.5/README.md
+-rw-r--r--   0        0        0     9969 1970-01-01 00:00:00.000000 hikari_core-0.9.0.5/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 hikari_core-0.9.0.5/PKG-INFO
```

### Comparing `hikari_core-0.9.0.4/hikari_core/__init__.py` & `hikari_core-0.9.0.5/hikari_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/analyze.py` & `hikari_core-0.9.0.5/hikari_core/analyze.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/command_select.py` & `hikari_core-0.9.0.5/hikari_core/command_select.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/config.py` & `hikari_core-0.9.0.5/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/data_source.py` & `hikari_core-0.9.0.5/hikari_core/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/game/ban_search.py` & `hikari_core-0.9.0.5/hikari_core/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/game/box_check.py` & `hikari_core-0.9.0.5/hikari_core/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/game/help.py` & `hikari_core-0.9.0.5/hikari_core/game/help.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/game/roll.py` & `hikari_core-0.9.0.5/hikari_core/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/game/sx.py` & `hikari_core-0.9.0.5/hikari_core/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0.5/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0.5/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0.5/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0.5/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0.5/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0.5/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0.5/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/model.py` & `hikari_core-0.9.0.5/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0.5/hikari_core/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_bind.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_real_game.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_real_game.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                             elif battles >= 2:
                                 msg = f'{nick_name}刚刚完成了{battles}场对局\n胜{win}负{loss}平{battles-win-loss}\n使用{ship_name_cn}\n总伤害{damage}'
                             else:
                                 continue
                             send_param = {'group_id': _group_id, 'msg': msg, 'type': 'text'}
                             send_list.append(send_param.copy())
         if not send_list:
-            return hikari.success('没有新的监控战绩')
+            return hikari.failed('没有新的监控战绩')
         return hikari.success(send_list)
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
         return hikari.error('请求超时了，请过会儿再尝试哦~')
     except PoolTimeout:
         await recreate_client_yuyuko()
         return hikari.error('连接池异常，请尝试重新查询~')
```

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_ship_info.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_ship_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_ship_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/moudle/wws_shiprank.py` & `hikari_core-0.9.0.5/hikari_core/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/bind-list.html` & `hikari_core-0.9.0.5/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0.5/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0.5/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0.5/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/hikari_core/utils.py` & `hikari_core-0.9.0.5/hikari_core/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/LICENSE` & `hikari_core-0.9.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0.4/pyproject.toml` & `hikari_core-0.9.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.9.0.4"
+version = "0.9.0.5"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
```

### Comparing `hikari_core-0.9.0.4/setup.py` & `hikari_core-0.9.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.9.0.4',
+    'version': '0.9.0.5',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-0.9.0.4/PKG-INFO` & `hikari_core-0.9.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.9.0.4
+Version: 0.9.0.5
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

