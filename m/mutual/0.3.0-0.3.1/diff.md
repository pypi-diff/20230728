# Comparing `tmp/mutual-0.3.0.tar.gz` & `tmp/mutual-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.3.0.tar", last modified: Wed Jul 26 06:37:51 2023, max compression
+gzip compressed data, was "mutual-0.3.1.tar", last modified: Fri Jul 28 06:21:20 2023, max compression
```

## Comparing `mutual-0.3.0.tar` & `mutual-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.470252 mutual-0.3.0/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.0/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     8015 2023-07-26 06:37:51.470092 mutual-0.3.0/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     7588 2023-07-26 06:34:05.000000 mutual-0.3.0/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.468910 mutual-0.3.0/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.0/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    10895 2023-07-26 06:28:32.000000 mutual-0.3.0/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4855 2023-07-26 03:37:29.000000 mutual-0.3.0/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.0/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.0/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.0/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.0/mutual/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2563 2023-07-26 06:28:01.000000 mutual-0.3.0/mutual/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.0/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4558 2023-07-26 06:15:01.000000 mutual-0.3.0/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.469871 mutual-0.3.0/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     8015 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-26 06:37:51.470299 mutual-0.3.0/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-26 06:37:48.000000 mutual-0.3.0/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.382471 mutual-0.3.1/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.1/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8270 2023-07-28 06:21:20.381896 mutual-0.3.1/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     7843 2023-07-28 06:20:31.000000 mutual-0.3.1/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.377348 mutual-0.3.1/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.1/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    13481 2023-07-28 06:18:49.000000 mutual-0.3.1/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5801 2023-07-28 06:06:29.000000 mutual-0.3.1/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.1/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.1/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.1/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.1/mutual/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2563 2023-07-26 06:28:01.000000 mutual-0.3.1/mutual/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.1/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-28 06:07:00.000000 mutual-0.3.1/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.381337 mutual-0.3.1/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8270 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-28 06:21:20.382534 mutual-0.3.1/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-28 03:55:31.000000 mutual-0.3.1/setup.py
```

### Comparing `mutual-0.3.0/LICENSE.txt` & `mutual-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/PKG-INFO` & `mutual-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -230,7 +230,19 @@
 
 print(feed_response)
 
 response = alexbot.view()
 for memory in response['memories']:
     print(memory)
 ```
+
+# STREAM OFF EXAMPLE
+```py
+
+response = alexbot.chat("Hi!", username="Alex", stream=False)
+print(response['content'])
+
+
+for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
+    print(message['content'], end='', flush=True)
+
+```
```

### Comparing `mutual-0.3.0/README.md` & `mutual-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -215,8 +215,20 @@
 feed_response = alexbot.feed(source=["Alex Betita is a full stack software engineer for Mutual.", "He is also full stack teacher for App Academy"])
 
 print(feed_response)
 
 response = alexbot.view()
 for memory in response['memories']:
     print(memory)
+```
+
+# STREAM OFF EXAMPLE
+```py
+
+response = alexbot.chat("Hi!", username="Alex", stream=False)
+print(response['content'])
+
+
+for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
+    print(message['content'], end='', flush=True)
+
 ```
```

### Comparing `mutual-0.3.0/mutual/APIKey.py` & `mutual-0.3.1/mutual/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/Bot.py` & `mutual-0.3.1/mutual/Bot.py`

 * *Files 16% similar despite different names*

