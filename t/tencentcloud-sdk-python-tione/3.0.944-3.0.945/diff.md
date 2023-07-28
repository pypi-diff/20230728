# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.944.tar", last modified: Thu Jul 27 02:25:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.945.tar", last modified: Fri Jul 28 00:37:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.944.tar` & `tencentcloud-sdk-python-tione-3.0.945.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51244 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12673 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   531149 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22102 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144266 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-27 02:25:44.000000 tencentcloud-sdk-python-tione-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51244 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12673 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   531149 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22102 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144266 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-tione-3.0.944/setup.py` & `tencentcloud-sdk-python-tione-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.944/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.944/README.rst` & `tencentcloud-sdk-python-tione-3.0.945/README.rst`

 * *Files identical despite different names*

