# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.944.tar", last modified: Thu Jul 27 02:20:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.945.tar", last modified: Fri Jul 28 00:32:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.944.tar` & `tencentcloud-sdk-python-ocr-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115943 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   821044 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:20:30.000000 tencentcloud-sdk-python-ocr-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115943 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   821044 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/setup.py` & `tencentcloud-sdk-python-ocr-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateAIFormTask(self, request):
         """本接口可创建智能表单录入任务，支持多个识别图片和PDF的URL上传，返回含有识别内容的操作页面URL。
 
-        智能表单录入产品提供高准确率的表单识别技术和人工核对工具，支持自定义字段，将识别结果自动填入到自定义条目中，并提供人工操作工具，完成整个表单识别过程。适用性强，可对票据、合同、货单等文件的识别，适用于金融、货代、保险、档案等领域。本产品免费公测中，您可以点击demo（超连接：https://ocr.smartform.cloud.tencent.com/）试用，如需购买请与商务团队联系。
+        智能表单录入产品提供高准确率的表单识别技术和人工核对工具，支持自定义字段，将识别结果自动填入到自定义条目中，并提供人工操作工具，完成整个表单识别过程。适用性强，可对票据、合同、货单等文件的识别，适用于金融、货代、保险、档案等领域。本产品免费公测中，您可以点击demo（超链接：https://ocr.smartform.cloud.tencent.com/）试用，如需购买请与商务团队联系。
 
         :param request: Request instance for CreateAIFormTask.
         :type request: :class:`tencentcloud.ocr.v20181119.models.CreateAIFormTaskRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.CreateAIFormTaskResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.944/README.rst` & `tencentcloud-sdk-python-ocr-3.0.945/README.rst`

 * *Files identical despite different names*

