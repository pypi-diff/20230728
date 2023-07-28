# Comparing `tmp/tencentcloud-sdk-python-bma-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-bma-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.944.tar", last modified: Thu Jul 27 02:09:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.945.tar", last modified: Fri Jul 28 00:22:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bma-3.0.944.tar` & `tencentcloud-sdk-python-bma-3.0.945.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10571 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/bma_client.py
--rw-r--r--   0 root         (0) root         (0)    65352 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25903 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/bma_client.py
--rw-r--r--   0 root         (0) root         (0)   146139 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:09:38.000000 tencentcloud-sdk-python-bma-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10571 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)    65814 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25903 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)   146139 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:22:07.000000 tencentcloud-sdk-python-bma-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-bma-3.0.944/setup.py` & `tencentcloud-sdk-python-bma-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud_sdk_python_bma.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud_sdk_python_bma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20221115/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1602,18 +1602,18 @@
         :type FakeURL: str
         :param _FakeDomain: 仿冒域名
 注意：此字段可能返回 null，表示取不到有效值。
         :type FakeDomain: str
         :param _Heat: 热度
 注意：此字段可能返回 null，表示取不到有效值。
         :type Heat: int
-        :param _BlockStatus: 协助处置状态：0-未处置 1-处置中 2-处置成功 3-处置失败
+        :param _BlockStatus: 拦截处置状态：0-未处置 1-处置中 2-处置成功 3-处置失败
 注意：此字段可能返回 null，表示取不到有效值。
         :type BlockStatus: int
-        :param _BlockNote: 协助处置状态说明
+        :param _BlockNote: 拦截处置状态说明
 注意：此字段可能返回 null，表示取不到有效值。
         :type BlockNote: str
         :param _OfflineStatus: 关停状态：0-未关停 1-关停中 2-关停成功 3-关停失败 4-重复上架
 注意：此字段可能返回 null，表示取不到有效值。
         :type OfflineStatus: int
         :param _OfflineNote: 关停状态说明
 注意：此字段可能返回 null，表示取不到有效值。
@@ -1650,14 +1650,17 @@
         :type CertificationStatus: int
         :param _Snapshot: 网址截图
 注意：此字段可能返回 null，表示取不到有效值。
         :type Snapshot: str
         :param _AccountStatus: 账户资源状态：0-不可用 1-可用
 注意：此字段可能返回 null，表示取不到有效值。
         :type AccountStatus: int
+        :param _AuditStatus: 审核状态：0-未审核 1-审核中 2-审核成功 3-审核失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AuditStatus: int
         """
         self._FakeURLId = None
         self._BrandName = None
         self._Origin = None
         self._FakeURL = None
         self._FakeDomain = None
         self._Heat = None
@@ -1673,14 +1676,15 @@
         self._WebICP = None
         self._WebCreateTime = None
         self._WebExpireTime = None
         self._InsertTime = None
         self._CertificationStatus = None
         self._Snapshot = None
         self._AccountStatus = None
+        self._AuditStatus = None
 
     @property
     def FakeURLId(self):
         return self._FakeURLId
 
     @FakeURLId.setter
     def FakeURLId(self, FakeURLId):
@@ -1850,14 +1854,22 @@
     def AccountStatus(self):
         return self._AccountStatus
 
     @AccountStatus.setter
     def AccountStatus(self, AccountStatus):
         self._AccountStatus = AccountStatus
 
+    @property
+    def AuditStatus(self):
+        return self._AuditStatus
+
+    @AuditStatus.setter
+    def AuditStatus(self, AuditStatus):
+        self._AuditStatus = AuditStatus
+
 
     def _deserialize(self, params):
         self._FakeURLId = params.get("FakeURLId")
         self._BrandName = params.get("BrandName")
         self._Origin = params.get("Origin")
         self._FakeURL = params.get("FakeURL")
         self._FakeDomain = params.get("FakeDomain")
@@ -1874,14 +1886,15 @@
         self._WebICP = params.get("WebICP")
         self._WebCreateTime = params.get("WebCreateTime")
         self._WebExpireTime = params.get("WebExpireTime")
         self._InsertTime = params.get("InsertTime")
         self._CertificationStatus = params.get("CertificationStatus")
         self._Snapshot = params.get("Snapshot")
         self._AccountStatus = params.get("AccountStatus")
+        self._AuditStatus = params.get("AuditStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-bma-3.0.945/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.944/README.rst` & `tencentcloud-sdk-python-bma-3.0.945/README.rst`

 * *Files identical despite different names*

