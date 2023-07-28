# Comparing `tmp/michina-0.2.0.tar.gz` & `tmp/michina-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michina-0.2.0.tar", max compression
+gzip compressed data, was "michina-0.2.1.tar", max compression
```

## Comparing `michina-0.2.0.tar` & `michina-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      185 2023-07-25 17:25:21.973986 michina-0.2.0/README.md
--rw-r--r--   0        0        0      122 2023-07-25 00:01:47.195488 michina-0.2.0/michina/checks/__init__.py
--rw-r--r--   0        0        0      648 2023-07-26 23:54:50.190542 michina-0.2.0/michina/checks/base_check.py
--rw-r--r--   0        0        0      183 2023-07-26 23:55:55.785232 michina-0.2.0/michina/checks/consistency/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-26 23:56:41.218881 michina-0.2.0/michina/checks/consistency/check.py
--rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.2.0/michina/checks/consistency/prompt.py
--rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.2.0/michina/checks/tone/__init__.py
--rw-r--r--   0        0        0     1419 2023-07-26 23:56:44.395259 michina-0.2.0/michina/checks/tone/check.py
--rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.2.0/michina/checks/tone/prompt.py
--rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.2.0/michina/exceptions/exceptions.py
--rw-r--r--   0        0        0      469 2023-07-27 00:01:25.349664 michina-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 michina-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1451 2023-07-27 00:07:32.206966 michina-0.2.1/README.md
+-rw-r--r--   0        0        0      114 2023-07-28 18:07:08.896265 michina-0.2.1/michina/checks/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-28 18:47:36.725936 michina-0.2.1/michina/checks/base/check.py
+-rw-r--r--   0        0        0      183 2023-07-26 23:55:55.785232 michina-0.2.1/michina/checks/consistency/__init__.py
+-rw-r--r--   0        0        0     1801 2023-07-28 18:06:45.360237 michina-0.2.1/michina/checks/consistency/check.py
+-rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.2.1/michina/checks/consistency/prompt.py
+-rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.2.1/michina/checks/tone/__init__.py
+-rw-r--r--   0        0        0     1446 2023-07-28 18:07:00.434977 michina-0.2.1/michina/checks/tone/check.py
+-rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.2.1/michina/checks/tone/prompt.py
+-rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.2.1/michina/exceptions/exceptions.py
+-rw-r--r--   0        0        0      469 2023-07-28 19:11:01.925070 michina-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 michina-0.2.1/PKG-INFO
```

### Comparing `michina-0.2.0/michina/checks/base_check.py` & `michina-0.2.1/michina/checks/base/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from abc import ABC, abstractmethod
 from typing import Optional
-from pydantic import BaseModel, root_validator
+from pydantic import BaseModel
 from langchain.schema import BaseLanguageModel
 from langchain.chat_models import ChatOpenAI
 
 
 class LLMConfig(BaseModel):
     model: str
     temperature: Optional[float]
     openai_api_key: str
 
+class BaseCheckResponse(BaseModel):
+    input: BaseModel
+    reasoning: str
+    judgment: float
 
 class BaseCheck(BaseModel, ABC):
     config: LLMConfig = None
     llm: BaseLanguageModel = None
 
     def __init__(self, **data):
         super().__init__(**data)  # for pydantic to not yell
         self.llm = ChatOpenAI(**data)
 
     @abstractmethod
-    def check(cls, *args, **kwargs):
+    def check(cls, *args, **kwargs) -> BaseCheckResponse:
         """Checks the input and returns a response."""
```

### Comparing `michina-0.2.0/michina/checks/consistency/check.py` & `michina-0.2.1/michina/checks/consistency/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This is a module for the Michina test suite.
 """
-from michina.checks.base_check import BaseCheck
+from michina.checks.base.check import BaseCheck, BaseCheckResponse
 from michina.exceptions.exceptions import (
     InvalidTypeException,
     InvalidXMLException,
     LanguageModelException,
 )
 from michina.checks.consistency.prompt import CONSISTENCY_CHECK_TEMPLATE
 from langchain.chat_models import ChatOpenAI
@@ -19,15 +19,15 @@
 
 
 class ConsistencyCheckInput(BaseModel):
     message: str
     statement: str
 
 
-class ConsistencyCheckResponse(BaseModel):
+class ConsistencyCheckResponse(BaseCheckResponse):
     input: ConsistencyCheckInput
     reasoning: str
     judgment: float
 
 
 class ConsistencyCheck(BaseCheck):
     description: str = "Checks whether the message is consistent with the statement."
```

### Comparing `michina-0.2.0/michina/checks/consistency/prompt.py` & `michina-0.2.1/michina/checks/consistency/prompt.py`

 * *Files identical despite different names*

### Comparing `michina-0.2.0/michina/checks/tone/check.py` & `michina-0.2.1/michina/checks/tone/check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from michina.checks.base_check import BaseCheck
+from michina.checks.base.check import BaseCheck, BaseCheckResponse
 from michina.checks.tone.prompt import TONE_CHECK_TEMPLATE
 from michina.exceptions.exceptions import (
     InvalidTypeException,
     InvalidXMLException,
     LanguageModelException,
 )
 from pydantic import BaseModel
@@ -17,15 +17,15 @@
 
 
 class ToneCheckInput(BaseModel):
     message: str
     tone: str
 
 
-class ToneCheckReponse(BaseModel):
+class ToneCheckReponse(BaseCheckResponse):
     input: ToneCheckInput
     reasoning: str
     judgment: float
 
 
 class ToneCheck(BaseCheck):
     description: str = (
```

### Comparing `michina-0.2.0/michina/checks/tone/prompt.py` & `michina-0.2.1/michina/checks/tone/prompt.py`

 * *Files identical despite different names*

