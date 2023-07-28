# Comparing `tmp/nonebot_plugin_eventmonitor-0.1.9.tar.gz` & `tmp/nonebot_plugin_eventmonitor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.9.tar", last modified: Sun Jul 23 15:01:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_eventmonitor-0.2.0.tar", last modified: Fri Jul 28 07:23:39 2023, max compression
```

## Comparing `nonebot_plugin_eventmonitor-0.1.9.tar` & `nonebot_plugin_eventmonitor-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:13.150708 nonebot_plugin_eventmonitor-0.1.9/
--rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     1601 2023-07-23 15:01:13.150708 nonebot_plugin_eventmonitor-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-07-23 14:56:54.000000 nonebot_plugin_eventmonitor-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:13.119050 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/
--rw-rw-rw-   0        0        0     8271 2023-07-23 14:55:01.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-23 12:12:06.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/admin.py
--rw-rw-rw-   0        0        0     1621 2023-07-23 14:34:04.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/honour.py
--rw-rw-rw-   0        0        0     2166 2023-07-23 12:34:54.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/stamp.py
--rw-rw-rw-   0        0        0     7116 2023-07-23 14:55:08.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 15:01:13.150708 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/
--rw-rw-rw-   0        0        0     1601 2023-07-23 15:01:12.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-23 15:01:13.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 15:01:12.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-23 15:01:12.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-23 15:01:12.000000 nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 15:01:13.150708 nonebot_plugin_eventmonitor-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-07-23 14:57:06.000000 nonebot_plugin_eventmonitor-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:23:39.800382 nonebot_plugin_eventmonitor-0.2.0/
+-rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5960 2023-07-28 07:23:39.800382 nonebot_plugin_eventmonitor-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5329 2023-07-26 09:56:03.000000 nonebot_plugin_eventmonitor-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 07:23:39.771940 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/
+-rw-rw-rw-   0        0        0     7727 2023-07-28 07:11:30.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/__init__.py
+-rw-rw-rw-   0        0        0     2790 2023-07-27 14:41:02.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/admin.py
+-rw-rw-rw-   0        0        0     1731 2023-07-27 08:46:41.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/honour.py
+-rw-rw-rw-   0        0        0     2166 2023-07-23 12:34:54.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/stamp.py
+-rw-rw-rw-   0        0        0     7482 2023-07-28 07:10:43.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 07:23:39.798382 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/
+-rw-rw-rw-   0        0        0     5960 2023-07-28 07:23:39.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-28 07:23:39.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 07:23:39.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-28 07:23:39.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-28 07:23:39.000000 nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 07:23:39.800382 nonebot_plugin_eventmonitor-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-07-28 07:18:19.000000 nonebot_plugin_eventmonitor-0.2.0/setup.py
```

### Comparing `nonebot_plugin_eventmonitor-0.1.9/LICENSE` & `nonebot_plugin_eventmonitor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/__init__.py` & `nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import nonebot
+
 from nonebot.rule import Rule
 from nonebot.matcher import Matcher
 from nonebot.plugin import on_notice, on_command
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11.permission import GROUP_OWNER, GROUP_ADMIN
 from nonebot.adapters.onebot.v11 import (
     Bot, Event, Message,
@@ -42,39 +43,71 @@
 async def _is_admin_change(event: Event) -> bool:
     return isinstance(event, GroupAdminNoticeEvent)
 # 红包运气王
 async def _is_red_packet(event: Event) -> bool:
     return isinstance(event, LuckyKingNotifyEvent)
 
 # 戳一戳
-chuo = on_notice(Rule(_is_poke), priority=50, block=True)
+chuo = on_notice(
+    Rule(_is_poke),
+    priority=50,
+    block=True
+)
 # 群荣誉
-qrongyu = on_notice(Rule(_is_rongyu), priority=50, block=True)
+qrongyu = on_notice(
+    Rule(_is_rongyu),
+    priority=50,
+    block=True
+)
 # 群文件
-files = on_notice(Rule(_is_checker), priority=50, block=True)
+files = on_notice(
+    Rule(_is_checker),
+    priority=50,
+    block=True
+)
 # 群员减少
-del_user = on_notice(Rule(_is_del_user), priority=50, block=True)
+del_user = on_notice(
+    Rule(_is_del_user),
+    priority=50,
+    block=True
+)
 # 群员增加
-add_user = on_notice(Rule(_is_add_user), priority=50, block=True)
+add_user = on_notice(
+    Rule(_is_add_user),
+    priority=50,
+    block=True
+)
 # 群管理
-group_admin = on_notice(Rule(_is_admin_change), priority=50, block=True)
+group_admin = on_notice(
+    Rule(_is_admin_change),
+    priority=50,
+    block=True
+)
 # 红包
-red_packet = on_notice(Rule(_is_red_packet), priority=50, block=True)
+red_packet = on_notice(
+    Rule(_is_red_packet),
+    priority=50,
+    block=True
+)
 # 功能开关
-switch_command = on_command("开启", aliases={"关闭"}, 
-                        permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
-                        priority=10,
-                        block=False
-                    )
+switch_command = on_command(
+    "开启",
+    aliases={"关闭"}, 
+    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    priority=10,
+    block=True
+)
 #功能状态
-state = on_command("event配置", aliases={"event状态"},
-                        permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
-                        priority=10,
-                        block=False
-                    )
+state = on_command(
+    "event配置",
+    aliases={"event状态"},
+    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+    priority=10,
+    block=True
+)
 
 #初始化配置配置文件
 @driver.on_bot_connect
 async def _():
     await init(g_temp)
     await config_check()
 
@@ -93,93 +126,88 @@
     if (
         cd > chuo_cd
         or event.get_user_id() in nonebot.get_driver().config.superusers
     ):# 记录cd                                                                                   
         chuo_CD_dir.update({uid: event.time})
     rely_msg = await chuo_send_msg()
     await chuo.finish(message=Message(rely_msg))
+
 #群荣誉变化
 @qrongyu.handle()                                                                       
 async def send_rongyu(event: HonorNotifyEvent, bot: Bot):
     if not (await check_honor(g_temp, str(event.group_id))):
-        await qrongyu.finish(notAllow, at_sender=True)
+        return
     bot_qq = int(bot.self_id)
     rely_msg = await monitor_rongyu(event.honor_type, event.user_id, bot_qq)
     await qrongyu.finish(message=Message(rely_msg))
+
 #上传群文件
 @files.handle()                                                                         
 async def handle_first_receive(event: GroupUploadNoticeEvent):
     if not (await check_file(g_temp, str(event.group_id))):
-        await files.finish(notAllow, at_sender=True)
+        return
     rely = MessageSegment.at(event.user_id) + '\n' + \
            MessageSegment.image(f'https://q4.qlogo.cn/headimg_dl?dst_uin={event.user_id}&spec=640') + \
            '\n 上传了新文件，感谢你一直为群里做贡献喵~' + MessageSegment.face(175)
     await files.finish(message=rely)
+
 #退群事件
 @del_user.handle()
 async def user_bye(event: GroupDecreaseNoticeEvent):
     if not (await check_del_user(g_temp, str(event.group_id))):
-        await del_user.finish(notAllow, at_sender=True)
+        return
     rely_msg = await  del_user_bye(event.time, event.user_id)
     await del_user.finish(message=Message(rely_msg))
+
 #入群事件
 @add_user.handle()
 async def user_welcome(event: GroupIncreaseNoticeEvent, bot: Bot):
+    await config_check()
     if not (await check_add_user(g_temp, str(event.group_id))):
-        await add_user.finish(notAllow, at_sender=True)
+        return
     bot_qq = int(bot.self_id)
     rely_msg = await  add_user_wecome(event.time, event.user_id, bot_qq)
     await add_user.finish(message=Message(rely_msg))
+
 #管理员变动
 @group_admin.handle()
 async def admin_chance(event: GroupAdminNoticeEvent, bot: Bot):
     if not (await check_admin(g_temp, str(event.group_id))):
-        await group_admin.finish(notAllow, at_sender=True)
+        return
     bot_qq = int(bot.self_id)
     rely_msg = await admin_changer(event.sub_type, event.user_id, bot_qq)
     await group_admin.finish(message=Message(rely_msg))
+    
 #红包运气王
 @red_packet.handle()
 async def hongbao(event: LuckyKingNotifyEvent):
     if not (await check_red_package(g_temp, str(event.group_id))):
-        await red_packet.finish(notAllow, at_sender=True)
+        return
     rely_msg = MessageSegment.at(event.user_id) + "\n" + "本次红包运气王为：" + MessageSegment.at(event.target_id)
     await red_packet.finish(message=rely_msg)
 
-
-def get_command_type(command: str) -> str:
-    """根据指令内容获取开关类型"""
-    return next(
-        (
-            key
-            for key, keywords in path.items()
-            if any(keyword in command for keyword in keywords)
-        ),
-        "",
-    )
-
 @switch_command.handle()
 async def switch(event: GroupMessageEvent, matcher: Matcher):
     # 获取开关指令的参数，即用户输入的指令内容
     command = str(event.get_message()).strip()
     # 获取群组ID
     gid = str(event.group_id)
     # 判断指令是否包含"开启"或"关闭"关键字
     if "开启" in command or "开始" in command:
         if key := get_command_type(command):
             g_temp[gid][key] = True
             write_group_data(g_temp)
             name = get_function_name(key)
-            await switch_command.finish(f"{name}功能已开启喵")
+            await matcher.finish(f"{name}功能已开启喵")
     elif "禁止" in command or "关闭" in command:
         if key := get_command_type(command):
             g_temp[gid][key] = False
             write_group_data(g_temp)
             name = get_function_name(key)
-            await switch_command.finish(f"{name}功能已禁用喵")
+            await matcher.finish(f"{name}功能已禁用喵")
 
 @state.handle()
 async def event_state(event:GroupMessageEvent, matcher: Matcher):
     gid = str(event.group_id)
     with open(address, "r", encoding="utf-8") as f:
         group_status = json.load(f)
     if gid not in group_status:
@@ -201,11 +229,11 @@
         description="监控群事件的插件，支持戳一戳，成员变动，群荣誉变化等提示的插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Reversedeer/nonebot_plugin_eventmonitor",
         supported_adapters={"onebot.v11"},
         extra={
             "author": "Reversedeer",
-            "version": "0.1.8",
+            "version": "0.2.0",
             "priority": 50,
         },
     )
