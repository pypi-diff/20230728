# Comparing `tmp/chatterstack-2.0.0.tar.gz` & `tmp/chatterstack-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatterstack-2.0.0.tar", last modified: Thu Jul 20 05:16:23 2023, max compression
+gzip compressed data, was "chatterstack-2.0.1.tar", last modified: Fri Jul 28 17:07:03 2023, max compression
```

## Comparing `chatterstack-2.0.0.tar` & `chatterstack-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-20 05:16:23.970864 chatterstack-2.0.0/
--rw-r--r--   0 davidschiller   (501) staff       (20)    13878 2023-07-20 05:16:23.970689 chatterstack-2.0.0/PKG-INFO
--rw-r--r--   0 davidschiller   (501) staff       (20)    13146 2023-07-20 05:05:46.000000 chatterstack-2.0.0/README.md
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-20 05:16:23.969857 chatterstack-2.0.0/chatterstack/
--rw-r--r--   0 davidschiller   (501) staff       (20)      378 2023-07-20 04:55:22.000000 chatterstack-2.0.0/chatterstack/__init__.py
--rw-r--r--   0 davidschiller   (501) staff       (20)    12696 2023-07-20 04:54:24.000000 chatterstack-2.0.0/chatterstack/chatterstack.py
--rw-r--r--   0 davidschiller   (501) staff       (20)    12120 2023-07-20 04:54:54.000000 chatterstack-2.0.0/chatterstack/chatterstackadvanced.py
--rw-r--r--   0 davidschiller   (501) staff       (20)     2136 2023-07-20 04:55:47.000000 chatterstack-2.0.0/chatterstack/commands.py
-drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-20 05:16:23.970506 chatterstack-2.0.0/chatterstack.egg-info/
--rw-r--r--   0 davidschiller   (501) staff       (20)    13878 2023-07-20 05:16:23.000000 chatterstack-2.0.0/chatterstack.egg-info/PKG-INFO
--rw-r--r--   0 davidschiller   (501) staff       (20)      313 2023-07-20 05:16:23.000000 chatterstack-2.0.0/chatterstack.egg-info/SOURCES.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)        1 2023-07-20 05:16:23.000000 chatterstack-2.0.0/chatterstack.egg-info/dependency_links.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)        7 2023-07-20 05:16:23.000000 chatterstack-2.0.0/chatterstack.egg-info/requires.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)       13 2023-07-20 05:16:23.000000 chatterstack-2.0.0/chatterstack.egg-info/top_level.txt
--rw-r--r--   0 davidschiller   (501) staff       (20)       38 2023-07-20 05:16:23.970907 chatterstack-2.0.0/setup.cfg
--rw-r--r--   0 davidschiller   (501) staff       (20)      949 2023-07-20 04:41:58.000000 chatterstack-2.0.0/setup.py
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-28 17:07:03.890117 chatterstack-2.0.1/
+-rw-r--r--   0 davidschiller   (501) staff       (20)    14067 2023-07-28 17:07:03.889931 chatterstack-2.0.1/PKG-INFO
+-rw-r--r--   0 davidschiller   (501) staff       (20)    13335 2023-07-27 19:05:39.000000 chatterstack-2.0.1/README.md
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-28 17:07:03.889028 chatterstack-2.0.1/chatterstack/
+-rw-r--r--   0 davidschiller   (501) staff       (20)      378 2023-07-20 04:55:22.000000 chatterstack-2.0.1/chatterstack/__init__.py
+-rw-r--r--   0 davidschiller   (501) staff       (20)    12696 2023-07-20 04:54:24.000000 chatterstack-2.0.1/chatterstack/chatterstack.py
+-rw-r--r--   0 davidschiller   (501) staff       (20)    12146 2023-07-28 17:00:48.000000 chatterstack-2.0.1/chatterstack/chatterstackadvanced.py
+-rw-r--r--   0 davidschiller   (501) staff       (20)     2136 2023-07-20 04:55:47.000000 chatterstack-2.0.1/chatterstack/commands.py
+drwxr-xr-x   0 davidschiller   (501) staff       (20)        0 2023-07-28 17:07:03.889730 chatterstack-2.0.1/chatterstack.egg-info/
+-rw-r--r--   0 davidschiller   (501) staff       (20)    14067 2023-07-28 17:07:03.000000 chatterstack-2.0.1/chatterstack.egg-info/PKG-INFO
+-rw-r--r--   0 davidschiller   (501) staff       (20)      313 2023-07-28 17:07:03.000000 chatterstack-2.0.1/chatterstack.egg-info/SOURCES.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)        1 2023-07-28 17:07:03.000000 chatterstack-2.0.1/chatterstack.egg-info/dependency_links.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)        7 2023-07-28 17:07:03.000000 chatterstack-2.0.1/chatterstack.egg-info/requires.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)       13 2023-07-28 17:07:03.000000 chatterstack-2.0.1/chatterstack.egg-info/top_level.txt
+-rw-r--r--   0 davidschiller   (501) staff       (20)       38 2023-07-28 17:07:03.890164 chatterstack-2.0.1/setup.cfg
+-rw-r--r--   0 davidschiller   (501) staff       (20)      949 2023-07-28 17:06:57.000000 chatterstack-2.0.1/setup.py
```

### Comparing `chatterstack-2.0.0/PKG-INFO` & `chatterstack-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatterstack
-Version: 2.0.0
+Version: 2.0.1
 Summary: A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.
 Home-page: https://github.com/dschil138/chatterstack
 Author: David Schiller
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -315,15 +315,15 @@
 Passing it a negative value will lock your system message to the index counting from the end of the conversation (the example above would make it always be the second to last message in the conversation).
 
 *NOTE: Currently, these methods assume that you only have one system message*
 
 ## 📊 Track and Debug Your Conversation
 Print a formatted version of your conversation (great for debugging)
 ```py
-convo.print_formatted_conversation
+convo.print_formatted_conversation()
 ```
 By default, prints like this:
 ```txt
 System: You are a helpful assistant.
 User: hi!
 Assistant: Hi! How can I help you?
 ```
