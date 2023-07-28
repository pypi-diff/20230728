# Comparing `tmp/alibabacloud_cms20190101-2.0.7.tar.gz` & `tmp/alibabacloud_cms20190101-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.7.tar", last modified: Thu Jul 13 10:49:10 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.8.tar", last modified: Fri Jul 28 05:32:44 2023, max compression
```

## Comparing `alibabacloud_cms20190101-2.0.7.tar` & `alibabacloud_cms20190101-2.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   666677 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/client.py
--rw-r--r--   0 root         (0) root         (0)  1807690 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   668027 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1808781 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2023-07-28 05:32:44.000000 alibabacloud_cms20190101-2.0.8/setup.py
```

### Comparing `alibabacloud_cms20190101-2.0.7/LICENSE` & `alibabacloud_cms20190101-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.7/PKG-INFO` & `alibabacloud_cms20190101-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cms20190101
-Version: 2.0.7
+Version: 2.0.8
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.7/README-CN.md` & `alibabacloud_cms20190101-2.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.7/README.md` & `alibabacloud_cms20190101-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/client.py` & `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5085,14 +5085,16 @@
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
@@ -5148,14 +5150,16 @@
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
@@ -5237,14 +5241,16 @@
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
@@ -5300,14 +5306,16 @@
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
@@ -5393,14 +5401,16 @@
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
@@ -5460,14 +5470,16 @@
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
@@ -13737,14 +13749,22 @@
         runtime = util_models.RuntimeOptions()
         return await self.modify_site_monitor_with_options_async(request, runtime)
 
     def open_cms_service_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.OpenCmsServiceResponse:
