# Comparing `tmp/alibabacloud_aiccs20230516-1.0.1.tar.gz` & `tmp/alibabacloud_aiccs20230516-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiccs20230516-1.0.1.tar", last modified: Tue Jul  4 13:12:45 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiccs20230516-1.0.2.tar", last modified: Fri Jul 28 03:58:18 2023, max compression
```

## Comparing `alibabacloud_aiccs20230516-1.0.1.tar` & `alibabacloud_aiccs20230516-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93024 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/client.py
--rw-r--r--   0 root         (0) root         (0)   205832 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-07-04 13:12:45.000000 alibabacloud_aiccs20230516-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93480 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/client.py
+-rw-r--r--   0 root         (0) root         (0)   207002 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 03:58:18.000000 alibabacloud_aiccs20230516-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-07-28 03:58:17.000000 alibabacloud_aiccs20230516-1.0.2/setup.py
```

### Comparing `alibabacloud_aiccs20230516-1.0.1/LICENSE` & `alibabacloud_aiccs20230516-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.1/PKG-INFO` & `alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_aiccs20230516
-Version: 1.0.1
+Name: alibabacloud-aiccs20230516
+Version: 1.0.2
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516-1.0.1/README-CN.md` & `alibabacloud_aiccs20230516-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.1/README.md` & `alibabacloud_aiccs20230516-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/client.py` & `alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
         if not UtilClient.is_unset(tmp_req.repeat_times):
             request.repeat_times_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.repeat_times, 'RepeatTimes', 'json')
         if not UtilClient.is_unset(tmp_req.send_sms_plan):
             request.send_sms_plan_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.send_sms_plan, 'SendSmsPlan', 'json')
         query = {}
         if not UtilClient.is_unset(request.call_time_list_shrink):
             query['CallTimeList'] = request.call_time_list_shrink
+        if not UtilClient.is_unset(request.callback_url):
+            query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.max_concurrency):
             query['MaxConcurrency'] = request.max_concurrency
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_sleep_val):
@@ -228,14 +230,16 @@
         if not UtilClient.is_unset(tmp_req.repeat_times):
             request.repeat_times_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.repeat_times, 'RepeatTimes', 'json')
         if not UtilClient.is_unset(tmp_req.send_sms_plan):
             request.send_sms_plan_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.send_sms_plan, 'SendSmsPlan', 'json')
         query = {}
         if not UtilClient.is_unset(request.call_time_list_shrink):
             query['CallTimeList'] = request.call_time_list_shrink
+        if not UtilClient.is_unset(request.callback_url):
+            query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.max_concurrency):
             query['MaxConcurrency'] = request.max_concurrency
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_sleep_val):
@@ -654,14 +658,16 @@
         if not UtilClient.is_unset(tmp_req.repeat_times):
             request.repeat_times_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.repeat_times, 'RepeatTimes', 'json')
         if not UtilClient.is_unset(tmp_req.send_sms_plan):
             request.send_sms_plan_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.send_sms_plan, 'SendSmsPlan', 'json')
         query = {}
         if not UtilClient.is_unset(request.call_time_list_shrink):
             query['CallTimeList'] = request.call_time_list_shrink
+        if not UtilClient.is_unset(request.callback_url):
+            query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.max_concurrency):
             query['MaxConcurrency'] = request.max_concurrency
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_sleep_val):
@@ -728,14 +734,16 @@
         if not UtilClient.is_unset(tmp_req.repeat_times):
             request.repeat_times_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.repeat_times, 'RepeatTimes', 'json')
         if not UtilClient.is_unset(tmp_req.send_sms_plan):
             request.send_sms_plan_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.send_sms_plan, 'SendSmsPlan', 'json')
         query = {}
         if not UtilClient.is_unset(request.call_time_list_shrink):
             query['CallTimeList'] = request.call_time_list_shrink
