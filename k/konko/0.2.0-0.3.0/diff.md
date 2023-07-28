# Comparing `tmp/konko-0.2.0.tar.gz` & `tmp/konko-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.2.0.tar", max compression
+gzip compressed data, was "konko-0.3.0.tar", max compression
```

## Comparing `konko-0.2.0.tar` & `konko-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       70 2023-07-21 02:21:54.288970 konko-0.2.0/README.md
--rw-r--r--   0        0        0      738 2023-07-21 02:34:10.654671 konko-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       95 2023-07-19 00:21:58.815710 konko-0.2.0/src/konko/__init__.py
--rw-r--r--   0        0        0      271 2023-07-19 00:58:56.301196 konko-0.2.0/src/konko/app.py
--rw-r--r--   0        0        0     1887 2023-07-04 09:17:33.179238 konko-0.2.0/src/konko/evaluate.py
--rw-r--r--   0        0        0     5296 2023-07-21 02:13:06.267673 konko-0.2.0/src/konko/generate.py
--rw-r--r--   0        0        0     2020 2023-07-19 22:59:01.411920 konko-0.2.0/src/konko/models.py
--rw-r--r--   0        0        0        0 2023-07-04 09:17:33.179880 konko-0.2.0/src/konko/utils/__init__.py
--rw-r--r--   0        0        0       42 2023-07-04 16:31:25.646577 konko-0.2.0/src/konko/utils/constants.py
--rw-r--r--   0        0        0     1543 2023-07-16 00:13:06.904294 konko-0.2.0/src/konko/utils/logs.py
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 konko-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       69 2023-07-28 02:05:43.140409 konko-0.3.0/README.md
+-rw-r--r--   0        0        0      781 2023-07-28 13:30:01.518945 konko-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-07-28 02:25:11.693562 konko-0.3.0/src/konko/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-28 00:39:32.576415 konko-0.3.0/src/konko/app.py
+-rw-r--r--   0        0        0     1887 2023-07-04 09:17:33.179238 konko-0.3.0/src/konko/evaluate.py
+-rw-r--r--   0        0        0     5144 2023-07-28 13:21:30.566061 konko-0.3.0/src/konko/generate.py
+-rw-r--r--   0        0        0     3109 2023-07-28 02:26:15.872754 konko-0.3.0/src/konko/models.py
+-rw-r--r--   0        0        0        0 2023-07-04 09:17:33.179880 konko-0.3.0/src/konko/utils/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-26 11:54:54.315365 konko-0.3.0/src/konko/utils/constants.py
+-rw-r--r--   0        0        0     1362 2023-07-28 02:17:37.991856 konko-0.3.0/src/konko/utils/logs.py
+-rw-r--r--   0        0        0      378 2023-07-28 01:51:28.605708 konko-0.3.0/src/konko/utils/utils.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 konko-0.3.0/PKG-INFO
```

### Comparing `konko-0.2.0/pyproject.toml` & `konko-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "konko"
-version = "0.2.0"
+version = "0.3.0"
 description = "\"Konko AI Python SDK: A client library to interact with Konko AI's API. With this SDK, developers can integrate, evaluate, fine-tune, and deploy Large Language Models (LLMs) using Konko AI's fully-managed, SOC 2 compliant platform. Ideal for enterprise use-cases, it allows you to focus on building great products without worrying about infrastructure.\""
 authors = ["Konko AI"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 requests = "^2.31.0"
 fastapi = "^0.100.0"
 pydantic = "^2.0.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
 uvicorn = "^0.22.0"
+locust = "^2.15.1"
 
 [build-system]
 requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `konko-0.2.0/src/konko/evaluate.py` & `konko-0.3.0/src/konko/evaluate.py`

 * *Files identical despite different names*

### Comparing `konko-0.2.0/src/konko/generate.py` & `konko-0.3.0/src/konko/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import List, Optional, Dict, Union
 from fastapi import APIRouter, HTTPException, Body, Depends
 from pydantic import BaseModel, Field
 from konko.utils.constants import TIMEOUT
-from konko.utils.logs import BackendError, get_env_variable
+from konko.utils.logs import BackendError
+from konko.utils.utils import get_konko_url
 import requests
 import os
 import json
 from fastapi import Depends
 from fastapi.security.api_key import APIKeyHeader
 
 class GeneratePayload(BaseModel):
     prompt: List[str]
-    models: List[str]
+    model: List[str]
+    mode: str
     prompt_file: Optional[str]
     prompt_delimiter: Optional[str]
-    mode: str
 
 generate_router = APIRouter()
 
 api_key_header = APIKeyHeader(name="x-api-key", description="API key to authorize requests")
 
 def get_api_key() -> str:
     if "KONKO_TOKEN" in os.environ:
@@ -30,44 +31,44 @@
             status_code=403, detail="Could not validate credentials. API key should be in the 'x-api-key' header or the 'API_KEY' environment variable."
         )
 
 @generate_router.post("/text",
         response_model=List[Dict[str, Union[str, float, int]]],
         tags=["Generate"],
         summary="GenerateText",
-        description="This endpoint generates a response for a user-specified prompt(s), set of models.")
+        description="This endpoint generates a response for a user-specified prompt(s)")
 def generate_text_api(
         prompt: List[str] = Body(default=["Summarize the Foundation by Isaac Asimov"],
                                  description="The list of prompts for which to generate responses. Each prompt should be a separate string in the list.\n" \
-                                 "Suggested Example: Summarize the Foundation by Isaac Asimov",
-                                 examples=["Summarize the Foundation by Isaac Asimov"]),
-        models: List[str] = Body(default=["mosaicml/mpt-7b-chat"],
+                                 "Suggested Example: Summarize the Foundation by Isaac Asimov",),
+        model: List[str] = Body(default=["mosaicml/mpt-7b-instruct"],
                                  description="A single model to be used for generating responses. We plan to support multiple models in the near future.\n" \
-                                 "Suggested Example: mosaicml/mpt-7b-chat",
-                                 examples=["mosaicml/mpt-7b-chat"]),
+                                 "Suggested Example: mosaicml/mpt-7b-instruct",),
         mode: str = Body(default='batch', 
                          description="Defines the mode of operation. Current available option is 'batch'. We plan to support 'stream' in the near future.",
-                         examples=["batch"]),
+                         example=["batch"]),
         prompt_file: Optional[str] =  Body(default=None, 
                                           description="Optional file path to a file containing prompts. This is used as an alternative to specifying prompts in the 'prompt' field.",
-                                          examples=None),
+                                          example=None),
         prompt_delimiter: Optional[str] = Body(default=None, 
                                                description="If 'prompt_file' is specified, this defines the separator string that divides separate prompts in the file."),
         api_key: str = Depends(api_key_header)
     ):
