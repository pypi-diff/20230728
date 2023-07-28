# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.944.tar", last modified: Thu Jul 27 02:24:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.945.tar", last modified: Fri Jul 28 00:36:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.944.tar` & `tencentcloud-sdk-python-tcss-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   318406 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1689506 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 02:24:31.000000 tencentcloud-sdk-python-tcss-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   318406 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1696870 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-28 00:36:35.000000 tencentcloud-sdk-python-tcss-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.945/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/setup.py` & `tencentcloud-sdk-python-tcss-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2292,25 +2292,28 @@
         :type RegistryVersion: str
         :param _RegistryRegion: 区域，列表：default（默认）
         :type RegistryRegion: str
         :param _SpeedLimit: 限速
         :type SpeedLimit: int
         :param _Insecure: 安全模式（证书校验）：0（默认） 非安全模式（跳过证书校验）：1
         :type Insecure: int
+        :param _ConnDetectConfig: 联通性检测的记录ID
+        :type ConnDetectConfig: list of ConnDetectConfig
         """
         self._Name = None
         self._Username = None
         self._Password = None
         self._Url = None
         self._RegistryType = None
         self._NetType = None
         self._RegistryVersion = None
         self._RegistryRegion = None
         self._SpeedLimit = None
         self._Insecure = None
+        self._ConnDetectConfig = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -2384,26 +2387,40 @@
     def Insecure(self):
         return self._Insecure
 
     @Insecure.setter
     def Insecure(self, Insecure):
         self._Insecure = Insecure
 
+    @property
+    def ConnDetectConfig(self):
+        return self._ConnDetectConfig
+
+    @ConnDetectConfig.setter
+    def ConnDetectConfig(self, ConnDetectConfig):
+        self._ConnDetectConfig = ConnDetectConfig
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Username = params.get("Username")
         self._Password = params.get("Password")
         self._Url = params.get("Url")
         self._RegistryType = params.get("RegistryType")
         self._NetType = params.get("NetType")
         self._RegistryVersion = params.get("RegistryVersion")
         self._RegistryRegion = params.get("RegistryRegion")
         self._SpeedLimit = params.get("SpeedLimit")
         self._Insecure = params.get("Insecure")
+        if params.get("ConnDetectConfig") is not None:
+            self._ConnDetectConfig = []
+            for item in params.get("ConnDetectConfig"):
+                obj = ConnDetectConfig()
+                obj._deserialize(item)
+                self._ConnDetectConfig.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7982,14 +7999,59 @@
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._Result = params.get("Result")
         self._RequestId = params.get("RequestId")
 
 
+class ConnDetectConfig(AbstractModel):
+    """联通性检测配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Quuid: 主机quuid
+        :type Quuid: str
+        :param _Uuid: 主机uuid
+        :type Uuid: str
+        """
+        self._Quuid = None
+        self._Uuid = None
+
+    @property
+    def Quuid(self):
+        return self._Quuid
+
+    @Quuid.setter
+    def Quuid(self, Quuid):
+        self._Quuid = Quuid
+
+    @property
+    def Uuid(self):
+        return self._Uuid
+
+    @Uuid.setter
+    def Uuid(self, Uuid):
+        self._Uuid = Uuid
+
+
+    def _deserialize(self, params):
+        self._Quuid = params.get("Quuid")
+        self._Uuid = params.get("Uuid")
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
 class ContainerInfo(AbstractModel):
     """容器列表集合
 
     """
 
     def __init__(self):
         r"""
@@ -8876,29 +8938,41 @@
 class CreateAssetImageRegistryScanTaskOneKeyResponse(AbstractModel):
     """CreateAssetImageRegistryScanTaskOneKey返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param _TaskID: 扫描任务id
+        :type TaskID: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self._TaskID = None
         self._RequestId = None
 
     @property
+    def TaskID(self):
+        return self._TaskID
+
+    @TaskID.setter
+    def TaskID(self, TaskID):
+        self._TaskID = TaskID
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
+        self._TaskID = params.get("TaskID")
         self._RequestId = params.get("RequestId")
 
 
 class CreateAssetImageRegistryScanTaskRequest(AbstractModel):
     """CreateAssetImageRegistryScanTask请求参数结构体
 
     """
@@ -9016,29 +9090,41 @@
 class CreateAssetImageRegistryScanTaskResponse(AbstractModel):
     """CreateAssetImageRegistryScanTask返回参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param _TaskID: 返回的任务ID
