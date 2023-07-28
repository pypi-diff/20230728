# Comparing `tmp/nonebot_plugin_blocker-0.3.2.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.2.tar", last modified: Thu Jul 27 16:37:11 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.3.tar", last modified: Fri Jul 28 18:33:41 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.2.tar` & `nonebot_plugin_blocker-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/LICENSE
--rw-r--r--   0        0        0     2447 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/README.md
--rw-r--r--   0        0        0      381 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3624 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     2544 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2370 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     2998 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     5056 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-27 16:36:55.422758 nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-07-27 16:37:11.966692 nonebot_plugin_blocker-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2538 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/README.md
+-rw-r--r--   0        0        0      381 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3285 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     3994 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2383 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     2780 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6055 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-07-28 18:33:41.490188 nonebot_plugin_blocker-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.2/LICENSE` & `nonebot_plugin_blocker-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.2/README.md` & `nonebot_plugin_blocker-0.3.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -72,9 +72,10 @@
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
 ### 如果你在WebUI设置了指令那么指令将会是你设置的文本
 
 ## TODO && 碎碎念
 
- * 准备接着改改配置项
- * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
+ * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
+ * 什么时候用上PydanticV2啊我要用RootModel啊（
+ * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -17,9 +17,11 @@
 æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
 ### å¦æä½ å¨WebUIè®¾ç½®äºæä»¤é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®çææ¬ ##
-TODO && ç¢ç¢å¿µ * åå¤æ¥çæ¹æ¹éç½®é¡¹ *
-ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
+TODO && ç¢ç¢å¿µ *
+åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
+* ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
+ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

### Comparing `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,82 +7,69 @@
 
 from nonebot.permission import SUPERUSER
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.message import run_preprocessor
 
 import re
-from .config import BlockerList, get_reply_config
+from .config import BlockerList, get_reply_config, upgrade_config, reply_config_raw
 from . import web
 
 blockerlist: BlockerList
     
 driver.server_app.mount("/blocker-webui", web.app, name="blocker-webui")
-logger.info("[Blocker]WebUI is now listening on "
-            f"http://{driver.config.host}:{driver.config.port}/blocker-webui/"
-)
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
+    upgrade_config()
+    logger.info("[Blocker]WebUI is now listening on "
+                f"http://{driver.config.host}:{driver.config.port}/blocker-webui/")
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
     
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
     if (event.get_plaintext().find('qq') != -1 and not event.is_tome()) or event.user_id == event.self_id:
         return False
     try:
         reply_config = get_reply_config().get(str(event.self_id))
-        if re.match(reply_config.get("command_on")+'$', event.get_plaintext()) is not None:
-            state['blocker_state'] = True
-            return True
-        elif re.match(reply_config.get("command_off")+'$', event.get_plaintext()) is not None:
-            state['blocker_state'] = False
-            return True
+        if re.match(reply_config.get("command_on")+'$', event.get_plaintext()):
+            state['blocker_state'] = "reply_on"
+        elif re.match(reply_config.get("command_off")+'$', event.get_plaintext()):
+            state['blocker_state'] = "reply_off"
     except (AttributeError,KeyError,TypeError):
-        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', event.get_plaintext()) is not None:
-            state['blocker_state'] = True
-            return True
-        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', event.get_plaintext()) is not None:
-            state['blocker_state'] = False
-            return True
-    return False
+        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', event.get_plaintext()):
+            state['blocker_state'] = "reply_on"
+        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', event.get_plaintext()):
+            state['blocker_state'] = "reply_off"
+    return True if 'blocker_state' in state else False
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id, event.self_id) and re.match('^nonebot_plugin_blocker$',matcher.plugin_name) is None:
+    if blockerlist.check_blocker(event.group_id, str(event.self_id)) and re.match('^nonebot_plugin_blocker$',matcher.plugin_name) is None:
         logger.info('[Blocker]Your Message is Blocked By Blocker.')
         matcher.handlers = None
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher, event: GroupMessageEvent, state: T_State):
-    reply_config = get_reply_config().get(str(event.self_id))
-    if state['blocker_state']:
-        blockerlist.del_blocker(event.group_id, event.self_id)
+    try:
+        reply_config = get_reply_config().get(str(event.self_id)).get(state['blocker_state'])
+    except AttributeError:
+        reply_config = reply_config_raw.get(state['blocker_state'])
+    msg_type = reply_config.get("type")
+    msg_data = reply_config.get("data")
+    if state['blocker_state'] == "reply_on":
+        blockerlist.del_blocker(event.group_id, str(event.self_id))
         logger.info('[Blocker]Delete Blocker Successful.')
