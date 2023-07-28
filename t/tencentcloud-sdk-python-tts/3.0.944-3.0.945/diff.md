# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.944.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.944.tar", last modified: Thu Jul 27 02:27:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.945.tar", last modified: Fri Jul 28 00:38:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.944.tar` & `tencentcloud-sdk-python-tts-3.0.945.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5572 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23692 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5922 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-27 02:27:06.000000 tencentcloud-sdk-python-tts-3.0.944/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23747 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:38:56.000000 tencentcloud-sdk-python-tts-3.0.945/README.rst
```

### Comparing `tencentcloud-sdk-python-tts-3.0.944/setup.py` & `tencentcloud-sdk-python-tts-3.0.945/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         :type PrimaryLanguage: int
         :param _SampleRate: 音频采样率：<li>16000：16k（默认）</li><li>8000：8k</li>
         :type SampleRate: int
         :param _Codec: 返回音频格式，可取值：mp3（默认），wav，pcm
         :type Codec: str
         :param _CallbackUrl: 回调 URL，用户自行搭建的用于接收识别结果的服务URL。如果用户使用轮询方式获取识别结果，则无需提交该参数。[回调说明](https://cloud.tencent.com/document/product/1073/55746)
         :type CallbackUrl: str
-        :param _VoiceoverDialogueSplit: 旁白与对白文本解析，分别合成相应风格（仅适用于旁对白音色），默认 false
+        :param _VoiceoverDialogueSplit: 旁白与对白文本解析，分别合成相应风格（仅适用于旁对白音色10510000、100510000），默认 false
         :type VoiceoverDialogueSplit: bool
         """
         self._Text = None
         self._ModelType = None
         self._Volume = None
         self._Speed = None
         self._ProjectId = None
@@ -521,15 +521,15 @@
         :type SampleRate: int
         :param _Codec: 返回音频格式，可取值：wav（默认），mp3，pcm
         :type Codec: str
         :param _EnableSubtitle: 是否开启时间戳功能，默认为false。
         :type EnableSubtitle: bool
         :param _SegmentRate: 断句敏感阈值，默认值为：0，取值范围：[0,1,2]。该值越大越不容易断句，模型会更倾向于仅按照标点符号断句。此参数建议不要随意调整，可能会影响合成效果。
         :type SegmentRate: int
-        :param _EmotionCategory: 控制合成音频的情感，仅支持多情感音色使用。取值: neutral(中性)、sad(悲伤)、happy(高兴)、angry(生气)、fear(恐惧)、news(新闻)、story(故事)、radio(广播)、poetry(诗歌)、call(客服)、撒娇(sajiao)、厌恶(disgusted)、震惊(amaze)、平静(peaceful)、兴奋(exciting)
+        :param _EmotionCategory: 控制合成音频的情感，仅支持多情感音色使用。取值: neutral(中性)、sad(悲伤)、happy(高兴)、angry(生气)、fear(恐惧)、news(新闻)、story(故事)、radio(广播)、poetry(诗歌)、call(客服)、撒娇(sajiao)、厌恶(disgusted)、震惊(amaze)、平静(peaceful)、兴奋(exciting)、傲娇(aojiao)、解说(jieshuo)
         :type EmotionCategory: str
         :param _EmotionIntensity: 控制合成音频情感程度，取值范围为[50,200],默认为100；只有EmotionCategory不为空时生效；
         :type EmotionIntensity: int
         """
         self._Text = None
         self._SessionId = None
         self._Volume = None
```

### Comparing `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.945/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.944/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.945/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.944/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.945/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.944/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.945/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.944
+Version: 3.0.945
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.944/README.rst` & `tencentcloud-sdk-python-tts-3.0.945/README.rst`

 * *Files identical despite different names*

