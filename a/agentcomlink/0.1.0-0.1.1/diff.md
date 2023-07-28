# Comparing `tmp/agentcomlink-0.1.0.tar.gz` & `tmp/agentcomlink-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcomlink-0.1.0.tar", last modified: Fri Jul 28 05:25:28 2023, max compression
+gzip compressed data, was "agentcomlink-0.1.1.tar", last modified: Fri Jul 28 07:29:48 2023, max compression
```

## Comparing `agentcomlink-0.1.0.tar` & `agentcomlink-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:25:28.851552 agentcomlink-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 05:25:28.851552 agentcomlink-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:25:28.851552 agentcomlink-0.1.0/agentcomlink/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/agentcomlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/agentcomlink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/agentcomlink/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/agentcomlink/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:25:28.851552 agentcomlink-0.1.0/agentcomlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 05:25:28.000000 agentcomlink-0.1.0/agentcomlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 05:25:28.000000 agentcomlink-0.1.0/agentcomlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:25:28.000000 agentcomlink-0.1.0/agentcomlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 05:25:28.000000 agentcomlink-0.1.0/agentcomlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 05:25:28.000000 agentcomlink-0.1.0/agentcomlink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:25:28.851552 agentcomlink-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-28 05:25:18.000000 agentcomlink-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:29:48.462766 agentcomlink-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 07:29:48.462766 agentcomlink-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:29:48.462766 agentcomlink-0.1.1/agentcomlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/agentcomlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/agentcomlink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/agentcomlink/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/agentcomlink/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:29:48.462766 agentcomlink-0.1.1/agentcomlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-28 07:29:48.000000 agentcomlink-0.1.1/agentcomlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 07:29:48.000000 agentcomlink-0.1.1/agentcomlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:29:48.000000 agentcomlink-0.1.1/agentcomlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 07:29:48.000000 agentcomlink-0.1.1/agentcomlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 07:29:48.000000 agentcomlink-0.1.1/agentcomlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 07:29:48.462766 agentcomlink-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-28 07:29:38.000000 agentcomlink-0.1.1/setup.py
```

### Comparing `agentcomlink-0.1.0/LICENSE` & `agentcomlink-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.0/PKG-INFO` & `agentcomlink-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.0/README.md` & `agentcomlink-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.0/agentcomlink/files.py` & `agentcomlink-0.1.1/agentcomlink/files.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.0/agentcomlink/server.py` & `agentcomlink-0.1.1/agentcomlink/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,107 +2,123 @@
 
 from fastapi import APIRouter, FastAPI, File, Form, HTTPException, UploadFile
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 
 from agentcomlink.constants import app, storage_path
 from agentcomlink.files import check_files, get_storage_path, set_storage_path
+from fastapi import FastAPI, WebSocket, WebSocketDisconnect
+from fastapi.staticfiles import StaticFiles
+from fastapi.responses import FileResponse
 
 router = APIRouter()
+app = FastAPI()
+
 
 class FilePath(BaseModel):
     path: str
 
+
 def get_server():
     global app
     return app
 
+
 def start_server(storage_path=None, port=8000):
     global app
     if storage_path:
         set_storage_path(storage_path)
     check_files()
-    app = FastAPI()
     app.include_router(router)
     app.mount(
         "/", StaticFiles(directory="static", html=True), name="static"
     )  # enable HTML support
     app.mount(
         "/files", StaticFiles(directory=get_storage_path(), html=False), name="files"
     )
     if port:
         os.environ["PORT"] = str(port)
     return app
 
+
 def stop_server():
     global app
     app = None
 
-from fastapi import FastAPI, WebSocket, WebSocketDisconnect
-from fastapi.staticfiles import StaticFiles
-from fastapi.responses import FileResponse
-from typing import List
 
-app = FastAPI()
 ws: WebSocket
 
-# Define a chat storage
-chats: List[str] = []
+handlers = []
+
 
 @app.get("/")
 async def get():
     return FileResponse("static/index.html")
 
+
 async def send_message(message):
-    print("sending message", message)
     await ws.send_text(message)
 
+
+def register_message_handler(handler):
+    global handlers
+    handlers.append(handler)
+
+
+def unregister_message_handler(handler):
+    global handlers
+    handlers.remove(handler)
+
+
 @app.websocket("/ws")
 async def websocket_endpoint(websocket: WebSocket):
     global ws
     ws = websocket
     await websocket.accept()
-
     try:
         while True:
             data = await websocket.receive_text()
-            print(f"Received message: {data}")
-            await send_message(data)
-            chats.append(data)
+            for handler in handlers:
+                handler(data)
     except WebSocketDisconnect:
         ws = None
 
+
 @router.post("/file/")
 async def http_add_file(path: str = Form(...), file: UploadFile = File(...)):
     check_files()
     with open(os.path.join(storage_path, path), "wb") as f:
         f.write(await file.read())
     return {"message": "File created"}
 
+
 @router.delete("/file/{path}")
 def http_remove_file(path: str):
     check_files()
     try:
         os.remove(os.path.join(storage_path, path))
         return {"message": "File removed"}
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
+
 @router.put("/file/")
 async def http_update_file(path: str = Form(...), file: UploadFile = File(...)):
     check_files()
     with open(os.path.join(storage_path, path), "wb") as f:
         f.write(await file.read())
     return {"message": "File updated"}
 
+
 @router.get("/files/")
 def http_list_files(path: str = "."):
     check_files()
     return {"files": os.listdir(os.path.join(storage_path, path))}
 
+
 @router.get("/file/{path}")
 def http_get_file(path: str):
     check_files()
     try:
         return FileResponse(os.path.join(storage_path, path))
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
```

### Comparing `agentcomlink-0.1.0/agentcomlink.egg-info/PKG-INFO` & `agentcomlink-0.1.1/agentcomlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.0/setup.py` & `agentcomlink-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentcomlink',
-    version='0.1.0',
+    version='0.1.1',
     description='Simple chat, debug and file management panel for agents',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentcomlink',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