-        try:
-            msg_type = reply_config.get("reply_on_type")
-            msg_data = reply_config.get("reply_on_content")
-            if msg_data == "":
-                raise AttributeError
-        except AttributeError:
-            await matcher.finish('在本群开启')
     else:
-        blockerlist.add_blocker(event.group_id, event.self_id)
+        blockerlist.add_blocker(event.group_id, str(event.self_id))
         logger.info('[Blocker]Add Blocker Successful.')
-        try:
-            msg_type = reply_config.get("reply_off_type")
-            msg_data = reply_config.get("reply_off_content")
-            if msg_data == "":
-                raise AttributeError
-        except AttributeError:
-            await matcher.finish('在本群关闭')
     if msg_type == "text":
         await matcher.finish(msg_data)
     else:
         await matcher.finish(MessageSegment(type=msg_type, data={"file":msg_data}))
```

### Comparing `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from fastapi import FastAPI, HTTPException, Depends
 from fastapi.security import HTTPBasicCredentials, HTTPBasic
-from secrets import compare_digest
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
+from secrets import compare_digest
 from ..config import(
     STATIC_FILE_PATH,
     MAIN_PAGE_PATH,
-    ReplyConfigModel,
+    ConfigModel,
     get_reply_config,
     save_reply_config,
     config
 )
 
 async def security_dependency(
     credentials: HTTPBasicCredentials = Depends(HTTPBasic()),
@@ -32,26 +32,26 @@
     description="Blocker plugin`s webui",
     dependencies=(
         [Depends(security_dependency)] if config.WEBUI_USERNAME and config.WEBUI_PASSWORD else []
     ),
     version=("nonebot-plugin-blocker")
 )
 
-app.mount("/static", StaticFiles(directory=STATIC_FILE_PATH, html=True), name="frontend")
+app.mount("/static", StaticFiles(directory=STATIC_FILE_PATH, html=False), name="frontend")
 
 @app.get("/",response_class=HTMLResponse)
 async def show_webpage():
     return HTMLResponse(content=MAIN_PAGE_PATH.read_text(encoding="UTF-8"), status_code=200)
 
 @app.post("/submit")
-async def __set_config__(form: ReplyConfigModel):
+async def __set_config__(form: ConfigModel):
+    save_dict = get_reply_config()
+    save_dict.update(form.dict().get("__root__"))
+    save_reply_config(ConfigModel.parse_obj(save_dict))
     try:
-        config_list = get_reply_config()
-        config_list.update(form.dict().get("__root__"))
-        save_reply_config(config_list)
         return {"result":"success"}
     except:
         return {"result":"failed"}
         
 @app.get("/query_reply_list")
 async def __get_reply_list__():
     try:
@@ -65,13 +65,13 @@
         return {"result":"success","data":get_reply_config().get(uin,"none")}
     except:
         return {"result":"failed"}
     
 @app.get("/delete")
 async def __delete_reply_config__(uin: str):
     try:
-        config_list = get_reply_config()
-        config_list.pop(uin)
-        save_reply_config(config_list)
+        save_dict = get_reply_config()
+        save_dict.pop(uin)
+        save_reply_config(ConfigModel.parse_obj(save_dict))
         return {"result":"success"}
     except:
         return {"result":"failed"}
