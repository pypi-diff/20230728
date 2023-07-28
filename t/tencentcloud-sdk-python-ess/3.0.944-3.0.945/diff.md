# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.944.tar", last modified: Thu Jul 27 02:15:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.945.tar", last modified: Fri Jul 28 00:28:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.944.tar` & `tencentcloud-sdk-python-ess-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    65423 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   453453 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:15:38.000000 tencentcloud-sdk-python-ess-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    65932 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   453727 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.944/setup.py` & `tencentcloud-sdk-python-ess-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,16 +448,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateFlowSignUrl(self, request):
-        """创建个人H5签署链接，请联系客户经理申请使用 <br/>
-        该接口用于发起合同后，生成C端签署人的签署链接 <br/>
+        """创建个人H5签署链接，请联系客户经理申请开通使用, 否则调用会返回失败 <br/>
+
+        该接口用于发起合同后，生成个人签署人的签署链接, 暂时不支持企业端签署 <br/>
+
         注意：该接口目前签署人类型仅支持个人签署方（PERSON） <br/>
         注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
         注意：该接口返回的签署链接是用于APP集成的场景，支持APP打开或浏览器直接打开，不支持微信小程序嵌入。微信小程序请使用小程序跳转或半屏弹窗的方式<br/>
 
         :param request: Request instance for CreateFlowSignUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlResponse`
@@ -1029,16 +1031,26 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowTemplates(self, request):
-        """当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。<br/>
-        该接口常用来配合“创建电子文档”接口作为前置的接口使用。<br/>
+        """本接口用于查询本企业模板列表。
+
+        当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。
+
+        > **适用场景**
+        >  该接口常用来配合“模板发起合同-创建电子文档”接口作为前置的接口使用。
+        >  一个模板通常会包含以下结构信息
+        >- 模板基本信息
+        >- 发起方参与信息Promoter、签署参与方 Recipients，后者会在模板发起合同时用于指定参与方
+        >- 填写控件 Components
+        >- 签署控件 SignComponents
+        >- 生成模板的文件基础信息 FileInfos
 
         :param request: Request instance for DescribeFlowTemplates.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowTemplatesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowTemplatesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.944/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3821,15 +3821,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FlowId: 流程编号
         :type FlowId: str
-        :param _FlowApproverInfos: 流程签署人，其中ApproverName，ApproverMobile和ApproverType必传，其他可不传，ApproverType目前只支持个人类型的签署人。还需注意签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
+        :param _FlowApproverInfos: 流程签署人列表，其中结构体的ApproverName，ApproverMobile和ApproverType必传，其他可不传，ApproverType目前只支持个人类型的签署人。
+
+签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
         :type FlowApproverInfos: list of FlowCreateApprover
         :param _Operator: 用户信息，此结构体UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Organization: 机构信息，暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
@@ -7510,27 +7512,35 @@
 class DescribeFlowTemplatesRequest(AbstractModel):
     """DescribeFlowTemplates请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Operator: 调用方用户信息，userId 必填
-        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
-        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
-        :param _ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
+        :param _Operator: 调用方员工/经办人信息
+UserId 必填，在企业控制台组织架构中可以查到员工的UserId
+注：请保证对应
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param _Agent: 代理相关应用信息
+如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param _ContentType: 查询内容类型
+0-模板列表及详情（默认）
+1-仅模板列表
         :type ContentType: int
-        :param _Filters: 搜索条件，具体参考Filter结构体。本接口取值：template-id：按照【 **模板唯一标识** 】进行过滤
+        :param _Filters: 搜索条件，本字段用于指定模板Id进行查询。
+Key：template-id
+Values：需要查询的模板Id列表
         :type Filters: list of Filter
-        :param _Offset: 查询偏移位置，默认0
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默从第一页返回。页码从0开始，即首页为0。
         :type Offset: int
-        :param _Limit: 查询个数，默认20，最大200
+        :param _Limit: 指定每页多少条数据，如果不传默认为20，单页最大200。
         :type Limit: int
-        :param _ApplicationId: ApplicationId不为空，查询指定应用下的模板列表
+        :param _ApplicationId: 用于查询指定应用号下单模板列表。
+ApplicationId不为空，查询指定应用下的模板列表
 ApplicationId为空，查询所有应用下的模板列表
         :type ApplicationId: str
         :param _IsChannel: 默认为false，查询SaaS模板库列表；
 为true，查询第三方应用集成平台企业模板库管理列表
         :type IsChannel: bool
         :param _Organization: 暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.944/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.945/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.944/README.rst` & `tencentcloud-sdk-python-ess-3.0.945/README.rst`

 * *Files identical despite different names*

