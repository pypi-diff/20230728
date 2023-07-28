# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.944.tar", last modified: Thu Jul 27 02:15:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.945.tar", last modified: Fri Jul 28 00:27:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.944.tar` & `tencentcloud-sdk-python-eis-3.0.945.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39966 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:15:23.000000 tencentcloud-sdk-python-eis-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:15:22.000000 tencentcloud-sdk-python-eis-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39966 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:27:52.000000 tencentcloud-sdk-python-eis-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.944/setup.py` & `tencentcloud-sdk-python-eis-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20210601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eis-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.944/README.rst` & `tencentcloud-sdk-python-eis-3.0.945/README.rst`

 * *Files identical despite different names*