-    models = [model.replace('/', '--') for model in models] 
-    baseUrl = get_env_variable('KONKO_URL')
-    headers = {"x-api-key": api_key}
 
+    model = [m.replace('/', '--') for m in model]
     if prompt_file:
         with open(prompt_file, "r") as f:
             prompt = f.read().split(prompt_delimiter)
-    path = '/generate/text/' 
+    
+    baseUrl = get_konko_url()
+    headers = {"x-api-key": api_key}
+    path = 'generate/text'
     url = f"{baseUrl}{path}"
-    payload = GeneratePayload(prompt=prompt, models=models, prompt_file=prompt_file, prompt_delimiter=prompt_delimiter, mode=mode)
+    payload = GeneratePayload(prompt=prompt, model=model, mode=mode, prompt_file=prompt_file, prompt_delimiter=prompt_delimiter)
+    print(payload)
     response = generate_request(url=url, headers=headers, payload=payload.dict(), stream=payload.mode == 'stream')
     return response
 
 def generate_request(url: str, headers: Dict, payload: Dict, stream: bool) -> List[Dict[str, Union[str, float, int]]]:
     response = requests.post(url, 
                              headers=headers, 
                              json=payload,
@@ -94,23 +95,23 @@
         elif isinstance(data, str):
             result = json.loads(data) 
         else:
             raise ValueError("Unexpected response format")
     return result
 
 def generate_text(prompt: Union[List[str], str], 
-                  model_ids: Union[List[str], str], 
+                  model_id: Union[List[str], str], 
                   mode: str = 'batch', 
                   prompt_file: Optional[str] = None, 
                   prompt_delimiter: Optional[str] = None):
     
     # If prompt is a string, convert it to a list
     if isinstance(prompt, str):
         prompt = [prompt]
     
-    # If model_ids is a string, convert it to a list
-    if isinstance(model_ids, str):
-        model_ids = [model_ids]
+    # If model_id is a string, convert it to a list
+    if isinstance(model_id, str):
+        model_id = [model_id]
 
     api_key = get_api_key()
-    return generate_text_api(prompt, model_ids, mode, prompt_file, prompt_delimiter, api_key)
+    return generate_text_api(prompt, model_id, mode, prompt_file, prompt_delimiter, api_key)
```

### Comparing `konko-0.2.0/src/konko/models.py` & `konko-0.3.0/src/konko/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-from typing import List
+from typing import List, Any
 from fastapi.security import APIKeyHeader
 from pydantic import BaseModel, Field
-from konko.utils.logs import get_request_json, get_env_variable
+from konko.utils.logs import get_request_json
+from konko.utils.utils import get_konko_url
+from konko.utils.constants import TIMEOUT
 from fastapi import APIRouter, HTTPException, Depends
 import os, json
 
 models_router = APIRouter()
 
 class Model(BaseModel):
+    id: str = Field(default=None, description="Unique model ID")
     name: str = Field(default=None, description="Name of the model")
     provider: str = Field(default=None, description="Provider of the model")
-    id: str = Field(default=None, description="Unique model ID")
+
+class ModelMetadata(BaseModel):
+    metadata: Any # TODO: Define the actual shape of the metadata object to make it more pertinent to users
 
 api_key_header = APIKeyHeader(name="x-api-key", description="API key to authorize requests")
 
 def get_api_key() -> str:
     if "KONKO_TOKEN" in os.environ:
         return os.environ["KONKO_TOKEN"]
     elif api_key_header:
@@ -28,26 +33,50 @@
          response_model=List[Model], 
          tags=["Models"],
          summary="RunningModels",
          description="This endpoint retrieves a list of models for all the models running on the Konko instance.",
          )
 def running_api(api_key: str = Depends(api_key_header)):
 