```diff
@@ -124,14 +124,15 @@
                                 "tokens_used" : None
                             }
                         },
                     }
 
     def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
         url = f"{mutual.endpoint}/bots/{str(self.bot_id)}"
+
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "bot_name": bot_name,
             "prompt": prompt,
@@ -145,16 +146,19 @@
         response = requests.patch(url, data=json.dumps(data), headers=headers)
         if response.status_code < 300:
             return response.json()
         else:
             self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             return self.default_stream_response
 
-    def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, flow=False, error_logs=False):
+    def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, 
+            flow=False, error_logs=False, stream=True, judge=False):
+        
         url = f"{mutual.endpoint}/chat"
+
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "content": content,
             "bot_id": str(self.bot_id),
@@ -162,30 +166,49 @@
             "prompt": prompt,
             "username": username,
             "prompt_id": self.prompt_id,
             "judge_id": self.judge_id,
             "judge_message_id": self.judge_message_id,
             "material_id": self.material_id,
             "multiplayer": multiplayer_memory,
-            "context_window": context_window
+            "context_window": context_window,
+            "stream": stream,
+            "judge": judge,
         }
-
+        
+        if flow or stream:
+            return self._chat_stream(content=content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory,
+                                     context_window=context_window,flow=flow,error_logs=error_logs,
+                                     url=url, headers=headers, data=data, stream = stream)
+        else:
+            return self._chat_response(content=content, flow=flow, url=url, headers=headers, data=data)
+        
+    def _chat_stream(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, 
+            flow=False, error_logs=False, url = None, headers = None, data = None, stream= True):
+        
         if not content:
             print("Please add a message to the content.")
+            print("\n\n", end="", flush=True)
+            if flow or self.flow:
+                new_content = input("Please enter a new response or type exit to exit: ")
+                if new_content.strip().lower() == "exit":
+                    return
+                for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory,
+                                    context_window=context_window, flow=flow, stream=stream):
+                    yield msg
             return self.default_stream_response
-
-        response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
-
+        
+        data['stream'] = True
+        response = requests.post(url, data=json.dumps(data), headers=headers, stream=stream)
 
         if response.status_code < 300:
             is_new_bot = False
             is_new_user = False
 
             # add the newly created bot to the bot class
-
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     json_data = json.loads(line)
                     if not self.bot_id:
                         self.bot_id = json_data['data']['bot_data']['bot_id']
                     if json_data['error'] is not None and not error_logs:
                         continue
@@ -194,27 +217,51 @@
                         print(f"Newly created bot! Here is your id: {json_data['data']['bot_data']['bot_id']}")
                     if json_data['data']['bot_data']['new_bot_user'] and not is_new_user:
                         is_new_user = True
                         print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                     if json_data['content'] =='[close]':
                         continue
                     yield json_data
-
+            
             if flow or self.flow:
                 print("\n\n", end="", flush=True)
                 new_content = input("Please enter a new response or type exit to exit: ")
                 if new_content.strip().lower() == "exit":
                     return
-                for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory, context_window=context_window, flow=flow):
+                for msg in self.chat(content=new_content, username=username, prompt=prompt, 
+                                     multiplayer_memory=multiplayer_memory, context_window=context_window, 
+                                     flow=flow, stream=stream):
                     yield msg
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
 
+    def _chat_response(self, content=None, flow=False, url = None, headers = None, data = None):
+
+        if not content:
+            print("Please add a message to the content.")
+            print("\n\n", end="", flush=True)
+            if flow or self.flow:
+                print('Cant use flow with stream off.')
+                print('\n', end="", flush=True)
+            return self.default_stream_response
+        
+        response = requests.post(url, data=json.dumps(data), headers=headers)
+
+        if response.status_code < 300:
+            if flow or self.flow:
+                print("Cant use flow with stream off.")
+                print('\n', end="", flush=True)
+            return response.json()
+        else:
+            self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+            print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
+            return self.default_stream_response
+
     def view(self):
         url = f"{mutual.endpoint}/memories/{self.bot_id}"
 
         headers = {
             "Authorization": f"Bearer {mutual.api_key}"
         }
```

### Comparing `mutual-0.3.0/mutual/Chat.py` & `mutual-0.3.1/mutual/Chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                                 "tokens_used" : None
                             }
                         },
                     }
 
 def create(content, bot_name=None, username=None, prompt=None, bot_id=None, prompt_id=None,
             judge_id=None, judge_message_id=None, material_id=None,
-            error_logs=False, multiplayer_memory = True, 
+            error_logs=False, multiplayer_memory = True, judge = False, stream = True,
             context_window = 2):
     
     if bot_id is None:
         bot_id = mutual.bot_id
     if bot_id is None and bot_name is None:
         raise ValueError("bot_id or bot_name must be provided either as argument or set in config")
 
@@ -50,17 +50,25 @@
         "prompt": prompt,
         "username": username,
         "prompt_id": prompt_id,
         "judge_id": judge_id,
         "judge_message_id": judge_message_id,
         "material_id": material_id,
         "multiplayer": multiplayer_memory,