```

### Comparing `nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/admin.py` & `nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     global del_user_msg
     del_time = datetime.fromtimestamp(add_time)
     
     # 检查用户ID是否在超级用户列表superusers中
     if user_id in superusers:
         # 如果是超级用户，生成特定的离开消息
         del_user_msg = f"⌈{del_time}⌋\n@{user_id}恭送主人离开喵~"
-        print(superusers)
     else:
         # 如果不是超级用户，生成通用的离开消息，包含用户的QQ号和头像图片
         del_user_msg = f"✈️ 成员变动 ✈️ \n时间: ⌈{del_time}⌋\nQQ号为：{user_id}的小可爱退群喵~" \
                        f"[CQ:image,file=https://q4.qlogo.cn/headimg_dl?dst_uin={user_id}&spec=640]"
                        
         return del_user_msg
 
@@ -54,10 +53,9 @@
     elif user_id in superusers:
         # 如果是超级用户加入群组，生成特定的欢迎消息，包含用户ID和CQ表情
         add_user_msg = f"✨ 成员变动 ✨\n@{user_id}欢迎主人进群喵~[CQ:face,id=175]"
     else:
         # 如果是普通用户加入群组，生成通用的欢迎消息，包含用户ID、加入时间和用户头像图片的链接
         add_user_msg = f"✨ 成员变动 ✨\n欢迎@{user_id}的加入喵~\n加入时间：⌈{add_time}⌋，请在群内积极发言喵~" \
                        f"[CQ:image,file=https://q4.qlogo.cn/headimg_dl?dst_uin={user_id}&spec=640]"