-    baseUrl = get_env_variable('KONKO_URL')
-    path = "/models/running/"
+    baseUrl = get_konko_url()
+    path = "models/running/"
     url = f"{baseUrl}{path}"
     headers = {"x-api-key": api_key}
     results = get_request_json(url, headers=headers)
 
     # TODO: Also grab model metadata from the Konko instance.
     # such as decoding parameters, quantization, acceleration, etc.
     # TODO: Once we have generate and embedding, do we keep one model endpoint 
     # or do we have separate model endpoints for each? /generate/model
     # /embedding/models /models /generate /embeddings
 
     # Convert each result dictionary into a Model object
     model_objects = [Model(**result) for result in results]
     return model_objects
 
+@models_router.get("/running/{model_id}",
+                   response_model=ModelMetadata,
+                   tags=["Models"],
+                   summary="ModelMetadata",
+                   description="This endpoint retrieves metadata for a specific model running on the Konko instance.",
+                    )
+def running_model_metadata_api(model_id: str, api_key: str = Depends(api_key_header)):
+
+    baseUrl = get_konko_url()
+    path = f"models/running/{model_id}"
+    url = f"{baseUrl}{path}"
+    headers = {"x-api-key": api_key}
+    model_metadata = get_request_json(url, headers=headers)
+
+    if not model_metadata:
+        raise HTTPException(status_code=404, detail="Model not found")
+
+    return model_metadata
+
 def running():
     api_key = get_api_key()
     return running_api(api_key)
+
+def running_model_metadata(model_id):
+    model_id = model_id.replace('/', '--')
+    api_key = get_api_key()
+    return running_model_metadata_api(model_id, api_key)
```

### Comparing `konko-0.2.0/PKG-INFO` & `konko-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konko
-Version: 0.2.0
+Version: 0.3.0
 Summary: "Konko AI Python SDK: A client library to interact with Konko AI's API. With this SDK, developers can integrate, evaluate, fine-tune, and deploy Large Language Models (LLMs) using Konko AI's fully-managed, SOC 2 compliant platform. Ideal for enterprise use-cases, it allows you to focus on building great products without worrying about infrastructure."
 License: Proprietary
 Author: Konko AI
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -15,8 +15,7 @@
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # For documentation please visit 
 [Link Text](https://docs.konko.ai/)
-
```