+        :type TaskID: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
+        self._TaskID = None
         self._RequestId = None
 
     @property
+    def TaskID(self):
+        return self._TaskID
+
+    @TaskID.setter
+    def TaskID(self, TaskID):
+        self._TaskID = TaskID
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
+        self._TaskID = params.get("TaskID")
         self._RequestId = params.get("RequestId")
 
 
 class CreateAssetImageScanSettingRequest(AbstractModel):
     """CreateAssetImageScanSetting请求参数结构体
 
     """
@@ -20266,38 +20352,44 @@
         :param _Url: 仓库url
         :type Url: str
         :param _RegistryType: 仓库类型，列表：harbor
         :type RegistryType: str
         :param _RegistryVersion: 仓库版本
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistryVersion: str
-        :param _NetType: 网络类型，列表：public（公网）
+        :param _NetType: 网络类型，列表：public（公网）,private（私网）
         :type NetType: str
         :param _RegistryRegion: 区域，列表:default（默认）
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistryRegion: str
         :param _SpeedLimit: 限速
 注意：此字段可能返回 null，表示取不到有效值。
         :type SpeedLimit: int
         :param _Insecure: 安全模式（证书校验）：0（默认） 非安全模式（跳过证书校验）：1
 注意：此字段可能返回 null，表示取不到有效值。
         :type Insecure: int
+        :param _ConnDetectDetail: 联通性检测结果详情
+        :type ConnDetectDetail: list of RegistryConnDetectResult
+        :param _InstanceID: tcr情况下instance_id
+        :type InstanceID: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Name = None
         self._Username = None
         self._Password = None
         self._Url = None
         self._RegistryType = None
         self._RegistryVersion = None
         self._NetType = None
         self._RegistryRegion = None
         self._SpeedLimit = None
         self._Insecure = None
+        self._ConnDetectDetail = None
+        self._InstanceID = None
         self._RequestId = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
@@ -20373,14 +20465,30 @@
         return self._Insecure
 
     @Insecure.setter
     def Insecure(self, Insecure):
         self._Insecure = Insecure
 
     @property
+    def ConnDetectDetail(self):
+        return self._ConnDetectDetail
+
+    @ConnDetectDetail.setter
+    def ConnDetectDetail(self, ConnDetectDetail):
+        self._ConnDetectDetail = ConnDetectDetail
+
+    @property
+    def InstanceID(self):
+        return self._InstanceID
+
+    @InstanceID.setter
+    def InstanceID(self, InstanceID):
+        self._InstanceID = InstanceID
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -20392,14 +20500,21 @@
         self._Url = params.get("Url")
         self._RegistryType = params.get("RegistryType")
         self._RegistryVersion = params.get("RegistryVersion")
         self._NetType = params.get("NetType")
         self._RegistryRegion = params.get("RegistryRegion")
         self._SpeedLimit = params.get("SpeedLimit")
         self._Insecure = params.get("Insecure")
+        if params.get("ConnDetectDetail") is not None:
+            self._ConnDetectDetail = []
+            for item in params.get("ConnDetectDetail"):
+                obj = RegistryConnDetectResult()
+                obj._deserialize(item)
+                self._ConnDetectDetail.append(obj)
+        self._InstanceID = params.get("InstanceID")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeAssetImageRegistryRegistryListRequest(AbstractModel):
     """DescribeAssetImageRegistryRegistryList请求参数结构体
 
     """
@@ -20749,18 +20864,21 @@
         r"""
         :param _Images: 需要获取进度的镜像列表
         :type Images: list of ImageInfo
         :param _All: 是否获取全部镜像
         :type All: bool
         :param _Id: 需要获取进度的镜像列表Id
         :type Id: list of int non-negative
+        :param _TaskID: 获取进度的任务ID
+        :type TaskID: int
         """
         self._Images = None
         self._All = None
         self._Id = None
