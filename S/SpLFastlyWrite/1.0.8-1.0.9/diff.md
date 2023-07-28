# Comparing `tmp/SpLFastlyWrite-1.0.8.tar.gz` & `tmp/SpLFastlyWrite-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpLFastlyWrite-1.0.8.tar", last modified: Mon Jul 10 09:11:05 2023, max compression
+gzip compressed data, was "/root/fw/dist/.tmp-91hgdf3n/SpLFastlyWrite-1.0.9.tar", last modified: Fri Jul 28 12:14:40 2023, max compression
```

## Comparing `SpLFastlyWrite-1.0.8.tar` & `SpLFastlyWrite-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-07-10 09:09:21.000000 SpLFastlyWrite-1.0.8/LICENSE
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-07-10 09:09:21.000000 SpLFastlyWrite-1.0.8/README.md
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.942369 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/SOURCES.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/dependency_links.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/not-zip-safe
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/top_level.txt
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.942369 SpLFastlyWrite-1.0.8/Spoiled/
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.945369 SpLFastlyWrite-1.0.8/Spoiled/Database/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-07-10 09:09:25.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/chat_words.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/chats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/completed.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/global_stats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/privacy.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/record.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/user_chat_info.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/users.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.946369 SpLFastlyWrite-1.0.8/Spoiled/Shannu/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/alpha.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1483 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/config.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1276 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/shivi.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/words.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     9309 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/callbacks.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6640 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/eval.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2891 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/fw.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/help.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/image.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/inline.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/leaderboard.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/served.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3762 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/start.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/templates.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/watchers.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       86 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/setup.cfg
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/
+-rw-rw-r--   0 root         (0) root         (0)     1074 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      657 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       16 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      657 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1118 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-28 12:14:37.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)        8 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/Spoiled/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/
+-rw-rw-r--   0 root         (0) root         (0)      195 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      788 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/chat_words.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/chats.py
+-rw-rw-r--   0 root         (0) root         (0)     1458 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/coins.py
+-rw-rw-r--   0 root         (0) root         (0)      937 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/completed.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/global_stats.py
+-rw-rw-r--   0 root         (0) root         (0)      560 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/privacy.py
+-rw-rw-r--   0 root         (0) root         (0)      443 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/record.py
+-rw-rw-r--   0 root         (0) root         (0)      634 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/user_chat_info.py
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Database/users.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/
+-rw-rw-r--   0 root         (0) root         (0)       51 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       41 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/alpha.py
+-rw-rw-r--   0 root         (0) root         (0)     1437 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/config.py
+-rw-rw-r--   0 root         (0) root         (0)     1464 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/shivi.py
+-rw-rw-r--   0 root         (0) root         (0)      456 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/Shannu/words.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/
+-rw-rw-r--   0 root         (0) root         (0)     1670 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9002 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/callbacks.py
+-rw-rw-r--   0 root         (0) root         (0)      524 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/coins.py
+-rw-rw-r--   0 root         (0) root         (0)     6431 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/eval.py
+-rw-rw-r--   0 root         (0) root         (0)     2785 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/fw.py
+-rw-rw-r--   0 root         (0) root         (0)      298 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/handlers.py
+-rw-rw-r--   0 root         (0) root         (0)     1074 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/help.py
+-rw-rw-r--   0 root         (0) root         (0)      932 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/image.py
+-rw-rw-r--   0 root         (0) root         (0)     1341 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/inline.py
+-rw-rw-r--   0 root         (0) root         (0)      770 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/leaderboard.py
+-rw-rw-r--   0 root         (0) root         (0)      816 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/served.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/start.py
+-rw-rw-r--   0 root         (0) root         (0)      523 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/templates.py
+-rw-rw-r--   0 root         (0) root         (0)       34 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/watchers.py
+-rw-rw-r--   0 root         (0) root         (0)       82 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/Spoiled/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-28 12:14:40.000000 SpLFastlyWrite-1.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      969 2023-07-28 12:12:53.000000 SpLFastlyWrite-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `SpLFastlyWrite-1.0.8/LICENSE` & `SpLFastlyWrite-1.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Keshava Tripathi 
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Keshava Tripathi 
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `SpLFastlyWrite-1.0.8/PKG-INFO` & `SpLFastlyWrite-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.8
+Version: 1.0.9
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/PKG-INFO` & `SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.8
+Version: 1.0.9
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/SOURCES.txt` & `SpLFastlyWrite-1.0.9/SpLFastlyWrite.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 Spoiled/Shannu/shivi.py
 Spoiled/Shannu/words.py
 Spoiled/SpoiledPlugins/__init__.py
 Spoiled/SpoiledPlugins/callbacks.py
 Spoiled/SpoiledPlugins/coins.py
 Spoiled/SpoiledPlugins/eval.py
 Spoiled/SpoiledPlugins/fw.py
