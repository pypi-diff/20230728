# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.944.tar", last modified: Thu Jul 27 02:13:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.945.tar", last modified: Fri Jul 28 00:25:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.944.tar` & `tencentcloud-sdk-python-cwp-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1462983 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)   253300 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:13:18.000000 tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1463419 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)   253300 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:25:47.000000 tencentcloud-sdk-python-cwp-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:25:48.000000 tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/setup.py` & `tencentcloud-sdk-python-cwp-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -41383,14 +41383,17 @@
         :param _SourceType: 是否试用订单.
         :type SourceType: int
         :param _Alias: 资源别名
         :type Alias: str
         :param _Tags: 平台标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of Tags
+        :param _FreezeNum: 冻结数,当为0时 为未冻结,非0 则表示冻结授权数额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FreezeNum: int
         """
         self._LicenseId = None
         self._LicenseType = None
         self._LicenseStatus = None
         self._LicenseCnt = None
         self._UsedLicenseCnt = None
         self._OrderStatus = None
@@ -41399,14 +41402,15 @@
         self._AutoRenewFlag = None
         self._ProjectId = None
         self._TaskId = None
         self._BuyTime = None
         self._SourceType = None
         self._Alias = None
         self._Tags = None
+        self._FreezeNum = None
 
     @property
     def LicenseId(self):
         return self._LicenseId
 
     @LicenseId.setter
     def LicenseId(self, LicenseId):
@@ -41520,14 +41524,22 @@
     def Tags(self):
         return self._Tags
 
     @Tags.setter
     def Tags(self, Tags):
         self._Tags = Tags
 
+    @property
+    def FreezeNum(self):
+        return self._FreezeNum
+
+    @FreezeNum.setter
+    def FreezeNum(self, FreezeNum):
+        self._FreezeNum = FreezeNum
+
 
     def _deserialize(self, params):
         self._LicenseId = params.get("LicenseId")
         self._LicenseType = params.get("LicenseType")
         self._LicenseStatus = params.get("LicenseStatus")
         self._LicenseCnt = params.get("LicenseCnt")
         self._UsedLicenseCnt = params.get("UsedLicenseCnt")
@@ -41542,14 +41554,15 @@
         self._Alias = params.get("Alias")
         if params.get("Tags") is not None:
             self._Tags = []
             for item in params.get("Tags"):
                 obj = Tags()
                 obj._deserialize(item)
                 self._Tags.append(obj)
+        self._FreezeNum = params.get("FreezeNum")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.945/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/README.rst` & `tencentcloud-sdk-python-cwp-3.0.945/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.944/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.945/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

