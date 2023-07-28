# Comparing `tmp/charset_mnbvc-0.0.8.tar.gz` & `tmp/charset_mnbvc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charset_mnbvc-0.0.8.tar", last modified: Tue Jul 18 06:25:52 2023, max compression
+gzip compressed data, was "charset_mnbvc-0.0.9.tar", last modified: Fri Jul 28 07:20:10 2023, max compression
```

## Comparing `charset_mnbvc-0.0.8.tar` & `charset_mnbvc-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.625591 charset_mnbvc-0.0.8/
--rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.8/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)    12352 2023-07-18 06:25:52.625405 charset_mnbvc-0.0.8/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)    11712 2023-07-07 03:47:36.000000 charset_mnbvc-0.0.8/README.md
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.624462 charset_mnbvc-0.0.8/charset_mnbvc/
--rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.8/charset_mnbvc/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)     6375 2023-07-18 06:24:28.000000 charset_mnbvc-0.0.8/charset_mnbvc/api.py
--rw-r--r--   0 alan       (501) staff       (20)      453 2023-07-07 02:45:15.000000 charset_mnbvc-0.0.8/charset_mnbvc/common_utils.py
--rw-r--r--   0 alan       (501) staff       (20)     3211 2023-07-07 03:34:44.000000 charset_mnbvc-0.0.8/charset_mnbvc/constant.py
--rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.8/charset_mnbvc/verify.py
--rw-r--r--   0 alan       (501) staff       (20)       70 2023-06-20 03:19:29.000000 charset_mnbvc-0.0.8/charset_mnbvc/version.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-18 06:25:52.625230 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)    12352 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      326 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       14 2023-07-18 06:25:52.000000 charset_mnbvc-0.0.8/charset_mnbvc.egg-info/top_level.txt
--rw-r--r--   0 alan       (501) staff       (20)       38 2023-07-18 06:25:52.625631 charset_mnbvc-0.0.8/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.8/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-28 07:20:10.153866 charset_mnbvc-0.0.9/
+-rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.9/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)    13052 2023-07-28 07:20:10.153670 charset_mnbvc-0.0.9/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)    12412 2023-07-28 07:19:08.000000 charset_mnbvc-0.0.9/README.md
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-28 07:20:10.152982 charset_mnbvc-0.0.9/charset_mnbvc/
+-rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.9/charset_mnbvc/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)     6444 2023-07-28 07:16:38.000000 charset_mnbvc-0.0.9/charset_mnbvc/api.py
+-rw-r--r--   0 alan       (501) staff       (20)      934 2023-07-28 07:18:09.000000 charset_mnbvc-0.0.9/charset_mnbvc/common_utils.py
+-rw-r--r--   0 alan       (501) staff       (20)     3224 2023-07-26 07:35:40.000000 charset_mnbvc-0.0.9/charset_mnbvc/constant.py
+-rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.9/charset_mnbvc/verify.py
+-rw-r--r--   0 alan       (501) staff       (20)       70 2023-07-28 07:17:05.000000 charset_mnbvc-0.0.9/charset_mnbvc/version.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-07-28 07:20:10.153419 charset_mnbvc-0.0.9/charset_mnbvc.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)    13052 2023-07-28 07:20:10.000000 charset_mnbvc-0.0.9/charset_mnbvc.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      326 2023-07-28 07:20:10.000000 charset_mnbvc-0.0.9/charset_mnbvc.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2023-07-28 07:20:10.000000 charset_mnbvc-0.0.9/charset_mnbvc.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       14 2023-07-28 07:20:10.000000 charset_mnbvc-0.0.9/charset_mnbvc.egg-info/top_level.txt
+-rw-r--r--   0 alan       (501) staff       (20)       38 2023-07-28 07:20:10.153905 charset_mnbvc-0.0.9/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.9/setup.py
```

### Comparing `charset_mnbvc-0.0.8/LICENSE` & `charset_mnbvc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.8/PKG-INFO` & `charset_mnbvc-0.0.9/charset_mnbvc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: charset_mnbvc
-Version: 0.0.8
+Name: charset-mnbvc
+Version: 0.0.9
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
@@ -77,14 +77,31 @@
 ###### 尝试修复乱码数据
 ```
 from charset_mnbvc import api
 data_1 = "变巨"
 
 result_1 = api.fix_data(s=data_1)
 print(f"修复测试1: {result_1}")
+
+from      | to        | origin | guess
+-----------------------------------
+utf-8     | gbk       | 变巨 | 鍙樺法
+utf-8     | gb18030   | 变巨 | 鍙樺法
+utf-8     | BIG5      | 变巨 | ���撌�
+utf-8     | shift_jis | 变巨 | 蜿伜ｷｨ
+utf-8     | euc_kr    | 变巨 | ���藥�
+utf-8     | ascii     | 变巨 | ������
+utf-8     | utf_16    | 变巨 | 迥ꢷ
+utf-8     | cp1252    | 变巨 | å�˜å·¨
+gbk       | utf-8     | 变巨 | ���
+gbk       | gb18030   | 变巨 | 变巨
+gbk       | BIG5      | 变巨 | 曹操
+gbk       | shift_jis | 变巨 | ｱ萓ﾞ
+gbk       | euc_kr    | 变巨 | 긴앵
+gbk       | ascii     | 变巨 | ����
 ```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
