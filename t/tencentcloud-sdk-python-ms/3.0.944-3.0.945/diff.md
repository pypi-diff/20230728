# Comparing `tmp/tencentcloud-sdk-python-ms-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-ms-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.944.tar", last modified: Thu Jul 27 02:19:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ms-3.0.945.tar", last modified: Fri Jul 28 00:32:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ms-3.0.944.tar` & `tencentcloud-sdk-python-ms-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)    21305 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   169826 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-27 02:19:58.000000 tencentcloud-sdk-python-ms-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    21305 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   169826 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-28 00:32:28.000000 tencentcloud-sdk-python-ms-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-ms-3.0.944/tencentcloud_sdk_python_ms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.945/tencentcloud_sdk_python_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.944/setup.py` & `tencentcloud-sdk-python-ms-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/ms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.944/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-ms-3.0.945/tencentcloud/ms/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ms-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ms-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ms-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-ms-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ms
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Ms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ms-3.0.944/README.rst` & `tencentcloud-sdk-python-ms-3.0.945/README.rst`

 * *Files identical despite different names*