+Spoiled/SpoiledPlugins/handlers.py
 Spoiled/SpoiledPlugins/help.py
 Spoiled/SpoiledPlugins/image.py
 Spoiled/SpoiledPlugins/inline.py
 Spoiled/SpoiledPlugins/leaderboard.py
 Spoiled/SpoiledPlugins/served.py
 Spoiled/SpoiledPlugins/start.py
 Spoiled/SpoiledPlugins/templates.py
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/Database/chats.py` & `SpLFastlyWrite-1.0.9/Spoiled/Database/chats.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from . import database
-
-db = database()
-
-chatsdb = db.chatsdb
-
-async def get_served_chats() -> list:
-    chats = chatsdb.find({"chat_id": {"$lt": 0}})
-    if not chats:
-        return []
-    chats_list = []
-    for chat in await chats.to_list(length=1000000000):
-        chats_list.append(chat["chat_id"])
-    return chats_list
-
-
-async def is_served_chat(chat_id: int) -> bool:
-    chat = await chatsdb.find_one({"chat_id": chat_id})
-    if not chat:
-        return False
-    return True
-
-
-async def add_served_chat(chat_id: int):
-    is_served = await is_served_chat(chat_id)
-    if is_served:
-        return
-    return await chatsdb.insert_one({"chat_id": chat_id})
-
-
-async def remove_served_chat(chat_id: int):
-    is_served = await is_served_chat(chat_id)
-    if not is_served:
-        return
-    return await chatsdb.delete_one({"chat_id": chat_id})
+from . import database
+
+db = database()
+
+chatsdb = db.chatsdb
+
+async def get_served_chats() -> list:
+    chats = chatsdb.find({"chat_id": {"$lt": 0}})
+    if not chats:
+        return []
+    chats_list = []
+    for chat in await chats.to_list(length=1000000000):
+        chats_list.append(chat["chat_id"])
+    return chats_list
+
+
+async def is_served_chat(chat_id: int) -> bool:
+    chat = await chatsdb.find_one({"chat_id": chat_id})
+    if not chat:
+        return False
+    return True
+
+
+async def add_served_chat(chat_id: int):
+    is_served = await is_served_chat(chat_id)
+    if is_served:
+        return
+    return await chatsdb.insert_one({"chat_id": chat_id})
+
+
+async def remove_served_chat(chat_id: int):
+    is_served = await is_served_chat(chat_id)
+    if not is_served:
+        return
+    return await chatsdb.delete_one({"chat_id": chat_id})
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/Database/coins.py` & `SpLFastlyWrite-1.0.9/Spoiled/Database/global_stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,63 @@
-from . import database
-
-db = database()
-
-cdb = db.coins
-
-async def add_coins(user_id: int, coins: int, chat_id: int):
-  chat_id = str(chat_id)
-  x = await cdb.find_one({"user_id": user_id})
-  if x:
-    dic = x['dic']
-  else:
-    dic = {}
-  if chat_id in dic:
-    dic[chat_id] += coins
-  else:
-    dic[chat_id] = coins
-  dic = await _get()
-  if str(user_id) in dic:
-    dic[str(user_id)] += coins
-  else:
-    dic[str(user_id)] = coins
-  await update(dic)
-  dic = await _get_chat()
-  if chat_id in dic:
-    dic[chat_id] += coins
-  else:
-    dic[chat_id] = coins
-  await update_chat(dic)
-  await cdb.update_one({"user_id": user_id}, {"$set": {"dic": dic}}, upsert=True)
-
-async def get_coins(user_id: int, chat_id: int = None):
-  if chat_id:
-    chat_id = str(chat_id)
-  x = await cdb.find_one({"user_id": user_id})
-  if x:
-    dic = x['dic']
-    if chat_id:
-      re = dic.get(chat_id, 0)
-      return re
-    tot = 0
-    for y in dic:
-      tot += dic[y]
-    return tot
-  return 0
-      
-
-ddb = db.coins_dict
-
-async def update(dic):
-    await ddb.update_one({"_": "_"}, {"$set": {"coins": dic}}, upsert=True)
-
-async def _get():
-    x = await ddb.find_one({"_": "_"})
-    if x:
-        return x["coins"]
-    return {}
-
-idb = db.coins_dict_chat
-
-async def update_chat(dic):
-    await idb.update_one({"_": "_"}, {"$set": {"coins": dic}}, upsert=True)
-
-async def _get_chat():
-    x = await idb.find_one({"_": "_"})
-    if x:
-        return x["coins"]
-    return {}
+from . import database
+
+db = database()
+
+gdb = db.global_chats
+
+async def incr_global_chat(chat_id: int):
+  chat_id = str(chat_id)
+  x = await gdb.find_one({"_": "_"})
+  if x:
+    dic = x['dic']
+  else:
+    dic = {}
+  if chat_id in dic:
+    dic[chat_id] += 1
+  else:
+    dic[chat_id] = 1
+  await gdb.update_one({"_": "_"}, {"$set": {"dic": dic}}, upsert=True)
+
+async def get_global_chat(chat_id: int):
+  chat_id = str(chat_id)
+  x = await gdb.find_one({"_": "_"})
+  if x:
+    dic = x['dic']
+    if chat_id in dic:
+      return dic[chat_id]
+    return 0
+
+async def get_chats_dic() -> dict:
+  x = await gdb.find_one({"_": "_"})
+  if x: 
+    return x['dic']
+  return {}
+
+udb = db.global_users
+
+async def incr_global_user(user_id: int):
+  user_id = str(user_id)
+  x = await udb.find_one({"_": "_"})
+  if x:
+    dic = x['dic']
+  else:
+    dic = {}
+  if user_id in dic:
+    dic[user_id] += 1
+  else:
+    dic[user_id] = 1
+  await udb.update_one({"_": "_"}, {"$set": {"dic": dic}}, upsert=True)
+
+async def get_global_user(user_id: int):
+  user_id = str(user_id)
+  x = await udb.find_one({"_": "_"})
+  if x:
+    dic = x['dic']
+    if user_id in dic:
+      return dic[user_id]
+    return 0
+
+async def get_users_dic() -> dict:
+  x = await udb.find_one({"_": "_"})
+  if x: 
+    return x['dic']
+  return {}
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/Database/users.py` & `SpLFastlyWrite-1.0.9/Spoiled/Database/users.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from . import database
-
-db = database()
-
-db = db.usersdb
-
-async def add_served_user(user_id: int):
-    x = await db.find_one({"user_id": user_id})
-    if not x:
-        return await db.insert_one({"user_id": user_id})
-
-async def rmv_served_user(user_id: int):
-    x = await db.find_one({"user_id": user_id})
-    if x:
-        return await db.delete_one({"user_id": user_id})
-
-async def get_served_users():
-    x = db.find({'user_id': {'$gt': 0}})
-    if not x:
-        return []
-    x = await x.to_list(length=1000000)
-    lis = []
-    for y in x:
-        lis.append(y['user_id'])
-    return lis
+from . import database
+
+db = database()
+
+db = db.usersdb
+
+async def add_served_user(user_id: int):
+    x = await db.find_one({"user_id": user_id})
+    if not x:
+        return await db.insert_one({"user_id": user_id})
+
+async def rmv_served_user(user_id: int):
+    x = await db.find_one({"user_id": user_id})
+    if x:
+        return await db.delete_one({"user_id": user_id})
+
+async def get_served_users():
+    x = db.find({'user_id': {'$gt': 0}})
+    if not x:
+        return []
+    x = await x.to_list(length=1000000)
+    lis = []
+    for y in x:
+        lis.append(y['user_id'])
+    return lis
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/Shannu/config.py` & `SpLFastlyWrite-1.0.9/Spoiled/Shannu/config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import os
-
-# DO NOT FILL ANYTHING HERE, FILL EVERYTHING IN ENVIRONMENT ITSELF !
-
-# mandatory vars
-BOT_TOKEN = os.getenv("BOT_TOKEN", None) # Get it from @BotFather [Telegram]
-MONGO_DB_URI = os.getenv("MONGO_DB_URI", None) # Get it from mongodb.com
-OWNER_ID = int(os.getenv("OWNER_ID", '')) # Get it from @SpL_Levi_Ackerman_Bot [Telegram]
-
-# non-mandatory vars
-API_ID = os.getenv("API_ID", None)
-API_HASH = os.getenv("API_HASH", None)
-BACKGROUND_IMAGE_URL = os.getenv("BACKGROUND_IMAGE_URL", None) # use Telegraph 
-WORD_SPAWN_TIME = os.getenv("WORD_SPAWN_TIME", None) # must be in seconds, Ex :- 900, Minimum :- 900
-SUPPORT_GROUP = os.getenv("SUPPORT_GROUP", None) # Ex :- 'Spoiled_Community' 
-SUPPORT_CHANNEL = os.getenv("SUPPORT_CHANNEL", None) # Ex :- 'SpLBots'
-
-# do not change code below
-if API_ID:
-  API_ID = int(API_ID)
-  
-if WORD_SPAWN_TIME:
-  try:
-    WORD_SPAWN_TIME = int(WORD_SPAWN_TIME)
-    if WORD_SPAWN_TIME < 900:
-      WORD_SPAWN_TIME = 900
-  except:
-    WORD_SPAWN_TIME = 900
-else:
-  WORD_SPAWN_TIME = 900
-
-if SUPPORT_GROUP:
-  if SUPPORT_GROUP[0] == '@':
-    SUPPORT_GROUP = SUPPORT_GROUP[1:]
-else:
-  SUPPORT_GROUP = 'Spoiled_Community'
-  
-if SUPPORT_CHANNEL:
-  if SUPPORT_CHANNEL[0] == '@':
-    SUPPORT_CHANNEL = SUPPORT_GROUP[1:]
-else:
-  SUPPORT_CHANNEL = 'SpLBots'
-
-if not BACKGROUND_IMAGE_URL:
-  print('Using Default Background Image...')
-  BACKGROUND_IMAGE_URL = 'https://telegra.ph/file/fe73eca247a491d4a6927.jpg'
+import os
+
+# DO NOT FILL ANYTHING HERE, FILL EVERYTHING IN ENVIRONMENT ITSELF !
+
+# mandatory vars
+BOT_TOKEN = os.getenv("BOT_TOKEN", None) # Get it from @BotFather [Telegram]
+MONGO_DB_URI = os.getenv("MONGO_DB_URI", None) # Get it from mongodb.com
+OWNER_ID = int(os.getenv("OWNER_ID", '')) # Get it from @SpL_Levi_Ackerman_Bot [Telegram]
+
+# non-mandatory vars
+API_ID = os.getenv("API_ID", None)
+API_HASH = os.getenv("API_HASH", None)
+BACKGROUND_IMAGE_URL = os.getenv("BACKGROUND_IMAGE_URL", None) # use Telegraph 
+WORD_SPAWN_TIME = os.getenv("WORD_SPAWN_TIME", None) # must be in seconds, Ex :- 900, Minimum :- 900
+SUPPORT_GROUP = os.getenv("SUPPORT_GROUP", None) # Ex :- 'Spoiled_Community' 
+SUPPORT_CHANNEL = os.getenv("SUPPORT_CHANNEL", None) # Ex :- 'SpLBots'
+
+# do not change code below
+if API_ID:
+  API_ID = int(API_ID)
+  
+if WORD_SPAWN_TIME:
+  try:
+    WORD_SPAWN_TIME = int(WORD_SPAWN_TIME)
+    if WORD_SPAWN_TIME < 900:
+      WORD_SPAWN_TIME = 900
+  except:
+    WORD_SPAWN_TIME = 900
+else:
+  WORD_SPAWN_TIME = 900
+
+if SUPPORT_GROUP:
+  if SUPPORT_GROUP[0] == '@':
+    SUPPORT_GROUP = SUPPORT_GROUP[1:]
+else:
+  SUPPORT_GROUP = 'Spoiled_Community'
+  
+if SUPPORT_CHANNEL:
+  if SUPPORT_CHANNEL[0] == '@':
+    SUPPORT_CHANNEL = SUPPORT_GROUP[1:]
+else:
+  SUPPORT_CHANNEL = 'SpLBots'
+
+if not BACKGROUND_IMAGE_URL:
+  print('Using Default Background Image...')
+  BACKGROUND_IMAGE_URL = 'https://telegra.ph/file/fe73eca247a491d4a6927.jpg'
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/callbacks.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/callbacks.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-from . import capsify, _sort, mention, title
-from .help import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
-from alphagram.types import IKM, IKB
-from alphagram import Alpha, filters
-from ..Database.privacy import *
-from ..Database.chats import get_served_chats
-from ..Database.users import get_served_users
-from ..Database.global_stats import get_users_dic, get_chats_dic
-from ..Database.chat_words import get_top_chat_users
-from ..Database.user_chat_info import get_user_info, get_chat_info
-from ..Database.coins import _get, _get_chat
-from .templates import info_template
-from Spoiled import CODE_OWNER_ID
-import asyncio
-
-@Alpha.on_callback_query(filters.regex('leaderboard'))
-async def leaderboard_cbq(_, q):
-  markup = IKM(
-    [
-      [
-        IKB(capsify('users'), callback_data='users'),
-        IKB(capsify('chats'), callback_data='chats')
-      ],
-      [
-        IKB(capsify("back"), callback_data="backtostart")
-      ]
-    ]
-  )
-  await q.answer()
-  await q.edit_message_text(capsify('» private accounts will be hidden.') + '\n\n' + capsify('choose from below !'), reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('help'))
-async def help_cbq(_, q):
-  txt = f'**{capsify("commands")}**\n\n'
-  txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
-  txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
-  txt += '\n'
-  txt += f'**{capsify("bot owner contact")}**\n\n'
-  group = capsify('group')
-  channel = capsify('channel')
-  txt += f'{group} : @{SUPPORT_GROUP}\n'
-  txt += f'{channel} : @{SUPPORT_CHANNEL}\n'
-  txt += '\n'
-  txt += f'**{capsify("code owner contact")}**\n\n'
-  txt += f'{group} : @Spoiled_Community\n'
-  txt += f'{channel} : @SpLBots\n'
-  markup = IKM(
-      [
-          [
-              IKB(capsify('bot owner'), user_id=OWNER_ID)
-          ],
-          [
-              IKB(capsify('code owner'), user_id=CODE_OWNER_ID)
-          ],
-          [
-              IKB(capsify('back'), callback_data='backtostart')
-          ]
-      ]
-  )
-  await q.answer()
-  await q.edit_message_text(txt, reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('info'))
-async def info_cbq(_, q):
-  chats, users = await asyncio.gather(get_served_chats(), get_served_users())
-  chats = str(len(chats))
-  users = str(len(users))
-  txt = info_template(chats, users)
-  markup = IKM(
-    [
-      [
-        IKB(capsify('owner'), user_id=CODE_OWNER_ID),
-        IKB(capsify('channel'), url='t.me/SpLBots')
-      ],
-      [
-        IKB(capsify('group'), url='t.me/Spoiled_Community'),
-        IKB(capsify('source'), url='github.com/ShutupKeshav/SpLFastlyWrite')
-      ],
-      [
-        IKB(capsify('back'), callback_data='backtostart')
-      ]
-    ]
-  )
-  await q.answer()
-  await q.edit_message_text(txt, reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('settings'))
-async def settings_cbq(_, q):
-  user_id = q.from_user.id
-  x = await get_private_users()
-  priv = True if user_id in x else False
-  enab = capsify("enabled 🔘") if priv else capsify("enabled")
-  disab = capsify("disabled") if priv else capsify("disabled 🔘")
-  markup = IKM(
-    [
-      [
-        IKB(capsify('privacy 🔒'), callback_data='privacy_answer')
-      ],
-      [
-        IKB(enab, callback_data='enable'),
-        IKB(disab, callback_data='disable')
-      ],
-      [
-        IKB(capsify('back'), callback_data='backtostart')
-      ]
-    ]
-  )
-  txt = capsify('⚙️ settings') + '\n\n'
-  txt += capsify('privacy enabled » your profile will be private.') + '\n'
-  txt += capsify('privacy disabled » your profile will be public.') + '\n\n'
-  txt += capsify('choose from below !')
-  await q.answer()
-  await q.edit_message_text(txt, reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('privacy_answer'))
-async def privacy_answer_cbq(_, q):
-  txt = 'use buttons below to toggle private mode !'
-  await q.answer(capsify(txt), show_alert=True)
-
-@Alpha.on_callback_query(filters.regex('users') | filters.regex('users_'))
-async def users(_, q):
-  if q.data == 'users':
-    x, dic = await asyncio.gather(get_private_users(), get_users_dic())
-    dic = _sort(dic)
-    a = 1
-    txt = capsify('top users by words') + "\n\n"
-    for y in dic:
-      y = int(y)
-      if y in x:
-        continue
-      txt += f'`{a}.` {await mention(y)} [`{dic[str(y)]}`]\n'
-      a += 1
-      if a >= 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('by coins'), callback_data='bycoinsusers')
-        ],
-        [
-          IKB(capsify('back'), callback_data='leaderboard')
-        ]
-      ]
-    )
-    await q.answer()
-    await q.edit_message_text(txt, reply_markup=markup)
-  else:
-    x, dic = await asyncio.gather(get_private_users(), _get())
-    dic = _sort(dic)
-    a = 1
-    txt = capsify('top users by coins') + '\n\n'
-    for y in dic:
-      y = int(y)
-      if y in x:
-        continue
-      txt += f'`{a}.` {await mention(y)} [`{dic[str(y)]}`]\n'
-      a += 1
-      if a >= 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('by words'), callback_data='users')
-        ],
-        [
-          IKB(capsify('back'), callback_data='leaderboard')
-        ]
-      ]
-    )
-    await q.answer()
-    await q.edit_message_text(txt, reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('chats') | filters.regex('chats_'))
-async def chats(_, q):
-  if q.data == 'chats':
-    dic = await get_chats_dic()
-    dic = _sort(dic)
-    a = 1
-    txt = capsify('top chats by words') + "\n\n"
-    for y in dic:
-      y = int(y)
-      txt += f'`{a}.` {(await title(y))[:25]} [`{dic[str(y)]}`]\n'
-      a += 1
-      if a >= 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('by coins'), callback_data='chats_')
-        ],
-        [
-          IKB(capsify('back'), callback_data='leaderboard')
-        ]
-      ]
-    )
-    await q.answer()
-    await q.edit_message_text(txt, reply_markup=markup)
-  else:
-    dic = await _get_chat()
-    dic = _sort(dic)
-    a = 1
-    txt = capsify('top chats by coins') + '\n\n'
-    for y in dic:
-      y = int(y)
-      txt += f'`{a}.` {(await title(y))[:25]} [`{dic[str(y)]}`]\n'
-      a += 1
-      if a >= 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('by words'), callback_data='chats')
-        ],
-        [
-          IKB(capsify('back'), callback_data='leaderboard')
-        ]
-      ]
-    )
-    await q.answer()
-    await q.edit_message_text(txt, reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('enable') | filters.regex('disable'))
-async def enab_priv(_, q):
-  user_id = q.from_user.id
-  data = q.data
-  x = await get_private_users()
-  if q.data == 'enable':
-    if user_id in x:
-      return await q.answer(capsify('private mode is already enabled !'), show_alert=True)
-    await enable_privacy(user_id)
-    priv = True
-  else:
-    if not user_id in x:
-      return await q.answer(capsify('private mode is already disabled !'), show_alert=True)
-    await disable_privacy(user_id)
-    priv = False
-  enab = capsify("enabled 🔘") if priv else capsify("enabled")
-  disab = capsify("disabled") if priv else capsify("disabled 🔘")
-  markup = IKM(
-    [
-      [
-        IKB(capsify('privacy 🔒'), callback_data='privacy_answer')
-      ],
-      [
-        IKB(enab, callback_data='enable'),
-        IKB(disab, callback_data='disable')
-      ],
-      [
-        IKB(capsify('back'), callback_data='backtostart')
-      ]
-    ]
-  )
-  await q.answer()
-  await q.edit_message_reply_markup(reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('topby_'))
-async def topby(_, q):
-  data = q.data.split('_')[1]
-  await q.answer()
-  if data == 'coins':
-    await q.edit_message_text(capsify('sorting top by coins, please wait...'))
-    get = await _get()
-    sor = _sort(get)
-    chat_mem = []
-    async for x in _.get_chat_members(q.message.chat.id):
-      if not x.user.is_bot and not x.user.is_deleted:
-        chat_mem.append(x.user.id)
-    txt = capsify('top coins holders in {}') + '\n\n'
-    txt = txt.format(q.message.chat.title)
-    a = 1
-    for y in sor:
-      y = int(y)
-      if not y in chat_mem:
-        continue
-      txt += f'`{a}.` {await mention(y)} [{sor[str(y)]}]\n'
-      a += 1
-      if a == 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('top by words'), callback_data='topby_words')
-        ]
-      ]
-    )
-    await q.edit_message_text(txt, reply_markup=markup)
-  else:
-    await q.edit_message_text(capsify('sorting top by words, please wait...'))
-    chat_id = q.message.chat.id
-    chat_title = q.message.chat.title
-    x = await get_top_chat_users(chat_id)
-    txt = capsify('top word completers in {}') + '\n\n'
-    txt = txt.format(chat_title)
-    a = 1
-    for y in x:
-      txt += f'`{a}.` {await mention(int(y))} [{x[y]}]\n'
-      a += 1
-      if a == 11:
-        break
-    markup = IKM(
-      [
-        [
-          IKB(capsify('top by coins'), callback_data='topby_coins')
-        ]
-      ]
-    )
-    await q.edit_message_text(txt, reply_markup=markup)
+from . import capsify, _sort, mention, title
+from .help import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
+from alphagram.types import IKM, IKB
+from alphagram import Alpha, filters
+from ..Database.privacy import *
+from ..Database.chats import get_served_chats
+from ..Database.users import get_served_users
+from ..Database.global_stats import get_users_dic, get_chats_dic
+from ..Database.chat_words import get_top_chat_users
+from ..Database.user_chat_info import get_user_info, get_chat_info
+from ..Database.coins import _get, _get_chat
+from .templates import info_template
+from Spoiled import CODE_OWNER_ID
+import asyncio
+
+@Alpha.on_callback_query(filters.regex('leaderboard'))
+async def leaderboard_cbq(_, q):
+  markup = IKM(
+    [
+      [
+        IKB(capsify('users'), callback_data='users'),
+        IKB(capsify('chats'), callback_data='chats')
+      ],
+      [
+        IKB(capsify("back"), callback_data="backtostart")
+      ]
+    ]
+  )
+  await q.answer()
+  await q.edit_message_text(capsify('» private accounts will be hidden.') + '\n\n' + capsify('choose from below !'), reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('help'))
+async def help_cbq(_, q):
+  txt = f'**{capsify("commands")}**\n\n'
+  txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
+  txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
+  txt += '\n'
+  txt += f'**{capsify("bot owner contact")}**\n\n'
+  group = capsify('group')
+  channel = capsify('channel')
+  txt += f'{group} : @{SUPPORT_GROUP}\n'
+  txt += f'{channel} : @{SUPPORT_CHANNEL}\n'
+  txt += '\n'
+  txt += f'**{capsify("code owner contact")}**\n\n'
+  txt += f'{group} : @Spoiled_Community\n'
+  txt += f'{channel} : @SpLBots\n'
+  markup = IKM(
+      [
+          [
+              IKB(capsify('bot owner'), user_id=OWNER_ID)
+          ],
+          [
+              IKB(capsify('code owner'), user_id=CODE_OWNER_ID)
+          ],
+          [
+              IKB(capsify('back'), callback_data='backtostart')
+          ]
+      ]
+  )
+  await q.answer()
+  await q.edit_message_text(txt, reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('info'))
+async def info_cbq(_, q):
+  chats, users = await asyncio.gather(get_served_chats(), get_served_users())
+  chats = str(len(chats))
+  users = str(len(users))
+  txt = info_template(chats, users)
+  markup = IKM(
+    [
+      [
+        IKB(capsify('owner'), user_id=CODE_OWNER_ID),
+        IKB(capsify('channel'), url='t.me/SpLBots')
+      ],
+      [
+        IKB(capsify('group'), url='t.me/Spoiled_Community'),
+        IKB(capsify('source'), url='github.com/ShutupKeshav/SpLFastlyWrite')
+      ],
+      [
+        IKB(capsify('back'), callback_data='backtostart')
+      ]
+    ]
+  )
+  await q.answer()
+  await q.edit_message_text(txt, reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('settings'))
+async def settings_cbq(_, q):
+  user_id = q.from_user.id
+  x = await get_private_users()
+  priv = True if user_id in x else False
+  enab = capsify("enabled 🔘") if priv else capsify("enabled")
+  disab = capsify("disabled") if priv else capsify("disabled 🔘")
+  markup = IKM(
+    [
+      [
+        IKB(capsify('privacy 🔒'), callback_data='privacy_answer')
+      ],
+      [
+        IKB(enab, callback_data='enable'),
+        IKB(disab, callback_data='disable')
+      ],
+      [
+        IKB(capsify('back'), callback_data='backtostart')
+      ]
+    ]
+  )
+  txt = capsify('⚙️ settings') + '\n\n'
+  txt += capsify('privacy enabled » your profile will be private.') + '\n'
+  txt += capsify('privacy disabled » your profile will be public.') + '\n\n'
+  txt += capsify('choose from below !')
+  await q.answer()
+  await q.edit_message_text(txt, reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('privacy_answer'))
+async def privacy_answer_cbq(_, q):
+  txt = 'use buttons below to toggle private mode !'
+  await q.answer(capsify(txt), show_alert=True)
+
+@Alpha.on_callback_query(filters.regex('users') | filters.regex('users_'))
+async def users(_, q):
+  if q.data == 'users':
+    x, dic = await asyncio.gather(get_private_users(), get_users_dic())
+    dic = _sort(dic)
+    a = 1
+    txt = capsify('top users by words') + "\n\n"
+    for y in dic:
+      y = int(y)
+      if y in x:
+        continue
+      txt += f'`{a}.` {await mention(y)} [`{dic[str(y)]}`]\n'
+      a += 1
+      if a >= 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('by coins'), callback_data='bycoinsusers')
+        ],
+        [
+          IKB(capsify('back'), callback_data='leaderboard')
+        ]
+      ]
+    )
+    await q.answer()
+    await q.edit_message_text(txt, reply_markup=markup)
+  else:
+    x, dic = await asyncio.gather(get_private_users(), _get())
+    dic = _sort(dic)
+    a = 1
+    txt = capsify('top users by coins') + '\n\n'
+    for y in dic:
+      y = int(y)
+      if y in x:
+        continue
+      txt += f'`{a}.` {await mention(y)} [`{dic[str(y)]}`]\n'
+      a += 1
+      if a >= 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('by words'), callback_data='users')
+        ],
+        [
+          IKB(capsify('back'), callback_data='leaderboard')
+        ]
+      ]
+    )
+    await q.answer()
+    await q.edit_message_text(txt, reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('chats') | filters.regex('chats_'))
+async def chats(_, q):
+  if q.data == 'chats':
+    dic = await get_chats_dic()
+    dic = _sort(dic)
+    a = 1
+    txt = capsify('top chats by words') + "\n\n"
+    for y in dic:
+      y = int(y)
+      txt += f'`{a}.` {(await title(y))[:25]} [`{dic[str(y)]}`]\n'
+      a += 1
+      if a >= 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('by coins'), callback_data='chats_')
+        ],
+        [
+          IKB(capsify('back'), callback_data='leaderboard')
+        ]
+      ]
+    )
+    await q.answer()
+    await q.edit_message_text(txt, reply_markup=markup)
+  else:
+    dic = await _get_chat()
+    dic = _sort(dic)
+    a = 1
+    txt = capsify('top chats by coins') + '\n\n'
+    for y in dic:
+      y = int(y)
+      txt += f'`{a}.` {(await title(y))[:25]} [`{dic[str(y)]}`]\n'
+      a += 1
+      if a >= 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('by words'), callback_data='chats')
+        ],
+        [
+          IKB(capsify('back'), callback_data='leaderboard')
+        ]
+      ]
+    )
+    await q.answer()
+    await q.edit_message_text(txt, reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('enable') | filters.regex('disable'))
+async def enab_priv(_, q):
+  user_id = q.from_user.id
+  data = q.data
+  x = await get_private_users()
+  if q.data == 'enable':
+    if user_id in x:
+      return await q.answer(capsify('private mode is already enabled !'), show_alert=True)
+    await enable_privacy(user_id)
+    priv = True
+  else:
+    if not user_id in x:
+      return await q.answer(capsify('private mode is already disabled !'), show_alert=True)
+    await disable_privacy(user_id)
+    priv = False
+  enab = capsify("enabled 🔘") if priv else capsify("enabled")
+  disab = capsify("disabled") if priv else capsify("disabled 🔘")
+  markup = IKM(
+    [
+      [
+        IKB(capsify('privacy 🔒'), callback_data='privacy_answer')
+      ],
+      [
+        IKB(enab, callback_data='enable'),
+        IKB(disab, callback_data='disable')
+      ],
+      [
+        IKB(capsify('back'), callback_data='backtostart')
+      ]
+    ]
+  )
+  await q.answer()
+  await q.edit_message_reply_markup(reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('topby_'))
+async def topby(_, q):
+  data = q.data.split('_')[1]
+  await q.answer()
+  if data == 'coins':
+    await q.edit_message_text(capsify('sorting top by coins, please wait...'))
+    get = await _get()
+    sor = _sort(get)
+    chat_mem = []
+    async for x in _.get_chat_members(q.message.chat.id):
+      if not x.user.is_bot and not x.user.is_deleted:
+        chat_mem.append(x.user.id)
+    txt = capsify('top coins holders in {}') + '\n\n'
+    txt = txt.format(q.message.chat.title)
+    a = 1
+    for y in sor:
+      y = int(y)
+      if not y in chat_mem:
+        continue
+      txt += f'`{a}.` {await mention(y)} [{sor[str(y)]}]\n'
+      a += 1
+      if a == 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('top by words'), callback_data='topby_words')
+        ]
+      ]
+    )
+    await q.edit_message_text(txt, reply_markup=markup)
+  else:
+    await q.edit_message_text(capsify('sorting top by words, please wait...'))
+    chat_id = q.message.chat.id
+    chat_title = q.message.chat.title
+    x = await get_top_chat_users(chat_id)
+    txt = capsify('top word completers in {}') + '\n\n'
+    txt = txt.format(chat_title)
+    a = 1
+    for y in x:
+      txt += f'`{a}.` {await mention(int(y))} [{x[y]}]\n'
+      a += 1
+      if a == 11:
+        break
+    markup = IKM(
+      [
+        [
+          IKB(capsify('top by coins'), callback_data='topby_coins')
+        ]
+      ]
+    )
+    await q.edit_message_text(txt, reply_markup=markup)
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/coins.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/coins.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from alphagram import Alpha, filters
-from ..Database.coins import get_coins
-from . import capsify
-
-@Alpha.on_message(filters.command('coins') & filters.group)
-async def coins(_, m):
-  user_id = m.from_user.id
-  chat_id = m.chat.id
-  title = m.chat.title
-  this_coins = await get_coins(user_id, chat_id=chat_id)
-  global_coins = await get_coins(user_id)
-  txt = capsify("coins in") + '\n\n'
-  txt += f'{title} : `{this_coins}`\n'
-  txt += f'{capsify("global")} : `{global_coins}`'
-  await m.reply(txt)
-                      
+from alphagram import Alpha, filters
+from ..Database.coins import get_coins
+from . import capsify
+
+@Alpha.on_message(filters.command('coins') & filters.group)
+async def coins(_, m):
+  user_id = m.from_user.id
+  chat_id = m.chat.id
+  title = m.chat.title
+  this_coins = await get_coins(user_id, chat_id=chat_id)
+  global_coins = await get_coins(user_id)
+  txt = capsify("coins in") + '\n\n'
+  txt += f'{title} : `{this_coins}`\n'
+  txt += f'{capsify("global")} : `{global_coins}`'
+  await m.reply(txt)
+
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/help.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/help.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from alphagram import Alpha, filters
-from config import OWNER_ID, SUPPORT_GROUP, SUPPORT_CHANNEL
-from Spoiled import CODE_OWNER_ID
-from . import capsify
-from alphagram.types import IKM, IKB
-
-@Alpha.on_message(filters.command('help') & filters.private)
-async def help(_, m):
-  txt = f'**{capsify("commands")}**\n\n'
-  txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
-  txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
-  txt += '\n'
-  txt += f'**{capsify("bot owner contact")}**\n\n'
-  group = capsify('group')
-  channel = capsify('channel')
-  txt += f'{group} : @{SUPPORT_GROUP}\n'
-  txt += f'{channel} : @{SUPPORT_CHANNEL}\n'
-  txt += '\n'
-  txt += f'**{capsify("code owner contact")}**\n\n'
-  txt += f'{group} : @Spoiled_Community\n'
-  txt += f'{channel} : @SpLBots\n'
-  markup = IKM(
-      [
-          [
-              IKB(capsify('bot owner'), user_id=OWNER_ID)
-          ],
-          [
-              IKB(capsify('code owner'), user_id=CODE_OWNER_ID)
-          ]
-      ]
-  )
-  await m.reply(txt, reply_markup=markup)
+from alphagram import Alpha, filters
+from config import OWNER_ID, SUPPORT_GROUP, SUPPORT_CHANNEL
+from Spoiled import CODE_OWNER_ID
+from . import capsify
+from alphagram.types import IKM, IKB
+
+@Alpha.on_message(filters.command('help') & filters.private)
+async def help(_, m):
+  txt = f'**{capsify("commands")}**\n\n'
+  txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
+  txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
+  txt += '\n'
+  txt += f'**{capsify("bot owner contact")}**\n\n'
+  group = capsify('group')
+  channel = capsify('channel')
+  txt += f'{group} : @{SUPPORT_GROUP}\n'
+  txt += f'{channel} : @{SUPPORT_CHANNEL}\n'
+  txt += '\n'
+  txt += f'**{capsify("code owner contact")}**\n\n'
+  txt += f'{group} : @Spoiled_Community\n'
+  txt += f'{channel} : @SpLBots\n'
+  markup = IKM(
+      [
+          [
+              IKB(capsify('bot owner'), user_id=OWNER_ID)
+          ],
+          [
+              IKB(capsify('code owner'), user_id=CODE_OWNER_ID)
+          ]
+      ]
+  )
+  await m.reply(txt, reply_markup=markup)
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/image.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/image.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from PIL import Image, ImageDraw, ImageFont
-import glob
-import requests
-import os
-from Spoiled.Shannu.config import BACKGROUND_IMAGE_URL as BIU
-
-def init_bg():
-  g = requests.get(BIU)
-  try:
-    os.mkdir("Images")
-  except:
-    pass
-  with open("Images/bg.jpg", "wb") as f:
-    f.write(g.content)
-
-def make_image(text, username):
-  text = text.capitalize()
-  username = 'by @' + username
-  x = './Images/bg.jpg'
-  f = './Fonts/font.ttf'
-  im = glob.glob('./saved_images/*')
-  if f'{text}.jpg' in im:
-    return f'saved_images/{text}.jpg'
-  i = Image.open(x)
-  wi, he = i.size
-  d = ImageDraw.Draw(i)
-  font = ImageFont.truetype(f, 120)
-  font1 = ImageFont.truetype(f, 60)
-  w, h = d.textsize(text, font)
-  new_w = (wi - w) / 2
-  new_h = (he - h) / 2
-  d.text((new_w, new_h), text, fill="black", font=font)
-  d.text((5, 5), username, fill="black", font=font1)
-  i.save(f'saved_images/{text}.jpg')
-  return f'saved_images/{text}.jpg'
+from PIL import Image, ImageDraw, ImageFont
+import glob
+import requests
+import os
+from Spoiled.Shannu.config import BACKGROUND_IMAGE_URL as BIU
+
+def init_bg():
+  g = requests.get(BIU)
+  try:
+    os.mkdir("Images")
+  except:
+    pass
+  with open("Images/bg.jpg", "wb") as f:
+    f.write(g.content)
+
+def make_image(text, username):
+  text = text.capitalize()
+  username = 'by @' + username
+  x = './Images/bg.jpg'
+  f = './Fonts/font.ttf'
+  im = glob.glob('./saved_images/*')
+  if f'{text}.jpg' in im:
+    return f'saved_images/{text}.jpg'
+  i = Image.open(x)
+  wi, he = i.size
+  d = ImageDraw.Draw(i)
+  font = ImageFont.truetype(f, 120)
+  font1 = ImageFont.truetype(f, 60)
+  w, h = d.textsize(text, font)
+  new_w = (wi - w) / 2
+  new_h = (he - h) / 2
+  d.text((new_w, new_h), text, fill="black", font=font)
+  d.text((5, 5), username, fill="black", font=font1)
+  i.save(f'saved_images/{text}.jpg')
+  return f'saved_images/{text}.jpg'
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/leaderboard.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/leaderboard.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from alphagram import Alpha, filters
-from ..Database.chat_words import get_top_chat_users
-from alphagram.types import IKM, IKB
-from . import capsify, mention, title
-
-@Alpha.on_message(filters.command('leaderboard') & filters.group)
-async def leaderboard(_, m):
-  ok = await m.reply(capsify('getting leaderboard...'))
-  chat_id = m.chat.id
-  chat_title = m.chat.title
-  x = await get_top_chat_users(chat_id)
-  txt = capsify('top word completers in {}') + '\n\n'
-  txt = txt.format(chat_title)
-  a = 1
-  for y in x:
-    txt += f'`{a}.` {await mention(int(y))} [{x[y]}]\n'
-    a += 1
-    if a == 11:
-      break
-  markup = IKM(
-    [
-      [
-        IKB(capsify('top by coins'), callback_data='topby_coins')
-      ]
-    ]
-  )
-  await ok.edit(txt, reply_markup=markup)
-    
+from alphagram import Alpha, filters
+from ..Database.chat_words import get_top_chat_users
+from alphagram.types import IKM, IKB
+from . import capsify, mention, title
+
+@Alpha.on_message(filters.command('leaderboard') & filters.group)
+async def leaderboard(_, m):
+  ok = await m.reply(capsify('getting leaderboard...'))
+  chat_id = m.chat.id
+  chat_title = m.chat.title
+  x = await get_top_chat_users(chat_id)
+  txt = capsify('top word completers in {}') + '\n\n'
+  txt = txt.format(chat_title)
+  a = 1
+  for y in x:
+    txt += f'`{a}.` {await mention(int(y))} [{x[y]}]\n'
+    a += 1
+    if a == 11:
+      break
+  markup = IKM(
+    [
+      [
+        IKB(capsify('top by coins'), callback_data='topby_coins')
+      ]
+    ]
+  )
+  await ok.edit(txt, reply_markup=markup)
+
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/served.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/served.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from .watchers import served_watcher
-from alphagram import Alpha, filters
-from ..Database.chats import add_served_chat
-from ..Database.users import add_served_user
-from ..Database.user_chat_info import update_chat_info, update_user_info
-
-@Alpha.on_message(group=served_watcher)
-async def cwf(_, m):
-  if m.from_user:
-    await add_served_user(m.from_user.id)
-    details = {}
-    details["first_name"] = m.from_user.first_name
-    details["last_name"] = m.from_user.last_name if m.from_user.last_name else None
-    details["username"] = m.from_user.username if m.from_user.username else None
-    await update_user_info(m.from_user.id, details)
-  if m.chat.id < 0:
-    await add_served_chat(m.chat.id)
-    chat_details = {}
-    chat_details["title"] = m.chat.title
-    await update_chat_info(m.chat.id, chat_details)
+from .watchers import served_watcher
+from alphagram import Alpha, filters
+from ..Database.chats import add_served_chat
+from ..Database.users import add_served_user
+from ..Database.user_chat_info import update_chat_info, update_user_info
+
+@Alpha.on_message(group=served_watcher)
+async def cwf(_, m):
+  if m.from_user:
+    await add_served_user(m.from_user.id)
+    details = {}
+    details["first_name"] = m.from_user.first_name
+    details["last_name"] = m.from_user.last_name if m.from_user.last_name else None
+    details["username"] = m.from_user.username if m.from_user.username else None
+    await update_user_info(m.from_user.id, details)
+  if m.chat.id < 0:
+    await add_served_chat(m.chat.id)
+    chat_details = {}
+    chat_details["title"] = m.chat.title
+    await update_chat_info(m.chat.id, chat_details)
```

### Comparing `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/start.py` & `SpLFastlyWrite-1.0.9/Spoiled/SpoiledPlugins/start.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from alphagram import Alpha, filters
-from alphagram.types import IKM, IKB
-from config import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
-from Spoiled.Database.users import add_served_user
-from Spoiled.Database.coins import get_coins
-from Spoiled.Database.completed import get_top_chat, get_completed_words
-from Spoiled.Database.record import get_record
-from . import capsify, get_readable_time, title
-from Spoiled.Shannu.alpha import alpha
-import asyncio
-
-@Alpha.on_message(filters.command('start') & filters.private)
-async def start(_, m):
-  await add_served_user(m.from_user.id)
-  txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
-  id = _.me.id
-  un = _.me.username
-  fn = _.me.first_name
-  user_first_name = m.from_user.first_name
-  markup = IKM(
-      [
-          [
-              IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
-          ],
-          [
-              IKB(capsify("Help 📘"), callback_data='help'),
-              IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
-          ],
-          [
-              IKB(capsify("Profile 👤"), callback_data='profile'),
-              IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
-          ],
-          [
-              IKB(capsify("Info ℹ️"), callback_data='info'),
-              IKB(capsify("Settings ⚙️"), callback_data='settings')
-          ]
-      ]
-  )
-  await m.reply(txt.format(user_first_name, fn), reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('backtostart'))
-async def backtostart(_, q):
-  txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
-  id = _.me.id
-  un = _.me.username
-  fn = _.me.first_name
-  user_first_name = q.from_user.first_name
-  markup = IKM(
-      [
-          [
-              IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
-          ],
-          [
-              IKB(capsify("Help 📘"), callback_data='help'),
-              IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
-          ],
-          [
-              IKB(capsify("Profile 👤"), callback_data='profile'),
-              IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
-          ],
-          [
-              IKB(capsify("Info ℹ️"), callback_data='info'),
-              IKB(capsify("Settings ⚙️"), callback_data='settings')
-          ]
-      ]
-  )
-  await q.answer()
-  await q.edit_message_text(txt.format(user_first_name, fn), reply_markup=markup)
-
-@Alpha.on_callback_query(filters.regex('profile'))
-async def profile_cbq(_, q):
-  await q.answer()
-  await q.edit_message_text(capsify('getting your profile, please wait...'))
-  user_id = q.from_user.id
-  cns, words, top_chat, record = await asyncio.gather(
-    get_coins(user_id),
-    get_completed_words(user_id),
-    get_top_chat(user_id),
-    get_record(user_id)
-  )
-  txt = capsify('👤 User Profile')
-  txt += '\n\n'
-  txt += capsify('words completed :') + f' `{words}`.'
-  txt += '\n'
-  txt += capsify('coins :') + f' `{cns}`.'
-  if top_chat:
-    top_chat = await title(int(top_chat))
-  txt += '\n'
-  txt += capsify('top chat :') + f' {top_chat}.'
-  txt += '\n'
-  txt += capsify('record :') + f' `{get_readable_time(int(record))}.`'
-  markup = IKM(
-    [
-      [
-        IKB(capsify("share profile"), switch_inline_query='share')
-      ],
-      [
-        IKB(capsify('back'), callback_data='backtostart')
-      ]
-    ]
-  )
-  await q.edit_message_text(txt, reply_markup=markup)
+from alphagram import Alpha, filters
+from alphagram.types import IKM, IKB
+from config import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
+from Spoiled.Database.users import add_served_user
+from Spoiled.Database.coins import get_coins
+from Spoiled.Database.completed import get_top_chat, get_completed_words
+from Spoiled.Database.record import get_record
+from . import capsify, get_readable_time, title
+from Spoiled import alpha
+import asyncio
+
+@Alpha.on_message(filters.command('start') & filters.private)
+async def start(_, m):
+  await add_served_user(m.from_user.id)
+  txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
+  id = _.me.id
+  un = _.me.username
+  fn = _.me.first_name
+  user_first_name = m.from_user.first_name
+  markup = IKM(
+      [
+          [
+              IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
+          ],
+          [
+              IKB(capsify("Help 📘"), callback_data='help'),
+              IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
+          ],
+          [
+              IKB(capsify("Profile 👤"), callback_data='profile'),
+              IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
+          ],
+          [
+              IKB(capsify("Info ℹ️"), callback_data='info'),
+              IKB(capsify("Settings ⚙️"), callback_data='settings')
+          ]
+      ]
+  )
+  await m.reply(txt.format(user_first_name, fn), reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('backtostart'))
+async def backtostart(_, q):
+  txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
+  id = _.me.id
+  un = _.me.username
+  fn = _.me.first_name
+  user_first_name = q.from_user.first_name
+  markup = IKM(
+      [
+          [
+              IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
+          ],
+          [
+              IKB(capsify("Help 📘"), callback_data='help'),
+              IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
+          ],
+          [
+              IKB(capsify("Profile 👤"), callback_data='profile'),
+              IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
+          ],
+          [
+              IKB(capsify("Info ℹ️"), callback_data='info'),
+              IKB(capsify("Settings ⚙️"), callback_data='settings')
+          ]
+      ]
+  )
+  await q.answer()
+  await q.edit_message_text(txt.format(user_first_name, fn), reply_markup=markup)
+
+@Alpha.on_callback_query(filters.regex('profile'))
+async def profile_cbq(_, q):
+  await q.answer()
+  await q.edit_message_text(capsify('getting your profile, please wait...'))
+  user_id = q.from_user.id
+  cns, words, top_chat, record = await asyncio.gather(
+    get_coins(user_id),
+    get_completed_words(user_id),
+    get_top_chat(user_id),
+    get_record(user_id)
+  )
+  txt = capsify('👤 User Profile')
+  txt += '\n\n'
+  txt += capsify('words completed :') + f' `{words}`.'
+  txt += '\n'
+  txt += capsify('coins :') + f' `{cns}`.'
+  if top_chat:
+    top_chat = await title(int(top_chat))
+  txt += '\n'
+  txt += capsify('top chat :') + f' {top_chat}.'
+  txt += '\n'
+  txt += capsify('record :') + f' `{get_readable_time(int(record))}.`'
+  markup = IKM(
+    [
+      [
+        IKB(capsify("share profile"), switch_inline_query='share')
+      ],
+      [
+        IKB(capsify('back'), callback_data='backtostart')
+      ]
+    ]
+  )
+  await q.edit_message_text(txt, reply_markup=markup)
```

### Comparing `SpLFastlyWrite-1.0.8/setup.py` & `SpLFastlyWrite-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup, Extension, find_packages
-
-with open("README.md", encoding="utf-8") as f:
-    readme = f.read()
-
-setup(
-    name="SpLFastlyWrite",
-    version="1.0.8",
-    description="SpLFastlyWrite",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    url="https://github.com/ShutupKeshav/SpLFastlyWrite",
-    download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
-    author="ShutupKeshav",
-    author_email="keshavatripathi@yahoo.com",
-    license="MIT",
-    keywords="SpLFastlyWrite",
-    project_urls={
-        "Tracker": "https://github.com/ShutupKeshav/SpLFastlyWrite/issues",
-        "Community": "https://t.me/SpLBots",
-        "Source": "https://github.com/ShutupKeshav/SpLFastlyWrite",
-        "Documentation": "https://t.me/SpLBots",
-    },
-    python_requires="~=3.7",
-    packages=find_packages(),
-    test_suite="tests",
-    zip_safe=False
-)
-
-print("SpLFastlyWrite BY SpL Network !")
+from setuptools import setup, Extension, find_packages
+
+with open("README.md", encoding="utf-8") as f:
+    readme = f.read()
+
+setup(
+    name="SpLFastlyWrite",
+    version="1.0.9",
+    description="SpLFastlyWrite",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url="https://github.com/ShutupKeshav/SpLFastlyWrite",
+    download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
+    author="ShutupKeshav",
+    author_email="keshavatripathi@yahoo.com",
+    license="MIT",
+    keywords="SpLFastlyWrite",
+    project_urls={
+        "Tracker": "https://github.com/ShutupKeshav/SpLFastlyWrite/issues",
+        "Community": "https://t.me/SpLBots",
+        "Source": "https://github.com/ShutupKeshav/SpLFastlyWrite",
+        "Documentation": "https://t.me/SpLBots",
+    },
+    python_requires="~=3.7",
+    packages=find_packages(),
+    test_suite="tests",
+    zip_safe=False
+)
+
+print("SpLFastlyWrite BY SpL Network !")
```

