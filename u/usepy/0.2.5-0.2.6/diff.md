# Comparing `tmp/usepy-0.2.5.tar.gz` & `tmp/usepy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy-0.2.5.tar", max compression
+gzip compressed data, was "usepy-0.2.6.tar", max compression
```

## Comparing `usepy-0.2.5.tar` & `usepy-0.2.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     1756 2023-07-20 02:47:09.435456 usepy-0.2.5/README.md
--rw-r--r--   0        0        0      619 2023-07-20 02:47:09.447456 usepy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3624 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/contrib/__init__.py
--rw-r--r--   0        0        0     1295 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/contrib/pydantic_.py
--rw-r--r--   0        0        0     2039 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/contrib/tenacity_.py
--rw-r--r--   0        0        0        0 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/core/__init__.py
--rw-r--r--   0        0        0     5575 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/core/useAddict.py
--rw-r--r--   0        0        0     2075 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/core/useBloomFilter.py
--rw-r--r--   0        0        0      467 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/core/useCachedProperty.py
--rw-r--r--   0        0        0      417 2023-07-20 02:47:09.447456 usepy-0.2.5/src/usepy/core/useCatchError.py
--rw-r--r--   0        0        0      883 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useCleanHtml.py
--rw-r--r--   0        0        0     1059 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useCounter.py
--rw-r--r--   0        0        0     6468 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useDateTime.py
--rw-r--r--   0        0        0     8828 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useDict.py
--rw-r--r--   0        0        0     1529 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useImport.py
--rw-r--r--   0        0        0      692 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useIs.py
--rw-r--r--   0        0        0     9024 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useList.py
--rw-r--r--   0        0        0      419 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useListify.py
--rw-r--r--   0        0        0     2909 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/usePath.py
--rw-r--r--   0        0        0      596 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useRandom.py
--rw-r--r--   0        0        0     1814 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useRetry.py
--rw-r--r--   0        0        0      379 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useRunInThread.py
--rw-r--r--   0        0        0      522 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useSingleton.py
--rw-r--r--   0        0        0     3146 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useString.py
--rw-r--r--   0        0        0      552 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useStringDecode.py
--rw-r--r--   0        0        0      534 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useStringEncode.py
--rw-r--r--   0        0        0      229 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useStringReverse.py
--rw-r--r--   0        0        0     1158 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useThread.py
--rw-r--r--   0        0        0      352 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useTimeIt.py
--rw-r--r--   0        0        0      840 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useTimeout.py
--rw-r--r--   0        0        0     4748 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useTimer.py
--rw-r--r--   0        0        0     2558 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/core/useTo.py
--rw-r--r--   0        0        0        0 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/__init__.py
--rw-r--r--   0        0        0     3399 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useCURL.py
--rw-r--r--   0        0        0      221 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useCookieToDict.py
--rw-r--r--   0        0        0      239 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useDataToDict.py
--rw-r--r--   0        0        0      267 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useHeaderToDict.py
--rw-r--r--   0        0        0     1382 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useURL.py
--rw-r--r--   0        0        0   711543 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/crawl/useUserAgent.py
--rw-r--r--   0        0        0        9 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/__init__.py
--rw-r--r--   0        0        0      266 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useLogger/__init__.py
--rw-r--r--   0        0        0     2042 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useLogger/formatters.py
--rw-r--r--   0        0        0     1149 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useLogger/handlers.py
--rw-r--r--   0        0        0     2791 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useLogger/intercept.py
--rw-r--r--   0        0        0     2087 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useLogger/logger.py
--rw-r--r--   0        0        0       84 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/__init__.py
--rw-r--r--   0        0        0      219 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/__init__.py
--rw-r--r--   0        0        0      508 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/bark.py
--rw-r--r--   0        0        0      271 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/base.py
--rw-r--r--   0        0        0      597 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/chanify.py
--rw-r--r--   0        0        0      897 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/ding.py
--rw-r--r--   0        0        0     1027 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/email.py
--rw-r--r--   0        0        0      578 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/pushdeer.py
--rw-r--r--   0        0        0      688 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/pushover.py
--rw-r--r--   0        0        0      675 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/channels/wechat.py
--rw-r--r--   0        0        0      534 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/integrations/useNotify/notification.py
--rw-r--r--   0        0        0        0 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/utils/__init__.py
--rw-r--r--   0        0        0      410 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/utils/useFormatSizeof.py
--rw-r--r--   0        0        0      306 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/utils/useFuncName.py
--rw-r--r--   0        0        0       38 2023-07-20 02:47:09.451456 usepy-0.2.5/src/usepy/vars.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 usepy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1756 2023-07-28 07:12:33.067802 usepy-0.2.6/README.md
+-rw-r--r--   0        0        0      618 2023-07-28 07:12:33.079802 usepy-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3624 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/contrib/__init__.py
+-rw-r--r--   0        0        0     1295 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/contrib/pydantic_.py
+-rw-r--r--   0        0        0     2039 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/contrib/tenacity_.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/__init__.py
+-rw-r--r--   0        0        0     5575 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useAddict.py
+-rw-r--r--   0        0        0     2075 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useBloomFilter.py
+-rw-r--r--   0        0        0      467 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useCachedProperty.py
+-rw-r--r--   0        0        0      417 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useCatchError.py
+-rw-r--r--   0        0        0      883 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useCleanHtml.py
+-rw-r--r--   0        0        0     1059 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useCounter.py
+-rw-r--r--   0        0        0     6468 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useDateTime.py
+-rw-r--r--   0        0        0     8828 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useDict.py
+-rw-r--r--   0        0        0     1529 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useImport.py
+-rw-r--r--   0        0        0      692 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useIs.py
+-rw-r--r--   0        0        0     9024 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useList.py
+-rw-r--r--   0        0        0      419 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useListify.py
+-rw-r--r--   0        0        0     2909 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/usePath.py
+-rw-r--r--   0        0        0      596 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useRandom.py
+-rw-r--r--   0        0        0     1814 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useRetry.py
+-rw-r--r--   0        0        0      379 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useRunInThread.py
+-rw-r--r--   0        0        0      522 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useSingleton.py
+-rw-r--r--   0        0        0     3146 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useString.py
+-rw-r--r--   0        0        0      552 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useStringDecode.py
+-rw-r--r--   0        0        0      534 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useStringEncode.py
+-rw-r--r--   0        0        0      229 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useStringReverse.py
+-rw-r--r--   0        0        0     1158 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useThread.py
+-rw-r--r--   0        0        0      352 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useTimeIt.py
+-rw-r--r--   0        0        0      840 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useTimeout.py
+-rw-r--r--   0        0        0     4748 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useTimer.py
+-rw-r--r--   0        0        0     2558 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/core/useTo.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/useCURL.py
+-rw-r--r--   0        0        0      221 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/useCookieToDict.py
+-rw-r--r--   0        0        0      239 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/useDataToDict.py
+-rw-r--r--   0        0        0      267 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/useHeaderToDict.py
+-rw-r--r--   0        0        0     1382 2023-07-28 07:12:33.079802 usepy-0.2.6/src/usepy/crawl/useURL.py
+-rw-r--r--   0        0        0   711543 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/crawl/useUserAgent.py
+-rw-r--r--   0        0        0        9 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useLogger/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useLogger/formatters.py
+-rw-r--r--   0        0        0     1149 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useLogger/handlers.py
+-rw-r--r--   0        0        0     2791 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useLogger/intercept.py
+-rw-r--r--   0        0        0     2087 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useLogger/logger.py
+-rw-r--r--   0        0        0       84 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/__init__.py
+-rw-r--r--   0        0        0      508 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/bark.py
+-rw-r--r--   0        0        0      271 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/base.py
+-rw-r--r--   0        0        0      597 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/chanify.py
+-rw-r--r--   0        0        0      897 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/ding.py
+-rw-r--r--   0        0        0     1027 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/email.py
+-rw-r--r--   0        0        0      578 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/pushdeer.py
+-rw-r--r--   0        0        0      688 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/pushover.py
+-rw-r--r--   0        0        0      675 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/channels/wechat.py
+-rw-r--r--   0        0        0      534 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/integrations/useNotify/notification.py
+-rw-r--r--   0        0        0      786 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/utils/__init__.py
+-rw-r--r--   0        0        0      410 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/utils/useFormatSizeof.py
+-rw-r--r--   0        0        0      306 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/utils/useFuncName.py
+-rw-r--r--   0        0        0       38 2023-07-28 07:12:33.083802 usepy-0.2.6/src/usepy/vars.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 usepy-0.2.6/PKG-INFO
```

### Comparing `usepy-0.2.5/README.md` & `usepy-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/pyproject.toml` & `usepy-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usepy"
-version = "0.2.5"
+version = "0.2.6"
 description = "usepy"
 homepage = "https://usepy.code05.com/"
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'usepy', from = 'src' }
 ]