@@ -345,15 +345,14 @@
 You can now tell the bot "remind me to take the take the garbage out at 8pm", or "remind me to take the garbage out in an hour"
 
 ```
 USER: hey, can you remind me to take the garbage out in an hour
 
 ASSISTANT: Sure! I'll send you a reminder in an hour.
 
-USER: 
 {...time passes...}
 
 ASSISTANT: Hey! Just a quick reminder to take the garbage out!
 ```
 The bot can keep track of as many reminders at you want to issue.
 
 ## Issuing Commands
@@ -363,16 +362,22 @@
 
 USER: [save]
 
 # quit the program
 
 USER: [quit]
 ```
+By default you issue commands by using [ and ] as delimiters. But you can change these to whatever you want:
 
-you can also self-call any method of the chatterstack class itself, right from the chat interface:
+```
+convo.open_command = "{{"
+convo.close_command = "}}"
+```
+
+you can also self-call any method (or set any attribute) of the chatterstack class itself, right from the chat interface:
 ```
 # if you want to see what is currently in the conversation history
 USER: [print_formatted_conversation]
 
 # or how many tokens you have used so far
 USER: [print_total_tokens]
```

### Comparing `chatterstack-2.0.0/README.md` & `chatterstack-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 Passing it a negative value will lock your system message to the index counting from the end of the conversation (the example above would make it always be the second to last message in the conversation).
 
 *NOTE: Currently, these methods assume that you only have one system message*
 
 ## 📊 Track and Debug Your Conversation
 Print a formatted version of your conversation (great for debugging)
 ```py
-convo.print_formatted_conversation
+convo.print_formatted_conversation()
 ```
 By default, prints like this:
 ```txt
 System: You are a helpful assistant.
 User: hi!
 Assistant: Hi! How can I help you?
 ```
@@ -328,15 +328,14 @@
 You can now tell the bot "remind me to take the take the garbage out at 8pm", or "remind me to take the garbage out in an hour"
 
 ```
 USER: hey, can you remind me to take the garbage out in an hour
 
 ASSISTANT: Sure! I'll send you a reminder in an hour.
 
-USER: 
 {...time passes...}
 
 ASSISTANT: Hey! Just a quick reminder to take the garbage out!
 ```
 The bot can keep track of as many reminders at you want to issue.
 
 ## Issuing Commands
