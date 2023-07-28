# Comparing `tmp/AppiumExtended-0.1.3.tar.gz` & `tmp/AppiumExtended-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.1.3.tar", last modified: Thu Jul 27 20:46:21 2023, max compression
+gzip compressed data, was "AppiumExtended-0.1.6.tar", last modified: Fri Jul 28 13:00:51 2023, max compression
```

## Comparing `AppiumExtended-0.1.3.tar` & `AppiumExtended-0.1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.273734 AppiumExtended-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.204734 AppiumExtended-0.1.3/AppiumExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:45.000000 AppiumExtended-0.1.3/AppiumExtended/__init__.py
--rw-rw-rw-   0        0        0     2564 2023-07-27 15:28:50.000000 AppiumExtended-0.1.3/AppiumExtended/appium_base.py
--rw-rw-rw-   0        0        0    28523 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_extended.py
--rw-rw-rw-   0        0        0    15339 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_get.py
--rw-rw-rw-   0        0        0     2505 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_is.py
--rw-rw-rw-   0        0        0     2259 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_swipe.py
--rw-rw-rw-   0        0        0     1888 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_tap.py
--rw-rw-rw-   0        0        0     7107 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_wait.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.213737 AppiumExtended-0.1.3/AppiumExtended.egg-info/
--rw-rw-rw-   0        0        0      486 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1328 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/requires.txt
--rw-rw-rw-   0        0        0      131 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.218738 AppiumExtended-0.1.3/AppiumGraph/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:49.000000 AppiumExtended-0.1.3/AppiumGraph/__init__.py
--rw-rw-rw-   0        0        0      486 2023-07-26 16:29:27.000000 AppiumExtended-0.1.3/AppiumGraph/appium_graph.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.226733 AppiumExtended-0.1.3/AppiumHelpers/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:54.000000 AppiumExtended-0.1.3/AppiumHelpers/__init__.py
--rw-rw-rw-   0        0        0    18033 2023-07-26 16:33:16.000000 AppiumExtended-0.1.3/AppiumHelpers/appium_helpers.py
--rw-rw-rw-   0        0        0    32167 2023-07-26 16:36:11.000000 AppiumExtended-0.1.3/AppiumHelpers/appium_image.py
--rw-rw-rw-   0        0        0    19788 2023-07-26 17:49:07.000000 AppiumExtended-0.1.3/AppiumHelpers/helpers_decorators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.230735 AppiumExtended-0.1.3/AppiumNavigator/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:58.000000 AppiumExtended-0.1.3/AppiumNavigator/__init__.py
--rw-rw-rw-   0        0        0     7472 2023-07-27 16:28:38.000000 AppiumExtended-0.1.3/AppiumNavigator/appium_navigator.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.237745 AppiumExtended-0.1.3/AppiumServer/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:03.000000 AppiumExtended-0.1.3/AppiumServer/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-07-27 20:06:25.000000 AppiumExtended-0.1.3/AppiumServer/appium_server.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.256736 AppiumExtended-0.1.3/AppiumWebElementExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:07.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/__init__.py
--rw-rw-rw-   0        0        0        6 2023-05-31 18:50:55.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_actions.py
--rw-rw-rw-   0        0        0     9210 2023-07-26 16:51:39.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_adb_actions.py
--rw-rw-rw-   0        0        0    11345 2023-07-26 16:53:53.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_click.py
--rw-rw-rw-   0        0        0    14511 2023-07-26 16:56:52.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_dom.py
--rw-rw-rw-   0        0        0    17174 2023-07-26 16:56:57.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_extended.py
--rw-rw-rw-   0        0        0    23257 2023-07-26 16:58:06.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_get.py
--rw-rw-rw-   0        0        0    11658 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_scroll.py
--rw-rw-rw-   0        0        0    12723 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_tap.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.259734 AppiumExtended-0.1.3/AppiumWebElementsExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:11.000000 AppiumExtended-0.1.3/AppiumWebElementsExtended/__init__.py
--rw-rw-rw-   0        0        0      493 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementsExtended/web_elements_extended.py
--rw-rw-rw-   0        0        0     1090 2023-07-26 20:30:30.000000 AppiumExtended-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      486 2023-07-27 20:46:21.273734 AppiumExtended-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-27 17:44:37.000000 AppiumExtended-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.264734 AppiumExtended-0.1.3/adb/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:39.000000 AppiumExtended-0.1.3/adb/__init__.py
--rw-rw-rw-   0        0        0    27262 2023-07-26 16:49:36.000000 AppiumExtended-0.1.3/adb/adb.py
--rw-rw-rw-   0        0        0       42 2023-07-27 20:46:21.274733 AppiumExtended-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-07-27 20:44:43.000000 AppiumExtended-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.271734 AppiumExtended-0.1.3/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:21.000000 AppiumExtended-0.1.3/utils/__init__.py
--rw-rw-rw-   0        0        0    16209 2023-07-26 16:53:52.000000 AppiumExtended-0.1.3/utils/operations.py
--rw-rw-rw-   0        0        0     6955 2023-07-26 17:07:41.000000 AppiumExtended-0.1.3/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28026 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_swipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumExtended/appium_wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumExtended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 13:00:51.000000 AppiumExtended-0.1.6/AppiumExtended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.636560 AppiumExtended-0.1.6/AppiumGraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumGraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumGraph/appium_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumHelpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/appium_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31656 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/appium_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumHelpers/helpers_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumNavigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumNavigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumNavigator/appium_navigator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumServer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumServer/appium_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumWebElementExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/AppiumWebElementsExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementsExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/AppiumWebElementsExtended/web_elements_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27562 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/adb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/adb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27272 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/adb/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:51.640560 AppiumExtended-0.1.6/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-28 13:00:41.000000 AppiumExtended-0.1.6/utils/utils.py
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_base.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# coding: utf-8
-import logging
-import json
-import time
-
-from appium import webdriver
-
-import config
-from AppiumServer.appium_server import AppiumServer
-from AppiumHelpers.appium_image import AppiumImage
-
-
-class AppiumBase(object):
-    """
-    Класс работы с Appium.
-    Обеспечивает подключение к устройству
-    """
-
-    def __init__(self):
-
-        # keep_alive_server: bool = False,
-        # log_level = 'error',
-        # url = 'http://localhost:4723/wd/hub',
-        # port = 4723,
-
-        self.url = f"http://{config.APPIUM_IP}:{config.APPIUM_PORT}/wd/hub"
-        self.capabilities = None
-        self.keep_alive_server = True
-        self.driver = None
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        self.server = AppiumServer(port=config.APPIUM_IP, log_level=config.APPIUM_LOG_LEVEL)
-        self.image = None
-
-    def connect(self, capabilities: dict):
-        """
-        Подключение к устройству
-        """
-        self.capabilities = capabilities
-        self.logger.debug(
-            f"connect(capabilities {self.capabilities}")
-        if not config.PROXY:
-            # запускаем локальный сервер Аппиум
-            if not self.server.is_alive():
-                self.server.start()
-                time.sleep(10)
-                self.server.wait_until_alive()
-
-        self.logger.info(f"Подключение к серверу: {self.url=}")
-        self.driver = webdriver.Remote(command_executor=self.url,
-                                       desired_capabilities=self.capabilities,
-                                       keep_alive=True)
-
-        app_capabilities = json.dumps(capabilities)
-
-        # Инициализация объектов требующих драйвер
-        self.image = AppiumImage(driver=self.driver)
-
-        self.logger.info('Подключение установлено: '.format(app_capabilities))
-        self.logger.info(f'Сессия №: {self.driver.session_id}')
-
-    def disconnect(self):
-        """
-        Отключение от устройства
-        """
-        if self.driver:
-            self.logger.debug(f"Отключение от сессии №: {self.driver.session_id}")
-            self.driver.quit()
-            self.driver = None
-        if not self.keep_alive_server:
-            self.server.stop()
-
-    def is_running(self):
-        return self.driver.is_running()
-
+# coding: utf-8
+import logging
+import json
+import time
+
+from appium import webdriver
+
+import config
+from AppiumServer.appium_server import AppiumServer
+from AppiumHelpers.appium_image import AppiumImage
+
+
+class AppiumBase(object):
+    """
+    Класс работы с Appium.
+    Обеспечивает подключение к устройству
+    """
+
+    def __init__(self):
+
+        # keep_alive_server: bool = False,
+        # log_level = 'error',
+        # url = 'http://localhost:4723/wd/hub',
+        # port = 4723,
+
+        self.url = f"http://{config.APPIUM_IP}:{config.APPIUM_PORT}/wd/hub"
+        self.capabilities = None
+        self.keep_alive_server = True
+        self.driver = None
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        self.server = AppiumServer(port=config.APPIUM_IP, log_level=config.APPIUM_LOG_LEVEL)
+        self.image = None
+
+    def connect(self, capabilities: dict):
+        """
+        Подключение к устройству
+        """
+        self.capabilities = capabilities
+        self.logger.debug(
+            f"connect(capabilities {self.capabilities}")
+        if not config.PROXY:
+            # запускаем локальный сервер Аппиум
+            if not self.server.is_alive():
+                self.server.start()
+                time.sleep(10)
+                self.server.wait_until_alive()
+
+        self.logger.info(f"Подключение к серверу: {self.url=}")
+        self.driver = webdriver.Remote(command_executor=self.url,
+                                       desired_capabilities=self.capabilities,
+                                       keep_alive=True)
+
+        app_capabilities = json.dumps(capabilities)
+
+        # Инициализация объектов требующих драйвер
+        self.image = AppiumImage(driver=self.driver)
+
+        self.logger.info('Подключение установлено: '.format(app_capabilities))
+        self.logger.info(f'Сессия №: {self.driver.session_id}')
+
+    def disconnect(self):
+        """
+        Отключение от устройства
+        """
+        if self.driver:
+            self.logger.debug(f"Отключение от сессии №: {self.driver.session_id}")
+            self.driver.quit()
+            self.driver = None
+        if not self.keep_alive_server:
+            self.server.stop()
+
+    def is_running(self):
+        return self.driver.is_running()
+
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_extended.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_extended.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,497 +1,497 @@
-# coding: utf-8
-import time
-from typing import Union, Tuple, Dict, List, Optional, cast, Any
-
-import numpy as np
-from PIL import Image
-from appium.webdriver import WebElement
-from appium.webdriver.common.appiumby import AppiumBy
-from appium.webdriver.common.mobileby import MobileBy
-from selenium.common import StaleElementReferenceException
-from selenium.webdriver.common.by import By
-
-from AppiumExtended.appium_is import AppiumIs
-from AppiumExtended.appium_swipe import AppiumSwipe
-from AppiumExtended.appium_tap import AppiumTap
-from AppiumExtended.appium_wait import AppiumWait
-from AppiumWebElementExtended.web_element_extended import WebElementExtended
-from adb import adb
-from utils import utils
-
-
-class AppiumExtended(AppiumIs, AppiumTap, AppiumSwipe, AppiumWait):
-    """
-    Класс работы с Appium.
-    Обеспечивает работу с устройством
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def __del__(self):
-        self.disconnect()
-
-    def get_element(self,
-                    locator: Union[Tuple, WebElementExtended, Dict[str, str], str] = None,
-                    by: Union[MobileBy, AppiumBy, By, str] = None,
-                    value: Union[str, Dict, None] = None,
-                    timeout_elem: int = 10,
-                    timeout_method: int = 600,
-                    elements_range: Union[Tuple, List[WebElementExtended], Dict[str, str], None] = None,
-                    contains: bool = True,
-                    ) -> Union[WebElementExtended, None]:
-        """
-        Получает элемент на странице, используя указанный локатор или параметры.
-
-        Аргументы:
-        - locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional):
-            Локатор или элемент для поиска. По умолчанию None.
-        - by (Union[MobileBy, AppiumBy, By, str], optional): Метод поиска элемента.
-            По умолчанию None.
-        - value (Union[str, Dict, None], optional): Значение для поиска элемента.
-            По умолчанию None.
-        - timeout_elem (int, optional): Время ожидания появления элемента.
-            По умолчанию 10.
-        - timeout_method (int, optional): Время ожидания выполнения метода.
-            По умолчанию 600.
-        - elements_range (Union[Tuple, List[WebElementExtended], Dict[str, str], None], optional):
-            Диапазон элементов для выбора. По умолчанию None.
-        - contains (bool, optional): Флаг, указывающий на необходимость использования частичного совпадения текста.
-            По умолчанию True.
-
-        Возвращает:
-        - Union[WebElementExtended, None]: Расширенный элемент WebElementExtended или None, если элемент не найден.
-        """
-        element = self._get_element(locator=locator,
-                                    by=by,
-                                    value=value,
-                                    timeout_elem=timeout_elem,
-                                    timeout_method=timeout_method,
-                                    elements_range=elements_range,
-                                    contains=contains)
-        return WebElementExtended(element.parent, element.id)
-
-    def get_elements(self,
-                     locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
-                     by: Union[MobileBy, AppiumBy, By, str] = None,
-                     value: Union[str, Dict, None] = None,
-                     timeout_elements: int = 10,
-                     timeout_method: int = 600,
-                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                     contains: bool = True,
-                     ) -> Union[List[WebElementExtended], List]:
-        """
-        Получает элементы на странице, используя указанный локатор или параметры.
-
-        Args:
-        - locator (Union[Tuple, List[WebElement], Dict[str, str], str], optional): Локатор или элементы для поиска.
-            По умолчанию None.
-        - by (Union[MobileBy, AppiumBy, By, str], optional): Метод поиска элементов.
-            По умолчанию None.
-        - value (Union[str, Dict, None], optional): Значение для поиска элементов.
-            По умолчанию None.
-        - timeout_elements (int, optional): Время ожидания появления элементов.
-            По умолчанию 10.
-        - timeout_method (int, optional): Время ожидания выполнения метода.
-            По умолчанию 600.
-        - elements_range (Union[Tuple, List[WebElement], Dict[str, str], None], optional): Диапазон элементов для выбора.
-            По умолчанию None.
-        - contains (bool, optional): Флаг, указывающий на необходимость использования частичного совпадения текста.
-            По умолчанию True.
-
-        Returns:
-        - Union[List[WebElementExtended], List]: Список расширенных элементов WebElementExtended или обычных элементов WebElement в случае ошибки.
-        """
-        elements = super()._get_elements(locator=locator,
-                                         by=by,
-                                         value=value,
-                                         timeout_elements=timeout_elements,
-                                         timeout_method=timeout_method,
-                                         elements_range=elements_range,
-                                         contains=contains)
-        elements_ext = []
-        for element in elements:
-            elements_ext.append(WebElementExtended(element.parent, element.id))
-        return elements_ext
-
-    def get_image_coordinates(self,
-                              image: Union[bytes, np.ndarray, Image.Image, str],
-                              full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                              threshold: float = 0.7,
-                              ) -> Union[Tuple, None]:
-        return self._get_image_coordinates(full_image=full_image,
-                                           image=image,
-                                           threshold=threshold)
-
-    def get_inner_image_coordinates(self,
-                                    outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                    inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                    threshold: Optional[float] = 0.9
-                                    ) -> Union[Tuple[int, int, int, int], None]:
-        """
-        Возвращает координаты x y (относительно экрана) по изображению внутри другого изображения
-        """
-        return self._get_inner_image_coordinates(outer_image_path=outer_image_path,
-                                                 inner_image_path=inner_image_path,
-                                                 threshold=threshold)
-
-    def get_many_coordinates_of_image(self,
-                                      image: Union[bytes, np.ndarray, Image.Image, str],
-                                      full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                                      cv_threshold: Optional[float] = 0.7,
-                                      coord_threshold: Optional[int] = 5,
-                                      ) -> Union[List[Tuple], None]:
-        return self.image.get_many_coordinates_of_image(full_image=full_image,
-                                                        image=image,
-                                                        cv_threshold=cv_threshold,
-                                                        coord_threshold=coord_threshold)
-
-    def get_text_coordinates(self,
-                             text: str,
-                             language: Optional[str] = 'rus',
-                             image: Union[bytes, str, Image.Image, np.ndarray] = None,
-                             ocr: Optional[bool] = True,
-                             ) -> Union[Tuple[int, int, int, int], None]:  # TODO реализовать None
-        """
-        # TODO fill
-        """
-        if ocr:
-            return self._get_text_coordinates(text=text, language=language, image=image)
-        else:
-            return self.get_element(locator={'text': text, 'displayed': 'true', 'enabled': 'true'}).get_coordinates()
-
-    # DOM
-
-    def get_element_contains(self,
-                             ) -> Any:
-        """
-        Возвращает элемент содержащий определенный элемент
-        """
-        raise NotImplementedError("This method is not implemented yet.")  # TODO implement
-
-    def get_elements_contains(self,
-                              ) -> Any:
-        """
-        Возвращает элементы содержащие определенный(е) элемент(ы)
-        """
-        raise NotImplementedError("This method is not implemented yet.")  # TODO implement
-
-    def get_screenshot_as_base64_decoded(self) -> bytes:
-        return self._get_screenshot_as_base64_decoded()
-
-    def find_and_get_element(self,
-                             locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-                             timeout: int = 10,
-                             ) -> Union[WebElementExtended, None]:
-        """
-        Ищет элемент на странице, если нет то скроллит все что скроллится и ищет там
-        """
-        if self.is_element_within_screen(locator=locator, timeout=1):
-            return self.get_element(locator=locator, timeout_elem=timeout)
-        recyclers = self.get_elements(locator={'scrollable': 'true', 'enabled': 'true', 'displayed': 'true'})
-        for recycler in recyclers:
-            try:
-                if recycler.scroll_until_find(locator=locator):
-                    return self.get_element(locator=locator, timeout_elem=timeout)
-            except StaleElementReferenceException as e:
-                print(e)
-                print("find_and_get_element StaleElementReferenceException")
-                print(f"{recycler=}")
-                print(f"{locator=}")
-        return None
-
-    def is_element_within_screen(self,
-                                 locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-                                 timeout: int = 10,
-                                 ) -> bool:
-        """
-        Метод проверяет, находится ли заданный элемент на видимом экране.
-
-        Аргументы:
-        - locator (Union[tuple, WebElement]): Локатор или элемент, который нужно проверить.
-        - timeout (int): Время ожидания элемента. Значение по умолчанию: 10.
-
-        Возвращает:
-        - bool: True, если элемент находится на экране, False, если нет.
-        """
-        return self._is_element_within_screen(locator=locator, timeout=timeout)
-
-    def is_text_on_screen(self,
-                          text: str,
-                          language: str = 'rus',
-                          ocr: bool = True,
-                          ) -> bool:
-        """
-        Проверяет, присутствует ли заданный текст на экране.
-        Если ocr=True:
-            Распознавание текста производит с помощью библиотеки pytesseract.
-        Если ocr=False:
-            Производится поиск элемента по xpath.
-
-        Аргументы:
-        - text (str): Текст, который нужно найти на экране.
-        - ocr (bool): Производить поиск по изображению или DOM.
-        - language (str): Язык распознавания текста. Значение по умолчанию: 'rus'.
-
-        Возвращает:
-        - bool: True, если заданный текст найден на экране. False в противном случае.
-        """
-        if ocr:
-            return self.image.is_text_on_ocr_screen(text=text, language=language)
-        else:
-            return self._is_element_within_screen(locator={'text': text})
-
-    def is_image_on_the_screen(self,
-                               image: Union[bytes, np.ndarray, Image.Image, str],
-                               threshold: float = 0.9,
-                               ) -> bool:
-        return self.image.is_image_on_the_screen(image=image,
-                                                 threshold=threshold)
-
-    def tap(self,
-            locator: Union[Tuple[str, str], WebElementExtended, WebElement, Dict[str, str], str] = None,
-            x: int = None,
-            y: int = None,
-            image: Union[bytes, np.ndarray, Image.Image, str] = None,
-            duration: Optional[int] = None,
-            timeout: int = 5,
-            ) -> Union['AppiumExtended', None]:
-        """
-        Тап по координатам / элементу / изображению
-        """
-        if locator is not None:
-            # Извлечение координат
-            x, y = self._extract_point_coordinates_by_typing(locator)
-        if image is not None:
-            start_time = time.time()
-            while not self.is_image_on_the_screen(image=image) and time.time() - start_time < timeout:
-                time.sleep(1)
-            # Извлечение координат
-            x, y = self._extract_point_coordinates_by_typing(image)
-
-        assert self._tap(x=x, y=y,
-                         duration=duration)
-        # Возвращаем экземпляр класса AppiumExtended
-        return cast('AppiumExtended', self)
-
-    # SWIPE
-
-    def swipe(self,
-              start_position: Union[
-                  Tuple[int, int], str, bytes, np.ndarray, Image.Image, WebElement, WebElementExtended, Tuple[str, str],
-                  Dict[str, str]],
-              end_position: Optional[Union[
-                  Tuple[int, int], str, bytes, np.ndarray, Image.Image, WebElement, WebElementExtended, Tuple[str, str],
-                  Dict[str, str]]] = None,
-              direction: Optional[int] = None,
-              distance: Optional[int] = None,
-              duration: Optional[int] = 0,
-              ) -> 'AppiumExtended':
-        """
-        Выполняет свайп (перетаскивание) элемента или изображения на экране.
-
-        Параметры:
-        - start_position: Позиция начала свайпа. Может быть задана в различных форматах:
-            - Если `start_position` является кортежем и оба его элемента являются строками, то он представляет собой
-              локатор элемента. В этом случае будет выполнен поиск элемента и используется его позиция.
-            - Если `start_position` является словарем, то считается, что это локатор элемента, основанный на атрибутах.
-              Например, {'text': 'some text'} или {'class': 'SomeClass', 'visible': 'true'}. В этом случае будет
-              выполнен поиск элемента по указанным атрибутам, и используется его позиция.
-            - Если `start_position` является экземпляром класса WebElement или WebElementExtended, то используется его
-              позиция.
-            - Если `start_position` является строкой, массивом байтов (bytes), массивом NumPy (np.ndarray) или объектом
-              класса Image.Image, то считается, что это изображение. В этом случае будет вычислен центр изображения и
-              используется его позиция.
-            - Если `start_position` является кортежем, и оба его элемента являются целыми числами, то считается, что это
-              координаты в формате (x_coordinate, y_coordinate).
-
-        - end_position: Позиция конца свайпа. Принимает те же форматы, что и `start_position`. По умолчанию None.
-        - direction (опционально): Направление свайпа. Принимает значения от 0 до 360 градусов.
-          Если указано направление, то будет вычислена конечная точка свайпа на основе текущего размера окна и
-          указанного расстояния. По умолчанию None.
-        - distance (опционально): Расстояние свайпа. Принимается в пикселях. Используется только в сочетании с параметром
-          `direction`. По умолчанию None.
-        - duration (опционально): Продолжительность свайпа в миллисекундах. По умолчанию 0.
-
-        Возвращает:
-        - self: Экземпляр класса AppiumExtended.
-
-        Примечания:
-        - В качестве конечной позиции свайпа должен быть указан end_position или пара direction, distance.
-        - str принимается как путь к изображению на экране и вычисляется его центр, а не как локатор элемента
-
-        """
-        # Извлечение координат начальной точки свайпа
-        start_x, start_y = self._extract_point_coordinates_by_typing(start_position)
-
-        if end_position is not None:
-            # Извлечение координат конечной точки свайпа
-            end_x, end_y = self._extract_point_coordinates_by_typing(end_position)
-        else:
-            # Извлечение координат конечной точки свайпа на основе направления и расстояния
-            end_x, end_y = self._extract_point_coordinates_by_direction(direction, distance, start_x, start_y)
-
-        # Выполнение свайпа
-        assert self._swipe(start_x=start_x, start_y=start_y,
-                           end_x=end_x, end_y=end_y,
-                           duration=duration)
-
-        # Возвращаем экземпляр класса AppiumExtended
-        return cast('AppiumExtended', self)
-
-    def swipe_right_to_left(self):
-        window_size = adb.get_screen_resolution()
-        width = window_size[0]
-        height = window_size[1]
-        left = int(width * 0.1)
-        right = int(width * 0.9)
-        self.swipe(start_position=(right, height // 2),
-                   end_position=(left, height // 2))
-
-    def swipe_left_to_right(self):
-        window_size = adb.get_screen_resolution()
-        width = window_size[0]
-        height = window_size[1]
-        left = int(width * 0.1)
-        right = int(width * 0.9)
-        self.swipe(start_position=(left, height // 2),
-                   end_position=(right, height // 2))
-
-    def swipe_top_to_bottom(self):
-        window_size = adb.get_screen_resolution()
-        height = window_size[1]
-        top = int(height * 0.1)
-        bottom = int(height * 0.9)
-        self.swipe(start_position=(top, height // 2),
-                   end_position=(bottom, height // 2))
-
-    def swipe_bottom_to_top(self):
-        window_size = adb.get_screen_resolution()
-        height = window_size[1]
-        top = int(height * 0.1)
-        bottom = int(height * 0.9)
-        self.swipe(start_position=(bottom, height // 2),
-                   end_position=(top, height // 2))
-
-    # WAIT
-
-    def wait_for(self,
-                 locator: Union[Tuple[str, str], WebElement, 'WebElementExtended', Dict[str, str], str,
-                 List[Tuple[str, str]], List[WebElement], List['WebElementExtended'], List[Dict[str, str]], List[
-                     str]] = None,
-                 image: Union[bytes, np.ndarray, Image.Image, str,
-                 List[bytes], List[np.ndarray], List[Image.Image], List[str]] = None,
-                 timeout: int = 10,
-                 contains: bool = True,
-                 full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                 ):
-        return self._wait_for(locator=locator,
-                              image=image,
-                              timeout=timeout,
-                              contains=contains)
-
-    def wait_for_not(self,
-                     locator: Union[Tuple[str, str], WebElement, 'WebElementExtended', Dict[str, str], str,
-                     List[Tuple[str, str]], List[WebElement], List['WebElementExtended'], List[Dict[str, str]], List[
-                         str]] = None,
-                     image: Union[bytes, np.ndarray, Image.Image, str,
-                     List[bytes], List[np.ndarray], List[Image.Image], List[str]] = None,
-                     timeout: int = 10,
-                     contains: bool = True,
-                     ):
-        return self._wait_for_not(locator=locator, image=image, timeout=timeout, contains=contains)
-
-    def wait_return_true(self, method, timeout: int = 10):
-        return self._wait_return_true(method=method, timeout=timeout)
-
-    # KEYBOARD
-
-    def input_by_virtual_keyboard(self) -> 'AppiumExtended':  # TODO реализовать возврат cast('AppiumExtended', self)
-        """
-        Вводит с помощью виртуально клавиатуры
-        """
-        raise NotImplementedError("This method is not implemented yet.")
-
-    # OTHER
-
-    def draw_by_coordinates(self,
-                            image: Union[bytes, str, Image.Image, np.ndarray] = None,
-                            coordinates: Tuple[int, int, int, int] = None,
-                            top_left: Tuple[int, int] = None,
-                            bottom_right: Tuple[int, int] = None,
-                            path: str = None,
-                            ) -> 'AppiumExtended':
-        assert self.image.draw_by_coordinates(image=image,
-                                              coordinates=coordinates,
-                                              top_left=top_left,
-                                              bottom_right=bottom_right,
-                                              path=path)
-        return cast('AppiumExtended', self)
-
-    # PRIVATE
-
-    def _extract_point_coordinates_by_typing(self,
-                                             position:
-                                             Union[Tuple[int, int], str, bytes, np.ndarray, Image.Image,
-                                             Tuple[str, str], Dict, WebElement, WebElementExtended]
-                                             ) -> Tuple[int, int]:
-        """
-        Извлекает координаты точки на основе типа переданной позиции.
-
-        Параметры:
-            position (
-            Union[Tuple[int, int], str, bytes, np.ndarray, Image.Image, Dict, WebElement, WebElementExtended]
-            ):
-                Позиция, для которой нужно извлечь координаты.
-                Либо локатор элемента, либо изображение, либо кортеж из координат.
-
-        Возвращает:
-            Tuple[int, int]: Кортеж координат точки, в формате (x, y).
-        """
-        x, y = 0, 0
-        # Вычисление позиции начала свайпа
-        if (isinstance(position, Tuple) and
-                isinstance(position[0], int) and
-                isinstance(position[1], int)):
-            # Если position является кортежем с двумя целыми числами, то считаем, что это координаты
-            x, y = position
-        elif (isinstance(position, Tuple) and
-              isinstance(position[0], str) and
-              isinstance(position[1], str)) or \
-                isinstance(position, WebElement) or \
-                isinstance(position, WebElementExtended) or \
-                isinstance(position, Dict):
-            # Если position является кортежем с двумя строковыми элементами или экземпляром WebElement,
-            # WebElementExtended или словарем, то получаем координаты центра элемента
-            x, y = utils.calculate_center_of_coordinates(
-                self.get_element(locator=position).get_coordinates())
-        elif isinstance(position, (bytes, np.ndarray, Image.Image, str)):
-            # Если position является строкой, байтами, массивом NumPy или объектом Image.Image,
-            # то получаем координаты центра изображения
-            x, y = utils.calculate_center_of_coordinates(
-                self.get_image_coordinates(image=position))
-        return x, y
-
-    def _extract_point_coordinates_by_direction(self,
-                                                direction: int, distance: int,
-                                                start_x: int, start_y: int
-                                                ) -> Tuple[int, int]:
-        """
-        Извлекает координаты точки на заданном расстоянии и в заданном направлении относительно начальных координат.
-
-        Параметры:
-            direction (str): Направление движения в пределах 360 градусов.
-            distance (int): Расстояние, на которое нужно переместиться относительно начальных координат в пикселях.
-            start_x (int): Начальная координата X.
-            start_y (int): Начальная координата Y.
-
-        Возвращает:
-            Tuple[int, int]: Координаты конечной точки в формате (x, y).
-        """
-        window_size = adb.get_screen_resolution()
-        width = window_size[0]
-        height = window_size[1]
-        end_x, end_y = utils.find_coordinates_by_vector(width=width, height=height,
-                                                        direction=direction, distance=distance,
-                                                        start_x=start_x, start_y=start_y)
-        return end_x, end_y
+# coding: utf-8
+import time
+from typing import Union, Tuple, Dict, List, Optional, cast, Any
+
+import numpy as np
+from PIL import Image
+from appium.webdriver import WebElement
+from appium.webdriver.common.appiumby import AppiumBy
+from appium.webdriver.common.mobileby import MobileBy
+from selenium.common import StaleElementReferenceException
+from selenium.webdriver.common.by import By
+
+from AppiumExtended.appium_is import AppiumIs
+from AppiumExtended.appium_swipe import AppiumSwipe
+from AppiumExtended.appium_tap import AppiumTap
+from AppiumExtended.appium_wait import AppiumWait
+from AppiumWebElementExtended.web_element_extended import WebElementExtended
+from adb import adb
+from utils import utils
+
+
+class AppiumExtended(AppiumIs, AppiumTap, AppiumSwipe, AppiumWait):
+    """
+    Класс работы с Appium.
+    Обеспечивает работу с устройством
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def __del__(self):
+        self.disconnect()
+
+    def get_element(self,
+                    locator: Union[Tuple, WebElementExtended, Dict[str, str], str] = None,
+                    by: Union[MobileBy, AppiumBy, By, str] = None,
+                    value: Union[str, Dict, None] = None,
+                    timeout_elem: int = 10,
+                    timeout_method: int = 600,
+                    elements_range: Union[Tuple, List[WebElementExtended], Dict[str, str], None] = None,
+                    contains: bool = True,
+                    ) -> Union[WebElementExtended, None]:
+        """
+        Получает элемент на странице, используя указанный локатор или параметры.
+
+        Аргументы:
+        - locator (Union[Tuple, WebElementExtended, Dict[str, str], str], optional):
+            Локатор или элемент для поиска. По умолчанию None.
+        - by (Union[MobileBy, AppiumBy, By, str], optional): Метод поиска элемента.
+            По умолчанию None.
+        - value (Union[str, Dict, None], optional): Значение для поиска элемента.
+            По умолчанию None.
+        - timeout_elem (int, optional): Время ожидания появления элемента.
+            По умолчанию 10.
+        - timeout_method (int, optional): Время ожидания выполнения метода.
+            По умолчанию 600.
+        - elements_range (Union[Tuple, List[WebElementExtended], Dict[str, str], None], optional):
+            Диапазон элементов для выбора. По умолчанию None.
+        - contains (bool, optional): Флаг, указывающий на необходимость использования частичного совпадения текста.
+            По умолчанию True.
+
+        Возвращает:
+        - Union[WebElementExtended, None]: Расширенный элемент WebElementExtended или None, если элемент не найден.
+        """
+        element = self._get_element(locator=locator,
+                                    by=by,
+                                    value=value,
+                                    timeout_elem=timeout_elem,
+                                    timeout_method=timeout_method,
+                                    elements_range=elements_range,
+                                    contains=contains)
+        return WebElementExtended(element.parent, element.id)
+
+    def get_elements(self,
+                     locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
+                     by: Union[MobileBy, AppiumBy, By, str] = None,
+                     value: Union[str, Dict, None] = None,
+                     timeout_elements: int = 10,
+                     timeout_method: int = 600,
+                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                     contains: bool = True,
+                     ) -> Union[List[WebElementExtended], List]:
+        """
+        Получает элементы на странице, используя указанный локатор или параметры.
+
+        Args:
+        - locator (Union[Tuple, List[WebElement], Dict[str, str], str], optional): Локатор или элементы для поиска.
+            По умолчанию None.
+        - by (Union[MobileBy, AppiumBy, By, str], optional): Метод поиска элементов.
+            По умолчанию None.
+        - value (Union[str, Dict, None], optional): Значение для поиска элементов.
+            По умолчанию None.
+        - timeout_elements (int, optional): Время ожидания появления элементов.
+            По умолчанию 10.
+        - timeout_method (int, optional): Время ожидания выполнения метода.
+            По умолчанию 600.
+        - elements_range (Union[Tuple, List[WebElement], Dict[str, str], None], optional): Диапазон элементов для выбора.
+            По умолчанию None.
+        - contains (bool, optional): Флаг, указывающий на необходимость использования частичного совпадения текста.
+            По умолчанию True.
+
+        Returns:
+        - Union[List[WebElementExtended], List]: Список расширенных элементов WebElementExtended или обычных элементов WebElement в случае ошибки.
+        """
+        elements = super()._get_elements(locator=locator,
+                                         by=by,
+                                         value=value,
+                                         timeout_elements=timeout_elements,
+                                         timeout_method=timeout_method,
+                                         elements_range=elements_range,
+                                         contains=contains)
+        elements_ext = []
+        for element in elements:
+            elements_ext.append(WebElementExtended(element.parent, element.id))
+        return elements_ext
+
+    def get_image_coordinates(self,
+                              image: Union[bytes, np.ndarray, Image.Image, str],
+                              full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                              threshold: float = 0.7,
+                              ) -> Union[Tuple, None]:
+        return self._get_image_coordinates(full_image=full_image,
+                                           image=image,
+                                           threshold=threshold)
+
+    def get_inner_image_coordinates(self,
+                                    outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                    inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                    threshold: Optional[float] = 0.9
+                                    ) -> Union[Tuple[int, int, int, int], None]:
+        """
+        Возвращает координаты x y (относительно экрана) по изображению внутри другого изображения
+        """
+        return self._get_inner_image_coordinates(outer_image_path=outer_image_path,
+                                                 inner_image_path=inner_image_path,
+                                                 threshold=threshold)
+
+    def get_many_coordinates_of_image(self,
+                                      image: Union[bytes, np.ndarray, Image.Image, str],
+                                      full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                                      cv_threshold: Optional[float] = 0.7,
+                                      coord_threshold: Optional[int] = 5,
+                                      ) -> Union[List[Tuple], None]:
+        return self.image.get_many_coordinates_of_image(full_image=full_image,
+                                                        image=image,
+                                                        cv_threshold=cv_threshold,
+                                                        coord_threshold=coord_threshold)
+
+    def get_text_coordinates(self,
+                             text: str,
+                             language: Optional[str] = 'rus',
+                             image: Union[bytes, str, Image.Image, np.ndarray] = None,
+                             ocr: Optional[bool] = True,
+                             ) -> Union[Tuple[int, int, int, int], None]:  # TODO реализовать None
+        """
+        # TODO fill
+        """
+        if ocr:
+            return self._get_text_coordinates(text=text, language=language, image=image)
+        else:
+            return self.get_element(locator={'text': text, 'displayed': 'true', 'enabled': 'true'}).get_coordinates()
+
+    # DOM
+
+    def get_element_contains(self,
+                             ) -> Any:
+        """
+        Возвращает элемент содержащий определенный элемент
+        """
+        raise NotImplementedError("This method is not implemented yet.")  # TODO implement
+
+    def get_elements_contains(self,
+                              ) -> Any:
+        """
+        Возвращает элементы содержащие определенный(е) элемент(ы)
+        """
+        raise NotImplementedError("This method is not implemented yet.")  # TODO implement
+
+    def get_screenshot_as_base64_decoded(self) -> bytes:
+        return self._get_screenshot_as_base64_decoded()
+
+    def find_and_get_element(self,
+                             locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+                             timeout: int = 10,
+                             ) -> Union[WebElementExtended, None]:
+        """
+        Ищет элемент на странице, если нет то скроллит все что скроллится и ищет там
+        """
+        if self.is_element_within_screen(locator=locator, timeout=1):
+            return self.get_element(locator=locator, timeout_elem=timeout)
+        recyclers = self.get_elements(locator={'scrollable': 'true', 'enabled': 'true', 'displayed': 'true'})
+        for recycler in recyclers:
+            try:
+                if recycler.scroll_until_find(locator=locator):
+                    return self.get_element(locator=locator, timeout_elem=timeout)
+            except StaleElementReferenceException as e:
+                print(e)
+                print("find_and_get_element StaleElementReferenceException")
+                print(f"{recycler=}")
+                print(f"{locator=}")
+        return None
+
+    def is_element_within_screen(self,
+                                 locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+                                 timeout: int = 10,
+                                 ) -> bool:
+        """
+        Метод проверяет, находится ли заданный элемент на видимом экране.
+
+        Аргументы:
+        - locator (Union[tuple, WebElement]): Локатор или элемент, который нужно проверить.
+        - timeout (int): Время ожидания элемента. Значение по умолчанию: 10.
+
+        Возвращает:
+        - bool: True, если элемент находится на экране, False, если нет.
+        """
+        return self._is_element_within_screen(locator=locator, timeout=timeout)
+
+    def is_text_on_screen(self,
+                          text: str,
+                          language: str = 'rus',
+                          ocr: bool = True,
+                          ) -> bool:
+        """
+        Проверяет, присутствует ли заданный текст на экране.
+        Если ocr=True:
+            Распознавание текста производит с помощью библиотеки pytesseract.
+        Если ocr=False:
+            Производится поиск элемента по xpath.
+
+        Аргументы:
+        - text (str): Текст, который нужно найти на экране.
+        - ocr (bool): Производить поиск по изображению или DOM.
+        - language (str): Язык распознавания текста. Значение по умолчанию: 'rus'.
+
+        Возвращает:
+        - bool: True, если заданный текст найден на экране. False в противном случае.
+        """
+        if ocr:
+            return self.image.is_text_on_ocr_screen(text=text, language=language)
+        else:
+            return self._is_element_within_screen(locator={'text': text})
+
+    def is_image_on_the_screen(self,
+                               image: Union[bytes, np.ndarray, Image.Image, str],
+                               threshold: float = 0.9,
+                               ) -> bool:
+        return self.image.is_image_on_the_screen(image=image,
+                                                 threshold=threshold)
+
+    def tap(self,
+            locator: Union[Tuple[str, str], WebElementExtended, WebElement, Dict[str, str], str] = None,
+            x: int = None,
+            y: int = None,
+            image: Union[bytes, np.ndarray, Image.Image, str] = None,
+            duration: Optional[int] = None,
+            timeout: int = 5,
+            ) -> Union['AppiumExtended', None]:
+        """
+        Тап по координатам / элементу / изображению
+        """
+        if locator is not None:
+            # Извлечение координат
+            x, y = self._extract_point_coordinates_by_typing(locator)
+        if image is not None:
+            start_time = time.time()
+            while not self.is_image_on_the_screen(image=image) and time.time() - start_time < timeout:
+                time.sleep(1)
+            # Извлечение координат
+            x, y = self._extract_point_coordinates_by_typing(image)
+
+        assert self._tap(x=x, y=y,
+                         duration=duration)
+        # Возвращаем экземпляр класса AppiumExtended
+        return cast('AppiumExtended', self)
+
+    # SWIPE
+
+    def swipe(self,
+              start_position: Union[
+                  Tuple[int, int], str, bytes, np.ndarray, Image.Image, WebElement, WebElementExtended, Tuple[str, str],
+                  Dict[str, str]],
+              end_position: Optional[Union[
+                  Tuple[int, int], str, bytes, np.ndarray, Image.Image, WebElement, WebElementExtended, Tuple[str, str],
+                  Dict[str, str]]] = None,
+              direction: Optional[int] = None,
+              distance: Optional[int] = None,
+              duration: Optional[int] = 0,
+              ) -> 'AppiumExtended':
+        """
+        Выполняет свайп (перетаскивание) элемента или изображения на экране.
+
+        Параметры:
+        - start_position: Позиция начала свайпа. Может быть задана в различных форматах:
+            - Если `start_position` является кортежем и оба его элемента являются строками, то он представляет собой
+              локатор элемента. В этом случае будет выполнен поиск элемента и используется его позиция.
+            - Если `start_position` является словарем, то считается, что это локатор элемента, основанный на атрибутах.
+              Например, {'text': 'some text'} или {'class': 'SomeClass', 'visible': 'true'}. В этом случае будет
+              выполнен поиск элемента по указанным атрибутам, и используется его позиция.
+            - Если `start_position` является экземпляром класса WebElement или WebElementExtended, то используется его
+              позиция.
+            - Если `start_position` является строкой, массивом байтов (bytes), массивом NumPy (np.ndarray) или объектом
+              класса Image.Image, то считается, что это изображение. В этом случае будет вычислен центр изображения и
+              используется его позиция.
+            - Если `start_position` является кортежем, и оба его элемента являются целыми числами, то считается, что это
+              координаты в формате (x_coordinate, y_coordinate).
+
+        - end_position: Позиция конца свайпа. Принимает те же форматы, что и `start_position`. По умолчанию None.
+        - direction (опционально): Направление свайпа. Принимает значения от 0 до 360 градусов.
+          Если указано направление, то будет вычислена конечная точка свайпа на основе текущего размера окна и
+          указанного расстояния. По умолчанию None.
+        - distance (опционально): Расстояние свайпа. Принимается в пикселях. Используется только в сочетании с параметром
+          `direction`. По умолчанию None.
+        - duration (опционально): Продолжительность свайпа в миллисекундах. По умолчанию 0.
+
+        Возвращает:
+        - self: Экземпляр класса AppiumExtended.
+
+        Примечания:
+        - В качестве конечной позиции свайпа должен быть указан end_position или пара direction, distance.
+        - str принимается как путь к изображению на экране и вычисляется его центр, а не как локатор элемента
+
+        """
+        # Извлечение координат начальной точки свайпа
+        start_x, start_y = self._extract_point_coordinates_by_typing(start_position)
+
+        if end_position is not None:
+            # Извлечение координат конечной точки свайпа
+            end_x, end_y = self._extract_point_coordinates_by_typing(end_position)
+        else:
+            # Извлечение координат конечной точки свайпа на основе направления и расстояния
+            end_x, end_y = self._extract_point_coordinates_by_direction(direction, distance, start_x, start_y)
+
+        # Выполнение свайпа
+        assert self._swipe(start_x=start_x, start_y=start_y,
+                           end_x=end_x, end_y=end_y,
+                           duration=duration)
+
+        # Возвращаем экземпляр класса AppiumExtended
+        return cast('AppiumExtended', self)
+
+    def swipe_right_to_left(self):
+        window_size = adb.get_screen_resolution()
+        width = window_size[0]
+        height = window_size[1]
+        left = int(width * 0.1)
+        right = int(width * 0.9)
+        self.swipe(start_position=(right, height // 2),
+                   end_position=(left, height // 2))
+
+    def swipe_left_to_right(self):
+        window_size = adb.get_screen_resolution()
+        width = window_size[0]
+        height = window_size[1]
+        left = int(width * 0.1)
+        right = int(width * 0.9)
+        self.swipe(start_position=(left, height // 2),
+                   end_position=(right, height // 2))
+
+    def swipe_top_to_bottom(self):
+        window_size = adb.get_screen_resolution()
+        height = window_size[1]
+        top = int(height * 0.1)
+        bottom = int(height * 0.9)
+        self.swipe(start_position=(top, height // 2),
+                   end_position=(bottom, height // 2))
+
+    def swipe_bottom_to_top(self):
+        window_size = adb.get_screen_resolution()
+        height = window_size[1]
+        top = int(height * 0.1)
+        bottom = int(height * 0.9)
+        self.swipe(start_position=(bottom, height // 2),
+                   end_position=(top, height // 2))
+
+    # WAIT
+
+    def wait_for(self,
+                 locator: Union[Tuple[str, str], WebElement, 'WebElementExtended', Dict[str, str], str,
+                 List[Tuple[str, str]], List[WebElement], List['WebElementExtended'], List[Dict[str, str]], List[
+                     str]] = None,
+                 image: Union[bytes, np.ndarray, Image.Image, str,
+                 List[bytes], List[np.ndarray], List[Image.Image], List[str]] = None,
+                 timeout: int = 10,
+                 contains: bool = True,
+                 full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                 ):
+        return self._wait_for(locator=locator,
+                              image=image,
+                              timeout=timeout,
+                              contains=contains)
+
+    def wait_for_not(self,
+                     locator: Union[Tuple[str, str], WebElement, 'WebElementExtended', Dict[str, str], str,
+                     List[Tuple[str, str]], List[WebElement], List['WebElementExtended'], List[Dict[str, str]], List[
+                         str]] = None,
+                     image: Union[bytes, np.ndarray, Image.Image, str,
+                     List[bytes], List[np.ndarray], List[Image.Image], List[str]] = None,
+                     timeout: int = 10,
+                     contains: bool = True,
+                     ):
+        return self._wait_for_not(locator=locator, image=image, timeout=timeout, contains=contains)
+
+    def wait_return_true(self, method, timeout: int = 10):
+        return self._wait_return_true(method=method, timeout=timeout)
+
+    # KEYBOARD
+
+    def input_by_virtual_keyboard(self) -> 'AppiumExtended':  # TODO реализовать возврат cast('AppiumExtended', self)
+        """
+        Вводит с помощью виртуально клавиатуры
+        """
+        raise NotImplementedError("This method is not implemented yet.")
+
+    # OTHER
+
+    def draw_by_coordinates(self,
+                            image: Union[bytes, str, Image.Image, np.ndarray] = None,
+                            coordinates: Tuple[int, int, int, int] = None,
+                            top_left: Tuple[int, int] = None,
+                            bottom_right: Tuple[int, int] = None,
+                            path: str = None,
+                            ) -> 'AppiumExtended':
+        assert self.image.draw_by_coordinates(image=image,
+                                              coordinates=coordinates,
+                                              top_left=top_left,
+                                              bottom_right=bottom_right,
+                                              path=path)
+        return cast('AppiumExtended', self)
+
+    # PRIVATE
+
+    def _extract_point_coordinates_by_typing(self,
+                                             position:
+                                             Union[Tuple[int, int], str, bytes, np.ndarray, Image.Image,
+                                             Tuple[str, str], Dict, WebElement, WebElementExtended]
+                                             ) -> Tuple[int, int]:
+        """
+        Извлекает координаты точки на основе типа переданной позиции.
+
+        Параметры:
+            position (
+            Union[Tuple[int, int], str, bytes, np.ndarray, Image.Image, Dict, WebElement, WebElementExtended]
+            ):
+                Позиция, для которой нужно извлечь координаты.
+                Либо локатор элемента, либо изображение, либо кортеж из координат.
+
+        Возвращает:
+            Tuple[int, int]: Кортеж координат точки, в формате (x, y).
+        """
+        x, y = 0, 0
+        # Вычисление позиции начала свайпа
+        if (isinstance(position, Tuple) and
+                isinstance(position[0], int) and
+                isinstance(position[1], int)):
+            # Если position является кортежем с двумя целыми числами, то считаем, что это координаты
+            x, y = position
+        elif (isinstance(position, Tuple) and
+              isinstance(position[0], str) and
+              isinstance(position[1], str)) or \
+                isinstance(position, WebElement) or \
+                isinstance(position, WebElementExtended) or \
+                isinstance(position, Dict):
+            # Если position является кортежем с двумя строковыми элементами или экземпляром WebElement,
+            # WebElementExtended или словарем, то получаем координаты центра элемента
+            x, y = utils.calculate_center_of_coordinates(
+                self.get_element(locator=position).get_coordinates())
+        elif isinstance(position, (bytes, np.ndarray, Image.Image, str)):
+            # Если position является строкой, байтами, массивом NumPy или объектом Image.Image,
+            # то получаем координаты центра изображения
+            x, y = utils.calculate_center_of_coordinates(
+                self.get_image_coordinates(image=position))
+        return x, y
+
+    def _extract_point_coordinates_by_direction(self,
+                                                direction: int, distance: int,
+                                                start_x: int, start_y: int
+                                                ) -> Tuple[int, int]:
+        """
+        Извлекает координаты точки на заданном расстоянии и в заданном направлении относительно начальных координат.
+
+        Параметры:
+            direction (str): Направление движения в пределах 360 градусов.
+            distance (int): Расстояние, на которое нужно переместиться относительно начальных координат в пикселях.
+            start_x (int): Начальная координата X.
+            start_y (int): Начальная координата Y.
+
+        Возвращает:
+            Tuple[int, int]: Координаты конечной точки в формате (x, y).
+        """
+        window_size = adb.get_screen_resolution()
+        width = window_size[0]
+        height = window_size[1]
+        end_x, end_y = utils.find_coordinates_by_vector(width=width, height=height,
+                                                        direction=direction, distance=distance,
+                                                        start_x=start_x, start_y=start_y)
+        return end_x, end_y
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_get.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_get.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-# coding: utf-8
-import time
-from typing import Union, Dict, List, Tuple
-
-import numpy as np
-from PIL import Image
-from appium.webdriver import WebElement
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.common.exceptions import WebDriverException, TimeoutException, NoSuchElementException
-from selenium.webdriver.support.wait import WebDriverWait
-from appium.webdriver.common.mobileby import MobileBy
-from appium.webdriver.common.appiumby import AppiumBy
-from selenium.webdriver.common.by import By
-
-from AppiumExtended.appium_base import AppiumBase
-from AppiumHelpers.appium_helpers import AppiumHelpers
-
-
-class AppiumGet(AppiumBase):
-    """
-    Класс расширяющий Appium.
-    Обеспечивает получение чего-либо со страницы.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.helper = None
-
-    def _get_element(self,
-                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                     by: Union[MobileBy, AppiumBy, By, str] = None,
-                     value: Union[str, Dict, None] = None,
-                     timeout_elem: int = 10,
-                     timeout_method: int = 600,
-                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                     contains: bool = False
-                     ) -> \
-            Union[WebElement, None]:
-        """
-        Метод обеспечивает поиск элемента в текущей DOM структуре.
-        Должен принимать либо локатор, либо значения by и value.
-
-        Usage:
-            element = app._get_element(locator=("id", "foo")).
-            element = app._get_element(element).
-            element = app._get_element(locator={'text': 'foo'}).
-            element = app._get_element(locator='/path/to/file/pay_agent.png').
-            element = app._get_element(locator=part_image, elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'}).
-            element = app._get_element(by="id", value="ru.sigma.app.debug:id/backButton").
-            element = app._get_element(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
-            element = app._get_element(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
-            element = app._get_element(by=By.ID, value="ru.sigma.app.debug:id/backButton").
-
-        Args:
-            locator: tuple / WebElement / dict / str, определяет локатор элемента.
-                tuple - локатор в виде ('атрибут', 'значение')
-                WebElement - объект веб элемента
-                dict - словарь, содержащий пары атрибут: значение
-                str - путь до файла с изображением элемента.
-            by: MobileBy, AppiumBy, By, str, тип локатора для поиска элемента (всегда в связке с value)
-            value: str, dict, None, значение локатора или словарь аргументов, если используется AppiumBy.XPATH.
-            timeout_elem: int, время ожидания элемента.
-            timeout_method: int, время ожидания метода поиска элемента.
-            elements_range: tuple, list, dict, None, ограничивает поиск элемента в указанном диапазоне
-            (для поиска по изображению).
-            contains: для поиска по dict, ищет элемент содержащий фрагмент значения
-
-        Returns:
-            WebElement или None, если элемент не был найден.
-        """
-        # Проверка и подготовка аргументов
-        if (not locator) and (not by or not value):
-            self.logger.error(f"Некорректные аргументы!\n"
-                              f"{locator=}\n"
-                              f"{by=}\n"
-                              f"{value=}\n"
-                              f"{timeout_elem=}\n")
-            return None
-        if not locator and (by and value):
-            locator = (by, value)
-        if locator is None:
-            return None
-
-        # Объявление стратегии поиска элементов
-        self.helper = AppiumHelpers(driver=self.driver)
-
-        locator_handler = {
-            # возвращает себя же
-            WebElement: self.helper.handle_webelement_locator,
-            # возвращает себя же
-            'WebElementExtended': self.helper.handle_webelement_locator,
-            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
-            dict: self.helper.handle_dict_locator,
-            # производит поиск элементов по фрагменту изображения, возвращает список элементов
-            str: self.helper.handle_string_locator,
-        }
-
-        # Цикл подготовки локатора и поиска элементов
-        start_time = time.time()
-        while not isinstance(locator, WebElement) and time.time() - start_time < timeout_method:
-            # Выявление типа данных локатора для его подготовки
-            locator_type = type(locator)
-            # Если локатор типа tuple, то выполняется извлечение элементов
-            if isinstance(locator, tuple):
-                wait = WebDriverWait(driver=self.driver, timeout=timeout_elem)
-                try:
-                    element = wait.until(EC.presence_of_element_located(locator))
-                    return element
-                except NoSuchElementException:
-                    return None
-                except TimeoutException:
-                    # self.logger.error(f"Элемент не обнаружен!\n"
-                    #                   f"{locator=}\n"
-                    #                   f"{timeout_elem=}\n\n" +
-                    #                   "{}\n".format(e))
-                    # self.logger.error("page source ", self.driver.page_source)
-                    return None
-                except WebDriverException:
-                    # self.logger.error(f"Элемент не обнаружен!\n"
-                    #                   f"{locator=}\n"
-                    #                   f"{timeout_elem=}\n\n" +
-                    #                   "{}\n".format(e))
-                    # self.logger.error("page source ", self.driver.page_source)
-                    return None
-            # Выполнение подготовки локатора
-            handler = locator_handler.get(locator_type)
-            if locator is None:
-                return None
-            locator = handler(locator=locator, timeout=timeout_elem, elements_range=elements_range, contains=contains)
-        # Подбирает результат после поиска по изображению
-        if isinstance(locator, WebElement):
-            return locator
-        self.logger.error(f"Что-то пошло не так\n"
-                          f"{locator=}\n"
-                          f"{by=}\n"
-                          f"{value=}\n"
-                          f"{timeout_elem=}\n"
-                          f"{timeout_method=}\n")
-        return None
-
-    def _get_elements(self,
-                      locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
-                      by: Union[MobileBy, AppiumBy, By, str] = None,
-                      value: Union[str, Dict, None] = None,
-                      timeout_elements: int = 10,
-                      timeout_method: int = 600,
-                      elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                      contains: bool = True) -> \
-            Union[List[WebElement], None]:
-        """
-        Метод обеспечивает поиск элементов в текущей DOM структуре.
-        Должен принять либо локатор, либо by и value.
-        При locator:str настоятельно рекомендуется использовать диапазон поиска elements_range.
-
-        Usage:
-            elements = app.get_elements(locator=("id", "foo")).
-            elements = app.get_elements(locator={'text': 'foo'}).
-            elements = app.get_elements(locator='/path/to/file/pay_agent.png').
-            elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=By.ID, value="ru.sigma.app.debug:id/backButton").
-
-        Args:
-            locator: tuple or WebElement or Dict[str, str], str, локатор tuple или Веб Элемент или словарь {'атрибут': 'значение'} или str как путь до файла с изображением элемента.
-            by:[MobileBy, AppiumBy, By, str], тип локатора для поиска элемента (всегда в связке с value)
-            value: Union[str, Dict, None], значение локатора или словарь аргументов, если используется AppiumBy.XPATH
-            timeout_elements: #TODO fill me
-            timeout_method: #TODO fill me
-            elements_range: #TODO fill me
-
-        Returns:
-            Список WebElement'ов, или пустой список в случае их отсутствия.
-        """
-        # Проверка и подготовка аргументов
-        if not locator and (not by or not value):
-            self.logger.error(f"Некорректные аргументы!\n"
-                              f"{locator=}\n"
-                              f"{by=}\n"
-                              f"{value=}\n"
-                              f"{timeout_elements=}\n"
-                              f"{timeout_method=}\n")
-            return None
-        if not locator and (by and value):
-            locator = (by, value)
-        if locator is None:
-            return None
-
-        # Объявление стратегии поиска элементов
-        self.helper = AppiumHelpers(driver=self.driver)
-        locator_handler = {
-            # подразумевается список элементов, возвращает себя же
-            list: self.helper.handle_webelement_locator_elements,
-            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
-            dict: self.helper.handle_dict_locator_elements,
-            # производит поиск элементов по фрагменту изображения, возвращает список элементов
-            str: self.helper.handle_string_locator_elements,
-        }
-
-        # Цикл подготовки локатора и поиска элементов
-        start_time = time.time()
-        while not isinstance(locator, list) and time.time() - start_time < timeout_method:
-            # Выявление типа данных локатора для его подготовки
-            locator_type = type(locator)
-            # Если локатор типа tuple, то выполняется извлечение элементов
-            if isinstance(locator, tuple):
-                wait = WebDriverWait(driver=self.driver, timeout=timeout_elements)
-                try:
-                    element = wait.until(EC.presence_of_all_elements_located(locator))
-                    return element
-                except WebDriverException:
-                    # self.logger.error(f"Элемент не обнаружен!\n"
-                    #                   f"{locator=}\n"
-                    #                   f"{by=}\n"
-                    #                   f"{value=}\n"
-                    #                   f"{timeout_elements=}\n"
-                    #                   f"{timeout_method=}\n\n" +
-                    #                   "{}\n".format(e))
-                    return None
-            # Выполнение подготовки локатора
-            handler = locator_handler.get(locator_type)
-            locator = handler(locator=locator,
-                              timeout=timeout_elements,
-                              elements_range=elements_range,
-                              contains=contains)
-        # Подбирает результат после поиска по изображению
-        if isinstance(locator, list):
-            return locator
-        self.logger.error(f"\nЧто-то пошло не так\n"
-                          f"{locator=}\n"
-                          f"{by=}\n"
-                          f"{value=}\n"
-                          f"{timeout_elements=}\n"
-                          f"{timeout_method=}\n")
-        return None
-
-    def _get_image_coordinates(self,
-                               image: Union[bytes, np.ndarray, Image.Image, str],
-                               full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                               threshold: float = 0.7,
-                               ) -> Union[Tuple[int, int, int, int], None]:
-        return self.image.get_image_coordinates(image=image, full_image=full_image, threshold=threshold)
-
-    def _get_inner_image_coordinates(self,
-                                     outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                     inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                     threshold: float = 0.9) -> \
-            Union[Tuple[int, int, int, int], None]:
-        return self.image.get_inner_image_coordinates(outer_image_path=outer_image_path,
-                                                      inner_image_path=inner_image_path,
-                                                      threshold=threshold)
-
-    def _get_text_coordinates(self,
-                              text: str,
-                              language: str = 'rus',
-                              image: Union[bytes, str, Image.Image, np.ndarray] = None, ) -> Tuple[int, int, int, int]:
-        return self.image.get_text_coordinates(text=text, language=language, image=image)
-
-    def _get_screenshot_as_base64_decoded(self):
-        return self.image.get_screenshot_as_base64_decoded()
+# coding: utf-8
+import time
+from typing import Union, Dict, List, Tuple
+
+import numpy as np
+from PIL import Image
+from appium.webdriver import WebElement
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.common.exceptions import WebDriverException, TimeoutException, NoSuchElementException
+from selenium.webdriver.support.wait import WebDriverWait
+from appium.webdriver.common.mobileby import MobileBy
+from appium.webdriver.common.appiumby import AppiumBy
+from selenium.webdriver.common.by import By
+
+from AppiumExtended.appium_base import AppiumBase
+from AppiumHelpers.appium_helpers import AppiumHelpers
+
+
+class AppiumGet(AppiumBase):
+    """
+    Класс расширяющий Appium.
+    Обеспечивает получение чего-либо со страницы.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.helper = None
+
+    def _get_element(self,
+                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                     by: Union[MobileBy, AppiumBy, By, str] = None,
+                     value: Union[str, Dict, None] = None,
+                     timeout_elem: int = 10,
+                     timeout_method: int = 600,
+                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                     contains: bool = False
+                     ) -> \
+            Union[WebElement, None]:
+        """
+        Метод обеспечивает поиск элемента в текущей DOM структуре.
+        Должен принимать либо локатор, либо значения by и value.
+
+        Usage:
+            element = app._get_element(locator=("id", "foo")).
+            element = app._get_element(element).
+            element = app._get_element(locator={'text': 'foo'}).
+            element = app._get_element(locator='/path/to/file/pay_agent.png').
+            element = app._get_element(locator=part_image, elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'}).
+            element = app._get_element(by="id", value="ru.sigma.app.debug:id/backButton").
+            element = app._get_element(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
+            element = app._get_element(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
+            element = app._get_element(by=By.ID, value="ru.sigma.app.debug:id/backButton").
+
+        Args:
+            locator: tuple / WebElement / dict / str, определяет локатор элемента.
+                tuple - локатор в виде ('атрибут', 'значение')
+                WebElement - объект веб элемента
+                dict - словарь, содержащий пары атрибут: значение
+                str - путь до файла с изображением элемента.
+            by: MobileBy, AppiumBy, By, str, тип локатора для поиска элемента (всегда в связке с value)
+            value: str, dict, None, значение локатора или словарь аргументов, если используется AppiumBy.XPATH.
+            timeout_elem: int, время ожидания элемента.
+            timeout_method: int, время ожидания метода поиска элемента.
+            elements_range: tuple, list, dict, None, ограничивает поиск элемента в указанном диапазоне
+            (для поиска по изображению).
+            contains: для поиска по dict, ищет элемент содержащий фрагмент значения
+
+        Returns:
+            WebElement или None, если элемент не был найден.
+        """
+        # Проверка и подготовка аргументов
+        if (not locator) and (not by or not value):
+            self.logger.error(f"Некорректные аргументы!\n"
+                              f"{locator=}\n"
+                              f"{by=}\n"
+                              f"{value=}\n"
+                              f"{timeout_elem=}\n")
+            return None
+        if not locator and (by and value):
+            locator = (by, value)
+        if locator is None:
+            return None
+
+        # Объявление стратегии поиска элементов
+        self.helper = AppiumHelpers(driver=self.driver)
+
+        locator_handler = {
+            # возвращает себя же
+            WebElement: self.helper.handle_webelement_locator,
+            # возвращает себя же
+            'WebElementExtended': self.helper.handle_webelement_locator,
+            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
+            dict: self.helper.handle_dict_locator,
+            # производит поиск элементов по фрагменту изображения, возвращает список элементов
+            str: self.helper.handle_string_locator,
+        }
+
+        # Цикл подготовки локатора и поиска элементов
+        start_time = time.time()
+        while not isinstance(locator, WebElement) and time.time() - start_time < timeout_method:
+            # Выявление типа данных локатора для его подготовки
+            locator_type = type(locator)
+            # Если локатор типа tuple, то выполняется извлечение элементов
+            if isinstance(locator, tuple):
+                wait = WebDriverWait(driver=self.driver, timeout=timeout_elem)
+                try:
+                    element = wait.until(EC.presence_of_element_located(locator))
+                    return element
+                except NoSuchElementException:
+                    return None
+                except TimeoutException:
+                    # self.logger.error(f"Элемент не обнаружен!\n"
+                    #                   f"{locator=}\n"
+                    #                   f"{timeout_elem=}\n\n" +
+                    #                   "{}\n".format(e))
+                    # self.logger.error("page source ", self.driver.page_source)
+                    return None
+                except WebDriverException:
+                    # self.logger.error(f"Элемент не обнаружен!\n"
+                    #                   f"{locator=}\n"
+                    #                   f"{timeout_elem=}\n\n" +
+                    #                   "{}\n".format(e))
+                    # self.logger.error("page source ", self.driver.page_source)
+                    return None
+            # Выполнение подготовки локатора
+            handler = locator_handler.get(locator_type)
+            if locator is None:
+                return None
+            locator = handler(locator=locator, timeout=timeout_elem, elements_range=elements_range, contains=contains)
+        # Подбирает результат после поиска по изображению
+        if isinstance(locator, WebElement):
+            return locator
+        self.logger.error(f"Что-то пошло не так\n"
+                          f"{locator=}\n"
+                          f"{by=}\n"
+                          f"{value=}\n"
+                          f"{timeout_elem=}\n"
+                          f"{timeout_method=}\n")
+        return None
+
+    def _get_elements(self,
+                      locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
+                      by: Union[MobileBy, AppiumBy, By, str] = None,
+                      value: Union[str, Dict, None] = None,
+                      timeout_elements: int = 10,
+                      timeout_method: int = 600,
+                      elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                      contains: bool = True) -> \
+            Union[List[WebElement], None]:
+        """
+        Метод обеспечивает поиск элементов в текущей DOM структуре.
+        Должен принять либо локатор, либо by и value.
+        При locator:str настоятельно рекомендуется использовать диапазон поиска elements_range.
+
+        Usage:
+            elements = app.get_elements(locator=("id", "foo")).
+            elements = app.get_elements(locator={'text': 'foo'}).
+            elements = app.get_elements(locator='/path/to/file/pay_agent.png').
+            elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=By.ID, value="ru.sigma.app.debug:id/backButton").
+
+        Args:
+            locator: tuple or WebElement or Dict[str, str], str, локатор tuple или Веб Элемент или словарь {'атрибут': 'значение'} или str как путь до файла с изображением элемента.
+            by:[MobileBy, AppiumBy, By, str], тип локатора для поиска элемента (всегда в связке с value)
+            value: Union[str, Dict, None], значение локатора или словарь аргументов, если используется AppiumBy.XPATH
+            timeout_elements: #TODO fill me
+            timeout_method: #TODO fill me
+            elements_range: #TODO fill me
+
+        Returns:
+            Список WebElement'ов, или пустой список в случае их отсутствия.
+        """
+        # Проверка и подготовка аргументов
+        if not locator and (not by or not value):
+            self.logger.error(f"Некорректные аргументы!\n"
+                              f"{locator=}\n"
+                              f"{by=}\n"
+                              f"{value=}\n"
+                              f"{timeout_elements=}\n"
+                              f"{timeout_method=}\n")
+            return None
+        if not locator and (by and value):
+            locator = (by, value)
+        if locator is None:
+            return None
+
+        # Объявление стратегии поиска элементов
+        self.helper = AppiumHelpers(driver=self.driver)
+        locator_handler = {
+            # подразумевается список элементов, возвращает себя же
+            list: self.helper.handle_webelement_locator_elements,
+            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
+            dict: self.helper.handle_dict_locator_elements,
+            # производит поиск элементов по фрагменту изображения, возвращает список элементов
+            str: self.helper.handle_string_locator_elements,
+        }
+
+        # Цикл подготовки локатора и поиска элементов
+        start_time = time.time()
+        while not isinstance(locator, list) and time.time() - start_time < timeout_method:
+            # Выявление типа данных локатора для его подготовки
+            locator_type = type(locator)
+            # Если локатор типа tuple, то выполняется извлечение элементов
+            if isinstance(locator, tuple):
+                wait = WebDriverWait(driver=self.driver, timeout=timeout_elements)
+                try:
+                    element = wait.until(EC.presence_of_all_elements_located(locator))
+                    return element
+                except WebDriverException:
+                    # self.logger.error(f"Элемент не обнаружен!\n"
+                    #                   f"{locator=}\n"
+                    #                   f"{by=}\n"
+                    #                   f"{value=}\n"
+                    #                   f"{timeout_elements=}\n"
+                    #                   f"{timeout_method=}\n\n" +
+                    #                   "{}\n".format(e))
+                    return None
+            # Выполнение подготовки локатора
+            handler = locator_handler.get(locator_type)
+            locator = handler(locator=locator,
+                              timeout=timeout_elements,
+                              elements_range=elements_range,
+                              contains=contains)
+        # Подбирает результат после поиска по изображению
+        if isinstance(locator, list):
+            return locator
+        self.logger.error(f"\nЧто-то пошло не так\n"
+                          f"{locator=}\n"
+                          f"{by=}\n"
+                          f"{value=}\n"
+                          f"{timeout_elements=}\n"
+                          f"{timeout_method=}\n")
+        return None
+
+    def _get_image_coordinates(self,
+                               image: Union[bytes, np.ndarray, Image.Image, str],
+                               full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                               threshold: float = 0.7,
+                               ) -> Union[Tuple[int, int, int, int], None]:
+        return self.image.get_image_coordinates(image=image, full_image=full_image, threshold=threshold)
+
+    def _get_inner_image_coordinates(self,
+                                     outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                     inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                     threshold: float = 0.9) -> \
+            Union[Tuple[int, int, int, int], None]:
+        return self.image.get_inner_image_coordinates(outer_image_path=outer_image_path,
+                                                      inner_image_path=inner_image_path,
+                                                      threshold=threshold)
+
+    def _get_text_coordinates(self,
+                              text: str,
+                              language: str = 'rus',
+                              image: Union[bytes, str, Image.Image, np.ndarray] = None, ) -> Tuple[int, int, int, int]:
+        return self.image.get_text_coordinates(text=text, language=language, image=image)
+
+    def _get_screenshot_as_base64_decoded(self):
+        return self.image.get_screenshot_as_base64_decoded()
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_is.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_is.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# coding: utf-8
-from typing import Union, Dict, Tuple
-
-from appium.webdriver import WebElement
-
-from AppiumExtended.appium_get import AppiumGet
-from adb import adb
-
-
-class AppiumIs(AppiumGet):
-    """
-    Класс расширяющий Appium.
-    Обеспечивает ....
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.helper = None
-
-
-    def _is_element_within_screen(
-            self,
-            locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-            timeout: int = 10
-    ) -> bool:
-        """
-        Метод проверяет, находится ли заданный элемент на видимом экране.
-
-        Аргументы:
-        - locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]):
-            Локатор или элемент, который нужно проверить.
-        - timeout (int): Время ожидания элемента. Значение по умолчанию: 10.
-
-        Возвращает:
-        - bool: True, если элемент находится на экране, False, если нет.
-        """
-        screen_size = adb.get_screen_resolution()  # Получаем размеры экрана
-        screen_width = screen_size[0]  # Ширина экрана
-        screen_height = screen_size[1]  # Высота экрана
-        element = self._get_element(locator=locator, timeout_elem=timeout)  # Получаем элемент по локатору
-        if element is None:
-            return False
-        if not element.get_attribute('displayed') == 'true':
-            # Если элемент не отображается на экране
-            return False
-        element_location = element.location  # Получаем координаты элемента
-        element_size = element.size  # Получаем размеры элемента
-        if (
-                element_location['y'] + element_size['height'] > screen_height or
-                element_location['x'] + element_size['width'] > screen_width or
-                element_location['y'] < 0 or
-                element_location['x'] < 0
-        ):
-            # Если элемент находится за пределами экрана
-            return False
-        # Если элемент находится на экране
-        return True
-
-
+# coding: utf-8
+from typing import Union, Dict, Tuple
+
+from appium.webdriver import WebElement
+
+from AppiumExtended.appium_get import AppiumGet
+from adb import adb
+
+
+class AppiumIs(AppiumGet):
+    """
+    Класс расширяющий Appium.
+    Обеспечивает ....
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.helper = None
+
+
+    def _is_element_within_screen(
+            self,
+            locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+            timeout: int = 10
+    ) -> bool:
+        """
+        Метод проверяет, находится ли заданный элемент на видимом экране.
+
+        Аргументы:
+        - locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]):
+            Локатор или элемент, который нужно проверить.
+        - timeout (int): Время ожидания элемента. Значение по умолчанию: 10.
+
+        Возвращает:
+        - bool: True, если элемент находится на экране, False, если нет.
+        """
+        screen_size = adb.get_screen_resolution()  # Получаем размеры экрана
+        screen_width = screen_size[0]  # Ширина экрана
+        screen_height = screen_size[1]  # Высота экрана
+        element = self._get_element(locator=locator, timeout_elem=timeout)  # Получаем элемент по локатору
+        if element is None:
+            return False
+        if not element.get_attribute('displayed') == 'true':
+            # Если элемент не отображается на экране
+            return False
+        element_location = element.location  # Получаем координаты элемента
+        element_size = element.size  # Получаем размеры элемента
+        if (
+                element_location['y'] + element_size['height'] > screen_height or
+                element_location['x'] + element_size['width'] > screen_width or
+                element_location['y'] < 0 or
+                element_location['x'] < 0
+        ):
+            # Если элемент находится за пределами экрана
+            return False
+        # Если элемент находится на экране
+        return True
+
+
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_swipe.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# coding: utf-8
-from selenium.common import WebDriverException
-from AppiumExtended.appium_get import AppiumGet
-
-
-class AppiumSwipe(AppiumGet):
-    """
-    Класс работы с Appium.
-    Обеспечивает swipe
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.helper = None
-
-    def _swipe(self,
-               start_x: int,
-               start_y: int,
-               end_x: int,
-               end_y: int,
-               duration: int = 0) -> bool:
-        """
-        Выполняет свайп на элементе.
-
-        Аргументы:
-        - start_x (int): Координата x начальной точки свайпа.
-        - start_y (int): Координата y начальной точки свайпа.
-        - end_x (int): Координата x конечной точки свайпа.
-        - end_y (int): Координата y конечной точки свайпа.
-        - duration (int, optional): Продолжительность свайпа в миллисекундах.
-
-        Возвращает:
-        - bool: True, если свайп выполнен успешно, False в случае исключения.
-
-        Исключения:
-        - WebDriverException: Если происходит ошибка при выполнении свайпа.
-
-        Примечание:
-        - Метод использует экземпляр драйвера self.driver для выполнения свайпа.
-        """
-        try:
-            self.driver.swipe(start_x=start_x, start_y=start_y,
-                              end_x=end_x, end_y=end_y,
-                              duration=duration)
-        except WebDriverException as e:
-            self.logger.error(f"Исключение в методе _swipe(). Аргументы:\n"
-                              f"start_x={start_x}\n"
-                              f"start_y={start_y}\n"
-                              f"end_x={end_x}\n"
-                              f"end_y={end_y}\n"
-                              f"duration={duration}")
-            self.logger.exception(e)
-            return False
-
-        return True
-
+# coding: utf-8
+from selenium.common import WebDriverException
+from AppiumExtended.appium_get import AppiumGet
+
+
+class AppiumSwipe(AppiumGet):
+    """
+    Класс работы с Appium.
+    Обеспечивает swipe
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.helper = None
+
+    def _swipe(self,
+               start_x: int,
+               start_y: int,
+               end_x: int,
+               end_y: int,
+               duration: int = 0) -> bool:
+        """
+        Выполняет свайп на элементе.
+
+        Аргументы:
+        - start_x (int): Координата x начальной точки свайпа.
+        - start_y (int): Координата y начальной точки свайпа.
+        - end_x (int): Координата x конечной точки свайпа.
+        - end_y (int): Координата y конечной точки свайпа.
+        - duration (int, optional): Продолжительность свайпа в миллисекундах.
+
+        Возвращает:
+        - bool: True, если свайп выполнен успешно, False в случае исключения.
+
+        Исключения:
+        - WebDriverException: Если происходит ошибка при выполнении свайпа.
+
+        Примечание:
+        - Метод использует экземпляр драйвера self.driver для выполнения свайпа.
+        """
+        try:
+            self.driver.swipe(start_x=start_x, start_y=start_y,
+                              end_x=end_x, end_y=end_y,
+                              duration=duration)
+        except WebDriverException as e:
+            self.logger.error(f"Исключение в методе _swipe(). Аргументы:\n"
+                              f"start_x={start_x}\n"
+                              f"start_y={start_y}\n"
+                              f"end_x={end_x}\n"
+                              f"end_y={end_y}\n"
+                              f"duration={duration}")
+            self.logger.exception(e)
+            return False
+
+        return True
+
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended/appium_tap.py` & `AppiumExtended-0.1.6/AppiumExtended/appium_tap.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# coding: utf-8
-from typing import Optional
-
-from selenium.common import WebDriverException
-
-from AppiumExtended.appium_get import AppiumGet
-
-
-class AppiumTap(AppiumGet):
-    """
-    Класс работы с Appium.
-    Обеспечивает tap
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.helper = None
-
-    def _tap(self,
-             x: int,
-             y: int,
-             duration: Optional[int] = None,
-             ) -> bool:
-        """
-        Выполняет касание на экране устройства в указанных координатах (x, y) или на основе изображения.
-
-        Аргументы:
-        - x (int): Горизонтальная координата X точки касания на экране устройства.
-        - y (int): Вертикальная координата Y точки касания на экране устройства.
-        - duration (Optional[int]): Длительность касания в миллисекундах (по умолчанию None).
-
-        Возвращает:
-        - True, если касание выполнено успешно.
-        - False, если произошла ошибка при выполнении касания.
-        """
-        position = (x, y)  # Координаты для касания
-
-        try:
-            self.driver.tap(positions=[position], duration=duration)  # Выполняем касание на указанных координатах
-        except WebDriverException as e:
-            self.logger.error("_tap() Ошибка в методе _tap()"
-                              f"{x=}, {y=}"
-                              f"{duration=}")
-            self.logger.error(e)
-            return False
-        return True
+# coding: utf-8
+from typing import Optional
+
+from selenium.common import WebDriverException
+
+from AppiumExtended.appium_get import AppiumGet
+
+
+class AppiumTap(AppiumGet):
+    """
+    Класс работы с Appium.
+    Обеспечивает tap
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.helper = None
+
+    def _tap(self,
+             x: int,
+             y: int,
+             duration: Optional[int] = None,
+             ) -> bool:
+        """
+        Выполняет касание на экране устройства в указанных координатах (x, y) или на основе изображения.
+
+        Аргументы:
+        - x (int): Горизонтальная координата X точки касания на экране устройства.
+        - y (int): Вертикальная координата Y точки касания на экране устройства.
+        - duration (Optional[int]): Длительность касания в миллисекундах (по умолчанию None).
+
+        Возвращает:
+        - True, если касание выполнено успешно.
+        - False, если произошла ошибка при выполнении касания.
+        """
+        position = (x, y)  # Координаты для касания
+
+        try:
+            self.driver.tap(positions=[position], duration=duration)  # Выполняем касание на указанных координатах
+        except WebDriverException as e:
+            self.logger.error("_tap() Ошибка в методе _tap()"
+                              f"{x=}, {y=}"
+                              f"{duration=}")
+            self.logger.error(e)
+            return False
+        return True
```

### Comparing `AppiumExtended-0.1.3/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.1.6/AppiumExtended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.3/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.1.6/AppiumHelpers/appium_helpers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,360 +1,360 @@
-# coding: utf-8
-import os
-from typing import Tuple, Dict, Union, List, Optional, Any
-
-from appium.webdriver import WebElement
-from selenium.common import WebDriverException
-
-from AppiumHelpers.appium_image import AppiumImage
-
-
-class AppiumHelpers(AppiumImage):
-
-    def __init__(self, driver):
-        super().__init__(driver=driver)
-
-    @staticmethod
-    def handle_webelement_locator(locator, timeout: int,
-                                  elements_range=None,
-                                  contains: bool = False) -> Union[WebElement, None]:
-        """
-        Обрабатывает локатор типа WebElement, возвращая его без дополнительных действий.
-
-        Args:
-            locator: Локатор типа WebElement.
-            timeout: Время ожидания элемента в секундах (игнорируется).
-            elements_range: Диапазон элементов для поиска (игнорируется).
-
-        Returns:
-            Union[WebElement, None]: Возвращает заданный WebElement.
-        """
-        return locator
-
-    def handle_dict_locator(self,
-                            locator,
-                            timeout: int = 10,
-                            elements_range=None,
-                            contains: bool = False) -> Union[Tuple, None]:
-        """
-        Создает локатор xpath на основе переданного словаря-локатора Dict[str, str] и использует его для поиска элемента.
-
-        Args:
-            locator: Словарь-локатор типа Dict[str, str].
-            timeout: Время ожидания элемента в секундах (игнорируется).
-            elements_range: Диапазон элементов для поиска (игнорируется).
-            contains: Ищет элемент содержащий фрагмент значения
-
-        Returns:
-            Union[Tuple, None]: Найденный WebElement или None, если элемент не найден.
-        """
-        if 'class' not in locator:
-            xpath = "//*"
-        else:
-            xpath = "//" + locator['class']
-        try:
-            if contains:
-                for attr, value in locator.items():
-                    xpath += f"[contains(@{attr}, '{value}')]"
-                new_locator = ("xpath", xpath)
-                return new_locator
-            else:
-                for attr, value in locator.items():
-                    xpath += f"[@{attr}='{value}']"
-                new_locator = ("xpath", xpath)
-                return new_locator
-        except KeyError as e:
-            self.logger.error(f"Ошибка dict: {locator}")
-            self.logger.error("{}".format(e))
-            return None
-
-    def handle_string_locator(self,
-                              locator,
-                              timeout: int,
-                              elements_range: Union[dict, list, tuple] = None,
-                              contains: bool = False
-                              ) -> Union[WebElement, None]:
-        """
-        Обрабатывает строковый локатор и возвращает найденный элемент.
-
-        Args:
-            locator: Строковый локатор для поиска элемента.
-            timeout: Время ожидания элемента в секундах.
-            elements_range: Диапазон элементов, в котором нужно искать ближайший к точке элемент.
-                                                        Если параметр не указан, будет произведен поиск среди всех элементов на странице.
-
-        Returns:
-            Union[WebElement, None]: Найденный WebElement, либо None, если элемент не найден.
-        """
-        if not self.is_image_on_the_screen(image=locator):
-            return None
-        # поиск координат фрагмента изображения на экране
-        screenshot = self.get_screenshot_as_base64_decoded()
-        full_image = self.to_ndarray(screenshot)
-        max_loc = self.get_image_coordinates(full_image=full_image, image=locator)
-        x = max_loc[0]
-        y = max_loc[1]
-
-        # определение списка элементов для поиска
-        elements = None
-        locator = ("xpath", "//*")
-        if isinstance(elements_range, dict):
-            locator = self.handle_dict_locator(elements_range)
-        elif isinstance(elements_range, list):
-            elements = elements_range
-        elif isinstance(elements_range, tuple):
-            locator = elements_range
-        if not elements:
-            elements = self.driver.find_elements(*locator)
-
-        # Поиск ближайшего к координатам элемента
-        element = self.get_closest_element_to_point(x=x, y=y, elements=elements)
-        if not element:
-            self.logger.error(f"Элемент не обнаружен\n"
-                              f"{locator=}\n"
-                              f"{elements_range=}\n")
-
-        return element
-
-    @staticmethod
-    def get_closest_element_to_point(x, y, elements,
-                                     ) -> Union[WebElement, None]:
-        """
-        Ищет ближайший элемент к заданным координатам на экране.
-
-        Args:
-            x (int): Координата по оси X.
-            y (int): Координата по оси Y.
-            elements:
-                Список элементов для поиска.
-
-        Returns:
-            Optional[WebElement]: Найденный элемент, или `None`, если ни один элемент не был найден.
-        """
-
-        closest_element = None
-        closest_distance = float("inf")
-
-        for element in elements:
-            left, top, right, bottom = map(int,
-                                           element.get_attribute('bounds').strip("[]").replace("][", ",").split(","))
-            distance = ((x - left) ** 2 + (y - top) ** 2) ** 0.5  # Euclidean distance formula
-
-            if distance < closest_distance:  # and left <= x and top <= y:
-                closest_distance = distance
-                closest_element = element
-
-        return closest_element
-
-    def handle_webelement_locator_elements(self,
-                                           locator: List[WebElement],
-                                           timeout: int,
-                                           elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                                           contains: bool = True) -> \
-            Union[List[WebElement], None]:
-        """
-        Обрабатывает локатор типа WebElement и возвращает его без дополнительных действий.
-
-        Args:
-            locator (WebElement): Локатор типа WebElement для обработки.
-            timeout (int): Время ожидания элемента (игнорируется).
-
-        Returns:
-            Union[WebElement, None]: Заданный WebElement.
-        """
-        if not isinstance(locator[0], WebElement):
-            self.logger.error(f"Элементы списка не WebElement\n"
-                              f"{locator=}\n"
-                              f"{timeout=}\n\n")
-            print("ERROR in handle_webelement_locator_elements()")
-            return None
-        return locator
-
-    def handle_dict_locator_elements(self,
-                                     locator: Dict[str, str],
-                                     timeout: int = 10,
-                                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                                     contains: bool = True) -> \
-            Optional[Tuple[str, str]]:
-        """
-        Обрабатывает локатор типа Dict[str, str], создавая на его основе локатор типа xpath и используя его для поиска элемента.
-        XPATH нельзя подавать в качестве ключа.
-
-        Args:
-            locator (Dict[str, str]): Локатор типа Dict[str, str].
-            timeout (int): Время ожидания элемента.
-
-        Returns:
-            Union[WebElement, None]: Найденный WebElement в виде списка, либо None, если элемент не найден.
-        """
-        if 'class' not in locator:
-            xpath = "//*"
-        else:
-            xpath = "//" + locator['class']
-        try:
-            if contains:
-                for attr, value in locator.items():
-                    xpath += f"[contains(@{attr}, '{value}')]"
-                new_locator = ("xpath", xpath)
-                return new_locator
-            else:
-                for attr, value in locator.items():
-                    xpath += f"[@{attr} = '{value}']"
-                new_locator = ("xpath", xpath)
-                return new_locator
-        except KeyError as e:
-            self.logger.error(f"Ошибка dict: {locator}")
-            self.logger.error("{}".format(e))
-            return None
-
-    def handle_string_locator_elements(self,  # FIXME оптимизировать используя силу xpath и/или xml tree
-                                       locator: str,
-                                       timeout: int = 10,
-                                       elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                                       cv_threshold: float = 0.7,  # веса откалиброваны
-                                       coord_threshold: int = 1,
-                                       contains: bool = True) -> \
-            Union[List, None]:
-        """
-        Обрабатывает строковый локатор, используя его как путь до файла с изображением.
-        Находит элемент на странице, соответствующий указанному изображению.
-        Настоятельно рекомендуется использовать диапазон поиска elements_range.
-
-        Args:
-            locator (str): Путь до файла с изображением.
-            timeout (int): Максимальное время ожидания появления элемента в секундах.
-
-        Returns:
-            Union[List[Tuple], None]: Найденные элементы, либо None, если элементы не найдены.
-        """
-        #  Сохранение скриншота изображения и поиск координат совпадающих изображений
-        with open('full_image.png', 'wb') as f:
-            f.write(self.driver.get_screenshot_as_png())
-        max_locs = self.get_many_coordinates_of_image(full_image='full_image.png',
-                                                      image=locator,
-                                                      cv_threshold=cv_threshold,
-                                                      coord_threshold=coord_threshold)
-        if not max_locs:
-            self.logger.error("Элементы не обнаружены")
-            return None
-        os.remove('full_image.png')
-
-        # определение списка элементов для поиска
-        elements = None
-        locator = ("xpath", "//*")
-        if isinstance(elements_range, dict):
-            locator = self.handle_dict_locator(elements_range)
-        elif isinstance(elements_range, list):
-            elements = elements_range
-        elif isinstance(elements_range, tuple):
-            locator = elements_range
-        if not elements:
-            elements = self.driver.find_elements(*locator)
-
-        # Поиск ближайших к координатам элементов
-        result = []
-        for max_loc in max_locs:
-            x = max_loc[0]
-            y = max_loc[1]
-            element = self.get_closest_element_to_point(x=x, y=y, elements=elements)
-            result.append(element)
-
-        # удаление родительских элементов
-        result = self.remove_nesting(result)
-        # сортировка по координатам
-        result = self.sort_elements_by_bounds(result)
-
-        # debug save to folder  TODO удалить фрагмент после тестов
-        for index, element in enumerate(result):
-            file_path = os.path.join('core', 'appium', 'unit_test', 'str_elements', f'screenshot_{index}.png')
-            with open(file_path, 'wb') as file:
-                file.write(element.screenshot_as_png)
-
-        return result
-
-    def add_bounds(self, elements: List[WebElement]) -> list[list[Union[WebElement, Any]]]:
-        """
-        Добавляет координаты в список элементов
-        """
-        elements_with_bounds = []
-        for element in elements:
-            try:
-                coord = element.get_attribute("bounds")
-                left, top, right, bottom = map(int, coord[1:-1].replace("][", ",").split(','))
-                elements_with_bounds.append([element, left, top, right, bottom])
-            except WebDriverException as e:
-                self.logger.error("Error sorting elements: {}".format(e))
-        return elements_with_bounds
-
-    @staticmethod
-    def remove_bounds(elements_with_bounds):
-        """
-        Удаляет координаты из списка элементов. Работает только в связке с add_bounds.
-        """
-        elements_without_bounds = [lst[0] for lst in elements_with_bounds]
-        return elements_without_bounds
-
-    def sort_elements_by_bounds(self, elements: List[WebElement], desc: bool = False) -> Optional[List[WebElement]]:
-        """
-        Сортирует список из WebElement, по значению их верхней координаты.
-
-        Args:
-            elements (List[WebElement]): список из WebElement объектов.
-            desc (bool): Если False (default), сортирует в обратном порядке.
-
-        Returns:
-            List[WebElement]: сортированный список WebElement объектов.
-            Если подан не корректный аргумент elements, возвращает None.
-
-        Usage:
-            elements = driver.find_elements_by_xpath("//div[@class='my-class']")
-            sorted_elements = sort_elements_by_bounds(elements, desc=False)
-        """
-        if not elements or not isinstance(elements, list) or not isinstance(elements[0], WebElement):
-            self.logger.error(f"Список невозможно сортировать, {elements=}")
-            return None
-
-        elements_with_coords = self.add_bounds(elements)
-        sorted_elements = sorted(elements_with_coords, key=lambda x: x[2], reverse=desc)
-        result = self.remove_bounds(sorted_elements)
-        return result
-
-    def remove_nesting(self, elements) -> List[WebElement]:  # FIXME реализовать через Axis а не координаты
-        """
-        Проверяет вхождение элементов в другие элементы по координатам.
-        При обнаружении удаляет большие по размеру.
-        """
-        # удаление дубликатов
-        elements = list(set(elements))
-
-        # добавление координат
-        elements_with_coords = self.add_bounds(elements)
-
-        # поиск элементов имеющих дочерние (по координатам, точное вхождение, без учета оверлапса)
-        for index, el1 in enumerate(elements_with_coords):
-            # координаты 0.0 в левом верхнем углу экрана
-            el1_left_top_x = el1[1]
-            el1_left_top_y = el1[2]
-            el1_right_bottom_x = el1[3]
-            el1_right_boot_y = el1[4]
-            for el2 in elements_with_coords:
-                el2_left_top_x = el2[1]
-                el2_left_top_y = el2[2]
-                el2_right_bottom_x = el2[3]
-                el2_right_boot_y = el2[4]
-                if el1_left_top_x < el2_left_top_x and el1_left_top_y < el2_left_top_y and el1_right_bottom_x > \
-                        el2_right_bottom_x and el1_right_boot_y > el2_right_boot_y:
-                    elements_with_coords[index] = [el1[0], el1[1], el1[2], el1[3], el1[4], 'parent']  # метка
-        elements_no_parent = []
-
-        # формирование списка не имеющих родительских элементов (по координатам)
-        for element in elements_with_coords:
-            if len(element) < 6:
-                elements_no_parent.append(element)
-
-        # удаление координат, приведение к списку элементов
-        result = self.remove_bounds(elements_no_parent)
-        return result
-
-    def find_only_children(self, element, elements):
-        return
-
+# coding: utf-8
+import os
+from typing import Tuple, Dict, Union, List, Optional, Any
+
+from appium.webdriver import WebElement
+from selenium.common import WebDriverException
+
+from AppiumHelpers.appium_image import AppiumImage
+
+
+class AppiumHelpers(AppiumImage):
+
+    def __init__(self, driver):
+        super().__init__(driver=driver)
+
+    @staticmethod
+    def handle_webelement_locator(locator, timeout: int,
+                                  elements_range=None,
+                                  contains: bool = False) -> Union[WebElement, None]:
+        """
+        Обрабатывает локатор типа WebElement, возвращая его без дополнительных действий.
+
+        Args:
+            locator: Локатор типа WebElement.
+            timeout: Время ожидания элемента в секундах (игнорируется).
+            elements_range: Диапазон элементов для поиска (игнорируется).
+
+        Returns:
+            Union[WebElement, None]: Возвращает заданный WebElement.
+        """
+        return locator
+
+    def handle_dict_locator(self,
+                            locator,
+                            timeout: int = 10,
+                            elements_range=None,
+                            contains: bool = False) -> Union[Tuple, None]:
+        """
+        Создает локатор xpath на основе переданного словаря-локатора Dict[str, str] и использует его для поиска элемента.
+
+        Args:
+            locator: Словарь-локатор типа Dict[str, str].
+            timeout: Время ожидания элемента в секундах (игнорируется).
+            elements_range: Диапазон элементов для поиска (игнорируется).
+            contains: Ищет элемент содержащий фрагмент значения
+
+        Returns:
+            Union[Tuple, None]: Найденный WebElement или None, если элемент не найден.
+        """
+        if 'class' not in locator:
+            xpath = "//*"
+        else:
+            xpath = "//" + locator['class']
+        try:
+            if contains:
+                for attr, value in locator.items():
+                    xpath += f"[contains(@{attr}, '{value}')]"
+                new_locator = ("xpath", xpath)
+                return new_locator
+            else:
+                for attr, value in locator.items():
+                    xpath += f"[@{attr}='{value}']"
+                new_locator = ("xpath", xpath)
+                return new_locator
+        except KeyError as e:
+            self.logger.error(f"Ошибка dict: {locator}")
+            self.logger.error("{}".format(e))
+            return None
+
+    def handle_string_locator(self,
+                              locator,
+                              timeout: int,
+                              elements_range: Union[dict, list, tuple] = None,
+                              contains: bool = False
+                              ) -> Union[WebElement, None]:
+        """
+        Обрабатывает строковый локатор и возвращает найденный элемент.
+
+        Args:
+            locator: Строковый локатор для поиска элемента.
+            timeout: Время ожидания элемента в секундах.
+            elements_range: Диапазон элементов, в котором нужно искать ближайший к точке элемент.
+                                                        Если параметр не указан, будет произведен поиск среди всех элементов на странице.
+
+        Returns:
+            Union[WebElement, None]: Найденный WebElement, либо None, если элемент не найден.
+        """
+        if not self.is_image_on_the_screen(image=locator):
+            return None
+        # поиск координат фрагмента изображения на экране
+        screenshot = self.get_screenshot_as_base64_decoded()
+        full_image = self.to_ndarray(screenshot)
+        max_loc = self.get_image_coordinates(full_image=full_image, image=locator)
+        x = max_loc[0]
+        y = max_loc[1]
+
+        # определение списка элементов для поиска
+        elements = None
+        locator = ("xpath", "//*")
+        if isinstance(elements_range, dict):
+            locator = self.handle_dict_locator(elements_range)
+        elif isinstance(elements_range, list):
+            elements = elements_range
+        elif isinstance(elements_range, tuple):
+            locator = elements_range
+        if not elements:
+            elements = self.driver.find_elements(*locator)
+
+        # Поиск ближайшего к координатам элемента
+        element = self.get_closest_element_to_point(x=x, y=y, elements=elements)
+        if not element:
+            self.logger.error(f"Элемент не обнаружен\n"
+                              f"{locator=}\n"
+                              f"{elements_range=}\n")
+
+        return element
+
+    @staticmethod
+    def get_closest_element_to_point(x, y, elements,
+                                     ) -> Union[WebElement, None]:
+        """
+        Ищет ближайший элемент к заданным координатам на экране.
+
+        Args:
+            x (int): Координата по оси X.
+            y (int): Координата по оси Y.
+            elements:
+                Список элементов для поиска.
+
+        Returns:
+            Optional[WebElement]: Найденный элемент, или `None`, если ни один элемент не был найден.
+        """
+
+        closest_element = None
+        closest_distance = float("inf")
+
+        for element in elements:
+            left, top, right, bottom = map(int,
+                                           element.get_attribute('bounds').strip("[]").replace("][", ",").split(","))
+            distance = ((x - left) ** 2 + (y - top) ** 2) ** 0.5  # Euclidean distance formula
+
+            if distance < closest_distance:  # and left <= x and top <= y:
+                closest_distance = distance
+                closest_element = element
+
+        return closest_element
+
+    def handle_webelement_locator_elements(self,
+                                           locator: List[WebElement],
+                                           timeout: int,
+                                           elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                                           contains: bool = True) -> \
+            Union[List[WebElement], None]:
+        """
+        Обрабатывает локатор типа WebElement и возвращает его без дополнительных действий.
+
+        Args:
+            locator (WebElement): Локатор типа WebElement для обработки.
+            timeout (int): Время ожидания элемента (игнорируется).
+
+        Returns:
+            Union[WebElement, None]: Заданный WebElement.
+        """
+        if not isinstance(locator[0], WebElement):
+            self.logger.error(f"Элементы списка не WebElement\n"
+                              f"{locator=}\n"
+                              f"{timeout=}\n\n")
+            print("ERROR in handle_webelement_locator_elements()")
+            return None
+        return locator
+
+    def handle_dict_locator_elements(self,
+                                     locator: Dict[str, str],
+                                     timeout: int = 10,
+                                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                                     contains: bool = True) -> \
+            Optional[Tuple[str, str]]:
+        """
+        Обрабатывает локатор типа Dict[str, str], создавая на его основе локатор типа xpath и используя его для поиска элемента.
+        XPATH нельзя подавать в качестве ключа.
+
+        Args:
+            locator (Dict[str, str]): Локатор типа Dict[str, str].
+            timeout (int): Время ожидания элемента.
+
+        Returns:
+            Union[WebElement, None]: Найденный WebElement в виде списка, либо None, если элемент не найден.
+        """
+        if 'class' not in locator:
+            xpath = "//*"
+        else:
+            xpath = "//" + locator['class']
+        try:
+            if contains:
+                for attr, value in locator.items():
+                    xpath += f"[contains(@{attr}, '{value}')]"
+                new_locator = ("xpath", xpath)
+                return new_locator
+            else:
+                for attr, value in locator.items():
+                    xpath += f"[@{attr} = '{value}']"
+                new_locator = ("xpath", xpath)
+                return new_locator
+        except KeyError as e:
+            self.logger.error(f"Ошибка dict: {locator}")
+            self.logger.error("{}".format(e))
+            return None
+
+    def handle_string_locator_elements(self,  # FIXME оптимизировать используя силу xpath и/или xml tree
+                                       locator: str,
+                                       timeout: int = 10,
+                                       elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                                       cv_threshold: float = 0.7,  # веса откалиброваны
+                                       coord_threshold: int = 1,
+                                       contains: bool = True) -> \
+            Union[List, None]:
+        """
+        Обрабатывает строковый локатор, используя его как путь до файла с изображением.
+        Находит элемент на странице, соответствующий указанному изображению.
+        Настоятельно рекомендуется использовать диапазон поиска elements_range.
+
+        Args:
+            locator (str): Путь до файла с изображением.
+            timeout (int): Максимальное время ожидания появления элемента в секундах.
+
+        Returns:
+            Union[List[Tuple], None]: Найденные элементы, либо None, если элементы не найдены.
+        """
+        #  Сохранение скриншота изображения и поиск координат совпадающих изображений
+        with open('full_image.png', 'wb') as f:
+            f.write(self.driver.get_screenshot_as_png())
+        max_locs = self.get_many_coordinates_of_image(full_image='full_image.png',
+                                                      image=locator,
+                                                      cv_threshold=cv_threshold,
+                                                      coord_threshold=coord_threshold)
+        if not max_locs:
+            self.logger.error("Элементы не обнаружены")
+            return None
+        os.remove('full_image.png')
+
+        # определение списка элементов для поиска
+        elements = None
+        locator = ("xpath", "//*")
+        if isinstance(elements_range, dict):
+            locator = self.handle_dict_locator(elements_range)
+        elif isinstance(elements_range, list):
+            elements = elements_range
+        elif isinstance(elements_range, tuple):
+            locator = elements_range
+        if not elements:
+            elements = self.driver.find_elements(*locator)
+
+        # Поиск ближайших к координатам элементов
+        result = []
+        for max_loc in max_locs:
+            x = max_loc[0]
+            y = max_loc[1]
+            element = self.get_closest_element_to_point(x=x, y=y, elements=elements)
+            result.append(element)
+
+        # удаление родительских элементов
+        result = self.remove_nesting(result)
+        # сортировка по координатам
+        result = self.sort_elements_by_bounds(result)
+
+        # debug save to folder  TODO удалить фрагмент после тестов
+        for index, element in enumerate(result):
+            file_path = os.path.join('core', 'appium', 'unit_test', 'str_elements', f'screenshot_{index}.png')
+            with open(file_path, 'wb') as file:
+                file.write(element.screenshot_as_png)
+
+        return result
+
+    def add_bounds(self, elements: List[WebElement]) -> list[list[Union[WebElement, Any]]]:
+        """
+        Добавляет координаты в список элементов
+        """
+        elements_with_bounds = []
+        for element in elements:
+            try:
+                coord = element.get_attribute("bounds")
+                left, top, right, bottom = map(int, coord[1:-1].replace("][", ",").split(','))
+                elements_with_bounds.append([element, left, top, right, bottom])
+            except WebDriverException as e:
+                self.logger.error("Error sorting elements: {}".format(e))
+        return elements_with_bounds
+
+    @staticmethod
+    def remove_bounds(elements_with_bounds):
+        """
+        Удаляет координаты из списка элементов. Работает только в связке с add_bounds.
+        """
+        elements_without_bounds = [lst[0] for lst in elements_with_bounds]
+        return elements_without_bounds
+
+    def sort_elements_by_bounds(self, elements: List[WebElement], desc: bool = False) -> Optional[List[WebElement]]:
+        """
+        Сортирует список из WebElement, по значению их верхней координаты.
+
+        Args:
+            elements (List[WebElement]): список из WebElement объектов.
+            desc (bool): Если False (default), сортирует в обратном порядке.
+
+        Returns:
+            List[WebElement]: сортированный список WebElement объектов.
+            Если подан не корректный аргумент elements, возвращает None.
+
+        Usage:
+            elements = driver.find_elements_by_xpath("//div[@class='my-class']")
+            sorted_elements = sort_elements_by_bounds(elements, desc=False)
+        """
+        if not elements or not isinstance(elements, list) or not isinstance(elements[0], WebElement):
+            self.logger.error(f"Список невозможно сортировать, {elements=}")
+            return None
+
+        elements_with_coords = self.add_bounds(elements)
+        sorted_elements = sorted(elements_with_coords, key=lambda x: x[2], reverse=desc)
+        result = self.remove_bounds(sorted_elements)
+        return result
+
+    def remove_nesting(self, elements) -> List[WebElement]:  # FIXME реализовать через Axis а не координаты
+        """
+        Проверяет вхождение элементов в другие элементы по координатам.
+        При обнаружении удаляет большие по размеру.
+        """
+        # удаление дубликатов
+        elements = list(set(elements))
+
+        # добавление координат
+        elements_with_coords = self.add_bounds(elements)
+
+        # поиск элементов имеющих дочерние (по координатам, точное вхождение, без учета оверлапса)
+        for index, el1 in enumerate(elements_with_coords):
+            # координаты 0.0 в левом верхнем углу экрана
+            el1_left_top_x = el1[1]
+            el1_left_top_y = el1[2]
+            el1_right_bottom_x = el1[3]
+            el1_right_boot_y = el1[4]
+            for el2 in elements_with_coords:
+                el2_left_top_x = el2[1]
+                el2_left_top_y = el2[2]
+                el2_right_bottom_x = el2[3]
+                el2_right_boot_y = el2[4]
+                if el1_left_top_x < el2_left_top_x and el1_left_top_y < el2_left_top_y and el1_right_bottom_x > \
+                        el2_right_bottom_x and el1_right_boot_y > el2_right_boot_y:
+                    elements_with_coords[index] = [el1[0], el1[1], el1[2], el1[3], el1[4], 'parent']  # метка
+        elements_no_parent = []
+
+        # формирование списка не имеющих родительских элементов (по координатам)
+        for element in elements_with_coords:
+            if len(element) < 6:
+                elements_no_parent.append(element)
+
+        # удаление координат, приведение к списку элементов
+        result = self.remove_bounds(elements_no_parent)
+        return result
+
+    def find_only_children(self, element, elements):
+        return
+
```

### Comparing `AppiumExtended-0.1.3/AppiumHelpers/appium_image.py` & `AppiumExtended-0.1.6/AppiumHelpers/appium_image.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,511 +1,511 @@
-# coding: utf-8
-import base64
-import logging
-import os
-from typing import Union, List, Tuple, Optional
-
-import cv2
-import numpy as np
-from PIL import Image
-from pytesseract import pytesseract
-
-from selenium.common.exceptions import WebDriverException
-
-import config
-from adb import adb
-from AppiumHelpers.helpers_decorators import retry
-
-
-class AppiumImage(object):
-    """
-    Класс работы с Appium.
-    Обеспечивает работу с изображениями
-    """
-
-    def __init__(self, driver=None):
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        self.driver = driver
-
-    def get_screenshot_as_base64_decoded(self):
-        screenshot = self.driver.get_screenshot_as_base64().encode('utf-8')
-        screenshot = base64.b64decode(screenshot)
-        return screenshot
-
-    @retry
-    def get_image_coordinates(self,
-                              image: Union[bytes, np.ndarray, Image.Image, str],
-                              full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                              threshold: Optional[float] = 0.7,
-                              ) -> Union[Tuple[int, int, int, int], None]:
-        """
-        Находит координаты наиболее вероятного совпадения частичного изображения в полном изображении.
-        Предназначен для поиска координат наиболее вероятного совпадения частичного изображения в полном изображении.
-
-        Args:
-            image (Union[bytes, np.ndarray, Image.Image, str]): путь к файлу частичного изображения, которое
-            нужно найти внутри полного изображения.
-            full_image (Union[bytes, np.ndarray, Image.Image, str]): путь к файлу полного изображения.
-            threshold (float, optional): минимальный порог совпадения, необходимый для считывания совпадения допустимым.
-                По умолчанию равно 0.7.
-
-        Returns:
-            tuple or None: кортеж с координатами наиболее вероятного совпадения (x1, y1, x2, y2) или None, если совпадение не найдено.
-            :param threshold:
-            :param full_image:
-        """
-        if full_image is None:
-            screenshot = self.get_screenshot_as_base64_decoded()
-            big_image = self.to_ndarray(image=screenshot, grayscale=True)
-        else:
-            big_image = self.to_ndarray(image=full_image, grayscale=True)  # Загрузка полного изображения
-
-        small_image = self.to_ndarray(image=image, grayscale=True)  # Загрузка частичного изображения
-
-        result = cv2.matchTemplate(big_image, small_image, cv2.TM_CCOEFF_NORMED)  # Поиск совпадений методом шаблона
-
-        min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(
-            result)  # Получение наименьшего и наибольшего значения, а также соответствующих координат
-
-        if not max_val >= threshold:  # Если наибольшее значение совпадения не превышает порога, возвращаем None
-            self.logger.error("find_coordinates_by_image(): Совпадений не найдено")
-            return None
-
-        # Вычисляем координаты левого верхнего и правого нижнего углов найденного совпадения
-        left = int(max_loc[0])
-        top = int(max_loc[1])
-        width = small_image.shape[1]
-        height = small_image.shape[0]
-        right = left + width
-        bottom = top + height
-
-        return int(left), int(top), int(right), int(bottom)  # Возвращаем координаты наиболее вероятного совпадения
-
-    @retry
-    def get_inner_image_coordinates(self,
-                                    outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                    inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
-                                    threshold: float = 0.9) -> Union[Tuple[int, int, int, int], None]:
-        """
-        Находит изображение на экране и внутри него находит другое изображение (внутреннее).
-        Предназначен для поиска изображения на экране и затем нахождения другого изображения (внутреннего)
-        внутри этого обнаруженного изображения.
-
-        Параметры:
-            outer_image_path (str): Путь к файлу с изображением, которое нужно найти на экране.
-            inner_image_path (str): Путь к файлу с изображением, которое нужно найти внутри внешнего изображения.
-            threshold (float, optional): Пороговое значение сходства для шаблонного сопоставления. По умолчанию 0.9.
-
-        Возвращает:
-            tuple: Координаты внутреннего изображения относительно экрана в формате ((x1, y1), (x2, y2)).
-                   Если внутреннее изображение не найдено, возвращает None.
-        """
-        # Получаем разрешение экрана
-        screen_width, screen_height = adb.get_screen_resolution()
-
-        # Захватываем скриншот
-        screenshot = base64.b64decode(self.driver.get_screenshot_as_base64())
-
-        # Читаем скриншот
-        full_image = self.to_ndarray(image=screenshot, grayscale=True)
-
-        # Прочитать внешнее изображение
-        outer_image = self.to_ndarray(image=outer_image_path, grayscale=True)
-
-        # Прочитать внутреннее изображение
-        inner_image = self.to_ndarray(image=inner_image_path, grayscale=True)
-
-        # Вычисляем коэффициенты масштабирования
-        width_ratio = screen_width / full_image.shape[1]
-        height_ratio = screen_height / full_image.shape[0]
-
-        # ...
-        inner_image = cv2.resize(inner_image, None, fx=width_ratio, fy=height_ratio)
-        outer_image = cv2.resize(outer_image, None, fx=width_ratio, fy=height_ratio)
-
-        # Применить шаблонное сопоставление для поиска внешнего изображения
-        outer_result = cv2.matchTemplate(full_image, outer_image, cv2.TM_CCOEFF_NORMED)
-
-        # Найти максимальное значение сходства и его положение для внешнего изображения
-        _, outer_max_val, _, outer_max_loc = cv2.minMaxLoc(outer_result)
-
-        # Проверить, превышает ли максимальное значение сходства для внешнего изображения пороговое значение
-        if outer_max_val >= threshold:
-            # Получить размеры внешнего изображения
-            outer_height, outer_width = outer_image.shape
-
-            # Вычислить координаты внешнего изображения на экране
-            outer_top_left = outer_max_loc
-            outer_bottom_right = (outer_top_left[0] + outer_width, outer_top_left[1] + outer_height)
-
-            # Извлечь область интереса (ROI), содержащую внешнее изображение
-            outer_roi = full_image[outer_top_left[1]:outer_bottom_right[1], outer_top_left[0]:outer_bottom_right[0]]
-
-            # Применить шаблонное сопоставление для поиска внутреннего изображения внутри ROI
-            inner_result = cv2.matchTemplate(outer_roi, inner_image, cv2.TM_CCOEFF_NORMED)
-
-            # Найти максимальное значение сходства и его положение для внутреннего изображения внутри ROI
-            _, inner_max_val, _, inner_max_loc = cv2.minMaxLoc(inner_result)
-
-            # Проверить, превышает ли максимальное значение сходства для внутреннего изображения пороговое значение
-            if inner_max_val >= threshold:
-                # Получить размеры внутреннего изображения
-                inner_height, inner_width = inner_image.shape
-
-                # Вычислить координаты внутреннего изображения относительно экрана
-                inner_top_left = (outer_top_left[0] + inner_max_loc[0], outer_top_left[1] + inner_max_loc[1])
-                inner_bottom_right = (inner_top_left[0] + inner_width, inner_top_left[1] + inner_height)
-
-                # Вернуть координаты внутреннего изображения относительно экрана
-                return inner_top_left + inner_bottom_right
-
-        # Вернуть None, если внутреннее изображение не найдено
-        return None
-
-    def is_image_on_the_screen(self,
-                               image: Union[bytes, np.ndarray, Image.Image, str],
-                               threshold: float = 0.9) -> bool:
-        """
-        Сравнивает, присутствует ли заданное изображение на экране.
-
-        Args:
-            image: Строка, содержащая имя файла частичного изображения для поиска.
-            threshold: Пороговое значение схожести части изображения со снимком экрана
-
-        Returns:
-            Логическое значение, указывающее, было ли частичное изображение найдено на экране.
-        """
-        screenshot = self.get_screenshot_as_base64_decoded()
-
-        # Чтение снимка экрана и частичного изображения
-        full_image = self.to_ndarray(image=screenshot, grayscale=True)
-        small_image = self.to_ndarray(image=image, grayscale=True)
-
-        # Сопоставление частичного изображения и снимка экрана
-        result = cv2.matchTemplate(full_image, small_image, cv2.TM_CCOEFF_NORMED)
-
-        # Извлечение коэффициента схожести и координат схожего участка
-        _, max_val, _, max_loc = cv2.minMaxLoc(result)
-
-        # Логирование
-        self.logger.debug(f"Коэффициент схожести изображения: {max_val}")
-
-        # Сравнение коэффициента схожести и порогового значения
-        if max_val >= threshold:
-            return True
-        else:
-            return False
-
-    def is_text_on_ocr_screen(self,
-                              text: str,
-                              screen: Union[bytes, np.ndarray, Image.Image, str] = None,
-                              language: str = 'rus'
-                              ) -> bool:
-        """
-        Проверяет, присутствует ли заданный текст на экране.
-        Распознавание текста производит с помощью библиотеки pytesseract.
-
-        Аргументы:
-        - text (str): Текст, который нужно найти на экране.
-        - screen (bytes, optional): Скриншот в формате bytes. Если не указан, будет захвачен скриншот с помощью `self.driver`.
-        - language (str): Язык распознавания текста. Значение по умолчанию: 'rus'.
-
-        Возвращает:
-        - bool: True, если заданный текст найден на экране. False в противном случае.
-        """
-        if screen is None:
-            screenshot = self.get_screenshot_as_base64_decoded()
-            image = self.to_ndarray(screenshot)
-        else:
-            image = self.to_ndarray(screen)
-
-        # Бинаризация изображения
-        _, image_bin = cv2.threshold(image, 0, 255,
-                                     cv2.THRESH_BINARY | cv2.THRESH_OTSU)  # Применение бинаризации для получения двоичного изображения
-
-        # Преобразование двоичного изображения в текст
-        ocr_text = pytesseract.image_to_string(image_bin, lang=language)
-
-        # Проверка наличия заданного текста в распознанном тексте
-        if text.lower() in ocr_text.lower():
-            return True
-        else:
-            return False
-
-    @retry
-    def get_many_coordinates_of_image(self,
-                                      image: Union[bytes, np.ndarray, Image.Image, str],
-                                      full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
-                                      cv_threshold: float = 0.7,
-                                      coord_threshold: int = 5) -> Union[List[Tuple], None]:
-        """
-        Находит все вхождения частичного изображения внутри полного изображения.
-
-        Args:
-            full_image (str): путь к файлу полного изображения.
-            image (str): путь к файлу частичного изображения, которое нужно найти внутри полного изображения.
-            cv_threshold (float, optional): минимальный порог совпадения, необходимый для считывания совпадения допустимым.
-                По умолчанию равно 0.7.
-            coord_threshold (int, optional): целое число, представляющее максимальное различие между значениями x и y двух
-                кортежей, чтобы они считались слишком близкими друг к другу. По умолчанию равно 5.
-
-        Returns:
-            list of tuples or None: список кортежей, содержащий расположение каждого найденного совпадения.
-                Если совпадений не найдено, возвращается None.
-        """
-
-        if full_image is None:
-            screenshot = self.get_screenshot_as_base64_decoded()
-            big_image = self.to_ndarray(image=screenshot, grayscale=True)
-        else:
-            big_image = self.to_ndarray(image=full_image, grayscale=True)  # Загрузка полного изображения
-
-        small_image = self.to_ndarray(image=image, grayscale=True)  # Загрузка частичного изображения
-
-        # Найти частичное изображение в полном изображении
-        result = cv2.matchTemplate(big_image, small_image, cv2.TM_CCOEFF_NORMED)  # Поиск совпадений методом шаблона
-
-        # Получить все совпадения выше порога
-        locations = np.where(result >= cv_threshold)  # Нахождение всех совпадений выше порога
-        matches = list(zip(*locations[::-1]))  # Преобразование координат в список кортежей
-
-        # Фильтрация слишком близких совпадений
-        unique_list = []  # Создаем пустой список для хранения уникальных кортежей
-        for i, (x1, y1) in enumerate(matches):  # Итерируемся по списку кортежей
-            exclude = False  # Инициализируем флаг exclude значением False
-            for (x2, y2) in unique_list:  # Итерируемся по уникальным кортежам
-                if abs(x1 - x2) <= coord_threshold and abs(y1 - y2) <= coord_threshold:
-                    # Если различие между значениями x и y двух кортежей меньше или равно порогу,
-                    # помечаем exclude как True и выходим из цикла
-                    exclude = True
-                    break
-            if not exclude:  # Если exclude равно False, добавляем кортеж в unique_list
-                unique_list.append((x1, y1))
-        matches = unique_list
-
-        if not matches:
-            self.logger.error(f"_find_many_coordinates_by_image() NO MATCHES, {image=}")
-            return None
-
-        # Добавляем правый нижний угол к каждому найденному совпадению
-        matches_with_corners = []
-        for match in matches:
-            x, y = match
-            w, h = small_image.shape[::-1]
-            top_left = (x, y)
-            bottom_right = (x + w, y + h)
-            matches_with_corners.append((top_left + bottom_right))
-
-        return matches_with_corners
-
-    @retry
-    def get_text_coordinates(
-            self,
-            text: str,
-            image: Union[bytes, str, Image.Image, np.ndarray] = None,
-            language: str = 'rus'
-    ) -> Union[Tuple[int, int, int, int], None]:
-        """
-        Возвращает координаты области с указанным текстом на предоставленном изображении или снимке экрана.
-
-        Аргументы:
-        - text (str): Искомый текст.
-        - image (bytes, str, Image.Image, np.ndarray, опционально): Изображение, на котором осуществляется поиск текста.
-          Если не указано, будет использован снимок экрана. По умолчанию None.
-        - language (str, опционально): Язык для распознавания текста. По умолчанию 'rus'.
-
-        Возвращает:
-        - Union[Tuple[int, int, int, int], None]: Координаты области с текстом или None, если текст не найден.
-        """
-
-        if not image:
-            # Получаем снимок экрана, если изображение не предоставлено
-            screenshot = self.get_screenshot_as_base64_decoded()  # Получение снимка экрана в формате base64
-            image = self.to_ndarray(image=screenshot,
-                                    grayscale=True)  # Преобразование снимка экрана в массив numpy и преобразование в оттенки серого
-        else:
-            # Если предоставлено, то преобразуем
-            image = self.to_ndarray(image=image,
-                                    grayscale=True)  # Преобразование изображения в массив numpy и преобразование в оттенки серого
-
-        # Бинаризация изображения
-        _, threshold = cv2.threshold(image, 0, 255,
-                                     cv2.THRESH_BINARY | cv2.THRESH_OTSU)  # Применение бинаризации для получения двоичного изображения
-
-        # Выполнение OCR с помощью PyTesseract
-        data = pytesseract.image_to_data(threshold, lang=language,
-                                         output_type=pytesseract.Output.DICT)  # Использование PyTesseract для распознавания текста и получения информации о распознанных словах
-
-        formatted_data = {}
-        for i in range(len(data['text'])):
-            word_text = data['text'][i]  # Текст слова
-            left = int(data['left'][i])  # Координата левой границы слова
-            top = int(data['top'][i])  # Координата верхней границы слова
-            width = int(data['width'][i])  # Ширина слова
-            height = int(data['height'][i])  # Высота слова
-            coordinates = [left, top, left + width, top + height]  # Координаты рамки слова
-
-            if word_text:
-                if i not in formatted_data:
-                    formatted_data[i] = {}
-                formatted_data[i] = {'text': word_text,
-                                     'coordinates': coordinates}  # Сохранение информации о слове и его координатах
-
-        # Разбить искомый текст на отдельные слова
-        words = text.split(' ')  # Разделение искомого текста на отдельные слова
-
-        # Инициализировать переменные для последовательности слов и соответствующих координат
-        current_sequence = []  # Текущая последовательность слов
-        result_coordinates = []  # Координаты текущей последовательности слов
-
-        for index, word_data in formatted_data.items():
-            word = word_data['text']  # Текущее слово
-            coordinates = word_data['coordinates']  # Координаты слова
-
-            if word in words:
-                current_sequence.append(word)  # Добавление слова в текущую последовательность
-                result_coordinates.append(coordinates)  # Добавление координат слова в результат
-            else:
-                if current_sequence == words:
-                    # Если найдена последовательность слов, вернуть соответствующие координаты
-                    top_left = tuple(map(int, result_coordinates[0][:2]))  # Верхний левый угол рамки
-                    bottom_right = tuple(map(int, result_coordinates[-1][2:]))  # Нижний правый угол рамки
-                    return top_left + bottom_right
-                current_sequence = []  # Сброс текущей последовательности слов
-                result_coordinates = []  # Сброс координат последовательности слов
-
-        return None
-
-    def draw_by_coordinates(self,
-                            image: Union[bytes, str, Image.Image, np.ndarray] = None,
-                            coordinates: Tuple[int, int, int, int] = None,
-                            top_left: Tuple[int, int] = None,
-                            bottom_right: Tuple[int, int] = None,
-                            path: str = None) -> bool:
-        """
-        Рисует прямоугольник на предоставленном изображении или снимке экрана с помощью драйвера.
-        Прямоугольник определяется либо координатами, либо верхней левой и нижней правой точками.
-        Результирующее изображение с нарисованным прямоугольником сохраняется по указанному пути.
-
-        Аргументы:
-            image (Union[bytes, str, Image.Image], опционально): Изображение, на котором будет рисоваться.
-                Может быть представлено в виде bytes, str (путь до файла) или PIL Image.
-                Если не указано, используется снимок экрана. По умолчанию None.
-            coordinates (Tuple[int, int, int, int], опционально): Координаты прямоугольника (x1, y1, x2, y2).
-                По умолчанию None.
-            top_left (Tuple[int, int], опционально): Верхняя левая точка прямоугольника (x, y). По умолчанию None.
-            bottom_right (Tuple[int, int], опционально): Нижняя правая точка прямоугольника (x, y). По умолчанию None.
-            path (str, опционально): Путь для сохранения результирующего изображения. По умолчанию None.
-
-        Usage:
-            image = self.driver.get_screenshot_as_base64().encode('utf-8')
-            draw_by_coordinates(image=image, coordinates=(123, 123, 123, 123), path='pictures')
-
-        Возвращает:
-            bool: True, если операция выполнена успешно, False в противном случае.
-        """
-        try:
-            if image is None:
-                # Если изображение не предоставлено, получаем снимок экрана с помощью драйвера
-                screenshot = self.get_screenshot_as_base64_decoded()
-                image = self.to_ndarray(screenshot)
-            else:
-                image = self.to_ndarray(image)
-
-            # Если верхняя левая и нижняя правая точки не предоставлены, используем координаты для определения
-            # прямоугольника
-            if not top_left and not bottom_right:
-                top_left = (coordinates[0], coordinates[1])
-                bottom_right = (coordinates[2], coordinates[3])
-
-            # Сохраняем снимок экрана с нарисованным прямоугольником
-            if path is None:
-                path = "screenshot_with_text_coordinates.png"
-            path = os.path.join(path)
-            cv2.rectangle(image, top_left, bottom_right, (0, 255, 0), 2)
-            cv2.imwrite(path, image)
-
-            return True
-        except WebDriverException as e:
-            # Обрабатываем исключение WebDriverException и записываем ошибку в журнал
-            self.logger.error(f'draw_by_coordinates() WebDriverException {e}')
-            return False
-        except cv2.error as e:
-            # Обработка исключения cv2.error
-            self.logger.error(f'draw_by_coordinates() cv2.error: {e}')
-            return False
-
-    @staticmethod
-    def is_rgb(image: np.ndarray) -> bool:
-        """
-        Проверяет, является ли изображение цветным (RGB).
-
-        Аргументы:
-        - image: np.ndarray - Входное изображение в формате NumPy ndarray.
-
-        Возвращает:
-        - bool - True, если изображение является цветным (RGB), False - в противном случае.
-        """
-        return len(image.shape) == 3 and image.shape[2] == 3 or image.ndim == 3 or image.ndim == '3'
-
-    @staticmethod
-    def is_grayscale(image: np.ndarray) -> bool:
-        """
-        Проверяет, является ли изображение оттенков серого.
-
-        Аргументы:
-        - image: np.ndarray - Входное изображение в формате NumPy ndarray.
-
-        Возвращает:
-        - bool - True, если изображение является оттенков серого, False - в противном случае.
-        """
-        return len(image.shape) == 2 or (
-                len(image.shape) == 3 and image.shape[2] == 1) or image.ndim == 2 or image.ndim == '2'
-
-    def to_grayscale(self, image: np.ndarray) -> np.ndarray:
-        """
-        Преобразует изображение в оттенки серого.
-
-        Аргументы:
-        - image: np.ndarray - Входное изображение в формате ndarray.
-
-        Возвращает:
-        - np.ndarray - Преобразованное изображение в оттенках серого.
-        """
-        # Проверяем, является ли изображение в формате RGB
-        if self.is_rgb(image):
-            # Если да, то преобразуем его в оттенки серого
-            gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-            # Приводим значения пикселей к диапазону от 0 до 255
-            gray_image = cv2.convertScaleAbs(gray_image)
-            return gray_image
-        # Иначе, возвращаем изображение без изменений
-        return image
-
-    def to_ndarray(self, image: Union[bytes, np.ndarray, Image.Image, str], grayscale: bool = True) -> np.ndarray:
-        """
-        Преобразует входные данные из различных типов в ndarray (NumPy array).
-
-        Аргументы:
-        - image: Union[bytes, np.ndarray, Image.Image, str] - Входные данные,
-          представляющие изображение. Может быть типами bytes, np.ndarray, PIL Image или str.
-
-        Возвращает:
-        - np.ndarray - Преобразованный массив NumPy (ndarray) представляющий изображение.
-        """
-        # Если входные данные являются массивом байтов, преобразовать их в массив NumPy
-        if isinstance(image, bytes):
-            image = cv2.imdecode(np.frombuffer(image, np.uint8), cv2.IMREAD_COLOR)
-
-        # Если входные данные являются строкой с путем к файлу, открыть изображение и преобразовать в массив NumPy
-        if isinstance(image, str):
-            # image = np.array(Image.open(image))
-            image = cv2.imread(image, cv2.IMREAD_COLOR)
-
-        # Если входные данные являются объектом PIL Image, преобразовать его в массив NumPy
-        if isinstance(image, Image.Image):
-            image = np.array(image)
-
-        # Вернуть преобразованный массив NumPy
-        if grayscale:
-            return self.to_grayscale(image=image)
-        return image
+# coding: utf-8
+import base64
+import logging
+import os
+from typing import Union, List, Tuple, Optional
+
+import cv2
+import numpy as np
+from PIL import Image
+from pytesseract import pytesseract
+
+from selenium.common.exceptions import WebDriverException
+
+import config
+from adb import adb
+from AppiumHelpers.helpers_decorators import retry
+
+
+class AppiumImage(object):
+    """
+    Класс работы с Appium.
+    Обеспечивает работу с изображениями
+    """
+
+    def __init__(self, driver=None):
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        self.driver = driver
+
+    def get_screenshot_as_base64_decoded(self):
+        screenshot = self.driver.get_screenshot_as_base64().encode('utf-8')
+        screenshot = base64.b64decode(screenshot)
+        return screenshot
+
+    @retry
+    def get_image_coordinates(self,
+                              image: Union[bytes, np.ndarray, Image.Image, str],
+                              full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                              threshold: Optional[float] = 0.7,
+                              ) -> Union[Tuple[int, int, int, int], None]:
+        """
+        Находит координаты наиболее вероятного совпадения частичного изображения в полном изображении.
+        Предназначен для поиска координат наиболее вероятного совпадения частичного изображения в полном изображении.
+
+        Args:
+            image (Union[bytes, np.ndarray, Image.Image, str]): путь к файлу частичного изображения, которое
+            нужно найти внутри полного изображения.
+            full_image (Union[bytes, np.ndarray, Image.Image, str]): путь к файлу полного изображения.
+            threshold (float, optional): минимальный порог совпадения, необходимый для считывания совпадения допустимым.
+                По умолчанию равно 0.7.
+
+        Returns:
+            tuple or None: кортеж с координатами наиболее вероятного совпадения (x1, y1, x2, y2) или None, если совпадение не найдено.
+            :param threshold:
+            :param full_image:
+        """
+        if full_image is None:
+            screenshot = self.get_screenshot_as_base64_decoded()
+            big_image = self.to_ndarray(image=screenshot, grayscale=True)
+        else:
+            big_image = self.to_ndarray(image=full_image, grayscale=True)  # Загрузка полного изображения
+
+        small_image = self.to_ndarray(image=image, grayscale=True)  # Загрузка частичного изображения
+
+        result = cv2.matchTemplate(big_image, small_image, cv2.TM_CCOEFF_NORMED)  # Поиск совпадений методом шаблона
+
+        min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(
+            result)  # Получение наименьшего и наибольшего значения, а также соответствующих координат
+
+        if not max_val >= threshold:  # Если наибольшее значение совпадения не превышает порога, возвращаем None
+            self.logger.error("find_coordinates_by_image(): Совпадений не найдено")
+            return None
+
+        # Вычисляем координаты левого верхнего и правого нижнего углов найденного совпадения
+        left = int(max_loc[0])
+        top = int(max_loc[1])
+        width = small_image.shape[1]
+        height = small_image.shape[0]
+        right = left + width
+        bottom = top + height
+
+        return int(left), int(top), int(right), int(bottom)  # Возвращаем координаты наиболее вероятного совпадения
+
+    @retry
+    def get_inner_image_coordinates(self,
+                                    outer_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                    inner_image_path: Union[bytes, np.ndarray, Image.Image, str],
+                                    threshold: float = 0.9) -> Union[Tuple[int, int, int, int], None]:
+        """
+        Находит изображение на экране и внутри него находит другое изображение (внутреннее).
+        Предназначен для поиска изображения на экране и затем нахождения другого изображения (внутреннего)
+        внутри этого обнаруженного изображения.
+
+        Параметры:
+            outer_image_path (str): Путь к файлу с изображением, которое нужно найти на экране.
+            inner_image_path (str): Путь к файлу с изображением, которое нужно найти внутри внешнего изображения.
+            threshold (float, optional): Пороговое значение сходства для шаблонного сопоставления. По умолчанию 0.9.
+
+        Возвращает:
+            tuple: Координаты внутреннего изображения относительно экрана в формате ((x1, y1), (x2, y2)).
+                   Если внутреннее изображение не найдено, возвращает None.
+        """
+        # Получаем разрешение экрана
+        screen_width, screen_height = adb.get_screen_resolution()
+
+        # Захватываем скриншот
+        screenshot = base64.b64decode(self.driver.get_screenshot_as_base64())
+
+        # Читаем скриншот
+        full_image = self.to_ndarray(image=screenshot, grayscale=True)
+
+        # Прочитать внешнее изображение
+        outer_image = self.to_ndarray(image=outer_image_path, grayscale=True)
+
+        # Прочитать внутреннее изображение
+        inner_image = self.to_ndarray(image=inner_image_path, grayscale=True)
+
+        # Вычисляем коэффициенты масштабирования
+        width_ratio = screen_width / full_image.shape[1]
+        height_ratio = screen_height / full_image.shape[0]
+
+        # ...
+        inner_image = cv2.resize(inner_image, None, fx=width_ratio, fy=height_ratio)
+        outer_image = cv2.resize(outer_image, None, fx=width_ratio, fy=height_ratio)
+
+        # Применить шаблонное сопоставление для поиска внешнего изображения
+        outer_result = cv2.matchTemplate(full_image, outer_image, cv2.TM_CCOEFF_NORMED)
+
+        # Найти максимальное значение сходства и его положение для внешнего изображения
+        _, outer_max_val, _, outer_max_loc = cv2.minMaxLoc(outer_result)
+
+        # Проверить, превышает ли максимальное значение сходства для внешнего изображения пороговое значение
+        if outer_max_val >= threshold:
+            # Получить размеры внешнего изображения
+            outer_height, outer_width = outer_image.shape
+
+            # Вычислить координаты внешнего изображения на экране
+            outer_top_left = outer_max_loc
+            outer_bottom_right = (outer_top_left[0] + outer_width, outer_top_left[1] + outer_height)
+
+            # Извлечь область интереса (ROI), содержащую внешнее изображение
+            outer_roi = full_image[outer_top_left[1]:outer_bottom_right[1], outer_top_left[0]:outer_bottom_right[0]]
+
+            # Применить шаблонное сопоставление для поиска внутреннего изображения внутри ROI
+            inner_result = cv2.matchTemplate(outer_roi, inner_image, cv2.TM_CCOEFF_NORMED)
+
+            # Найти максимальное значение сходства и его положение для внутреннего изображения внутри ROI
+            _, inner_max_val, _, inner_max_loc = cv2.minMaxLoc(inner_result)
+
+            # Проверить, превышает ли максимальное значение сходства для внутреннего изображения пороговое значение
+            if inner_max_val >= threshold:
+                # Получить размеры внутреннего изображения
+                inner_height, inner_width = inner_image.shape
+
+                # Вычислить координаты внутреннего изображения относительно экрана
+                inner_top_left = (outer_top_left[0] + inner_max_loc[0], outer_top_left[1] + inner_max_loc[1])
+                inner_bottom_right = (inner_top_left[0] + inner_width, inner_top_left[1] + inner_height)
+
+                # Вернуть координаты внутреннего изображения относительно экрана
+                return inner_top_left + inner_bottom_right
+
+        # Вернуть None, если внутреннее изображение не найдено
+        return None
+
+    def is_image_on_the_screen(self,
+                               image: Union[bytes, np.ndarray, Image.Image, str],
+                               threshold: float = 0.9) -> bool:
+        """
+        Сравнивает, присутствует ли заданное изображение на экране.
+
+        Args:
+            image: Строка, содержащая имя файла частичного изображения для поиска.
+            threshold: Пороговое значение схожести части изображения со снимком экрана
+
+        Returns:
+            Логическое значение, указывающее, было ли частичное изображение найдено на экране.
+        """
+        screenshot = self.get_screenshot_as_base64_decoded()
+
+        # Чтение снимка экрана и частичного изображения
+        full_image = self.to_ndarray(image=screenshot, grayscale=True)
+        small_image = self.to_ndarray(image=image, grayscale=True)
+
+        # Сопоставление частичного изображения и снимка экрана
+        result = cv2.matchTemplate(full_image, small_image, cv2.TM_CCOEFF_NORMED)
+
+        # Извлечение коэффициента схожести и координат схожего участка
+        _, max_val, _, max_loc = cv2.minMaxLoc(result)
+
+        # Логирование
+        self.logger.debug(f"Коэффициент схожести изображения: {max_val}")
+
+        # Сравнение коэффициента схожести и порогового значения
+        if max_val >= threshold:
+            return True
+        else:
+            return False
+
+    def is_text_on_ocr_screen(self,
+                              text: str,
+                              screen: Union[bytes, np.ndarray, Image.Image, str] = None,
+                              language: str = 'rus'
+                              ) -> bool:
+        """
+        Проверяет, присутствует ли заданный текст на экране.
+        Распознавание текста производит с помощью библиотеки pytesseract.
+
+        Аргументы:
+        - text (str): Текст, который нужно найти на экране.
+        - screen (bytes, optional): Скриншот в формате bytes. Если не указан, будет захвачен скриншот с помощью `self.driver`.
+        - language (str): Язык распознавания текста. Значение по умолчанию: 'rus'.
+
+        Возвращает:
+        - bool: True, если заданный текст найден на экране. False в противном случае.
+        """
+        if screen is None:
+            screenshot = self.get_screenshot_as_base64_decoded()
+            image = self.to_ndarray(screenshot)
+        else:
+            image = self.to_ndarray(screen)
+
+        # Бинаризация изображения
+        _, image_bin = cv2.threshold(image, 0, 255,
+                                     cv2.THRESH_BINARY | cv2.THRESH_OTSU)  # Применение бинаризации для получения двоичного изображения
+
+        # Преобразование двоичного изображения в текст
+        ocr_text = pytesseract.image_to_string(image_bin, lang=language)
+
+        # Проверка наличия заданного текста в распознанном тексте
+        if text.lower() in ocr_text.lower():
+            return True
+        else:
+            return False
+
+    @retry
+    def get_many_coordinates_of_image(self,
+                                      image: Union[bytes, np.ndarray, Image.Image, str],
+                                      full_image: Union[bytes, np.ndarray, Image.Image, str] = None,
+                                      cv_threshold: float = 0.7,
+                                      coord_threshold: int = 5) -> Union[List[Tuple], None]:
+        """
+        Находит все вхождения частичного изображения внутри полного изображения.
+
+        Args:
+            full_image (str): путь к файлу полного изображения.
+            image (str): путь к файлу частичного изображения, которое нужно найти внутри полного изображения.
+            cv_threshold (float, optional): минимальный порог совпадения, необходимый для считывания совпадения допустимым.
+                По умолчанию равно 0.7.
+            coord_threshold (int, optional): целое число, представляющее максимальное различие между значениями x и y двух
+                кортежей, чтобы они считались слишком близкими друг к другу. По умолчанию равно 5.
+
+        Returns:
+            list of tuples or None: список кортежей, содержащий расположение каждого найденного совпадения.
+                Если совпадений не найдено, возвращается None.
+        """
+
+        if full_image is None:
+            screenshot = self.get_screenshot_as_base64_decoded()
+            big_image = self.to_ndarray(image=screenshot, grayscale=True)
+        else:
+            big_image = self.to_ndarray(image=full_image, grayscale=True)  # Загрузка полного изображения
+
+        small_image = self.to_ndarray(image=image, grayscale=True)  # Загрузка частичного изображения
+
+        # Найти частичное изображение в полном изображении
+        result = cv2.matchTemplate(big_image, small_image, cv2.TM_CCOEFF_NORMED)  # Поиск совпадений методом шаблона
+
+        # Получить все совпадения выше порога
+        locations = np.where(result >= cv_threshold)  # Нахождение всех совпадений выше порога
+        matches = list(zip(*locations[::-1]))  # Преобразование координат в список кортежей
+
+        # Фильтрация слишком близких совпадений
+        unique_list = []  # Создаем пустой список для хранения уникальных кортежей
+        for i, (x1, y1) in enumerate(matches):  # Итерируемся по списку кортежей
+            exclude = False  # Инициализируем флаг exclude значением False
+            for (x2, y2) in unique_list:  # Итерируемся по уникальным кортежам
+                if abs(x1 - x2) <= coord_threshold and abs(y1 - y2) <= coord_threshold:
+                    # Если различие между значениями x и y двух кортежей меньше или равно порогу,
+                    # помечаем exclude как True и выходим из цикла
+                    exclude = True
+                    break
+            if not exclude:  # Если exclude равно False, добавляем кортеж в unique_list
+                unique_list.append((x1, y1))
+        matches = unique_list
+
+        if not matches:
+            self.logger.error(f"_find_many_coordinates_by_image() NO MATCHES, {image=}")
+            return None
+
+        # Добавляем правый нижний угол к каждому найденному совпадению
+        matches_with_corners = []
+        for match in matches:
+            x, y = match
+            w, h = small_image.shape[::-1]
+            top_left = (x, y)
+            bottom_right = (x + w, y + h)
+            matches_with_corners.append((top_left + bottom_right))
+
+        return matches_with_corners
+
+    @retry
+    def get_text_coordinates(
+            self,
+            text: str,
+            image: Union[bytes, str, Image.Image, np.ndarray] = None,
+            language: str = 'rus'
+    ) -> Union[Tuple[int, int, int, int], None]:
+        """
+        Возвращает координаты области с указанным текстом на предоставленном изображении или снимке экрана.
+
+        Аргументы:
+        - text (str): Искомый текст.
+        - image (bytes, str, Image.Image, np.ndarray, опционально): Изображение, на котором осуществляется поиск текста.
+          Если не указано, будет использован снимок экрана. По умолчанию None.
+        - language (str, опционально): Язык для распознавания текста. По умолчанию 'rus'.
+
+        Возвращает:
+        - Union[Tuple[int, int, int, int], None]: Координаты области с текстом или None, если текст не найден.
+        """
+
+        if not image:
+            # Получаем снимок экрана, если изображение не предоставлено
+            screenshot = self.get_screenshot_as_base64_decoded()  # Получение снимка экрана в формате base64
+            image = self.to_ndarray(image=screenshot,
+                                    grayscale=True)  # Преобразование снимка экрана в массив numpy и преобразование в оттенки серого
+        else:
+            # Если предоставлено, то преобразуем
+            image = self.to_ndarray(image=image,
+                                    grayscale=True)  # Преобразование изображения в массив numpy и преобразование в оттенки серого
+
+        # Бинаризация изображения
+        _, threshold = cv2.threshold(image, 0, 255,
+                                     cv2.THRESH_BINARY | cv2.THRESH_OTSU)  # Применение бинаризации для получения двоичного изображения
+
+        # Выполнение OCR с помощью PyTesseract
+        data = pytesseract.image_to_data(threshold, lang=language,
+                                         output_type=pytesseract.Output.DICT)  # Использование PyTesseract для распознавания текста и получения информации о распознанных словах
+
+        formatted_data = {}
+        for i in range(len(data['text'])):
+            word_text = data['text'][i]  # Текст слова
+            left = int(data['left'][i])  # Координата левой границы слова
+            top = int(data['top'][i])  # Координата верхней границы слова
+            width = int(data['width'][i])  # Ширина слова
+            height = int(data['height'][i])  # Высота слова
+            coordinates = [left, top, left + width, top + height]  # Координаты рамки слова
+
+            if word_text:
+                if i not in formatted_data:
+                    formatted_data[i] = {}
+                formatted_data[i] = {'text': word_text,
+                                     'coordinates': coordinates}  # Сохранение информации о слове и его координатах
+
+        # Разбить искомый текст на отдельные слова
+        words = text.split(' ')  # Разделение искомого текста на отдельные слова
+
+        # Инициализировать переменные для последовательности слов и соответствующих координат
+        current_sequence = []  # Текущая последовательность слов
+        result_coordinates = []  # Координаты текущей последовательности слов
+
+        for index, word_data in formatted_data.items():
+            word = word_data['text']  # Текущее слово
+            coordinates = word_data['coordinates']  # Координаты слова
+
+            if word in words:
+                current_sequence.append(word)  # Добавление слова в текущую последовательность
+                result_coordinates.append(coordinates)  # Добавление координат слова в результат
+            else:
+                if current_sequence == words:
+                    # Если найдена последовательность слов, вернуть соответствующие координаты
+                    top_left = tuple(map(int, result_coordinates[0][:2]))  # Верхний левый угол рамки
+                    bottom_right = tuple(map(int, result_coordinates[-1][2:]))  # Нижний правый угол рамки
+                    return top_left + bottom_right
+                current_sequence = []  # Сброс текущей последовательности слов
+                result_coordinates = []  # Сброс координат последовательности слов
+
+        return None
+
+    def draw_by_coordinates(self,
+                            image: Union[bytes, str, Image.Image, np.ndarray] = None,
+                            coordinates: Tuple[int, int, int, int] = None,
+                            top_left: Tuple[int, int] = None,
+                            bottom_right: Tuple[int, int] = None,
+                            path: str = None) -> bool:
+        """
+        Рисует прямоугольник на предоставленном изображении или снимке экрана с помощью драйвера.
+        Прямоугольник определяется либо координатами, либо верхней левой и нижней правой точками.
+        Результирующее изображение с нарисованным прямоугольником сохраняется по указанному пути.
+
+        Аргументы:
+            image (Union[bytes, str, Image.Image], опционально): Изображение, на котором будет рисоваться.
+                Может быть представлено в виде bytes, str (путь до файла) или PIL Image.
+                Если не указано, используется снимок экрана. По умолчанию None.
+            coordinates (Tuple[int, int, int, int], опционально): Координаты прямоугольника (x1, y1, x2, y2).
+                По умолчанию None.
+            top_left (Tuple[int, int], опционально): Верхняя левая точка прямоугольника (x, y). По умолчанию None.
+            bottom_right (Tuple[int, int], опционально): Нижняя правая точка прямоугольника (x, y). По умолчанию None.
+            path (str, опционально): Путь для сохранения результирующего изображения. По умолчанию None.
+
+        Usage:
+            image = self.driver.get_screenshot_as_base64().encode('utf-8')
+            draw_by_coordinates(image=image, coordinates=(123, 123, 123, 123), path='pictures')
+
+        Возвращает:
+            bool: True, если операция выполнена успешно, False в противном случае.
+        """
+        try:
+            if image is None:
+                # Если изображение не предоставлено, получаем снимок экрана с помощью драйвера
+                screenshot = self.get_screenshot_as_base64_decoded()
+                image = self.to_ndarray(screenshot)
+            else:
+                image = self.to_ndarray(image)
+
+            # Если верхняя левая и нижняя правая точки не предоставлены, используем координаты для определения
+            # прямоугольника
+            if not top_left and not bottom_right:
+                top_left = (coordinates[0], coordinates[1])
+                bottom_right = (coordinates[2], coordinates[3])
+
+            # Сохраняем снимок экрана с нарисованным прямоугольником
+            if path is None:
+                path = "screenshot_with_text_coordinates.png"
+            path = os.path.join(path)
+            cv2.rectangle(image, top_left, bottom_right, (0, 255, 0), 2)
+            cv2.imwrite(path, image)
+
+            return True
+        except WebDriverException as e:
+            # Обрабатываем исключение WebDriverException и записываем ошибку в журнал
+            self.logger.error(f'draw_by_coordinates() WebDriverException {e}')
+            return False
+        except cv2.error as e:
+            # Обработка исключения cv2.error
+            self.logger.error(f'draw_by_coordinates() cv2.error: {e}')
+            return False
+
+    @staticmethod
+    def is_rgb(image: np.ndarray) -> bool:
+        """
+        Проверяет, является ли изображение цветным (RGB).
+
+        Аргументы:
+        - image: np.ndarray - Входное изображение в формате NumPy ndarray.
+
+        Возвращает:
+        - bool - True, если изображение является цветным (RGB), False - в противном случае.
+        """
+        return len(image.shape) == 3 and image.shape[2] == 3 or image.ndim == 3 or image.ndim == '3'
+
+    @staticmethod
+    def is_grayscale(image: np.ndarray) -> bool:
+        """
+        Проверяет, является ли изображение оттенков серого.
+
+        Аргументы:
+        - image: np.ndarray - Входное изображение в формате NumPy ndarray.
+
+        Возвращает:
+        - bool - True, если изображение является оттенков серого, False - в противном случае.
+        """
+        return len(image.shape) == 2 or (
+                len(image.shape) == 3 and image.shape[2] == 1) or image.ndim == 2 or image.ndim == '2'
+
+    def to_grayscale(self, image: np.ndarray) -> np.ndarray:
+        """
+        Преобразует изображение в оттенки серого.
+
+        Аргументы:
+        - image: np.ndarray - Входное изображение в формате ndarray.
+
+        Возвращает:
+        - np.ndarray - Преобразованное изображение в оттенках серого.
+        """
+        # Проверяем, является ли изображение в формате RGB
+        if self.is_rgb(image):
+            # Если да, то преобразуем его в оттенки серого
+            gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+            # Приводим значения пикселей к диапазону от 0 до 255
+            gray_image = cv2.convertScaleAbs(gray_image)
+            return gray_image
+        # Иначе, возвращаем изображение без изменений
+        return image
+
+    def to_ndarray(self, image: Union[bytes, np.ndarray, Image.Image, str], grayscale: bool = True) -> np.ndarray:
+        """
+        Преобразует входные данные из различных типов в ndarray (NumPy array).
+
+        Аргументы:
+        - image: Union[bytes, np.ndarray, Image.Image, str] - Входные данные,
+          представляющие изображение. Может быть типами bytes, np.ndarray, PIL Image или str.
+
+        Возвращает:
+        - np.ndarray - Преобразованный массив NumPy (ndarray) представляющий изображение.
+        """
+        # Если входные данные являются массивом байтов, преобразовать их в массив NumPy
+        if isinstance(image, bytes):
+            image = cv2.imdecode(np.frombuffer(image, np.uint8), cv2.IMREAD_COLOR)
+
+        # Если входные данные являются строкой с путем к файлу, открыть изображение и преобразовать в массив NumPy
+        if isinstance(image, str):
+            # image = np.array(Image.open(image))
+            image = cv2.imread(image, cv2.IMREAD_COLOR)
+
+        # Если входные данные являются объектом PIL Image, преобразовать его в массив NumPy
+        if isinstance(image, Image.Image):
+            image = np.array(image)
+
+        # Вернуть преобразованный массив NumPy
+        if grayscale:
+            return self.to_grayscale(image=image)
+        return image
```

### Comparing `AppiumExtended-0.1.3/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.1.6/AppiumHelpers/helpers_decorators.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-# coding: utf-8
-import sys
-import io
-import time
-import functools
-import logging
-from functools import wraps
-from datetime import datetime
-
-import allure
-import numpy as np
-from PIL import Image
-
-import config
-
-logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-
-def retry(func):
-    max_retries = 3
-
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        result = None
-        for _ in range(max_retries):
-            result = func(*args, **kwargs)
-            if result is not None and result is not False:
-                return result
-            else:
-                time.sleep(1)
-        return result
-
-    return wrapper
-
-
-def wait_until_window_change(poll_frequency: float = 0.1):
-    """
-    Декоратор, который ожидает изменения содержимого окна в течение заданного периода времени.
-
-    Аргументы:
-        poll_frequency (float): Частота опроса содержимого окна на наличие изменений в секундах.
-                               По умолчанию 0.1 секунды.
-
-    Возвращает:
-        function: Декорированная функция.
-    """
-
-    def func_decorator(func):
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            """
-            Оберточная функция, которая инкапсулирует декорированную функцию с логикой обнаружения изменений окна.
-
-            Аргументы:
-                self: Экземпляр класса, к которому принадлежит декорированный метод.
-                *args: Произвольное число аргументов, переданных в декорированный метод.
-                **kwargs: Произвольное число именованных аргументов, переданных в декорированный метод.
-
-            Возвращает:
-                bool: True, если содержимое окна изменяется в течение заданного периода времени, иначе False.
-            """
-            print("wait_until_window_change")
-
-            # Инициализация
-            result = False
-            func_result = None
-            decorator_args = kwargs.get('decorator_args', {})
-            timeout_window = decorator_args.get('timeout_window', 30)
-            window_not_changing_period = decorator_args.get('window_not_changing_period', 10)
-
-            start_time = time.time()  # Запись начального времени
-            print("func_result = func(self, *args, **kwargs)")
-            func_result = func(self, *args, **kwargs)  # Вызов декорированной функции и сохранение результата
-            print("func_result: ", func_result)
-
-            # Обнаружение изменений экрана с экспоненциальной задержкой
-            poll_interval = poll_frequency
-            while time.time() - start_time < timeout_window:  # Продолжаем до достижения тайм-аута
-                window_not_changing_period_start_time = time.time()  # Запускаем новый период, в течение которого окно не изменяется
-                window_not_changed = True  # Флаг для отслеживания того, изменилось ли окно за период
-
-                while time.time() - window_not_changing_period_start_time < window_not_changing_period:
-                    # Делаем снимок экрана и сохраняем его в памяти
-                    # self.driver.set_window_size(800, 600)  # Установить меньшее разрешение, если необходимо
-                    image_bytes = self.driver.get_screenshot_as_png()
-                    image = Image.open(io.BytesIO(image_bytes)).convert('L')  # Преобразуем в оттенки серого
-                    # Обрезаем снимок до определенной области
-                    box = (50, 50, 400, 400)  # Определяем координаты для обрезки (лево, верх, право, низ)
-                    image = image.crop(box)
-
-                    time.sleep(poll_interval)  # Ждем указанный интервал между опросами
-                    new_image_bytes = self.driver.get_screenshot_as_png()
-                    new_image = Image.open(io.BytesIO(new_image_bytes)).convert('L')  # Преобразуем в оттенки серого
-                    new_image = new_image.crop(box)
-
-                    # Проверяем, отличается ли сумма значений пикселей на двух изображениях
-                    if np.sum(image) != np.sum(new_image):
-                        window_not_changed = False  # Содержимое окна изменилось
-                        break
-
-                if window_not_changed:
-                    logger.debug("Содержимое окна не изменялось в течение периода")
-                    return True
-
-                poll_interval *= 2  # Удваиваем время ожидания для каждого опроса
-
-            if not result:
-                logger.info(f"{func.__name__}() > {func_result}. Изменение экрана: False")
-                return False
-
-        return wrapper
-
-    return func_decorator
-
-
-def wait_for_window_change(poll_frequency: float = 0.5):
-    """
-    Декоратор, который ожидает изменения окна перед выполнением декорированной функции.
-    Он делает снимок экрана окна, обрезает его и сравнивает с последующими снимками,
-    чтобы обнаружить любые изменения.
-
-    Аргументы:
-        poll_frequency (float): Частота проверки окна на изменения.
-
-    Возвращает:
-        Декоратор функции.
-    """
-
-    def func_decorator(func):
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            """
-            Оберточная функция, которая выполняет обнаружение изменения окна и выполнение декорированной функции.
-
-            Аргументы:
-                self: Экземпляр класса, содержащего декорированную функцию.
-                *args: Переменное число аргументов.
-                **kwargs: Произвольные именованные аргументы.
-
-            Возвращает:
-                Результат декорированной функции или False, если изменение окна не было обнаружено.
-            """
-
-            # Инициализация
-            result = False
-            func_result = None
-            decorator_args = kwargs.get('decorator_args', {})
-            timeout_window = decorator_args.get('timeout_window', 10)
-            tries = decorator_args.get('tries', 3)
-
-            # Сделать снимок экрана и сохранить его в памяти
-            image_bytes = self.driver.get_screenshot_as_png()  # Сделать снимок экрана окна и получить данные изображения в виде байтов
-            image = Image.open(io.BytesIO(image_bytes)).convert(
-                'L')  # Открыть изображение из байтов и преобразовать его в оттенки серого
-
-            # Обрезать снимок экрана до определенной области
-            box = (50, 50, 400, 400)  # Определить координаты прямоугольной области для обрезки (лево, верх, право, низ)
-            image = image.crop(box)  # Обрезать изображение на основе заданных координат области
-
-            # Попытаться обнаружить изменение экрана
-            for _ in range(tries):  # Выполнить попытки обнаружения на основе заданного числа попыток
-                start_time = time.time()  # Записать текущее время начала попытки обнаружения
-                func_result = func(self, *args, **kwargs)  # Выполнить декорированную функцию и сохранить результат
-
-                # Обнаружить изменение экрана с экспоненциальной задержкой
-                poll_interval = poll_frequency  # Установить начальный интервал проверки равным заданной частоте проверки
-                while time.time() - start_time < timeout_window:  # Проверить, находится ли прошедшее время в пределах заданного окна времени ожидания
-                    time.sleep(poll_interval)  # Приостановить выполнение на заданный интервал проверки
-                    new_image_bytes = self.driver.get_screenshot_as_png()  # Сделать новый снимок экрана окна и получить данные изображения в виде байтов
-                    new_image = Image.open(io.BytesIO(new_image_bytes)).convert(
-                        'L')  # Открыть новое изображение из байтов и преобразовать его в оттенки серого
-                    new_image = new_image.crop(box)  # Обрезать новое изображение на основе заданных координат области
-
-                    if not np.sum(image) == np.sum(
-                            new_image):  # Сравнить суммы значений пикселей между исходным и новым изображениями
-                        logger.debug(
-                            "Изменение экрана обнаружено")  # Записать сообщение о том, что произошло изменение экрана
-                        return True  # Вернуть True для обозначения обнаружения изменения экрана
-
-                    poll_interval *= 2  # Удвоить интервал проверки для следующей итерации (экспоненциальная задержка)
-
-            if not result:
-                logger.info(
-                    f"{func.__name__}() > {func_result}. Изменение экрана: False")  # Записать сообщение о том, что изменение экрана не было обнаружено
-                return False  # Вернуть False для обозначения отсутствия обнаружения изменения экрана
-
-        return wrapper
-
-    return func_decorator
-
-
-def time_it(func):
-    def wrapper(*args, **kwargs):
-        start_time = time.time()
-        result = func(*args, **kwargs)
-        end_time = time.time()
-        execution_time = end_time - start_time
-        print(f"Execution time of {func.__name__}: {execution_time:.2f} seconds")
-        return result
-
-    return wrapper
-
-
-def step_info(my_str):
-    """
-    Декоратор, который перед вызовом метода вызывает logger.info и @allure.step,
-    передавая в них строковую переменную, принятую в параметрах.
-
-    Аргументы:
-        my_str (str): Строковая переменная для использования в logger.info и @allure.step.
-
-    Возвращает:
-        function: Декоратор функций.
-
-    Пример использования:
-        @my_step_info("Мой шаг")
-        def my_function():
-            ...
-    """
-
-    # Определяем декоратор функций
-    def func_decorator(func):
-        # Создаем обертку функции, сохраняющую метаданные исходной функции
-        @allure.step(my_str)
-        def wrapper(*args, **kwargs):
-            # Логируем информацию перед вызовом метода
-            logger.info(my_str)
-            # Выполняем исходную функцию
-            result = func(*args, **kwargs)
-            # Логируем информацию после успешного выполнения метода
-            logger.info(f"{my_str} [выполнено успешно]")
-            # Возвращаем результат выполнения исходной функции
-            return result
-
-        # Возвращаем обертку функции
-        return wrapper
-
-    # Возвращаем декоратор функций
-    return func_decorator
-
-
-def screenshots():
-    """
-    В случае возникновения AssertionError в обернутом методе - прикрепляет к allure report скриншот до выполнения
-    метода и после возникновения исключения, а также информацию об ошибке.
-    В ином случае скриншот не прикрепляется.
-    """
-
-    # Определяем декоратор функций
-    def func_decorator(func):
-        # Создаем обертку функции, сохраняющую метаданные исходной функции
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            # Получаем скриншот до вызова метода
-            screenshot = self.driver.get_screenshot_as_png()
-            # Генерируем временную метку для имени скриншота
-            timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
-            # Устанавливаем имя скриншота до вызова метода
-            screenshot_name_begin = f"screenshot_begin_{timestamp}.png"
-            try:
-                # Выполняем исходную функцию
-                result = func(self, *args, **kwargs)
-            except AssertionError as e:
-                # Если произошло исключение, прикрепляем скриншот до вызова метода к отчету
-                allure.attach(screenshot, name=screenshot_name_begin, attachment_type=allure.attachment_type.PNG)
-                # Прикрепляем информацию об ошибке AssertionError к отчету
-                allure.attach(str(e), name="AssertionError", attachment_type=allure.attachment_type.TEXT)
-                # Рейзим исключение AssertionError с сохраненным traceback
-                raise AssertionError(str(e)).with_traceback(sys.exc_info()[2])
-            finally:
-                # Получаем скриншот после вызова метода
-                screenshot = self.driver.get_screenshot_as_png()
-                # Обновляем временную метку для имени скриншота
-                timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
-                # Устанавливаем имя скриншота после вызова метода
-                screenshot_name_end = f"screenshot_end_{timestamp}.png"
-                # Прикрепляем скриншот после вызова метода к отчету
-                allure.attach(screenshot, name=screenshot_name_end, attachment_type=allure.attachment_type.PNG)
-            # Возвращаем результат выполнения исходной функции
-            return result
-
-        # Возвращаем обертку функции
-        return wrapper
-
-    # Возвращаем декоратор функций
-    return func_decorator
-
-
-def log_debug():
-    """
-    Логирует начало и завершение обернутого метода
-    """
-
-    # Определяем декоратор функций
-    def func_decorator(func):
-        # Создаем обертку функции, сохраняющую метаданные исходной функции
-        def wrapper(*args, **kwargs):
-            # Получаем имя метода
-            method_name = func.__name__
-            # Логируем начало выполнения метода и переданные аргументы
-            logger.debug(f"{method_name}() < {', '.join(map(str, args))}, "
-                         f"{', '.join(f'{k}={v}' for k, v in kwargs.items())}")
-            # Выполняем исходную функцию
-            result = func(*args, **kwargs)
-            # Если результат существует, логируем его
-            if result:
-                logger.debug(f"{method_name}() > {str(result)}")
-            # Возвращаем результат выполнения исходной функции
-            return result
-
-        # Возвращаем обертку функции
-        return wrapper
-
-    # Возвращаем декоратор функций
-    return func_decorator
-
-
-def print_me():
-    """
-    Печатает начало и завершение обернутого метода
-    """
-
-    # Определяем декоратор функций
-    def func_decorator(func):
-        # Создаем обертку функции, сохраняющую метаданные исходной функции
-        def wrapper(*args, **kwargs):
-            # Получаем имя метода
-            method_name = func.__name__
-            # Печатаем начало выполнения метода и переданные аргументы
-            print(f"{method_name}() < {', '.join(map(str, args))}, "
-                  f"{', '.join(f'{k}={v}' for k, v in kwargs.items())}")
-            # Выполняем исходную функцию
-            result = func(*args, **kwargs)
-            # Если результат существует, логируем его
-            if result:
-                print(f"{method_name}() > {str(result)}")
-            # Возвращаем результат выполнения исходной функции
-            return result
-
-        # Возвращаем обертку функции
-        return wrapper
-
-    # Возвращаем декоратор функций
-    return func_decorator
+# coding: utf-8
+import sys
+import io
+import time
+import functools
+import logging
+from functools import wraps
+from datetime import datetime
+
+import allure
+import numpy as np
+from PIL import Image
+
+import config
+
+logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+
+def retry(func):
+    max_retries = 3
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        result = None
+        for _ in range(max_retries):
+            result = func(*args, **kwargs)
+            if result is not None and result is not False:
+                return result
+            else:
+                time.sleep(1)
+        return result
+
+    return wrapper
+
+
+def wait_until_window_change(poll_frequency: float = 0.1):
+    """
+    Декоратор, который ожидает изменения содержимого окна в течение заданного периода времени.
+
+    Аргументы:
+        poll_frequency (float): Частота опроса содержимого окна на наличие изменений в секундах.
+                               По умолчанию 0.1 секунды.
+
+    Возвращает:
+        function: Декорированная функция.
+    """
+
+    def func_decorator(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            """
+            Оберточная функция, которая инкапсулирует декорированную функцию с логикой обнаружения изменений окна.
+
+            Аргументы:
+                self: Экземпляр класса, к которому принадлежит декорированный метод.
+                *args: Произвольное число аргументов, переданных в декорированный метод.
+                **kwargs: Произвольное число именованных аргументов, переданных в декорированный метод.
+
+            Возвращает:
+                bool: True, если содержимое окна изменяется в течение заданного периода времени, иначе False.
+            """
+            print("wait_until_window_change")
+
+            # Инициализация
+            result = False
+            func_result = None
+            decorator_args = kwargs.get('decorator_args', {})
+            timeout_window = decorator_args.get('timeout_window', 30)
+            window_not_changing_period = decorator_args.get('window_not_changing_period', 10)
+
+            start_time = time.time()  # Запись начального времени
+            print("func_result = func(self, *args, **kwargs)")
+            func_result = func(self, *args, **kwargs)  # Вызов декорированной функции и сохранение результата
+            print("func_result: ", func_result)
+
+            # Обнаружение изменений экрана с экспоненциальной задержкой
+            poll_interval = poll_frequency
+            while time.time() - start_time < timeout_window:  # Продолжаем до достижения тайм-аута
+                window_not_changing_period_start_time = time.time()  # Запускаем новый период, в течение которого окно не изменяется
+                window_not_changed = True  # Флаг для отслеживания того, изменилось ли окно за период
+
+                while time.time() - window_not_changing_period_start_time < window_not_changing_period:
+                    # Делаем снимок экрана и сохраняем его в памяти
+                    # self.driver.set_window_size(800, 600)  # Установить меньшее разрешение, если необходимо
+                    image_bytes = self.driver.get_screenshot_as_png()
+                    image = Image.open(io.BytesIO(image_bytes)).convert('L')  # Преобразуем в оттенки серого
+                    # Обрезаем снимок до определенной области
+                    box = (50, 50, 400, 400)  # Определяем координаты для обрезки (лево, верх, право, низ)
+                    image = image.crop(box)
+
+                    time.sleep(poll_interval)  # Ждем указанный интервал между опросами
+                    new_image_bytes = self.driver.get_screenshot_as_png()
+                    new_image = Image.open(io.BytesIO(new_image_bytes)).convert('L')  # Преобразуем в оттенки серого
+                    new_image = new_image.crop(box)
+
+                    # Проверяем, отличается ли сумма значений пикселей на двух изображениях
+                    if np.sum(image) != np.sum(new_image):
+                        window_not_changed = False  # Содержимое окна изменилось
+                        break
+
+                if window_not_changed:
+                    logger.debug("Содержимое окна не изменялось в течение периода")
+                    return True
+
+                poll_interval *= 2  # Удваиваем время ожидания для каждого опроса
+
+            if not result:
+                logger.info(f"{func.__name__}() > {func_result}. Изменение экрана: False")
+                return False
+
+        return wrapper
+
+    return func_decorator
+
+
+def wait_for_window_change(poll_frequency: float = 0.5):
+    """
+    Декоратор, который ожидает изменения окна перед выполнением декорированной функции.
+    Он делает снимок экрана окна, обрезает его и сравнивает с последующими снимками,
+    чтобы обнаружить любые изменения.
+
+    Аргументы:
+        poll_frequency (float): Частота проверки окна на изменения.
+
+    Возвращает:
+        Декоратор функции.
+    """
+
+    def func_decorator(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            """
+            Оберточная функция, которая выполняет обнаружение изменения окна и выполнение декорированной функции.
+
+            Аргументы:
+                self: Экземпляр класса, содержащего декорированную функцию.
+                *args: Переменное число аргументов.
+                **kwargs: Произвольные именованные аргументы.
+
+            Возвращает:
+                Результат декорированной функции или False, если изменение окна не было обнаружено.
+            """
+
+            # Инициализация
+            result = False
+            func_result = None
+            decorator_args = kwargs.get('decorator_args', {})
+            timeout_window = decorator_args.get('timeout_window', 10)
+            tries = decorator_args.get('tries', 3)
+
+            # Сделать снимок экрана и сохранить его в памяти
+            image_bytes = self.driver.get_screenshot_as_png()  # Сделать снимок экрана окна и получить данные изображения в виде байтов
+            image = Image.open(io.BytesIO(image_bytes)).convert(
+                'L')  # Открыть изображение из байтов и преобразовать его в оттенки серого
+
+            # Обрезать снимок экрана до определенной области
+            box = (50, 50, 400, 400)  # Определить координаты прямоугольной области для обрезки (лево, верх, право, низ)
+            image = image.crop(box)  # Обрезать изображение на основе заданных координат области
+
+            # Попытаться обнаружить изменение экрана
+            for _ in range(tries):  # Выполнить попытки обнаружения на основе заданного числа попыток
+                start_time = time.time()  # Записать текущее время начала попытки обнаружения
+                func_result = func(self, *args, **kwargs)  # Выполнить декорированную функцию и сохранить результат
+
+                # Обнаружить изменение экрана с экспоненциальной задержкой
+                poll_interval = poll_frequency  # Установить начальный интервал проверки равным заданной частоте проверки
+                while time.time() - start_time < timeout_window:  # Проверить, находится ли прошедшее время в пределах заданного окна времени ожидания
+                    time.sleep(poll_interval)  # Приостановить выполнение на заданный интервал проверки
+                    new_image_bytes = self.driver.get_screenshot_as_png()  # Сделать новый снимок экрана окна и получить данные изображения в виде байтов
+                    new_image = Image.open(io.BytesIO(new_image_bytes)).convert(
+                        'L')  # Открыть новое изображение из байтов и преобразовать его в оттенки серого
+                    new_image = new_image.crop(box)  # Обрезать новое изображение на основе заданных координат области
+
+                    if not np.sum(image) == np.sum(
+                            new_image):  # Сравнить суммы значений пикселей между исходным и новым изображениями
+                        logger.debug(
+                            "Изменение экрана обнаружено")  # Записать сообщение о том, что произошло изменение экрана
+                        return True  # Вернуть True для обозначения обнаружения изменения экрана
+
+                    poll_interval *= 2  # Удвоить интервал проверки для следующей итерации (экспоненциальная задержка)
+
+            if not result:
+                logger.info(
+                    f"{func.__name__}() > {func_result}. Изменение экрана: False")  # Записать сообщение о том, что изменение экрана не было обнаружено
+                return False  # Вернуть False для обозначения отсутствия обнаружения изменения экрана
+
+        return wrapper
+
+    return func_decorator
+
+
+def time_it(func):
+    def wrapper(*args, **kwargs):
+        start_time = time.time()
+        result = func(*args, **kwargs)
+        end_time = time.time()
+        execution_time = end_time - start_time
+        print(f"Execution time of {func.__name__}: {execution_time:.2f} seconds")
+        return result
+
+    return wrapper
+
+
+def step_info(my_str):
+    """
+    Декоратор, который перед вызовом метода вызывает logger.info и @allure.step,
+    передавая в них строковую переменную, принятую в параметрах.
+
+    Аргументы:
+        my_str (str): Строковая переменная для использования в logger.info и @allure.step.
+
+    Возвращает:
+        function: Декоратор функций.
+
+    Пример использования:
+        @my_step_info("Мой шаг")
+        def my_function():
+            ...
+    """
+
+    # Определяем декоратор функций
+    def func_decorator(func):
+        # Создаем обертку функции, сохраняющую метаданные исходной функции
+        @allure.step(my_str)
+        def wrapper(*args, **kwargs):
+            # Логируем информацию перед вызовом метода
+            logger.info(my_str)
+            # Выполняем исходную функцию
+            result = func(*args, **kwargs)
+            # Логируем информацию после успешного выполнения метода
+            logger.info(f"{my_str} [выполнено успешно]")
+            # Возвращаем результат выполнения исходной функции
+            return result
+
+        # Возвращаем обертку функции
+        return wrapper
+
+    # Возвращаем декоратор функций
+    return func_decorator
+
+
+def screenshots():
+    """
+    В случае возникновения AssertionError в обернутом методе - прикрепляет к allure report скриншот до выполнения
+    метода и после возникновения исключения, а также информацию об ошибке.
+    В ином случае скриншот не прикрепляется.
+    """
+
+    # Определяем декоратор функций
+    def func_decorator(func):
+        # Создаем обертку функции, сохраняющую метаданные исходной функции
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            # Получаем скриншот до вызова метода
+            screenshot = self.driver.get_screenshot_as_png()
+            # Генерируем временную метку для имени скриншота
+            timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+            # Устанавливаем имя скриншота до вызова метода
+            screenshot_name_begin = f"screenshot_begin_{timestamp}.png"
+            try:
+                # Выполняем исходную функцию
+                result = func(self, *args, **kwargs)
+            except AssertionError as e:
+                # Если произошло исключение, прикрепляем скриншот до вызова метода к отчету
+                allure.attach(screenshot, name=screenshot_name_begin, attachment_type=allure.attachment_type.PNG)
+                # Прикрепляем информацию об ошибке AssertionError к отчету
+                allure.attach(str(e), name="AssertionError", attachment_type=allure.attachment_type.TEXT)
+                # Рейзим исключение AssertionError с сохраненным traceback
+                raise AssertionError(str(e)).with_traceback(sys.exc_info()[2])
+            finally:
+                # Получаем скриншот после вызова метода
+                screenshot = self.driver.get_screenshot_as_png()
+                # Обновляем временную метку для имени скриншота
+                timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+                # Устанавливаем имя скриншота после вызова метода
+                screenshot_name_end = f"screenshot_end_{timestamp}.png"
+                # Прикрепляем скриншот после вызова метода к отчету
+                allure.attach(screenshot, name=screenshot_name_end, attachment_type=allure.attachment_type.PNG)
+            # Возвращаем результат выполнения исходной функции
+            return result
+
+        # Возвращаем обертку функции
+        return wrapper
+
+    # Возвращаем декоратор функций
+    return func_decorator
+
+
+def log_debug():
+    """
+    Логирует начало и завершение обернутого метода
+    """
+
+    # Определяем декоратор функций
+    def func_decorator(func):
+        # Создаем обертку функции, сохраняющую метаданные исходной функции
+        def wrapper(*args, **kwargs):
+            # Получаем имя метода
+            method_name = func.__name__
+            # Логируем начало выполнения метода и переданные аргументы
+            logger.debug(f"{method_name}() < {', '.join(map(str, args))}, "
+                         f"{', '.join(f'{k}={v}' for k, v in kwargs.items())}")
+            # Выполняем исходную функцию
+            result = func(*args, **kwargs)
+            # Если результат существует, логируем его
+            if result:
+                logger.debug(f"{method_name}() > {str(result)}")
+            # Возвращаем результат выполнения исходной функции
+            return result
+
+        # Возвращаем обертку функции
+        return wrapper
+
+    # Возвращаем декоратор функций
+    return func_decorator
+
+
+def print_me():
+    """
+    Печатает начало и завершение обернутого метода
+    """
+
+    # Определяем декоратор функций
+    def func_decorator(func):
+        # Создаем обертку функции, сохраняющую метаданные исходной функции
+        def wrapper(*args, **kwargs):
+            # Получаем имя метода
+            method_name = func.__name__
+            # Печатаем начало выполнения метода и переданные аргументы
+            print(f"{method_name}() < {', '.join(map(str, args))}, "
+                  f"{', '.join(f'{k}={v}' for k, v in kwargs.items())}")
+            # Выполняем исходную функцию
+            result = func(*args, **kwargs)
+            # Если результат существует, логируем его
+            if result:
+                print(f"{method_name}() > {str(result)}")
+            # Возвращаем результат выполнения исходной функции
+            return result
+
+        # Возвращаем обертку функции
+        return wrapper
+
+    # Возвращаем декоратор функций
+    return func_decorator
```

### Comparing `AppiumExtended-0.1.3/AppiumServer/appium_server.py` & `AppiumExtended-0.1.6/AppiumServer/appium_server.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# coding: utf-8
-import subprocess
-import time
-
-import requests
-import logging
-
-import config
-
-
-class AppiumServer(object):
-    def __init__(self, port: int = 4723, log_level='error'):
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        self.port = port
-        self.log_level = log_level
-
-    def start(self) -> bool:
-        self.logger.info("Start Appium server")
-        cmd = f'appium server -ka 800 --log-level {self.log_level} --use-plugins=device-farm,appium-dashboard -p {self.port} -a 0.0.0.0 -pa /wd/hub --plugin-device-farm-platform=android'
-        try:
-            subprocess.Popen(cmd, shell=True)
-            return True
-        except subprocess.CalledProcessError:
-            self.logger.error("Error starting Appium server: subprocess.CalledProcessError")
-            return False
-        except OSError:
-            self.logger.error("Error starting Appium server: OSError")
-            return False
-
-    def is_alive(self) -> bool:
-        self.logger.info("Checking Appium server status")
-        try:
-            response = requests.get("http://127.0.0.1:4723/wd/hub/sessions")
-            if response.status_code == 200:
-                self.logger.info("Appium server ready")
-                return True
-            else:
-                self.logger.warning(f"Appium server responded with status code {response.status_code}")
-                return False
-        except requests.exceptions.RequestException as e:
-            self.logger.error(f"Error checking Appium server status: {e}")
-            return False
-
-    def stop(self) -> bool:
-        self.logger.info("Stop Appium server")
-        try:
-            cmd = 'taskkill /F /IM node.exe'
-            subprocess.check_output(cmd, shell=True)
-            return True
-        except subprocess.CalledProcessError:
-            return False
-
-    def wait_until_alive(self, timeout: int = 60, poll: int = 2):
-        self.logger.info("Wait for Appium server")
-        start_time = time.time()
-        while time.time() < start_time + timeout:
-            if self.is_alive():
-                return True
-            time.sleep(poll)
-        return False
+# coding: utf-8
+import subprocess
+import time
+
+import requests
+import logging
+
+import config
+
+
+class AppiumServer(object):
+    def __init__(self, port: int = 4723, log_level='error'):
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        self.port = port
+        self.log_level = log_level
+
+    def start(self) -> bool:
+        self.logger.info("Start Appium server")
+        cmd = f'appium server -ka 800 --log-level {self.log_level} --use-plugins=device-farm,appium-dashboard -p {self.port} -a 0.0.0.0 -pa /wd/hub --plugin-device-farm-platform=android'
+        try:
+            subprocess.Popen(cmd, shell=True)
+            return True
+        except subprocess.CalledProcessError:
+            self.logger.error("Error starting Appium server: subprocess.CalledProcessError")
+            return False
+        except OSError:
+            self.logger.error("Error starting Appium server: OSError")
+            return False
+
+    def is_alive(self) -> bool:
+        self.logger.info("Checking Appium server status")
+        try:
+            response = requests.get("http://127.0.0.1:4723/wd/hub/sessions")
+            if response.status_code == 200:
+                self.logger.info("Appium server ready")
+                return True
+            else:
+                self.logger.warning(f"Appium server responded with status code {response.status_code}")
+                return False
+        except requests.exceptions.RequestException as e:
+            self.logger.error(f"Error checking Appium server status: {e}")
+            return False
+
+    def stop(self) -> bool:
+        self.logger.info("Stop Appium server")
+        try:
+            cmd = 'taskkill /F /IM node.exe'
+            subprocess.check_output(cmd, shell=True)
+            return True
+        except subprocess.CalledProcessError:
+            return False
+
+    def wait_until_alive(self, timeout: int = 60, poll: int = 2):
+        self.logger.info("Wait for Appium server")
+        start_time = time.time()
+        while time.time() < start_time + timeout:
+            if self.is_alive():
+                return True
+            time.sleep(poll)
+        return False
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_adb_actions.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# coding: utf-8
-import logging
-import subprocess
-
-from appium.webdriver import WebElement
-
-import config
-
-from adb import adb
-from AppiumWebElementExtended.web_element_get import WebElementGet
-from AppiumHelpers.helpers_decorators import wait_for_window_change
-from utils.utils import find_coordinates_by_vector
-
-
-class WebElementAdbActions(WebElementGet):
-    """
-    Класс для выполнения adb-действий с элементами.
-    Наследуется от класса WebElementGet.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    def _adb_tap(self,
-                 decorator_args: dict = None,
-                 wait: bool = False) -> bool:
-        """
-        Выполняет нажатие на элемент с помощью adb.
-
-        Аргументы:
-            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
-                timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
-                tries (int): Количество попыток нажатия (по умолчанию 3).
-            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
-
-        Возвращает:
-            bool: True, если нажатие выполнено успешно; False в противном случае.
-        """
-        if wait:
-            # Если нужно ожидать изменения окна.
-            if not decorator_args:
-                decorator_args = {"timeout_window": 5,
-                                  "tries": 5}
-            return self._adb_tap_to_element_and_wait(decorator_args=decorator_args)
-        else:
-            # Если не нужно ожидать изменения окна.
-            return self._adb_tap_to_element()
-
-    def _adb_tap_to_element(self) -> bool:
-        return self.__adb_tap()
-
-    @wait_for_window_change()
-    def _adb_tap_to_element_and_wait(self,
-                                     decorator_args: dict = None) -> bool:
-        return self.__adb_tap()
-
-    def __adb_tap(self) -> bool:
-        """
-        Выполняет нажатие на элемент с помощью adb.
-
-        Возвращает:
-            bool: True, если нажатие выполнено успешно, False в противном случае.
-        """
-        try:
-            x, y = self._get_center()
-            return adb.tap(x=x, y=y)
-        except Exception:
-            return False
-
-    def _adb_multi_tap(self,
-                       decorator_args: dict = None,
-                       wait: bool = False) -> bool:
-        """
-        Выполняет несколько нажатий с помощью adb.
-
-        Args:
-            decorator_args (dict, optional): Дополнительные аргументы для декоратора.
-                По умолчанию None.
-                Если None то будут преобразованы в decorator_args = {"timeout_window": 5, "tries": 5}), где
-                    timeout_window: время ожидания изменения окна в секундах.
-                    tries: количество попыток (выполнения настоящего метода) для изменения окна.
-            wait (bool, optional): Флаг, указывающий, нужно ли ожидать изменение окна после нажатия.
-                По умолчанию False.
-
-        Returns:
-            bool: True, если нажатие выполнено успешно, False в противном случае.
-        """
-        if wait:
-            if not decorator_args:
-                decorator_args = {"timeout_window": 5,
-                                  "tries": 5}
-            return self._adb_multi_tap_to_element_and_wait(decorator_args=decorator_args)
-        else:
-            return self._adb_multi_tap_to_element()
-
-    def _adb_multi_tap_to_element(self) -> bool:
-        """
-        Выполняет три быстрых нажатия с помощью adb.
-        """
-        return self.__adb_multi_tap()
-
-    @wait_for_window_change()
-    def _adb_multi_tap_to_element_and_wait(self,
-                                           decorator_args: dict = None) -> bool:
-        """
-        Выполняет три быстрых нажатия с помощью adb и ожидает изменения окна.
-        """
-        return self.__adb_multi_tap()
-
-    def __adb_multi_tap(self) -> bool:
-        """
-        Выполняет три быстрых нажатия с помощью adb.
-        Если подавать последовательно, через ";", то выполняются с задержкой в пару секунд.
-        Если подавать два тапа, то выполняются одновременно и сливаются.
-        С текущей конфигурацией команды - в 90% нажимает два раза. В 10% нажимает 3 раза.
-        Для выделения текста подходит.
-        """
-        try:
-            x, y = self._get_center()
-            # command = f'adb shell "input tap {x} {y} & input tap {x} {y} & input tap {x} {y}"'
-            command = ['adb', 'shell', f'input tap {x} {y} & input tap {x} {y} & input tap {x} {y}']
-
-            subprocess.run(command, check=True)
-            return True
-        except Exception as e:
-            self.logger.error("__adb_multi_tap() ERROR:\n", e)
-            return False
-
-    def _adb_swipe(self,
-                   root,
-                   element: WebElement = None,
-                   x: int = None,
-                   y: int = None,
-                   direction: int = None,
-                   distance: int = None,
-                   duration: int = 1) -> bool:
-        """
-        Выполняет прокрутку с помощью adb.
-
-        Аргументы:
-            root: Корневой элемент на странице.
-            element (WebElement): Целевой элемент.
-            x (int): Координата X целевой позиции прокрутки.
-            y (int): Координата Y целевой позиции прокрутки.
-            direction (int): Направление прокрутки в градусах (от 0 до 360).
-            distance (int): Расстояние прокрутки в пикселях.
-            duration (int): Длительность прокрутки в секундах.
-
-        Возвращает:
-            bool: True, если прокрутка выполнена успешно; False в противном случае.
-        """
-        # Проверка наличия входных данных
-        if element is None and (x is None or y is None) and (direction is None or distance is None):
-            return False
-
-        # Получение координат центра начальной позиции прокрутки
-        x1, y1 = self._get_center()
-        x2, y2 = self._get_center()
-
-        # Расчет целевой позиции прокрутки на основе предоставленных входных данных
-        if element is not None:
-            # Если предоставлен локатор, получаем координаты центра целевого элемента
-            x2, y2 = self._get_center(element)
-        elif x is not None and y is not None:
-            # Если предоставлены координаты x и y, используем их в качестве целевой позиции прокрутки
-            x2, y2 = x, y
-        elif direction is not None and distance is not None:
-            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
-            window_size = adb.get_screen_resolution()
-            width = window_size[0]
-            height = window_size[1]
-            x2, y2 = find_coordinates_by_vector(width=width, height=height,
-                                                direction=direction, distance=distance,
-                                                start_x=x1, start_y=y1)
-
-        # Выполнение adb-команды прокрутки с заданными координатами и длительностью
-        command = ['adb', 'shell', 'input', 'swipe', str(x1), str(y1), str(x2), str(y2), str(duration * 1000)]
-        subprocess.run(command, check=True)
-
-        return True
+# coding: utf-8
+import logging
+import subprocess
+
+from appium.webdriver import WebElement
+
+import config
+
+from adb import adb
+from AppiumWebElementExtended.web_element_get import WebElementGet
+from AppiumHelpers.helpers_decorators import wait_for_window_change
+from utils.utils import find_coordinates_by_vector
+
+
+class WebElementAdbActions(WebElementGet):
+    """
+    Класс для выполнения adb-действий с элементами.
+    Наследуется от класса WebElementGet.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    def _adb_tap(self,
+                 decorator_args: dict = None,
+                 wait: bool = False) -> bool:
+        """
+        Выполняет нажатие на элемент с помощью adb.
+
+        Аргументы:
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
+                tries (int): Количество попыток нажатия (по умолчанию 3).
+            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
+
+        Возвращает:
+            bool: True, если нажатие выполнено успешно; False в противном случае.
+        """
+        if wait:
+            # Если нужно ожидать изменения окна.
+            if not decorator_args:
+                decorator_args = {"timeout_window": 5,
+                                  "tries": 5}
+            return self._adb_tap_to_element_and_wait(decorator_args=decorator_args)
+        else:
+            # Если не нужно ожидать изменения окна.
+            return self._adb_tap_to_element()
+
+    def _adb_tap_to_element(self) -> bool:
+        return self.__adb_tap()
+
+    @wait_for_window_change()
+    def _adb_tap_to_element_and_wait(self,
+                                     decorator_args: dict = None) -> bool:
+        return self.__adb_tap()
+
+    def __adb_tap(self) -> bool:
+        """
+        Выполняет нажатие на элемент с помощью adb.
+
+        Возвращает:
+            bool: True, если нажатие выполнено успешно, False в противном случае.
+        """
+        try:
+            x, y = self._get_center()
+            return adb.tap(x=x, y=y)
+        except Exception:
+            return False
+
+    def _adb_multi_tap(self,
+                       decorator_args: dict = None,
+                       wait: bool = False) -> bool:
+        """
+        Выполняет несколько нажатий с помощью adb.
+
+        Args:
+            decorator_args (dict, optional): Дополнительные аргументы для декоратора.
+                По умолчанию None.
+                Если None то будут преобразованы в decorator_args = {"timeout_window": 5, "tries": 5}), где
+                    timeout_window: время ожидания изменения окна в секундах.
+                    tries: количество попыток (выполнения настоящего метода) для изменения окна.
+            wait (bool, optional): Флаг, указывающий, нужно ли ожидать изменение окна после нажатия.
+                По умолчанию False.
+
+        Returns:
+            bool: True, если нажатие выполнено успешно, False в противном случае.
+        """
+        if wait:
+            if not decorator_args:
+                decorator_args = {"timeout_window": 5,
+                                  "tries": 5}
+            return self._adb_multi_tap_to_element_and_wait(decorator_args=decorator_args)
+        else:
+            return self._adb_multi_tap_to_element()
+
+    def _adb_multi_tap_to_element(self) -> bool:
+        """
+        Выполняет три быстрых нажатия с помощью adb.
+        """
+        return self.__adb_multi_tap()
+
+    @wait_for_window_change()
+    def _adb_multi_tap_to_element_and_wait(self,
+                                           decorator_args: dict = None) -> bool:
+        """
+        Выполняет три быстрых нажатия с помощью adb и ожидает изменения окна.
+        """
+        return self.__adb_multi_tap()
+
+    def __adb_multi_tap(self) -> bool:
+        """
+        Выполняет три быстрых нажатия с помощью adb.
+        Если подавать последовательно, через ";", то выполняются с задержкой в пару секунд.
+        Если подавать два тапа, то выполняются одновременно и сливаются.
+        С текущей конфигурацией команды - в 90% нажимает два раза. В 10% нажимает 3 раза.
+        Для выделения текста подходит.
+        """
+        try:
+            x, y = self._get_center()
+            # command = f'adb shell "input tap {x} {y} & input tap {x} {y} & input tap {x} {y}"'
+            command = ['adb', 'shell', f'input tap {x} {y} & input tap {x} {y} & input tap {x} {y}']
+
+            subprocess.run(command, check=True)
+            return True
+        except Exception as e:
+            self.logger.error("__adb_multi_tap() ERROR:\n", e)
+            return False
+
+    def _adb_swipe(self,
+                   root,
+                   element: WebElement = None,
+                   x: int = None,
+                   y: int = None,
+                   direction: int = None,
+                   distance: int = None,
+                   duration: int = 1) -> bool:
+        """
+        Выполняет прокрутку с помощью adb.
+
+        Аргументы:
+            root: Корневой элемент на странице.
+            element (WebElement): Целевой элемент.
+            x (int): Координата X целевой позиции прокрутки.
+            y (int): Координата Y целевой позиции прокрутки.
+            direction (int): Направление прокрутки в градусах (от 0 до 360).
+            distance (int): Расстояние прокрутки в пикселях.
+            duration (int): Длительность прокрутки в секундах.
+
+        Возвращает:
+            bool: True, если прокрутка выполнена успешно; False в противном случае.
+        """
+        # Проверка наличия входных данных
+        if element is None and (x is None or y is None) and (direction is None or distance is None):
+            return False
+
+        # Получение координат центра начальной позиции прокрутки
+        x1, y1 = self._get_center()
+        x2, y2 = self._get_center()
+
+        # Расчет целевой позиции прокрутки на основе предоставленных входных данных
+        if element is not None:
+            # Если предоставлен локатор, получаем координаты центра целевого элемента
+            x2, y2 = self._get_center(element)
+        elif x is not None and y is not None:
+            # Если предоставлены координаты x и y, используем их в качестве целевой позиции прокрутки
+            x2, y2 = x, y
+        elif direction is not None and distance is not None:
+            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
+            window_size = adb.get_screen_resolution()
+            width = window_size[0]
+            height = window_size[1]
+            x2, y2 = find_coordinates_by_vector(width=width, height=height,
+                                                direction=direction, distance=distance,
+                                                start_x=x1, start_y=y1)
+
+        # Выполнение adb-команды прокрутки с заданными координатами и длительностью
+        command = ['adb', 'shell', 'input', 'swipe', str(x1), str(y1), str(x2), str(y2), str(duration * 1000)]
+        subprocess.run(command, check=True)
+
+        return True
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_click.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-# coding: utf-8
-import logging
-from typing import Union, Tuple, Dict
-
-from appium.webdriver import WebElement
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.common import ElementNotInteractableException, StaleElementReferenceException, \
-    InvalidElementStateException
-
-import config
-
-from AppiumWebElementExtended.web_element_get import WebElementGet
-from adb import adb
-from AppiumHelpers.helpers_decorators import wait_for_window_change
-from utils.utils import find_coordinates_by_vector
-
-
-class WebElementClick(WebElementGet):
-    """
-    Класс для выполнения действий клика на элементе, двойного клика и клика с зажатием и перемещением курсора.
-    Наследуется от класса WebElementGet.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    def _click(self,
-               duration: int = 0,
-               decorator_args: dict = None,
-               wait: bool = False) -> bool:
-        """
-        Нажимает на элемент.
-
-        Аргументы:
-            duration (int): Время в секундах для продолжительности нажатия (по умолчанию 0).
-            decorator_args (dict): Параметры для декоратора.
-                timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
-                tries (int): Количество попыток нажатия (по умолчанию 3).
-            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
-
-        Использование:
-            decorator_args = {"timeout_window": 5,
-                              "tries": 5}
-            element._click(duration=0, wait=True, decorator_args=decorator_args)
-
-        Возвращает:
-            bool: True, если нажатие выполнено успешно; False в противном случае.
-        """
-        if wait:
-            # Если нужно ожидать изменения окна после нажатия
-            if not decorator_args:
-                # Декоратор по умолчанию
-                decorator_args = {"timeout_window": 5,
-                                  "tries": 5}
-            return self._click_to_element_and_wait(duration=duration, decorator_args=decorator_args)
-        else:
-            # Если не нужно ожидать результата после нажатия
-            return self._click_to_element(duration=duration)
-
-    def _click_to_element(self,
-                          duration: int = 0) -> bool:
-        return self.__click(duration=duration)
-
-    @wait_for_window_change()
-    def _click_to_element_and_wait(self,
-                                   duration: int = 0,
-                                   decorator_args: dict = None) -> bool:
-        return self.__click(duration=duration)
-
-    def __click(self,
-                duration: int = 0) -> bool:
-        """
-        Выполняет клик на элементе.
-
-        Аргументы:
-            duration (int): Длительность удержания клика в секундах.
-
-        Возвращает:
-            bool: True, если клик выполнен успешно; False в противном случае.
-        """
-        try:
-            action = ActionChains(self.driver)
-            element = self
-
-            if duration > 0:
-                # Если указана длительность клика, выполняется клик с удержанием на заданную длительность
-                action.click_and_hold(element).pause(duration / 1000).release()
-                action.perform()
-            else:
-                # Если не указана длительность клика, выполняется обычный клик
-                action.click(element).perform()
-
-        except (ElementNotInteractableException, StaleElementReferenceException, InvalidElementStateException) as e:
-            self.logger.error(f"Не удалось кликнуть по элементу")
-            self.logger.error("{}".format(e))
-            return False
-        return True
-
-    def _double_click(self,
-                      decorator_args: dict = None,
-                      wait: bool = False) -> bool:
-        """
-        Выполняет двойное нажатие (double click) на элементе.
-
-        Аргументы:
-            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
-                Например:
-                    decorator_args = {"timeout_window": 5,
-                                      "tries": 5}, где
-                    timeout_window (int): время ожидания изменения окна
-                    tries (int): количество попыток для изменения окна
-            wait (bool): Флаг, указывающий, нужно ли ожидать выполнения двойного нажатия.
-
-        Возвращает:
-        - True, если двойное нажатие выполнено успешно; False в противном случае.
-        """
-        decorator_args = {"timeout_window": 5,
-                          "tries": 5}
-        if wait:
-            return self._double_click_to_element_and_wait(decorator_args=decorator_args)
-        else:
-            return self._double_click_to_element()
-
-    def _double_click_to_element(self) -> bool:
-        return self.__double_click()
-
-    @wait_for_window_change()
-    def _double_click_to_element_and_wait(self, decorator_args: dict = None) -> bool:
-        return self.__double_click()
-
-    def __double_click(self):
-        """
-        Выполняет двойное нажатие (double click) на элементе.
-        Возвращает:
-        - True, если двойное нажатие выполнено успешно; False в противном случае.
-        """
-        try:
-            action = ActionChains(self.driver)
-            action.click(self).click(self).perform()
-            return True
-        except InvalidElementStateException:
-            return True
-        except (ElementNotInteractableException, StaleElementReferenceException) as e:
-            self.logger.error(f"Не удалось тапнуть по элементу")
-            self.logger.error("{}".format(e))
-            return False
-
-    def _click_and_move(self,
-                        root=None,
-                        locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                        x: int = None,
-                        y: int = None,
-                        direction: int = None,
-                        distance: int = None,
-                        ) -> bool:
-        """
-        Нажимает левую кнопку мыши, перемещает курсор к указанной цели и отпускает кнопку.
-
-        Целью может быть WebElement, абсолютные координаты (x, y) или направление и расстояние.
-        Если предоставлены направление и расстояние, функция вычисляет целевую позицию
-        на основе вектора, определенного этими значениями.
-        Если предоставлены абсолютные координаты (x, y), курсор перемещается в указанные позиции.
-        Если предоставлен локатор, функция перемещается к найденному элементу на веб-странице.
-
-        Параметры:
-        - root: Первый элемент на странице.
-        - locator: Локатор для поиска целевого элемента на веб-странице.
-        - x: Абсолютная координата по оси X для перемещения курсора.
-        - y: Абсолютная координата по оси Y для перемещения курсора.
-        - direction: Направление в градусах для перемещения курсора, где 0/360 - вверх, 90 - вправо, 180 - вниз, 270 - влево.
-        - distance: Расстояние в пикселях для перемещения курсора.
-
-        Возвращает:
-        - True, если действие было успешно выполнено, в противном случае False.
-
-        Примечание: Если не предоставлены аргументы, функция возвращает False и регистрирует ошибку.
-        """
-        element = self
-        action = ActionChains(self.driver)
-        action.click_and_hold(element)
-
-        # Получение координат центра начальной позиции прокрутки
-        x1, y1 = self._get_center()
-
-        if (x is None and y is None) and locator is None and (direction is None and distance is None):
-            # Если не предоставлены аргументы
-            self.logger.error(f"_click_and_move(): Нет аргументов")
-            return False
-        elif x is not None and y is not None:
-            # Если указаны абсолютные координаты (x, y) для перемещения курсора
-            action.move_by_offset(x-x1, y-y1)
-            action.release().perform()
-            return True
-        elif locator is not None and root is not None:
-            # Если указан локатор элемента и корневой элемент
-            target_element = root.get_element(locator)
-            action.move_to_element(target_element)
-            return True
-        elif direction is not None and distance is not None:
-            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
-            window_size = adb.get_screen_resolution()
-            width = window_size[0]
-            height = window_size[1]
-
-            x2, y2 = find_coordinates_by_vector(width=width, height=height,
-                                                direction=direction, distance=distance,
-                                                start_x=x1, start_y=y1)
-            action.move_by_offset(x2-x1, y2-y1)
-            action.release().perform()
-            return True
-
-        return False
-
+# coding: utf-8
+import logging
+from typing import Union, Tuple, Dict
+
+from appium.webdriver import WebElement
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.common import ElementNotInteractableException, StaleElementReferenceException, \
+    InvalidElementStateException
+
+import config
+
+from AppiumWebElementExtended.web_element_get import WebElementGet
+from adb import adb
+from AppiumHelpers.helpers_decorators import wait_for_window_change
+from utils.utils import find_coordinates_by_vector
+
+
+class WebElementClick(WebElementGet):
+    """
+    Класс для выполнения действий клика на элементе, двойного клика и клика с зажатием и перемещением курсора.
+    Наследуется от класса WebElementGet.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    def _click(self,
+               duration: int = 0,
+               decorator_args: dict = None,
+               wait: bool = False) -> bool:
+        """
+        Нажимает на элемент.
+
+        Аргументы:
+            duration (int): Время в секундах для продолжительности нажатия (по умолчанию 0).
+            decorator_args (dict): Параметры для декоратора.
+                timeout_window (int): Время ожидания нового окна (умножается на количество попыток).
+                tries (int): Количество попыток нажатия (по умолчанию 3).
+            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна.
+
+        Использование:
+            decorator_args = {"timeout_window": 5,
+                              "tries": 5}
+            element._click(duration=0, wait=True, decorator_args=decorator_args)
+
+        Возвращает:
+            bool: True, если нажатие выполнено успешно; False в противном случае.
+        """
+        if wait:
+            # Если нужно ожидать изменения окна после нажатия
+            if not decorator_args:
+                # Декоратор по умолчанию
+                decorator_args = {"timeout_window": 5,
+                                  "tries": 5}
+            return self._click_to_element_and_wait(duration=duration, decorator_args=decorator_args)
+        else:
+            # Если не нужно ожидать результата после нажатия
+            return self._click_to_element(duration=duration)
+
+    def _click_to_element(self,
+                          duration: int = 0) -> bool:
+        return self.__click(duration=duration)
+
+    @wait_for_window_change()
+    def _click_to_element_and_wait(self,
+                                   duration: int = 0,
+                                   decorator_args: dict = None) -> bool:
+        return self.__click(duration=duration)
+
+    def __click(self,
+                duration: int = 0) -> bool:
+        """
+        Выполняет клик на элементе.
+
+        Аргументы:
+            duration (int): Длительность удержания клика в секундах.
+
+        Возвращает:
+            bool: True, если клик выполнен успешно; False в противном случае.
+        """
+        try:
+            action = ActionChains(self.driver)
+            element = self
+
+            if duration > 0:
+                # Если указана длительность клика, выполняется клик с удержанием на заданную длительность
+                action.click_and_hold(element).pause(duration / 1000).release()
+                action.perform()
+            else:
+                # Если не указана длительность клика, выполняется обычный клик
+                action.click(element).perform()
+
+        except (ElementNotInteractableException, StaleElementReferenceException, InvalidElementStateException) as e:
+            self.logger.error(f"Не удалось кликнуть по элементу")
+            self.logger.error("{}".format(e))
+            return False
+        return True
+
+    def _double_click(self,
+                      decorator_args: dict = None,
+                      wait: bool = False) -> bool:
+        """
+        Выполняет двойное нажатие (double click) на элементе.
+
+        Аргументы:
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                Например:
+                    decorator_args = {"timeout_window": 5,
+                                      "tries": 5}, где
+                    timeout_window (int): время ожидания изменения окна
+                    tries (int): количество попыток для изменения окна
+            wait (bool): Флаг, указывающий, нужно ли ожидать выполнения двойного нажатия.
+
+        Возвращает:
+        - True, если двойное нажатие выполнено успешно; False в противном случае.
+        """
+        decorator_args = {"timeout_window": 5,
+                          "tries": 5}
+        if wait:
+            return self._double_click_to_element_and_wait(decorator_args=decorator_args)
+        else:
+            return self._double_click_to_element()
+
+    def _double_click_to_element(self) -> bool:
+        return self.__double_click()
+
+    @wait_for_window_change()
+    def _double_click_to_element_and_wait(self, decorator_args: dict = None) -> bool:
+        return self.__double_click()
+
+    def __double_click(self):
+        """
+        Выполняет двойное нажатие (double click) на элементе.
+        Возвращает:
+        - True, если двойное нажатие выполнено успешно; False в противном случае.
+        """
+        try:
+            action = ActionChains(self.driver)
+            action.click(self).click(self).perform()
+            return True
+        except InvalidElementStateException:
+            return True
+        except (ElementNotInteractableException, StaleElementReferenceException) as e:
+            self.logger.error(f"Не удалось тапнуть по элементу")
+            self.logger.error("{}".format(e))
+            return False
+
+    def _click_and_move(self,
+                        root=None,
+                        locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                        x: int = None,
+                        y: int = None,
+                        direction: int = None,
+                        distance: int = None,
+                        ) -> bool:
+        """
+        Нажимает левую кнопку мыши, перемещает курсор к указанной цели и отпускает кнопку.
+
+        Целью может быть WebElement, абсолютные координаты (x, y) или направление и расстояние.
+        Если предоставлены направление и расстояние, функция вычисляет целевую позицию
+        на основе вектора, определенного этими значениями.
+        Если предоставлены абсолютные координаты (x, y), курсор перемещается в указанные позиции.
+        Если предоставлен локатор, функция перемещается к найденному элементу на веб-странице.
+
+        Параметры:
+        - root: Первый элемент на странице.
+        - locator: Локатор для поиска целевого элемента на веб-странице.
+        - x: Абсолютная координата по оси X для перемещения курсора.
+        - y: Абсолютная координата по оси Y для перемещения курсора.
+        - direction: Направление в градусах для перемещения курсора, где 0/360 - вверх, 90 - вправо, 180 - вниз, 270 - влево.
+        - distance: Расстояние в пикселях для перемещения курсора.
+
+        Возвращает:
+        - True, если действие было успешно выполнено, в противном случае False.
+
+        Примечание: Если не предоставлены аргументы, функция возвращает False и регистрирует ошибку.
+        """
+        element = self
+        action = ActionChains(self.driver)
+        action.click_and_hold(element)
+
+        # Получение координат центра начальной позиции прокрутки
+        x1, y1 = self._get_center()
+
+        if (x is None and y is None) and locator is None and (direction is None and distance is None):
+            # Если не предоставлены аргументы
+            self.logger.error(f"_click_and_move(): Нет аргументов")
+            return False
+        elif x is not None and y is not None:
+            # Если указаны абсолютные координаты (x, y) для перемещения курсора
+            action.move_by_offset(x-x1, y-y1)
+            action.release().perform()
+            return True
+        elif locator is not None and root is not None:
+            # Если указан локатор элемента и корневой элемент
+            target_element = root.get_element(locator)
+            action.move_to_element(target_element)
+            return True
+        elif direction is not None and distance is not None:
+            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
+            window_size = adb.get_screen_resolution()
+            width = window_size[0]
+            height = window_size[1]
+
+            x2, y2 = find_coordinates_by_vector(width=width, height=height,
+                                                direction=direction, distance=distance,
+                                                start_x=x1, start_y=y1)
+            action.move_by_offset(x2-x1, y2-y1)
+            action.release().perform()
+            return True
+
+        return False
+
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_dom.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-# coding: utf-8
-import logging
-import time
-from typing import Union, List, Dict
-from appium.webdriver import WebElement
-from selenium.common.exceptions import NoSuchElementException
-
-import config
-
-from AppiumWebElementExtended.web_element_get import WebElementGet
-
-
-class WebElementDOM(WebElementGet):
-    """
-    Класс поиска элементов по DOM структуре относительно текущего элемента.
-    Наследуется от класса WebElementGet.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.helper = None
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-        self.stable_attributes = ['bounds', 'enabled', 'displayed', 'focused', 'focusable', 'class', 'resource-id',
-                                  'text']
-
-    def _get_parent(self) -> WebElement:
-        """
-        Возвращает родительский элемент
-        """
-        # Формирование XPath для поиска всех родительского элемента
-        xpath = self._get_xpath() + "/.."
-
-        # Поиск всех родительского элемента по XPath
-        parent = self.driver.find_element(by='xpath', value=xpath)
-
-        return parent
-
-    def _get_parents(self) -> List[WebElement]:
-        """
-        Возвращает всех родителей элемента.
-
-        Возвращает:
-            List[WebElement]: Список всех родительских элементов, начиная от ближайшего и до корневого элемента.
-        """
-        # Формирование XPath для поиска всех родительских элементов
-        xpath = self._get_xpath() + "/ancestor::*"
-
-        # Поиск всех родительских элементов по XPath
-        parents = self.driver.find_elements(by='xpath', value=xpath)
-
-        return parents
-
-
-    def _get_sibling(self, attributes: Dict[str, str], contains: bool = True) -> Union[WebElement, None]:
-        """
-        Возвращает брата элемента по указанным атрибутам.
-        То есть соседнего элемента в пределах первого предка.
-
-        Аргументы:
-            attributes (dict): Словарь с атрибутами и их значениями для поиска брата или сестры.
-            contains (bool): Флаг, указывающий, использовать ли функцию contains для атрибутов (по умолчанию: True).
-
-        Возвращает:
-            WebElement or None: Брат или сестра элемента, соответствующие указанным атрибутам, или None, если не найдено.
-
-        Примечание:
-            В случае, если используется contains=True и не найдено ни брата, ни сестры, возвращается None.
-
-        """
-        xpath_attributes = ""
-
-        # Формирование XPath атрибутов в зависимости от значения contains
-        if contains:
-            # Для поиска по фрагменту значения атрибута
-            for attr, value in attributes.items():
-                xpath_attributes += f"[contains(@{attr}, '{value}')]"
-        else:
-            # Для поиска по полному совпадению значения атрибута
-            for attr, value in attributes.items():
-                xpath_attributes += f"[(@{attr}='{value}')]"
-        try:
-            # Поиск брата перед текущим элементом с указанными атрибутами
-            xpath = self._get_xpath() + "/preceding-sibling::*" + xpath_attributes
-            sibling_before = self.driver.find_element(by='xpath', value=xpath)
-            return sibling_before
-        except NoSuchElementException:
-            try:
-                # Поиск брата после текущего элемента с указанными атрибутами
-                xpath = self._get_xpath() + "/following-sibling::*" + xpath_attributes
-                sibling_after = self.driver.find_element(by='xpath', value=xpath)
-                return sibling_after
-            except NoSuchElementException:
-                return None
-
-    def _get_siblings(self) -> Union[List[WebElement], List]:
-        """
-        Возвращает всех братьев элемента.
-        То есть соседних элементов в пределах первого предка.
-
-        Возвращает:
-            List[WebElement]: Список всех братьев и сестер элемента.
-        """
-        try:
-            # Получение XPath текущего элемента
-            xpath = self._get_xpath() + "/preceding-sibling::*"
-            # Поиск всех предшествующих братьев
-            siblings_before = self.driver.find_elements(by='xpath', value=xpath)
-            # Формирование XPath для последующих братьев
-            xpath = self._get_xpath() + "/following-sibling::*"
-            # Поиск всех последующих братьев
-            siblings_after = self.driver.find_elements(by='xpath', value=xpath)
-            # Объединение предшествующих и последующих братьев
-            siblings = siblings_before + siblings_after
-            return siblings
-        except NoSuchElementException as e:
-            self.logger.error("Ошибка при _get_siblings: {}".format(e))
-            return []
-
-    def _get_cousin(self,
-                    ancestor: WebElement,
-                    cousin: Dict[str, str],
-                    contains: bool = True) -> Union[WebElement, None]:
-        """
-        Поиск одного кузена элемента.
-        То есть элемента находящегося на аналогичной глубине относительно указанного предка.
-
-        Аргументы:
-            ancestor (WebElement): Элемент-предок.
-            cousin (Dict[str, str]): Атрибуты кузина для поиска.
-            contains (bool): Флаг, указывающий на использование функции contains при формировании XPath (по умолчанию: True).
-
-        Возвращает:
-            WebElement: Кузин элемента или None, если кузин не найден.
-        """
-        # Получение количество поколений между предком и текущим элементом
-        generation_len = self._generation_counter(ancestor=ancestor, descendant=self)
-
-        # Проверка наличия атрибута 'class' в словаре cousin и получение его значения из текущего элемента,
-        # если отсутствует
-        if 'class' not in cousin:
-            cousin['class'] = self.get_attribute('class')
-
-        # Формирование начального XPath с использованием класса кузина
-        xpath = "//" + cousin['class']
-
-        # Формирование XPath с использованием остальных атрибутов кузина
-        if contains:
-            # Для поиска по фрагменту значения атрибута
-            for attr, value in cousin.items():
-                xpath += f"[contains(@{attr}, '{value}')]"
-        else:
-            # Для поиска по полному совпадению значения атрибута
-            for attr, value in cousin.items():
-                xpath += f"[@{attr}='{value}']"
-
-        # Поиск потенциальных кузенов с помощью XPath
-        possible_cousins = ancestor.find_elements('xpath', xpath)
-
-        # Проверка поколения между предком и каждым потенциальным кузеном и возврат первого подходящего элемента
-        for element in possible_cousins:
-            if self._generation_counter(ancestor=ancestor, descendant=element) == generation_len:
-                return element
-
-        return None
-
-    def _get_cousins(self, ancestor: WebElement, cousin: Dict[str, str], contains: bool = True) -> \
-            Union[List[WebElement], List]:
-        """
-        Возвращает список кузенов элемента.
-        То есть элементов находящихся на аналогичной глубине относительно указанного предка.
-
-        Аргументы:
-            ancestor (WebElement): Элемент-предок.
-            cousin (dict): Атрибуты кузина для поиска.
-            contains (bool): Флаг, указывающий на использование функции contains при формировании XPath (по умолчанию: True).
-
-        Возвращает:
-            list: Список элементов-кузенов.
-        """
-        # Получение количество поколений между предком и текущим элементом
-        generation_len = self._generation_counter(ancestor=ancestor, descendant=self, )
-
-        # Проверка наличия атрибута 'class' в словаре cousin и получение его значения из текущего элемента,
-        # если отсутствует
-        if 'class' not in cousin:
-            cousin['class'] = self.get_attribute('class')
-
-        # Формирование начального XPath с использованием класса кузена
-        xpath = "//" + cousin['class']
-
-        # Формирование начального XPath с использованием класса кузина
-        if contains:
-            # Для поиска по фрагменту значения атрибута
-            for attr, value in cousin.items():
-                xpath += f"[contains(@{attr}, '{value}')]"
-        else:
-            # Для поиска по полному совпадению значения атрибута
-            for attr, value in cousin.items():
-                xpath += f"[@{attr}='{value}']"
-
-        # Поиск потенциальных кузенов с помощью XPath
-        possible_cousins = ancestor.find_elements('xpath', xpath)
-        result = []
-
-        # Проверка поколения между предком и каждым потенциальным кузеном и добавление их в список результатов
-        for element in possible_cousins:
-            if self._generation_counter(ancestor=ancestor, descendant=element) == generation_len:
-                result.append(element)
-
-        return result
-
-    def _generation_counter(self,
-                            ancestor: WebElement,
-                            descendant: WebElement,
-                            timeout: int = 90) -> int:
-        """
-        Подсчитывает количество поколений между элементами предком и потомком.
-
-        Аргументы:
-            ancestor (WebElement): элемент-предок.
-            descendant (WebElement): элемент-потомок.
-            timeout (int): время ожидания в секундах (по умолчанию: 90).
-        Возвращает:
-            int: количество поколений между элементами.
-        """
-        # Инициализация
-        start_time = time.time()
-        generation_count = 0
-        current_element = descendant
-
-        # Цикл выполняется, пока текущий элемент не станет None, не будет равен предку или не будет превышено время ожидания.
-        while current_element is not None and current_element != ancestor and time.time() - start_time < timeout:
-            attributes = {}
-            # Цикл проходит по всем стабильным атрибутам и получает их значения для текущего элемента.
-            for attribute in self.stable_attributes:
-                attributes[attribute] = current_element.get_attribute(attribute)
-
-            # Удаление атрибутов со значением None
-            attributes = {k: v for k, v in attributes.items() if v is not None}
-            # Создание начального xpath с использованием класса текущего элемента.
-            xpath = "//" + attributes['class']
-
-            # Цикл проходит по всем оставшимся атрибутам и добавляет их в xpath.
-            for attr, value in attributes.items():
-                xpath += f"[@{attr}='{value}']"
-
-            # Добавление "/.." в конец xpath для перехода к родительскому элементу.
-            xpath += "/.."
-            try:
-                # Поиск предка элемента по xpath
-                current_element = self.driver.find_element(by='xpath', value=xpath)
-                generation_count += 1
-            except NoSuchElementException:
-                # Если не удалось найти элемент-предка, возвращаем 0 и выводим сообщение об ошибке
-                self.logger.error("Элементы не связаны связью предок-потомок")
-                return 0
-
-        return generation_count
+# coding: utf-8
+import logging
+import time
+from typing import Union, List, Dict
+from appium.webdriver import WebElement
+from selenium.common.exceptions import NoSuchElementException
+
+import config
+
+from AppiumWebElementExtended.web_element_get import WebElementGet
+
+
+class WebElementDOM(WebElementGet):
+    """
+    Класс поиска элементов по DOM структуре относительно текущего элемента.
+    Наследуется от класса WebElementGet.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.helper = None
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+        self.stable_attributes = ['bounds', 'enabled', 'displayed', 'focused', 'focusable', 'class', 'resource-id',
+                                  'text']
+
+    def _get_parent(self) -> WebElement:
+        """
+        Возвращает родительский элемент
+        """
+        # Формирование XPath для поиска всех родительского элемента
+        xpath = self._get_xpath() + "/.."
+
+        # Поиск всех родительского элемента по XPath
+        parent = self.driver.find_element(by='xpath', value=xpath)
+
+        return parent
+
+    def _get_parents(self) -> List[WebElement]:
+        """
+        Возвращает всех родителей элемента.
+
+        Возвращает:
+            List[WebElement]: Список всех родительских элементов, начиная от ближайшего и до корневого элемента.
+        """
+        # Формирование XPath для поиска всех родительских элементов
+        xpath = self._get_xpath() + "/ancestor::*"
+
+        # Поиск всех родительских элементов по XPath
+        parents = self.driver.find_elements(by='xpath', value=xpath)
+
+        return parents
+
+
+    def _get_sibling(self, attributes: Dict[str, str], contains: bool = True) -> Union[WebElement, None]:
+        """
+        Возвращает брата элемента по указанным атрибутам.
+        То есть соседнего элемента в пределах первого предка.
+
+        Аргументы:
+            attributes (dict): Словарь с атрибутами и их значениями для поиска брата или сестры.
+            contains (bool): Флаг, указывающий, использовать ли функцию contains для атрибутов (по умолчанию: True).
+
+        Возвращает:
+            WebElement or None: Брат или сестра элемента, соответствующие указанным атрибутам, или None, если не найдено.
+
+        Примечание:
+            В случае, если используется contains=True и не найдено ни брата, ни сестры, возвращается None.
+
+        """
+        xpath_attributes = ""
+
+        # Формирование XPath атрибутов в зависимости от значения contains
+        if contains:
+            # Для поиска по фрагменту значения атрибута
+            for attr, value in attributes.items():
+                xpath_attributes += f"[contains(@{attr}, '{value}')]"
+        else:
+            # Для поиска по полному совпадению значения атрибута
+            for attr, value in attributes.items():
+                xpath_attributes += f"[(@{attr}='{value}')]"
+        try:
+            # Поиск брата перед текущим элементом с указанными атрибутами
+            xpath = self._get_xpath() + "/preceding-sibling::*" + xpath_attributes
+            sibling_before = self.driver.find_element(by='xpath', value=xpath)
+            return sibling_before
+        except NoSuchElementException:
+            try:
+                # Поиск брата после текущего элемента с указанными атрибутами
+                xpath = self._get_xpath() + "/following-sibling::*" + xpath_attributes
+                sibling_after = self.driver.find_element(by='xpath', value=xpath)
+                return sibling_after
+            except NoSuchElementException:
+                return None
+
+    def _get_siblings(self) -> Union[List[WebElement], List]:
+        """
+        Возвращает всех братьев элемента.
+        То есть соседних элементов в пределах первого предка.
+
+        Возвращает:
+            List[WebElement]: Список всех братьев и сестер элемента.
+        """
+        try:
+            # Получение XPath текущего элемента
+            xpath = self._get_xpath() + "/preceding-sibling::*"
+            # Поиск всех предшествующих братьев
+            siblings_before = self.driver.find_elements(by='xpath', value=xpath)
+            # Формирование XPath для последующих братьев
+            xpath = self._get_xpath() + "/following-sibling::*"
+            # Поиск всех последующих братьев
+            siblings_after = self.driver.find_elements(by='xpath', value=xpath)
+            # Объединение предшествующих и последующих братьев
+            siblings = siblings_before + siblings_after
+            return siblings
+        except NoSuchElementException as e:
+            self.logger.error("Ошибка при _get_siblings: {}".format(e))
+            return []
+
+    def _get_cousin(self,
+                    ancestor: WebElement,
+                    cousin: Dict[str, str],
+                    contains: bool = True) -> Union[WebElement, None]:
+        """
+        Поиск одного кузена элемента.
+        То есть элемента находящегося на аналогичной глубине относительно указанного предка.
+
+        Аргументы:
+            ancestor (WebElement): Элемент-предок.
+            cousin (Dict[str, str]): Атрибуты кузина для поиска.
+            contains (bool): Флаг, указывающий на использование функции contains при формировании XPath (по умолчанию: True).
+
+        Возвращает:
+            WebElement: Кузин элемента или None, если кузин не найден.
+        """
+        # Получение количество поколений между предком и текущим элементом
+        generation_len = self._generation_counter(ancestor=ancestor, descendant=self)
+
+        # Проверка наличия атрибута 'class' в словаре cousin и получение его значения из текущего элемента,
+        # если отсутствует
+        if 'class' not in cousin:
+            cousin['class'] = self.get_attribute('class')
+
+        # Формирование начального XPath с использованием класса кузина
+        xpath = "//" + cousin['class']
+
+        # Формирование XPath с использованием остальных атрибутов кузина
+        if contains:
+            # Для поиска по фрагменту значения атрибута
+            for attr, value in cousin.items():
+                xpath += f"[contains(@{attr}, '{value}')]"
+        else:
+            # Для поиска по полному совпадению значения атрибута
+            for attr, value in cousin.items():
+                xpath += f"[@{attr}='{value}']"
+
+        # Поиск потенциальных кузенов с помощью XPath
+        possible_cousins = ancestor.find_elements('xpath', xpath)
+
+        # Проверка поколения между предком и каждым потенциальным кузеном и возврат первого подходящего элемента
+        for element in possible_cousins:
+            if self._generation_counter(ancestor=ancestor, descendant=element) == generation_len:
+                return element
+
+        return None
+
+    def _get_cousins(self, ancestor: WebElement, cousin: Dict[str, str], contains: bool = True) -> \
+            Union[List[WebElement], List]:
+        """
+        Возвращает список кузенов элемента.
+        То есть элементов находящихся на аналогичной глубине относительно указанного предка.
+
+        Аргументы:
+            ancestor (WebElement): Элемент-предок.
+            cousin (dict): Атрибуты кузина для поиска.
+            contains (bool): Флаг, указывающий на использование функции contains при формировании XPath (по умолчанию: True).
+
+        Возвращает:
+            list: Список элементов-кузенов.
+        """
+        # Получение количество поколений между предком и текущим элементом
+        generation_len = self._generation_counter(ancestor=ancestor, descendant=self, )
+
+        # Проверка наличия атрибута 'class' в словаре cousin и получение его значения из текущего элемента,
+        # если отсутствует
+        if 'class' not in cousin:
+            cousin['class'] = self.get_attribute('class')
+
+        # Формирование начального XPath с использованием класса кузена
+        xpath = "//" + cousin['class']
+
+        # Формирование начального XPath с использованием класса кузина
+        if contains:
+            # Для поиска по фрагменту значения атрибута
+            for attr, value in cousin.items():
+                xpath += f"[contains(@{attr}, '{value}')]"
+        else:
+            # Для поиска по полному совпадению значения атрибута
+            for attr, value in cousin.items():
+                xpath += f"[@{attr}='{value}']"
+
+        # Поиск потенциальных кузенов с помощью XPath
+        possible_cousins = ancestor.find_elements('xpath', xpath)
+        result = []
+
+        # Проверка поколения между предком и каждым потенциальным кузеном и добавление их в список результатов
+        for element in possible_cousins:
+            if self._generation_counter(ancestor=ancestor, descendant=element) == generation_len:
+                result.append(element)
+
+        return result
+
+    def _generation_counter(self,
+                            ancestor: WebElement,
+                            descendant: WebElement,
+                            timeout: int = 90) -> int:
+        """
+        Подсчитывает количество поколений между элементами предком и потомком.
+
+        Аргументы:
+            ancestor (WebElement): элемент-предок.
+            descendant (WebElement): элемент-потомок.
+            timeout (int): время ожидания в секундах (по умолчанию: 90).
+        Возвращает:
+            int: количество поколений между элементами.
+        """
+        # Инициализация
+        start_time = time.time()
+        generation_count = 0
+        current_element = descendant
+
+        # Цикл выполняется, пока текущий элемент не станет None, не будет равен предку или не будет превышено время ожидания.
+        while current_element is not None and current_element != ancestor and time.time() - start_time < timeout:
+            attributes = {}
+            # Цикл проходит по всем стабильным атрибутам и получает их значения для текущего элемента.
+            for attribute in self.stable_attributes:
+                attributes[attribute] = current_element.get_attribute(attribute)
+
+            # Удаление атрибутов со значением None
+            attributes = {k: v for k, v in attributes.items() if v is not None}
+            # Создание начального xpath с использованием класса текущего элемента.
+            xpath = "//" + attributes['class']
+
+            # Цикл проходит по всем оставшимся атрибутам и добавляет их в xpath.
+            for attr, value in attributes.items():
+                xpath += f"[@{attr}='{value}']"
+
+            # Добавление "/.." в конец xpath для перехода к родительскому элементу.
+            xpath += "/.."
+            try:
+                # Поиск предка элемента по xpath
+                current_element = self.driver.find_element(by='xpath', value=xpath)
+                generation_count += 1
+            except NoSuchElementException:
+                # Если не удалось найти элемент-предка, возвращаем 0 и выводим сообщение об ошибке
+                self.logger.error("Элементы не связаны связью предок-потомок")
+                return 0
+
+        return generation_count
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_extended.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,416 +1,416 @@
-# coding: utf-8
-import logging
-from typing import Union, Tuple, Dict, List, cast
-
-from appium.webdriver import WebElement
-from appium.webdriver.common.appiumby import AppiumBy
-from appium.webdriver.common.mobileby import MobileBy
-from selenium.webdriver.common.by import By
-
-import config
-from AppiumWebElementExtended.web_element_click import WebElementClick
-from AppiumWebElementExtended.web_element_dom import WebElementDOM
-from AppiumWebElementExtended.web_element_scroll import WebElementScroll
-from AppiumWebElementExtended.web_element_tap import WebElementTap
-from AppiumWebElementsExtended.web_elements_extended import WebElementsExtended
-from AppiumWebElementExtended.web_element_adb_actions import WebElementAdbActions
-
-
-class WebElementExtended(WebElementClick,
-                         WebElementAdbActions,
-                         WebElementsExtended,
-                         WebElementDOM,
-                         WebElementTap,
-                         WebElementScroll):
-    """
-    Основной интерфейс для работы с WebElementExtended
-    """
-
-    def __init__(self, *args, **kwargs):
-
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    # GET
-    def get_element(self,
-                    locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                    by: Union[MobileBy, AppiumBy, By, str] = None,
-                    value: Union[str, Dict, None] = None,
-                    timeout_elem: int = 10,
-                    timeout_method: int = 600,
-                    elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                    contains: bool = True,
-                    ) -> Union['WebElementExtended', None]:
-        """
-        # TODO fill
-        """
-        inner_element = self._get_element(locator=locator,
-                                          by=by,
-                                          value=value,
-                                          timeout_elem=timeout_elem,
-                                          timeout_method=timeout_method,
-                                          elements_range=elements_range,
-                                          contains=contains)
-        return WebElementExtended(inner_element.parent, inner_element.id)
-
-    def get_attributes(self,
-                       desired_attributes: Union[str, List[str]] = None,
-                       ) -> Union[str, Dict[str, str], None]:
-        """
-        # TODO fill
-        """
-        attributes = self._get_attributes(desired_attributes=desired_attributes)
-        return attributes
-
-    # CLICK
-    def click(self,
-              duration: int = 0,
-              decorator_args: dict = None,
-              wait: bool = False,
-              ) -> 'WebElementExtended':
-        """
-        Нажимает на элемент.
-        Args:
-            duration: время в секундах продолжительности нажатия (по умолчанию 0)
-            wait: ожидать изменение окна или нет
-            decorator_args: параметры для декоратора.
-                timeout_window: int время ожидания нового окна (умножается на количество попыток)
-                tries: int количество попыток нажатия (по умолчанию 3)
-        Usage:
-            decorator_args = {"timeout_window": 5,
-                              "tries": 5}
-            element._tap(duration=0, wait=True, decorator_args=decorator_args)
-
-        Returns:
-            True если удалось нажать на элемент, иначе False
-        """
-        assert self._click(duration=duration,
-                           wait=wait,
-                           decorator_args=decorator_args)
-        return cast('WebElementExtended', self)
-
-    def double_click(self,
-                     decorator_args: dict = None,
-                     wait: bool = False,
-                     ) -> 'WebElementExtended':
-        """
-        fill me
-        # TODO fill
-        """
-        assert self._double_click(decorator_args=decorator_args,
-                                  wait=wait)
-        return cast('WebElementExtended', self)
-
-    def click_and_move(self, locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                       x: int = None,
-                       y: int = None,
-                       direction: int = None,
-                       distance: int = None,
-                       ) -> 'WebElementExtended':
-        """
-        fill me
-        # TODO fill
-        """
-        root = self.driver.find_element('xpath', '//*')
-        root = WebElementExtended(root.parent, root.id)
-        assert super()._click_and_move(root=root, locator=locator, x=x, y=y, direction=direction, distance=distance)
-        return cast('WebElementExtended', self)
-
-    # ADB TAP
-    def adb_tap(self,
-                decorator_args: dict = None,
-                wait: bool = False,
-                ) -> 'WebElementExtended':
-        """
-        tap by adb
-        # TODO fill
-        """
-        assert self._adb_tap(wait=wait,
-                             decorator_args=decorator_args)
-        return cast('WebElementExtended', self)
-
-    def adb_multi_tap(self) -> 'WebElementExtended':
-        """
-        double tap by adb
-        # TODO fill
-        """
-        assert self._adb_multi_tap()
-        return cast('WebElementExtended', self)
-
-    def adb_swipe(self,
-                  locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                  x: int = None,
-                  y: int = None,
-                  direction: int = None,
-                  distance: int = None,
-                  duration: int = 1,
-                  contains: bool = True,
-                  ) -> 'WebElementExtended':
-        """
-        swipe by adb
-        # TODO fill
-        """
-        root = self.driver.find_element('xpath', '//*')
-        root = WebElementExtended(root.parent, root.id)
-        element = None
-        if locator is not None:
-            element = root.get_element(locator=locator, contains=contains)
-        assert self._adb_swipe(root=root, element=element,
-                               x=x, y=y,
-                               direction=direction, distance=distance,
-                               duration=duration)
-        return cast('WebElementExtended', self)
-
-    # TAP
-    def tap(self,
-            duration: int = 0,
-            decorator_args: dict = None,
-            wait: bool = False,
-            ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        positions = self.get_center()
-        assert self._tap(positions=[positions],
-                         duration=duration,
-                         decorator_args=decorator_args,
-                         wait=wait)
-        return cast('WebElementExtended', self)
-
-    def double_tap(self,
-                   decorator_args: dict = None,
-                   wait: bool = False,
-                   pause: float = 0.2,
-                   ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        positions = self.get_center()
-        assert self._double_tap(positions=positions,
-                                decorator_args=decorator_args,
-                                wait=wait,
-                                pause=pause)
-        return cast('WebElementExtended', self)
-
-    def tap_and_move(self,
-                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                     x: int = None,
-                     y: int = None,
-                     direction: int = None,
-                     distance: int = None,
-                     ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        root = self.driver.find_element('xpath', '//*')
-        root = WebElementExtended(root.parent, root.id)
-        assert self._tap_and_move(root=root, locator=locator, x=x, y=y, direction=direction, distance=distance)
-        return cast('WebElementExtended', self)
-
-    # ELEMENTS
-    def get_elements(self,
-                     locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
-                     by: Union[MobileBy, AppiumBy, By, str] = None,
-                     value: Union[str, Dict, None] = None,
-                     timeout_elements: int = 10,
-                     timeout_method: int = 600,
-                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                     contains: bool = True,
-                     ) -> Union[List[WebElement], None]:
-        """
-        # TODO fill
-        """
-        elements = self._get_elements(locator=locator,
-                                      by=by,
-                                      value=value,
-                                      timeout_elements=timeout_elements,
-                                      timeout_method=timeout_method,
-                                      elements_range=elements_range,
-                                      contains=contains)
-        result = []
-        for element in elements:
-            result.append(WebElementExtended(element.parent, element.id))
-        return result
-
-    # SCROLL
-    def scroll_down(self,
-                    locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                    duration: int = None,
-                    ) -> 'WebElementExtended':
-        """
-        Скроллит элемент вниз от нижнего до верхнего элемента.
-        :param child_locator: str, имя класса дочернего элемента.
-        :param timeout: int, время ожидания элемента, по умолчанию 10 секунд.
-        :return: bool, True, если скроллинг выполнен успешно.
-        # TODO fill
-        """
-        assert self._scroll_down(locator=locator,
-                                 duration=duration)
-        return cast('WebElementExtended', self)
-
-    def scroll_up(self,
-                  locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                  duration: int = None,
-                  ) -> 'WebElementExtended':
-        """
-        Скроллит элемент вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента.
-        :param locator: Union[tuple, WebElement], локатор или элемент, который нужно проскроллить.
-        :param child_locator: str, имя класса дочернего элемента.
-        :param timeout: int, время ожидания элемента, по умолчанию 10 секунд.
-        :return: bool, True, если скроллинг выполнен успешно.
-        # TODO fill
-        """
-        assert self._scroll_up(locator=locator,
-                               duration=duration)
-
-        return cast('WebElementExtended', self)
-
-    def scroll_to_bottom(self,
-                         locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                         timeout_method: int = 120,
-                         ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        assert self._scroll_to_bottom(locator=locator,
-                                      timeout_method=timeout_method)
-        return cast('WebElementExtended', self)
-
-    def scroll_to_top(self,
-                      locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                      timeout_method: int = 120,
-                      ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        assert self._scroll_to_top(locator=locator,
-                                   timeout_method=timeout_method)
-        return cast('WebElementExtended', self)
-
-    def scroll_until_find(self,
-                          locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str],
-                          roll_locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                          timeout_method: int = 120,
-                          ) -> Union['WebElementExtended', None]:
-        """
-        # TODO fill
-        """
-        if not self._scroll_until_find(locator=locator,
-                                       timeout_method=timeout_method):
-            return None
-        return cast('WebElementExtended', self)
-
-    # DOM
-    def get_parent(self) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        element = self._get_parent()
-        return WebElementExtended(element.parent, element.id)
-
-    def get_parents(self) -> List['WebElementExtended']:
-        """
-        # TODO fill
-        """
-        elements = self._get_parents()
-        elements_ext = []
-        for element in elements:
-            elements_ext.append(WebElementExtended(element.parent, element.id))
-        return elements_ext
-
-    def get_sibling(self,
-                    attributes: Dict[str, str],
-                    contains: bool = True,
-                    ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        element = self._get_sibling(attributes=attributes, contains=contains)
-        return WebElementExtended(element.parent, element.id)
-
-    def get_siblings(self) -> List['WebElementExtended']:
-        """
-        # TODO fill
-        """
-        elements = self._get_siblings()
-        elements_ext = []
-        for element in elements:
-            elements_ext.append(WebElementExtended(element.parent, element.id))
-        return elements_ext
-
-    def get_cousin(self,
-                   ancestor: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-                   cousin: Dict[str, str],
-                   contains: bool = True,
-                   ) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        root = self.driver.find_element('xpath', '//*')
-        root = WebElementExtended(root.parent, root.id)
-        ancestor = root.get_element(ancestor)
-        ancestor = WebElement(ancestor.parent, ancestor.id)
-        element = self._get_cousin(ancestor=ancestor, cousin=cousin, contains=contains)
-        return WebElementExtended(element.parent, element.id)
-
-    def get_cousins(self,
-                    ancestor: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-                    cousin: Dict[str, str],
-                    contains: bool = True,
-                    ) -> List['WebElementExtended']:
-        """
-        # TODO fill
-        """
-        root = self.driver.find_element('xpath', '//*')
-        root = WebElementExtended(root.parent, root.id)
-        ancestor = root.get_element(ancestor)
-        ancestor = WebElement(ancestor.parent, ancestor.id)
-        elements = self._get_cousins(ancestor=ancestor, cousin=cousin, contains=contains)
-        elements_ext = []
-        for element in elements:
-            elements_ext.append(WebElementExtended(element.parent, element.id))
-        return elements_ext
-
-    def is_contains(self,
-                    locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
-                    contains: bool = True,
-                    ) -> bool:
-        """
-        # TODO fill
-        """
-        child_element = self.get_element(locator=locator, contains=contains)
-        if child_element is not None:
-            return True
-        return False
-
-    # ACTIONS
-    def zoom(self, hold: bool) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        raise NotImplementedError  # TODO implement
-
-    def unzoom(self, hold: bool) -> 'WebElementExtended':
-        """
-        # TODO fill
-        """
-        raise NotImplementedError  # TODO implement
-
-    def get_center(self) -> Union[Tuple[int, int], None]:
-        """
-        Вычисляет координаты центра заданного элемента.
-
-        Аргументы:
-            element (WebElement): Веб-элемент.
-
-        Возвращает:
-            tuple: Координаты центра в виде (x, y). Возвращает None, если произошла ошибка.
-        """
-        return self._get_center()
-
-    def get_coordinates(self) -> Union[Tuple[int, int, int, int], None]:
-        """
-        # TODO fill
-        """
-        return self._get_coordinates()
+# coding: utf-8
+import logging
+from typing import Union, Tuple, Dict, List, cast
+
+from appium.webdriver import WebElement
+from appium.webdriver.common.appiumby import AppiumBy
+from appium.webdriver.common.mobileby import MobileBy
+from selenium.webdriver.common.by import By
+
+import config
+from AppiumWebElementExtended.web_element_click import WebElementClick
+from AppiumWebElementExtended.web_element_dom import WebElementDOM
+from AppiumWebElementExtended.web_element_scroll import WebElementScroll
+from AppiumWebElementExtended.web_element_tap import WebElementTap
+from AppiumWebElementsExtended.web_elements_extended import WebElementsExtended
+from AppiumWebElementExtended.web_element_adb_actions import WebElementAdbActions
+
+
+class WebElementExtended(WebElementClick,
+                         WebElementAdbActions,
+                         WebElementsExtended,
+                         WebElementDOM,
+                         WebElementTap,
+                         WebElementScroll):
+    """
+    Основной интерфейс для работы с WebElementExtended
+    """
+
+    def __init__(self, *args, **kwargs):
+
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    # GET
+    def get_element(self,
+                    locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                    by: Union[MobileBy, AppiumBy, By, str] = None,
+                    value: Union[str, Dict, None] = None,
+                    timeout_elem: int = 10,
+                    timeout_method: int = 600,
+                    elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                    contains: bool = True,
+                    ) -> Union['WebElementExtended', None]:
+        """
+        # TODO fill
+        """
+        inner_element = self._get_element(locator=locator,
+                                          by=by,
+                                          value=value,
+                                          timeout_elem=timeout_elem,
+                                          timeout_method=timeout_method,
+                                          elements_range=elements_range,
+                                          contains=contains)
+        return WebElementExtended(inner_element.parent, inner_element.id)
+
+    def get_attributes(self,
+                       desired_attributes: Union[str, List[str]] = None,
+                       ) -> Union[str, Dict[str, str], None]:
+        """
+        # TODO fill
+        """
+        attributes = self._get_attributes(desired_attributes=desired_attributes)
+        return attributes
+
+    # CLICK
+    def click(self,
+              duration: int = 0,
+              decorator_args: dict = None,
+              wait: bool = False,
+              ) -> 'WebElementExtended':
+        """
+        Нажимает на элемент.
+        Args:
+            duration: время в секундах продолжительности нажатия (по умолчанию 0)
+            wait: ожидать изменение окна или нет
+            decorator_args: параметры для декоратора.
+                timeout_window: int время ожидания нового окна (умножается на количество попыток)
+                tries: int количество попыток нажатия (по умолчанию 3)
+        Usage:
+            decorator_args = {"timeout_window": 5,
+                              "tries": 5}
+            element._tap(duration=0, wait=True, decorator_args=decorator_args)
+
+        Returns:
+            True если удалось нажать на элемент, иначе False
+        """
+        assert self._click(duration=duration,
+                           wait=wait,
+                           decorator_args=decorator_args)
+        return cast('WebElementExtended', self)
+
+    def double_click(self,
+                     decorator_args: dict = None,
+                     wait: bool = False,
+                     ) -> 'WebElementExtended':
+        """
+        fill me
+        # TODO fill
+        """
+        assert self._double_click(decorator_args=decorator_args,
+                                  wait=wait)
+        return cast('WebElementExtended', self)
+
+    def click_and_move(self, locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                       x: int = None,
+                       y: int = None,
+                       direction: int = None,
+                       distance: int = None,
+                       ) -> 'WebElementExtended':
+        """
+        fill me
+        # TODO fill
+        """
+        root = self.driver.find_element('xpath', '//*')
+        root = WebElementExtended(root.parent, root.id)
+        assert super()._click_and_move(root=root, locator=locator, x=x, y=y, direction=direction, distance=distance)
+        return cast('WebElementExtended', self)
+
+    # ADB TAP
+    def adb_tap(self,
+                decorator_args: dict = None,
+                wait: bool = False,
+                ) -> 'WebElementExtended':
+        """
+        tap by adb
+        # TODO fill
+        """
+        assert self._adb_tap(wait=wait,
+                             decorator_args=decorator_args)
+        return cast('WebElementExtended', self)
+
+    def adb_multi_tap(self) -> 'WebElementExtended':
+        """
+        double tap by adb
+        # TODO fill
+        """
+        assert self._adb_multi_tap()
+        return cast('WebElementExtended', self)
+
+    def adb_swipe(self,
+                  locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                  x: int = None,
+                  y: int = None,
+                  direction: int = None,
+                  distance: int = None,
+                  duration: int = 1,
+                  contains: bool = True,
+                  ) -> 'WebElementExtended':
+        """
+        swipe by adb
+        # TODO fill
+        """
+        root = self.driver.find_element('xpath', '//*')
+        root = WebElementExtended(root.parent, root.id)
+        element = None
+        if locator is not None:
+            element = root.get_element(locator=locator, contains=contains)
+        assert self._adb_swipe(root=root, element=element,
+                               x=x, y=y,
+                               direction=direction, distance=distance,
+                               duration=duration)
+        return cast('WebElementExtended', self)
+
+    # TAP
+    def tap(self,
+            duration: int = 0,
+            decorator_args: dict = None,
+            wait: bool = False,
+            ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        positions = self.get_center()
+        assert self._tap(positions=[positions],
+                         duration=duration,
+                         decorator_args=decorator_args,
+                         wait=wait)
+        return cast('WebElementExtended', self)
+
+    def double_tap(self,
+                   decorator_args: dict = None,
+                   wait: bool = False,
+                   pause: float = 0.2,
+                   ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        positions = self.get_center()
+        assert self._double_tap(positions=positions,
+                                decorator_args=decorator_args,
+                                wait=wait,
+                                pause=pause)
+        return cast('WebElementExtended', self)
+
+    def tap_and_move(self,
+                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                     x: int = None,
+                     y: int = None,
+                     direction: int = None,
+                     distance: int = None,
+                     ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        root = self.driver.find_element('xpath', '//*')
+        root = WebElementExtended(root.parent, root.id)
+        assert self._tap_and_move(root=root, locator=locator, x=x, y=y, direction=direction, distance=distance)
+        return cast('WebElementExtended', self)
+
+    # ELEMENTS
+    def get_elements(self,
+                     locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
+                     by: Union[MobileBy, AppiumBy, By, str] = None,
+                     value: Union[str, Dict, None] = None,
+                     timeout_elements: int = 10,
+                     timeout_method: int = 600,
+                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                     contains: bool = True,
+                     ) -> Union[List[WebElement], None]:
+        """
+        # TODO fill
+        """
+        elements = self._get_elements(locator=locator,
+                                      by=by,
+                                      value=value,
+                                      timeout_elements=timeout_elements,
+                                      timeout_method=timeout_method,
+                                      elements_range=elements_range,
+                                      contains=contains)
+        result = []
+        for element in elements:
+            result.append(WebElementExtended(element.parent, element.id))
+        return result
+
+    # SCROLL
+    def scroll_down(self,
+                    locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                    duration: int = None,
+                    ) -> 'WebElementExtended':
+        """
+        Скроллит элемент вниз от нижнего до верхнего элемента.
+        :param child_locator: str, имя класса дочернего элемента.
+        :param timeout: int, время ожидания элемента, по умолчанию 10 секунд.
+        :return: bool, True, если скроллинг выполнен успешно.
+        # TODO fill
+        """
+        assert self._scroll_down(locator=locator,
+                                 duration=duration)
+        return cast('WebElementExtended', self)
+
+    def scroll_up(self,
+                  locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                  duration: int = None,
+                  ) -> 'WebElementExtended':
+        """
+        Скроллит элемент вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента.
+        :param locator: Union[tuple, WebElement], локатор или элемент, который нужно проскроллить.
+        :param child_locator: str, имя класса дочернего элемента.
+        :param timeout: int, время ожидания элемента, по умолчанию 10 секунд.
+        :return: bool, True, если скроллинг выполнен успешно.
+        # TODO fill
+        """
+        assert self._scroll_up(locator=locator,
+                               duration=duration)
+
+        return cast('WebElementExtended', self)
+
+    def scroll_to_bottom(self,
+                         locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                         timeout_method: int = 120,
+                         ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        assert self._scroll_to_bottom(locator=locator,
+                                      timeout_method=timeout_method)
+        return cast('WebElementExtended', self)
+
+    def scroll_to_top(self,
+                      locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                      timeout_method: int = 120,
+                      ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        assert self._scroll_to_top(locator=locator,
+                                   timeout_method=timeout_method)
+        return cast('WebElementExtended', self)
+
+    def scroll_until_find(self,
+                          locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str],
+                          roll_locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                          timeout_method: int = 120,
+                          ) -> Union['WebElementExtended', None]:
+        """
+        # TODO fill
+        """
+        if not self._scroll_until_find(locator=locator,
+                                       timeout_method=timeout_method):
+            return None
+        return cast('WebElementExtended', self)
+
+    # DOM
+    def get_parent(self) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        element = self._get_parent()
+        return WebElementExtended(element.parent, element.id)
+
+    def get_parents(self) -> List['WebElementExtended']:
+        """
+        # TODO fill
+        """
+        elements = self._get_parents()
+        elements_ext = []
+        for element in elements:
+            elements_ext.append(WebElementExtended(element.parent, element.id))
+        return elements_ext
+
+    def get_sibling(self,
+                    attributes: Dict[str, str],
+                    contains: bool = True,
+                    ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        element = self._get_sibling(attributes=attributes, contains=contains)
+        return WebElementExtended(element.parent, element.id)
+
+    def get_siblings(self) -> List['WebElementExtended']:
+        """
+        # TODO fill
+        """
+        elements = self._get_siblings()
+        elements_ext = []
+        for element in elements:
+            elements_ext.append(WebElementExtended(element.parent, element.id))
+        return elements_ext
+
+    def get_cousin(self,
+                   ancestor: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+                   cousin: Dict[str, str],
+                   contains: bool = True,
+                   ) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        root = self.driver.find_element('xpath', '//*')
+        root = WebElementExtended(root.parent, root.id)
+        ancestor = root.get_element(ancestor)
+        ancestor = WebElement(ancestor.parent, ancestor.id)
+        element = self._get_cousin(ancestor=ancestor, cousin=cousin, contains=contains)
+        return WebElementExtended(element.parent, element.id)
+
+    def get_cousins(self,
+                    ancestor: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+                    cousin: Dict[str, str],
+                    contains: bool = True,
+                    ) -> List['WebElementExtended']:
+        """
+        # TODO fill
+        """
+        root = self.driver.find_element('xpath', '//*')
+        root = WebElementExtended(root.parent, root.id)
+        ancestor = root.get_element(ancestor)
+        ancestor = WebElement(ancestor.parent, ancestor.id)
+        elements = self._get_cousins(ancestor=ancestor, cousin=cousin, contains=contains)
+        elements_ext = []
+        for element in elements:
+            elements_ext.append(WebElementExtended(element.parent, element.id))
+        return elements_ext
+
+    def is_contains(self,
+                    locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str],
+                    contains: bool = True,
+                    ) -> bool:
+        """
+        # TODO fill
+        """
+        child_element = self.get_element(locator=locator, contains=contains)
+        if child_element is not None:
+            return True
+        return False
+
+    # ACTIONS
+    def zoom(self, hold: bool) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        raise NotImplementedError  # TODO implement
+
+    def unzoom(self, hold: bool) -> 'WebElementExtended':
+        """
+        # TODO fill
+        """
+        raise NotImplementedError  # TODO implement
+
+    def get_center(self) -> Union[Tuple[int, int], None]:
+        """
+        Вычисляет координаты центра заданного элемента.
+
+        Аргументы:
+            element (WebElement): Веб-элемент.
+
+        Возвращает:
+            tuple: Координаты центра в виде (x, y). Возвращает None, если произошла ошибка.
+        """
+        return self._get_center()
+
+    def get_coordinates(self) -> Union[Tuple[int, int, int, int], None]:
+        """
+        # TODO fill
+        """
+        return self._get_coordinates()
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_get.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,431 +1,431 @@
-# coding: utf-8
-import logging
-import time
-from typing import Union, Dict, List, Tuple
-
-import xml.etree.ElementTree as ET
-
-from appium.webdriver import WebElement
-from selenium.common import WebDriverException
-
-from appium.webdriver.common.mobileby import MobileBy
-from appium.webdriver.common.appiumby import AppiumBy
-from selenium.webdriver.common.by import By
-
-import config
-from AppiumHelpers.appium_helpers import AppiumHelpers
-from AppiumHelpers.appium_image import AppiumImage
-
-
-class WebElementGet(WebElement):
-    """
-    Класс расширяющий Appium WebElement.
-    Обеспечивает получение сущностей из элемента.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.image = AppiumImage(driver=self.driver)
-        self.helper = None
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    def _get_element(self,
-                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                     by: Union[MobileBy, AppiumBy, By, str] = None,
-                     value: Union[str, Dict, None] = None,
-                     timeout_elem: int = 10,
-                     timeout_method: int = 600,
-                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                     contains: bool = True
-                     ) -> \
-            Union[WebElement, None]:
-        """
-        Извлекает элемент из элемента.
-        Должен принимать как минимум либо локатор, либо значения by и value.
-
-        Usage:
-            inner_element = element.get_element(locator=("id", "foo")).
-            inner_element = element.get_element(element).
-            inner_element = element.get_element(locator={'text': 'foo'}).
-            inner_element = element.get_element(locator='/path/to/file/pay_agent.png').
-            inner_element = element.get_element(locator=part_image,
-                                       elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'}).
-            inner_element = element.get_element(by="id", value="ru.sigma.app.debug:id/backButton").
-            inner_element = element.get_element(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
-            inner_element = element.get_element(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
-            inner_element = element.get_element(by=By.ID, value="ru.sigma.app.debug:id/backButton").
-
-        Args:
-            locator: tuple / WebElement / dict / str, определяет локатор элемента.
-                tuple - локатор в виде ('стратегия', 'значение'), например ('xpath', '//*'), ('id', 'elem_id') и т.д.
-                WebElement / WebElementExtended - объект веб элемента
-                dict - словарь, содержащий пары атрибут: значение (элемента), например {'text':'foo', 'enabled':'true'}
-                str - путь до файла с изображением элемента.
-            by: MobileBy, AppiumBy, By, str, тип локатора для поиска элемента (всегда в связке с value)
-            value: str, dict, None, значение локатора или словарь аргументов, если используется AppiumBy.XPATH.
-            timeout_elem: int, время ожидания элемента.
-            timeout_method: int, время ожидания метода поиска элемента.
-            elements_range: tuple, list, dict, None, ограничивает поиск элемента в указанном диапазоне
-            (для поиска по изображению). По умолчанию - все элементы внутри текущего элемента
-
-        Returns:
-            WebElement или None, если элемент не был найден.
-        """
-        # Проверка и подготовка аргументов
-        if (not locator) and (not by or not value):
-            self.logger.error(f"Некорректные аргументы!\n"
-                              f"{locator=}\n"
-                              f"{by=}\n"
-                              f"{value=}\n"
-                              f"{timeout_elem=}\n")
-            return None
-        if not locator and (by and value):
-            locator = (by, value)
-        if locator is None:
-            return None
-
-        # Поиск по изображению в пределах текущего элемента
-        if elements_range is None:
-            elements_range = self.find_elements("xpath", ".//*")
-
-        # Объявление стратегии поиска элементов
-        self.helper = AppiumHelpers(driver=self.driver)
-        locator_handler = {
-            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
-            dict: self.helper.handle_dict_locator,
-            # производит поиск элементов по фрагменту изображения, возвращает список элементов
-            str: self.helper.handle_string_locator,
-        }
-
-        # Цикл подготовки локатора и поиска элементов
-        start_time = time.time()
-        while time.time() - start_time < timeout_method:
-            # Выявление типа данных локатора для его подготовки
-            if isinstance(locator, WebElement):
-                return locator
-            locator_type = type(locator)
-            # Если локатор типа tuple, то выполняется извлечение элементов
-            if isinstance(locator, tuple):
-                try:
-                    element = self.find_element(*locator)
-                    return element
-                except WebDriverException:
-                    # self.logger.error(f"Элемент не обнаружен!\n"
-                    #                   f"{locator=}\n"
-                    #                   f"{timeout_elem=}\n\n" +
-                    #                   "{}\n".format(e))
-                    # self.logger.error(self.driver.page_source)
-                    return None
-            # Выполнение подготовки локатора
-            handler = locator_handler.get(locator_type)
-            if locator is None:
-                return None
-            locator = handler(locator=locator,
-                              timeout=int(timeout_elem),
-                              elements_range=elements_range,
-                              contains=contains)
-        # Подбирает результат после поиска по изображению
-        if isinstance(locator, WebElement):
-            return locator
-        self.logger.error(f"Что-то пошло не так\n"
-                          f"{locator=}\n"
-                          f"{by=}\n"
-                          f"{value=}\n"
-                          f"{timeout_elem=}\n"
-                          f"{timeout_method=}\n")
-        return None
-
-    def _get_elements(self,
-                      locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
-                      by: Union[MobileBy, AppiumBy, By, str] = None,
-                      value: Union[str, Dict, None] = None,
-                      timeout_elements: int = 10,
-                      timeout_method: int = 600,
-                      elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
-                      contains: bool = True) -> \
-            Union[List[WebElement], None]:
-        """
-        Метод обеспечивает поиск элементов в текущей DOM структуре.
-        Должен принять либо локатор, либо by и value.
-
-        Usage:
-            elements = app.get_elements(locator=("id", "foo")).
-            elements = app.get_elements(locator={'text': 'foo'}).
-            elements = app.get_elements(locator='/path/to/file/pay_agent.png').
-            elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
-            elements = app.get_elements(by=By.ID, value="ru.sigma.app.debug:id/backButton").
-
-        Args:
-            locator: tuple or WebElement or Dict[str, str], str, локатор tuple или Веб Элемент или словарь {'атрибут': 'значение'} или str как путь до файла с изображением элемента.
-            by:[MobileBy, AppiumBy, By, str], тип локатора для поиска элемента (всегда в связке с value)
-            value: Union[str, Dict, None], значение локатора или словарь аргументов, если используется AppiumBy.XPATH
-            timeout_elements:
-            timeout_method:
-            elements_range:
-
-        Returns:
-            Список WebElement'ов, или пустой список в случае их отсутствия.
-        """
-        # Проверка и подготовка аргументов
-        if not locator and (not by or not value):
-            self.logger.error(f"Некорректные аргументы!\n"
-                              f"{locator=}\n"
-                              f"{by=}\n"
-                              f"{value=}\n"
-                              f"{timeout_elements=}\n"
-                              f"{timeout_method=}\n"
-                              f"{contains=}")
-            return None
-        if not locator and (by and value):
-            locator = (by, value)
-        if locator is None:
-            return None
-
-        # Объявление стратегии поиска элементов
-        self.helper = AppiumHelpers(driver=self.driver)
-        locator_handler = {
-            # подразумевается список элементов, возвращает себя же
-            list: self.helper.handle_webelement_locator_elements,
-            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
-            dict: self.helper.handle_dict_locator_elements,
-            # производит поиск элементов по фрагменту изображения, возвращает список элементов
-            str: self.helper.handle_string_locator_elements,
-        }
-
-        # Цикл подготовки локатора и поиска элементов
-        start_time = time.time()
-        while not isinstance(locator, list) and time.time() - start_time < timeout_method:
-            # Если локатор типа tuple, то выполняется извлечение элементов
-            if isinstance(locator, tuple):
-                try:
-                    elements = self.find_elements(*locator)
-                    return elements
-                except WebDriverException:
-                    # self.logger.error(f"Элемент не обнаружен!\n"
-                    #                   f"{locator=}\n"
-                    #                   f"{by=}\n"
-                    #                   f"{value=}\n"
-                    #                   f"{timeout_elements=}\n"
-                    #                   f"{timeout_method=}\n"
-                    #                   f"{contains=}" +
-                    #                   "{}\n".format(e))
-                    return None
-            # Выявление типа данных локатора для его подготовки
-            locator_type = type(locator)
-            # Выполнение подготовки локатора
-            handler = locator_handler.get(locator_type)
-            locator = handler(locator=locator,
-                              timeout=int(timeout_elements),
-                              elements_range=elements_range,
-                              contains=contains)
-        # Подбирает результат после поиска по изображению
-        if isinstance(locator, list):
-            return locator
-        self.logger.error(f"Что-то пошло не так\n"
-                          f"{locator=}\n"
-                          f"{by=}\n"
-                          f"{value=}\n"
-                          f"{timeout_elements=}\n"
-                          f"{timeout_method=}\n"
-                          f"{contains=}")
-        return None
-
-    def _get_attributes(self,
-                        desired_attributes: List[str] = None) -> Dict[str, str]:
-        """
-        Получает атрибуты элемента.
-        Если хотя бы один запрашиваемый атрибут не найден, возвращает все атрибуты.
-
-        Usage:
-            element._get_attributes(['text', 'bounds', 'class'])
-            element._get_attributes()
-
-         Args:
-            desired_attributes: список имен атрибутов для получения.
-            Если не указан, будут возвращены все атрибуты элемента.
-
-        Returns:
-            Если указан desired_attributes и найдены в атрибутах элемента, возвращает словарь с требуемыми атрибутами
-            и их значениями.
-            Если desired_attributes не указан или атрибут не найден у элемента, возвращает словарь со всеми атрибутами.
-        """
-        # Инициализация пустого словаря для хранения атрибутов
-        result = {}
-
-        # Если desired_attributes не указан, установка значения 'all'
-        if not desired_attributes:
-            desired_attributes = 'all'
-
-        # Если desired_attributes не указан, установка значения 'all'
-        root = ET.fromstring(self.parent.page_source)
-
-        # Поиск требуемого элемента по критериям атрибутов
-        found_element = None
-        for element in root.iter():
-            if 'bounds' in element.attrib and 'class' in element.attrib:
-                if self.get_attribute('bounds') == element.attrib['bounds'] and self.get_attribute('class') == \
-                        element.attrib['class']:
-                    found_element = element
-                    break
-
-        # Если элемент найден, получение его атрибутов
-        if found_element is not None:
-            attributes = found_element.attrib
-            # Сохранение атрибутов в словаре result
-            for attribute_name, attribute_value in attributes.items():
-                result[attribute_name] = attribute_value
-
-        # Если desired_attributes указан, фильтрация словаря result
-        if desired_attributes:
-            new_result = {}
-            for attribute in desired_attributes:
-                if attribute not in result:
-                    # Возврат всех атрибутов если не найден искомый
-                    return result
-                new_result[attribute] = result[attribute]
-            # Возврат отфильтрованных атрибутов
-            return new_result
-        # Возврат всех атрибутов
-        return result
-
-    def _get_xpath(self) -> Union[str, None]:
-        """
-        Подбирает атрибуты элемента и на их основе составляет XPath элемента.
-
-        Returns:
-            str: XPath элемента.
-        """
-        try:
-            # Инициализация переменных
-            element = self
-            xpath = "//"
-            attrs = element._get_attributes()
-            element_type = attrs.get('class')
-            except_attrs = ['hint',
-                            'content-desc',
-                            'selection-start',
-                            'selection-end',
-                            'extras',
-                            ]
-
-            # Формирование начальной части XPath в зависимости от наличия типа (класса) элемента
-            if element_type:
-                xpath += element_type
-            else:
-                xpath += "*"
-
-            # Перебор атрибутов элемента для формирования остальной части XPath
-            for key, value in attrs.items():
-                if key in except_attrs:
-                    continue
-
-                # Добавление атрибута в XPath с соответствующим значением или без него, если значение равно None
-                if value is None:
-                    xpath += "[@{}]".format(key)
-                else:
-                    xpath += "[@{}='{}']".format(key, value)
-            return xpath
-        except (AttributeError, KeyError) as e:
-            self.logger.error("Ошибка при формировании XPath: {}".format(str(e)))
-        except Exception as e:
-            self.logger.error("Неизвестная ошибка при формировании XPath: {}".format(str(e)))
-        return None
-
-    def _get_center(self, element: WebElement = None) -> Union[Tuple[int, int], None]:
-        """
-        Получение координат центра элемента.
-
-        Returns:
-            tuple: Координаты x и y центра элемента.
-        """
-        try:
-            if element:
-                # Получение границ элемента
-                left, top, right, bottom = self._get_coordinates()
-            else:
-                # Получение границ элемента
-                left, top, right, bottom = self._get_coordinates()
-            # Расчет координат центра элемента
-            x = (left + right) / 2
-            y = (top + bottom) / 2
-
-            return x, y
-        except Exception as e:
-            self.logger.error("some exception with _get_center(): {}".format(e))
-            return None
-
-    def _get_coordinates(self) -> Union[Tuple[int, int, int, int], None]:
-        """
-        fill me
-        """
-        try:
-            left, top, right, bottom = map(int, self.get_attribute('bounds').strip("[]").replace("][", ",").split(","))
-            return left, top, right, bottom
-        except WebDriverException as e:
-            self.logger.error("Ошибка в методе _get_coordinates()")
-            self.logger.exception(e)
-
-    def _get_first_child_class(self) -> str:
-        """
-        Возвращает класс первого дочернего элемента, отличный от родительского
-        """
-        parent_element = self
-        parent_class = parent_element.get_attribute('class')
-        child_elements = parent_element.find_elements("xpath", "//*[1]")
-        for i, child_element in enumerate(child_elements):
-            child_class = child_element.get_attribute('class')
-            if parent_class != child_class:
-                return str(child_class)
-
-    def _get_top_child_from_parent(self,
-                                   locator: Union[Tuple[str, str], WebElement, Dict[str, str]] = None) -> \
-            Union[WebElement, None]:
-        """
-        Возвращает самый верхний дочерний элемент родительского элемента.
-        Если дочерний элемент только один, ищет внутри.
-
-        Args:
-            locator: Кортеж / объект WebElement / словарь, представляющий локатор для дочернего элемента.
-
-        Returns:
-            Самый верхний дочерний элемент родительского элемента, указанному в локаторе дочерних элементов,
-            или None, если соответствующий дочерний элемент не найден.
-        """
-        if locator is None:
-            locator = {'class': self._get_first_child_class()}
-        children = self._get_elements(locator=locator)
-        if len(children) <= 1:
-            while not len(children) > 1:
-                if len(children) == 0:
-                    return None
-                children = children[0].find_elements(by='xpath', value=f'//*')
-        top_child = sorted(children, key=lambda x: x.location['y'])[0]
-        return top_child
-
-    def _get_bottom_child_from_parent(self,
-                                      locator: Union[Tuple[str, str], WebElement, Dict[str, str]] = None) -> \
-            Union[WebElement, None]:
-        """
-        Метод возвращает нижний дочерний элемент родительского элемента с заданным классом.
-        Если дочерний элемент только один, ищет внутри.
-
-        Args:
-            locator: Union[Tuple[str, str], WebElement, Dict[str, str]], локатор дочернего элемента.
-        Returns:
-            Найденный элемент или None, в случае его отсутствия.
-        """
-        if locator is None:
-            locator = {'class': self._get_first_child_class()}
-        children = self._get_elements(locator=locator)
-        if len(children) == 0:
-            return None
-        if len(children) <= 1:
-            while not len(children) > 1:
-                if len(children) == 0:
-                    return None
-                children = children[0].find_elements(by='xpath', value=f'//*')
-        bottom_child = sorted(children, key=lambda x: x.location['y'] + x.size['height'])[-1]
-        return bottom_child
+# coding: utf-8
+import logging
+import time
+from typing import Union, Dict, List, Tuple
+
+import xml.etree.ElementTree as ET
+
+from appium.webdriver import WebElement
+from selenium.common import WebDriverException
+
+from appium.webdriver.common.mobileby import MobileBy
+from appium.webdriver.common.appiumby import AppiumBy
+from selenium.webdriver.common.by import By
+
+import config
+from AppiumHelpers.appium_helpers import AppiumHelpers
+from AppiumHelpers.appium_image import AppiumImage
+
+
+class WebElementGet(WebElement):
+    """
+    Класс расширяющий Appium WebElement.
+    Обеспечивает получение сущностей из элемента.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.image = AppiumImage(driver=self.driver)
+        self.helper = None
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    def _get_element(self,
+                     locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                     by: Union[MobileBy, AppiumBy, By, str] = None,
+                     value: Union[str, Dict, None] = None,
+                     timeout_elem: int = 10,
+                     timeout_method: int = 600,
+                     elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                     contains: bool = True
+                     ) -> \
+            Union[WebElement, None]:
+        """
+        Извлекает элемент из элемента.
+        Должен принимать как минимум либо локатор, либо значения by и value.
+
+        Usage:
+            inner_element = element.get_element(locator=("id", "foo")).
+            inner_element = element.get_element(element).
+            inner_element = element.get_element(locator={'text': 'foo'}).
+            inner_element = element.get_element(locator='/path/to/file/pay_agent.png').
+            inner_element = element.get_element(locator=part_image,
+                                       elements_range={'class':'android.widget.FrameLayout', 'package':'ru.app.debug'}).
+            inner_element = element.get_element(by="id", value="ru.sigma.app.debug:id/backButton").
+            inner_element = element.get_element(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
+            inner_element = element.get_element(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
+            inner_element = element.get_element(by=By.ID, value="ru.sigma.app.debug:id/backButton").
+
+        Args:
+            locator: tuple / WebElement / dict / str, определяет локатор элемента.
+                tuple - локатор в виде ('стратегия', 'значение'), например ('xpath', '//*'), ('id', 'elem_id') и т.д.
+                WebElement / WebElementExtended - объект веб элемента
+                dict - словарь, содержащий пары атрибут: значение (элемента), например {'text':'foo', 'enabled':'true'}
+                str - путь до файла с изображением элемента.
+            by: MobileBy, AppiumBy, By, str, тип локатора для поиска элемента (всегда в связке с value)
+            value: str, dict, None, значение локатора или словарь аргументов, если используется AppiumBy.XPATH.
+            timeout_elem: int, время ожидания элемента.
+            timeout_method: int, время ожидания метода поиска элемента.
+            elements_range: tuple, list, dict, None, ограничивает поиск элемента в указанном диапазоне
+            (для поиска по изображению). По умолчанию - все элементы внутри текущего элемента
+
+        Returns:
+            WebElement или None, если элемент не был найден.
+        """
+        # Проверка и подготовка аргументов
+        if (not locator) and (not by or not value):
+            self.logger.error(f"Некорректные аргументы!\n"
+                              f"{locator=}\n"
+                              f"{by=}\n"
+                              f"{value=}\n"
+                              f"{timeout_elem=}\n")
+            return None
+        if not locator and (by and value):
+            locator = (by, value)
+        if locator is None:
+            return None
+
+        # Поиск по изображению в пределах текущего элемента
+        if elements_range is None:
+            elements_range = self.find_elements("xpath", ".//*")
+
+        # Объявление стратегии поиска элементов
+        self.helper = AppiumHelpers(driver=self.driver)
+        locator_handler = {
+            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
+            dict: self.helper.handle_dict_locator,
+            # производит поиск элементов по фрагменту изображения, возвращает список элементов
+            str: self.helper.handle_string_locator,
+        }
+
+        # Цикл подготовки локатора и поиска элементов
+        start_time = time.time()
+        while time.time() - start_time < timeout_method:
+            # Выявление типа данных локатора для его подготовки
+            if isinstance(locator, WebElement):
+                return locator
+            locator_type = type(locator)
+            # Если локатор типа tuple, то выполняется извлечение элементов
+            if isinstance(locator, tuple):
+                try:
+                    element = self.find_element(*locator)
+                    return element
+                except WebDriverException:
+                    # self.logger.error(f"Элемент не обнаружен!\n"
+                    #                   f"{locator=}\n"
+                    #                   f"{timeout_elem=}\n\n" +
+                    #                   "{}\n".format(e))
+                    # self.logger.error(self.driver.page_source)
+                    return None
+            # Выполнение подготовки локатора
+            handler = locator_handler.get(locator_type)
+            if locator is None:
+                return None
+            locator = handler(locator=locator,
+                              timeout=int(timeout_elem),
+                              elements_range=elements_range,
+                              contains=contains)
+        # Подбирает результат после поиска по изображению
+        if isinstance(locator, WebElement):
+            return locator
+        self.logger.error(f"Что-то пошло не так\n"
+                          f"{locator=}\n"
+                          f"{by=}\n"
+                          f"{value=}\n"
+                          f"{timeout_elem=}\n"
+                          f"{timeout_method=}\n")
+        return None
+
+    def _get_elements(self,
+                      locator: Union[Tuple, List[WebElement], Dict[str, str], str] = None,
+                      by: Union[MobileBy, AppiumBy, By, str] = None,
+                      value: Union[str, Dict, None] = None,
+                      timeout_elements: int = 10,
+                      timeout_method: int = 600,
+                      elements_range: Union[Tuple, List[WebElement], Dict[str, str], None] = None,
+                      contains: bool = True) -> \
+            Union[List[WebElement], None]:
+        """
+        Метод обеспечивает поиск элементов в текущей DOM структуре.
+        Должен принять либо локатор, либо by и value.
+
+        Usage:
+            elements = app.get_elements(locator=("id", "foo")).
+            elements = app.get_elements(locator={'text': 'foo'}).
+            elements = app.get_elements(locator='/path/to/file/pay_agent.png').
+            elements = app.get_elements(by="id", value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=MobileBy.ID, value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=AppiumBy.ID, value="ru.sigma.app.debug:id/backButton").
+            elements = app.get_elements(by=By.ID, value="ru.sigma.app.debug:id/backButton").
+
+        Args:
+            locator: tuple or WebElement or Dict[str, str], str, локатор tuple или Веб Элемент или словарь {'атрибут': 'значение'} или str как путь до файла с изображением элемента.
+            by:[MobileBy, AppiumBy, By, str], тип локатора для поиска элемента (всегда в связке с value)
+            value: Union[str, Dict, None], значение локатора или словарь аргументов, если используется AppiumBy.XPATH
+            timeout_elements:
+            timeout_method:
+            elements_range:
+
+        Returns:
+            Список WebElement'ов, или пустой список в случае их отсутствия.
+        """
+        # Проверка и подготовка аргументов
+        if not locator and (not by or not value):
+            self.logger.error(f"Некорректные аргументы!\n"
+                              f"{locator=}\n"
+                              f"{by=}\n"
+                              f"{value=}\n"
+                              f"{timeout_elements=}\n"
+                              f"{timeout_method=}\n"
+                              f"{contains=}")
+            return None
+        if not locator and (by and value):
+            locator = (by, value)
+        if locator is None:
+            return None
+
+        # Объявление стратегии поиска элементов
+        self.helper = AppiumHelpers(driver=self.driver)
+        locator_handler = {
+            # подразумевается список элементов, возвращает себя же
+            list: self.helper.handle_webelement_locator_elements,
+            # составляет локатор типа tuple из словаря с атрибутами искомого элемента
+            dict: self.helper.handle_dict_locator_elements,
+            # производит поиск элементов по фрагменту изображения, возвращает список элементов
+            str: self.helper.handle_string_locator_elements,
+        }
+
+        # Цикл подготовки локатора и поиска элементов
+        start_time = time.time()
+        while not isinstance(locator, list) and time.time() - start_time < timeout_method:
+            # Если локатор типа tuple, то выполняется извлечение элементов
+            if isinstance(locator, tuple):
+                try:
+                    elements = self.find_elements(*locator)
+                    return elements
+                except WebDriverException:
+                    # self.logger.error(f"Элемент не обнаружен!\n"
+                    #                   f"{locator=}\n"
+                    #                   f"{by=}\n"
+                    #                   f"{value=}\n"
+                    #                   f"{timeout_elements=}\n"
+                    #                   f"{timeout_method=}\n"
+                    #                   f"{contains=}" +
+                    #                   "{}\n".format(e))
+                    return None
+            # Выявление типа данных локатора для его подготовки
+            locator_type = type(locator)
+            # Выполнение подготовки локатора
+            handler = locator_handler.get(locator_type)
+            locator = handler(locator=locator,
+                              timeout=int(timeout_elements),
+                              elements_range=elements_range,
+                              contains=contains)
+        # Подбирает результат после поиска по изображению
+        if isinstance(locator, list):
+            return locator
+        self.logger.error(f"Что-то пошло не так\n"
+                          f"{locator=}\n"
+                          f"{by=}\n"
+                          f"{value=}\n"
+                          f"{timeout_elements=}\n"
+                          f"{timeout_method=}\n"
+                          f"{contains=}")
+        return None
+
+    def _get_attributes(self,
+                        desired_attributes: List[str] = None) -> Dict[str, str]:
+        """
+        Получает атрибуты элемента.
+        Если хотя бы один запрашиваемый атрибут не найден, возвращает все атрибуты.
+
+        Usage:
+            element._get_attributes(['text', 'bounds', 'class'])
+            element._get_attributes()
+
+         Args:
+            desired_attributes: список имен атрибутов для получения.
+            Если не указан, будут возвращены все атрибуты элемента.
+
+        Returns:
+            Если указан desired_attributes и найдены в атрибутах элемента, возвращает словарь с требуемыми атрибутами
+            и их значениями.
+            Если desired_attributes не указан или атрибут не найден у элемента, возвращает словарь со всеми атрибутами.
+        """
+        # Инициализация пустого словаря для хранения атрибутов
+        result = {}
+
+        # Если desired_attributes не указан, установка значения 'all'
+        if not desired_attributes:
+            desired_attributes = 'all'
+
+        # Если desired_attributes не указан, установка значения 'all'
+        root = ET.fromstring(self.parent.page_source)
+
+        # Поиск требуемого элемента по критериям атрибутов
+        found_element = None
+        for element in root.iter():
+            if 'bounds' in element.attrib and 'class' in element.attrib:
+                if self.get_attribute('bounds') == element.attrib['bounds'] and self.get_attribute('class') == \
+                        element.attrib['class']:
+                    found_element = element
+                    break
+
+        # Если элемент найден, получение его атрибутов
+        if found_element is not None:
+            attributes = found_element.attrib
+            # Сохранение атрибутов в словаре result
+            for attribute_name, attribute_value in attributes.items():
+                result[attribute_name] = attribute_value
+
+        # Если desired_attributes указан, фильтрация словаря result
+        if desired_attributes:
+            new_result = {}
+            for attribute in desired_attributes:
+                if attribute not in result:
+                    # Возврат всех атрибутов если не найден искомый
+                    return result
+                new_result[attribute] = result[attribute]
+            # Возврат отфильтрованных атрибутов
+            return new_result
+        # Возврат всех атрибутов
+        return result
+
+    def _get_xpath(self) -> Union[str, None]:
+        """
+        Подбирает атрибуты элемента и на их основе составляет XPath элемента.
+
+        Returns:
+            str: XPath элемента.
+        """
+        try:
+            # Инициализация переменных
+            element = self
+            xpath = "//"
+            attrs = element._get_attributes()
+            element_type = attrs.get('class')
+            except_attrs = ['hint',
+                            'content-desc',
+                            'selection-start',
+                            'selection-end',
+                            'extras',
+                            ]
+
+            # Формирование начальной части XPath в зависимости от наличия типа (класса) элемента
+            if element_type:
+                xpath += element_type
+            else:
+                xpath += "*"
+
+            # Перебор атрибутов элемента для формирования остальной части XPath
+            for key, value in attrs.items():
+                if key in except_attrs:
+                    continue
+
+                # Добавление атрибута в XPath с соответствующим значением или без него, если значение равно None
+                if value is None:
+                    xpath += "[@{}]".format(key)
+                else:
+                    xpath += "[@{}='{}']".format(key, value)
+            return xpath
+        except (AttributeError, KeyError) as e:
+            self.logger.error("Ошибка при формировании XPath: {}".format(str(e)))
+        except Exception as e:
+            self.logger.error("Неизвестная ошибка при формировании XPath: {}".format(str(e)))
+        return None
+
+    def _get_center(self, element: WebElement = None) -> Union[Tuple[int, int], None]:
+        """
+        Получение координат центра элемента.
+
+        Returns:
+            tuple: Координаты x и y центра элемента.
+        """
+        try:
+            if element:
+                # Получение границ элемента
+                left, top, right, bottom = self._get_coordinates()
+            else:
+                # Получение границ элемента
+                left, top, right, bottom = self._get_coordinates()
+            # Расчет координат центра элемента
+            x = (left + right) / 2
+            y = (top + bottom) / 2
+
+            return x, y
+        except Exception as e:
+            self.logger.error("some exception with _get_center(): {}".format(e))
+            return None
+
+    def _get_coordinates(self) -> Union[Tuple[int, int, int, int], None]:
+        """
+        fill me
+        """
+        try:
+            left, top, right, bottom = map(int, self.get_attribute('bounds').strip("[]").replace("][", ",").split(","))
+            return left, top, right, bottom
+        except WebDriverException as e:
+            self.logger.error("Ошибка в методе _get_coordinates()")
+            self.logger.exception(e)
+
+    def _get_first_child_class(self) -> str:
+        """
+        Возвращает класс первого дочернего элемента, отличный от родительского
+        """
+        parent_element = self
+        parent_class = parent_element.get_attribute('class')
+        child_elements = parent_element.find_elements("xpath", "//*[1]")
+        for i, child_element in enumerate(child_elements):
+            child_class = child_element.get_attribute('class')
+            if parent_class != child_class:
+                return str(child_class)
+
+    def _get_top_child_from_parent(self,
+                                   locator: Union[Tuple[str, str], WebElement, Dict[str, str]] = None) -> \
+            Union[WebElement, None]:
+        """
+        Возвращает самый верхний дочерний элемент родительского элемента.
+        Если дочерний элемент только один, ищет внутри.
+
+        Args:
+            locator: Кортеж / объект WebElement / словарь, представляющий локатор для дочернего элемента.
+
+        Returns:
+            Самый верхний дочерний элемент родительского элемента, указанному в локаторе дочерних элементов,
+            или None, если соответствующий дочерний элемент не найден.
+        """
+        if locator is None:
+            locator = {'class': self._get_first_child_class()}
+        children = self._get_elements(locator=locator)
+        if len(children) <= 1:
+            while not len(children) > 1:
+                if len(children) == 0:
+                    return None
+                children = children[0].find_elements(by='xpath', value=f'//*')
+        top_child = sorted(children, key=lambda x: x.location['y'])[0]
+        return top_child
+
+    def _get_bottom_child_from_parent(self,
+                                      locator: Union[Tuple[str, str], WebElement, Dict[str, str]] = None) -> \
+            Union[WebElement, None]:
+        """
+        Метод возвращает нижний дочерний элемент родительского элемента с заданным классом.
+        Если дочерний элемент только один, ищет внутри.
+
+        Args:
+            locator: Union[Tuple[str, str], WebElement, Dict[str, str]], локатор дочернего элемента.
+        Returns:
+            Найденный элемент или None, в случае его отсутствия.
+        """
+        if locator is None:
+            locator = {'class': self._get_first_child_class()}
+        children = self._get_elements(locator=locator)
+        if len(children) == 0:
+            return None
+        if len(children) <= 1:
+            while not len(children) > 1:
+                if len(children) == 0:
+                    return None
+                children = children[0].find_elements(by='xpath', value=f'//*')
+        bottom_child = sorted(children, key=lambda x: x.location['y'] + x.size['height'])[-1]
+        return bottom_child
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_scroll.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# coding: utf-8
-import logging
-import time
-from typing import Union, Tuple, Dict
-
-from appium.webdriver import WebElement
-from selenium.common import StaleElementReferenceException, NoSuchElementException, TimeoutException
-
-import config
-
-from AppiumWebElementExtended.web_element_get import WebElementGet
-
-
-class WebElementScroll(WebElementGet):
-    """
-    Класс для выполнения действий прокрутки элемента.
-    Наследуется от класса WebElementGet.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    def _scroll_down(self,
-                     locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                     duration: int = None) -> bool:
-        """
-        Прокручивает элемент вниз от нижнего дочернего элемента до верхнего дочернего элемента родительского элемента.
-
-        Args:
-            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
-            duration (int, optional): Продолжительность прокрутки в миллисекундах (по умолчанию: None).
-
-        Returns:
-            bool: True, если прокрутка выполнена успешно.
-
-        """
-        try:
-            recycler = self
-
-            # Проверка, является ли элемент прокручиваемым
-            if recycler.get_attribute('scrollable') != 'true':
-                self.logger.error("Элемент не крутиться")
-                return False
-
-            # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
-            if not locator:
-                locator = {'class': self._get_first_child_class()}
-
-            # Получение верхнего и нижнего дочерних элементов родительского элемента
-            top_child = self._get_top_child_from_parent(locator=locator)
-            bottom_child = self._get_bottom_child_from_parent(locator=locator)
-
-            # Прокрутка вниз от нижнего дочернего элемента до верхнего дочернего элемента родительского элемента
-            self.driver.scroll(origin_el=bottom_child, destination_el=top_child, duration=duration)
-            return True
-
-        except (NoSuchElementException, StaleElementReferenceException, TimeoutException) as e:
-            self.logger.error("_scroll_down(): Ошибка. {}".format(e))
-            return False
-
-    def _scroll_up(self,
-                   locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
-                   duration: int = None) -> bool:
-        """
-        Прокручивает элемент вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента.
-
-        Args:
-            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
-            duration (int, optional): Продолжительность прокрутки в миллисекундах (по умолчанию: None).
-
-        Returns:
-            bool: True, если прокрутка выполнена успешно.
-
-        """
-        try:
-            recycler = self
-
-            # Проверка, является ли элемент прокручиваемым
-            if recycler.get_attribute('scrollable') != 'true':
-                self.logger.error("Элемент не крутиться")
-                return False
-
-            # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
-            if not locator:
-                locator = {'class': self._get_first_child_class()}
-
-            # Получение верхнего и нижнего дочерних элементов родительского элемента
-            top_child = self._get_top_child_from_parent(locator=locator)
-            bottom_child = self._get_bottom_child_from_parent(locator=locator)
-
-            # Прокрутка вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента
-            self.driver.scroll(origin_el=top_child, destination_el=bottom_child, duration=duration)
-            return True
-
-        except (NoSuchElementException, StaleElementReferenceException, TimeoutException) as e:
-            self.logger.error("_scroll_up(): Ошибка. {}".format(e))
-            return False
-
-    def _scroll_to_bottom(self,
-                          locator: Union[Tuple, WebElement, Dict[str, str], str] = None,
-                          timeout_method: int = 120) -> bool:
-        """
-        Прокручивает элемент вниз до упора.
-
-        Args:
-            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
-            timeout_method (int, optional): Время ожидания элемента в секундах (по умолчанию: 120).
-
-        Returns:
-            bool: True, если прокрутка выполнена успешно.
-
-        """
-        recycler = self
-
-        # Проверка, является ли элемент прокручиваемым
-        if recycler.get_attribute('scrollable') != 'true':
-            self.logger.error("Элемент не крутиться")
-            return False
-
-        # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
-        if not locator:
-            locator = {'class': self._get_first_child_class()}
-
-        last_child = None
-        start_time = time.time()
-
-        # Прокрутка вниз до упора
-        while time.time() - start_time < timeout_method:
-            child = self._get_element(locator=locator)
-            if child == last_child:
-                return True
-            last_child = child
-            self._scroll_down(locator=locator)
-        self.logger.error("_scroll_to_bottom(): Неизвестная ошибка")
-        return False
-
-    def _scroll_to_top(self,
-                       locator: Union[Tuple, WebElement, Dict[str, str], str],
-                       timeout_method: int = 120) -> bool:
-        """
-        Прокручивает элемент вверх до упора.
-
-        Args:
-            locator (Union[Tuple, WebElement, Dict[str, str], str]): Локатор или элемент для прокрутки (за что крутить).
-            timeout_method (int): Время ожидания элемента в секундах (по умолчанию: 120).
-
-        Returns:
-            bool: True, если прокрутка выполнена успешно.
-
-        """
-        recycler = self
-
-        # Проверка, является ли элемент прокручиваемым
-        if recycler.get_attribute('scrollable') != 'true':
-            self.logger.error("Элемент не крутиться")
-            return False
-
-        # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
-        if not locator:
-            locator = {'class': self._get_first_child_class()}
-        last_child = None
-        start_time = time.time()
-
-        # Прокрутка вверх до упора
-        while time.time() - start_time < timeout_method:
-            child = self._get_element(locator=locator)
-            if child == last_child:
-                return True
-            last_child = child
-            self._scroll_up(locator=locator)
-
-        self.logger.error("_scroll_to_top(): Неизвестная ошибка")
-        return False
-
-    def _scroll_until_find(self,
-                           locator: Union[Tuple, WebElement, Dict[str, str], str],
-                           timeout_method: int = 120) -> bool:
-        """
-        Крутит элемент вниз, а затем вверх для поиска элемента по заданному локатору.
-
-        Args:
-            locator (Union[Tuple, WebElement, Dict[str, str], str]): Локатор или элемент, для которого производится
-                поиск.
-            timeout_method (int): Время на поиск в одном направлении (по умолчанию: 120 вниз и 120 вверх).
-
-        Returns:
-            bool: True, если элемент найден. False, если элемент не найден.
-
-        """
-        recycler = self
-
-        # Проверка, является ли элемент scrollable
-        if recycler.get_attribute('scrollable') != 'true':
-            self.logger.error("Элемент не крутиться")
-            return False
-
-        start_time = time.time()
-
-        last_element_image = None
-
-        # Прокрутка вниз до поиска элемента
-        while time.time() - start_time < timeout_method:
-            try:
-                if isinstance(locator, str):
-                    if self.image.is_image_on_the_screen(image=locator):
-                        return True
-                element = self._get_element(locator=locator, timeout_elem=1)
-                if element is not None:
-                    return True
-            except NoSuchElementException:
-                continue
-            current_element_image = self.screenshot_as_base64
-            if current_element_image == last_element_image:
-                break
-            last_element_image = self.screenshot_as_base64
-            recycler._scroll_down()
-
-        # Прокрутка вверх до поиска элемента
-        while time.time() - start_time < timeout_method:
-            try:
-                if isinstance(locator, str):
-                    if self.image.is_image_on_the_screen(image=locator):
-                        return True
-                element = self._get_element(locator=locator, timeout_elem=1)
-                if element is not None:
-                    return True
-            except NoSuchElementException:
-                pass
-            current_element_image = self.screenshot_as_base64
-            if current_element_image == last_element_image:
-                break
-            last_element_image = self.screenshot_as_base64
-            recycler._scroll_up()
-
-        self.logger.error("_scroll_until_find(): Элемент не найден")
-        return False
+# coding: utf-8
+import logging
+import time
+from typing import Union, Tuple, Dict
+
+from appium.webdriver import WebElement
+from selenium.common import StaleElementReferenceException, NoSuchElementException, TimeoutException
+
+import config
+
+from AppiumWebElementExtended.web_element_get import WebElementGet
+
+
+class WebElementScroll(WebElementGet):
+    """
+    Класс для выполнения действий прокрутки элемента.
+    Наследуется от класса WebElementGet.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    def _scroll_down(self,
+                     locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                     duration: int = None) -> bool:
+        """
+        Прокручивает элемент вниз от нижнего дочернего элемента до верхнего дочернего элемента родительского элемента.
+
+        Args:
+            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
+            duration (int, optional): Продолжительность прокрутки в миллисекундах (по умолчанию: None).
+
+        Returns:
+            bool: True, если прокрутка выполнена успешно.
+
+        """
+        try:
+            recycler = self
+
+            # Проверка, является ли элемент прокручиваемым
+            if recycler.get_attribute('scrollable') != 'true':
+                self.logger.error("Элемент не крутиться")
+                return False
+
+            # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
+            if not locator:
+                locator = {'class': self._get_first_child_class()}
+
+            # Получение верхнего и нижнего дочерних элементов родительского элемента
+            top_child = self._get_top_child_from_parent(locator=locator)
+            bottom_child = self._get_bottom_child_from_parent(locator=locator)
+
+            # Прокрутка вниз от нижнего дочернего элемента до верхнего дочернего элемента родительского элемента
+            self.driver.scroll(origin_el=bottom_child, destination_el=top_child, duration=duration)
+            return True
+
+        except (NoSuchElementException, StaleElementReferenceException, TimeoutException) as e:
+            self.logger.error("_scroll_down(): Ошибка. {}".format(e))
+            return False
+
+    def _scroll_up(self,
+                   locator: Union[Tuple, 'WebElementExtended', Dict[str, str], str] = None,
+                   duration: int = None) -> bool:
+        """
+        Прокручивает элемент вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента.
+
+        Args:
+            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
+            duration (int, optional): Продолжительность прокрутки в миллисекундах (по умолчанию: None).
+
+        Returns:
+            bool: True, если прокрутка выполнена успешно.
+
+        """
+        try:
+            recycler = self
+
+            # Проверка, является ли элемент прокручиваемым
+            if recycler.get_attribute('scrollable') != 'true':
+                self.logger.error("Элемент не крутиться")
+                return False
+
+            # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
+            if not locator:
+                locator = {'class': self._get_first_child_class()}
+
+            # Получение верхнего и нижнего дочерних элементов родительского элемента
+            top_child = self._get_top_child_from_parent(locator=locator)
+            bottom_child = self._get_bottom_child_from_parent(locator=locator)
+
+            # Прокрутка вверх от верхнего дочернего элемента до нижнего дочернего элемента родительского элемента
+            self.driver.scroll(origin_el=top_child, destination_el=bottom_child, duration=duration)
+            return True
+
+        except (NoSuchElementException, StaleElementReferenceException, TimeoutException) as e:
+            self.logger.error("_scroll_up(): Ошибка. {}".format(e))
+            return False
+
+    def _scroll_to_bottom(self,
+                          locator: Union[Tuple, WebElement, Dict[str, str], str] = None,
+                          timeout_method: int = 120) -> bool:
+        """
+        Прокручивает элемент вниз до упора.
+
+        Args:
+            locator (Union[Tuple, WebElement, Dict[str, str], str], optional): Локатор или элемент для прокрутки (за что крутить).
+            timeout_method (int, optional): Время ожидания элемента в секундах (по умолчанию: 120).
+
+        Returns:
+            bool: True, если прокрутка выполнена успешно.
+
+        """
+        recycler = self
+
+        # Проверка, является ли элемент прокручиваемым
+        if recycler.get_attribute('scrollable') != 'true':
+            self.logger.error("Элемент не крутиться")
+            return False
+
+        # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
+        if not locator:
+            locator = {'class': self._get_first_child_class()}
+
+        last_child = None
+        start_time = time.time()
+
+        # Прокрутка вниз до упора
+        while time.time() - start_time < timeout_method:
+            child = self._get_element(locator=locator)
+            if child == last_child:
+                return True
+            last_child = child
+            self._scroll_down(locator=locator)
+        self.logger.error("_scroll_to_bottom(): Неизвестная ошибка")
+        return False
+
+    def _scroll_to_top(self,
+                       locator: Union[Tuple, WebElement, Dict[str, str], str],
+                       timeout_method: int = 120) -> bool:
+        """
+        Прокручивает элемент вверх до упора.
+
+        Args:
+            locator (Union[Tuple, WebElement, Dict[str, str], str]): Локатор или элемент для прокрутки (за что крутить).
+            timeout_method (int): Время ожидания элемента в секундах (по умолчанию: 120).
+
+        Returns:
+            bool: True, если прокрутка выполнена успешно.
+
+        """
+        recycler = self
+
+        # Проверка, является ли элемент прокручиваемым
+        if recycler.get_attribute('scrollable') != 'true':
+            self.logger.error("Элемент не крутиться")
+            return False
+
+        # Если локатор для прокрутки не указан, используется локатор первого дочернего элемента
+        if not locator:
+            locator = {'class': self._get_first_child_class()}
+        last_child = None
+        start_time = time.time()
+
+        # Прокрутка вверх до упора
+        while time.time() - start_time < timeout_method:
+            child = self._get_element(locator=locator)
+            if child == last_child:
+                return True
+            last_child = child
+            self._scroll_up(locator=locator)
+
+        self.logger.error("_scroll_to_top(): Неизвестная ошибка")
+        return False
+
+    def _scroll_until_find(self,
+                           locator: Union[Tuple, WebElement, Dict[str, str], str],
+                           timeout_method: int = 120) -> bool:
+        """
+        Крутит элемент вниз, а затем вверх для поиска элемента по заданному локатору.
+
+        Args:
+            locator (Union[Tuple, WebElement, Dict[str, str], str]): Локатор или элемент, для которого производится
+                поиск.
+            timeout_method (int): Время на поиск в одном направлении (по умолчанию: 120 вниз и 120 вверх).
+
+        Returns:
+            bool: True, если элемент найден. False, если элемент не найден.
+
+        """
+        recycler = self
+
+        # Проверка, является ли элемент scrollable
+        if recycler.get_attribute('scrollable') != 'true':
+            self.logger.error("Элемент не крутиться")
+            return False
+
+        start_time = time.time()
+
+        last_element_image = None
+
+        # Прокрутка вниз до поиска элемента
+        while time.time() - start_time < timeout_method:
+            try:
+                if isinstance(locator, str):
+                    if self.image.is_image_on_the_screen(image=locator):
+                        return True
+                element = self._get_element(locator=locator, timeout_elem=1)
+                if element is not None:
+                    return True
+            except NoSuchElementException:
+                continue
+            current_element_image = self.screenshot_as_base64
+            if current_element_image == last_element_image:
+                break
+            last_element_image = self.screenshot_as_base64
+            recycler._scroll_down()
+
+        # Прокрутка вверх до поиска элемента
+        while time.time() - start_time < timeout_method:
+            try:
+                if isinstance(locator, str):
+                    if self.image.is_image_on_the_screen(image=locator):
+                        return True
+                element = self._get_element(locator=locator, timeout_elem=1)
+                if element is not None:
+                    return True
+            except NoSuchElementException:
+                pass
+            current_element_image = self.screenshot_as_base64
+            if current_element_image == last_element_image:
+                break
+            last_element_image = self.screenshot_as_base64
+            recycler._scroll_up()
+
+        self.logger.error("_scroll_until_find(): Элемент не найден")
+        return False
```

### Comparing `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_tap.py` & `AppiumExtended-0.1.6/AppiumWebElementExtended/web_element_tap.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# coding: utf-8
-import logging
-from typing import Union, Tuple, Dict, List, Optional
-
-from appium.webdriver import WebElement
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.webdriver.common.actions import interaction
-from selenium.webdriver.common.actions.action_builder import ActionBuilder
-from selenium.webdriver.common.actions.pointer_input import PointerInput
-
-import config
-
-from AppiumWebElementExtended.web_element_get import WebElementGet
-from adb import adb
-from AppiumHelpers.helpers_decorators import wait_for_window_change
-from utils.utils import find_coordinates_by_vector
-
-
-class WebElementTap(WebElementGet):
-    """
-    Класс для выполнения действий нажатия (Tap), а также нажатия и перемещения с использованием элементов веб-страницы.
-    Наследуется от класса WebElementGet.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.driver = args[0]
-        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-    def _tap(self,
-             positions: List[Tuple[int, int]],
-             duration: int = 0,
-             decorator_args: dict = None,
-             wait: bool = False) -> bool:
-        """
-        Выполняет нажатие на указанные координаты.
-
-        Аргументы:
-            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
-            duration (int): Длительность нажатия в миллисекундах.
-            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
-                    Например:
-                        decorator_args = {"timeout_window": 5,
-                                          "tries": 5}, где
-                        timeout_window (int): время ожидания изменения окна
-                        tries (int): количество попыток для изменения окна
-            wait (bool): Флаг, указывающий, нужно ли ожидать результата после нажатия.
-
-        Возвращает:
-            bool: True, если нажатие выполнено успешно; False в противном случае.
-        """
-
-        if wait:
-            # Если нужно ожидать результата после нажатия
-
-            if not decorator_args:
-                # Декоратор по умолчанию
-                decorator_args = {"timeout_window": 5,
-                                  "tries": 5}
-
-            return self._tap_to_element_and_wait(positions=positions, duration=duration, decorator_args=decorator_args)
-        else:
-            # Если не нужно ожидать результата после нажатия
-            return self._tap_to_element(positions=positions, duration=duration)
-
-    @wait_for_window_change()
-    def _tap_to_element_and_wait(self,
-                                 positions: List[Tuple[int, int]],
-                                 duration: int = 0,
-                                 decorator_args: dict = None, ):
-        return self.__tap(positions=positions, duration=duration)
-
-    def _tap_to_element(self,
-                        positions: List[Tuple[int, int]],
-                        duration: int = 0, ):
-        return self.__tap(positions=positions, duration=duration)
-
-    def __tap(self, positions: List[Tuple[int, int]], duration: Optional[int] = None):
-        """
-        Выполняет нажатие по указанным координатам.
-
-        Аргументы:
-            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
-            duration (Optional[int]): Длительность нажатия в миллисекундах.
-
-        Возвращает:
-            bool: True, если нажатие выполнено успешно; False в противном случае.
-        """
-
-        try:
-            self.driver.tap(positions=positions, duration=duration)
-            return True
-        except Exception as e:
-            self.logger.error("some exception with __tap(): {}".format(e))
-            return False
-
-    def _double_tap(self,
-                    positions: Tuple[int, int],
-                    decorator_args: dict = None,
-                    wait: bool = False,
-                    pause: float = 0.2) -> bool:
-        """
-        Выполняет двойное нажатие (double tap) на указанных координатах.
-
-        Аргументы:
-            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
-            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
-                Например:
-                    decorator_args = {"timeout_window": 5,
-                                      "tries": 5}, где
-                    timeout_window (int): время ожидания изменения окна
-                    tries (int): количество попыток для изменения окна
-            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна после двойного нажатия.
-            pause (float): Пауза между двумя нажатиями в секундах.
-
-        Возвращает:
-            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
-        """
-
-        # Декоратор по умолчанию
-        decorator_args = {"timeout_window": 5,
-                          "tries": 5}
-
-        if wait:
-            # Если нужно ожидать результата после двойного нажатия
-            return self._double_tap_to_element_and_wait(positions=positions, decorator_args=decorator_args, pause=pause)
-        else:
-            # Если не нужно ожидать результата после двойного нажатия
-            return self._double_tap_to_element(positions=positions, pause=pause)
-
-    @wait_for_window_change()
-    def _double_tap_to_element_and_wait(self, positions: Tuple[int, int], decorator_args: dict = None,
-                                        pause: float = 0.2) -> bool:
-        return self.__double_tap(positions=positions, pause=pause)
-
-    def _double_tap_to_element(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
-        return self.__double_tap(positions=positions, pause=pause)
-
-    def __double_tap(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
-        """
-        Выполняет двойное нажатие (double tap) по указанным координатам.
-
-        Аргументы:
-            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
-            pause (float): Пауза между двумя нажатиями в секундах.
-
-        Возвращает:
-            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
-        """
-        actions = ActionChains(self.driver)
-        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
-        x = positions[0]
-        y = positions[1]
-
-        # Первое нажатие
-        actions.w3c_actions.pointer_action.move_to_location(x, y)
-        actions.w3c_actions.pointer_action.pointer_down()
-        actions.w3c_actions.pointer_action.pause(0.1)
-        actions.w3c_actions.pointer_action.pointer_up()
-        actions.w3c_actions.pointer_action.pause(pause)
-
-        # Второе нажатие
-        actions.w3c_actions.pointer_action.pointer_down()
-        actions.w3c_actions.pointer_action.pause(0.1)
-        actions.w3c_actions.pointer_action.release()
-
-        try:
-            actions.perform()
-            return True
-        except Exception as e:
-            self.logger.error("some exception with __double_tap(): {}".format(e))
-            return False
-
-    def _tap_and_move(self,
-                      root=None,
-                      locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
-                      x: int = None,
-                      y: int = None,
-                      direction: int = None,
-                      distance: int = None,
-                      ) -> bool:
-        """
-        Выполняет операцию "нажать и переместить" на веб-элементе или на указанных координатах.
-
-        Аргументы:
-            root (WebElementExtended): Корневой элемент, относительно которого будет выполнено нажатие и перемещение.
-            locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]): Локатор элемента,
-                на который будет выполнено нажатие и перемещение.
-            x (int): Координата X для нажатия и перемещения.
-            y (int): Координата Y для нажатия и перемещения.
-            direction (int): Направление прокрутки в градусах (0 - вверх, 90 - вправо, 180 - вниз, 270 - влево).
-            distance (int): Расстояние прокрутки в пикселях.
-
-        Возвращает:
-            bool: True, если операция успешно выполнена; False в противном случае.
-        """
-        # Получение координат центра начальной позиции прокрутки
-        x1, y1 = self._get_center()
-
-        actions = ActionChains(self.driver)
-        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
-        actions.w3c_actions.pointer_action.move_to_location(x1, y1)
-        actions.w3c_actions.pointer_action.pointer_down()
-
-        # Проверка аргументов для определения типа операции
-        if (x is None and y is None) and locator is None and (direction is None and distance is None):
-            # Если не предоставлены аргументы
-            self.logger.error(f"_tap_and_move(): Нет аргументов")
-            return False
-        elif x is not None and y is not None:
-            # Если указаны координаты для нажатия и перемещения
-            actions.w3c_actions.pointer_action.move_to_location(x, y)
-            actions.w3c_actions.pointer_action.release()
-            actions.perform()
-            return True
-        elif locator is not None and root is not None:
-            # Если указан локатор элемента и корневой элемент
-            target_element = root.get_element(locator)
-            x, y = target_element._get_center()
-            actions.w3c_actions.pointer_action.move_to_location(x, y)
-            actions.w3c_actions.pointer_action.release()
-            actions.perform()
-            return True
-        elif direction is not None and distance is not None:
-            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
-            window_size = adb.get_screen_resolution()
-            width = window_size[0]
-            height = window_size[1]
-
-            x2, y2 = find_coordinates_by_vector(width=width, height=height,
-                                                direction=direction, distance=distance,
-                                                start_x=x1, start_y=y1)
-            actions.w3c_actions.pointer_action.move_to_location(x2, y2)
-            actions.w3c_actions.pointer_action.release()
-            actions.perform()
-            return True
-
-        return False
+# coding: utf-8
+import logging
+from typing import Union, Tuple, Dict, List, Optional
+
+from appium.webdriver import WebElement
+from selenium.webdriver.common.action_chains import ActionChains
+from selenium.webdriver.common.actions import interaction
+from selenium.webdriver.common.actions.action_builder import ActionBuilder
+from selenium.webdriver.common.actions.pointer_input import PointerInput
+
+import config
+
+from AppiumWebElementExtended.web_element_get import WebElementGet
+from adb import adb
+from AppiumHelpers.helpers_decorators import wait_for_window_change
+from utils.utils import find_coordinates_by_vector
+
+
+class WebElementTap(WebElementGet):
+    """
+    Класс для выполнения действий нажатия (Tap), а также нажатия и перемещения с использованием элементов веб-страницы.
+    Наследуется от класса WebElementGet.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.driver = args[0]
+        self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+    def _tap(self,
+             positions: List[Tuple[int, int]],
+             duration: int = 0,
+             decorator_args: dict = None,
+             wait: bool = False) -> bool:
+        """
+        Выполняет нажатие на указанные координаты.
+
+        Аргументы:
+            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
+            duration (int): Длительность нажатия в миллисекундах.
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                    Например:
+                        decorator_args = {"timeout_window": 5,
+                                          "tries": 5}, где
+                        timeout_window (int): время ожидания изменения окна
+                        tries (int): количество попыток для изменения окна
+            wait (bool): Флаг, указывающий, нужно ли ожидать результата после нажатия.
+
+        Возвращает:
+            bool: True, если нажатие выполнено успешно; False в противном случае.
+        """
+
+        if wait:
+            # Если нужно ожидать результата после нажатия
+
+            if not decorator_args:
+                # Декоратор по умолчанию
+                decorator_args = {"timeout_window": 5,
+                                  "tries": 5}
+
+            return self._tap_to_element_and_wait(positions=positions, duration=duration, decorator_args=decorator_args)
+        else:
+            # Если не нужно ожидать результата после нажатия
+            return self._tap_to_element(positions=positions, duration=duration)
+
+    @wait_for_window_change()
+    def _tap_to_element_and_wait(self,
+                                 positions: List[Tuple[int, int]],
+                                 duration: int = 0,
+                                 decorator_args: dict = None, ):
+        return self.__tap(positions=positions, duration=duration)
+
+    def _tap_to_element(self,
+                        positions: List[Tuple[int, int]],
+                        duration: int = 0, ):
+        return self.__tap(positions=positions, duration=duration)
+
+    def __tap(self, positions: List[Tuple[int, int]], duration: Optional[int] = None):
+        """
+        Выполняет нажатие по указанным координатам.
+
+        Аргументы:
+            positions (List[Tuple[int, int]]): Список координат X и Y для нажатия.
+            duration (Optional[int]): Длительность нажатия в миллисекундах.
+
+        Возвращает:
+            bool: True, если нажатие выполнено успешно; False в противном случае.
+        """
+
+        try:
+            self.driver.tap(positions=positions, duration=duration)
+            return True
+        except Exception as e:
+            self.logger.error("some exception with __tap(): {}".format(e))
+            return False
+
+    def _double_tap(self,
+                    positions: Tuple[int, int],
+                    decorator_args: dict = None,
+                    wait: bool = False,
+                    pause: float = 0.2) -> bool:
+        """
+        Выполняет двойное нажатие (double tap) на указанных координатах.
+
+        Аргументы:
+            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
+            decorator_args (dict): Дополнительные аргументы для использования в декораторе.
+                Например:
+                    decorator_args = {"timeout_window": 5,
+                                      "tries": 5}, где
+                    timeout_window (int): время ожидания изменения окна
+                    tries (int): количество попыток для изменения окна
+            wait (bool): Флаг, указывающий, нужно ли ожидать изменения окна после двойного нажатия.
+            pause (float): Пауза между двумя нажатиями в секундах.
+
+        Возвращает:
+            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
+        """
+
+        # Декоратор по умолчанию
+        decorator_args = {"timeout_window": 5,
+                          "tries": 5}
+
+        if wait:
+            # Если нужно ожидать результата после двойного нажатия
+            return self._double_tap_to_element_and_wait(positions=positions, decorator_args=decorator_args, pause=pause)
+        else:
+            # Если не нужно ожидать результата после двойного нажатия
+            return self._double_tap_to_element(positions=positions, pause=pause)
+
+    @wait_for_window_change()
+    def _double_tap_to_element_and_wait(self, positions: Tuple[int, int], decorator_args: dict = None,
+                                        pause: float = 0.2) -> bool:
+        return self.__double_tap(positions=positions, pause=pause)
+
+    def _double_tap_to_element(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
+        return self.__double_tap(positions=positions, pause=pause)
+
+    def __double_tap(self, positions: Tuple[int, int], pause: float = 0.2) -> bool:
+        """
+        Выполняет двойное нажатие (double tap) по указанным координатам.
+
+        Аргументы:
+            positions (Tuple[int, int]): Координаты X и Y для двойного нажатия.
+            pause (float): Пауза между двумя нажатиями в секундах.
+
+        Возвращает:
+            bool: True, если двойное нажатие выполнено успешно; False в противном случае.
+        """
+        actions = ActionChains(self.driver)
+        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+        x = positions[0]
+        y = positions[1]
+
+        # Первое нажатие
+        actions.w3c_actions.pointer_action.move_to_location(x, y)
+        actions.w3c_actions.pointer_action.pointer_down()
+        actions.w3c_actions.pointer_action.pause(0.1)
+        actions.w3c_actions.pointer_action.pointer_up()
+        actions.w3c_actions.pointer_action.pause(pause)
+
+        # Второе нажатие
+        actions.w3c_actions.pointer_action.pointer_down()
+        actions.w3c_actions.pointer_action.pause(0.1)
+        actions.w3c_actions.pointer_action.release()
+
+        try:
+            actions.perform()
+            return True
+        except Exception as e:
+            self.logger.error("some exception with __double_tap(): {}".format(e))
+            return False
+
+    def _tap_and_move(self,
+                      root=None,
+                      locator: Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str] = None,
+                      x: int = None,
+                      y: int = None,
+                      direction: int = None,
+                      distance: int = None,
+                      ) -> bool:
+        """
+        Выполняет операцию "нажать и переместить" на веб-элементе или на указанных координатах.
+
+        Аргументы:
+            root (WebElementExtended): Корневой элемент, относительно которого будет выполнено нажатие и перемещение.
+            locator (Union[Tuple, WebElement, 'WebElementExtended', Dict[str, str], str]): Локатор элемента,
+                на который будет выполнено нажатие и перемещение.
+            x (int): Координата X для нажатия и перемещения.
+            y (int): Координата Y для нажатия и перемещения.
+            direction (int): Направление прокрутки в градусах (0 - вверх, 90 - вправо, 180 - вниз, 270 - влево).
+            distance (int): Расстояние прокрутки в пикселях.
+
+        Возвращает:
+            bool: True, если операция успешно выполнена; False в противном случае.
+        """
+        # Получение координат центра начальной позиции прокрутки
+        x1, y1 = self._get_center()
+
+        actions = ActionChains(self.driver)
+        actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+        actions.w3c_actions.pointer_action.move_to_location(x1, y1)
+        actions.w3c_actions.pointer_action.pointer_down()
+
+        # Проверка аргументов для определения типа операции
+        if (x is None and y is None) and locator is None and (direction is None and distance is None):
+            # Если не предоставлены аргументы
+            self.logger.error(f"_tap_and_move(): Нет аргументов")
+            return False
+        elif x is not None and y is not None:
+            # Если указаны координаты для нажатия и перемещения
+            actions.w3c_actions.pointer_action.move_to_location(x, y)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
+            return True
+        elif locator is not None and root is not None:
+            # Если указан локатор элемента и корневой элемент
+            target_element = root.get_element(locator)
+            x, y = target_element._get_center()
+            actions.w3c_actions.pointer_action.move_to_location(x, y)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
+            return True
+        elif direction is not None and distance is not None:
+            # Если предоставлены направление и расстояние, вычисляем целевую позицию прокрутки
+            window_size = adb.get_screen_resolution()
+            width = window_size[0]
+            height = window_size[1]
+
+            x2, y2 = find_coordinates_by_vector(width=width, height=height,
+                                                direction=direction, distance=distance,
+                                                start_x=x1, start_y=y1)
+            actions.w3c_actions.pointer_action.move_to_location(x2, y2)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
+            return True
+
+        return False
```

### Comparing `AppiumExtended-0.1.3/adb/adb.py` & `AppiumExtended-0.1.6/adb/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         x: Координата X для нажатия.
         y: Координата Y для нажатия.
 
     Возвращает:
         bool: True, если команда была успешно выполнена, False в противном случае.
     """
     # Формируем команду для выполнения нажатия по указанным координатам с использованием ADB
-    command = ['adb', 'shell', 'input', 'tap', x, y]
+    command = ['adb', 'shell', 'input', 'tap', str(x), str(y)]
     try:
         # Выполняем команду
         subprocess_run(command)
         return True
     except Exception as e:
         # Логируем ошибку, если возникло исключение
         logger.error("adb.tap()")
```

### Comparing `AppiumExtended-0.1.3/utils/operations.py` & `AppiumExtended-0.1.6/utils/operations.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.3/utils/utils.py` & `AppiumExtended-0.1.6/utils/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-import json
-import logging
-import math
-import os
-from typing import Tuple
-
-import config
-
-START_DIR = os.getcwd()
-PROJECT_ROOT_DIR = os.path.dirname(__file__)
-logger = logging.getLogger(config.APPIUM_LOG_NAME)
-
-
-def write_to_json(path, filename, data):
-    try:
-        filepath = os.path.join(START_DIR, path, filename)
-        with open(filepath, 'x', encoding='utf-8') as f:
-            json.dump(data, f)
-        return True
-    except:
-        return False
-
-
-def remove_keys_from_json_files_recursively(keys: list, path: str):
-    """
-    Метод рекурсивно проходит по всем вложенным папкам в поисках .json файлов.
-    В каждом файле удаляет ключи и значения заданные в параметрах.
-    Например:
-    keys_to_remove = ["1038",
-                      "1040",
-                      "1042",
-                      "qr",
-                      "1021",
-                      "1012",
-                      "1042",
-                      "1077",
-                      ]
-    path = os.path.join('test_data', 'FFD_1_05', 'cash')
-    operations.change_values_in_json_files_recursively(keys=keys_to_remove, path=path)
-    """
-    # Define the directory to traverse
-    root_dir = os.path.join(START_DIR, path)
-
-    # Traverse the directory tree and modify JSON files
-    for subdir, dirs, files in os.walk(root_dir):
-        for file in files:
-            # Check if the file is a JSON file
-            if file.endswith('.json'):
-                # Load the JSON data from the file
-                file_path = os.path.join(subdir, file)
-                print("file_path: ", file_path)
-                with open(file_path, 'r', encoding='utf-8') as f:
-                    data = json.load(f)
-
-                # Delete the text-value pair from the JSON data
-                for key in keys:
-                    if key in data:
-                        del data[key]
-
-                # Write the modified JSON data back to the file
-                with open(file_path, 'w', encoding='utf-8') as f:
-                    json.dump(data, f)
-
-
-def change_values_in_json_files_recursively(keys: dict, path: str):
-    """
-    Метод рекурсивно проходит по всем вложенным папкам в поисках .json файлов.
-    В каждом файле меняет значения у ключей заданных в параметрах.
-    Например:
-    keys = {
-    "1031": 0,
-    "1081": 1,
-    }
-    path = os.path.join('test_data', 'FFD_1_05', 'card')
-    operations.change_values_in_json_files_recursively(keys=keys, path=path)
-    """
-    print("change_values_in_json_files_recursively()")
-    print("keys: ", keys)
-    print("path: ", path)
-    # Define the directory to traverse
-    root_dir = os.path.join(START_DIR, path)
-
-    # Traverse the directory tree and modify JSON files
-    for subdir, dirs, files in os.walk(root_dir):
-        for file in files:
-            # Check if the file is a JSON file
-            if file.endswith('.json'):
-                # Load the JSON data from the file
-                file_path = os.path.join(subdir, file)
-                print("file_path: ", file_path)
-                with open(file_path, 'r', encoding='utf-8') as f:
-                    data = json.load(f)
-
-                # Delete the text-value pair from the JSON data
-                for key in keys:
-                    if key in data:
-                        print("data[text]: ", data[key])
-                        print("keys[text]: ", keys[key])
-                        data[key] = keys[key]
-
-                # Write the modified JSON data back to the file
-                with open(file_path, 'w', encoding='utf-8') as f:
-                    json.dump(data, f)
-
-
-def change_values_in_dict(dict_needs_to_change: dict, changes: dict) -> dict:
-    """
-    Метод изменяет поданный словарь, согласно поданным параметрам (поиск с заменой).
-    Если значение None, то удаляет ключ.
-    Возвращает измененный словарь.
-    """
-    logger.debug("change_values_in_dict()")
-    # Delete the text-value pair from the JSON data
-    count = 0
-    for key in changes:
-        if key in dict_needs_to_change:
-            if changes[key] is None:
-                dict_needs_to_change.pop(key)
-            else:
-                dict_needs_to_change[key] = changes[key]
-            count += 1
-    if count > 0:
-        logger.debug("change_values_in_dict(): Словарь подготовлен")
-        return dict_needs_to_change
-    else:
-        logger.debug("change_values_in_dict(): В словаре нечего менять")
-
-
-def find_coordinates_by_vector(width, height, direction: int, distance: int, start_x: int, start_y: int) -> Tuple[int, int]:
-    """
-    fill me
-    """
-
-    # Расчет конечной точки на основе направления и расстояния
-    angle_radians = direction * (math.pi / 180)  # Преобразование направления в радианы
-    dy = abs(distance * math.cos(angle_radians))
-    dx = abs(distance * math.sin(angle_radians))
-
-    if 0 <= direction <= 180:
-        x = start_x + dx
-    else:
-        x = start_x - dx
-
-    if 0 <= direction <= 90 or 270 <= direction <= 360:
-        y = start_y - dy
-    else:
-        y = start_y + dy
-
-    # Обрезка конечной точки до границ экрана
-    x2 = (max(0, min(x, width)))
-    y2 = (max(0, min(y, height)))
-
-    return x2, y2
-
-
-def calculate_center_of_coordinates(coordinates: Tuple[int, int, int, int]) -> Tuple[int, int]:
-    """
-    Вычисляет центр координат для четырех точек.
-
-    Аргументы:
-    coordinates (Tuple[int, int, int, int]): Кортеж из четырех целочисленных значений координат: x1, y1, x2, y2.
-
-    Возвращает:
-    Tuple[int, int]: Кортеж из двух целочисленных значений, представляющих координаты центра.
-
-    """
-    # Распаковываем координаты из кортежа
-    x1, y1, x2, y2 = coordinates
-
-    # Вычисляем центр по оси x путем сложения x1 и x2, деленного на 2
-    center_x = (x1 + x2) // 2
-
-    # Вычисляем центр по оси y путем сложения y1 и y2, деленного на 2
-    center_y = (y1 + y2) // 2
-
-    # Возвращаем кортеж с центральными координатами (center_x, center_y)
-    return center_x, center_y
-
-
-
-
-
+import json
+import logging
+import math
+import os
+from typing import Tuple
+
+import config
+
+START_DIR = os.getcwd()
+PROJECT_ROOT_DIR = os.path.dirname(__file__)
+logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+
+def write_to_json(path, filename, data):
+    try:
+        filepath = os.path.join(START_DIR, path, filename)
+        with open(filepath, 'x', encoding='utf-8') as f:
+            json.dump(data, f)
+        return True
+    except:
+        return False
+
+
+def remove_keys_from_json_files_recursively(keys: list, path: str):
+    """
+    Метод рекурсивно проходит по всем вложенным папкам в поисках .json файлов.
+    В каждом файле удаляет ключи и значения заданные в параметрах.
+    Например:
+    keys_to_remove = ["1038",
+                      "1040",
+                      "1042",
+                      "qr",
+                      "1021",
+                      "1012",
+                      "1042",
+                      "1077",
+                      ]
+    path = os.path.join('test_data', 'FFD_1_05', 'cash')
+    operations.change_values_in_json_files_recursively(keys=keys_to_remove, path=path)
+    """
+    # Define the directory to traverse
+    root_dir = os.path.join(START_DIR, path)
+
+    # Traverse the directory tree and modify JSON files
+    for subdir, dirs, files in os.walk(root_dir):
+        for file in files:
+            # Check if the file is a JSON file
+            if file.endswith('.json'):
+                # Load the JSON data from the file
+                file_path = os.path.join(subdir, file)
+                print("file_path: ", file_path)
+                with open(file_path, 'r', encoding='utf-8') as f:
+                    data = json.load(f)
+
+                # Delete the text-value pair from the JSON data
+                for key in keys:
+                    if key in data:
+                        del data[key]
+
+                # Write the modified JSON data back to the file
+                with open(file_path, 'w', encoding='utf-8') as f:
+                    json.dump(data, f)
+
+
+def change_values_in_json_files_recursively(keys: dict, path: str):
+    """
+    Метод рекурсивно проходит по всем вложенным папкам в поисках .json файлов.
+    В каждом файле меняет значения у ключей заданных в параметрах.
+    Например:
+    keys = {
+    "1031": 0,
+    "1081": 1,
+    }
+    path = os.path.join('test_data', 'FFD_1_05', 'card')
+    operations.change_values_in_json_files_recursively(keys=keys, path=path)
+    """
+    print("change_values_in_json_files_recursively()")
+    print("keys: ", keys)
+    print("path: ", path)
+    # Define the directory to traverse
+    root_dir = os.path.join(START_DIR, path)
+
+    # Traverse the directory tree and modify JSON files
+    for subdir, dirs, files in os.walk(root_dir):
+        for file in files:
+            # Check if the file is a JSON file
+            if file.endswith('.json'):
+                # Load the JSON data from the file
+                file_path = os.path.join(subdir, file)
+                print("file_path: ", file_path)
+                with open(file_path, 'r', encoding='utf-8') as f:
+                    data = json.load(f)
+
+                # Delete the text-value pair from the JSON data
+                for key in keys:
+                    if key in data:
+                        print("data[text]: ", data[key])
+                        print("keys[text]: ", keys[key])
+                        data[key] = keys[key]
+
+                # Write the modified JSON data back to the file
+                with open(file_path, 'w', encoding='utf-8') as f:
+                    json.dump(data, f)
+
+
+def change_values_in_dict(dict_needs_to_change: dict, changes: dict) -> dict:
+    """
+    Метод изменяет поданный словарь, согласно поданным параметрам (поиск с заменой).
+    Если значение None, то удаляет ключ.
+    Возвращает измененный словарь.
+    """
+    logger.debug("change_values_in_dict()")
+    # Delete the text-value pair from the JSON data
+    count = 0
+    for key in changes:
+        if key in dict_needs_to_change:
+            if changes[key] is None:
+                dict_needs_to_change.pop(key)
+            else:
+                dict_needs_to_change[key] = changes[key]
+            count += 1
+    if count > 0:
+        logger.debug("change_values_in_dict(): Словарь подготовлен")
+        return dict_needs_to_change
+    else:
+        logger.debug("change_values_in_dict(): В словаре нечего менять")
+
+
+def find_coordinates_by_vector(width, height, direction: int, distance: int, start_x: int, start_y: int) -> Tuple[int, int]:
+    """
+    fill me
+    """
+
+    # Расчет конечной точки на основе направления и расстояния
+    angle_radians = direction * (math.pi / 180)  # Преобразование направления в радианы
+    dy = abs(distance * math.cos(angle_radians))
+    dx = abs(distance * math.sin(angle_radians))
+
+    if 0 <= direction <= 180:
+        x = start_x + dx
+    else:
+        x = start_x - dx
+
+    if 0 <= direction <= 90 or 270 <= direction <= 360:
+        y = start_y - dy
+    else:
+        y = start_y + dy
+
+    # Обрезка конечной точки до границ экрана
+    x2 = (max(0, min(x, width)))
+    y2 = (max(0, min(y, height)))
+
+    return x2, y2
+
+
+def calculate_center_of_coordinates(coordinates: Tuple[int, int, int, int]) -> Tuple[int, int]:
+    """
+    Вычисляет центр координат для четырех точек.
+
+    Аргументы:
+    coordinates (Tuple[int, int, int, int]): Кортеж из четырех целочисленных значений координат: x1, y1, x2, y2.
+
+    Возвращает:
+    Tuple[int, int]: Кортеж из двух целочисленных значений, представляющих координаты центра.
+
+    """
+    # Распаковываем координаты из кортежа
+    x1, y1, x2, y2 = coordinates
+
+    # Вычисляем центр по оси x путем сложения x1 и x2, деленного на 2
+    center_x = (x1 + x2) // 2
+
+    # Вычисляем центр по оси y путем сложения y1 и y2, деленного на 2
+    center_y = (y1 + y2) // 2
+
+    # Возвращаем кортеж с центральными координатами (center_x, center_y)
+    return center_x, center_y
+
+
+
+
+
```

