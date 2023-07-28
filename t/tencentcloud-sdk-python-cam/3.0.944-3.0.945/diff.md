# Comparing `tmp/tencentcloud-sdk-python-cam-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-cam-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.944.tar", last modified: Thu Jul 27 02:10:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cam-3.0.945.tar", last modified: Fri Jul 28 00:22:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cam-3.0.944.tar` & `tencentcloud-sdk-python-cam-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11057 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    78350 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/cam_client.py
--rw-r--r--   0 root         (0) root         (0)   294347 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:10:16.000000 tencentcloud-sdk-python-cam-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    78350 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/cam_client.py
+-rw-r--r--   0 root         (0) root         (0)   295195 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:22:45.000000 tencentcloud-sdk-python-cam-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-cam-3.0.944/setup.py` & `tencentcloud-sdk-python-cam-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.944/tencentcloud_sdk_python_cam.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.945/tencentcloud_sdk_python_cam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cam-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cam-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/errorcodes.py` & `tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/cam_client.py` & `tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/cam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cam-3.0.944/tencentcloud/cam/v20190116/models.py` & `tencentcloud-sdk-python-cam-3.0.945/tencentcloud/cam/v20190116/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5978,15 +5978,15 @@
 class ListAttachedGroupPoliciesResponse(AbstractModel):
     """ListAttachedGroupPolicies返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TotalNum: 策略总数
+        :param _TotalNum: 策略总数。取值范围大于等于0。
         :type TotalNum: int
         :param _List: 策略列表
         :type List: list of AttachPolicyInfo
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TotalNum = None
@@ -10284,31 +10284,31 @@
     """UpdateUserOIDCConfig请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _IdentityUrl: 身份提供商URL。OpenID Connect身份提供商标识。
-对应企业IdP提供的Openid-configuration中"issuer"字段的值。
+对应企业IdP提供的Openid-configuration中"issuer"字段的值，该URL必须以https开头，符合标准URL格式，不允许带有query参数（以?标识）、fragment片段（以#标识）和登录信息（以@标识）。
         :type IdentityUrl: str
-        :param _IdentityKey: 签名公钥，需要base64_encode。验证OpenID Connect身份提供商ID Token签名的公钥。为了您的帐号安全，建议您定期轮换签名公钥。
+        :param _IdentityKey: RSA签名公钥，JWKS格式，需要进行base64_encode。验证OpenID Connect身份提供商ID Token签名的公钥。为了您的账号安全，建议您定期轮换签名公钥。
         :type IdentityKey: str
-        :param _ClientId: 客户端ID，在OpenID Connect身份提供商注册的客户端ID。
+        :param _ClientId: 客户端ID，在OpenID Connect身份提供商注册的客户端ID，允许英文字母、数字、特殊字符.-_:/，不能以特殊字符.-_:/开头，单个客户端ID最大64个字符。
         :type ClientId: str
-        :param _AuthorizationEndpoint: 授权请求Endpoint，OpenID Connect身份提供商授权地址。对应企业IdP提供的Openid-configuration中"authorization_endpoint"字段的值。
+        :param _AuthorizationEndpoint: 授权请求Endpoint，OpenID Connect身份提供商授权地址。对应企业IdP提供的Openid-configuration中"authorization_endpoint"字段的值，该URL必须以https开头，符合标准URL格式，不允许带有query参数（以?标识）、fragment片段（以#标识）和登录信息（以@标识）。
         :type AuthorizationEndpoint: str
-        :param _ResponseType: 授权请求Response type，固定值id_token。
+        :param _ResponseType: 授权请求Response type，有code，id_token，固定值id_token。
         :type ResponseType: str
-        :param _ResponseMode: 授权请求Response mode。授权请求返回模式，form_post和fragment两种可选模式，推荐选择form_post模式。
+        :param _ResponseMode: 授权请求Response mode。授权请求返回模式，有form_post和fragment两种可选模式，推荐选择form_post模式。
         :type ResponseMode: str
-        :param _MappingFiled: 映射字段名称。IdP的id_token中哪一个字段映射到子用户的用户名，通常是sub或者name字段
+        :param _MappingFiled: 映射字段名称。IdP的id_token中哪一个字段映射到子用户的用户名，通常是sub或者name字段,仅支持英文字母、数宇、汉字、符号@、＆_[]-的组合，1-255个中文或英文字符
         :type MappingFiled: str
-        :param _Scope: 授权请求Scope。openid; email;profile。授权请求信息范围。默认必选openid。
+        :param _Scope: 授权请求Scope。有openid; email;profile三种。代表授权请求信息范围openid表示请求访问用户的身份信息，email表示请求访问用户的电子邮件地址，profile表示请求访问用户的基本信息。默认必选openid。
         :type Scope: list of str
-        :param _Description: 描述
+        :param _Description: 描述，长度为1~255个英文或中文字符，默认值为空。
         :type Description: str
         """
         self._IdentityUrl = None
         self._IdentityKey = None
         self._ClientId = None
         self._AuthorizationEndpoint = None
         self._ResponseType = None
```

### Comparing `tencentcloud-sdk-python-cam-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-cam-3.0.945/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cam
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Cam SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cam-3.0.944/README.rst` & `tencentcloud-sdk-python-cam-3.0.945/README.rst`

 * *Files identical despite different names*

