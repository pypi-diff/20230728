# Comparing `tmp/uagents_twilio_test_dummy-1.0.3.tar.gz` & `tmp/uagents_twilio_test_dummy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio_test_dummy-1.0.3.tar", max compression
+gzip compressed data, was "uagents_twilio_test_dummy-1.0.4.tar", max compression
```

## Comparing `uagents_twilio_test_dummy-1.0.3.tar` & `uagents_twilio_test_dummy-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio_test_dummy-1.0.3/LICENSE
--rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio_test_dummy-1.0.3/README.rst
--rw-r--r--   0        0        0      883 2023-07-21 10:29:43.965352 uagents_twilio_test_dummy-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-19 05:23:14.531167 uagents_twilio_test_dummy-1.0.3/uagents_twilio/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 11:32:55.835669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/__init__.py
--rw-r--r--   0        0        0     1727 2023-07-18 11:32:55.843669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/constants.py
--rw-r--r--   0        0        0    14304 2023-07-19 05:23:14.931181 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/google_calendar.py
--rw-r--r--   0        0        0     1229 2023-07-18 11:32:55.847669 uagents_twilio_test_dummy-1.0.3/uagents_twilio/gc_integration/utils.py
--rw-r--r--   0        0        0      219 2023-07-21 10:10:13.473269 uagents_twilio_test_dummy-1.0.3/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1432 2023-07-21 10:10:13.621270 uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/sms.py
--rw-r--r--   0        0        0      769 2023-07-21 10:10:13.485269 uagents_twilio_test_dummy-1.0.3/uagents_twilio/webhook.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1969 2023-07-19 09:32:47.021259 uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/smsWrapper.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 uagents_twilio_test_dummy-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio_test_dummy-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1478 2023-07-25 06:57:41.723405 uagents_twilio_test_dummy-1.0.4/README.rst
+-rw-r--r--   0        0        0      939 2023-07-28 05:17:51.138825 uagents_twilio_test_dummy-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio_test_dummy-1.0.4/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio_test_dummy-1.0.4/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio_test_dummy-1.0.4/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio_test_dummy-1.0.4/uagents_twilio/protocols/messages.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio_test_dummy-1.0.4/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio_test_dummy-1.0.4/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 uagents_twilio_test_dummy-1.0.4/PKG-INFO
```

### Comparing `uagents_twilio_test_dummy-1.0.3/LICENSE` & `uagents_twilio_test_dummy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio_test_dummy-1.0.3/pyproject.toml` & `uagents_twilio_test_dummy-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "uagents-twilio-test-dummy"
 #
-version = '1.0.3'
+version = '1.0.4'
 #
-description = ""
-authors = ["Harsh <harsh@gmail.com>"]
+description = "Use uagents to automate SMS/Whatsapp by twilio"
+authors = ["Harsh <harsh.patel@fetch.ai>"]
 readme = "README.rst"
-repository = "https://github.com/Github User/uagents-twilio"
+repository = "https://github.com/harshpatel199259/uagents_twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
```

### Comparing `uagents_twilio_test_dummy-1.0.3/uagents_twilio/protocols/sms.py` & `uagents_twilio_test_dummy-1.0.4/uagents_twilio/protocols/messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from decouple import config
 from uagents import Context, Protocol
 
-from uagents_twilio.models import WhatsAppCustomMsg, WhatsAppWebhookMsg
-from uagents_twilio.wrappers.smsWrapper import WhatsappClient
+from uagents_twilio.models import Message, MessageType
+from uagents_twilio.wrappers.messageWrapper import MessageClient
 
 service_protocol = Protocol()
-
-AGENT1_EMAIL = config("AGENT1_EMAIL")
-AGENT2_EMAIL = config("AGENT2_EMAIL")
-
+AGENT_ADDRESS = config("AGENT_ADDRESS")
 ACCOUNT_SID = config("ACCOUNT_SID")
 AUTH_TOKEN = config("AUTH_TOKEN")
 FROM_NUMBER = config("FROM_NUMBER")
+WP_FROM_NUMBER = config("WP_FROM_NUMBER")
 TO_NUMBER = config("TO_NUMBER")
 
 