-    
     return add_user_msg
```

### Comparing `nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/honour.py` & `nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/honour.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 async def monitor_rongyu(honor_type, user_id, bot_qq):
     rely = ""  
     # 根据honor_type选择不同的消息
     if honor_type == "emotion":
         # 如果用户ID等于机器人的QQ号，不作任何操作
         if user_id == bot_qq:
-            pass
+            rely = "你们又不行了，本喵喜提快乐源泉🤣~"
         # 如果用户ID在superusers列表中，返回特定消息
         elif user_id in superusers:
             rely = f"@{user_id}恭喜主人荣获快乐源泉🤣标识喵~"
         # 否则，返回通用消息
         else:
             rely = f"恭喜@{user_id}荣获快乐源泉🤣标识喵~"
             
     elif honor_type == "performer":
         # 如果用户ID等于机器人的QQ号，不作任何操作
         if user_id == bot_qq:
-            pass
+            rely = "你们又不行了，本喵喜提群聊之火🔥~"
         # 如果用户ID在superusers列表中，返回特定消息
         elif user_id in superusers:
             rely = f"@{user_id}恭喜主人荣获群聊之火🔥标识喵~"
         # 否则，返回通用消息
         else:
             rely = f"恭喜@{user_id}荣获群聊之火🔥标识喵~"
