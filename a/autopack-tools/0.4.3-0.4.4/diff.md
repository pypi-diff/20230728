# Comparing `tmp/autopack_tools-0.4.3.tar.gz` & `tmp/autopack_tools-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.4.3.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.4.tar", max compression
```

## Comparing `autopack_tools-0.4.3.tar` & `autopack_tools-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.3/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.3/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.3/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.3/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.3/autopack/__main__.py
--rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.3/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.3/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.3/autopack/errors.py
--rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.3/autopack/filesystem_emulation/__init__.py
--rw-r--r--   0        0        0      950 2023-07-27 03:50:15.932646 autopack_tools-0.4.3/autopack/filesystem_emulation/file_manager.py
--rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.3/autopack/filesystem_emulation/filesystem_file_manager.py
--rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.3/autopack/filesystem_emulation/ram_file_manager.py
--rw-r--r--   0        0        0     4052 2023-07-27 04:47:20.015891 autopack_tools-0.4.3/autopack/filesystem_emulation/workspace_file_manager.py
--rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.3/autopack/get_pack.py
--rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.3/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.3/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5529 2023-07-27 04:17:12.352396 autopack_tools-0.4.3/autopack/pack.py
--rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.3/autopack/pack_config.py
--rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.3/autopack/pack_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.3/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.3/autopack/search.py
--rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.3/autopack/selection.py
--rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.3/autopack/utils.py
--rw-r--r--   0        0        0     1101 2023-07-27 04:54:38.971302 autopack_tools-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.4/README.md
+-rw-r--r--   0        0        0        6 2023-07-27 22:24:02.938972 autopack_tools-0.4.4/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-27 22:24:02.910492 autopack_tools-0.4.4/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-27 22:24:02.910843 autopack_tools-0.4.4/autopack/__main__.py
+-rw-r--r--   0        0        0     2824 2023-07-27 22:27:08.593199 autopack_tools-0.4.4/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-27 22:24:02.924162 autopack_tools-0.4.4/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-27 22:24:02.924415 autopack_tools-0.4.4/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-27 22:24:02.929186 autopack_tools-0.4.4/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-27 22:24:02.935685 autopack_tools-0.4.4/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     3562 2023-07-27 22:24:02.927211 autopack_tools-0.4.4/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     2985 2023-07-27 22:24:02.928880 autopack_tools-0.4.4/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     4052 2023-07-27 22:24:02.934181 autopack_tools-0.4.4/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 22:24:02.936287 autopack_tools-0.4.4/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-27 22:24:02.936559 autopack_tools-0.4.4/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-27 22:24:02.936811 autopack_tools-0.4.4/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5529 2023-07-27 22:24:02.937091 autopack_tools-0.4.4/autopack/pack.py
+-rw-r--r--   0        0        0     3309 2023-07-27 22:26:44.374185 autopack_tools-0.4.4/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 22:24:02.937629 autopack_tools-0.4.4/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-27 22:24:02.937878 autopack_tools-0.4.4/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-27 22:24:02.938125 autopack_tools-0.4.4/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 22:24:02.938390 autopack_tools-0.4.4/autopack/selection.py
+-rw-r--r--   0        0        0     8049 2023-07-28 20:01:33.520893 autopack_tools-0.4.4/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-07-28 20:01:33.521215 autopack_tools-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.4/PKG-INFO
```

### Comparing `autopack_tools-0.4.3/LICENSE` & `autopack_tools-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/README.md` & `autopack_tools-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/api.py` & `autopack_tools-0.4.4/autopack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from json import JSONDecodeError
 from urllib.parse import urljoin
 
 import requests
 from marshmallow import ValidationError
 
 from autopack.errors import AutoPackFetchError
+from autopack.pack_config import PackConfig
 from autopack.pack_response import PackResponse
 from autopack.utils import find_or_create_autopack_dir
 
-API_URL = os.environ.get("AUTOPACK_API_URL", "https://autopack.ai/")
-
 
 def get_pack_details(pack_id: str, remote=False) -> PackResponse:
     if remote:
         return get_pack_details_remotely(pack_id)
 
     return get_pack_details_locally(pack_id)
 
@@ -40,15 +39,15 @@
 
     return PackResponse(**pack_metadata)
 
 
 def get_pack_details_remotely(pack_id: str) -> PackResponse:
     endpoint = "/api/details"
 
-    url = urljoin(API_URL, endpoint)
+    url = urljoin(PackConfig.global_config().api_url, endpoint)
     params = {"id": pack_id}
 
     response = requests.get(url, params=params)
     if response.status_code == 200:
         data = response.json()
 
         try:
@@ -61,15 +60,15 @@
         raise AutoPackFetchError(f"Error: {response.status_code}")
     else:
         raise AutoPackFetchError(f"Error: {response.status_code}")
 
 
 def pack_search(query: str) -> list[PackResponse]:
     endpoint = "/api/search"
-    url = urljoin(API_URL, endpoint)
+    url = urljoin(PackConfig.global_config().api_url, endpoint)
     params = {"query": query}
 
     response = requests.get(url, params=params)
     if response.status_code == 200:
         data = response.json()
 
         try:
```

### Comparing `autopack_tools-0.4.3/autopack/cli.py` & `autopack_tools-0.4.4/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/filesystem_emulation/file_manager.py` & `autopack_tools-0.4.4/autopack/filesystem_emulation/file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/filesystem_emulation/filesystem_file_manager.py` & `autopack_tools-0.4.4/autopack/filesystem_emulation/filesystem_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/filesystem_emulation/ram_file_manager.py` & `autopack_tools-0.4.4/autopack/filesystem_emulation/ram_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/filesystem_emulation/workspace_file_manager.py` & `autopack_tools-0.4.4/autopack/filesystem_emulation/workspace_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/get_pack.py` & `autopack_tools-0.4.4/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/installation.py` & `autopack_tools-0.4.4/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/langchain_wrapper.py` & `autopack_tools-0.4.4/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/pack.py` & `autopack_tools-0.4.4/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/pack_config.py` & `autopack_tools-0.4.4/autopack/pack_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     )
     installer_style: InstallerStyle = Field(
         description="Style and permissiveness of Pack installation", default=InstallerStyle.automatic
     )
     restrict_code_execution: bool = Field(
         description="If True will signal to Packs that they should not execute code", default=False
     )
+    api_url: str = Field(
+        description="Scheme, hostname, and port of the AutoPack API you wish to use.", default="https://autopack.ai/"
+    )
     # Not implemented yet
     local_packs: list[type["Pack"]] = Field(
         description="A list of local Pack classes that you wish to be included in the selection process",
         default_factory=list,
     )
 
     @classmethod
```

### Comparing `autopack_tools-0.4.3/autopack/prompts.py` & `autopack_tools-0.4.4/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/selection.py` & `autopack_tools-0.4.4/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.3/autopack/utils.py` & `autopack_tools-0.4.4/autopack/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             "name": param_name,
             "description": param.get("description", ""),
             "required": param_name in schema.get("required", []),
         }
     return run_args
 
 
-def functions_bulleted_list(packs: list[type["Pack"]]) -> str:
+def functions_bulleted_list(packs: list[Union[PackResponse, type["Pack"]]]) -> str:
     functions_string = []
     grouped_packs: dict[str, list[type[Pack]]] = {}
     for pack in packs:
         if not pack.categories:
             continue
 
         for category in pack.categories:
@@ -154,20 +154,24 @@
                 grouped_packs[category] = []
             grouped_packs[category].append(pack)
 
     for category, category_packs in grouped_packs.items():
         functions_string.append(f"\n## {category}")
         sorted_by_name = sorted(category_packs, key=lambda p: p.name)
         for pack in sorted_by_name:
-            args: list[dict[str, str]] = []
-            if pack.args_schema:
-                args = list(run_args_from_args_schema(pack.args_schema).values())
-            args_signature = ", ".join([f"{arg.get('name')}: {arg.get('type')}" for arg in args])
+            if hasattr(pack, "run_args"):
+                args = pack.run_args
+            elif hasattr(pack, "args_schema") and pack.args_schema:
+                args = run_args_from_args_schema(pack.args_schema)
+            else:
+                args = {}
+
+            args_signature = ", ".join([f"{name}: {arg.get('type')}" for name, arg in args.items()])
             args_descriptions = (
-                "; ".join([f"{arg.get('name')} ({arg.get('type')}): {arg.get('description')}" for arg in args])
+                "; ".join([f"{name} ({arg.get('type')}): {arg.get('description')}" for name, arg in args.items()])
                 or "None."
             )
             functions_string.append(
                 f"- {pack.name}({args_signature}): {pack.description} | Arguments: {args_descriptions}"
             )
 
     return "\n".join(functions_string)
```

### Comparing `autopack_tools-0.4.3/pyproject.toml` & `autopack_tools-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.4.3"
+version = "0.4.4"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.4.3/PKG-INFO` & `autopack_tools-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

