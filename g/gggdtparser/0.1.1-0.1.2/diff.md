# Comparing `tmp/gggdtparser-0.1.1.tar.gz` & `tmp/gggdtparser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.1.1.tar", last modified: Tue Jul  4 07:37:37 2023, max compression
+gzip compressed data, was "gggdtparser-0.1.2.tar", last modified: Fri Jul 28 02:32:51 2023, max compression
```

## Comparing `gggdtparser-0.1.1.tar` & `gggdtparser-0.1.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.704491 gggdtparser-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-07-04 07:37:37.704491 gggdtparser-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.665595 gggdtparser-0.1.1/gggdtparser/
--rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.1.1/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0     3260 2023-06-19 03:06:17.000000 gggdtparser-0.1.1/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    17850 2023-06-19 03:07:20.000000 gggdtparser-0.1.1/gggdtparser/dtparser.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.691526 gggdtparser-0.1.1/gggdtparser/langs/
--rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.1.1/gggdtparser/langs/__init__.py
--rw-rw-rw-   0        0        0      235 2023-06-19 02:32:34.000000 gggdtparser-0.1.1/gggdtparser/langs/_id.py
--rw-rw-rw-   0        0        0      246 2023-06-19 02:32:40.000000 gggdtparser-0.1.1/gggdtparser/langs/az.py
--rw-rw-rw-   0        0        0      678 2023-06-19 02:44:22.000000 gggdtparser-0.1.1/gggdtparser/langs/de.py
--rw-rw-rw-   0        0        0     4783 2023-07-04 07:25:34.000000 gggdtparser-0.1.1/gggdtparser/langs/default.py
--rw-rw-rw-   0        0        0     3438 2023-06-19 01:52:13.000000 gggdtparser-0.1.1/gggdtparser/langs/en.py
--rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/es.py
--rw-rw-rw-   0        0        0      950 2023-07-04 07:27:57.000000 gggdtparser-0.1.1/gggdtparser/langs/fra.py
--rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.1.1/gggdtparser/langs/hi.py
--rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.1.1/gggdtparser/langs/ky.py
--rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.1.1/gggdtparser/langs/mr.py
--rw-rw-rw-   0        0        0      813 2023-06-19 02:00:07.000000 gggdtparser-0.1.1/gggdtparser/langs/ru.py
--rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.1.1/gggdtparser/langs/rw.py
--rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.1.1/gggdtparser/langs/si.py
--rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/so.py
--rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.1.1/gggdtparser/langs/sw.py
--rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/swe.py
--rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.1.1/gggdtparser/langs/tg.py
--rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.1.1/gggdtparser/langs/tr.py
--rw-rw-rw-   0        0        0      815 2023-06-19 02:54:06.000000 gggdtparser-0.1.1/gggdtparser/langs/uk.py
--rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.1.1/gggdtparser/langs/ur.py
--rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/vie.py
--rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.1.1/gggdtparser/langs/zh.py
--rw-rw-rw-   0        0        0      631 2023-07-04 07:26:09.000000 gggdtparser-0.1.1/gggdtparser/langs/zht.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.703493 gggdtparser-0.1.1/gggdtparser/test/
--rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.1.1/gggdtparser/test/__init__.py
--rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.1.1/gggdtparser/test/_id.py
--rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.1.1/gggdtparser/test/az.py
--rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.1.1/gggdtparser/test/hi.py
--rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.1.1/gggdtparser/test/ky.py
--rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.1.1/gggdtparser/test/mr.py
--rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.1.1/gggdtparser/test/ru.py
--rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.1.1/gggdtparser/test/rw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.1.1/gggdtparser/test/si.py
--rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.1.1/gggdtparser/test/sw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.1.1/gggdtparser/test/tg.py
--rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.1.1/gggdtparser/test/tr.py
--rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.1.1/gggdtparser/test/uk.py
--rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.1.1/gggdtparser/test/ur.py
--rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.1.1/gggdtparser/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 07:37:37.669584 gggdtparser-0.1.1/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 07:37:37.000000 gggdtparser-0.1.1/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-07-04 07:37:37.705488 gggdtparser-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:32:51.214004 gggdtparser-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-07-28 02:32:51.214004 gggdtparser-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 02:32:51.173114 gggdtparser-0.1.2/gggdtparser/
+-rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.1.2/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0     3432 2023-07-28 02:26:49.000000 gggdtparser-0.1.2/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    18150 2023-07-28 02:30:52.000000 gggdtparser-0.1.2/gggdtparser/dtparser.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:32:51.200041 gggdtparser-0.1.2/gggdtparser/langs/
+-rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.1.2/gggdtparser/langs/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-19 02:32:34.000000 gggdtparser-0.1.2/gggdtparser/langs/_id.py
+-rw-rw-rw-   0        0        0      246 2023-06-19 02:32:40.000000 gggdtparser-0.1.2/gggdtparser/langs/az.py
+-rw-rw-rw-   0        0        0      678 2023-06-19 02:44:22.000000 gggdtparser-0.1.2/gggdtparser/langs/de.py
+-rw-rw-rw-   0        0        0     4783 2023-07-04 07:25:34.000000 gggdtparser-0.1.2/gggdtparser/langs/default.py
+-rw-rw-rw-   0        0        0     3438 2023-06-19 01:52:13.000000 gggdtparser-0.1.2/gggdtparser/langs/en.py
+-rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.1.2/gggdtparser/langs/es.py
+-rw-rw-rw-   0        0        0      950 2023-07-04 07:27:57.000000 gggdtparser-0.1.2/gggdtparser/langs/fra.py
+-rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.1.2/gggdtparser/langs/hi.py
+-rw-rw-rw-   0        0        0      259 2023-07-26 07:38:07.000000 gggdtparser-0.1.2/gggdtparser/langs/ja.py
+-rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.1.2/gggdtparser/langs/ky.py
+-rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.1.2/gggdtparser/langs/mr.py
+-rw-rw-rw-   0        0        0      822 2023-07-07 01:00:21.000000 gggdtparser-0.1.2/gggdtparser/langs/ru.py
+-rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.1.2/gggdtparser/langs/rw.py
+-rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.1.2/gggdtparser/langs/si.py
+-rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.1.2/gggdtparser/langs/so.py
+-rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.1.2/gggdtparser/langs/sw.py
+-rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.1.2/gggdtparser/langs/swe.py
+-rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.1.2/gggdtparser/langs/tg.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.1.2/gggdtparser/langs/tr.py
+-rw-rw-rw-   0        0        0      815 2023-06-19 02:54:06.000000 gggdtparser-0.1.2/gggdtparser/langs/uk.py
+-rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.1.2/gggdtparser/langs/ur.py
+-rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.1.2/gggdtparser/langs/vie.py
+-rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.1.2/gggdtparser/langs/zh.py
+-rw-rw-rw-   0        0        0      631 2023-07-04 07:26:09.000000 gggdtparser-0.1.2/gggdtparser/langs/zht.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:32:51.213007 gggdtparser-0.1.2/gggdtparser/test/
+-rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.1.2/gggdtparser/test/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.1.2/gggdtparser/test/_id.py
+-rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.1.2/gggdtparser/test/az.py
+-rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.1.2/gggdtparser/test/hi.py
+-rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.1.2/gggdtparser/test/ky.py
+-rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.1.2/gggdtparser/test/mr.py
+-rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.1.2/gggdtparser/test/ru.py
+-rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.1.2/gggdtparser/test/rw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.1.2/gggdtparser/test/si.py
+-rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.1.2/gggdtparser/test/sw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.1.2/gggdtparser/test/tg.py
+-rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.1.2/gggdtparser/test/tr.py
+-rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.1.2/gggdtparser/test/uk.py
+-rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.1.2/gggdtparser/test/ur.py
+-rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.1.2/gggdtparser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 02:32:51.177103 gggdtparser-0.1.2/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-07-28 02:32:51.000000 gggdtparser-0.1.2/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-07-28 02:32:51.000000 gggdtparser-0.1.2/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 02:32:51.000000 gggdtparser-0.1.2/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-28 02:32:51.000000 gggdtparser-0.1.2/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-28 02:32:51.215002 gggdtparser-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.1.2/setup.py
```

### Comparing `gggdtparser-0.1.1/LICENSE` & `gggdtparser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/PKG-INFO` & `gggdtparser-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.1.1/README.md` & `gggdtparser-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/dtconfigs.py` & `gggdtparser-0.1.2/gggdtparser/dtconfigs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import importlib
 import re
 
 from .utils import get_sort_dict
 
 BASE_DIR = os.path.dirname(os.path.abspath(__file__))
 