+        self._TaskID = None
 
     @property
     def Images(self):
         return self._Images
 
     @Images.setter
     def Images(self, Images):
@@ -20778,24 +20896,33 @@
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
         self._Id = Id
 
+    @property
+    def TaskID(self):
+        return self._TaskID
+
+    @TaskID.setter
+    def TaskID(self, TaskID):
+        self._TaskID = TaskID
+
 
     def _deserialize(self, params):
         if params.get("Images") is not None:
             self._Images = []
             for item in params.get("Images"):
                 obj = ImageInfo()
                 obj._deserialize(item)
                 self._Images.append(obj)
         self._All = params.get("All")
         self._Id = params.get("Id")
+        self._TaskID = params.get("TaskID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -46256,18 +46383,21 @@
         r"""
         :param _All: 是否扫描全部镜像
         :type All: bool
         :param _Images: 扫描的镜像列表
         :type Images: list of ImageInfo
         :param _Id: 扫描的镜像列表Id
         :type Id: list of int non-negative
+        :param _TaskID: 停止的任务ID
+        :type TaskID: int
         """
         self._All = None
         self._Images = None
         self._Id = None
+        self._TaskID = None
 
     @property
     def All(self):
         return self._All
 
     @All.setter
     def All(self, All):
@@ -46285,24 +46415,33 @@
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
         self._Id = Id
 
+    @property
+    def TaskID(self):
+        return self._TaskID
+
+    @TaskID.setter
+    def TaskID(self, TaskID):
+        self._TaskID = TaskID
+
 
     def _deserialize(self, params):
         self._All = params.get("All")
         if params.get("Images") is not None:
             self._Images = []
             for item in params.get("Images"):
                 obj = ImageInfo()
                 obj._deserialize(item)
                 self._Images.append(obj)
         self._Id = params.get("Id")
+        self._TaskID = params.get("TaskID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -46349,21 +46488,24 @@
         :type Id: list of int non-negative
         :param _Filters: 过滤条件
         :type Filters: list of AssetFilters
         :param _ExcludeImageList: 不要扫描的镜像列表，与Filters配合使用
         :type ExcludeImageList: list of int non-negative
         :param _OnlyScanLatest: 是否仅扫描各repository最新版本的镜像
         :type OnlyScanLatest: bool
+        :param _TaskID: 停止的任务ID
+        :type TaskID: int
         """
         self._All = None
         self._Images = None
         self._Id = None
         self._Filters = None
         self._ExcludeImageList = None
         self._OnlyScanLatest = None
+        self._TaskID = None
 
     @property
     def All(self):
         return self._All
 
     @All.setter
     def All(self, All):
@@ -46405,14 +46547,22 @@
     def OnlyScanLatest(self):
         return self._OnlyScanLatest
 
     @OnlyScanLatest.setter
     def OnlyScanLatest(self, OnlyScanLatest):
         self._OnlyScanLatest = OnlyScanLatest
 
+    @property
+    def TaskID(self):
+        return self._TaskID
+
+    @TaskID.setter
+    def TaskID(self, TaskID):
+        self._TaskID = TaskID
+
 
     def _deserialize(self, params):
         self._All = params.get("All")
         if params.get("Images") is not None:
             self._Images = []
             for item in params.get("Images"):
                 obj = ImageInfo()
@@ -46423,14 +46573,15 @@
             self._Filters = []
             for item in params.get("Filters"):
                 obj = AssetFilters()
                 obj._deserialize(item)
                 self._Filters.append(obj)
         self._ExcludeImageList = params.get("ExcludeImageList")
         self._OnlyScanLatest = params.get("OnlyScanLatest")
+        self._TaskID = params.get("TaskID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -50954,14 +51105,107 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RegistryConnDetectResult(AbstractModel):
+    """镜像仓库联通性检测结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Quuid: 联通性检测的主机quuid 或者 backend
+        :type Quuid: str
+        :param _Uuid: 联通性检测的主机uuid 或者 backend
+        :type Uuid: str
+        :param _ConnDetectStatus: 检测结果状态
+        :type ConnDetectStatus: str
+        :param _ConnDetectMessage: 检测结果信息
+        :type ConnDetectMessage: str
+        :param _Solution: 失败的解决方案
+        :type Solution: str
+        :param _FailReason: 失败原因
+        :type FailReason: str
+        """
+        self._Quuid = None
+        self._Uuid = None
+        self._ConnDetectStatus = None
+        self._ConnDetectMessage = None
+        self._Solution = None
+        self._FailReason = None
+
+    @property
+    def Quuid(self):
+        return self._Quuid
+
+    @Quuid.setter
+    def Quuid(self, Quuid):
+        self._Quuid = Quuid
+
+    @property
+    def Uuid(self):
+        return self._Uuid
+
+    @Uuid.setter
+    def Uuid(self, Uuid):
+        self._Uuid = Uuid
+
+    @property
+    def ConnDetectStatus(self):
+        return self._ConnDetectStatus
+
+    @ConnDetectStatus.setter
+    def ConnDetectStatus(self, ConnDetectStatus):
+        self._ConnDetectStatus = ConnDetectStatus
+
+    @property
+    def ConnDetectMessage(self):
+        return self._ConnDetectMessage
+
+    @ConnDetectMessage.setter
+    def ConnDetectMessage(self, ConnDetectMessage):
+        self._ConnDetectMessage = ConnDetectMessage
+
+    @property
+    def Solution(self):
+        return self._Solution
+
+    @Solution.setter
+    def Solution(self, Solution):
+        self._Solution = Solution
+
+    @property
+    def FailReason(self):
+        return self._FailReason
+
+    @FailReason.setter
+    def FailReason(self, FailReason):
+        self._FailReason = FailReason
+
+
+    def _deserialize(self, params):
+        self._Quuid = params.get("Quuid")
+        self._Uuid = params.get("Uuid")
+        self._ConnDetectStatus = params.get("ConnDetectStatus")
+        self._ConnDetectMessage = params.get("ConnDetectMessage")
+        self._Solution = params.get("Solution")
+        self._FailReason = params.get("FailReason")
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
 class RemoveAssetImageRegistryRegistryDetailRequest(AbstractModel):
     """RemoveAssetImageRegistryRegistryDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -55362,25 +55606,28 @@
         :type RegistryVersion: str
         :param _RegistryRegion: 区域，列表：default（默认）
         :type RegistryRegion: str
         :param _SpeedLimit: 限速
         :type SpeedLimit: int
         :param _Insecure: 安全模式（证书校验）：0（默认） 非安全模式（跳过证书校验）：1
         :type Insecure: int
+        :param _ConnDetectConfig: 联通性检测的配置
+        :type ConnDetectConfig: list of ConnDetectConfig
         """
         self._Name = None
         self._Username = None
         self._Password = None
         self._Url = None
         self._RegistryType = None
         self._NetType = None
         self._RegistryVersion = None
         self._RegistryRegion = None
         self._SpeedLimit = None
         self._Insecure = None
+        self._ConnDetectConfig = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -55454,26 +55701,40 @@
     def Insecure(self):
         return self._Insecure
 
     @Insecure.setter
     def Insecure(self, Insecure):
         self._Insecure = Insecure
 
+    @property
+    def ConnDetectConfig(self):
+        return self._ConnDetectConfig
+
+    @ConnDetectConfig.setter
+    def ConnDetectConfig(self, ConnDetectConfig):
+        self._ConnDetectConfig = ConnDetectConfig
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Username = params.get("Username")
         self._Password = params.get("Password")
         self._Url = params.get("Url")
         self._RegistryType = params.get("RegistryType")
         self._NetType = params.get("NetType")
         self._RegistryVersion = params.get("RegistryVersion")
         self._RegistryRegion = params.get("RegistryRegion")
         self._SpeedLimit = params.get("SpeedLimit")
         self._Insecure = params.get("Insecure")
+        if params.get("ConnDetectConfig") is not None:
+            self._ConnDetectConfig = []
+            for item in params.get("ConnDetectConfig"):
+                obj = ConnDetectConfig()
+                obj._deserialize(item)
+                self._ConnDetectConfig.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.944/README.rst` & `tencentcloud-sdk-python-tcss-3.0.945/README.rst`

 * *Files identical despite different names*

