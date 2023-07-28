# Comparing `tmp/tencentcloud-sdk-python-dts-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-dts-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.944.tar", last modified: Thu Jul 27 02:14:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dts-3.0.945.tar", last modified: Fri Jul 28 00:27:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dts-3.0.944.tar` & `tencentcloud-sdk-python-dts-3.0.945.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/
--rw-r--r--   0 root         (0) root         (0)    47354 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/dts_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   327362 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/
--rw-r--r--   0 root         (0) root         (0)    24853 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/dts_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   124284 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:14:53.000000 tencentcloud-sdk-python-dts-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/
+-rw-r--r--   0 root         (0) root         (0)    47354 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   327662 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/
+-rw-r--r--   0 root         (0) root         (0)    24853 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/dts_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   124284 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:27:23.000000 tencentcloud-sdk-python-dts-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:27:22.000000 tencentcloud-sdk-python-dts-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-dts-3.0.944/setup.py` & `tencentcloud-sdk-python-dts-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/dts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20211206/models.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20211206/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6822,15 +6822,15 @@
         :param _IsOverrideRoot: 是否用源库Root账户覆盖目标库，值包括：false-不覆盖，true-覆盖，选择库表或者结构迁移时应该为false，注意只对旧版迁移有效
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsOverrideRoot: bool
         :param _IsDstReadOnly: 是否在迁移时设置目标库只读(仅对mysql有效)，true(设置只读)、false(不设置只读，默认此值)
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsDstReadOnly: bool
         :param _ExtraAttr: 其他附加信息，对于特定库可设置额外参数，Redis可定义如下的参数: 
-["ClientOutputBufferHardLimit":512, 	从机缓冲区的硬性容量限制(MB) 	"ClientOutputBufferSoftLimit":512, 	从机缓冲区的软性容量限制(MB) 	"ClientOutputBufferPersistTime":60, 从机缓冲区的软性限制持续时间(秒) 	"ReplBacklogSize":512, 	环形缓冲区容量限制(MB) 	"ReplTimeout":120，		复制超时时间(秒) ]
+["DstWriteMode":normal, 	目标库写入模式,可取值clearData(清空目标实例数据)、overwrite(以覆盖写的方式执行任务)、normal(跟正常流程一样，不做额外动作) 	"IsDstReadOnly":true, 	是否在迁移时设置目标库只读,true(设置只读)、false(不设置只读) 	"ClientOutputBufferHardLimit":512, 	从机缓冲区的硬性容量限制(MB) 	"ClientOutputBufferSoftLimit":512, 	从机缓冲区的软性容量限制(MB) 	"ClientOutputBufferPersistTime":60, 从机缓冲区的软性限制持续时间(秒) 	"ReplBacklogSize":512, 	环形缓冲区容量限制(MB) 	"ReplTimeout":120，		复制超时时间(秒) ]
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExtraAttr: list of KeyValuePairOption
         """
         self._DatabaseTable = None
         self._MigrateType = None
         self._Consistency = None
         self._IsMigrateAccount = None
```

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/dts_client.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/dts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/errorcodes.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud/dts/v20180330/models.py` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud/dts/v20180330/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dts-3.0.944/tencentcloud_sdk_python_dts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.945/tencentcloud_sdk_python_dts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-dts-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dts
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Dts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dts-3.0.944/README.rst` & `tencentcloud-sdk-python-dts-3.0.945/README.rst`

 * *Files identical despite different names*

