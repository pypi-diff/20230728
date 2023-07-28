# Comparing `tmp/blaster-server-0.0.438b0.tar.gz` & `tmp/blaster-server-0.0.439.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.438b0.tar", last modified: Thu Jul 27 22:00:51 2023, max compression
+gzip compressed data, was "blaster-server-0.0.439.tar", last modified: Fri Jul 28 21:35:50 2023, max compression
```

## Comparing `blaster-server-0.0.438b0.tar` & `blaster-server-0.0.439.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.438b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.438b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.438b0/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.438b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-07-19 07:59:01.000000 blaster-server-0.0.438b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15799 2023-07-27 00:06:27.000000 blaster-server-0.0.438b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38638 2023-07-27 00:05:21.000000 blaster-server-0.0.438b0/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    44678 2023-07-27 19:45:14.000000 blaster-server-0.0.438b0/blaster/tools/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.438b0/blaster/tools/sanitize_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.438b0/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-07-27 22:00:51.000000 blaster-server-0.0.438b0/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-07-27 22:00:51.000000 blaster-server-0.0.438b0/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-07-27 22:00:51.000000 blaster-server-0.0.438b0/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-07-27 22:00:51.000000 blaster-server-0.0.438b0/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-07-27 22:00:51.000000 blaster-server-0.0.438b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.438b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-07-27 14:45:21.000000 blaster-server-0.0.438b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-27 22:00:51.095337 blaster-server-0.0.438b0/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.438b0/test/test_command_line_parser.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.438b0/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.438b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.438b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.439/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.439/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-28 21:35:50.748765 blaster-server-0.0.439/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.439/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.439/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.439/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.439/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.439/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-07-19 07:59:01.000000 blaster-server-0.0.439/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15799 2023-07-27 00:06:27.000000 blaster-server-0.0.439/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38638 2023-07-27 00:05:21.000000 blaster-server-0.0.439/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    44805 2023-07-28 20:32:15.000000 blaster-server-0.0.439/blaster/tools/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.439/blaster/tools/sanitize_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.439/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.439/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-07-28 21:35:50.748765 blaster-server-0.0.439/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-07-28 20:32:45.000000 blaster-server-0.0.439/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.439/test/test_command_line_parser.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.439/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.439/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.439/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.438b0/LICENSE.txt` & `blaster-server-0.0.439/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/PKG-INFO` & `blaster-server-0.0.439/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.438b0
+Version: 0.0.439
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.438b0/README.md` & `blaster-server-0.0.439/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/__init__.py` & `blaster-server-0.0.439/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/cloud/analytics.py` & `blaster-server-0.0.439/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.439/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.439/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/cloud/storage.py` & `blaster-server-0.0.439/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/config.py` & `blaster-server-0.0.439/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/connection_pool.py` & `blaster-server-0.0.439/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/env.py` & `blaster-server-0.0.439/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/logging.py` & `blaster-server-0.0.439/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/mongo_orm.py` & `blaster-server-0.0.439/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/schema.py` & `blaster-server-0.0.439/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/server.py` & `blaster-server-0.0.439/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/tools/__init__.py` & `blaster-server-0.0.439/blaster/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,15 +851,15 @@
 EMAIL_REGEX = re.compile(r'^[_a-z0-9-]+(\.[_a-z0-9-]+)*(\+[_a-z0-9-]+)?\@[a-z0-9-]+(\.[a-z0-9-]+)*(\.[a-z]{2,6})$')
 
 
 def is_valid_email(email):
 	return EMAIL_REGEX.match(email)
 
 
-SANITIZE_EMAIL_REGEX_NO_PLUS_ALLOWED = re.compile("\+[^@]*")
+SANITIZE_EMAIL_REGEX_NO_PLUS_ALLOWED = re.compile(r"\+[^@]*")
 
 
 def sanitize_email_id(email_id, plus_allowed=True):
 	if(not email_id):
 		return None
 	email_id = email_id.strip().lower()
 	if(not EMAIL_REGEX.match(email_id)):
