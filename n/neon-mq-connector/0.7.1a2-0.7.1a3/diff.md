# Comparing `tmp/neon_mq_connector-0.7.1a2.tar.gz` & `tmp/neon_mq_connector-0.7.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_mq_connector-0.7.1a2.tar", last modified: Thu Jul 27 00:59:20 2023, max compression
+gzip compressed data, was "neon_mq_connector-0.7.1a3.tar", last modified: Fri Jul 28 00:52:43 2023, max compression
```

## Comparing `neon_mq_connector-0.7.1a2.tar` & `neon_mq_connector-0.7.1a3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.354092 neon_mq_connector-0.7.1a2/neon_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32870 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/rabbit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/thread_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/neon_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32870 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/rabbit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/neon_mq_connector/utils/thread_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 00:52:43.000000 neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 00:52:43.083589 neon_mq_connector-0.7.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-28 00:52:39.000000 neon_mq_connector-0.7.1a3/setup.py
```

### Comparing `neon_mq_connector-0.7.1a2/LICENSE.md` & `neon_mq_connector-0.7.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/PKG-INFO` & `neon_mq_connector-0.7.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_mq_connector
-Version: 0.7.1a2
+Version: 0.7.1a3
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.1a2/README.md` & `neon_mq_connector-0.7.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/__init__.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/config.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/connector.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/connector.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/__init__.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/client_utils.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/client_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,16 +90,25 @@
 
     def handle_mq_response(channel: Channel, method, _, body):
         """
         Method that handles Neon API output.
         In case received output message with the desired id, event stops
         """
         api_output = b64_to_dict(body)
-        api_output_msg_id = api_output.get('message_id', None)
 
+        # The Messagebus connector generates a unique `message_id` for each
+        # response message. Check context for the original one; otherwise,
+        # check in output directly as some APIs emit responses without a unique
+        # message_id
+        api_output_msg_id = \
+            api_output.get('context',
+                           api_output).get('mq', api_output).get('message_id')
+        # TODO: One of these specs should be deprecated
+        if api_output_msg_id != api_output.get('message_id'):
+            LOG.debug(f"Handling message_id from response context")
         if api_output_msg_id == message_id:
             LOG.debug(f'MQ output: {api_output}')
             channel.basic_ack(delivery_tag=method.delivery_tag)
             channel.close()
             response_data.update(api_output)
             response_event.set()
         else:
```

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/connection_utils.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/network_utils.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/rabbit_utils.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/rabbit_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/thread_utils.py` & `neon_mq_connector-0.7.1a3/neon_mq_connector/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/PKG-INFO` & `neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mq-connector
-Version: 0.7.1a2
+Version: 0.7.1a3
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/SOURCES.txt` & `neon_mq_connector-0.7.1a3/neon_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a2/setup.py` & `neon_mq_connector-0.7.1a3/setup.py`

 * *Files identical despite different names*

