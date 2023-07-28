# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.944.tar", last modified: Thu Jul 27 02:27:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.945.tar", last modified: Fri Jul 28 00:39:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.944.tar` & `tencentcloud-sdk-python-waf-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    47687 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   309253 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:27:50.000000 tencentcloud-sdk-python-waf-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    48616 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   314432 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/setup.py` & `tencentcloud-sdk-python-waf-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.944'
+__version__ = '3.0.945'
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,14 +367,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeAccessHistogram(self, request):
+        """本接口用于访问日志柱状趋势图
+
+        :param request: Request instance for DescribeAccessHistogram.
+        :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAccessHistogramRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.DescribeAccessHistogramResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAccessHistogram", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAccessHistogramResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeAccessIndex(self, request):
         """本接口用于获取访问日志索引配置信息
 
         :param request: Request instance for DescribeAccessIndex.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribeAccessIndexRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.DescribeAccessIndexResponse`
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,59 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AccessHistogramItem(AbstractModel):
+    """用于接口DescribeAccessHistogram 的出参
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _BTime: 时间，单位ms
+        :type BTime: int
+        :param _Count: 日志条数
+        :type Count: int
+        """
+        self._BTime = None
+        self._Count = None
+
+    @property
+    def BTime(self):
+        return self._BTime
+
+    @BTime.setter
+    def BTime(self, BTime):
+        self._BTime = BTime
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+
+    def _deserialize(self, params):
+        self._BTime = params.get("BTime")
+        self._Count = params.get("Count")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AccessKeyValueInfo(AbstractModel):
     """用于 DescribeAccessIndex 的出参
 
     """
 
     def __init__(self):
         r"""
@@ -3056,14 +3101,162 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DescribeAccessHistogramRequest(AbstractModel):
+    """DescribeAccessHistogram请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TopicId: 老版本查询的日志主题ID，新版本传空字符串即可
+        :type TopicId: str
+        :param _From: 要查询的日志的起始时间，Unix时间戳，单位ms
+        :type From: int
+        :param _To: 要查询的日志的结束时间，Unix时间戳，单位ms
+        :type To: int
+        :param _Query: 查询语句，语句长度最大为4096
+        :type Query: str
+        :param _Interval: 柱状图间隔时间差，单位ms
+        :type Interval: int
+        """
+        self._TopicId = None
+        self._From = None
+        self._To = None
+        self._Query = None
+        self._Interval = None
+
+    @property
+    def TopicId(self):
+        return self._TopicId
+
+    @TopicId.setter
+    def TopicId(self, TopicId):
+        self._TopicId = TopicId
+
+    @property
+    def From(self):
+        return self._From
+
+    @From.setter
+    def From(self, From):
+        self._From = From
+
+    @property
+    def To(self):
+        return self._To
+
+    @To.setter
+    def To(self, To):
+        self._To = To
+
+    @property
+    def Query(self):
+        return self._Query
+
+    @Query.setter
+    def Query(self, Query):
+        self._Query = Query
+
+    @property
+    def Interval(self):
+        return self._Interval
+
+    @Interval.setter
+    def Interval(self, Interval):
+        self._Interval = Interval
+
+
+    def _deserialize(self, params):
+        self._TopicId = params.get("TopicId")
+        self._From = params.get("From")
+        self._To = params.get("To")
+        self._Query = params.get("Query")
+        self._Interval = params.get("Interval")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAccessHistogramResponse(AbstractModel):
+    """DescribeAccessHistogram返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Interval: 柱状图间隔时间差，单位ms
+        :type Interval: int
+        :param _TotalCount: 满足条件的日志条数
+        :type TotalCount: int
+        :param _HistogramInfos: 注意：此字段可能返回 null，表示取不到有效值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HistogramInfos: list of AccessHistogramItem
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Interval = None
+        self._TotalCount = None
+        self._HistogramInfos = None
+        self._RequestId = None
+
+    @property
+    def Interval(self):
+        return self._Interval
+
+    @Interval.setter
+    def Interval(self, Interval):
+        self._Interval = Interval
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def HistogramInfos(self):
+        return self._HistogramInfos
+
+    @HistogramInfos.setter
+    def HistogramInfos(self, HistogramInfos):
+        self._HistogramInfos = HistogramInfos
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Interval = params.get("Interval")
+        self._TotalCount = params.get("TotalCount")
+        if params.get("HistogramInfos") is not None:
+            self._HistogramInfos = []
+            for item in params.get("HistogramInfos"):
+                obj = AccessHistogramItem()
+                obj._deserialize(item)
+                self._HistogramInfos.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeAccessIndexRequest(AbstractModel):
     """DescribeAccessIndex请求参数结构体
 
     """
 
 
 class DescribeAccessIndexResponse(AbstractModel):
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.945/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.944/README.rst` & `tencentcloud-sdk-python-waf-3.0.945/README.rst`

 * *Files identical despite different names*