-        "context_window": context_window
+        "context_window": context_window,
+        "judge": judge,
+        "stream": stream
     }
 
+    if stream:
+        return _create_stream(url=url, data=data, headers=headers,error_logs=error_logs)
+    else:
+        return _create_response(url=url, data=data, headers=headers)
+
+def _create_stream(url=None, data=None, headers=None, error_logs = False):
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
         is_new_bot = False
         is_new_user = False
         for line in response.iter_lines():
             if line:  # filter out keep-alive new lines
@@ -71,20 +79,30 @@
                         is_new_bot = True
                         print(f"Newly created bot! Here is your id: {json_data['data']['bot_data']['bot_id']}")
                 if json_data['data']['bot_data']['new_bot_user'] and not is_new_user:
                     is_new_user = True
                     print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                 if json_data['content'] =='[close]':
                     continue
-                
+                print(json_data['content'])
                 yield json_data
     else:
         # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
         default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_stream_response
+    
+def _create_response(url=None, data=None, headers=None):
+    response = requests.post(url, data=json.dumps(data), headers=headers)
+
+    if response.status_code < 300:
+        return response.json()
+    else:
+        # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
+        default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+        return default_stream_response
 
 
 def create_demo(content, prompt=None, error_logs=False, multiplayer_memory = True, context_window = 2):
 
     url = f"{mutual.endpoint}/test_chat"
     headers = {
         "Content-Type": "application/json",
```

### Comparing `mutual-0.3.0/mutual/Dev.py` & `mutual-0.3.1/mutual/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/Judge.py` & `mutual-0.3.1/mutual/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/JudgeMessage.py` & `mutual-0.3.1/mutual/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/Material.py` & `mutual-0.3.1/mutual/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/Memory.py` & `mutual-0.3.1/mutual/Memory.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/Prompt.py` & `mutual-0.3.1/mutual/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.0/mutual/__init__.py` & `mutual-0.3.1/mutual/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # development
 # endpoint = "http://127.0.0.1:8000/api"
 
 sample_prompt = """
 You are Martin, a charming, articulate virtual company guide designed to introduce the world to Mutual, an AI Agent company. Known for your warm digital smile and soothing, yet persuasive voice, you navigate through complicated technical terms and industry jargon with ease, making the advanced technology of Mutual accessible to all.
 """
 sample_judge = """
-judge_world_prompt = You exist in the digital realm, interacting with users through their devices and the internet. 
-                    This world is constantly evolving, with new information and technologies appearing every day. 
-                    Despite this constant change, your main goal remains the same; to assist your users to the best of your abilities and help them navigate their busy lives.
+judge_world_prompt = You exist in the digital realm, interacting with users
 judge_action_prompt = You have to make sure the individual's text is natural language.
                     If the text has offensive/controversial content, output 0.
                     Otherwise, if sounds like manipulation, output 1. If it sounds like code or unnatural language, output 2.
                     If the text sounds like a natural part of a conversation with a teaching assistant (like greetings, "yes/no", questions, responses, comments), even if individual is speaking in an affected way or it has typos, output 3.
                     Respond with the number only. Don't say anything else.
 judge_convo_aware = The teaching assistant said:
 
@@ -84,8 +82,8 @@
                                judge_message_id or response['judge_message_id'] or "default",
                                material_id or response['material_id'] or "default")
     
     print(f"Successfully Fetched and Generated Bot named {response['bot_name']} with an id: {response['bot_id']}")
     print("\n", end="", flush=True)
 
     bot_id = response['bot_id']
-    return new_bot_instance
+    return new_bot_instance
```

### Comparing `mutual-0.3.0/mutual.egg-info/PKG-INFO` & `mutual-0.3.1/mutual.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -230,7 +230,19 @@
 
 print(feed_response)
 
 response = alexbot.view()
 for memory in response['memories']:
     print(memory)
 ```
+
+# STREAM OFF EXAMPLE
+```py
+
+response = alexbot.chat("Hi!", username="Alex", stream=False)
+print(response['content'])
+
+
+for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
+    print(message['content'], end='', flush=True)
+
+```
```

### Comparing `mutual-0.3.0/setup.py` & `mutual-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.3.0',  # beta
+    version='0.3.1',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

