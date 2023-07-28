# Comparing `tmp/usepy_plugin_logger-0.1.4.tar.gz` & `tmp/usepy_plugin_logger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy_plugin_logger-0.1.4.tar", max compression
+gzip compressed data, was "usepy_plugin_logger-0.1.6.tar", max compression
```

## Comparing `usepy_plugin_logger-0.1.4.tar` & `usepy_plugin_logger-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1634 2023-03-16 05:21:59.499727 usepy_plugin_logger-0.1.4/README.md
--rw-r--r--   0        0        0      443 2023-04-18 05:54:08.855988 usepy_plugin_logger-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      266 2023-03-16 05:22:21.156519 usepy_plugin_logger-0.1.4/src/usepy_logger/__init__.py
--rw-r--r--   0        0        0     2042 2023-02-28 14:41:08.787739 usepy_plugin_logger-0.1.4/src/usepy_logger/formatters.py
--rw-r--r--   0        0        0     1176 2023-03-18 11:44:20.698249 usepy_plugin_logger-0.1.4/src/usepy_logger/handlers.py
--rw-r--r--   0        0        0     2791 2023-03-10 14:10:02.480477 usepy_plugin_logger-0.1.4/src/usepy_logger/intercept.py
--rw-r--r--   0        0        0     2087 2023-04-18 05:53:23.372461 usepy_plugin_logger-0.1.4/src/usepy_logger/logger.py
--rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.4/setup.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1567 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/README.md
+-rw-r--r--   0        0        0      568 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      266 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/__init__.py
+-rw-r--r--   0        0        0     2058 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/formatters.py
+-rw-r--r--   0        0        0     1149 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/handlers.py
+-rw-r--r--   0        0        0     2791 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/intercept.py
+-rw-r--r--   0        0        0     2087 2023-07-28 05:49:34.621620 usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/logger.py
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.6/PKG-INFO
```

### Comparing `usepy_plugin_logger-0.1.4/README.md` & `usepy_plugin_logger-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,56 +4,55 @@
     <img src="https://img.shields.io/pypi/v/usepy-plugin-logger.svg" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/usepy-plugin-logger" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/usepy-plugin-logger.svg" alt="Supported Python versions">
 </a>
 
-#### 文档
-
-[useLogger | UsePy](https://usepy.code05.com/api/logger.html) 
-
 #### 安装
 
-> pip install usepy-plugin-logger
+> pip install 'usepy[logger]'
 
 #### 使用
 
 ```python
 from usepy import useLogger
 
-useLogger() # 使用默认配置
+useLogger()  # 使用默认配置
 
 ```
 
 如果你自身项目正在使用`loguru`，这一切似乎感觉毫无变化。因为默认的配置只是修改了一点输出样式。
 
 如果想要感受它带来的“魔法”，需要稍微配置一下。
 
 ```python
 from usepy import useLogger
-useLogger(packages=["scrapy",  "django",  "usepy"]) 
+
+useLogger(packages=["scrapy", "django", "usepy"])
 
 ```
 
 ##### Logstash/Filebeat
 
-日志的更重要能力是将日志记录发送到`Logstash`/`Filebeat`，这样就可以将日志记录存储到`Elasticsearch`中，方便进行日志分析。所以统一日志的最终输出格式是非常重要的。
+日志的更重要能力是将日志记录发送到`Logstash`/`Filebeat`，这样就可以将日志记录存储到`Elasticsearch`
+中，方便进行日志分析。所以统一日志的最终输出格式是非常重要的。
 
 `useLogger`内置一个`logstash_handler`统一化输出格式。
 
 ```python
 from loguru import logger
 from usepy import useLogger, useLoggerHandlers
+
 useLogger(
- handlers=[
-    useLoggerHandlers.logstash_handler(level="DEBUG",  extra={"app_name":  "spider"})
- ],
- packages=["usepy"],  # hook拦截 usepy 的日志
- extra={"project_name":  "usepy"}
+    handlers=[
+        useLoggerHandlers.logstash_handler(level="DEBUG", extra={"app_name": "spider"})
+    ],
+    packages=["usepy"],  # hook拦截 usepy 的日志
+    extra={"project_name": "usepy"}
 )
 logger.warning("test warning")
 logger.info("test info")
 logger.debug("test debug")
 
 ```
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 ### ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ [Package_version]
-[Supported_Python_versions] #### ææ¡£ [useLogger | UsePy](https://
-usepy.code05.com/api/logger.html) #### å®è£ > pip install usepy-plugin-logger
-#### ä½¿ç¨ ```python from usepy import useLogger useLogger() #
-ä½¿ç¨é»è®¤éç½® ```
+[Supported_Python_versions] #### å®è£ > pip install 'usepy[logger]' ####
+ä½¿ç¨ ```python from usepy import useLogger useLogger() # ä½¿ç¨é»è®¤éç½®
+```
 å¦æä½ èªèº«é¡¹ç®æ­£å¨ä½¿ç¨`loguru`ï¼è¿ä¸åä¼¼ä¹æè§æ¯«æ ååãå ä¸ºé»è®¤çéç½®åªæ¯ä¿®æ¹äºä¸ç¹è¾åºæ ·å¼ã
 å¦ææ³è¦æåå®å¸¦æ¥çâé­æ³âï¼éè¦ç¨å¾®éç½®ä¸ä¸ã
 ```python from usepy import useLogger useLogger(packages=["scrapy", "django",
 "usepy"]) ``` ##### Logstash/Filebeat
 æ¥å¿çæ´éè¦è½åæ¯å°æ¥å¿è®°å½åéå°`Logstash`/
-`Filebeat`ï¼è¿æ ·å°±å¯ä»¥å°æ¥å¿è®°å½å­å¨å°`Elasticsearch`ä¸­ï¼æ¹ä¾¿è¿è¡æ¥å¿åæãæä»¥ç»ä¸æ¥å¿çæç»è¾åºæ ¼å¼æ¯éå¸¸éè¦çã
+`Filebeat`ï¼è¿æ ·å°±å¯ä»¥å°æ¥å¿è®°å½å­å¨å°`Elasticsearch`
+ä¸­ï¼æ¹ä¾¿è¿è¡æ¥å¿åæãæä»¥ç»ä¸æ¥å¿çæç»è¾åºæ ¼å¼æ¯éå¸¸éè¦çã
 `useLogger`åç½®ä¸ä¸ª`logstash_handler`ç»ä¸åè¾åºæ ¼å¼ã ```python
 from loguru import logger from usepy import useLogger, useLoggerHandlers
 useLogger( handlers=[ useLoggerHandlers.logstash_handler(level="DEBUG", extra=
 {"app_name": "spider"}) ], packages=["usepy"], # hookæ¦æª usepy çæ¥å¿
 extra={"project_name": "usepy"} ) logger.warning("test warning") logger.info
 ("test info") logger.debug("test debug") ```
```

