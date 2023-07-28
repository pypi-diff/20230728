# Comparing `tmp/im_openai-0.7.2.tar.gz` & `tmp/im_openai-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.7.2.tar", last modified: Wed Jul 26 22:08:36 2023, max compression
+gzip compressed data, was "im_openai-0.7.3.tar", last modified: Fri Jul 28 00:48:46 2023, max compression
```

## Comparing `im_openai-0.7.2.tar` & `im_openai-0.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.322852 im_openai-0.7.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.7.2/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.7.2/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.7.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.7.2/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-26 22:08:36.323721 im_openai-0.7.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.7.2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.246557 im_openai-0.7.2/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.7.2/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.7.2/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.263656 im_openai-0.7.2/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-26 22:07:56.000000 im_openai-0.7.2/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5456 2023-07-21 22:04:26.000000 im_openai-0.7.2/im_openai/client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.297186 im_openai-0.7.2/im_openai/langchain/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.7.2/im_openai/langchain/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17290 2023-07-25 00:41:12.000000 im_openai-0.7.2/im_openai/langchain/callbacks.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.7.2/im_openai/langchain/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7888 2023-07-25 03:35:20.000000 im_openai-0.7.2/im_openai/langchain/util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3834 2023-07-21 22:37:56.000000 im_openai-0.7.2/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.7.2/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.283445 im_openai-0.7.2/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.7.2/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-26 22:08:36.326246 im_openai-0.7.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-26 22:07:53.000000 im_openai-0.7.2/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.318875 im_openai-0.7.2/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.7.2/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.7.2/tests/test_im_openai.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9375 2023-07-20 01:08:51.000000 im_openai-0.7.2/tests/test_langchain.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13484 2023-07-25 03:36:46.000000 im_openai-0.7.2/tests/test_langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-07-21 22:42:02.000000 im_openai-0.7.2/tests/test_patch.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.694106 im_openai-0.7.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.7.3/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.7.3/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.7.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.7.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-07-28 00:48:46.695011 im_openai-0.7.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4315 2023-07-26 22:37:33.000000 im_openai-0.7.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.566681 im_openai-0.7.3/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.7.3/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.7.3/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.589998 im_openai-0.7.3/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-28 00:48:07.000000 im_openai-0.7.3/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5671 2023-07-28 00:44:13.000000 im_openai-0.7.3/im_openai/client.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.641518 im_openai-0.7.3/im_openai/langchain/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.7.3/im_openai/langchain/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17280 2023-07-26 22:18:17.000000 im_openai-0.7.3/im_openai/langchain/callbacks.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.7.3/im_openai/langchain/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7888 2023-07-25 03:35:20.000000 im_openai-0.7.3/im_openai/langchain/util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4003 2023-07-28 00:45:25.000000 im_openai-0.7.3/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.7.3/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.621863 im_openai-0.7.3/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.7.3/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-28 00:48:46.697580 im_openai-0.7.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-28 00:48:07.000000 im_openai-0.7.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.688904 im_openai-0.7.3/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.7.3/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.7.3/tests/test_im_openai.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9375 2023-07-20 01:08:51.000000 im_openai-0.7.3/tests/test_langchain.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13484 2023-07-25 03:36:46.000000 im_openai-0.7.3/tests/test_langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-07-21 22:42:02.000000 im_openai-0.7.3/tests/test_patch.py
```

### Comparing `im_openai-0.7.2/CONTRIBUTING.rst` & `im_openai-0.7.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/LICENSE` & `im_openai-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/docs/Makefile` & `im_openai-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/docs/conf.py` & `im_openai-0.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/docs/installation.rst` & `im_openai-0.7.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/docs/make.bat` & `im_openai-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/im_openai/client.py` & `im_openai-0.7.3/im_openai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import aiohttp
 
 
 async def send_event(
     session: aiohttp.ClientSession,
     project_key: str,
+    api_key: str | None,
     *,
     api_name: str | None,
     prompt_event_id: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     prompt_params: Dict | None,
     chat_id: str | None,
@@ -26,21 +27,26 @@
     model_params: Dict | None = None,
 ) -> str | None:
     """Send an event to Imaginary Dev. Returns the id of the event that was added on the server."""
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
-        "projectKey": project_key,
         "apiName": api_name,
         "params": {},
         "prompt": prompt or {},
         "promptEventId": prompt_event_id,
         "modelParameters": model_params or {},
     }
+
+    if project_key is not None:
+        event["projectKey"] = project_key
+    if api_key is not None:
+        event["apiKey"] = api_key
+
     if prompt_template_text is not None:
         if isinstance(prompt_template_text, str):
             # first default template to just the raw text
             event["promptTemplateText"] = prompt_template_text
             if prompt_params is None and getattr(prompt_template_text, "params", None):
                 # Can be TemplateString or any other
                 prompt_params = prompt_template_text.params  # type: ignore