@@ -1579,24 +1579,22 @@
 				func_name=func.__name__,
 				delay_ms=delay_ms,
 				exec_ms=exec_ms
 			)
 
 
 _process_task_queue.can_process = True
-_process_task_queue._background_thread_started = False
 # singleton
 
 
 def start_background_task_processors(n):
-	if(_process_task_queue._background_thread_started):
-		return
-	_process_task_queue._background_thread_started = True
-
 	global _partitioned_background_task_queues
+	if(_partitioned_background_task_queues != None):
+		return
+	_partitioned_background_task_queues = tuple()  # empty tuple, so we don't run this twice
 	_queues = []
 	for _ in range(n):
 		_queues.append(_queue := Queue())
 		_thread_to_start = Thread(
 			target=_process_task_queue,
 			args=(_queue,),
 		)
@@ -1617,17 +1615,23 @@
 	now_millis = cur_ms()
 	if(partition_key == None):
 		partition_key = now_millis  # choose a random key
 
 	if(not _process_task_queue.can_process):
 		raise Exception("Cannot submit tasks to a queue which is not processing")
 
-	if(not _process_task_queue._background_thread_started):
+	# wait for processors to start
+	while(not _partitioned_background_task_queues):
 		from blaster.config import NUM_BACKGROUND_TASK_PROCESSORS
 		start_background_task_processors(NUM_BACKGROUND_TASK_PROCESSORS or 4)
+		LOG_APP_INFO(
+			"background_threads_starting",
+			msg="waiting for background tasks processors to start",
+		)
+		sleep(0.1)
 
 	_queue = _partitioned_background_task_queues[hash(str(partition_key)) % len(_partitioned_background_task_queues)]
 	_queue.put((now_millis, func, args, kwargs))
 	try:
 		_item = _queue.peek(block=False)  # this won't block or raise exception
 		delay = _item[0] - now_millis
 		if(delay > 15000):
```

### Comparing `blaster-server-0.0.438b0/blaster/tools/sanitize_html.py` & `blaster-server-0.0.439/blaster/tools/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/data/countries.json` & `blaster-server-0.0.439/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.439/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/data_utils.py` & `blaster-server-0.0.439/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/events.py` & `blaster-server-0.0.439/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/fork.py` & `blaster-server-0.0.439/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.439/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.439/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/utils/xss_html.py` & `blaster-server-0.0.439/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/__init__.py` & `blaster-server-0.0.439/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.439/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_app.py` & `blaster-server-0.0.439/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_core.py` & `blaster-server-0.0.439/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.439/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.439/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_http.py` & `blaster-server-0.0.439/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_logging.py` & `blaster-server-0.0.439/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_socket.py` & `blaster-server-0.0.439/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.439/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_url.py` & `blaster-server-0.0.439/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/_utils.py` & `blaster-server-0.0.439/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/server.py` & `blaster-server-0.0.439/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.439/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.439/blaster_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.438b0
+Version: 0.0.439
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.438b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.439/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.439/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/mongo_ormexample.py` & `blaster-server-0.0.439/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/simple_examples.py` & `blaster-server-0.0.439/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/test_chat_room.py` & `blaster-server-0.0.439/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/tornado_hello_world.py` & `blaster-server-0.0.439/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/examples/wheezy_hello.py` & `blaster-server-0.0.439/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/setup.py` & `blaster-server-0.0.439/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.438b',
+	version='0.0.439',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.438b0/test/test_mongo_orm.py` & `blaster-server-0.0.439/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/test/test_phone_number_utils.py` & `blaster-server-0.0.439/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/test/test_schema.py` & `blaster-server-0.0.439/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/test/test_tools.py` & `blaster-server-0.0.439/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/test/test_utils.py` & `blaster-server-0.0.439/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.438b0/test/timeit_snippets.py` & `blaster-server-0.0.439/test/timeit_snippets.py`

 * *Files identical despite different names*

