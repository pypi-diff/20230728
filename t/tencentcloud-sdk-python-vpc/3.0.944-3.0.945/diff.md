# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.944.tar", last modified: Thu Jul 27 02:27:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.945.tar", last modified: Fri Jul 28 00:39:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.944.tar` & `tencentcloud-sdk-python-vpc-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   333624 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43190 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1312271 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:27:39.000000 tencentcloud-sdk-python-vpc-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   334726 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43302 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1324725 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:39:25.000000 tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:39:24.000000 tencentcloud-sdk-python-vpc-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/setup.py` & `tencentcloud-sdk-python-vpc-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4019,14 +4019,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeSpecificTrafficPackageUsedDetails(self, request):
+        """本接口 (DescribeSpecificTrafficPackageUsedDetails) 用于查询指定 共享流量包 的用量明细。
+
+        :param request: Request instance for DescribeSpecificTrafficPackageUsedDetails.
+        :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSpecificTrafficPackageUsedDetailsRequest`
+        :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeSpecificTrafficPackageUsedDetailsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSpecificTrafficPackageUsedDetails", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSpecificTrafficPackageUsedDetailsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeSubnetResourceDashboard(self, request):
         """本接口(DescribeSubnetResourceDashboard)用于查看Subnet资源信息。
 
         :param request: Request instance for DescribeSubnetResourceDashboard.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetResourceDashboardRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeSubnetResourceDashboardResponse`
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,17 @@
 
 # 标签值不存在。
 INVALIDPARAMETERVALUE_TAGVALNOTEXISTS = 'InvalidParameterValue.TagValNotExists'
 
 # 无效参数值。参数值太长。
 INVALIDPARAMETERVALUE_TOOLONG = 'InvalidParameterValue.TooLong'
 
+# 流量包ID格式错误。
+INVALIDPARAMETERVALUE_TRAFFICPACKAGEID = 'InvalidParameterValue.TrafficPackageId'
+
 # 该流量包ID不合法。
 INVALIDPARAMETERVALUE_TRAFFICPACKAGEIDMALFORMED = 'InvalidParameterValue.TrafficPackageIdMalformed'
 
 # 未查询到此流量包。
 INVALIDPARAMETERVALUE_TRAFFICPACKAGENOTFOUND = 'InvalidParameterValue.TrafficPackageNotFound'
 
 # 指定的流量包不支持此操作
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/vpc/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20883,14 +20883,190 @@
                 obj = SnapshotPolicy()
                 obj._deserialize(item)
                 self._SnapshotPolicySet.append(obj)
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
+class DescribeSpecificTrafficPackageUsedDetailsRequest(AbstractModel):
+    """DescribeSpecificTrafficPackageUsedDetails请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TrafficPackageId: 共享流量包唯一ID
+        :type TrafficPackageId: str
+        :param _Filters: 每次请求的`Filters`的上限为10，`Filter.Values`的上限为5。详细的过滤条件如下：<li> resource-id - String - 是否必填：否 - （过滤条件）按照抵扣流量资源的唯一 ID 过滤。</li><li> resource-type - String - 是否必填：否 - （过滤条件）按照资源类型过滤，资源类型包括 CVM 和 EIP </li>
+        :type Filters: list of Filter
+        :param _OrderField: 排序条件。该参数仅支持根据抵扣量排序，传值为 deduction
+        :type OrderField: str
+        :param _OrderType: 排序类型，仅支持0和1，0-降序，1-升序。不传默认为0
+        :type OrderType: int
+        :param _StartTime: 开始时间。不传默认为当前时间往前推30天
+        :type StartTime: str
+        :param _EndTime: 结束时间。不传默认为当前时间
+        :type EndTime: str
+        :param _Offset: 分页参数
+        :type Offset: int
+        :param _Limit: 分页参数
+        :type Limit: int
+        """
+        self._TrafficPackageId = None
+        self._Filters = None
+        self._OrderField = None
+        self._OrderType = None
+        self._StartTime = None
+        self._EndTime = None
+        self._Offset = None
+        self._Limit = None
+
+    @property
+    def TrafficPackageId(self):
+        return self._TrafficPackageId
+
+    @TrafficPackageId.setter
+    def TrafficPackageId(self, TrafficPackageId):
+        self._TrafficPackageId = TrafficPackageId
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
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def OrderType(self):
+        return self._OrderType
+
+    @OrderType.setter
+    def OrderType(self, OrderType):
+        self._OrderType = OrderType
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
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
+
+    def _deserialize(self, params):
+        self._TrafficPackageId = params.get("TrafficPackageId")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._OrderField = params.get("OrderField")
+        self._OrderType = params.get("OrderType")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
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
+class DescribeSpecificTrafficPackageUsedDetailsResponse(AbstractModel):
+    """DescribeSpecificTrafficPackageUsedDetails返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 符合查询条件的共享流量包用量明细的总数
+        :type TotalCount: int
+        :param _UsedDetailSet: 共享流量包用量明细列表
+        :type UsedDetailSet: list of UsedDetail
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._UsedDetailSet = None
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
+    def UsedDetailSet(self):
+        return self._UsedDetailSet
+
+    @UsedDetailSet.setter
+    def UsedDetailSet(self, UsedDetailSet):
+        self._UsedDetailSet = UsedDetailSet
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
+        if params.get("UsedDetailSet") is not None:
+            self._UsedDetailSet = []
+            for item in params.get("UsedDetailSet"):
+                obj = UsedDetail()
+                obj._deserialize(item)
+                self._UsedDetailSet.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeSubnetResourceDashboardRequest(AbstractModel):
     """DescribeSubnetResourceDashboard请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -21776,19 +21952,22 @@
         :type Filters: list of Filter
         :param _Offset: 偏移量，默认为0。
         :type Offset: int
         :param _Limit: 单页返回数量，默认为20，最大值为100。
         :type Limit: int
         :param _EndPointServiceIds: 终端节点服务ID。不支持同时传入参数 EndPointServiceIds and Filters。
         :type EndPointServiceIds: list of str
+        :param _IsListAuthorizedEndPointService: <li>不支持同时传入参数 Filters 。</li> <li>列出授权给当前账号的的终端节点服务信息。可以配合EndPointServiceIds参数进行过滤，那些终端节点服务授权了该账户。</li>
+        :type IsListAuthorizedEndPointService: bool
         """
         self._Filters = None
         self._Offset = None
         self._Limit = None
         self._EndPointServiceIds = None
+        self._IsListAuthorizedEndPointService = None
 
     @property
     def Filters(self):
         return self._Filters
 
     @Filters.setter
     def Filters(self, Filters):
@@ -21814,25 +21993,34 @@
     def EndPointServiceIds(self):
         return self._EndPointServiceIds
 
     @EndPointServiceIds.setter
     def EndPointServiceIds(self, EndPointServiceIds):
         self._EndPointServiceIds = EndPointServiceIds
 
+    @property
+    def IsListAuthorizedEndPointService(self):
+        return self._IsListAuthorizedEndPointService
+
+    @IsListAuthorizedEndPointService.setter
+    def IsListAuthorizedEndPointService(self, IsListAuthorizedEndPointService):
+        self._IsListAuthorizedEndPointService = IsListAuthorizedEndPointService
+
 
     def _deserialize(self, params):
         if params.get("Filters") is not None:
             self._Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self._Filters.append(obj)
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._EndPointServiceIds = params.get("EndPointServiceIds")
+        self._IsListAuthorizedEndPointService = params.get("IsListAuthorizedEndPointService")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -40983,14 +41171,73 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class TrafficFlow(AbstractModel):
+    """流量描述。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Value: 实际流量，单位为 字节
+        :type Value: int
+        :param _FormatValue: 格式化后的流量，单位见参数 FormatUnit
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FormatValue: float
+        :param _FormatUnit: 格式化后流量的单位
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FormatUnit: str
+        """
+        self._Value = None
+        self._FormatValue = None
+        self._FormatUnit = None
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+    @property
+    def FormatValue(self):
+        return self._FormatValue
+
+    @FormatValue.setter
+    def FormatValue(self, FormatValue):
+        self._FormatValue = FormatValue
+
+    @property
+    def FormatUnit(self):
+        return self._FormatUnit
+
+    @FormatUnit.setter
+    def FormatUnit(self, FormatUnit):
+        self._FormatUnit = FormatUnit
+
+
+    def _deserialize(self, params):
+        self._Value = params.get("Value")
+        self._FormatValue = params.get("FormatValue")
+        self._FormatUnit = params.get("FormatUnit")
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
 class TrafficPackage(AbstractModel):
     """流量包信息描述类型
 
     """
 
     def __init__(self):
         r"""
@@ -41614,14 +41861,162 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class UsedDetail(AbstractModel):
+    """共享流量包用量明细
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TrafficPackageId: 流量包唯一ID
+        :type TrafficPackageId: str
+        :param _TrafficPackageName: 流量包名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TrafficPackageName: str
+        :param _TotalAmount: 流量包总量
+        :type TotalAmount: :class:`tencentcloud.vpc.v20170312.models.TrafficFlow`
+        :param _Deduction: 本次抵扣
+        :type Deduction: :class:`tencentcloud.vpc.v20170312.models.TrafficFlow`
+        :param _RemainingAmount: 本次抵扣后剩余量
+        :type RemainingAmount: :class:`tencentcloud.vpc.v20170312.models.TrafficFlow`
+        :param _Time: 抵扣时间
+        :type Time: str
+        :param _ResourceType: 资源类型。可能的值: CVM, LB, NAT, HAVIP, EIP
+        :type ResourceType: str
+        :param _ResourceId: 资源ID
+        :type ResourceId: str
+        :param _ResourceName: 资源名称
+        :type ResourceName: str
+        :param _Deadline: 流量包到期时间
+        :type Deadline: str
+        """
+        self._TrafficPackageId = None
+        self._TrafficPackageName = None
+        self._TotalAmount = None
+        self._Deduction = None
+        self._RemainingAmount = None
+        self._Time = None
+        self._ResourceType = None
+        self._ResourceId = None
+        self._ResourceName = None
+        self._Deadline = None
+
+    @property
+    def TrafficPackageId(self):
+        return self._TrafficPackageId
+
+    @TrafficPackageId.setter
+    def TrafficPackageId(self, TrafficPackageId):
+        self._TrafficPackageId = TrafficPackageId
+
+    @property
+    def TrafficPackageName(self):
+        return self._TrafficPackageName
+
+    @TrafficPackageName.setter
+    def TrafficPackageName(self, TrafficPackageName):
+        self._TrafficPackageName = TrafficPackageName
+
+    @property
+    def TotalAmount(self):
+        return self._TotalAmount
+
+    @TotalAmount.setter
+    def TotalAmount(self, TotalAmount):
+        self._TotalAmount = TotalAmount
+
+    @property
+    def Deduction(self):
+        return self._Deduction
+
+    @Deduction.setter
+    def Deduction(self, Deduction):
+        self._Deduction = Deduction
+
+    @property
+    def RemainingAmount(self):
+        return self._RemainingAmount
+
+    @RemainingAmount.setter
+    def RemainingAmount(self, RemainingAmount):
+        self._RemainingAmount = RemainingAmount
+
+    @property
+    def Time(self):
+        return self._Time
+
+    @Time.setter
+    def Time(self, Time):
+        self._Time = Time
+
+    @property
+    def ResourceType(self):
+        return self._ResourceType
+
+    @ResourceType.setter
+    def ResourceType(self, ResourceType):
+        self._ResourceType = ResourceType
+
+    @property
+    def ResourceId(self):
+        return self._ResourceId
+
+    @ResourceId.setter
+    def ResourceId(self, ResourceId):
+        self._ResourceId = ResourceId
+
+    @property
+    def ResourceName(self):
+        return self._ResourceName
+
+    @ResourceName.setter
+    def ResourceName(self, ResourceName):
+        self._ResourceName = ResourceName
+
+    @property
+    def Deadline(self):
+        return self._Deadline
+
+    @Deadline.setter
+    def Deadline(self, Deadline):
+        self._Deadline = Deadline
+
+
+    def _deserialize(self, params):
+        self._TrafficPackageId = params.get("TrafficPackageId")
+        self._TrafficPackageName = params.get("TrafficPackageName")
+        if params.get("TotalAmount") is not None:
+            self._TotalAmount = TrafficFlow()
+            self._TotalAmount._deserialize(params.get("TotalAmount"))
+        if params.get("Deduction") is not None:
+            self._Deduction = TrafficFlow()
+            self._Deduction._deserialize(params.get("Deduction"))
+        if params.get("RemainingAmount") is not None:
+            self._RemainingAmount = TrafficFlow()
+            self._RemainingAmount._deserialize(params.get("RemainingAmount"))
+        self._Time = params.get("Time")
+        self._ResourceType = params.get("ResourceType")
+        self._ResourceId = params.get("ResourceId")
+        self._ResourceName = params.get("ResourceName")
+        self._Deadline = params.get("Deadline")
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
 class Vpc(AbstractModel):
     """私有网络(VPC)对象。
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.945/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.945/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.944/README.rst` & `tencentcloud-sdk-python-vpc-3.0.945/README.rst`

 * *Files identical despite different names*

