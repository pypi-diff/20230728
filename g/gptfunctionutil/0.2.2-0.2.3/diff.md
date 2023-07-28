# Comparing `tmp/gptfunctionutil-0.2.2.tar.gz` & `tmp/gptfunctionutil-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.2.2.tar", last modified: Tue Jul 25 20:34:51 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.2.3.tar", last modified: Fri Jul 28 02:54:13 2023, max compression
```

## Comparing `gptfunctionutil-0.2.2.tar` & `gptfunctionutil-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.229600 gptfunctionutil-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.221600 gptfunctionutil-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/examples/custom_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:34:51.229600 gptfunctionutil-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/converter_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/convertutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib_discord.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/src/gptfunctionutil/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 20:34:51.000000 gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:34:51.225600 gptfunctionutil-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-25 20:34:24.000000 gptfunctionutil-0.2.2/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.870466 gptfunctionutil-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.858466 gptfunctionutil-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/examples/async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/examples/custom_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 02:54:13.870466 gptfunctionutil-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.862466 gptfunctionutil-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/converter_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/convertutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/src/gptfunctionutil/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 02:54:13.000000 gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 02:54:13.866466 gptfunctionutil-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-28 02:53:55.000000 gptfunctionutil-0.2.3/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.2.2/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.2.3/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/.gitignore` & `gptfunctionutil-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/.vscode/settings.json` & `gptfunctionutil-0.2.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/LICENSE` & `gptfunctionutil-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/PKG-INFO` & `gptfunctionutil-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
    + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
```

### Comparing `gptfunctionutil-0.2.2/README.md` & `gptfunctionutil-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
    + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
```

### Comparing `gptfunctionutil-0.2.2/examples/custom_converters.py` & `gptfunctionutil-0.2.3/examples/custom_converters.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/pyproject.toml` & `gptfunctionutil-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.2.2"
+version = "0.2.3"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
 description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
 readme = 'README.md'
 
 keywords = ['OpenAI', 'Function Calling API', 'GPT']
 requires-python = '>=3.10'
```

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/__init__.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/__init__.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/converter_core.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/converter_core.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/convertutil.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/convertutil.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/errors.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/errors.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,14 +317,51 @@
             if len(function_args)>0:
                 #for i, v in function_args.items():
                 #    print("st",i,v)
                 return libmethod.command(self, **function_args)
             return libmethod.command(self)
         else:
             raise AttributeError(f"Method '{function_name}' not found or not callable.")
+    async def call_by_dict_async(self,function_dict: Dict[str, Any]):
+        """
+        Call an function based on the provided dictionary.
+        This function works with coroutines.
+
+        Args:
+            function_dict (Dict[str, Any]): The dictionary containing the function name and arguments.
+
+        Returns:
+            The result of the function call.
+
+        Raises:
+            AttributeError: If the function name is not found or not callable.
+        """
+        try:
+            function_name,function_args=self.parse_name_args(function_dict)
+        except GPTLibError as e:
+            if isinstance(e, FunctionNotFound):
+                '''Invoke a default function so something is returned...'''
+                return self.default_callback(e.function_name,e.arguments)
+
+            result=str(e)
+            return result
+        libmethod = self.FunctionDict.get(function_name)
+
+        if libmethod.comm_type=='coroutine':
+            if len(function_args)>0:
+                return await libmethod.command(self,**function_args)
+            return await libmethod.command(self)
+
+        elif libmethod.comm_type=='callable':
+            function_args=libmethod.convert_args(function_args)
+            if len(function_args)>0:
+                return libmethod.command(self, **function_args)
+            return libmethod.command(self)
+        else:
+            raise AttributeError(f"Method '{function_name}' not found or not callable.")
 
 def genspec(name:str,description:str,**kwargs):
     spec={}
     spec[name]={}
     spec[name]['description']=description
     spec[name].update(kwargs)
     return spec
```

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/functionlib_discord.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/functionlib_discord.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil/logger.py` & `gptfunctionutil-0.2.3/src/gptfunctionutil/logger.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/PKG-INFO` & `gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,15 +60,15 @@
 - **Convert into complex types:** The utility is capable of converting some more complex data types into a json schema, such as datetimes and Literals.
    + Define Custom Converters to automatically use response arguments to initalize objects.
      +  (see examples/custom_converters.py for an example.)
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    + Simply import `gptfunctionutil` into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if a function.) to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)`(or `call_by_dict_ctx` if decorating a discord.py command.) to invoke the corresponding function with the provided arguments.
    + The method also checks if there is a function by that name, falling back to a default response if something goes wrong.
    + Schema can also validate and convert responces returned from the chat/completions endpoint.
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
```

### Comparing `gptfunctionutil-0.2.2/src/gptfunctionutil.egg-info/SOURCES.txt` & `gptfunctionutil-0.2.3/src/gptfunctionutil.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publishpackage.yaml
 .vscode/settings.json
+examples/async_functions.py
 examples/custom_converters.py
 src/README.md
 src/gptfunctionutil/__init__.py
 src/gptfunctionutil/converter_core.py
 src/gptfunctionutil/convertutil.py
 src/gptfunctionutil/errors.py
 src/gptfunctionutil/functionlib.py
```

### Comparing `gptfunctionutil-0.2.2/tests/conftest.py` & `gptfunctionutil-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.2.2/tests/test_methods.py` & `gptfunctionutil-0.2.3/tests/test_methods.py`

 * *Files identical despite different names*