+STRING_DATETIME_CLEAR_REGEX = [
+    re.compile(r'\n+'),
+    re.compile(r'(\r\n)+'),
+    re.compile(r' {2,}')
+]
 LANG_MAPPING = {
     # 英语
     "en": "en",
     # 中文
     "zh": "zh",
     "zh-CN": "zh",
     "zh-CHS": "zh",
@@ -63,27 +68,30 @@
     "rw": "rw",
     # 僧伽罗语
     "si": "si",
     # 塔吉克语
     "tg": "tg",
     # 印地语
     "hi": "hi",
+    # 日语
+    "ja": 'ja'
 }
 
 TRANSLATE_LANGS = [
     # 阿拉伯语
     'ara',
     'ar',
     # 泰语
     'th'
 ]
 
 _LANG_LIST_SORT = ['default', 'en', 'zh', 'zht', 'de', 'fra', 'swe',
                    'vie', 'ru', 'es', 'so', 'mr', 'az', "uk", 'sw',
-                   'tr', 'ky', 'ur', '_id', 'rw', 'si', 'tg', 'hi'
+                   'tr', 'ky', 'ur', '_id', 'rw', 'si', 'tg', 'hi',
+                   'ja'
                    ]
 
 
 def compile_regex(regex, flags=0):
     return re.compile(regex, flags)
