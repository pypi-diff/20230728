# Comparing `tmp/usepy_plugin_notify-0.2.4.tar.gz` & `tmp/usepy_plugin_notify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy_plugin_notify-0.2.4.tar", max compression
+gzip compressed data, was "usepy_plugin_notify-0.3.0.tar", max compression
```

## Comparing `usepy_plugin_notify-0.2.4.tar` & `usepy_plugin_notify-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1053 2023-03-10 07:25:22.644908 usepy_plugin_notify-0.2.4/README.md
--rw-r--r--   0        0        0      440 2023-03-10 14:11:23.318689 usepy_plugin_notify-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       53 2023-03-09 07:40:51.827282 usepy_plugin_notify-0.2.4/src/usepy_notify/__init__.py
--rw-r--r--   0        0        0      219 2023-03-09 05:51:26.637490 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/__init__.py
--rw-r--r--   0        0        0      508 2023-03-09 07:42:41.912831 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/bark.py
--rw-r--r--   0        0        0      271 2023-03-09 05:36:00.163670 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/base.py
--rw-r--r--   0        0        0      597 2023-03-09 05:38:51.414074 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/chanify.py
--rw-r--r--   0        0        0      897 2023-03-09 06:16:48.548893 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/ding.py
--rw-r--r--   0        0        0     1027 2023-03-09 06:26:41.986675 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/email.py
--rw-r--r--   0        0        0      578 2023-03-09 05:40:59.163466 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/pushdeer.py
--rw-r--r--   0        0        0      688 2023-03-09 05:42:38.745593 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/pushover.py
--rw-r--r--   0        0        0      675 2023-03-09 05:43:19.819767 usepy_plugin_notify-0.2.4/src/usepy_notify/channels/wechat.py
--rw-r--r--   0        0        0      534 2023-03-09 06:00:12.144324 usepy_plugin_notify-0.2.4/src/usepy_notify/notification.py
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 usepy_plugin_notify-0.2.4/setup.py
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 usepy_plugin_notify-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1170 2023-07-28 15:30:43.906916 usepy_plugin_notify-0.3.0/README.md
+-rw-r--r--   0        0        0      478 2023-07-28 15:38:27.981598 usepy_plugin_notify-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-28 14:16:03.475094 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-28 13:43:34.603009 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/__init__.py
+-rw-r--r--   0        0        0      962 2023-07-28 15:29:07.121713 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/bark.py
+-rw-r--r--   0        0        0      367 2023-07-28 14:34:20.033887 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/base.py
+-rw-r--r--   0        0        0     1066 2023-07-28 15:29:07.123638 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/chanify.py
+-rw-r--r--   0        0        0     1343 2023-07-28 15:29:07.127631 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/ding.py
+-rw-r--r--   0        0        0     1690 2023-07-28 15:14:07.368445 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/email.py
+-rw-r--r--   0        0        0     1069 2023-07-28 15:29:07.132002 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/pushdeer.py
+-rw-r--r--   0        0        0     1166 2023-07-28 15:29:07.125499 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/pushover.py
+-rw-r--r--   0        0        0     1137 2023-07-28 15:29:07.130064 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/wechat.py
+-rw-r--r--   0        0        0     1201 2023-07-28 15:26:18.238249 usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/notification.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 usepy_plugin_notify-0.3.0/PKG-INFO
```

### Comparing `usepy_plugin_notify-0.2.4/README.md` & `usepy_plugin_notify-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### 一个简单可扩展的消息通知库
+### 一个简单可扩展的异步消息通知库
 
 <a href="https://pypi.org/project/ml-simple-notify" target="_blank">
     <img src="https://img.shields.io/pypi/v/ml-simple-notify.svg" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/ml-simple-notify" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/ml-simple-notify.svg" alt="Supported Python versions">
@@ -11,21 +11,21 @@
 #### 安装
 
 > pip install usepy-plugin-notify
 
 #### 使用
 
 ```python
-from notify import useNotify, channels
+from usepy.plugin import useNotify, useNotifyChannel
 
 notify = useNotify()
 notify.add(
     # 添加多个通知渠道
-    channels.Bark({"token": "xxxxxx"}),
-    channels.Ding({
+    useNotifyChannel.Bark({"token": "xxxxxx"}),
+    useNotifyChannel.Ding({
         "token": "xxxxx",
         "at_all": True
     })
 )
 
 notify.publish(title="消息标题", content="消息正文")
 
@@ -40,16 +40,19 @@
 - Chanify
 - Pushdeer
 - Pushover
 
 #### 自己开发消息通知
 
 ```python
-from notify.channels import BaseChannel
+from usepy.plugin import useNotifyChannel
 
 
-class Custom(BaseChannel):
+class Custom(useNotifyChannel.BaseChannel):
     """自定义消息通知"""
 
     def send(self, *args, **kwargs):
         ...
+
+    async def send_async(self, *args, **kwargs):
+        ...
 ```
```

### Comparing `usepy_plugin_notify-0.2.4/src/usepy_notify/channels/email.py` & `usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/email.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
+import asyncio
 import logging
 import smtplib
 from email.header import Header
 from email.mime.text import MIMEText
