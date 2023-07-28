# Comparing `tmp/alibabacloud_aiccs20230516_py2-1.0.1.tar.gz` & `tmp/alibabacloud_aiccs20230516_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiccs20230516_py2-1.0.1.tar", last modified: Tue Jul  4 13:12:38 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiccs20230516_py2-1.0.2.tar", last modified: Fri Jul 28 03:56:39 2023, max compression
```

## Comparing `alibabacloud_aiccs20230516_py2-1.0.1.tar` & `alibabacloud_aiccs20230516_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41712 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/client.py
--rw-r--r--   0 root         (0) root         (0)   206433 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-07-04 13:12:38.000000 alibabacloud_aiccs20230516_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41940 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/client.py
+-rw-r--r--   0 root         (0) root         (0)   207612 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-07-28 03:56:39.000000 alibabacloud_aiccs20230516_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/LICENSE` & `alibabacloud_aiccs20230516_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/PKG-INFO` & `alibabacloud_aiccs20230516_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiccs20230516_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/README-CN.md` & `alibabacloud_aiccs20230516_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/README.md` & `alibabacloud_aiccs20230516_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/client.py` & `alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
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
@@ -305,14 +307,16 @@
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

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516/models.py` & `alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         return self
 
 
 class AddTaskRequestSendSmsPlan(TeaModel):
     def __init__(self, intent_tags=None, sms_template_id=None):
         # 意向标签
         self.intent_tags = intent_tags  # type: list[str]
-        # 重呼条件
+        # 短信模板ID
         self.sms_template_id = sms_template_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddTaskRequestSendSmsPlan, self).to_map()
@@ -276,20 +276,22 @@
             self.intent_tags = m.get('IntentTags')
         if m.get('SmsTemplateId') is not None:
             self.sms_template_id = m.get('SmsTemplateId')
         return self
 
 
 class AddTaskRequest(TeaModel):
-    def __init__(self, call_time_list=None, max_concurrency=None, name=None, owner_id=None, play_sleep_val=None,
-                 play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
+    def __init__(self, call_time_list=None, callback_url=None, max_concurrency=None, name=None, owner_id=None,
+                 play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
                  repeat_reason=None, repeat_times=None, resource_owner_account=None, resource_owner_id=None, send_sms_plan=None,
                  start_time=None, task_type=None, template_id=None, template_type=None):
         # 外呼时间
         self.call_time_list = call_time_list  # type: list[AddTaskRequestCallTimeList]
+        # 回调地址
+        self.callback_url = callback_url  # type: str
         # 并发数
         self.max_concurrency = max_concurrency  # type: long
         # 任务名称
         self.name = name  # type: str
         self.owner_id = owner_id  # type: long
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val  # type: long
@@ -336,14 +338,16 @@
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
@@ -383,14 +387,16 @@
     def from_map(self, m=None):
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
@@ -426,20 +432,23 @@
             self.template_id = m.get('TemplateId')
         if m.get('TemplateType') is not None:
             self.template_type = m.get('TemplateType')
         return self
 
 
 class AddTaskShrinkRequest(TeaModel):
-    def __init__(self, call_time_list_shrink=None, max_concurrency=None, name=None, owner_id=None,
-                 play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
-                 repeat_reason_shrink=None, repeat_times_shrink=None, resource_owner_account=None, resource_owner_id=None,
-                 send_sms_plan_shrink=None, start_time=None, task_type=None, template_id=None, template_type=None):
+    def __init__(self, call_time_list_shrink=None, callback_url=None, max_concurrency=None, name=None,
+                 owner_id=None, play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None,
+                 repeat_interval=None, repeat_reason_shrink=None, repeat_times_shrink=None, resource_owner_account=None,
+                 resource_owner_id=None, send_sms_plan_shrink=None, start_time=None, task_type=None, template_id=None,
+                 template_type=None):
         # 外呼时间
         self.call_time_list_shrink = call_time_list_shrink  # type: str
+        # 回调地址
+        self.callback_url = callback_url  # type: str
         # 并发数
         self.max_concurrency = max_concurrency  # type: long
         # 任务名称
         self.name = name  # type: str
         self.owner_id = owner_id  # type: long
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val  # type: long
@@ -477,14 +486,16 @@
         _map = super(AddTaskShrinkRequest, self).to_map()
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
@@ -519,14 +530,16 @@
             result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m=None):
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
@@ -1628,20 +1641,22 @@
             self.intent_tags = m.get('IntentTags')
         if m.get('SmsTemplateId') is not None:
             self.sms_template_id = m.get('SmsTemplateId')
         return self
 
 
 class EditTaskRequest(TeaModel):
