# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.944.tar", last modified: Thu Jul 27 02:10:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.945.tar", last modified: Fri Jul 28 00:23:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.944.tar` & `tencentcloud-sdk-python-ccc-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36562 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   232215 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:10:45.000000 tencentcloud-sdk-python-ccc-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36562 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   232988 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:23:15.000000 tencentcloud-sdk-python-ccc-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/setup.py` & `tencentcloud-sdk-python-ccc-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.945/tencentcloud/ccc/v20200210/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6358,20 +6358,24 @@
         :type Name: str
         :param _StaffBuyNum: 坐席购买数（还在有效期内）
         :type StaffBuyNum: int
         :param _StaffBuyList: 坐席购买列表 （还在有效期内）
         :type StaffBuyList: list of StaffBuyInfo
         :param _PhoneNumBuyList: 号码购买列表
         :type PhoneNumBuyList: list of PhoneNumBuyInfo
+        :param _SipBuyNum: 办公电话购买数（还在有效期内）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SipBuyNum: int
         """
         self._SdkAppId = None
         self._Name = None
         self._StaffBuyNum = None
         self._StaffBuyList = None
         self._PhoneNumBuyList = None
+        self._SipBuyNum = None
 
     @property
     def SdkAppId(self):
         return self._SdkAppId
 
     @SdkAppId.setter
     def SdkAppId(self, SdkAppId):
@@ -6405,14 +6409,22 @@
     def PhoneNumBuyList(self):
         return self._PhoneNumBuyList
 
     @PhoneNumBuyList.setter
     def PhoneNumBuyList(self, PhoneNumBuyList):
         self._PhoneNumBuyList = PhoneNumBuyList
 
+    @property
+    def SipBuyNum(self):
+        return self._SipBuyNum
+
+    @SipBuyNum.setter
+    def SipBuyNum(self, SipBuyNum):
+        self._SipBuyNum = SipBuyNum
+
 
     def _deserialize(self, params):
         self._SdkAppId = params.get("SdkAppId")
         self._Name = params.get("Name")
         self._StaffBuyNum = params.get("StaffBuyNum")
         if params.get("StaffBuyList") is not None:
             self._StaffBuyList = []
@@ -6422,14 +6434,15 @@
                 self._StaffBuyList.append(obj)
         if params.get("PhoneNumBuyList") is not None:
             self._PhoneNumBuyList = []
             for item in params.get("PhoneNumBuyList"):
                 obj = PhoneNumBuyInfo()
                 obj._deserialize(item)
                 self._PhoneNumBuyList.append(obj)
+        self._SipBuyNum = params.get("SipBuyNum")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6998,18 +7011,22 @@
         r"""
         :param _Num: 购买坐席数量
         :type Num: int
         :param _BuyTime: 购买时间戳
         :type BuyTime: int
         :param _EndTime: 截止时间戳
         :type EndTime: int
+        :param _SipNum: 购买办公电话数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SipNum: int
         """
         self._Num = None
         self._BuyTime = None
         self._EndTime = None
+        self._SipNum = None
 
     @property
     def Num(self):
         return self._Num
 
     @Num.setter
     def Num(self, Num):
@@ -7027,19 +7044,28 @@
     def EndTime(self):
         return self._EndTime
 
     @EndTime.setter
     def EndTime(self, EndTime):
         self._EndTime = EndTime
 
+    @property
+    def SipNum(self):
+        return self._SipNum
+
+    @SipNum.setter
+    def SipNum(self, SipNum):
+        self._SipNum = SipNum
+
 
     def _deserialize(self, params):
         self._Num = params.get("Num")
         self._BuyTime = params.get("BuyTime")
         self._EndTime = params.get("EndTime")
+        self._SipNum = params.get("SipNum")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.945/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.944/README.rst` & `tencentcloud-sdk-python-ccc-3.0.945/README.rst`

 * *Files identical despite different names*

