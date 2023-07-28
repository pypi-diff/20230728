# Comparing `tmp/swml-python-0.1.2.tar.gz` & `tmp/swml-python-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swml-python-0.1.2.tar", last modified: Fri Jul 28 17:07:13 2023, max compression
+gzip compressed data, was "swml-python-0.1.2.1.tar", last modified: Fri Jul 28 17:20:10 2023, max compression
```

## Comparing `swml-python-0.1.2.tar` & `swml-python-0.1.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:07:13.066376 swml-python-0.1.2/
--rw-rw-rw-   0        0        0        2 2023-07-16 09:58:28.000000 swml-python-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-07-21 22:53:30.000000 swml-python-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7484 2023-07-28 17:07:13.066376 swml-python-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6778 2023-07-21 23:25:09.000000 swml-python-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 17:07:13.066376 swml-python-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-07-28 17:06:27.000000 swml-python-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:07:13.012319 swml-python-0.1.2/swml/
--rw-rw-rw-   0        0        0      367 2023-07-28 16:50:46.000000 swml-python-0.1.2/swml/__init__.py
--rw-rw-rw-   0        0        0    16948 2023-07-21 21:48:55.000000 swml-python-0.1.2/swml/swml_instructions.py
--rw-rw-rw-   0        0        0    14355 2023-07-21 21:47:41.000000 swml-python-0.1.2/swml/swml_response.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:07:13.016318 swml-python-0.1.2/swml_python.egg-info/
--rw-rw-rw-   0        0        0     7484 2023-07-28 17:07:12.000000 swml-python-0.1.2/swml_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2594 2023-07-28 17:07:13.000000 swml-python-0.1.2/swml_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:07:12.000000 swml-python-0.1.2/swml_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-28 17:07:12.000000 swml-python-0.1.2/swml_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 17:07:12.000000 swml-python-0.1.2/swml_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 17:07:13.039363 swml-python-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-07-18 00:40:23.000000 swml-python-0.1.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:07:13.065376 swml-python-0.1.2/tests/__pycache__/
--rw-rw-rw-   0        0        0      153 2023-07-18 01:12:56.000000 swml-python-0.1.2/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1319 2023-07-20 15:35:07.000000 swml-python-0.1.2/tests/__pycache__/test_swml_add_instruction.cpython-310.pyc
--rw-rw-rw-   0        0        0     3649 2023-07-21 17:13:02.000000 swml-python-0.1.2/tests/__pycache__/test_swml_ai.cpython-310.pyc
--rw-rw-rw-   0        0        0     1765 2023-07-20 17:29:01.000000 swml-python-0.1.2/tests/__pycache__/test_swml_answer_hangup.cpython-310.pyc
--rw-rw-rw-   0        0        0     1318 2023-07-21 15:55:18.000000 swml-python-0.1.2/tests/__pycache__/test_swml_cond.cpython-310.pyc
--rw-rw-rw-   0        0        0     3010 2023-07-21 21:47:41.000000 swml-python-0.1.2/tests/__pycache__/test_swml_connect.cpython-310.pyc
--rw-rw-rw-   0        0        0     1125 2023-07-20 15:33:07.000000 swml-python-0.1.2/tests/__pycache__/test_swml_denoise.cpython-310.pyc
--rw-rw-rw-   0        0        0     1450 2023-07-21 16:03:52.000000 swml-python-0.1.2/tests/__pycache__/test_swml_execute.cpython-310.pyc
--rw-rw-rw-   0        0        0     1348 2023-07-21 16:49:58.000000 swml-python-0.1.2/tests/__pycache__/test_swml_goto.cpython-310.pyc
--rw-rw-rw-   0        0        0     1268 2023-07-20 12:36:18.000000 swml-python-0.1.2/tests/__pycache__/test_swml_join_room.cpython-310.pyc
--rw-rw-rw-   0        0        0     1438 2023-07-20 12:23:03.000000 swml-python-0.1.2/tests/__pycache__/test_swml_play.cpython-310.pyc
--rw-rw-rw-   0        0        0     1796 2023-07-20 12:21:23.000000 swml-python-0.1.2/tests/__pycache__/test_swml_prompt.cpython-310.pyc
--rw-rw-rw-   0        0        0     1168 2023-07-20 15:36:13.000000 swml-python-0.1.2/tests/__pycache__/test_swml_receive_fax.cpython-310.pyc
--rw-rw-rw-   0        0        0     1580 2023-07-21 16:02:26.000000 swml-python-0.1.2/tests/__pycache__/test_swml_record.cpython-310.pyc
--rw-rw-rw-   0        0        0     1690 2023-07-21 16:02:26.000000 swml-python-0.1.2/tests/__pycache__/test_swml_record_call.cpython-310.pyc
--rw-rw-rw-   0        0        0     1600 2023-07-21 16:10:06.000000 swml-python-0.1.2/tests/__pycache__/test_swml_request.cpython-310.pyc
--rw-rw-rw-   0        0        0     1252 2023-07-21 16:05:34.000000 swml-python-0.1.2/tests/__pycache__/test_swml_return.cpython-310.pyc
--rw-rw-rw-   0        0        0     1295 2023-07-21 21:36:38.000000 swml-python-0.1.2/tests/__pycache__/test_swml_send_digits.cpython-310.pyc
--rw-rw-rw-   0        0        0     1304 2023-07-20 15:39:15.000000 swml-python-0.1.2/tests/__pycache__/test_swml_send_fax.cpython-310.pyc
--rw-rw-rw-   0        0        0     1569 2023-07-21 21:49:43.000000 swml-python-0.1.2/tests/__pycache__/test_swml_send_sms.cpython-310.pyc
--rw-rw-rw-   0        0        0     1268 2023-07-21 15:34:38.000000 swml-python-0.1.2/tests/__pycache__/test_swml_set.cpython-310.pyc
--rw-rw-rw-   0        0        0     1539 2023-07-20 15:47:53.000000 swml-python-0.1.2/tests/__pycache__/test_swml_sip_refer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1180 2023-07-20 15:35:07.000000 swml-python-0.1.2/tests/__pycache__/test_swml_stop_denoise.cpython-310.pyc
--rw-rw-rw-   0        0        0     1366 2023-07-20 15:35:07.000000 swml-python-0.1.2/tests/__pycache__/test_swml_stop_record_call.cpython-310.pyc
--rw-rw-rw-   0        0        0     1263 2023-07-21 15:16:34.000000 swml-python-0.1.2/tests/__pycache__/test_swml_stop_tap.cpython-310.pyc
--rw-rw-rw-   0        0        0     1533 2023-07-21 16:49:58.000000 swml-python-0.1.2/tests/__pycache__/test_swml_switch.cpython-310.pyc
--rw-rw-rw-   0        0        0     1376 2023-07-21 15:25:35.000000 swml-python-0.1.2/tests/__pycache__/test_swml_tap.cpython-310.pyc
--rw-rw-rw-   0        0        0     1471 2023-07-21 15:36:23.000000 swml-python-0.1.2/tests/__pycache__/test_swml_transfer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1219 2023-07-21 15:35:12.000000 swml-python-0.1.2/tests/__pycache__/test_swml_unset.cpython-310.pyc
--rw-rw-rw-   0        0        0      931 2023-07-20 15:34:41.000000 swml-python-0.1.2/tests/test_swml_add_instruction.py
--rw-rw-rw-   0        0        0     5293 2023-07-21 17:11:07.000000 swml-python-0.1.2/tests/test_swml_ai.py
--rw-rw-rw-   0        0        0     1552 2023-07-20 17:29:01.000000 swml-python-0.1.2/tests/test_swml_answer_hangup.py
--rw-rw-rw-   0        0        0     1023 2023-07-21 15:55:18.000000 swml-python-0.1.2/tests/test_swml_cond.py
--rw-rw-rw-   0        0        0     3203 2023-07-21 21:47:41.000000 swml-python-0.1.2/tests/test_swml_connect.py
--rw-rw-rw-   0        0        0      721 2023-07-20 15:33:07.000000 swml-python-0.1.2/tests/test_swml_denoise.py
--rw-rw-rw-   0        0        0     1300 2023-07-21 16:03:52.000000 swml-python-0.1.2/tests/test_swml_execute.py
--rw-rw-rw-   0        0        0     1067 2023-07-21 16:49:52.000000 swml-python-0.1.2/tests/test_swml_goto.py
--rw-rw-rw-   0        0        0      870 2023-07-20 12:36:18.000000 swml-python-0.1.2/tests/test_swml_join_room.py
--rw-rw-rw-   0        0        0     1339 2023-07-20 12:23:02.000000 swml-python-0.1.2/tests/test_swml_play.py
--rw-rw-rw-   0        0        0     2053 2023-07-20 11:37:48.000000 swml-python-0.1.2/tests/test_swml_prompt.py
--rw-rw-rw-   0        0        0      746 2023-07-20 15:36:13.000000 swml-python-0.1.2/tests/test_swml_receive_fax.py
--rw-rw-rw-   0        0        0     1631 2023-07-21 16:02:26.000000 swml-python-0.1.2/tests/test_swml_record.py
--rw-rw-rw-   0        0        0     1788 2023-07-21 16:02:26.000000 swml-python-0.1.2/tests/test_swml_record_call.py
--rw-rw-rw-   0        0        0     1489 2023-07-21 16:10:06.000000 swml-python-0.1.2/tests/test_swml_request.py
--rw-rw-rw-   0        0        0      874 2023-07-21 16:05:34.000000 swml-python-0.1.2/tests/test_swml_return.py
--rw-rw-rw-   0        0        0      878 2023-07-21 21:36:38.000000 swml-python-0.1.2/tests/test_swml_send_digits.py
--rw-rw-rw-   0        0        0     1032 2023-07-20 15:39:15.000000 swml-python-0.1.2/tests/test_swml_send_fax.py
--rw-rw-rw-   0        0        0     1368 2023-07-21 21:49:43.000000 swml-python-0.1.2/tests/test_swml_send_sms.py
--rw-rw-rw-   0        0        0      943 2023-07-21 15:34:38.000000 swml-python-0.1.2/tests/test_swml_set.py
--rw-rw-rw-   0        0        0     1595 2023-07-20 15:47:45.000000 swml-python-0.1.2/tests/test_swml_sip_refer.py
--rw-rw-rw-   0        0        0      754 2023-07-20 15:35:07.000000 swml-python-0.1.2/tests/test_swml_stop_denoise.py
--rw-rw-rw-   0        0        0      963 2023-07-20 15:34:41.000000 swml-python-0.1.2/tests/test_swml_stop_record_call.py
--rw-rw-rw-   0        0        0      870 2023-07-21 15:16:34.000000 swml-python-0.1.2/tests/test_swml_stop_tap.py
--rw-rw-rw-   0        0        0     1399 2023-07-21 16:49:57.000000 swml-python-0.1.2/tests/test_swml_switch.py
--rw-rw-rw-   0        0        0     1139 2023-07-21 15:25:35.000000 swml-python-0.1.2/tests/test_swml_tap.py
--rw-rw-rw-   0        0        0     1271 2023-07-21 15:36:23.000000 swml-python-0.1.2/tests/test_swml_transfer.py
--rw-rw-rw-   0        0        0      825 2023-07-21 15:35:12.000000 swml-python-0.1.2/tests/test_swml_unset.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:20:10.665054 swml-python-0.1.2.1/
+-rw-rw-rw-   0        0        0        2 2023-07-16 09:58:28.000000 swml-python-0.1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-07-21 22:53:30.000000 swml-python-0.1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7486 2023-07-28 17:20:10.664055 swml-python-0.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6778 2023-07-21 23:25:09.000000 swml-python-0.1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:20:10.665054 swml-python-0.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-07-28 17:19:57.000000 swml-python-0.1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:20:10.610186 swml-python-0.1.2.1/swml/
+-rw-rw-rw-   0        0        0      367 2023-07-28 16:50:46.000000 swml-python-0.1.2.1/swml/__init__.py
+-rw-rw-rw-   0        0        0    16948 2023-07-21 21:48:55.000000 swml-python-0.1.2.1/swml/swml_instructions.py
+-rw-rw-rw-   0        0        0    14355 2023-07-21 21:47:41.000000 swml-python-0.1.2.1/swml/swml_response.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:20:10.614186 swml-python-0.1.2.1/swml_python.egg-info/
+-rw-rw-rw-   0        0        0     7486 2023-07-28 17:20:10.000000 swml-python-0.1.2.1/swml_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2594 2023-07-28 17:20:10.000000 swml-python-0.1.2.1/swml_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:20:10.000000 swml-python-0.1.2.1/swml_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-28 17:20:10.000000 swml-python-0.1.2.1/swml_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 17:20:10.000000 swml-python-0.1.2.1/swml_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 17:20:10.638479 swml-python-0.1.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-18 00:40:23.000000 swml-python-0.1.2.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:20:10.663054 swml-python-0.1.2.1/tests/__pycache__/
+-rw-rw-rw-   0        0        0      153 2023-07-18 01:12:56.000000 swml-python-0.1.2.1/tests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1319 2023-07-20 15:35:07.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_add_instruction.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3649 2023-07-21 17:13:02.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_ai.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1765 2023-07-20 17:29:01.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_answer_hangup.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1318 2023-07-21 15:55:18.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_cond.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3010 2023-07-21 21:47:41.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_connect.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1125 2023-07-20 15:33:07.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_denoise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1450 2023-07-21 16:03:52.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_execute.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1348 2023-07-21 16:49:58.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_goto.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1268 2023-07-20 12:36:18.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_join_room.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1438 2023-07-20 12:23:03.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_play.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1796 2023-07-20 12:21:23.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_prompt.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1168 2023-07-20 15:36:13.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_receive_fax.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1580 2023-07-21 16:02:26.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_record.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1690 2023-07-21 16:02:26.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_record_call.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1600 2023-07-21 16:10:06.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_request.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1252 2023-07-21 16:05:34.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_return.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1295 2023-07-21 21:36:38.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_send_digits.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1304 2023-07-20 15:39:15.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_send_fax.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1569 2023-07-21 21:49:43.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_send_sms.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1268 2023-07-21 15:34:38.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_set.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1539 2023-07-20 15:47:53.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_sip_refer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1180 2023-07-20 15:35:07.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_denoise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1366 2023-07-20 15:35:07.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_record_call.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1263 2023-07-21 15:16:34.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_tap.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1533 2023-07-21 16:49:58.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_switch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1376 2023-07-21 15:25:35.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_tap.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1471 2023-07-21 15:36:23.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_transfer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1219 2023-07-21 15:35:12.000000 swml-python-0.1.2.1/tests/__pycache__/test_swml_unset.cpython-310.pyc
+-rw-rw-rw-   0        0        0      931 2023-07-20 15:34:41.000000 swml-python-0.1.2.1/tests/test_swml_add_instruction.py
+-rw-rw-rw-   0        0        0     5293 2023-07-21 17:11:07.000000 swml-python-0.1.2.1/tests/test_swml_ai.py
+-rw-rw-rw-   0        0        0     1552 2023-07-20 17:29:01.000000 swml-python-0.1.2.1/tests/test_swml_answer_hangup.py
+-rw-rw-rw-   0        0        0     1023 2023-07-21 15:55:18.000000 swml-python-0.1.2.1/tests/test_swml_cond.py
+-rw-rw-rw-   0        0        0     3203 2023-07-21 21:47:41.000000 swml-python-0.1.2.1/tests/test_swml_connect.py
+-rw-rw-rw-   0        0        0      721 2023-07-20 15:33:07.000000 swml-python-0.1.2.1/tests/test_swml_denoise.py
+-rw-rw-rw-   0        0        0     1300 2023-07-21 16:03:52.000000 swml-python-0.1.2.1/tests/test_swml_execute.py
+-rw-rw-rw-   0        0        0     1067 2023-07-21 16:49:52.000000 swml-python-0.1.2.1/tests/test_swml_goto.py
+-rw-rw-rw-   0        0        0      870 2023-07-20 12:36:18.000000 swml-python-0.1.2.1/tests/test_swml_join_room.py
+-rw-rw-rw-   0        0        0     1339 2023-07-20 12:23:02.000000 swml-python-0.1.2.1/tests/test_swml_play.py
+-rw-rw-rw-   0        0        0     2053 2023-07-20 11:37:48.000000 swml-python-0.1.2.1/tests/test_swml_prompt.py
+-rw-rw-rw-   0        0        0      746 2023-07-20 15:36:13.000000 swml-python-0.1.2.1/tests/test_swml_receive_fax.py
+-rw-rw-rw-   0        0        0     1631 2023-07-21 16:02:26.000000 swml-python-0.1.2.1/tests/test_swml_record.py
+-rw-rw-rw-   0        0        0     1788 2023-07-21 16:02:26.000000 swml-python-0.1.2.1/tests/test_swml_record_call.py
+-rw-rw-rw-   0        0        0     1489 2023-07-21 16:10:06.000000 swml-python-0.1.2.1/tests/test_swml_request.py
+-rw-rw-rw-   0        0        0      874 2023-07-21 16:05:34.000000 swml-python-0.1.2.1/tests/test_swml_return.py
+-rw-rw-rw-   0        0        0      878 2023-07-21 21:36:38.000000 swml-python-0.1.2.1/tests/test_swml_send_digits.py
+-rw-rw-rw-   0        0        0     1032 2023-07-20 15:39:15.000000 swml-python-0.1.2.1/tests/test_swml_send_fax.py
+-rw-rw-rw-   0        0        0     1368 2023-07-21 21:49:43.000000 swml-python-0.1.2.1/tests/test_swml_send_sms.py
+-rw-rw-rw-   0        0        0      943 2023-07-21 15:34:38.000000 swml-python-0.1.2.1/tests/test_swml_set.py
+-rw-rw-rw-   0        0        0     1595 2023-07-20 15:47:45.000000 swml-python-0.1.2.1/tests/test_swml_sip_refer.py
+-rw-rw-rw-   0        0        0      754 2023-07-20 15:35:07.000000 swml-python-0.1.2.1/tests/test_swml_stop_denoise.py
+-rw-rw-rw-   0        0        0      963 2023-07-20 15:34:41.000000 swml-python-0.1.2.1/tests/test_swml_stop_record_call.py
+-rw-rw-rw-   0        0        0      870 2023-07-21 15:16:34.000000 swml-python-0.1.2.1/tests/test_swml_stop_tap.py
+-rw-rw-rw-   0        0        0     1399 2023-07-21 16:49:57.000000 swml-python-0.1.2.1/tests/test_swml_switch.py
+-rw-rw-rw-   0        0        0     1139 2023-07-21 15:25:35.000000 swml-python-0.1.2.1/tests/test_swml_tap.py
+-rw-rw-rw-   0        0        0     1271 2023-07-21 15:36:23.000000 swml-python-0.1.2.1/tests/test_swml_transfer.py
+-rw-rw-rw-   0        0        0      825 2023-07-21 15:35:12.000000 swml-python-0.1.2.1/tests/test_swml_unset.py
```

### Comparing `swml-python-0.1.2/PKG-INFO` & `swml-python-0.1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swml-python
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: A Python wrapper for the new SignalWire product SWML (SignalWire MarkUp Language) 
 Home-page: https://github.com/Devon-White/SWML-python
 Author: Devon White
 Author-email: devon.white@signalwire.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `swml-python-0.1.2/README.md` & `swml-python-0.1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/swml/swml_instructions.py` & `swml-python-0.1.2.1/swml/swml_instructions.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/swml/swml_response.py` & `swml-python-0.1.2.1/swml/swml_response.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/swml_python.egg-info/PKG-INFO` & `swml-python-0.1.2.1/swml_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swml-python
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: A Python wrapper for the new SignalWire product SWML (SignalWire MarkUp Language) 
 Home-page: https://github.com/Devon-White/SWML-python
 Author: Devon White
 Author-email: devon.white@signalwire.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `swml-python-0.1.2/swml_python.egg-info/SOURCES.txt` & `swml-python-0.1.2.1/swml_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_add_instruction.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_add_instruction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_ai.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_ai.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_answer_hangup.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_answer_hangup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_cond.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_cond.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_connect.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_denoise.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_denoise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_execute.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_execute.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_goto.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_goto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_join_room.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_join_room.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_play.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_play.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_prompt.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_prompt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_receive_fax.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_receive_fax.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_record.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_record.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_record_call.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_record_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_request.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_request.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_return.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_return.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_send_digits.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_send_digits.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_send_fax.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_send_fax.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_send_sms.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_send_sms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_set.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_set.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_sip_refer.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_sip_refer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_stop_denoise.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_denoise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_stop_record_call.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_record_call.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_stop_tap.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_stop_tap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_switch.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_switch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_tap.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_tap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_transfer.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_transfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/__pycache__/test_swml_unset.cpython-310.pyc` & `swml-python-0.1.2.1/tests/__pycache__/test_swml_unset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_add_instruction.py` & `swml-python-0.1.2.1/tests/test_swml_add_instruction.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_ai.py` & `swml-python-0.1.2.1/tests/test_swml_ai.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_answer_hangup.py` & `swml-python-0.1.2.1/tests/test_swml_answer_hangup.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_cond.py` & `swml-python-0.1.2.1/tests/test_swml_cond.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_connect.py` & `swml-python-0.1.2.1/tests/test_swml_connect.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_denoise.py` & `swml-python-0.1.2.1/tests/test_swml_denoise.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_execute.py` & `swml-python-0.1.2.1/tests/test_swml_execute.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_goto.py` & `swml-python-0.1.2.1/tests/test_swml_goto.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_join_room.py` & `swml-python-0.1.2.1/tests/test_swml_join_room.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_play.py` & `swml-python-0.1.2.1/tests/test_swml_play.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_prompt.py` & `swml-python-0.1.2.1/tests/test_swml_prompt.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_receive_fax.py` & `swml-python-0.1.2.1/tests/test_swml_receive_fax.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_record.py` & `swml-python-0.1.2.1/tests/test_swml_record.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_record_call.py` & `swml-python-0.1.2.1/tests/test_swml_record_call.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_request.py` & `swml-python-0.1.2.1/tests/test_swml_request.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_return.py` & `swml-python-0.1.2.1/tests/test_swml_return.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_send_digits.py` & `swml-python-0.1.2.1/tests/test_swml_send_digits.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_send_fax.py` & `swml-python-0.1.2.1/tests/test_swml_send_fax.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_send_sms.py` & `swml-python-0.1.2.1/tests/test_swml_send_sms.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_set.py` & `swml-python-0.1.2.1/tests/test_swml_set.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_sip_refer.py` & `swml-python-0.1.2.1/tests/test_swml_sip_refer.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_stop_denoise.py` & `swml-python-0.1.2.1/tests/test_swml_stop_denoise.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_stop_record_call.py` & `swml-python-0.1.2.1/tests/test_swml_stop_record_call.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_stop_tap.py` & `swml-python-0.1.2.1/tests/test_swml_stop_tap.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_switch.py` & `swml-python-0.1.2.1/tests/test_swml_switch.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_tap.py` & `swml-python-0.1.2.1/tests/test_swml_tap.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_transfer.py` & `swml-python-0.1.2.1/tests/test_swml_transfer.py`

 * *Files identical despite different names*

### Comparing `swml-python-0.1.2/tests/test_swml_unset.py` & `swml-python-0.1.2.1/tests/test_swml_unset.py`

 * *Files identical despite different names*

