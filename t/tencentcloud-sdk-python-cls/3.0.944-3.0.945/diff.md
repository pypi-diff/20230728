# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.944.tar", last modified: Thu Jul 27 02:12:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.945.tar", last modified: Fri Jul 28 00:24:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.944.tar` & `tencentcloud-sdk-python-cls-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    81003 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9048 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   486508 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:12:25.000000 tencentcloud-sdk-python-cls-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    81890 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   499532 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.944/setup.py` & `tencentcloud-sdk-python-cls-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,14 +1011,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeDashboards(self, request):
+        """本接口用于获取仪表盘
+
+        :param request: Request instance for DescribeDashboards.
+        :type request: :class:`tencentcloud.cls.v20201016.models.DescribeDashboardsRequest`
+        :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeDashboardsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDashboards", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDashboardsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeDataTransformInfo(self, request):
         """本接口用于获取数据加工任务列表基本信息
 
         :param request: Request instance for DescribeDataTransformInfo.
         :type request: :class:`tencentcloud.cls.v20201016.models.DescribeDataTransformInfoRequest`
         :rtype: :class:`tencentcloud.cls.v20201016.models.DescribeDataTransformInfoResponse`
```

### Comparing `tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.944/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5245,14 +5245,230 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DashboardInfo(AbstractModel):
+    """仪表盘信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _DashboardId: 仪表盘id
+        :type DashboardId: str
+        :param _DashboardName: 仪表盘名字
+        :type DashboardName: str
+        :param _Data: 仪表盘数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: str
+        :param _CreateTime: 创建仪表盘的时间
+        :type CreateTime: str
+        :param _AssumerUin: AssumerUin非空则表示创建该日志主题的服务方Uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssumerUin: int
+        :param _RoleName: RoleName非空则表示创建该日志主题的服务方使用的角色
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RoleName: str
+        :param _AssumerName: AssumerName非空则表示创建该日志主题的服务方名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssumerName: str
+        :param _Tags: 日志主题绑定的标签信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of Tag
+        :param _DashboardRegion: 仪表盘所在地域： 为了兼容老的地域。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DashboardRegion: str
+        :param _UpdateTime: 修改仪表盘的时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param _DashboardTopicInfos: 仪表盘对应的topic相关信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DashboardTopicInfos: list of DashboardTopicInfo
+        """
+        self._DashboardId = None
+        self._DashboardName = None
+        self._Data = None
+        self._CreateTime = None
+        self._AssumerUin = None
+        self._RoleName = None
+        self._AssumerName = None
+        self._Tags = None
+        self._DashboardRegion = None
+        self._UpdateTime = None
+        self._DashboardTopicInfos = None
+
+    @property
+    def DashboardId(self):
+        return self._DashboardId
+
+    @DashboardId.setter
+    def DashboardId(self, DashboardId):
+        self._DashboardId = DashboardId
+
+    @property
+    def DashboardName(self):
+        return self._DashboardName
+
+    @DashboardName.setter
+    def DashboardName(self, DashboardName):
+        self._DashboardName = DashboardName
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def AssumerUin(self):
+        return self._AssumerUin
+
+    @AssumerUin.setter
+    def AssumerUin(self, AssumerUin):
+        self._AssumerUin = AssumerUin
+
+    @property
+    def RoleName(self):
+        return self._RoleName
+
+    @RoleName.setter
+    def RoleName(self, RoleName):
+        self._RoleName = RoleName
+
+    @property
+    def AssumerName(self):
+        return self._AssumerName
+
+    @AssumerName.setter
+    def AssumerName(self, AssumerName):
+        self._AssumerName = AssumerName
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def DashboardRegion(self):
+        return self._DashboardRegion
+
+    @DashboardRegion.setter
+    def DashboardRegion(self, DashboardRegion):
+        self._DashboardRegion = DashboardRegion
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def DashboardTopicInfos(self):
+        return self._DashboardTopicInfos
+
+    @DashboardTopicInfos.setter
+    def DashboardTopicInfos(self, DashboardTopicInfos):
+        self._DashboardTopicInfos = DashboardTopicInfos
+
+
+    def _deserialize(self, params):
+        self._DashboardId = params.get("DashboardId")
+        self._DashboardName = params.get("DashboardName")
+        self._Data = params.get("Data")
+        self._CreateTime = params.get("CreateTime")
+        self._AssumerUin = params.get("AssumerUin")
+        self._RoleName = params.get("RoleName")
+        self._AssumerName = params.get("AssumerName")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        self._DashboardRegion = params.get("DashboardRegion")
+        self._UpdateTime = params.get("UpdateTime")
+        if params.get("DashboardTopicInfos") is not None:
+            self._DashboardTopicInfos = []
+            for item in params.get("DashboardTopicInfos"):
+                obj = DashboardTopicInfo()
+                obj._deserialize(item)
+                self._DashboardTopicInfos.append(obj)
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
+class DashboardTopicInfo(AbstractModel):
+    """仪表盘关联的topic信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TopicId: 主题id
+        :type TopicId: str
+        :param _Region: topic所在的地域
+        :type Region: str
+        """
+        self._TopicId = None
+        self._Region = None
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
+    def Region(self):
+        return self._Region
+
+    @Region.setter
+    def Region(self, Region):
+        self._Region = Region
+
+
+    def _deserialize(self, params):
+        self._TopicId = params.get("TopicId")
+        self._Region = params.get("Region")
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
 class DataTransformResouceInfo(AbstractModel):
     """数据加工的资源信息
 
     """
 
     def __init__(self):
         r"""
@@ -7416,14 +7632,184 @@
             for item in params.get("Data"):
                 obj = CosRechargeInfo()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDashboardsRequest(AbstractModel):
+    """DescribeDashboards请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Offset: 分页的偏移量，默认值为0。
+        :type Offset: int
+        :param _Limit: 分页单页限制数目，默认值为20，最大值100。
+        :type Limit: int
+        :param _Filters: <br><li> dashboardId
+
+按照【仪表盘id】进行过滤。
+类型：String
+
+必选：否
+
+<br><li> dashboardName
+
+按照【仪表盘名字】进行模糊搜索过滤。
+类型：String
+
+必选：否
+
+<br><li> dashboardRegion
+
+按照【仪表盘地域】进行过滤，为了兼容老的仪表盘，通过云API创建的仪表盘没有地域属性
+类型：String
+
+必选：否
+
+<br><li> tagKey
+
+按照【标签键】进行过滤。
+
+类型：String
+
+必选：否
+
+<br><li> tag:tagKey
+
+按照【标签键值对】进行过滤。tag-key使用具体的标签键进行替换。使用请参考示例2。
+
+类型：String
+
+必选：否
+
+每次请求的Filters的上限为10，Filter.Values的上限为100。
+        :type Filters: list of Filter
+        :param _TopicIdRegionFilter: 按照topicId和regionId过滤。
+        :type TopicIdRegionFilter: list of TopicIdAndRegion
+        """
+        self._Offset = None
+        self._Limit = None
+        self._Filters = None
+        self._TopicIdRegionFilter = None
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def TopicIdRegionFilter(self):
+        return self._TopicIdRegionFilter
+
+    @TopicIdRegionFilter.setter
+    def TopicIdRegionFilter(self, TopicIdRegionFilter):
+        self._TopicIdRegionFilter = TopicIdRegionFilter
+
+
+    def _deserialize(self, params):
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        if params.get("TopicIdRegionFilter") is not None:
+            self._TopicIdRegionFilter = []
+            for item in params.get("TopicIdRegionFilter"):
+                obj = TopicIdAndRegion()
+                obj._deserialize(item)
+                self._TopicIdRegionFilter.append(obj)
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
+class DescribeDashboardsResponse(AbstractModel):
+    """DescribeDashboards返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 仪表盘的数量
+        :type TotalCount: int
+        :param _DashboardInfos: 仪表盘详细明细
+        :type DashboardInfos: list of DashboardInfo
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._DashboardInfos = None
+        self._RequestId = None
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
+    def DashboardInfos(self):
+        return self._DashboardInfos
+
+    @DashboardInfos.setter
+    def DashboardInfos(self, DashboardInfos):
+        self._DashboardInfos = DashboardInfos
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("DashboardInfos") is not None:
+            self._DashboardInfos = []
+            for item in params.get("DashboardInfos"):
+                obj = DashboardInfo()
+                obj._deserialize(item)
+                self._DashboardInfos.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeDataTransformInfoRequest(AbstractModel):
     """DescribeDataTransformInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15266,19 +15652,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param _TopicId: 目标主题id
         :type TopicId: str
-        :param _Region: topic的地域信息
+        :param _Region: 主题的的地域信息
         :type Region: str
+        :param _BizType: 主题类型：0为日志主题，1为指标主题
+        :type BizType: int
+        :param _MetricName: 指标名称
+        :type MetricName: str
         """
         self._TopicId = None
         self._Region = None