+        if not UtilClient.is_unset(request.callback_url):
+            query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.max_concurrency):
             query['MaxConcurrency'] = request.max_concurrency
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.play_sleep_val):
```

### Comparing `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516/models.py` & `alibabacloud_aiccs20230516-1.0.2/alibabacloud_aiccs20230516/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
     def __init__(
         self,
         intent_tags: List[str] = None,
         sms_template_id: int = None,
     ):
         # 意向标签
         self.intent_tags = intent_tags
-        # 重呼条件
+        # 短信模板ID
         self.sms_template_id = sms_template_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -317,14 +317,15 @@
         return self
 
 
 class AddTaskRequest(TeaModel):
     def __init__(
         self,
         call_time_list: List[AddTaskRequestCallTimeList] = None,
+        callback_url: str = None,
         max_concurrency: int = None,
         name: str = None,
         owner_id: int = None,
         play_sleep_val: int = None,
         play_times: int = None,
         recall_type: int = None,
         record_path: str = None,
@@ -338,14 +339,16 @@
         start_time: str = None,
         task_type: int = None,
         template_id: int = None,
         template_type: int = None,
     ):
         # 外呼时间
         self.call_time_list = call_time_list
+        # 回调地址
+        self.callback_url = callback_url
         # 并发数
         self.max_concurrency = max_concurrency
         # 任务名称
         self.name = name
         self.owner_id = owner_id
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val
@@ -392,14 +395,16 @@
             return _map
 
         result = dict()
         result['CallTimeList'] = []
         if self.call_time_list is not None:
             for k in self.call_time_list:
                 result['CallTimeList'].append(k.to_map() if k else None)
+        if self.callback_url is not None:
+            result['CallbackUrl'] = self.callback_url
         if self.max_concurrency is not None:
             result['MaxConcurrency'] = self.max_concurrency
         if self.name is not None:
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_sleep_val is not None:
@@ -439,14 +444,16 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.call_time_list = []
         if m.get('CallTimeList') is not None:
             for k in m.get('CallTimeList'):
                 temp_model = AddTaskRequestCallTimeList()
                 self.call_time_list.append(temp_model.from_map(k))
+        if m.get('CallbackUrl') is not None:
+            self.callback_url = m.get('CallbackUrl')
         if m.get('MaxConcurrency') is not None:
             self.max_concurrency = m.get('MaxConcurrency')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlaySleepVal') is not None:
@@ -485,14 +492,15 @@
         return self
 
 
 class AddTaskShrinkRequest(TeaModel):
     def __init__(
         self,
         call_time_list_shrink: str = None,
+        callback_url: str = None,
         max_concurrency: int = None,
         name: str = None,
         owner_id: int = None,
         play_sleep_val: int = None,
         play_times: int = None,
         recall_type: int = None,
         record_path: str = None,
@@ -506,14 +514,16 @@
         start_time: str = None,
         task_type: int = None,
         template_id: int = None,
         template_type: int = None,
     ):
         # 外呼时间
         self.call_time_list_shrink = call_time_list_shrink
+        # 回调地址
+        self.callback_url = callback_url
         # 并发数
         self.max_concurrency = max_concurrency
         # 任务名称
         self.name = name
         self.owner_id = owner_id
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val
@@ -551,14 +561,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.call_time_list_shrink is not None:
             result['CallTimeList'] = self.call_time_list_shrink
+        if self.callback_url is not None:
+            result['CallbackUrl'] = self.callback_url
         if self.max_concurrency is not None:
             result['MaxConcurrency'] = self.max_concurrency
         if self.name is not None:
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_sleep_val is not None:
@@ -593,14 +605,16 @@
             result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CallTimeList') is not None:
             self.call_time_list_shrink = m.get('CallTimeList')
+        if m.get('CallbackUrl') is not None:
+            self.callback_url = m.get('CallbackUrl')
         if m.get('MaxConcurrency') is not None:
             self.max_concurrency = m.get('MaxConcurrency')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlaySleepVal') is not None:
@@ -1852,14 +1866,15 @@
         return self
 
 
 class EditTaskRequest(TeaModel):
     def __init__(
         self,
         call_time_list: List[EditTaskRequestCallTimeList] = None,
+        callback_url: str = None,
         max_concurrency: int = None,
         name: str = None,
         owner_id: int = None,
         play_sleep_val: int = None,
         play_times: int = None,
         recall_type: int = None,
         record_path: str = None,
@@ -1873,14 +1888,16 @@
         status: int = None,
         task_id: int = None,
         template_id: int = None,
         template_type: int = None,
     ):
         # 外呼时间
         self.call_time_list = call_time_list
+        # 回调地址
+        self.callback_url = callback_url
         # 并发数
         self.max_concurrency = max_concurrency
         # 任务名称
         self.name = name
         self.owner_id = owner_id
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val
@@ -1927,14 +1944,16 @@
             return _map
 
         result = dict()
         result['CallTimeList'] = []
         if self.call_time_list is not None:
             for k in self.call_time_list:
                 result['CallTimeList'].append(k.to_map() if k else None)
+        if self.callback_url is not None:
+            result['CallbackUrl'] = self.callback_url
         if self.max_concurrency is not None:
             result['MaxConcurrency'] = self.max_concurrency
         if self.name is not None:
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_sleep_val is not None:
@@ -1974,14 +1993,16 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.call_time_list = []
         if m.get('CallTimeList') is not None:
             for k in m.get('CallTimeList'):
                 temp_model = EditTaskRequestCallTimeList()
                 self.call_time_list.append(temp_model.from_map(k))
+        if m.get('CallbackUrl') is not None:
+            self.callback_url = m.get('CallbackUrl')
         if m.get('MaxConcurrency') is not None:
             self.max_concurrency = m.get('MaxConcurrency')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlaySleepVal') is not None:
@@ -2020,14 +2041,15 @@
         return self
 
 
 class EditTaskShrinkRequest(TeaModel):
     def __init__(
         self,
         call_time_list_shrink: str = None,
+        callback_url: str = None,
         max_concurrency: int = None,
         name: str = None,
         owner_id: int = None,
         play_sleep_val: int = None,
         play_times: int = None,
         recall_type: int = None,
         record_path: str = None,
@@ -2041,14 +2063,16 @@
         status: int = None,
         task_id: int = None,
         template_id: int = None,
         template_type: int = None,
     ):
         # 外呼时间
         self.call_time_list_shrink = call_time_list_shrink
+        # 回调地址
+        self.callback_url = callback_url
         # 并发数
         self.max_concurrency = max_concurrency
         # 任务名称
         self.name = name
         self.owner_id = owner_id
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val
@@ -2086,14 +2110,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.call_time_list_shrink is not None:
             result['CallTimeList'] = self.call_time_list_shrink
+        if self.callback_url is not None:
+            result['CallbackUrl'] = self.callback_url
         if self.max_concurrency is not None:
             result['MaxConcurrency'] = self.max_concurrency
         if self.name is not None:
             result['Name'] = self.name
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.play_sleep_val is not None:
@@ -2128,14 +2154,16 @@
             result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CallTimeList') is not None:
             self.call_time_list_shrink = m.get('CallTimeList')
+        if m.get('CallbackUrl') is not None:
+            self.callback_url = m.get('CallbackUrl')
         if m.get('MaxConcurrency') is not None:
             self.max_concurrency = m.get('MaxConcurrency')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PlaySleepVal') is not None:
```

### Comparing `alibabacloud_aiccs20230516-1.0.1/alibabacloud_aiccs20230516.egg-info/PKG-INFO` & `alibabacloud_aiccs20230516-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-aiccs20230516
-Version: 1.0.1
+Name: alibabacloud_aiccs20230516
+Version: 1.0.2
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516-1.0.1/setup.py` & `alibabacloud_aiccs20230516-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiccs20230516.
 
-Created on 04/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiccs20230516"
 NAME = "alibabacloud_aiccs20230516" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud aiccs (20230516) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