```

### Comparing `nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/stamp.py` & `nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/stamp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.9/nonebot_plugin_eventmonitor/utils.py` & `nonebot_plugin_eventmonitor-0.2.0/nonebot_plugin_eventmonitor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 import os
 import nonebot
 import json
 from pathlib import Path
 from typing import Optional
 
 g_temp = {}
+chuo_CD_dir = {}
+
 config_path = Path() / 'data/eventmonitor'
 address = config_path / 'config.json'
 
+driver = nonebot.get_driver()
+#从 配置文件中获取SUPERUSER, NICKNAME
+config = nonebot.get_driver().config
+superusers = {int(uid) for uid in config.superusers}
+nickname = next(iter(config.nickname))
+#戳一戳cd,感觉很鸡肋，自行调整
+
+notAllow = "功能未开启"
+
+
 async def init(g_temp):
     """
     初始化配置文件
     :return:
     """   
-    # 如果数据文件路径不存在，则创建目录，并初始化群组数据为空字典，并写入对应的文件
+    # 如果数据文件路径不存在，则创建目录
     if not os.path.exists(config_path):  
         os.makedirs(config_path)  
     if os.path.exists(address):
         # 如果数据文件路径存在，尝试读取数据文件（config.json）
         with open(address, "r", encoding="utf-8") as f:
             g_temp.update(json.load(f))
     else:
         # 如果群数据文件不存在，则初始化g_temp为空字典，并写入对应的文件
         bot = nonebot.get_bot()
-        group_list = (await bot.get_group_list())
+        group_list = await bot.get_group_list()
         #从group_list中遍历每个群组
         for group in group_list:
             # 为每个群组创建一个临时字典temp，用于存储群组的配置信息
             temp = {}
             for g_name in path:
                 # 将群组的每个配置项设置为默认值True
                 temp[g_name] = True
@@ -39,20 +51,22 @@
             # 将临时字典temp作为值，群组ID作为键，添加到g_temp字典中
             g_temp[gid] = temp
             # 将更新后的g_temp字典写入群组数据
             write_group_data(g_temp)
 
 
 async def config_check():