-    def __init__(self, call_time_list=None, max_concurrency=None, name=None, owner_id=None, play_sleep_val=None,
-                 play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
+    def __init__(self, call_time_list=None, callback_url=None, max_concurrency=None, name=None, owner_id=None,
+                 play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
                  repeat_reason=None, repeat_times=None, resource_owner_account=None, resource_owner_id=None, send_sms_plan=None,
                  status=None, task_id=None, template_id=None, template_type=None):
         # 外呼时间
         self.call_time_list = call_time_list  # type: list[EditTaskRequestCallTimeList]
+        # 回调地址
+        self.callback_url = callback_url  # type: str
         # 并发数
         self.max_concurrency = max_concurrency  # type: long
         # 任务名称
         self.name = name  # type: str
         self.owner_id = owner_id  # type: long
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val  # type: long
@@ -1688,14 +1703,16 @@
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
@@ -1735,14 +1752,16 @@
     def from_map(self, m=None):
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
@@ -1778,20 +1797,22 @@
             self.template_id = m.get('TemplateId')
         if m.get('TemplateType') is not None:
             self.template_type = m.get('TemplateType')
         return self
 
 
 class EditTaskShrinkRequest(TeaModel):
-    def __init__(self, call_time_list_shrink=None, max_concurrency=None, name=None, owner_id=None,
-                 play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None, repeat_interval=None,
-                 repeat_reason_shrink=None, repeat_times_shrink=None, resource_owner_account=None, resource_owner_id=None,
-                 send_sms_plan_shrink=None, status=None, task_id=None, template_id=None, template_type=None):
+    def __init__(self, call_time_list_shrink=None, callback_url=None, max_concurrency=None, name=None,
+                 owner_id=None, play_sleep_val=None, play_times=None, recall_type=None, record_path=None, repeat_count=None,
+                 repeat_interval=None, repeat_reason_shrink=None, repeat_times_shrink=None, resource_owner_account=None,
+                 resource_owner_id=None, send_sms_plan_shrink=None, status=None, task_id=None, template_id=None, template_type=None):
         # 外呼时间
         self.call_time_list_shrink = call_time_list_shrink  # type: str
+        # 回调地址
+        self.callback_url = callback_url  # type: str
         # 并发数
         self.max_concurrency = max_concurrency  # type: long
         # 任务名称
         self.name = name  # type: str
         self.owner_id = owner_id  # type: long
         # 播放间隔时长
         self.play_sleep_val = play_sleep_val  # type: long
@@ -1829,14 +1850,16 @@
         _map = super(EditTaskShrinkRequest, self).to_map()
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
@@ -1871,14 +1894,16 @@
             result['TemplateType'] = self.template_type
         return result
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO` & `alibabacloud_aiccs20230516_py2-1.0.2/alibabacloud_aiccs20230516_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiccs20230516-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud aiccs (20230516) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiccs20230516_py2-1.0.1/setup.py` & `alibabacloud_aiccs20230516_py2-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiccs20230516_py2.
 
-Created on 04/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiccs20230516"
 NAME = "alibabacloud_aiccs20230516_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud aiccs (20230516) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

