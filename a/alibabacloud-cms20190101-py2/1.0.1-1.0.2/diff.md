# Comparing `tmp/alibabacloud_cms20190101_py2-1.0.1.tar.gz` & `tmp/alibabacloud_cms20190101_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cms20190101_py2-1.0.1.tar", last modified: Thu Jul 13 09:16:52 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cms20190101_py2-1.0.2.tar", last modified: Fri Jul 28 05:32:56 2023, max compression
```

## Comparing `alibabacloud_cms20190101_py2-1.0.1.tar` & `alibabacloud_cms20190101_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   281346 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/client.py
--rw-r--r--   0 root         (0) root         (0)  1827512 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2482 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-07-13 09:16:52.000000 alibabacloud_cms20190101_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   282025 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1828595 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-07-28 05:32:56.000000 alibabacloud_cms20190101_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_cms20190101_py2-1.0.1/LICENSE` & `alibabacloud_cms20190101_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.1/PKG-INFO` & `alibabacloud_cms20190101_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cms20190101_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101_py2-1.0.1/README-CN.md` & `alibabacloud_cms20190101_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.1/README.md` & `alibabacloud_cms20190101_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/client.py` & `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2297,14 +2297,16 @@
             query['Product'] = request.product
         if not UtilClient.is_unset(request.rule_name):
             query['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.search_key):
             query['SearchKey'] = request.search_key
         if not UtilClient.is_unset(request.send_status):
             query['SendStatus'] = request.send_status
+        if not UtilClient.is_unset(request.source_type):
+            query['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeAlertLogCount',
@@ -2371,14 +2373,16 @@
             query['Product'] = request.product
         if not UtilClient.is_unset(request.rule_name):
             query['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.search_key):
             query['SearchKey'] = request.search_key
         if not UtilClient.is_unset(request.send_status):
             query['SendStatus'] = request.send_status
+        if not UtilClient.is_unset(request.source_type):
+            query['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeAlertLogHistogram',
@@ -2449,14 +2453,16 @@
             query['RuleId'] = request.rule_id
         if not UtilClient.is_unset(request.rule_name):
             query['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.search_key):
             query['SearchKey'] = request.search_key
         if not UtilClient.is_unset(request.send_status):
             query['SendStatus'] = request.send_status
+        if not UtilClient.is_unset(request.source_type):
+            query['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeAlertLogList',
@@ -6189,14 +6195,25 @@
 
         @return: ModifySiteMonitorResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_site_monitor_with_options(request, runtime)
 
     def open_cms_service_with_options(self, runtime):
+        """
+        @deprecated
+        
+
+        @param request: OpenCmsServiceRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: OpenCmsServiceResponse
+        Deprecated
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='OpenCmsService',
             version='2019-01-01',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -6207,14 +6224,21 @@
         )
         return TeaCore.from_map(
             cms_20190101_models.OpenCmsServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def open_cms_service(self):
+        """
+        @deprecated
+        
+
+        @return: OpenCmsServiceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_cms_service_with_options(runtime)
 
     def put_contact_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.contact_name):
```

### Comparing `alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101/models.py` & `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12048,15 +12048,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertLogCountRequest(TeaModel):
     def __init__(self, contact_group=None, end_time=None, group_by=None, group_id=None, last_min=None, level=None,
                  metric_name=None, namespace=None, page_number=None, page_size=None, product=None, region_id=None,
-                 rule_name=None, search_key=None, send_status=None, start_time=None):
+                 rule_name=None, search_key=None, send_status=None, source_type=None, start_time=None):
         # The alert group.
         self.contact_group = contact_group  # type: str
         # The statistical period of alert logs. Unit: minutes.
         self.end_time = end_time  # type: long
         # The dimension based on which data is aggregated. This parameter is similar to the Group By clause of SQL statements. Valid values:
         # 
         # *   `product`: aggregates data by cloud service.
@@ -12105,14 +12105,15 @@
         # *   1: The alert is generated not during the effective period.
         # *   2: The alert is muted and not triggered in a specified period.
         # *   3: The host is restarting.
         # *   4: Notifications are not sent for the alert.
         # 
         # When the value of the SendStatus parameter is 0, the value P4 of the Level parameter indicates a triggered alert and the value OK indicates a cleared alert.
         self.send_status = send_status  # type: str
+        self.source_type = source_type  # type: str
         # The name of the metric.
         # 
         # > For more information about the metrics of different cloud services, see [Appendix 1: Metrics](~~163515~~).
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
@@ -12149,14 +12150,16 @@
             result['RegionId'] = self.region_id
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.search_key is not None:
             result['SearchKey'] = self.search_key
         if self.send_status is not None:
             result['SendStatus'] = self.send_status
+        if self.source_type is not None:
+            result['SourceType'] = self.source_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -12185,14 +12188,16 @@
             self.region_id = m.get('RegionId')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('SearchKey') is not None:
             self.search_key = m.get('SearchKey')
         if m.get('SendStatus') is not None:
             self.send_status = m.get('SendStatus')
+        if m.get('SourceType') is not None:
+            self.source_type = m.get('SourceType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAlertLogCountResponseBodyAlertLogCountLogs(TeaModel):
     def __init__(self, name=None, value=None):
@@ -12364,15 +12369,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertLogHistogramRequest(TeaModel):
     def __init__(self, contact_group=None, end_time=None, group_by=None, group_id=None, last_min=None, level=None,
                  metric_name=None, namespace=None, page_number=None, page_size=None, product=None, region_id=None,
-                 rule_name=None, search_key=None, send_status=None, start_time=None):
+                 rule_name=None, search_key=None, send_status=None, source_type=None, start_time=None):
         # The name of the metric.
         # 
         # >  For more information about the metrics of different cloud services, see [Appendix 1: Metrics](~~163515~~).
         self.contact_group = contact_group  # type: str
         # The number of entries to return on each page. Default value: 10.
         self.end_time = end_time  # type: long
         # The error message.
@@ -12417,14 +12422,15 @@
         self.region_id = region_id  # type: str
         # The statistical period of alert logs. Unit: minutes.
         self.rule_name = rule_name  # type: str
         # The abbreviation of the service name.
         self.search_key = search_key  # type: str
         # The name of the alert rule.
         self.send_status = send_status  # type: str
+        self.source_type = source_type  # type: str
         # The number of the page to return. Default value: 1
         self.start_time = start_time  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -12459,14 +12465,16 @@
             result['RegionId'] = self.region_id
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.search_key is not None:
             result['SearchKey'] = self.search_key
         if self.send_status is not None:
             result['SendStatus'] = self.send_status
+        if self.source_type is not None:
+            result['SourceType'] = self.source_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -12495,14 +12503,16 @@
             self.region_id = m.get('RegionId')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('SearchKey') is not None:
             self.search_key = m.get('SearchKey')
         if m.get('SendStatus') is not None:
             self.send_status = m.get('SendStatus')
+        if m.get('SourceType') is not None:
+            self.source_type = m.get('SourceType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAlertLogHistogramResponseBodyAlertLogHistogramList(TeaModel):
     def __init__(self, count=None, from_=None, to=None):
@@ -12639,15 +12649,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAlertLogListRequest(TeaModel):
     def __init__(self, contact_group=None, end_time=None, group_by=None, group_id=None, last_min=None, level=None,
                  metric_name=None, namespace=None, page_number=None, page_size=None, product=None, region_id=None, rule_id=None,
-                 rule_name=None, search_key=None, send_status=None, start_time=None):
+                 rule_name=None, search_key=None, send_status=None, source_type=None, start_time=None):
         # The start timestamp of the alert logs to be queried. Unit: milliseconds.
         self.contact_group = contact_group  # type: str
         # The alert contact group.
         self.end_time = end_time  # type: long
         # The alert information in a JSON string.
         self.group_by = group_by  # type: str
         # The operation that you want to perform. Set the value to **DescribeAlertLogList**.
@@ -12687,14 +12697,15 @@
         # *   If the cloud service is provided by Alibaba Cloud, the abbreviation of the service name is returned. Example: ECS.
         # *   If the cloud service is not provided by Alibaba Cloud, a value in the `acs_Service keyword` format is returned. Example: acs_networkmonitor.
         self.rule_name = rule_name  # type: str
         # The ID of the log.
         self.search_key = search_key  # type: str
         # The sending results of alert notifications.
         self.send_status = send_status  # type: str
+        self.source_type = source_type  # type: str
         # Indicates whether the alert level was changed. Valid values:
         # 
         # *   `P4->OK`: The alert level was changed from P4 to OK.
         # *   `P4->P4`: The alert level was still P4.
         self.start_time = start_time  # type: long
 
     def validate(self):
@@ -12734,14 +12745,16 @@
             result['RuleId'] = self.rule_id
         if self.rule_name is not None:
             result['RuleName'] = self.rule_name
         if self.search_key is not None:
             result['SearchKey'] = self.search_key
         if self.send_status is not None:
             result['SendStatus'] = self.send_status
+        if self.source_type is not None:
+            result['SourceType'] = self.source_type
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -12772,14 +12785,16 @@
             self.rule_id = m.get('RuleId')
         if m.get('RuleName') is not None:
             self.rule_name = m.get('RuleName')
         if m.get('SearchKey') is not None:
             self.search_key = m.get('SearchKey')
         if m.get('SendStatus') is not None:
             self.send_status = m.get('SendStatus')
+        if m.get('SourceType') is not None:
+            self.source_type = m.get('SourceType')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeAlertLogListResponseBodyAlertLogListDimensions(TeaModel):
     def __init__(self, key=None, value=None):
@@ -29151,27 +29166,28 @@
             self.instance_ids = m.get('InstanceIds')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeMonitoringAgentStatusesResponseBodyNodeStatusListNodeStatus(TeaModel):
-    def __init__(self, auto_install=None, instance_id=None, os_monitor_error_code=None,
+    def __init__(self, auto_install=None, instance_id=None, os_monitor_config=None, os_monitor_error_code=None,
                  os_monitor_error_detail=None, os_monitor_status=None, os_monitor_version=None, status=None):
         # The error status of SysOM. Valid values:
         # 
         # *   `install_fail`: SysOM fails to be installed or an unknown error occurs.
         # *   `install_assist_invalid`: SysOM fails to be installed because the status of Cloud Assistant is invalid.
         # *   `install_assist_command_fail`: SysOM fails to be installed because the installation command fails to run.
         # *   `uninstall_fail`: SysOM fails to be uninstalled or an unknown error occurs.
         # *   `uninstall_assist_invalid`: SysOM fails to be uninstalled because the status of Cloud Assistant is invalid.
         # *   `uninstall_assist_command_fail`: SysOM fails to be uninstalled because the uninstallation command fails to run.
         self.auto_install = auto_install  # type: bool
         # The ID of the request.
         self.instance_id = instance_id  # type: str
+        self.os_monitor_config = os_monitor_config  # type: str
         self.os_monitor_error_code = os_monitor_error_code  # type: str
         self.os_monitor_error_detail = os_monitor_error_detail  # type: str
         # For more information about common request parameters, see [Common parameters](~~199331~~).
         self.os_monitor_status = os_monitor_status  # type: str
         self.os_monitor_version = os_monitor_version  # type: str
         # The status of the CloudMonitor agent. Valid values:
         # 
@@ -29192,14 +29208,16 @@
             return _map
 
         result = dict()
         if self.auto_install is not None:
             result['AutoInstall'] = self.auto_install
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.os_monitor_config is not None:
+            result['OsMonitorConfig'] = self.os_monitor_config
         if self.os_monitor_error_code is not None:
             result['OsMonitorErrorCode'] = self.os_monitor_error_code
         if self.os_monitor_error_detail is not None:
             result['OsMonitorErrorDetail'] = self.os_monitor_error_detail
         if self.os_monitor_status is not None:
             result['OsMonitorStatus'] = self.os_monitor_status
         if self.os_monitor_version is not None:
@@ -29210,14 +29228,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AutoInstall') is not None:
             self.auto_install = m.get('AutoInstall')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('OsMonitorConfig') is not None:
+            self.os_monitor_config = m.get('OsMonitorConfig')
         if m.get('OsMonitorErrorCode') is not None:
             self.os_monitor_error_code = m.get('OsMonitorErrorCode')
         if m.get('OsMonitorErrorDetail') is not None:
             self.os_monitor_error_detail = m.get('OsMonitorErrorDetail')
         if m.get('OsMonitorStatus') is not None:
             self.os_monitor_status = m.get('OsMonitorStatus')
         if m.get('OsMonitorVersion') is not None:
```

### Comparing `alibabacloud_cms20190101_py2-1.0.1/alibabacloud_cms20190101_py2.egg-info/PKG-INFO` & `alibabacloud_cms20190101_py2-1.0.2/alibabacloud_cms20190101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cms20190101-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101_py2-1.0.1/setup.py` & `alibabacloud_cms20190101_py2-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cms20190101_py2.
 
-Created on 13/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cms20190101"
 NAME = "alibabacloud_cms20190101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python2"
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

