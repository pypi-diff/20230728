# Comparing `tmp/llm_prompt_creator-0.4.0.tar.gz` & `tmp/llm_prompt_creator-0.5.0.tar.gz`

## Comparing `llm_prompt_creator-0.4.0.tar` & `llm_prompt_creator-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/src/llm_prompt_creator/__init__.py
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/src/llm_prompt_creator/prompt.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/LICENSE
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/README.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 llm_prompt_creator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/src/llm_prompt_creator/__init__.py
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/src/llm_prompt_creator/prompt.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/README.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 llm_prompt_creator-0.5.0/PKG-INFO
```

### Comparing `llm_prompt_creator-0.4.0/.DS_Store` & `llm_prompt_creator-0.5.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.4.0/src/llm_prompt_creator/prompt.py` & `llm_prompt_creator-0.5.0/src/llm_prompt_creator/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,16 @@
     promptTemplate = ""
     questions=[]
 
     # Load the promptTemplate for model context :
     if filePath != None:
         with open(filePath, "r") as f:
             data = json.load(f)
-            promptTemplate = data['promptTemplate']
-            questions = data['questions']
+            promptTemplate = data.get('promptTemplate', "")
+            questions = data.get('questions',[])
     if promptTemplate=="":
         promptTemplate = """You are a world-class Java developer with an eagle eye for unintended bugs and edge cases. You carefully explain code with great detail and accuracy. You organize your explanations in markdown-formatted, bulleted lists.
         You write careful, accurate unit tests. When asked to reply only with code, you write all of your code in a single block.
         A good unit test suite should aim to:
         - Test the function's behavior for a wide range of possible inputs
         - Test edge cases that the author may not have foreseen
         - Take advantage of the features of `pytest` to make the tests easy to write and maintain
@@ -207,14 +207,15 @@
     # Retrieve chunks based on the question and assemble them into a joined context:
     """
     Lock the user in a loop to keep asking questions until they type 'exit'
     Add the LLM's answer to the chat history to keep the feedback more conversational
     """
     while True:
         for q in questions:
+            print(q)
             handle_question(q, store,llm,show_context, write_to_disk,promptTemplate,history)
             print('---------------------------------------------------------- \n')
 
         if len(questions) > 0:
             break
         #break if reading questions from file - if we want the functionality to instead continue
         #to prompt user, remove this if check
```

### Comparing `llm_prompt_creator-0.4.0/LICENSE` & `llm_prompt_creator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.4.0/README.md` & `llm_prompt_creator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.4.0/pyproject.toml` & `llm_prompt_creator-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "archive/",
     "venv/",
     "*.json",
 ]
 
 [project]
 name = "llm_prompt_creator"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     {name="Chris Mills", email="cmills@breakfreesolutions.com"},
     {name="Zak Alford", email="zalford@breakfreesolutions.com"}
 ]
 description = "Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `llm_prompt_creator-0.4.0/PKG-INFO` & `llm_prompt_creator-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_prompt_creator
-Version: 0.4.0
+Version: 0.5.0
 Summary: Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models.
 Project-URL: Homepage, https://github.com/break-free/fineract-unit-tests-openai
 Project-URL: Issues, https://github.com/break-free/fineract-unit-tests-openai/issues
 Author-email: Chris Mills <cmills@breakfreesolutions.com>, Zak Alford <zalford@breakfreesolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