+        self._BizType = None
+        self._MetricName = None
 
     @property
     def TopicId(self):
         return self._TopicId
 
     @TopicId.setter
     def TopicId(self, TopicId):
@@ -15288,18 +15680,36 @@
     def Region(self):
         return self._Region
 
     @Region.setter
     def Region(self, Region):
         self._Region = Region
 
+    @property
+    def BizType(self):
+        return self._BizType
+
+    @BizType.setter
+    def BizType(self, BizType):
+        self._BizType = BizType
+
+    @property
+    def MetricName(self):
+        return self._MetricName
+
+    @MetricName.setter
+    def MetricName(self, MetricName):
+        self._MetricName = MetricName
+
 
     def _deserialize(self, params):
         self._TopicId = params.get("TopicId")
         self._Region = params.get("Region")
+        self._BizType = params.get("BizType")
+        self._MetricName = params.get("MetricName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -16440,14 +16850,60 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TopicIdAndRegion(AbstractModel):
+    """仪表盘 topic与地域信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TopicId: 日志主题id
+        :type TopicId: str
+        :param _RegionId: 日志主题id 所在的地域id
+地域ID - 访问链接查看详情：https://iwiki.woa.com/pages/viewpage.action?pageId=780556968#id-地域码表-一.region大区（标准地域）
+        :type RegionId: int
+        """
+        self._TopicId = None
+        self._RegionId = None
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
+    def RegionId(self):
+        return self._RegionId
+
+    @RegionId.setter
+    def RegionId(self, RegionId):
+        self._RegionId = RegionId
+
+
+    def _deserialize(self, params):
+        self._TopicId = params.get("TopicId")
+        self._RegionId = params.get("RegionId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TopicInfo(AbstractModel):
     """日志主题信息
 
     """
```

### Comparing `tencentcloud-sdk-python-cls-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.944/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.945/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.944/README.rst` & `tencentcloud-sdk-python-cls-3.0.945/README.rst`

 * *Files identical despite different names*

