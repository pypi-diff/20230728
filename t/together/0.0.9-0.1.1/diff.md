# Comparing `tmp/together-0.0.9.tar.gz` & `tmp/together-0.1.1.tar.gz`

## Comparing `together-0.0.9.tar` & `together-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.9/.github/workflows/check_code_quality.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.9/src/together/__init__.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 together-0.0.9/src/together/api.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 together-0.0.9/src/together/files.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 together-0.0.9/src/together/finetune.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 together-0.0.9/src/together/inference.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.9/src/together/cli/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 together-0.0.9/src/together/cli/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/api.py
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/chat.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/files.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/finetune.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 together-0.0.9/src/together/commands/inference.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.9/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 together-0.0.9/src/together/utils/conversation.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.9/src/together/utils/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.9/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.9/README.md
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 together-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 together-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.1.1/.github/workflows/check_code_quality.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 together-0.1.1/src/together/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 together-0.1.1/src/together/complete.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 together-0.1.1/src/together/error.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 together-0.1.1/src/together/files.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 together-0.1.1/src/together/finetune.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 together-0.1.1/src/together/image.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 together-0.1.1/src/together/models.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 together-0.1.1/src/together/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/cli/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 together-0.1.1/src/together/cli/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/chat.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/complete.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/files.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/finetune.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/image.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 together-0.1.1/src/together/commands/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/conversation.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 together-0.1.1/src/together/utils/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 together-0.1.1/README.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 together-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 together-0.1.1/PKG-INFO
```

### Comparing `together-0.0.9/.github/workflows/check_code_quality.yml` & `together-0.1.1/.github/workflows/check_code_quality.yml`

 * *Files identical despite different names*

### Comparing `together-0.0.9/src/together/inference.py` & `together-0.1.1/src/together/complete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,179 +1,151 @@
 import json
-import os
-import urllib.parse
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Iterator, Optional
 
 import requests
 import sseclient  # type: ignore
 
-from together.utils.utils import exit_1, get_logger
+import together
+from together import get_logger, verify_api_key
 
 
-DEFAULT_ENDPOINT = "https://api.together.xyz/"
+logger = get_logger(str(__name__), log_level=together.log_level)
 
 
-class Inference:
+class Complete:
     def __init__(
         self,
-        endpoint_url: Optional[str] = None,
-        log_level: str = "WARNING",
-        task: Optional[str] = "text2text",
-        model: Optional[str] = None,
+    ) -> None:
+        verify_api_key(logger)
+
+    @classmethod
+    def create(
+        self,
+        prompt: str,
+        model: Optional[str] = "",
         max_tokens: Optional[int] = 128,
         stop: Optional[str] = None,
         temperature: Optional[float] = 0.7,
         top_p: Optional[float] = 0.7,
         top_k: Optional[int] = 50,
         repetition_penalty: Optional[float] = None,
         logprobs: Optional[int] = None,
-        raw: Optional[bool] = False,
-        # TODO stream_tokens: Optional[bool] = None
-        steps: Optional[int] = 50,
-        seed: Optional[int] = 42,
-        results: Optional[int] = 1,
-        height: Optional[int] = 512,
-        width: Optional[int] = 512,
-    ) -> None:
-        # Setup logger
-        self.logger = get_logger(str(__name__), log_level=log_level)
-
-        together_api_key = os.environ.get("TOGETHER_API_KEY", None)
-        if together_api_key is None:
-            self.logger.critical(
-                "TOGETHER_API_KEY not found. Please set it as an environment variable."
-            )
-            exit_1(self.logger)
-
-        if endpoint_url is None:
-            endpoint_url = DEFAULT_ENDPOINT
-
-        self.together_api_key = together_api_key
-        self.endpoint_url = urllib.parse.urljoin(endpoint_url, "/api/inference")
-
-        self.task = task
-        self.model = model
-        self.max_tokens = max_tokens
-        self.stop = stop
-        self.temperature = temperature
-        self.top_p = top_p
-        self.top_k = top_k
-        self.repetition_penalty = repetition_penalty
-        self.logprobs = logprobs
-
-        # text2img arguments
-        self.steps = steps
-        self.seed = seed
-        self.results = results
-        self.height = height
-        self.width = width
-
-    def inference(
-        self,
-        prompt: str,
     ) -> Dict[str, Any]:
-        if self.task == "text2text":
-            parameter_payload = {
-                "model": self.model,
-                "prompt": prompt,
-                "top_p": self.top_p,
-                "top_k": self.top_k,
-                "temperature": self.temperature,
-                "max_tokens": self.max_tokens,
-                "stop": self.stop,
-                "repetition_penalty": self.repetition_penalty,
-                "logprobs": self.logprobs,
-            }
-        elif self.task == "text2img":
-            parameter_payload = {
-                "model": self.model,
-                "prompt": prompt,
-                "n": self.results,
-                "mode": self.task,
-                "steps": self.steps,
-                "seed": self.seed,
-                "height": self.height,
-                "width": self.width,
-            }
-        else:
-            self.logger.critical(
-                f"Invalid task: {self.task}. Pick from either text2text or text2img."
-            )
-            exit_1(self.logger)
+        if model == "":
+            model = together.default_text_model
+
+        parameter_payload = {
+            "model": model,
+            "prompt": prompt,
+            "top_p": top_p,
+            "top_k": top_k,
+            "temperature": temperature,
+            "max_tokens": max_tokens,
+            "stop": stop,
+            "repetition_penalty": repetition_penalty,
+            "logprobs": logprobs,
+        }
 
         # HTTP headers for authorization
         headers = {
-            "Authorization": f"Bearer {self.together_api_key}",
+            "Authorization": f"Bearer {together.api_key}",
             "Content-Type": "application/json",
+            "User-Agent": together.user_agent,
         }
 
         # send request
         try:
             response = requests.post(
-                self.endpoint_url,
+                together.api_base_complete,
                 headers=headers,
                 json=parameter_payload,
             )
         except requests.exceptions.RequestException as e:
-            self.logger.critical(f"Response error raised: {e}")
-            exit_1(self.logger)
+            logger.critical(f"Response error raised: {e}")
+            raise together.ResponseError(e)
+
+        if response.status_code == 429:
+            logger.critical(
+                f"No running instances for {model}. You can start an instance by navigating to the Together Playground at api.together.ai"
+            )
+            raise together.InstanceError(model=model)
+
+        response.raise_for_status()
 
         try:
             response_json = dict(response.json())
+
         except Exception as e:
-            self.logger.critical(
-                f"JSON Error raised: {e}\nResponse status code = {response.status_code}"
+            logger.critical(
+                f"Error raised: {e}\nResponse status code = {response.status_code}"
             )
-            exit_1(self.logger)
+            raise together.JSONError(e, http_status=response.status_code)
         return response_json
 
-    def streaming_inference(self, prompt: str) -> str:
+    @classmethod
+    def create_streaming(
+        self,
+        prompt: str,
+        model: Optional[str] = "",
+        max_tokens: Optional[int] = 128,
+        stop: Optional[str] = None,
+        temperature: Optional[float] = 0.7,
+        top_p: Optional[float] = 0.7,
+        top_k: Optional[int] = 50,
+        repetition_penalty: Optional[float] = None,
+    ) -> Iterator[str]:
+        """
+        Prints streaming responses and returns the completed text.
+        """
+
+        if model == "":
+            model = together.default_text_model
+
         parameter_payload = {
-            "model": self.model,
+            "model": model,
             "prompt": prompt,
-            "top_p": self.top_p,
-            "top_k": self.top_k,
-            "temperature": self.temperature,
-            "max_tokens": self.max_tokens,
-            "stop": self.stop,
-            "repetition_penalty": self.repetition_penalty,
-            "logprobs": self.logprobs,
+            "top_p": top_p,
+            "top_k": top_k,
+            "temperature": temperature,
+            "max_tokens": max_tokens,
+            "stop": stop,
+            "repetition_penalty": repetition_penalty,
             "stream_tokens": True,
         }
         # HTTP headers for authorization
         headers = {
-            "Authorization": f"Bearer {self.together_api_key}",
+            "Authorization": f"Bearer {together.api_key}",
             "Content-Type": "application/json",
+            "User-Agent": together.user_agent,
         }
 
         # send request
         try:
             response = requests.post(
-                self.endpoint_url,
+                together.api_base_complete,
                 headers=headers,
                 json=parameter_payload,
                 stream=True,
             )
         except requests.exceptions.RequestException as e:
-            self.logger.critical(f"Response error raised: {e}")
-            exit_1(self.logger)
+            logger.critical(f"Response error raised: {e}")
+            raise together.ResponseError(e)
 
         if response.status_code == 200:
             output = ""
             client = sseclient.SSEClient(response)
             for event in client.events():
                 if event.data != "[DONE]":
                     text = json.loads(event.data)["choices"][0]["text"]
                     output += text
-                    print(text, end="", flush=True),
-            print("\n")
+                    yield text
         elif response.status_code == 429:
-            self.logger.critical(
-                f"No running instances for {self.model}. You can start an instance by navigating to the Together Playground at api.together.xyz"
+            logger.critical(
+                f"No running instances for {model}. You can start an instance by navigating to the Together Playground at api.together.ai"
             )
-            exit_1(self.logger)
+            raise together.InstanceError(model=model)
         else:
-            self.logger.critical(
+            logger.critical(
                 f"Unknown error raised.\nResponse status code = {response.status_code}"
             )
-            exit_1(self.logger)
-        return output
+            response.raise_for_status()
+            raise together.ResponseError(http_status=response.status_code)
```

### Comparing `together-0.0.9/src/together/cli/cli.py` & `together-0.1.1/src/together/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 #! python
 import argparse
 
-from together.commands import api, chat, files, finetune, inference
-from together.utils.utils import get_logger
+import together
+from together import get_logger
+from together.commands import chat, complete, files, finetune, image, models
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
-        description="CLI client for Together API",
+        description="Together Python Library",
         prog="together",
     )
 
     parser.add_argument(
         "--endpoint",
         "-e",
         help="[Optional] Together API Endpoint URL",
         type=str,
         required=False,
         default=None,
     )
 
-    base_subparser = argparse.ArgumentParser(add_help=False)
-    base_subparser.add_argument(
+    parser.add_argument(
         "--log",
-        default="WARNING",
+        default=together.log_level,
         choices=["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"],
         type=str,
         help="Set logging level. Defaults to WARNING. DEBUG will show all logs.",
         required=False,
     )
 
     subparser = parser.add_subparsers(dest="base")
 
-    api.add_parser(subparser, parents=[base_subparser])
-    inference.add_parser(subparser, parents=[base_subparser])
-    finetune.add_parser(subparser, parents=[base_subparser])
-    files.add_parser(subparser, parents=[base_subparser])
-    chat.add_parser(subparser, parents=[base_subparser])
+    models.add_parser(subparser)
+    chat.add_parser(subparser)
+    complete.add_parser(subparser)
+    image.add_parser(subparser)
+    files.add_parser(subparser)
+    finetune.add_parser(subparser)
 
     args = parser.parse_args()
 
     # Setup logging
     try:
         get_logger(__name__, log_level=args.log)
     except Exception:
-        get_logger(__name__, log_level="WARNING")
+        get_logger(__name__, log_level=together.log_level)
+
+    together.log_level = args.log
 
-    # try:
-    args.func(args)
-    # except AttributeError as e:
-    #    # print error, but ignore if `together` is run.
-    ##    if str(e) != "'Namespace' object has no attribute 'func'":
-    #        logger.critical(f"Error raised: {e}")
-    #        exit_1(logger)
-    #    parser.print_help()
+    try:
+        args.func(args)
+    except AttributeError as e:
+        # print error, but ignore if `together` is run.
+        if str(e) != "'Namespace' object has no attribute 'func'":
+            raise together.AttributeError(e)
+        parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `together-0.0.9/src/together/commands/files.py` & `together-0.1.1/src/together/commands/files.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,111 @@
 from __future__ import annotations
 
 import argparse
 import json
-from typing import List
 
-from together.files import Files
+from together import Files, extract_time
 
 
-def add_parser(
-    subparsers: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def add_parser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     COMMAND_NAME = "files"
     parser = subparsers.add_parser(COMMAND_NAME)
 
     child_parsers = parser.add_subparsers(required=True)
 
-    _add_list(child_parsers, parents=parents)
-    _add_upload(child_parsers, parents=parents)
-    _add_delete(child_parsers, parents=parents)
-    _add_retrieve(child_parsers, parents=parents)
-    _add_retrieve_content(child_parsers, parents=parents)
+    _add_list(child_parsers)
+    _add_upload(child_parsers)
+    _add_delete(child_parsers)
+    _add_retrieve(child_parsers)
+    _add_retrieve_content(child_parsers)
 
 
-def _add_list(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    list_parser = parser.add_parser("list", parents=parents)
-    list_parser.set_defaults(func=_run_list)
+def _add_list(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    subparser = parser.add_parser("list")
+    subparser.set_defaults(func=_run_list)
 
 
-def _add_upload(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    upload_file_parser = parser.add_parser("upload", parents=parents)
-    upload_file_parser.add_argument(
+def _add_upload(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    subparser = parser.add_parser("upload")
+    subparser.add_argument(
         "file",
         metavar="FILENAME",
         help="Local file to upload",
         type=str,
     )
-    upload_file_parser.set_defaults(func=_run_upload)
+    subparser.set_defaults(func=_run_upload)
 
 
-def _add_delete(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    delete_file_parser = parser.add_parser("delete", parents=parents)
-    delete_file_parser.add_argument(
+def _add_delete(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    subparser = parser.add_parser("delete")
+    subparser.add_argument(
         "file_id",
         metavar="FILE-ID",
         help="File ID of remote file",
         type=str,
     )
-    delete_file_parser.set_defaults(func=_run_delete)
+    subparser.set_defaults(func=_run_delete)
 
 
-def _add_retrieve(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    retrieve_file_parser = parser.add_parser("retrieve", parents=parents)
-    retrieve_file_parser.add_argument(
+def _add_retrieve(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    subparser = parser.add_parser("retrieve")
+    subparser.add_argument(
         "file_id",
         metavar="FILE-ID",
         help="File ID of remote file",
         type=str,
     )
-    retrieve_file_parser.set_defaults(func=_run_retrieve)
+    subparser.set_defaults(func=_run_retrieve)
 
 
 def _add_retrieve_content(
     parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
 ) -> None:
-    retrieve_file_content_parser = parser.add_parser(
-        "retrieve-content", parents=parents
-    )
-    retrieve_file_content_parser.add_argument(
+    subparser = parser.add_parser("retrieve-content")
+    subparser.add_argument(
         "file_id",
         metavar="FILE-ID",
         help="File ID of remote file",
         type=str,
     )
-    retrieve_file_content_parser.add_argument(
+    subparser.add_argument(
         "--output",
         "-o",
         default=None,
-        metavar="OUT_FILENAME",
+        metavar="OUTPUT_FILE",
         help="Optional output filename. Defaults to remote filename.",
         type=str,
         required=False,
     )
 
-    retrieve_file_content_parser.set_defaults(func=_run_retrieve_content)
+    subparser.set_defaults(func=_run_retrieve_content)
 
 
 def _run_list(args: argparse.Namespace) -> None:
-    files = Files(args.endpoint, log_level=args.log)
-    response = files.list_files()
+    files = Files()
+    response = files.list()
+    response["data"].sort(key=extract_time)
     print(json.dumps(response, indent=4))
 
 
 def _run_upload(args: argparse.Namespace) -> None:
-    files = Files(args.endpoint, log_level=args.log)
-    response = files.upload_file(args.file)
+    files = Files()
+    response = files.upload(args.file)
     print(json.dumps(response, indent=4))
 
 
 def _run_delete(args: argparse.Namespace) -> None:
-    files = Files(args.endpoint, log_level=args.log)
-    response = files.delete_file(args.file_id)
+    files = Files()
+    response = files.delete(args.file_id)
     print(json.dumps(response, indent=4))
 
 
 def _run_retrieve(args: argparse.Namespace) -> None:
-    files = Files(args.endpoint, log_level=args.log)
-    response = files.retrieve_file(args.file_id)
+    files = Files()
+    response = files.retrieve(args.file_id)
     print(json.dumps(response, indent=4))
 
 
 def _run_retrieve_content(args: argparse.Namespace) -> None:
-    files = Files(args.endpoint, log_level=args.log)
-    output = files.retrieve_file_content(args.file_id, args.output)
+    files = Files()
+    output = files.retrieve_content(args.file_id, args.output)
     print(output)
```

### Comparing `together-0.0.9/src/together/commands/finetune.py` & `together-0.1.1/src/together/commands/finetune.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,211 +1,184 @@
 from __future__ import annotations
 
 import argparse
 import json
-from typing import Any, Dict, List
 
-from together.finetune import Finetune
+from together import Finetune, extract_time
 
 
-def extract_time(json_obj: Dict[str, Any]) -> int:
-    try:
-        return int(json_obj["updated_at"])
-    except KeyError:
-        return 0
-
-
-def add_parser(
-    subparsers: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def add_parser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     COMMAND_NAME = "finetune"
     parser = subparsers.add_parser(COMMAND_NAME)
 
     child_parsers = parser.add_subparsers(required=True)
 
-    _add_create(child_parsers, parents=parents)
-    _add_list(child_parsers, parents=parents)
-    _add_retrieve(child_parsers, parents=parents)
-    _add_list_events(child_parsers, parents=parents)
-    _add_cancel(child_parsers, parents=parents)
-    _add_download(child_parsers, parents=parents)
-    _add_status(child_parsers, parents=parents)
-    _add_checkpoints(child_parsers, parents=parents)
+    _add_create(child_parsers)
+    _add_list(child_parsers)
+    _add_retrieve(child_parsers)
+    _add_list_events(child_parsers)
+    _add_cancel(child_parsers)
+    _add_download(child_parsers)
+    _add_status(child_parsers)
+    _add_checkpoints(child_parsers)
     # _add_delete_model(child_parsers)
 
 
-def _add_create(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def _add_create(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     # Create_finetune
-    create_finetune_parser = parser.add_parser("create", parents=parents)
-    create_finetune_parser.add_argument(
+    subparser = parser.add_parser("create")
+    subparser.add_argument(
         "--training-file",
         "-t",
         metavar="FILE-ID",
         help="File-ID of an uploaded file that contains training data.",
         required=True,
         type=str,
     )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--validation-file",
     #     "-v",
     #     default=None,
     #     help="The ID of an uploaded file that contains validation data.",
     #     type=str,
     # )
-    create_finetune_parser.add_argument(
+    subparser.add_argument(
         "--model",
         "-m",
         metavar="MODEL",
         default=None,
         help="The name of the base model to fine-tune. Default='togethercomputer/RedPajama-INCITE-7B-Chat'.",
         type=str,
     )
-    create_finetune_parser.add_argument(
+    subparser.add_argument(
         "--n-epochs",
         "-ne",
         metavar="EPOCHS",
         default=4,
         help="The number of epochs to train the model for. Default=4",
         type=int,
     )
-    create_finetune_parser.add_argument(
+    subparser.add_argument(
         "--batch-size",
         "-b",
         metavar="BATCH_SIZE",
         default=32,
         help="The batch size to use for training. Default=32",
         type=int,
     )
-    create_finetune_parser.add_argument(
+    subparser.add_argument(
         "--learning-rate",
         "-lr",
         metavar="LEARNING_RATE",
         default=0.00001,
         help="The learning rate multiplier to use for training. Default=0.00001",
         type=float,
     )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--warmup-steps",
     #     "-ws",
     #     default=0,
     #     help="Warmup steps",
     #     type=int,
     # )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--train-warmup-steps",
     #     "-tws",
     #     default=0,
     #     help="Train warmup steps",
     #     type=int,
     # )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--sequence-length",
     #     "-sl",
     #     default=2048,
     #     help="Max sequence length",
     #     type=int,
     # )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--seed",
     #     default=42,
     #     help="Training seed",
     #     type=int,
     # )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--fp32",
     #     help="Enable FP32 training. Defaults to false (FP16 training).",
     #     default=False,
     #     action="store_true",
     # )
-    # create_finetune_parser.add_argument(
+    # subparser.add_argument(
     #     "--checkpoint-steps",
     #     "-b",
     #     default=0,
     #     help="Number of steps between each checkpoint. Defaults to 0 = checkpoints per epoch.",
     #     type=int,
     # )
-    create_finetune_parser.add_argument(
+    subparser.add_argument(
         "--suffix",
         "-s",
         metavar="SUFFIX",
         default=None,
         help="Up to 40 characters that will be added to your fine-tuned model name.",
         type=str,
     )
-    create_finetune_parser.set_defaults(func=_run_create)
+    subparser.set_defaults(func=_run_create)
 
     # End of create_finetune
 
 
-def _add_list(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def _add_list(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     # List_Finetune
-    list_parser = parser.add_parser("list", parents=parents)
+    list_parser = parser.add_parser("list")
     list_parser.set_defaults(func=_run_list)
 
 
-def _add_retrieve(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    retrieve_finetune_parser = parser.add_parser("retrieve", parents=parents)
+def _add_retrieve(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    retrieve_finetune_parser = parser.add_parser("retrieve")
     retrieve_finetune_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
     retrieve_finetune_parser.set_defaults(func=_run_retrieve)
 
 
-def _add_cancel(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def _add_cancel(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     # Cancel Finetune
-    cancel_finetune_parser = parser.add_parser("cancel", parents=parents)
+    cancel_finetune_parser = parser.add_parser("cancel")
     cancel_finetune_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
     cancel_finetune_parser.set_defaults(func=_run_cancel)
 
 
 def _add_list_events(
     parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
 ) -> None:
     # List finetune events
-    list_finetune_events_parser = parser.add_parser("list-events", parents=parents)
+    list_finetune_events_parser = parser.add_parser("list-events")
     list_finetune_events_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
     list_finetune_events_parser.set_defaults(func=_run_list_events)
 
 
-def _add_download(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def _add_download(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     # List finetune events
-    download_parser = parser.add_parser("download", parents=parents)
+    download_parser = parser.add_parser("download")
     download_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
@@ -214,47 +187,43 @@
         "-o",
         metavar="FILENAME",
         default=None,
         help="Output filename. Defaults to remote name.",
         type=str,
         required=False,
     )
-    # download_parser.add_argument(
-    #     "--checkpoint-num",
-    #     "-n",
-    #     default=-1,
-    #     help="Checkpoint number. Defaults to the latest checkpoint = -1.",
-    #     type=int,
-    #     required=False,
-    # )
+    download_parser.add_argument(
+        "--checkpoint-step",
+        "-s",
+        default=-1,
+        help="Checkpoint step to download. Defaults to the latest checkpoint = -1.",
+        type=int,
+        required=False,
+    )
     download_parser.set_defaults(func=_run_download)
 
 
-def _add_status(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
+def _add_status(parser: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     # List finetune events
-    status_parser = parser.add_parser("status", parents=parents)
+    status_parser = parser.add_parser("status")
     status_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
     status_parser.set_defaults(func=_run_status)
 
 
 def _add_checkpoints(
     parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
 ) -> None:
     # List finetune events
-    checkpoint_parser = parser.add_parser("checkpoints", parents=parents)
+    checkpoint_parser = parser.add_parser("checkpoints")
     checkpoint_parser.add_argument(
         "fine_tune_id",
         metavar="FINETUNE-ID",
         default=None,
         help="Fine-tuning ID",
         type=str,
     )
@@ -274,17 +243,17 @@
 #         type=str,
 #         required=True,
 #     )
 #     delete_finetune_model_parser.set_defaults(func=_run_delete_model)
 
 
 def _run_create(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
+    finetune = Finetune()
 
-    response = finetune.create_finetune(
+    response = finetune.create(
         training_file=args.training_file,  # training file_id
         # validation_file=args.validation_file,  # validation file_id
         model=args.model,
         n_epochs=args.n_epochs,
         batch_size=args.batch_size,
         learning_rate=args.learning_rate,
         # warmup_steps=args.warmup_steps,
@@ -296,55 +265,54 @@
         suffix=args.suffix,
     )
 
     print(json.dumps(response, indent=4))
 
 
 def _run_list(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
-    response = finetune.list_finetune()
+    finetune = Finetune()
+    response = finetune.list()
     for item in response["data"]:
         item.pop("events", None)
     response["data"].sort(key=extract_time)
     print(json.dumps(response, indent=4))
 
 
 def _run_retrieve(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
-    response = finetune.retrieve_finetune(args.fine_tune_id)
+    finetune = Finetune()
+    response = finetune.retrieve(args.fine_tune_id)
     print(json.dumps(response, indent=4))
 
 
 def _run_cancel(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
-    response = finetune.cancel_finetune(args.fine_tune_id)
+    finetune = Finetune()
+    response = finetune.cancel(args.fine_tune_id)
     print(json.dumps(response, indent=4))
 
 
 def _run_list_events(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
-    response = finetune.list_finetune_events(args.fine_tune_id)
+    finetune = Finetune()
+    response = finetune.list_events(args.fine_tune_id)
     print(json.dumps(response, indent=4))
 
 
 def _run_download(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
-    args.checkpoint_num = -1  # hardcoded until enabled in remote
-    response = finetune.download(args.fine_tune_id, args.output, args.checkpoint_num)
+    finetune = Finetune()
+    response = finetune.download(args.fine_tune_id, args.output, args.checkpoint_step)
     print(response)
 
 
 def _run_status(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
+    finetune = Finetune()
     response = finetune.get_job_status(args.fine_tune_id)
     print(response)
 
 
 def _run_checkpoint(args: argparse.Namespace) -> None:
-    finetune = Finetune(args.endpoint, log_level=args.log)
+    finetune = Finetune()
     checkpoints = finetune.get_checkpoints(args.fine_tune_id)
     print(json.dumps(checkpoints, indent=4))
     print(f"\n{len(checkpoints)} checkpoints found")
 
 
 # def _run_delete_model(args: argparse.Namespace) -> None:
 #     finetune = Finetune(args.endpoint)
```

### Comparing `together-0.0.9/src/together/utils/conversation.py` & `together-0.1.1/src/together/utils/conversation.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,47 +14,47 @@
     for word in MEANINGLESS_WORDS:
         response = response.replace(word, "")
     response = response.strip("\n")
     return response
 
 
 class Conversation:
-    def __init__(self, human_id: str, bot_id: str) -> None:
+    def __init__(self, prompt_id: str, response_id: str) -> None:
         cur_date = time.strftime("%Y-%m-%d")
         cur_time = time.strftime("%H:%M:%S %p %Z")
 
-        self._human_id = human_id
-        self._bot_id = bot_id
+        self._prompt_id = prompt_id
+        self._response_id = response_id
         self._prompt = PRE_PROMPT.format(cur_date, cur_time)
 
     def push_context_turn(self, context: str) -> None:
         # for now, context is represented as a human turn
-        self._prompt += f"{self._human_id}: {context}\n"
+        self._prompt += f"{self._prompt_id}: {context}\n"
 
     def push_human_turn(self, query: str) -> None:
-        self._prompt += f"{self._human_id}: {query}\n"
-        self._prompt += f"{self._bot_id}:"
+        self._prompt += f"{self._prompt_id}: {query}\n"
+        self._prompt += f"{self._response_id}:"
 
     def push_model_response(self, response: str) -> None:
-        # has_finished = self._human_id in response
-        bot_turn = response.split(f"{self._human_id}:")[0]
+        # has_finished = self._prompt_id in response
+        bot_turn = response.split(f"{self._prompt_id}:")[0]
         bot_turn = clean_response(bot_turn)
         # if it is truncated, then append "..." to the end of the response
         # if not has_finished:
         #    bot_turn += "..."
 
         self._prompt += f"{bot_turn}\n"
 
     def get_last_turn(self) -> str:
-        human_tag = f"{self._human_id}:"
-        bot_tag = f"{self._bot_id}:"
+        human_tag = f"{self._prompt_id}:"
+        bot_tag = f"{self._response_id}:"
         turns = re.split(f"({human_tag}|{bot_tag})\W?", self._prompt)
         return turns[-1]
 
     def get_raw_prompt(self) -> str:
         return self._prompt
 
     @classmethod
-    def from_raw_prompt(cls, human_id: str, bot_id: str, prompt: str):  # type: ignore
-        convo = Conversation(human_id, bot_id)
+    def from_raw_prompt(cls, prompt_id: str, response_id: str, prompt: str):  # type: ignore
+        convo = Conversation(prompt_id, response_id)
         convo._prompt = prompt
         return convo
```

### Comparing `together-0.0.9/.gitignore` & `together-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `together-0.0.9/LICENSE` & `together-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `together-0.0.9/pyproject.toml` & `together-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "together"
-version = "0.0.9"
+version = "0.1.1"
 authors = [
   { name="Together Computer", email="community@together.xyz" },
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
```

### Comparing `together-0.0.9/PKG-INFO` & `together-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 0.0.9
+Version: 0.1.1
 Summary: Python client for Together's Cloud Platform!
 Project-URL: Homepage, https://github.com/togethercomputer/together
 Project-URL: Bug Tracker, https://github.com/togethercomputer/together/issues
 Author-email: Together Computer <community@together.xyz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -219,25 +219,107 @@
 Requires-Dist: black~=23.1; extra == 'quality'
 Requires-Dist: mypy>=1.3.0; extra == 'quality'
 Requires-Dist: ruff<=0.0.259,>=0.0.241; extra == 'quality'
 Requires-Dist: types-requests>=2.31.0.1; extra == 'quality'
 Requires-Dist: types-tqdm>=4.65.0.0; extra == 'quality'
 Description-Content-Type: text/markdown
 
-Python client for Together's Cloud Platform
+The [Together Python Library](https://pypi.org/project/together/) is the official Python client for Together's API platform, providing a convenient way for interacting with the Together APIs and enables easy integration of the inference API with your applications.
 
-## Installation
-`pip install git+https://github.com/togethercomputer/together.git`
+# Installation
 
-OR
-1. Clone this repo
-2. `pip install -e .`
+To install Together CLI , simply run:
 
-Run `together --help` to see available commands
+```shell Shell
+pip install --upgrade together
+```
 
+# Usage
+
+The Python Library requires your Together API Key to be configured. This key can be found in your Account's settings on the Playground. Simply click on and navigate to Profile Button > Settings > API Keys.
+
+The API Key can be configured by either setting the `TOGETHER_API_KEY` environment variable, like this:
+
+```shell
+export TOGETHER_API_KEY=xxxxx
+```
+
+Or by setting `together.api_key`:
+
+```python
+import together
+together.api_key = "xxxxx"
+```
+
+> 🚧 You will need to start a model instance from the Playground before you can query it from the API
+
+Once you've started a model instance, you can start querying:
+
+```python
+import together
+
+# set your API key
+together.api_key = "xxxxx"
+
+# list available models and descriptons
+models = together.Models.list()
+
+# print the first model's name
+print(models[0]['name'])
+
+output = together.Complete.create("Space robots", model="togethercomputer/RedPajama-INCITE-7B-Base")
+
+# print generated text
+print(output['output']['choices'][0]['text'])
+```
+
+## Chat
+
+The `chat` command is a CLI-based chat application that can be used for back-and-forth conversations with models in a pre-defined format.
+
+Refer to the [Chat docs](https://docs.together.ai/docs/python-chat) on how to chat with your favorite models.
+
+## Complete
+
+The `complete` command can be used to inference with all the models available in the Together Playground. This is recommended for custom applications and raw queries. It provides all the functions you need to run inference on all the leading open-source models available with the Together API. You can use these functions by interacting with the command line utility from your terminal or for usage in your custom Python applications.
+
+Refer to the [Complete docs](https://docs.together.ai/docs/python-complete) on how you can query these models.
+
+## Image
+
+The `image` command can be used to generate images from the leading open-source image generation models available with the Together API. You can use these functions by interacting with the command line utility from your terminal or for usage in your custom Python applications.
+
+Refer to the [Image docs](https://docs.together.ai/docs/python-image) on how you can generate images.
+
+## Files
+
+Files are used for uploading training and validation datasets that are used for [fine-tuning](https://docs.together.ai/docs/python-fine-tuning).
+
+Refer to the [Files docs](https://docs.together.ai/docs/python-files) on the correct way to prepare your files and managing them.
+
+## Fine-tuning
+
+Run and manage your fine-tuning jobs, enabling you to tune all model layers, control hyper-parameters, download the weights and checkpoints.
+
+Refer to the [Fine-tuning docs](https://docs.together.ai/docs/python-fine-tuning) on how to get started.
+
+# Command-line interface
+
+All the above commands are also available through a CLI:
+
+```shell
+# list commands
+together --help
+
+# list available models
+together models list
+
+# create completion
+together complete "Space robots" -m togethercomputer/RedPajama-INCITE-7B-Base
+```
 ## Contributing
 1. Clone the repo and make your changes
 2. Run `pip install together['quality']`
 3. From the root of the repo, run
     - `black .`
     - `ruff .`
       - And if necessary, `ruff . --fix`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