```

### Comparing `charset_mnbvc-0.0.8/README.md` & `charset_mnbvc-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: charset_mnbvc
+Version: 0.0.9
+Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
+Home-page: https://github.com/alanshi/charset_mnbvc
+Author: Alan Shi
+Author-email: alan.shi86@gmail.com
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
+Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### 项目描述
 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 
 
 #### 模块安装
 ```
 pip install charset-mnbvc
@@ -60,14 +77,31 @@
 ###### 尝试修复乱码数据
 ```
 from charset_mnbvc import api
 data_1 = "变巨"
 
 result_1 = api.fix_data(s=data_1)
 print(f"修复测试1: {result_1}")
+
+from      | to        | origin | guess
+-----------------------------------
+utf-8     | gbk       | 变巨 | 鍙樺法
+utf-8     | gb18030   | 变巨 | 鍙樺法
+utf-8     | BIG5      | 变巨 | ���撌�
+utf-8     | shift_jis | 变巨 | 蜿伜ｷｨ
+utf-8     | euc_kr    | 变巨 | ���藥�
+utf-8     | ascii     | 变巨 | ������
+utf-8     | utf_16    | 变巨 | 迥ꢷ
+utf-8     | cp1252    | 变巨 | å�˜å·¨
+gbk       | utf-8     | 变巨 | ���
+gbk       | gb18030   | 变巨 | 变巨
+gbk       | BIG5      | 变巨 | 曹操
+gbk       | shift_jis | 变巨 | ｱ萓ﾞ
+gbk       | euc_kr    | 变巨 | 긴앵
+gbk       | ascii     | 变巨 | ����
 ```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
@@ -213,7 +247,9 @@
                 sb.append(line).append(System.lineSeparator());
             }
         }
         return sb.toString();
     }
 }
 ```
+
+
```

### Comparing `charset_mnbvc-0.0.8/charset_mnbvc/api.py` & `charset_mnbvc-0.0.9/charset_mnbvc/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     REGEX_FEATURE,
     CHUNK_SIZE,
     ENCODINGS,
     EXT_ENCODING,
     CCHARDECT_ENCODING_MAP
 )
 
+from .common_utils import (
+    print_table
+)
 
 # compile makes it more efficient
 re_char_check = compile(REGEX_FEATURE_ALL)
 
 
 def has_control_characters(text):
     """
@@ -42,15 +45,15 @@
         guess_text = s.encode(encoding=item, errors='replace')
         for target in EXT_ENCODING:
             if item == target:
                 continue
             fixed_text = guess_text.decode(encoding=target, errors='replace')
             dic = {"origin": s, "guess": fixed_text, "from": item, "to": target}
             result.append(dic)
-
+    print_table(result)
     return result
 
 
 def from_data(data, mode) -> str:
     """
     :param data: data
     :param mode: 1: use mnbvc, 2: use cchardet
```

### Comparing `charset_mnbvc-0.0.8/charset_mnbvc/constant.py` & `charset_mnbvc-0.0.9/charset_mnbvc/constant.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                     r'\u672c\u524d\u5f00\u4f46\u56e0\u53ea\u4ece\u60f3\u5b9e]'
 
 ENCODINGS = [
     'utf_8',
     'utf_16',
     'gb18030',
     'big5',
+    'gb2312'
 ]
 
 EXT_ENCODING = [
     'utf-8',
     'gbk', # 简体中文 (GB2312)
     'gb18030', # 简体中文 (GB2312)
     'BIG5', # 繁体中文 (BIG5)
```

### Comparing `charset_mnbvc-0.0.8/charset_mnbvc/verify.py` & `charset_mnbvc-0.0.9/charset_mnbvc/verify.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.8/charset_mnbvc.egg-info/PKG-INFO` & `charset_mnbvc-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: charset-mnbvc
-Version: 0.0.8
-Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
-Home-page: https://github.com/alanshi/charset_mnbvc
-Author: Alan Shi
-Author-email: alan.shi86@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
-Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### 项目描述
 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 
 
 #### 模块安装
 ```
 pip install charset-mnbvc
@@ -77,14 +60,31 @@
 ###### 尝试修复乱码数据
 ```
 from charset_mnbvc import api
 data_1 = "变巨"
 
 result_1 = api.fix_data(s=data_1)
 print(f"修复测试1: {result_1}")
+
+from      | to        | origin | guess
+-----------------------------------
+utf-8     | gbk       | 变巨 | 鍙樺法
+utf-8     | gb18030   | 变巨 | 鍙樺法
+utf-8     | BIG5      | 变巨 | ���撌�
+utf-8     | shift_jis | 变巨 | 蜿伜ｷｨ
+utf-8     | euc_kr    | 变巨 | ���藥�
+utf-8     | ascii     | 变巨 | ������
+utf-8     | utf_16    | 变巨 | 迥ꢷ
+utf-8     | cp1252    | 变巨 | å�˜å·¨
+gbk       | utf-8     | 变巨 | ���
+gbk       | gb18030   | 变巨 | 变巨
+gbk       | BIG5      | 变巨 | 曹操
+gbk       | shift_jis | 变巨 | ｱ萓ﾞ
+gbk       | euc_kr    | 变巨 | 긴앵
+gbk       | ascii     | 变巨 | ����
 ```
 
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
@@ -230,9 +230,7 @@
                 sb.append(line).append(System.lineSeparator());
             }
         }
         return sb.toString();
     }
 }
 ```
-
-
```

### Comparing `charset_mnbvc-0.0.8/setup.py` & `charset_mnbvc-0.0.9/setup.py`

 * *Files identical despite different names*