@@ -13,15 +13,14 @@
 python = "^3.7"
 typing-extensions = [
     { version = "^4.0.0", python = ">=3.6,<3.7" },
     { version = "^4.5.0", python = ">=3.7" }
 ]
 
 
-
 [tool.poetry.group.test.dependencies]
 pytest = [
     { version = "^7.0.0", python = ">=3.6,<3.7" },
     { version = "^7.3.1", python = ">=3.7" }
 ]
 
 [build-system]
```

### Comparing `usepy-0.2.5/src/usepy/__init__.py` & `usepy-0.2.6/src/usepy/__init__.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/contrib/pydantic_.py` & `usepy-0.2.6/src/usepy/contrib/pydantic_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/contrib/tenacity_.py` & `usepy-0.2.6/src/usepy/contrib/tenacity_.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useAddict.py` & `usepy-0.2.6/src/usepy/core/useAddict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useBloomFilter.py` & `usepy-0.2.6/src/usepy/core/useBloomFilter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useCleanHtml.py` & `usepy-0.2.6/src/usepy/core/useCleanHtml.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useCounter.py` & `usepy-0.2.6/src/usepy/core/useCounter.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useDateTime.py` & `usepy-0.2.6/src/usepy/core/useDateTime.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useDict.py` & `usepy-0.2.6/src/usepy/core/useDict.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useImport.py` & `usepy-0.2.6/src/usepy/core/useImport.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useIs.py` & `usepy-0.2.6/src/usepy/core/useIs.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useList.py` & `usepy-0.2.6/src/usepy/core/useList.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/usePath.py` & `usepy-0.2.6/src/usepy/core/usePath.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useRandom.py` & `usepy-0.2.6/src/usepy/core/useRandom.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useRetry.py` & `usepy-0.2.6/src/usepy/core/useRetry.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useSingleton.py` & `usepy-0.2.6/src/usepy/core/useSingleton.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useString.py` & `usepy-0.2.6/src/usepy/core/useString.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useStringDecode.py` & `usepy-0.2.6/src/usepy/core/useStringDecode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useStringEncode.py` & `usepy-0.2.6/src/usepy/core/useStringEncode.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useThread.py` & `usepy-0.2.6/src/usepy/core/useThread.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useTimeout.py` & `usepy-0.2.6/src/usepy/core/useTimeout.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useTimer.py` & `usepy-0.2.6/src/usepy/core/useTimer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/core/useTo.py` & `usepy-0.2.6/src/usepy/core/useTo.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/crawl/useCURL.py` & `usepy-0.2.6/src/usepy/crawl/useCURL.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/crawl/useURL.py` & `usepy-0.2.6/src/usepy/crawl/useURL.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/crawl/useUserAgent.py` & `usepy-0.2.6/src/usepy/crawl/useUserAgent.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useLogger/formatters.py` & `usepy-0.2.6/src/usepy/integrations/useLogger/formatters.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useLogger/handlers.py` & `usepy-0.2.6/src/usepy/integrations/useLogger/handlers.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useLogger/intercept.py` & `usepy-0.2.6/src/usepy/integrations/useLogger/intercept.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useLogger/logger.py` & `usepy-0.2.6/src/usepy/integrations/useLogger/logger.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/chanify.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/chanify.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/ding.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/ding.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/email.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/email.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/pushdeer.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/pushdeer.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/pushover.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/pushover.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/channels/wechat.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/channels/wechat.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/src/usepy/integrations/useNotify/notification.py` & `usepy-0.2.6/src/usepy/integrations/useNotify/notification.py`

 * *Files identical despite different names*

### Comparing `usepy-0.2.5/PKG-INFO` & `usepy-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usepy
-Version: 0.2.5
+Version: 0.2.6
 Summary: usepy
 Home-page: https://usepy.code05.com/
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usepy Version: 0.2.5 Summary: usepy Home-page:
+Metadata-Version: 2.1 Name: usepy Version: 0.2.6 Summary: usepy Home-page:
 https://usepy.code05.com/ Author: miclon Author-email: jcnd@163.com Requires-
 Python: >=3.7,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) ;
 python_version >= "3.6" and python_version < "3.7" Requires-Dist: typing-
```