```

### Comparing `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -8,46 +8,66 @@
                 $(".active").removeClass("active");
                 $(this).addClass("active")
                 $.get("query_reply", {
                     uin: $(this).text()
                 }, function(result) {
                     if (result.result == "success") {
                         $.each(result.data, function(key, val) {
+                            if (typeof(val) == "object") {
+                                $.each(val, function(val_key, val_val) {
+                                    $("[name=" + key + "]").find("[name=" + val_key + "]").val(val_val)
+                                });
+                            }
                             $("[name=" + key + "]").val(val)
                         });
                     }
                 });
             });
         }
     });
     $(".submit").click(function() {
-        var data = {}
-        $(".blocker_submit_form").serializeArray().map(function(val, key) {
-            data[val.name] = val.value;
+        var raw_data = {}
+        var reply_on = {}
+        var reply_off = {}
+        $(".command").serializeArray().map(function(val, key) {
+            raw_data[val.name] = val.value;
+        });
+        $(".reply_on").serializeArray().map(function(val, key) {
+            reply_on[val.name] = val.value;
         });
-        var newdata = {}
+        $(".reply_off").serializeArray().map(function(val, key) {
+            reply_off[val.name] = val.value;
+        });
+        raw_data["reply_on"] = reply_on
+        raw_data["reply_off"] = reply_off
+        var data = {}
         if (String($(".active").text()) == "") {
             alert("您还没有选择或添加账号");
         } else {
-            newdata[String($(".active").text())] = data
-            console.log(newdata)
+            data[String($(".active").text())] = raw_data
+            console.log(data)
             $.ajax({
                 contentType: "application/json",
-                data: JSON.stringify(newdata),
+                data: JSON.stringify(data),
                 url: "submit",
                 type: "POST",
                 success: function(result) {
                     if (result.result == "success") {
                         alert("修改/增加配置成功")
                         if ($(".active").hasClass("newadd")) {
                             $(".active").removeClass("newadd").bind("click", function() {
                                 $.get("query_reply", {
                                     uin: $(this).text()
                                 }, function(result) {
                                     if (result.result == "success") {
+                                        if (typeof(val) == "object") {
+                                            $.each(val, function(val_key, val_val) {
+                                                $("[name=" + key + "]").find("[name=" + val_key + "]").val(val_val)
+                                            });
+                                        }
                                         $.each(result.data, function(key, val) {
                                             $("[name=" + key + "]").val(val)
                                         });
                                     }
                                 });
                             });
                         }
```

### Comparing `nonebot_plugin_blocker-0.3.2/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.2/pyproject.toml` & `nonebot_plugin_blocker-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.2"
+version = "0.3.3"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.2/PKG-INFO` & `nonebot_plugin_blocker-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.2
+Version: 0.3.3
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
@@ -94,9 +94,10 @@
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
 ### 如果你在WebUI设置了指令那么指令将会是你设置的文本
 
 ## TODO && 碎碎念
 
- * 准备接着改改配置项
- * 我测，这WebUI写的我感觉我像个乡下来写代码的，用的30年前的老教材学的东西在写属于是
+ * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
+ * 什么时候用上PydanticV2啊我要用RootModel啊（
+ * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.3 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -38,9 +38,11 @@
 æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
 ### å¦æä½ å¨WebUIè®¾ç½®äºæä»¤é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®çææ¬ ##
-TODO && ç¢ç¢å¿µ * åå¤æ¥çæ¹æ¹éç½®é¡¹ *
-ææµï¼è¿WebUIåçææè§æåä¸ªä¹¡ä¸æ¥åä»£ç çï¼ç¨ç30å¹´åçèææå­¦çä¸è¥¿å¨åå±äºæ¯
+TODO && ç¢ç¢å¿µ *
+åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
+* ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
+ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