-whatsapp_handler = WhatsappClient(
+message_handler = MessageClient(
     agent=service_protocol,
-    to_agent_address="agent1qfrs3x9eh4pvaymsmwgjkjq4srqq4ctfw8h5hjduscmq4asq027tucn2gqw",
+    to_agent_address=AGENT_ADDRESS,
     account_sid=ACCOUNT_SID,
     auth_token=AUTH_TOKEN,
     from_number=FROM_NUMBER,
     to_number=TO_NUMBER,
 )
 
 
-@service_protocol.on_query(model=WhatsAppWebhookMsg)
-async def receive_msg(ctx: Context, sender: str, message: WhatsAppWebhookMsg):
-    await ctx.send(sender, WhatsAppWebhookMsg(sender=message.sender, msg="Received"))
+@service_protocol.on_query(model=Message)
+async def receive_wp_msg(ctx: Context, sender: str, message: Message):
+    """Receive message from Twilio Webhook and send starting message on Whatsapp"""
     ctx.storage.set("message", message.msg)
-    whatsapp_handler.send_new_message(message.sender, message.start_message)
+    if message.type == MessageType.whatsapp:
+        if not message.receiver.startswith("whatsapp:"):
+            message.receiver = f"whatsapp:{message.receiver}"
+        message_handler.from_number = WP_FROM_NUMBER
+    message_handler.send_message(message.receiver, message.msg, message.type)
 
 
-@service_protocol.on_message(model=WhatsAppCustomMsg)
-async def send_wp_msg(ctx: Context, sender: str, message: WhatsAppCustomMsg):
-    await ctx.send(
-        sender,
-        WhatsAppCustomMsg(receiver=message.receiver, msg="Sending a msg on Whatsapp"),
-    )
+@service_protocol.on_message(model=Message)
+async def send_wp_msg(ctx: Context, sender: str, message: Message):
+    """Send Whatsapp Message or SMS using uagent"""
     ctx.storage.set("message", message.msg)
-    whatsapp_handler.send_new_message(message.receiver, message.msg)
+    if message.type == MessageType.whatsapp:
+        if not message.receiver.startswith("whatsapp:"):
+            message.receiver = f"whatsapp:{message.receiver}"
+        message_handler.from_number = WP_FROM_NUMBER
+    message_handler.send_message(message.receiver, message.msg, message.type)
```

### Comparing `uagents_twilio_test_dummy-1.0.3/uagents_twilio/wrappers/smsWrapper.py` & `uagents_twilio_test_dummy-1.0.4/uagents_twilio/wrappers/messageWrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Start writing utility wrapper from here
 import requests
-from uagents import Agent, Context
+from uagents import Agent
 
-# from uagents.setup import fund_agent_if_low
+from uagents_twilio.models import MessageType
 
 
-class WhatsappClient:
+class MessageClient:
     """Base class for handling WhatsApp operations"""
 
     def __init__(
         self,
         agent: Agent,
         to_agent_address: str,
         account_sid: str,
@@ -19,28 +19,22 @@
     ):
         self.agent = agent
         self.to_agent_address = to_agent_address
         self.account_sid = account_sid
         self.auth_token = auth_token
         self.from_number = from_number
         self.to_number = to_number
-        # fund_agent_if_low(agent.wallet.address())
 
-    def listen_for_new_message(self, ctx: Context, sender_no: str, body: str):
-        if sender_no == "" or body == "":
-            return
-        else:
-            ctx.logger.info(
-                f"Received a new message from {sender_no}, message : {body}"
-            )
-            self.send_new_message(body)
-
-    def send_new_message(self, receiver, message: str):
+    def send_message(self, receiver, message: str, message_type):
         body = message
         twilio = TwilioWrapper(self.account_sid, self.auth_token)
+        if message_type == MessageType.whatsapp and not self.from_number.startswith(
+            "whatsapp:"
+        ):
+            self.from_number = f"whatsapp:{self.from_number}"
         twilio.send_message(self.from_number, receiver, body)
 
 
 class TwilioWrapper:
     def __init__(self, account_sid, auth_token):
         self.account_sid = account_sid
         self.auth_token = auth_token
```