+    global g_temp
     # 获取机器人实例
     bot = nonebot.get_bot()
     # 获取所有群组的列表
-    group_list = (await bot.get_group_list())  
+    group_list = await bot.get_group_list()
     # 加载配置文件，得到一个包含配置信息的字典
-    config_dict = json_load(address)  
+    with open(address, "r", encoding="utf-8") as f:
+        config_dict = json.load(f)  
     # 遍历所有群组
     for group in group_list:
         gid = str(group['group_id']) 
         # 如果配置字典中没有该群组的信息，将其添加到配置字典中
         if not config_dict.get(gid):
             config_dict[gid] = {}
             # 遍历配置文件路径中的所有配置项，并初始化为默认值
@@ -66,15 +80,15 @@
             other_group = config_dict[gid]
             for group_name in path:
                 if other_group.get(group_name) is None:
                     other_group[gid][group_name] = True
                     # 特殊情况下（group_name为'red_package'），将该配置项设为False
                     if group_name in ['red_package']:
                         other_group[gid][group_name] = False
-   
+    g_temp.update(config_dict)
     # 将更新后的配置字典上传到配置文件中
     json_upload(address, config_dict)
 
 
 def json_load(path) -> Optional[dict]:
     """
     加载json文件
@@ -108,66 +122,72 @@
     if gid in g_temp and not g_temp[gid]["chuo"]:
         return False
     return g_temp[gid]["chuo"]
 
 #检查群荣誉是否允许 
 async def check_honor(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["honor"]:
+        print(g_temp)
         return False
     return g_temp[gid]["honor"]
 
 #检查群文件是否允许 
 async def check_file(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["files"]:
         return False
     return g_temp[gid]["files"]
 
 #检查群成员减少是否允许 
 async def check_del_user(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["del_user"]:
         return False
+    print(g_temp)
     return g_temp[gid]["del_user"]
 
 #检查群成员增加是否允许
 async def check_add_user(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["add_user"]:
         return False
+    print(g_temp)
     return g_temp[gid]["add_user"]
+    
 
 #检查管理员是否允许
 async def check_admin(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["admin"]:
         return False
     return g_temp[gid]["admin"]
 
 #检查运气王是否允许
 async def check_red_package(g_temp, gid: str) -> bool:
     if gid in g_temp and not g_temp[gid]["red_package"]:
         return False
     return g_temp[gid]["red_package"]
 
 #根据关键词获取对应功能名称
-async def get_function_name(key: str) -> str:
+def get_function_name(key: str) -> str:
     return path[key][0]
 
+#根据指令内容获取开关类型
+def get_command_type(command: str) -> str:
+    return next(
+        (
+            key
+            for key, keywords in path.items()
+            if any(keyword in command for keyword in keywords)
+        ),
+        "",
+    )
+
 #戳一戳cd默认值    
 try:
     chuo_cd = nonebot.get_driver().config.chuo_cd
 except Exception:
     chuo_cd = 0   
  
-#从 配置文件中获取SUPERUSER, NICKNAME
-config = nonebot.get_driver().config
-superusers = {int(uid) for uid in config.superusers}
-nickname = next(iter(config.nickname))
-#戳一戳cd,感觉很鸡肋，自行调整
-chuo_CD_dir = {}
-driver = nonebot.get_driver()
-notAllow = "功能未开启"
-
 
 path = {
     'chuo': ['戳一戳'],
     'honor': ['群荣誉检测'],
     'files': ['群文件检测'],
     'del_user': ['群成员减少检测'],
     'add_user': ['群成员增加检测'],
```

### Comparing `nonebot_plugin_eventmonitor-0.1.9/setup.py` & `nonebot_plugin_eventmonitor-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_eventmonitor",
-    version="0.1.9",
+    version="0.2.0",
     author="schwarzwald",
     description="监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Reversedeer/nonebot_plugin_eventmonitor",
     project_urls={
         "Bug Tracker": "https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues",
```