@@ -80,14 +86,15 @@
     if isinstance(json, dict):
         return json.get("id")
 
 
 @asynccontextmanager
 async def event_session(
     project_key: str,
+    api_key: str | None,
     api_name: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     model_params: Dict | None = None,
     chat_id: str | None = None,
     prompt_template_params: dict | None = None,
     prompt_event_id: str | None = None,
@@ -107,14 +114,15 @@
         prompt_event_id = str(uuid.uuid4())
 
     async with aiohttp.ClientSession() as session:
         pending_events_sent = []
         first_event_sent = send_event(
             session=session,
             project_key=project_key,
+            api_key=api_key,
             api_name=api_name,
             prompt_event_id=prompt_event_id,
             prompt_template_text=prompt_template_text,
             prompt_template_chat=prompt_template_chat,
             prompt_params=prompt_template_params,
             chat_id=chat_id,
             parent_event_id=parent_event_id,
@@ -123,14 +131,15 @@
         pending_events_sent.append(first_event_sent)
 
         async def complete_event(response):
             response_time = (time.time() - start) * 1000
             second_event_sent = send_event(
                 session=session,
                 project_key=project_key,
+                api_key=api_key,
                 api_name=api_name,
                 prompt_event_id=prompt_event_id,
                 prompt_template_text=prompt_template_text,
                 prompt_template_chat=prompt_template_chat,
                 prompt_params=prompt_template_params,
                 chat_id=chat_id,
                 parent_event_id=parent_event_id,
```

### Comparing `im_openai-0.7.2/im_openai/langchain/callbacks.py` & `im_openai-0.7.3/im_openai/langchain/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,16 +461,17 @@
         return template_text
 
 
 def _extract_openai_params(serialized: Dict):
     return {k: v for k, v in serialized["kwargs"].items() if isinstance(v, (int, float, str, bool))}
 
 
-def enable_prompt_watch_tracing(callbacks: PromptWatchCallbacks):
+def enable_prompt_watch_tracing(*args, **kwargs):
     """Manually enable prompt watch tracing, returns the previous callback handler to be used when disabling"""
+    callbacks = PromptWatchCallbacks(*args, **kwargs)
     old_tracing_v2_callback = tracing_v2_callback_var.get()
     tracing_v2_callback_var.set(cast(Any, callbacks))
     return old_tracing_v2_callback
 
 
 def disable_prompt_watch_tracing(old_callbacks: BaseCallbackHandler | None):
     """Manually disable prompt watch tracing, possibly restoring the previous callback handler"""
@@ -485,11 +486,10 @@
 
     usage::
 
         with prompt_watch_tracing(project_key, api_name, template_text="Hello {name}"):
             chain = LLMChain(llm=...)
             chain.run("Hello world", inputs={"name": "world"})
     """
-    callbacks = PromptWatchCallbacks(*args, **kwargs)
-    old_tracing_v2_callback = enable_prompt_watch_tracing(callbacks)
+    old_tracing_v2_callback = enable_prompt_watch_tracing(*args, **kwargs)
     yield
     disable_prompt_watch_tracing(old_tracing_v2_callback)
```

### Comparing `im_openai-0.7.2/im_openai/langchain/patch.py` & `im_openai-0.7.3/im_openai/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/im_openai/langchain/util.py` & `im_openai-0.7.3/im_openai/langchain/util.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/im_openai/patch.py` & `im_openai-0.7.3/im_openai/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 def patch_openai_class(cls, get_prompt_template: Callable, get_result: Callable):
     oldcreate = cls.create
 
     async def local_create(
         cls,
         *args,
         ip_project_key=None,
+        ip_api_key=None,
         ip_api_name: str | None = None,
         ip_event_id: str | None = None,
         ip_template_text: str | None = None,
         ip_template_chat: List | None = None,
         ip_template_params=None,
         ip_chat_id: str | None = None,
         ip_parent_event_id: str | None = None,
         **kwargs,
     ):
         if ip_project_key is None:
             ip_project_key = os.environ.get("PROMPT_PROJECT_KEY")
-        if ip_project_key is None:
+        if ip_api_key is None:
+            ip_api_key = os.environ.get("PROMPT_API_KEY")
+        if ip_project_key is None and ip_api_key is None:
             return oldcreate(*args, **kwargs)
 
         model_params = kwargs.copy()
         model_params["modelProvider"] = "openai"
         if "messages" in kwargs:
             template_params = {}
             del model_params["messages"]
@@ -49,14 +52,15 @@
             if isinstance(ip_template, str):
                 ip_template_text = ip_template
             elif isinstance(ip_template, list):
                 ip_template_chat = ip_template
 
         async with event_session(
             project_key=ip_project_key,
+            api_key=ip_api_key,
             api_name=ip_api_name,
             model_params=model_params,
             prompt_template_text=ip_template_text,
             prompt_template_chat=ip_template_chat,
             chat_id=ip_chat_id,
             prompt_template_params=ip_template_params,
             prompt_event_id=ip_event_id,
```

### Comparing `im_openai-0.7.2/im_openai.egg-info/SOURCES.txt` & `im_openai-0.7.3/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/setup.py` & `im_openai-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.7.2",
+    version="0.7.3",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.7.2/tests/test_im_openai.py` & `im_openai-0.7.3/tests/test_im_openai.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/tests/test_langchain.py` & `im_openai-0.7.3/tests/test_langchain.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/tests/test_langchain_util.py` & `im_openai-0.7.3/tests/test_langchain_util.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.2/tests/test_patch.py` & `im_openai-0.7.3/tests/test_patch.py`

 * *Files identical despite different names*

