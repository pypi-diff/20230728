# Comparing `tmp/elia_chat-0.1.0.tar.gz` & `tmp/elia_chat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elia_chat-0.1.0.tar", max compression
+gzip compressed data, was "elia_chat-0.2.0.tar", max compression
```

## Comparing `elia_chat-0.1.0.tar` & `elia_chat-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,24 @@
--rw-r--r--   0        0        0      110 2023-05-04 20:34:03.302813 elia_chat-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-04 16:19:27.149530 elia_chat-0.1.0/elia_chat/__init__.py
--rw-r--r--   0        0        0      862 2023-05-04 20:40:46.062451 elia_chat-0.1.0/elia_chat/app.py
--rw-r--r--   0        0        0      456 2023-05-04 20:16:38.678562 elia_chat-0.1.0/elia_chat/elia.scss
--rw-r--r--   0        0        0      185 2023-05-04 19:36:23.052712 elia_chat-0.1.0/elia_chat/models.py
--rw-r--r--   0        0        0     4626 2023-05-04 20:21:25.767427 elia_chat-0.1.0/elia_chat/widgets/__pycache__/conversation.cpython-310.pyc
--rw-r--r--   0        0        0     5020 2023-05-04 20:40:46.064934 elia_chat-0.1.0/elia_chat/widgets/conversation.py
--rw-r--r--   0        0        0      472 2023-05-04 20:40:46.059943 elia_chat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 elia_chat-0.1.0/setup.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 elia_chat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1827 2023-07-28 16:46:45.255626 elia_chat-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-04 16:19:27.149530 elia_chat-0.2.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     1495 2023-07-28 16:46:45.255892 elia_chat-0.2.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0      436 2023-07-28 16:46:45.256780 elia_chat-0.2.0/elia_chat/app.py
+-rw-r--r--   0        0        0     2697 2023-05-30 18:31:05.278158 elia_chat-0.2.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0        0 2023-07-28 16:46:45.256896 elia_chat-0.2.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1670 2023-06-09 20:15:04.806574 elia_chat-0.2.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      201 2023-07-28 16:46:45.257828 elia_chat-0.2.0/elia_chat/database/create_database.py
+-rw-r--r--   0        0        0     1977 2023-06-09 20:15:04.805077 elia_chat-0.2.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     2531 2023-07-28 16:46:45.258424 elia_chat-0.2.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     5621 2023-06-08 19:09:56.860546 elia_chat-0.2.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0     1319 2023-06-09 20:28:13.980800 elia_chat-0.2.0/elia_chat/models.py
+-rw-r--r--   0        0        0     4325 2023-05-30 20:15:10.408485 elia_chat-0.2.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     2378 2023-06-09 19:42:22.443881 elia_chat-0.2.0/elia_chat/screens/message_info_modal.py
+-rw-r--r--   0        0        0      801 2023-06-09 20:18:50.764174 elia_chat-0.2.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0      286 2023-05-23 21:08:47.713606 elia_chat-0.2.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0    11170 2023-07-28 16:46:45.259372 elia_chat-0.2.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0      877 2023-05-27 16:37:32.190885 elia_chat-0.2.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4563 2023-07-28 16:57:25.646333 elia_chat-0.2.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     4714 2023-05-24 19:12:58.245413 elia_chat-0.2.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0     2912 2023-06-08 19:11:26.791155 elia_chat-0.2.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     1446 2023-05-31 20:48:24.143848 elia_chat-0.2.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0      667 2023-07-28 16:54:18.567249 elia_chat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 elia_chat-0.2.0/PKG-INFO
```

