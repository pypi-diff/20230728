# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.943.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.943.tar", last modified: Wed Jul 26 00:40:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.944.tar", last modified: Thu Jul 27 02:18:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.943.tar` & `tencentcloud-sdk-python-lighthouse-3.0.944.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104972 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)    27298 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   404234 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 00:40:07.000000 tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104972 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)    27298 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   404234 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-27 02:18:32.000000 tencentcloud-sdk-python-lighthouse-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:18:33.000000 tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.944/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.943'
+__version__ = '3.0.944'
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.944/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.944/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.943/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.944/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.943
+Version: 3.0.944
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

