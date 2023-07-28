# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.944.tar", last modified: Thu Jul 27 02:14:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.945.tar", last modified: Fri Jul 28 00:26:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.944.tar` & `tencentcloud-sdk-python-dnspod-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    61922 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24132 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   351707 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-27 02:14:24.000000 tencentcloud-sdk-python-dnspod-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    61922 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24132 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   351981 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-28 00:26:57.000000 tencentcloud-sdk-python-dnspod-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud/dnspod/v20210323/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1985,26 +1985,29 @@
         :type MX: int
         :param _TTL: TTL，范围1-604800，不同等级域名最小值不同。
         :type TTL: int
         :param _Weight: 权重信息，0到100的整数。仅企业 VIP 域名可用，0 表示关闭，不传该参数，表示不设置权重信息。
         :type Weight: int
         :param _Status: 记录初始状态，取值范围为 ENABLE 和 DISABLE 。默认为 ENABLE ，如果传入 DISABLE，解析不会生效，也不会验证负载均衡的限制。
         :type Status: str
+        :param _Remark: 备注
+        :type Remark: str
         """
         self._Domain = None
         self._RecordType = None
         self._RecordLine = None
         self._Value = None
         self._DomainId = None
         self._SubDomain = None
         self._RecordLineId = None
         self._MX = None
         self._TTL = None
         self._Weight = None
         self._Status = None
+        self._Remark = None
 
     @property
     def Domain(self):
         return self._Domain
 
     @Domain.setter
     def Domain(self, Domain):
@@ -2086,27 +2089,36 @@
     def Status(self):
         return self._Status
 
     @Status.setter
     def Status(self, Status):
         self._Status = Status
 
+    @property
+    def Remark(self):
+        return self._Remark
+
+    @Remark.setter
+    def Remark(self, Remark):
+        self._Remark = Remark
+
 
     def _deserialize(self, params):
         self._Domain = params.get("Domain")
         self._RecordType = params.get("RecordType")
         self._RecordLine = params.get("RecordLine")
         self._Value = params.get("Value")
         self._DomainId = params.get("DomainId")
         self._SubDomain = params.get("SubDomain")
         self._RecordLineId = params.get("RecordLineId")
         self._MX = params.get("MX")
         self._TTL = params.get("TTL")
         self._Weight = params.get("Weight")
         self._Status = params.get("Status")
+        self._Remark = params.get("Remark")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.945/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.944/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.945/README.rst`

 * *Files identical despite different names*

