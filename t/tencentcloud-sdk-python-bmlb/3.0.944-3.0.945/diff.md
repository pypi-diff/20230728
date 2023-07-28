# Comparing `tmp/tencentcloud-sdk-python-bmlb-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-bmlb-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.944.tar", last modified: Thu Jul 27 02:09:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bmlb-3.0.945.tar", last modified: Fri Jul 28 00:22:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bmlb-3.0.944.tar` & `tencentcloud-sdk-python-bmlb-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/
--rw-r--r--   0 root         (0) root         (0)    47282 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/bmlb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   327109 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-27 02:09:46.000000 tencentcloud-sdk-python-bmlb-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    47282 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/bmlb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   327109 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-28 00:22:16.000000 tencentcloud-sdk-python-bmlb-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/setup.py` & `tencentcloud-sdk-python-bmlb-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud_sdk_python_bmlb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/bmlb_client.py` & `tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/bmlb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/errorcodes.py` & `tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/tencentcloud/bmlb/v20180625/models.py` & `tencentcloud-sdk-python-bmlb-3.0.945/tencentcloud/bmlb/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-bmlb-3.0.945/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bmlb
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Bmlb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bmlb-3.0.944/README.rst` & `tencentcloud-sdk-python-bmlb-3.0.945/README.rst`

 * *Files identical despite different names*