+from functools import partial
 
 from .base import BaseChannel
 
 logger = logging.getLogger(__name__)
 
 
 class Email(BaseChannel):
@@ -14,18 +16,35 @@
 
     def __init__(self, config):
         super().__init__(config)
         self.smtp = smtplib.SMTP_SSL(self.config.server, self.config.port)
         self.smtp.connect(self.config.server, self.config.port)
         self.smtp.login(self.config.username, self.config.password)
 
-    def send(self, content, title=None):
-        if not self.config.receivers:
-            logger.error('请先设置接收邮箱<receivers>')
-            return
+    @staticmethod
+    def build_message(content, title=None):
         message = MIMEText(content, 'html', 'utf-8')
         message['From'] = Header('notify', 'utf-8')
         subject = title or '消息提醒'
         message['Subject'] = Header(subject, 'utf-8')
+        return message.as_string()
+
+    def send(self, content, title=None):
+        if not self.config.receivers:
+            logger.error('请先设置接收邮箱<receivers>')
+            return
+        message = self.build_message(content, title)
+
+        self.smtp.sendmail(self.config.sender, self.config.receivers, message)
+        logger.debug('邮件通知推送成功')
+
+    async def send_async(self, content, title=None):
+        if not self.config.receivers:
+            logger.error('请先设置接收邮箱<receivers>')
+            return
+        message = self.build_message(content, title)
 
-        self.smtp.sendmail(self.config.sender, self.config.receivers, message.as_string())
+        loop = asyncio.get_event_loop()
+        sendmail_func = partial(self.smtp.sendmail, self.config.sender, self.config.receivers, message)
+        await loop.run_in_executor(None, sendmail_func)
         logger.debug('邮件通知推送成功')
+
```

### Comparing `usepy_plugin_notify-0.2.4/src/usepy_notify/channels/pushover.py` & `usepy_plugin_notify-0.3.0/src/usepy_plugin_notify/channels/pushover.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,19 +7,34 @@
 
 logger = logging.getLogger(__name__)
 
 
 class PushOver(BaseChannel):
     """pushover app 消息通知"""
 
-    def send(self, content, title=None):
-        api_url = 'https://api.pushover.net/1/messages.json'
-        api_body = {
+    @property
+    def api_url(self):
+        return 'https://api.pushover.net/1/messages.json'
+
+    @property
+    def headers(self):
+        return {'Content-Type': 'application/x-www-form-urlencoded'}
+
+    def build_api_body(self, content, title=None):
+        return {
             'token': self.config.token,
             'user': self.config.user,
             'title': title,
             'message': content,
         }
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+
+    def send(self, content, title=None):
+        api_body = self.build_api_body(content, title)
         with httpx.Client() as client:
-            client.post(api_url, data=api_body, headers=headers)
-        logger.debug("pushover消息推送成功")
+            client.post(self.api_url, data=api_body, headers=self.headers)
+        logger.debug("`pushover` send successfully")
+
+    async def send_async(self, content, title=None):
+        api_body = self.build_api_body(content, title)
+        async with httpx.AsyncClient() as client:
+            await client.post(self.api_url, data=api_body, headers=self.headers)
+        logger.debug("`pushover` send successfully")
```

### Comparing `usepy_plugin_notify-0.2.4/PKG-INFO` & `usepy_plugin_notify-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: usepy-plugin-notify
-Version: 0.2.4
-Summary: 一个简单可扩展的消息通知库
+Version: 0.3.0
+Summary: 一个简单可扩展的异步消息通知库
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: usepy (>=0.1.34,<0.2.0)
+Requires-Dist: usepy (>=0.2.6,<0.3.0)
 Description-Content-Type: text/markdown
 
-### 一个简单可扩展的消息通知库
+### 一个简单可扩展的异步消息通知库
 
 <a href="https://pypi.org/project/ml-simple-notify" target="_blank">
     <img src="https://img.shields.io/pypi/v/ml-simple-notify.svg" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/ml-simple-notify" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/ml-simple-notify.svg" alt="Supported Python versions">
@@ -27,21 +27,21 @@
 #### 安装
 
 > pip install usepy-plugin-notify
 
 #### 使用
 
 ```python
-from notify import useNotify, channels
+from usepy.plugin import useNotify, useNotifyChannel
 
 notify = useNotify()
 notify.add(
     # 添加多个通知渠道
-    channels.Bark({"token": "xxxxxx"}),
-    channels.Ding({
+    useNotifyChannel.Bark({"token": "xxxxxx"}),
+    useNotifyChannel.Ding({
         "token": "xxxxx",
         "at_all": True
     })
 )
 
 notify.publish(title="消息标题", content="消息正文")
 
@@ -56,17 +56,20 @@
 - Chanify
 - Pushdeer
 - Pushover
 
 #### 自己开发消息通知
 
 ```python
-from notify.channels import BaseChannel
+from usepy.plugin import useNotifyChannel
 
 
-class Custom(BaseChannel):
+class Custom(useNotifyChannel.BaseChannel):
     """自定义消息通知"""
 
     def send(self, *args, **kwargs):
         ...
+
+    async def send_async(self, *args, **kwargs):
+        ...
 ```
```

