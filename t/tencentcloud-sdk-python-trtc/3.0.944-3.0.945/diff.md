# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.944.tar", last modified: Thu Jul 27 02:26:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.945.tar", last modified: Fri Jul 28 00:38:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.944.tar` & `tencentcloud-sdk-python-trtc-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9679 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65738 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)   287958 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:26:44.000000 tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65738 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)   289132 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:38:35.000000 tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/setup.py` & `tencentcloud-sdk-python-trtc-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/trtc/v20190722/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4164,40 +4164,43 @@
         :type ImageHeight: int
         :param _LocationX: 子画面在输出时的X偏移，单位为像素值，LocationX与ImageWidth之和不能超过混流输出的总宽度，不填默认为0。
         :type LocationX: int
         :param _LocationY: 子画面在输出时的Y偏移，单位为像素值，LocationY与ImageHeight之和不能超过混流输出的总高度，不填默认为0。
         :type LocationY: int
         :param _ZOrder: 子画面在输出时的层级，不填默认为0。
         :type ZOrder: int
-        :param _RenderMode: 子画面在输出时的显示模式：0为裁剪，1为缩放，2为缩放并显示黑底。不填默认为0。
+        :param _RenderMode: 子画面在输出时的显示模式：0为裁剪，1为缩放并显示背景，2为缩放并显示黑底。不填默认为0。
         :type RenderMode: int
         :param _BackGroundColor: 【此参数配置无效，暂不支持】子画面的背景颜色，常用的颜色有：
 红色：0xcc0033。
 黄色：0xcc9900。
 绿色：0xcccc33。
 蓝色：0x99CCFF。
 黑色：0x000000。
 白色：0xFFFFFF。
 灰色：0x999999。
         :type BackGroundColor: str
         :param _BackgroundImageUrl: 子画面的背景图url，填写该参数，当用户关闭摄像头或未进入TRTC房间时，会在布局位置填充为指定图片。若指定图片与布局位置尺寸比例不一致，则会对图片进行拉伸处理，优先级高于BackGroundColor。
         :type BackgroundImageUrl: str
         :param _CustomCrop: 客户自定义裁剪，针对原始输入流裁剪
         :type CustomCrop: :class:`tencentcloud.trtc.v20190722.models.McuCustomCrop`
+        :param _BackgroundRenderMode: 子背景图在输出时的显示模式：0为裁剪，1为缩放并显示背景，2为缩放并显示黑底，3为变比例伸缩。不填默认为3。
+        :type BackgroundRenderMode: int
         """
         self._UserMediaStream = None
         self._ImageWidth = None
         self._ImageHeight = None
         self._LocationX = None
         self._LocationY = None
         self._ZOrder = None
         self._RenderMode = None
         self._BackGroundColor = None
         self._BackgroundImageUrl = None
         self._CustomCrop = None
+        self._BackgroundRenderMode = None
 
     @property
     def UserMediaStream(self):
         return self._UserMediaStream
 
     @UserMediaStream.setter
     def UserMediaStream(self, UserMediaStream):
@@ -4271,14 +4274,22 @@
     def CustomCrop(self):
         return self._CustomCrop
 
     @CustomCrop.setter
     def CustomCrop(self, CustomCrop):
         self._CustomCrop = CustomCrop
 
+    @property
+    def BackgroundRenderMode(self):
+        return self._BackgroundRenderMode
+
+    @BackgroundRenderMode.setter
+    def BackgroundRenderMode(self, BackgroundRenderMode):
+        self._BackgroundRenderMode = BackgroundRenderMode
+
 
     def _deserialize(self, params):
         if params.get("UserMediaStream") is not None:
             self._UserMediaStream = UserMediaStream()
             self._UserMediaStream._deserialize(params.get("UserMediaStream"))
         self._ImageWidth = params.get("ImageWidth")
         self._ImageHeight = params.get("ImageHeight")
@@ -4287,14 +4298,15 @@
         self._ZOrder = params.get("ZOrder")
         self._RenderMode = params.get("RenderMode")
         self._BackGroundColor = params.get("BackGroundColor")
         self._BackgroundImageUrl = params.get("BackgroundImageUrl")
         if params.get("CustomCrop") is not None:
             self._CustomCrop = McuCustomCrop()
             self._CustomCrop._deserialize(params.get("CustomCrop"))
+        self._BackgroundRenderMode = params.get("BackgroundRenderMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4689,20 +4701,23 @@
 白色：0xFFFFFF。
 灰色：0x999999。
         :type BackGroundColor: str
         :param _BackgroundImageUrl: 整个画布的背景图url，优先级高于BackGroundColor。
         :type BackgroundImageUrl: str
         :param _WaterMarkList: 混流布局的水印参数。
         :type WaterMarkList: list of McuWaterMarkParams
+        :param _BackgroundRenderMode: 背景图在输出时的显示模式：0为裁剪，1为缩放并显示黑底，2为变比例伸缩。后台默认为变比例伸缩。
+        :type BackgroundRenderMode: int
         """
         self._VideoEncode = None
         self._LayoutParams = None
         self._BackGroundColor = None
         self._BackgroundImageUrl = None
         self._WaterMarkList = None
+        self._BackgroundRenderMode = None
 
     @property
     def VideoEncode(self):
         return self._VideoEncode
 
     @VideoEncode.setter
     def VideoEncode(self, VideoEncode):
@@ -4736,14 +4751,22 @@
     def WaterMarkList(self):
         return self._WaterMarkList
 
     @WaterMarkList.setter
     def WaterMarkList(self, WaterMarkList):
         self._WaterMarkList = WaterMarkList
 
+    @property
+    def BackgroundRenderMode(self):
+        return self._BackgroundRenderMode
+
+    @BackgroundRenderMode.setter
+    def BackgroundRenderMode(self, BackgroundRenderMode):
+        self._BackgroundRenderMode = BackgroundRenderMode
+
 
     def _deserialize(self, params):
         if params.get("VideoEncode") is not None:
             self._VideoEncode = VideoEncode()
             self._VideoEncode._deserialize(params.get("VideoEncode"))
         if params.get("LayoutParams") is not None:
             self._LayoutParams = McuLayoutParams()
@@ -4752,14 +4775,15 @@
         self._BackgroundImageUrl = params.get("BackgroundImageUrl")
         if params.get("WaterMarkList") is not None:
             self._WaterMarkList = []
             for item in params.get("WaterMarkList"):
                 obj = McuWaterMarkParams()
                 obj._deserialize(item)
                 self._WaterMarkList.append(obj)
+        self._BackgroundRenderMode = params.get("BackgroundRenderMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/README.rst` & `tencentcloud-sdk-python-trtc-3.0.945/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.944/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.945/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