@@ -346,16 +345,22 @@
 
 USER: [save]
 
 # quit the program
 
 USER: [quit]
 ```
+By default you issue commands by using [ and ] as delimiters. But you can change these to whatever you want:
 
-you can also self-call any method of the chatterstack class itself, right from the chat interface:
+```
+convo.open_command = "{{"
+convo.close_command = "}}"
+```
+
+you can also self-call any method (or set any attribute) of the chatterstack class itself, right from the chat interface:
 ```
 # if you want to see what is currently in the conversation history
 USER: [print_formatted_conversation]
 
 # or how many tokens you have used so far
 USER: [print_total_tokens]
```

### Comparing `chatterstack-2.0.0/chatterstack/chatterstack.py` & `chatterstack-2.0.1/chatterstack/chatterstack.py`

 * *Files identical despite different names*

### Comparing `chatterstack-2.0.0/chatterstack/chatterstackadvanced.py` & `chatterstack-2.0.1/chatterstack/chatterstackadvanced.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from chatterstack import *
-from commands import *
+from chatterstack.chatterstack import *
+from chatterstack.commands import *
 import signal, ast, datetime, json, re
 
 
 # ---------------- --------------------- ---------------- ---------------------
 # CHATTERSTACK ADVANCED
 # ---------------- --------------------- ---------------- ---------------------
```

### Comparing `chatterstack-2.0.0/chatterstack/commands.py` & `chatterstack-2.0.1/chatterstack/commands.py`

 * *Files identical despite different names*

### Comparing `chatterstack-2.0.0/chatterstack.egg-info/PKG-INFO` & `chatterstack-2.0.1/chatterstack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatterstack
-Version: 2.0.0
+Version: 2.0.1
 Summary: A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.
 Home-page: https://github.com/dschil138/chatterstack
 Author: David Schiller
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -315,15 +315,15 @@
 Passing it a negative value will lock your system message to the index counting from the end of the conversation (the example above would make it always be the second to last message in the conversation).
 
 *NOTE: Currently, these methods assume that you only have one system message*
 
 ## 📊 Track and Debug Your Conversation
 Print a formatted version of your conversation (great for debugging)
 ```py
-convo.print_formatted_conversation
+convo.print_formatted_conversation()
 ```
 By default, prints like this:
 ```txt
 System: You are a helpful assistant.
 User: hi!
 Assistant: Hi! How can I help you?
 ```
@@ -345,15 +345,14 @@
 You can now tell the bot "remind me to take the take the garbage out at 8pm", or "remind me to take the garbage out in an hour"
 
 ```
 USER: hey, can you remind me to take the garbage out in an hour
 
 ASSISTANT: Sure! I'll send you a reminder in an hour.
 
-USER: 
 {...time passes...}
 
 ASSISTANT: Hey! Just a quick reminder to take the garbage out!
 ```
 The bot can keep track of as many reminders at you want to issue.
 
 ## Issuing Commands
@@ -363,16 +362,22 @@
 
 USER: [save]
 
 # quit the program
 
 USER: [quit]
 ```
+By default you issue commands by using [ and ] as delimiters. But you can change these to whatever you want:
 
-you can also self-call any method of the chatterstack class itself, right from the chat interface:
+```
+convo.open_command = "{{"
+convo.close_command = "}}"
+```
+
+you can also self-call any method (or set any attribute) of the chatterstack class itself, right from the chat interface:
 ```
 # if you want to see what is currently in the conversation history
 USER: [print_formatted_conversation]
 
 # or how many tokens you have used so far
 USER: [print_total_tokens]
```

### Comparing `chatterstack-2.0.0/setup.py` & `chatterstack-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatterstack",
-    version="2.0.0",
+    version="2.0.1",
     description="A custom class to manage a list of dictionaries representing a conversation, specifically for ChatGPT models like gpt-3.5-turbo and gpt-4.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="David Schiller",
     url="https://github.com/dschil138/chatterstack",
     packages=find_packages(),
     classifiers=[
```