### Comparing `usepy_plugin_logger-0.1.4/src/usepy_logger/formatters.py` & `usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 )
 
 
 class JsonFormatter(Formatter):
     """格式化日志到Json，并删除某些字段"""
 
     def __init__(
-        self,
-        extra_ignore_keys: Optional[Union[List[str], Tuple[str]]] = EXTRA_IGNORE_FIELDS_DEFAULT,
-        with_timestamp: bool = True,
-        **kwargs
+            self,
+            extra_ignore_keys: Optional[Union[List[str], Tuple[str]]] = EXTRA_IGNORE_FIELDS_DEFAULT,
+            with_timestamp: bool = True,
+            **kwargs
     ):
         """
         :param ignore_fields: 需要从 record[extra] 里忽略(排除)的字段
         :param kwargs: 这里的 key:val 会添加到格式化后的消息中 eg: app=explore
         """
         super(JsonFormatter, self).__init__()
         self.extra_ignore_keys = extra_ignore_keys
```

### Comparing `usepy_plugin_logger-0.1.4/src/usepy_logger/handlers.py` & `usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 import sys
 
 from .formatters import JsonFormatter
 
-from loguru import logger
-
 DEFAULT_HANDLER_FORMAT = "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | " \
                          "<level>{level}</level> | <level>{message}</level>"
 LOGSTASH_HANDLER_FORMAT = "{message}"
 
 
 def default_handler(level="DEBUG", format=DEFAULT_HANDLER_FORMAT, **kwargs) -> dict:
     return dict(sink=sys.stderr, level=level, format=format, **kwargs)
```

### Comparing `usepy_plugin_logger-0.1.4/src/usepy_logger/intercept.py` & `usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/intercept.py`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.4/src/usepy_logger/logger.py` & `usepy_plugin_logger-0.1.6/src/usepy_plugin_logger/logger.py`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.4/PKG-INFO` & `usepy_plugin_logger-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: usepy-plugin-logger
-Version: 0.1.4
+Version: 0.1.6
 Summary: 一个全局拦截日志并转为loguru日志的插件
 Author: nowanti
 Author-email: believel.y@qq.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
@@ -19,56 +20,55 @@
     <img src="https://img.shields.io/pypi/v/usepy-plugin-logger.svg" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/usepy-plugin-logger" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/usepy-plugin-logger.svg" alt="Supported Python versions">
 </a>
 
