# Comparing `tmp/nonebot_plugin_nagabus-0.2.4.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.5.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.4.tar` & `nonebot_plugin_nagabus-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.4/LICENSE
--rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     4040 2023-06-27 03:05:14.179567 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      997 2023-06-27 03:09:17.964805 nonebot_plugin_nagabus-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.4/README.md
--rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0      998 2023-07-28 15:04:21.945700 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     4050 2023-07-28 15:04:21.966695 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      996 2023-07-28 15:12:11.221793 nonebot_plugin_nagabus-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.5/README.md
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.4/LICENSE` & `nonebot_plugin_nagabus-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from nonebot import logger
-from nonebot_plugin_majsoul.paipu import get_downloader
+from nonebot_plugin_majsoul.paipu import download_paipu
 from sqlalchemy import select
 
 from ..data.mjs import MajsoulPaipuOrm
 from ..data.session import get_session
 from ..data.utils import insert
 
 
@@ -16,15 +16,15 @@
     res = (await sess.execute(stmt)).scalar_one_or_none()
 
     if res is not None:
         logger.opt(colors=True).info(f"Use cached majsoul paipu <y>{uuid}</y>")
         return json.loads(res.content)
 
     logger.opt(colors=True).info(f"Downloading majsoul paipu <y>{uuid}</y> ...")
-    data = await get_downloader().download(uuid)
+    data = await download_paipu(uuid)
 
     stmt = (insert(MajsoulPaipuOrm)
             .values(paipu_uuid=uuid, content=json.dumps(data))
             .on_conflict_do_nothing(index_elements=[MajsoulPaipuOrm.paipu_uuid]))
 
     await sess.execute(stmt)
     await sess.commit()
```

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     _HEADER = {
         "Cache-Control": "no-cache",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.35",
     }
 
     def __init__(self, cookies: Dict[str, str]):
         async def req_hook(request):
+            request.cookies = cookies
             logger.trace(f"Request: {request.method} {request.url} - Waiting for response")
 
         async def resp_hook(response):
             request = response.request
             logger.trace(f"Response: {request.method} {request.url} - Status {response.status_code}")
             response.raise_for_status()
 
         self.client: AsyncClient = AsyncClient(
             base_url=self._BASE_URL,
-            cookies=cookies,
             headers=self._HEADER,
             follow_redirects=True,
-            event_hooks={'request': [req_hook], 'response': [resp_hook]}
+            event_hooks={'request': [req_hook], 'response': [resp_hook]},
         )
 
     async def close(self):
         await self.client.aclose()
 
     async def order_report_list(self, year: int, month: int) -> OrderReportList:
         resp = await self.client.get(
```

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/naga/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.5/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/pyproject.toml` & `nonebot_plugin_nagabus-0.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = {extras = ["httpx"], version = "^2.0.0"}
-nonebot-adapter-onebot = "^2.2.3"
+nonebot-adapter-onebot = ">=2.2.3"
 nonebot-plugin-access-control = ">=0.5.1"
 nonebot-plugin-datastore = ">=0.6.3"
 nonebot-plugin-get-nickname = ">=0.1.0"
-nonebot-plugin-majsoul = ">=0.2.0.post4"
+nonebot-plugin-majsoul = ">=0.2.2"
 nonebot-plugin-session = ">=0.0.3"
-nonebot-plugin-send-anything-anywhere = "^0.2.4"
-typing-extensions = "^4.6.2"
-pydantic = "^1.10.8"
-monthdelta = "^0.9.1"
+nonebot-plugin-send-anything-anywhere = ">=0.2.4"
+typing-extensions = ">=4.6.2"
+pydantic = ">=1.10.8"
+monthdelta = ">=0.9.1"
 
 [tool.poetry.group.dev.dependencies]
 nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0" }
 nonebot-plugin-escape-url = "^0.1.0"
 nonebot-adapter-qqguild = "^0.2.2"
 
 [tool.nonebot]
```

### Comparing `nonebot_plugin_nagabus-0.2.4/README.md` & `nonebot_plugin_nagabus-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.4/PKG-INFO` & `nonebot_plugin_nagabus-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: monthdelta (>=0.9.1,<0.10.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: monthdelta (>=0.9.1)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
 Requires-Dist: nonebot-plugin-access-control (>=0.5.1)
 Requires-Dist: nonebot-plugin-datastore (>=0.6.3)
 Requires-Dist: nonebot-plugin-get-nickname (>=0.1.0)
-Requires-Dist: nonebot-plugin-majsoul (>=0.2.0.post4)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0)
+Requires-Dist: nonebot-plugin-majsoul (>=0.2.2)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4)
 Requires-Dist: nonebot-plugin-session (>=0.0.3)
 Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
+Requires-Dist: pydantic (>=1.10.8)
+Requires-Dist: typing-extensions (>=4.6.2)
 Description-Content-Type: text/markdown
 
 nonebot-plugin-nagabus
 ==========
 
 NAGA公交车。为群友提供NAGA拼车服务。
```