+        """
+        @deprecated
+        
+        @param request: OpenCmsServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
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
@@ -13758,14 +13778,22 @@
             self.call_api(params, req, runtime)
         )
 
     async def open_cms_service_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.OpenCmsServiceResponse:
+        """
+        @deprecated
+        
+        @param request: OpenCmsServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
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
@@ -13776,18 +13804,30 @@
         )
         return TeaCore.from_map(
             cms_20190101_models.OpenCmsServiceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def open_cms_service(self) -> cms_20190101_models.OpenCmsServiceResponse:
+        """
+        @deprecated
+        
+        @return: OpenCmsServiceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_cms_service_with_options(runtime)
 
     async def open_cms_service_async(self) -> cms_20190101_models.OpenCmsServiceResponse:
+        """
+        @deprecated
+        
+        @return: OpenCmsServiceResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_cms_service_with_options_async(runtime)
 
     def put_contact_with_options(
         self,
         request: cms_20190101_models.PutContactRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/models.py` & `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13587,14 +13587,15 @@
         page_number: int = None,
         page_size: int = None,
         product: str = None,
         region_id: str = None,
         rule_name: str = None,
         search_key: str = None,
         send_status: str = None,
+        source_type: str = None,
         start_time: int = None,
     ):
         # The alert group.
         self.contact_group = contact_group
         # The statistical period of alert logs. Unit: minutes.
         self.end_time = end_time
         # The dimension based on which data is aggregated. This parameter is similar to the Group By clause of SQL statements. Valid values:
@@ -13645,14 +13646,15 @@
         # *   1: The alert is generated not during the effective period.
         # *   2: The alert is muted and not triggered in a specified period.
         # *   3: The host is restarting.
         # *   4: Notifications are not sent for the alert.
         # 
         # When the value of the SendStatus parameter is 0, the value P4 of the Level parameter indicates a triggered alert and the value OK indicates a cleared alert.
         self.send_status = send_status
+        self.source_type = source_type
         # The name of the metric.
         # 
         # > For more information about the metrics of different cloud services, see [Appendix 1: Metrics](~~163515~~).
         self.start_time = start_time
 
     def validate(self):
         pass
@@ -13689,14 +13691,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -13725,14 +13729,16 @@
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
     def __init__(
@@ -13939,14 +13945,15 @@
         page_number: int = None,
         page_size: int = None,
         product: str = None,
         region_id: str = None,
         rule_name: str = None,
         search_key: str = None,
         send_status: str = None,
+        source_type: str = None,
         start_time: int = None,
     ):
         # The name of the metric.
         # 
         # >  For more information about the metrics of different cloud services, see [Appendix 1: Metrics](~~163515~~).
         self.contact_group = contact_group
         # The number of entries to return on each page. Default value: 10.
@@ -13993,14 +14000,15 @@
         self.region_id = region_id
         # The statistical period of alert logs. Unit: minutes.
         self.rule_name = rule_name
         # The abbreviation of the service name.
         self.search_key = search_key
         # The name of the alert rule.
         self.send_status = send_status
+        self.source_type = source_type
         # The number of the page to return. Default value: 1
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14035,14 +14043,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -14071,14 +14081,16 @@
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
     def __init__(
@@ -14248,14 +14260,15 @@
         page_size: int = None,
         product: str = None,
         region_id: str = None,
         rule_id: str = None,
         rule_name: str = None,
         search_key: str = None,
         send_status: str = None,
+        source_type: str = None,
         start_time: int = None,
     ):
         # The start timestamp of the alert logs to be queried. Unit: milliseconds.
         self.contact_group = contact_group
         # The alert contact group.
         self.end_time = end_time
         # The alert information in a JSON string.
@@ -14297,14 +14310,15 @@
         # *   If the cloud service is provided by Alibaba Cloud, the abbreviation of the service name is returned. Example: ECS.
         # *   If the cloud service is not provided by Alibaba Cloud, a value in the `acs_Service keyword` format is returned. Example: acs_networkmonitor.
         self.rule_name = rule_name
         # The ID of the log.
         self.search_key = search_key
         # The sending results of alert notifications.
         self.send_status = send_status
+        self.source_type = source_type
         # Indicates whether the alert level was changed. Valid values:
         # 
         # *   `P4->OK`: The alert level was changed from P4 to OK.
         # *   `P4->P4`: The alert level was still P4.
         self.start_time = start_time
 
     def validate(self):
@@ -14344,14 +14358,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ContactGroup') is not None:
@@ -14382,14 +14398,16 @@
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
     def __init__(
@@ -32698,14 +32716,15 @@
 
 
 class DescribeMonitoringAgentStatusesResponseBodyNodeStatusListNodeStatus(TeaModel):
     def __init__(
         self,
         auto_install: bool = None,
         instance_id: str = None,
+        os_monitor_config: str = None,
         os_monitor_error_code: str = None,
         os_monitor_error_detail: str = None,
         os_monitor_status: str = None,
         os_monitor_version: str = None,
         status: str = None,
     ):
         # The error status of SysOM. Valid values:
@@ -32715,14 +32734,15 @@
         # *   `install_assist_command_fail`: SysOM fails to be installed because the installation command fails to run.
         # *   `uninstall_fail`: SysOM fails to be uninstalled or an unknown error occurs.
         # *   `uninstall_assist_invalid`: SysOM fails to be uninstalled because the status of Cloud Assistant is invalid.
         # *   `uninstall_assist_command_fail`: SysOM fails to be uninstalled because the uninstallation command fails to run.
         self.auto_install = auto_install
         # The ID of the request.
         self.instance_id = instance_id
+        self.os_monitor_config = os_monitor_config
         self.os_monitor_error_code = os_monitor_error_code
         self.os_monitor_error_detail = os_monitor_error_detail
         # For more information about common request parameters, see [Common parameters](~~199331~~).
         self.os_monitor_status = os_monitor_status
         self.os_monitor_version = os_monitor_version
         # The status of the CloudMonitor agent. Valid values:
         # 
@@ -32743,14 +32763,16 @@
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
@@ -32761,14 +32783,16 @@
 
     def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/PKG-INFO` & `alibabacloud_cms20190101-2.0.8/alibabacloud_cms20190101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cms20190101
-Version: 2.0.7
+Version: 2.0.8
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.7/setup.py` & `alibabacloud_cms20190101-2.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cms20190101.
 
-Created on 13/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cms20190101"
 NAME = "alibabacloud_cms20190101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python"
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