-#### 文档
-
-[useLogger | UsePy](https://usepy.code05.com/api/logger.html) 
-
 #### 安装
 
-> pip install usepy-plugin-logger
+> pip install 'usepy[logger]'
 
 #### 使用
 
 ```python
 from usepy import useLogger
 
-useLogger() # 使用默认配置
+useLogger()  # 使用默认配置
 
 ```
 
 如果你自身项目正在使用`loguru`，这一切似乎感觉毫无变化。因为默认的配置只是修改了一点输出样式。
 
 如果想要感受它带来的“魔法”，需要稍微配置一下。
 
 ```python
 from usepy import useLogger
-useLogger(packages=["scrapy",  "django",  "usepy"]) 
+
+useLogger(packages=["scrapy", "django", "usepy"])
 
 ```
 
 ##### Logstash/Filebeat
 
-日志的更重要能力是将日志记录发送到`Logstash`/`Filebeat`，这样就可以将日志记录存储到`Elasticsearch`中，方便进行日志分析。所以统一日志的最终输出格式是非常重要的。
+日志的更重要能力是将日志记录发送到`Logstash`/`Filebeat`，这样就可以将日志记录存储到`Elasticsearch`
+中，方便进行日志分析。所以统一日志的最终输出格式是非常重要的。
 
 `useLogger`内置一个`logstash_handler`统一化输出格式。
 
 ```python
 from loguru import logger
 from usepy import useLogger, useLoggerHandlers
+
 useLogger(
- handlers=[
-    useLoggerHandlers.logstash_handler(level="DEBUG",  extra={"app_name":  "spider"})
- ],
- packages=["usepy"],  # hook拦截 usepy 的日志
- extra={"project_name":  "usepy"}
+    handlers=[
+        useLoggerHandlers.logstash_handler(level="DEBUG", extra={"app_name": "spider"})
+    ],
+    packages=["usepy"],  # hook拦截 usepy 的日志
+    extra={"project_name": "usepy"}
 )
 logger.warning("test warning")
 logger.info("test info")
 logger.debug("test debug")
 
 ```
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: usepy-plugin-logger Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: usepy-plugin-logger Version: 0.1.6 Summary:
 ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ Author: nowanti Author-
-email: believel.y@qq.com Requires-Python: >=3.8,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru (>=0.6.0,<0.7.0) Description-Content-Type: text/markdown
-### ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ [Package_version]
-[Supported_Python_versions] #### ææ¡£ [useLogger | UsePy](https://
-usepy.code05.com/api/logger.html) #### å®è£ > pip install usepy-plugin-logger
-#### ä½¿ç¨ ```python from usepy import useLogger useLogger() #
-ä½¿ç¨é»è®¤éç½® ```
+email: believel.y@qq.com Requires-Python: >=3.7,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: loguru
+(>=0.6.0,<0.7.0) Description-Content-Type: text/markdown ###
+ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ [Package_version]
+[Supported_Python_versions] #### å®è£ > pip install 'usepy[logger]' ####
+ä½¿ç¨ ```python from usepy import useLogger useLogger() # ä½¿ç¨é»è®¤éç½®
+```
 å¦æä½ èªèº«é¡¹ç®æ­£å¨ä½¿ç¨`loguru`ï¼è¿ä¸åä¼¼ä¹æè§æ¯«æ ååãå ä¸ºé»è®¤çéç½®åªæ¯ä¿®æ¹äºä¸ç¹è¾åºæ ·å¼ã
 å¦ææ³è¦æåå®å¸¦æ¥çâé­æ³âï¼éè¦ç¨å¾®éç½®ä¸ä¸ã
 ```python from usepy import useLogger useLogger(packages=["scrapy", "django",
 "usepy"]) ``` ##### Logstash/Filebeat
 æ¥å¿çæ´éè¦è½åæ¯å°æ¥å¿è®°å½åéå°`Logstash`/
-`Filebeat`ï¼è¿æ ·å°±å¯ä»¥å°æ¥å¿è®°å½å­å¨å°`Elasticsearch`ä¸­ï¼æ¹ä¾¿è¿è¡æ¥å¿åæãæä»¥ç»ä¸æ¥å¿çæç»è¾åºæ ¼å¼æ¯éå¸¸éè¦çã
+`Filebeat`ï¼è¿æ ·å°±å¯ä»¥å°æ¥å¿è®°å½å­å¨å°`Elasticsearch`
+ä¸­ï¼æ¹ä¾¿è¿è¡æ¥å¿åæãæä»¥ç»ä¸æ¥å¿çæç»è¾åºæ ¼å¼æ¯éå¸¸éè¦çã
 `useLogger`åç½®ä¸ä¸ª`logstash_handler`ç»ä¸åè¾åºæ ¼å¼ã ```python
 from loguru import logger from usepy import useLogger, useLoggerHandlers
 useLogger( handlers=[ useLoggerHandlers.logstash_handler(level="DEBUG", extra=
 {"app_name": "spider"}) ], packages=["usepy"], # hookæ¦æª usepy çæ¥å¿
 extra={"project_name": "usepy"} ) logger.warning("test warning") logger.info
 ("test info") logger.debug("test debug") ```
```

