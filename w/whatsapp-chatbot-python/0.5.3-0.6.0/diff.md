# Comparing `tmp/whatsapp-chatbot-python-0.5.3.tar.gz` & `tmp/whatsapp-chatbot-python-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.5.3.tar", last modified: Fri Jul 21 05:38:42 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.6.0.tar", last modified: Fri Jul 28 09:31:10 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.5.3.tar` & `whatsapp-chatbot-python-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/
--rw-rw-rw-   0        0        0    18829 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/LICENSE
--rw-rw-rw-   0        0        0    15842 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    14404 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 05:38:42.443641 whatsapp-chatbot-python-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-07-21 05:37:30.000000 whatsapp-chatbot-python-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.430608 whatsapp-chatbot-python-0.5.3/tests/
--rw-rw-rw-   0        0        0     1459 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.432612 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      270 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-20 12:30:27.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     4362 2023-07-21 05:35:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.441636 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     4595 2023-07-21 05:35:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     2022 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/router.py
--rw-rw-rw-   0        0        0     2643 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/state.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:38:42.437627 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    15842 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-21 05:38:42.000000 whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:10.674035 whatsapp-chatbot-python-0.6.0/
+-rw-rw-rw-   0        0        0    18829 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    15842 2023-07-28 09:31:10.673033 whatsapp-chatbot-python-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14404 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:31:10.674035 whatsapp-chatbot-python-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-28 07:17:56.000000 whatsapp-chatbot-python-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:10.662004 whatsapp-chatbot-python-0.6.0/tests/
+-rw-rw-rw-   0        0        0     1498 2023-07-28 07:13:41.000000 whatsapp-chatbot-python-0.6.0/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:10.664009 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      270 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     2664 2023-07-28 07:13:41.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     4362 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:10.673033 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     4595 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     2022 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/router.py
+-rw-rw-rw-   0        0        0     2643 2023-07-28 04:40:27.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/state.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:31:10.668020 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    15842 2023-07-28 09:31:10.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-28 09:31:10.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:31:10.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-28 09:31:10.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-28 09:31:10.000000 whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.5.3/LICENSE` & `whatsapp-chatbot-python-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/PKG-INFO` & `whatsapp-chatbot-python-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.3
+Version: 0.6.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.3/README.md` & `whatsapp-chatbot-python-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/setup.py` & `whatsapp-chatbot-python-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.5.3",
+    version="0.6.0",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.5.3/tests/test_manager.py` & `whatsapp-chatbot-python-0.6.0/tests/test_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 
         self.assertEqual(len(bot.router.message.handlers), 2)
 
     @patch("whatsapp_chatbot_python.bot.Bot._update_settings")
     def create_bot(self, mock__update_settings: MagicMock) -> GreenAPIBot:
         mock__update_settings.return_value = None
 
-        return GreenAPIBot("", "")
+        return GreenAPIBot("", "", delete_notifications_at_startup=False)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,30 @@
 
 from whatsapp_api_client_python.API import GreenApi
 
 from .manager.router import Router
 
 
 class Bot:
-    def __init__(self, id_instance: str, api_token_instance: str):
+    def __init__(
+            self,
+            id_instance: str,
+            api_token_instance: str,
+            settings: Optional[dict] = None,
+            delete_notifications_at_startup: bool = True
+    ):
         self.api = GreenAPI(id_instance, api_token_instance)
 
-        self._update_settings()
+        if not settings:
+            self._update_settings()
+        else:
+            self.api.account.setSettings(settings)
+
+        if delete_notifications_at_startup:
+            self._delete_notifications_at_startup()
 
         self.router = Router(self.api)
 
     def run_forever(self) -> Optional[NoReturn]:
         while True:
             try:
                 response = self.api.receiving.receiveNotification()
@@ -47,14 +59,25 @@
         ):
             self.api.account.setSettings({
                 "incomingWebhook": "yes",
                 "outgoingMessageWebhook": "yes",
                 "outgoingAPIMessageWebhook": "yes"
             })
 
+    def _delete_notifications_at_startup(self) -> Optional[NoReturn]:
+        while True:
+            response = self.api.receiving.receiveNotification()
+            if response.error:
+                raise GreenAPIError(response.error)
+
+            if not response.data:
+                break
+
+            self.api.receiving.deleteNotification(response.data["receiptId"])
+
 
 class GreenAPI(GreenApi):
     pass
 
 
 class GreenAPIBot(Bot):
     pass
```

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python/manager/state.py` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python/manager/state.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.3
+Version: 0.6.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.3/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.6.0/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

