# Comparing `tmp/filtro-0.1.1.tar.gz` & `tmp/filtro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filtro-0.1.1.tar", max compression
+gzip compressed data, was "filtro-0.1.3.tar", max compression
```

## Comparing `filtro-0.1.1.tar` & `filtro-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1264 2023-06-14 07:34:49.810751 filtro-0.1.1/README.md
--rw-r--r--   0        0        0       35 2023-06-13 23:04:54.215294 filtro-0.1.1/filtro/__init__.py
--rw-r--r--   0        0        0      652 2023-06-14 07:20:21.528966 filtro-0.1.1/filtro/api_client.py
--rw-r--r--   0        0        0      339 2023-06-14 07:45:06.400431 filtro-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 filtro-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1368 2023-07-28 09:15:52.235204 filtro-0.1.3/README.md
+-rw-r--r--   0        0        0       35 2023-07-28 09:15:52.239205 filtro-0.1.3/filtro/__init__.py
+-rw-r--r--   0        0        0      775 2023-07-28 09:15:52.239205 filtro-0.1.3/filtro/api_client.py
+-rw-r--r--   0        0        0      339 2023-07-28 09:15:52.239205 filtro-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 filtro-0.1.3/PKG-INFO
```

### Comparing `filtro-0.1.1/README.md` & `filtro-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -11,34 +11,30 @@
 ## 🗣️ Usage
 
 ```py
 from filtro import mask, clear
 
 masked, mapping = mask(
     "Hi my name is Giovanni, I work at Google. What's up?"
-)
+) # Hi my name is Maria, I work at Marvel. What's up?
 
 from langchain.llms import OpenAI
 llm = OpenAI(temperature=0.9)
-response = llm(masked)
+response = llm(masked) # Hi Maria! Im fine. Yourself?
 
-cleared = clear(response, mapping)
+cleared = clear(response, mapping) # Hi Giovanni! Im fine. Yourself?
 ```
 
 ## 🥽 Examples
+The standard discussion
+```diff
+Hi my name is Gianmarco Rengucci! I am a software engineer at Apple, here in Milan. Whats up?
++[filtro.ai] Hi my name is Terri Clark! I am a manager at Google, here in Singapore. Whats up?
+-[chat.openai.com] Hey there Terri! Doing great. Curious to learn more about Google. Tell me more!
++[filtro.ai]  Hey there Gianmarco! Doing great. Curious to learn more about Apple. Tell me more!
+```
 
-```py
-python examples/basic.py
-````
-
-
-<details> <summary> Show output </summary>
-
-[YOUR INPUT] Hi my name is Gianmarco Rengucci! I am a Software Engineer at Apple, here in Milan. Whats up?
-
-[FILTRO.AI] Hi my name is Terri Clark! I am a Software Engineer at Compton-Krueger, here in Lake Erin. Whats up?
-
-[OPENAI] Hey there Terri, nice to meet you! Im doing great, but Im curious to learn more about what you do at Compton-Krueger. Could you tell me a little bit about your role at the company?
-
-[FILTRO.AI] Hey there Gianmarco, nice to meet you! Im doing great, but Im curious to learn more about what you do at Apple. Could you tell me a little bit about your role at the company?
-
-</details>
+The email and credit cards credentials
+```diff
+Card number is 1234 5678 9012 3456. You can reach out to richard@gmail.com for questions 🤗 
++[filtro.ai] Card number is 6546410405081471.. You can reach out to teresabrooks@example.org for questions 🍖
+```
```

### Comparing `filtro-0.1.1/PKG-INFO` & `filtro-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filtro
-Version: 0.1.1
+Version: 0.1.3
 Summary: The official filtro python package.
 Author: Andrea Pinto
 Author-email: andrea@filtro.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,35 +26,31 @@
 ## 🗣️ Usage
 
 ```py
 from filtro import mask, clear
 
 masked, mapping = mask(
     "Hi my name is Giovanni, I work at Google. What's up?"
-)
+) # Hi my name is Maria, I work at Marvel. What's up?
 
 from langchain.llms import OpenAI
 llm = OpenAI(temperature=0.9)
-response = llm(masked)
+response = llm(masked) # Hi Maria! Im fine. Yourself?
 
-cleared = clear(response, mapping)
+cleared = clear(response, mapping) # Hi Giovanni! Im fine. Yourself?
 ```
 
 ## 🥽 Examples
+The standard discussion
+```diff
+Hi my name is Gianmarco Rengucci! I am a software engineer at Apple, here in Milan. Whats up?
++[filtro.ai] Hi my name is Terri Clark! I am a manager at Google, here in Singapore. Whats up?
+-[chat.openai.com] Hey there Terri! Doing great. Curious to learn more about Google. Tell me more!
++[filtro.ai]  Hey there Gianmarco! Doing great. Curious to learn more about Apple. Tell me more!
+```
 
-```py
-python examples/basic.py
-````
-
-
-<details> <summary> Show output </summary>
-
-[YOUR INPUT] Hi my name is Gianmarco Rengucci! I am a Software Engineer at Apple, here in Milan. Whats up?
-
-[FILTRO.AI] Hi my name is Terri Clark! I am a Software Engineer at Compton-Krueger, here in Lake Erin. Whats up?
-
-[OPENAI] Hey there Terri, nice to meet you! Im doing great, but Im curious to learn more about what you do at Compton-Krueger. Could you tell me a little bit about your role at the company?
-
-[FILTRO.AI] Hey there Gianmarco, nice to meet you! Im doing great, but Im curious to learn more about what you do at Apple. Could you tell me a little bit about your role at the company?
-
-</details>
+The email and credit cards credentials
+```diff
+Card number is 1234 5678 9012 3456. You can reach out to richard@gmail.com for questions 🤗 
++[filtro.ai] Card number is 6546410405081471.. You can reach out to teresabrooks@example.org for questions 🍖
+```
```