```

### Comparing `gggdtparser-0.1.1/gggdtparser/dtparser.py` & `gggdtparser-0.1.2/gggdtparser/dtparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         :param langs: 语言
         :param result_accurately: 是否遵循严格判断
         :param extract_accurately: 是否只进行精确抽取
         :param max_datetime: 最大时间，超过解析失败
         :param min_datetime: 最小时间，超过解析失败
         :return:
         """
+        string_datetime = cls.clear_string_datetime(string_datetime)
         if not langs:
             langs = []
         _langs = []
         for lang in langs:
             try:
                 _langs.append(dtconfigs.LANG_MAPPING[lang.lower()])
             except KeyError:
@@ -83,14 +84,20 @@
         result = cls.match_and_parse(
             string_datetime, regex_list,
             result_accurately, max_datetime, min_datetime)
         if result:
             return result
 
     @classmethod
+    def clear_string_datetime(cls, string_datetime):
+        for regex in dtconfigs.STRING_DATETIME_CLEAR_REGEX:
+            string_datetime = regex.sub(' ', string_datetime)
+        return string_datetime
+
+    @classmethod
     def get_default_regex_list(cls, langs, extract_accurately):
         regex_list = []
         if langs:
             if extract_accurately:
                 for lang in langs:
                     regex_list.extend(cls._get_default_regex_list(lang, True))
             else:
```

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/de.py` & `gggdtparser-0.1.2/gggdtparser/langs/de.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/default.py` & `gggdtparser-0.1.2/gggdtparser/langs/default.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/en.py` & `gggdtparser-0.1.2/gggdtparser/langs/en.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/es.py` & `gggdtparser-0.1.2/gggdtparser/langs/es.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/fra.py` & `gggdtparser-0.1.2/gggdtparser/langs/fra.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/ru.py` & `gggdtparser-0.1.2/gggdtparser/langs/ru.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 SUB_TRANSLATE = [
     (r"январь", "1月"),
     (r"февраль", "2月"),
     (r"март", "3月"),
     (r"апрель|апреля|апрел", "4月"),
     (r"май", "5月"),
     (r"июнь|июня", "6月"),
-    (r"июль", "7月"),
+    (r"июль|июля", "7月"),
     (r"август", "8月"),
     (r"сентябрь", "9月"),
     (r"октябрь", "10月"),
     (r"ноябрь", "11月"),
     (r"декабрь", "12月"),
     (r"сегодня  в|сегодня", "今天"),
     (r"вчера  в|вчера", "昨天"),
```

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/swe.py` & `gggdtparser-0.1.2/gggdtparser/langs/swe.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/uk.py` & `gggdtparser-0.1.2/gggdtparser/langs/uk.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/zh.py` & `gggdtparser-0.1.2/gggdtparser/langs/zh.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/langs/zht.py` & `gggdtparser-0.1.2/gggdtparser/langs/zht.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/test/__init__.py` & `gggdtparser-0.1.2/gggdtparser/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/test/az.py` & `gggdtparser-0.1.2/gggdtparser/test/az.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser/utils.py` & `gggdtparser-0.1.2/gggdtparser/utils.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.1.1/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.1.2/gggdtparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.1.1/gggdtparser.egg-info/SOURCES.txt` & `gggdtparser-0.1.2/gggdtparser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 gggdtparser/langs/az.py
 gggdtparser/langs/de.py
 gggdtparser/langs/default.py
 gggdtparser/langs/en.py
 gggdtparser/langs/es.py
 gggdtparser/langs/fra.py
 gggdtparser/langs/hi.py
+gggdtparser/langs/ja.py
 gggdtparser/langs/ky.py
 gggdtparser/langs/mr.py
 gggdtparser/langs/ru.py
 gggdtparser/langs/rw.py
 gggdtparser/langs/si.py
 gggdtparser/langs/so.py
 gggdtparser/langs/sw.py
```

### Comparing `gggdtparser-0.1.1/setup.cfg` & `gggdtparser-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 310d  version = 0.1.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

