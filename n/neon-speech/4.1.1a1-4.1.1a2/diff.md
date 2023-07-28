# Comparing `tmp/neon_speech-4.1.1a1.tar.gz` & `tmp/neon_speech-4.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_speech-4.1.1a1.tar", last modified: Thu Jul 27 22:59:56 2023, max compression
+gzip compressed data, was "neon_speech-4.1.1a2.tar", last modified: Fri Jul 28 00:51:28 2023, max compression
```

## Comparing `neon_speech-4.1.1a1.tar` & `neon_speech-4.1.1a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:59:56.847667 neon_speech-4.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-27 22:59:56.847667 neon_speech-4.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:59:56.843667 neon_speech-4.1.1a1/neon_speech/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/stt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/neon_speech/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:59:56.847667 neon_speech-4.1.1a1/neon_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 22:59:56.000000 neon_speech-4.1.1a1/neon_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:59:56.847667 neon_speech-4.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-27 22:59:51.000000 neon_speech-4.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:51:28.277692 neon_speech-4.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-28 00:51:28.277692 neon_speech-4.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:51:28.277692 neon_speech-4.1.1a2/neon_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/stt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/neon_speech/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:51:28.277692 neon_speech-4.1.1a2/neon_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 00:51:28.000000 neon_speech-4.1.1a2/neon_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:51:28.277692 neon_speech-4.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-28 00:51:21.000000 neon_speech-4.1.1a2/setup.py
```

### Comparing `neon_speech-4.1.1a1/LICENSE.md` & `neon_speech-4.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/PKG-INFO` & `neon_speech-4.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_speech
-Version: 4.1.1a1
+Version: 4.1.1a2
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.1.1a1/README.md` & `neon_speech-4.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech/__init__.py` & `neon_speech-4.1.1a2/neon_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech/__main__.py` & `neon_speech-4.1.1a2/neon_speech/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech/cli.py` & `neon_speech-4.1.1a2/neon_speech/cli.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech/service.py` & `neon_speech-4.1.1a2/neon_speech/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,30 +109,52 @@
                                         watchdog=watchdog)
         self.daemon = daemonic
         self.config.bus = self.bus
         from neon_utils.signal_utils import init_signal_handlers, \
             init_signal_bus
         init_signal_bus(self.bus)
         init_signal_handlers()
+        try:
+            self._default_user = get_neon_user_config()
+        except PermissionError:
+            LOG.warning("Unable to get writable config path; fallback to /tmp")
+            self._default_user = get_neon_user_config("/tmp")
 
-        self._default_user = get_neon_user_config()
         self._default_user['user']['username'] = "local"
 
         self.lock = Lock()
-
+        self._stop_service = Event()
         if self.config.get('listener', {}).get('enable_stt_api', True):
             self.api_stt = STTFactory.create(config=self.config,
                                              results_event=None)
         else:
             LOG.info("Skipping api_stt init")
             self.api_stt = None
 
+    def run(self):
+        if self.config.get('listener', {}).get('enable_voice_loop', True):
+            OVOSDinkumVoiceService.run(self)
+        else:
+            LOG.info(f"Running without voice_loop")
+            self.register_event_handlers()
+            self.status.set_ready()
+            try:
+                self._stop_service.wait()
+            except KeyboardInterrupt:
+                self.status.set_stopping()
+            except Exception as e:
+                LOG.exception("voice_loop failed")
+                self.status.set_error(str(e))
+            LOG.info("Service stopped")
+            self._after_stop()
+
     def shutdown(self):
         LOG.info("Shutting Down")
         self.stop()
+        self._stop_service.set()
 
     def register_event_handlers(self):
         OVOSDinkumVoiceService.register_event_handlers(self)
         # Register handler for internet (re-)connection
         self.bus.on("mycroft.internet.connected",
                     self.handle_internet_connected)
         self.bus.on("ovos.phal.wifi.plugin.fully_offline",
```

### Comparing `neon_speech-4.1.1a1/neon_speech/stt.py` & `neon_speech-4.1.1a2/neon_speech/stt.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech/utils.py` & `neon_speech-4.1.1a2/neon_speech/utils.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.1.1a1/neon_speech.egg-info/PKG-INFO` & `neon_speech-4.1.1a2/neon_speech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 4.1.1a1
+Version: 4.1.1a2
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.1.1a1/setup.py` & `neon_speech-4.1.1a2/setup.py`

 * *Files identical despite different names*

