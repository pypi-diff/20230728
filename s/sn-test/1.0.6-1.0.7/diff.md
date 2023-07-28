# Comparing `tmp/sn_test-1.0.6.tar.gz` & `tmp/sn_test-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sn_test-1.0.6.tar", last modified: Fri Jul 28 08:08:40 2023, max compression
+gzip compressed data, was "dist/sn_test-1.0.7.tar", last modified: Fri Jul 28 08:14:32 2023, max compression
```

## Comparing `sn_test-1.0.6.tar` & `sn_test-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:08:40.000000 sn_test-1.0.6/
--rw-r--r--   0 mac        (501) staff       (20)     4731 2023-07-28 08:08:40.000000 sn_test-1.0.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-28 08:08:32.000000 sn_test-1.0.6/set_up.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 08:08:40.000000 sn_test-1.0.6/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:08:40.000000 sn_test-1.0.6/sn_test/
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 08:42:56.000000 sn_test-1.0.6/sn_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.6/sn_test/test_sn.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:08:40.000000 sn_test-1.0.6/sn_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     4731 2023-07-28 08:08:39.000000 sn_test-1.0.6/sn_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-28 08:08:39.000000 sn_test-1.0.6/sn_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 08:08:39.000000 sn_test-1.0.6/sn_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-28 08:08:39.000000 sn_test-1.0.6/sn_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 08:08:39.000000 sn_test-1.0.6/sn_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)     5081 2023-07-28 08:14:32.000000 sn_test-1.0.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3180 2023-07-28 08:14:25.000000 sn_test-1.0.7/set_up.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-28 08:14:32.000000 sn_test-1.0.7/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/sn_test/
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-07-21 08:42:56.000000 sn_test-1.0.7/sn_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      294 2023-07-21 06:40:48.000000 sn_test-1.0.7/sn_test/test_sn.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-28 08:14:32.000000 sn_test-1.0.7/sn_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     5081 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      202 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-28 08:14:31.000000 sn_test-1.0.7/sn_test.egg-info/top_level.txt
```

### Comparing `sn_test-1.0.6/PKG-INFO` & `sn_test-1.0.7/sn_test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sn_test
-Version: 1.0.6
+Name: sn-test
+Version: 1.0.7
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
 Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,16 +12,102 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-#### GET https://dma-api.defi.wiki/redoc
-<a href="#test">跳转get_market</a>
+#### zerocap-api-test使用
+
+# <a href="#testapi">跳转restapi</a>
+# <a href="#test">跳转websocket</a>
+
+
+
+```
+各种描述
+公司介绍
+等等描述
+1
+
+1
+1
+
+1
+1
+1
+1
+1
+1
+
+1
+1
+1
+
+1
+1
+1
+
+1
+1
+2
+2
+2
+
+2
+2
+
+2
+2
+2
+2
+
+2
+
+2
+2
+
+2
+2
+2
+
+2
+```
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+<a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi 接口文档</a>
+GET https://dma-api.defi.wiki/redoc
+
+
+
+
+
+
+```
+restapi 的使用
+。。。。。。。。。
+
+
+```
+
+
+
 
 请求参数:
 
 | 参数名称 | 是否必须 | 类型   | 描述                            | 默认值 | 取值范围                                                     |
 | -------- | -------- | ------ | ------------------------------- | ------ | ------------------------------------------------------------ |
 | symbol   | true     | string | 交易对                          |        | btcbitcny, bchbtc, eoseth ...                                |
 | types    | false    | string | 查询的订单类型组合，使用','分割 | 全部   | buy-market：市价买, sell-market：市价卖, buy-limit：限价买, sell-limit：限价卖 |
@@ -54,18 +140,15 @@
 
 
 
 
 
 
 
-
-
-
-<span id='test'>get matket</span>
+## <span id='test'>websocket</span>
 
 ```
 GET https://dma-api.defi.wiki/redoc
 ```
 响应数据:
 
 | 参数名称    | 是否必须 | 数据类型 | 描述           | 取值范围                                                     |
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1 Name: sn_test Version: 1.0.6 Summary: shuainan test Home-
+Metadata-Version: 2.1 Name: sn-test Version: 1.0.7 Summary: shuainan test Home-
 page: https://github.com/me/myproject Author: shuainan Author-email:
 15294627382@163.com License: MIT Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.6.0 Description-Content-Type: text/markdown #### GET https://dma-
-api.defi.wiki/redoc è·³è½¬get_market è¯·æ±åæ°: | åæ°åç§° |
+Python: >=3.6.0 Description-Content-Type: text/markdown #### zerocap-api-
+testä½¿ç¨ # è·³è½¬restapi # è·³è½¬websocket ``` åç§æè¿° å¬å¸ä»ç»
+ç­ç­æè¿° 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2
+``` restapi_æ¥å£ææ¡£ GET https://dma-api.defi.wiki/redoc ``` restapi
+çä½¿ç¨ ããããããããã ``` è¯·æ±åæ°: | åæ°åç§° |
 æ¯å¦å¿é¡» | ç±»å | æè¿° | é»è®¤å¼ | åå¼èå´ | | -------- | ------
 -- | ------ | ------------------------------- | ------ | ----------------------
 -------------------------------------- | | symbol | true | string | äº¤æå¯¹ |
 | btcbitcny, bchbtc, eoseth ... | | types | false | string |
 æ¥è¯¢çè®¢åç±»åç»åï¼ä½¿ç¨','åå² | å¨é¨ | buy-
 marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
 limitï¼éä»·å | | states | true | string |
 æ¥è¯¢çè®¢åç¶æç»åï¼ä½¿ç¨','åå² | | new ï¼æ°è®¢å, part_filled
 ï¼é¨åæäº¤ | | from | false | string | æ¥è¯¢èµ·å§ ID ï¼è®¢åIDï¼ | |
 éådirect ä½¿ç¨ | | direct | false | string | æ¥è¯¢æ¹å | next | prev
 ååï¼next åå | | size | false | string | æ¥è¯¢è®°å½å¤§å° | 50 |
 æå¤ä¸æ¬¡æ¥è¯¢50æ¡æ°æ® | | time | true | string | å½åæ¶é´æ³ | | |
-è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ get
-matket ``` GET https://dma-api.defi.wiki/redoc ``` ååºæ°æ®: | åæ°åç§°
-| æ¯å¦å¿é¡» | æ°æ®ç±»å | æè¿° | åå¼èå´ | | ----------- | -------
-- | -------- | -------------- | -----------------------------------------------
-------------- | | id | true | string | è®¢åid | | | user_id | true | long |
-è´¦æ· ID | | | volume | true | string | è®¢åæ°é | | | deal_volume | false
-| string | æäº¤æ°é | | | deal_money | true | string | å·²æäº¤éé¢ | |
-| fee | true | string | æç»­è´¹ | | | price | true | string |
-éä»·åæåä»·æ ¼ | | | status | false | string | è®¢åç¶æ | 0 æ 1
-ï¼æ°è®¢å, 3 ï¼é¨åæäº¤ | | type | true | string | è®¢åç±»å | buy-
-marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
+è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ##
+websocket ``` GET https://dma-api.defi.wiki/redoc ``` ååºæ°æ®: |
+åæ°åç§° | æ¯å¦å¿é¡» | æ°æ®ç±»å | æè¿° | åå¼èå´ | | --------
+--- | -------- | -------- | -------------- | ----------------------------------
+-------------------------- | | id | true | string | è®¢åid | | | user_id |
+true | long | è´¦æ· ID | | | volume | true | string | è®¢åæ°é | | |
+deal_volume | false | string | æäº¤æ°é | | | deal_money | true | string |
+å·²æäº¤éé¢ | | | fee | true | string | æç»­è´¹ | | | price | true |
+string | éä»·åæåä»·æ ¼ | | | status | false | string | è®¢åç¶æ | 0
+æ 1 ï¼æ°è®¢å, 3 ï¼é¨åæäº¤ | | type | true | string | è®¢åç±»å |
+buy-marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
 limitï¼éä»·å | | source | true | string | è®¢åæ¥æº | api | | symbol |
 true | string | äº¤æå¯¹ | btcbitcny, eoseth, ethbtc ... | | ctime | true |
 string | è®¢ååå»ºæ¶é´ | æ¶é´ååº | | mtime | true | string |
 æåæäº¤æ¶é´ | | ååºä¾å­: ``` { "code": '0', "msg": "suc", "data":
 [ { "symbol": "ethbtc", "fee": "0.00100000", "avg_price": "0.07231094",
 "source": 1, "type": "buy-limit", "mtime": 1524823324000, "volume": "1.000",
 "user_id": 10278, "price": "0.07231094", "ctime": 1524823301000, "deal_volume":
```

### Comparing `sn_test-1.0.6/set_up.py` & `sn_test-1.0.7/set_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'sn_test'
 DESCRIPTION = 'shuainan test'
 URL = 'https://github.com/me/myproject'
 EMAIL = '15294627382@163.com'
 AUTHOR = 'shuainan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'websocket'
 ]
```

### Comparing `sn_test-1.0.6/sn_test.egg-info/PKG-INFO` & `sn_test-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sn-test
-Version: 1.0.6
+Name: sn_test
+Version: 1.0.7
 Summary: shuainan test
 Home-page: https://github.com/me/myproject
 Author: shuainan
 Author-email: 15294627382@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,16 +12,102 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 
-#### GET https://dma-api.defi.wiki/redoc
-<a href="#test">跳转get_market</a>
+#### zerocap-api-test使用
+
+# <a href="#testapi">跳转restapi</a>
+# <a href="#test">跳转websocket</a>
+
+
+
+```
+各种描述
+公司介绍
+等等描述
+1
+
+1
+1
+
+1
+1
+1
+1
+1
+1
+
+1
+1
+1
+
+1
+1
+1
+
+1
+1
+2
+2
+2
+
+2
+2
+
+2
+2
+2
+2
+
+2
+
+2
+2
+
+2
+2
+2
+
+2
+```
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+<a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi 接口文档</a>
+GET https://dma-api.defi.wiki/redoc
+
+
+
+
+
+
+```
+restapi 的使用
+。。。。。。。。。
+
+
+```
+
+
+
 
 请求参数:
 
 | 参数名称 | 是否必须 | 类型   | 描述                            | 默认值 | 取值范围                                                     |
 | -------- | -------- | ------ | ------------------------------- | ------ | ------------------------------------------------------------ |
 | symbol   | true     | string | 交易对                          |        | btcbitcny, bchbtc, eoseth ...                                |
 | types    | false    | string | 查询的订单类型组合，使用','分割 | 全部   | buy-market：市价买, sell-market：市价卖, buy-limit：限价买, sell-limit：限价卖 |
@@ -54,18 +140,15 @@
 
 
 
 
 
 
 
-
-
-
-<span id='test'>get matket</span>
+## <span id='test'>websocket</span>
 
 ```
 GET https://dma-api.defi.wiki/redoc
 ```
 响应数据:
 
 | 参数名称    | 是否必须 | 数据类型 | 描述           | 取值范围                                                     |
```

#### html2text {}

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1 Name: sn-test Version: 1.0.6 Summary: shuainan test Home-
+Metadata-Version: 2.1 Name: sn_test Version: 1.0.7 Summary: shuainan test Home-
 page: https://github.com/me/myproject Author: shuainan Author-email:
 15294627382@163.com License: MIT Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.6.0 Description-Content-Type: text/markdown #### GET https://dma-
-api.defi.wiki/redoc è·³è½¬get_market è¯·æ±åæ°: | åæ°åç§° |
+Python: >=3.6.0 Description-Content-Type: text/markdown #### zerocap-api-
+testä½¿ç¨ # è·³è½¬restapi # è·³è½¬websocket ``` åç§æè¿° å¬å¸ä»ç»
+ç­ç­æè¿° 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2
+``` restapi_æ¥å£ææ¡£ GET https://dma-api.defi.wiki/redoc ``` restapi
+çä½¿ç¨ ããããããããã ``` è¯·æ±åæ°: | åæ°åç§° |
 æ¯å¦å¿é¡» | ç±»å | æè¿° | é»è®¤å¼ | åå¼èå´ | | -------- | ------
 -- | ------ | ------------------------------- | ------ | ----------------------
 -------------------------------------- | | symbol | true | string | äº¤æå¯¹ |
 | btcbitcny, bchbtc, eoseth ... | | types | false | string |
 æ¥è¯¢çè®¢åç±»åç»åï¼ä½¿ç¨','åå² | å¨é¨ | buy-
 marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
 limitï¼éä»·å | | states | true | string |
 æ¥è¯¢çè®¢åç¶æç»åï¼ä½¿ç¨','åå² | | new ï¼æ°è®¢å, part_filled
 ï¼é¨åæäº¤ | | from | false | string | æ¥è¯¢èµ·å§ ID ï¼è®¢åIDï¼ | |
 éådirect ä½¿ç¨ | | direct | false | string | æ¥è¯¢æ¹å | next | prev
 ååï¼next åå | | size | false | string | æ¥è¯¢è®°å½å¤§å° | 50 |
 æå¤ä¸æ¬¡æ¥è¯¢50æ¡æ°æ® | | time | true | string | å½åæ¶é´æ³ | | |
-è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ get
-matket ``` GET https://dma-api.defi.wiki/redoc ``` ååºæ°æ®: | åæ°åç§°
-| æ¯å¦å¿é¡» | æ°æ®ç±»å | æè¿° | åå¼èå´ | | ----------- | -------
-- | -------- | -------------- | -----------------------------------------------
-------------- | | id | true | string | è®¢åid | | | user_id | true | long |
-è´¦æ· ID | | | volume | true | string | è®¢åæ°é | | | deal_volume | false
-| string | æäº¤æ°é | | | deal_money | true | string | å·²æäº¤éé¢ | |
-| fee | true | string | æç»­è´¹ | | | price | true | string |
-éä»·åæåä»·æ ¼ | | | status | false | string | è®¢åç¶æ | 0 æ 1
-ï¼æ°è®¢å, 3 ï¼é¨åæäº¤ | | type | true | string | è®¢åç±»å | buy-
-marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
+è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ##
+websocket ``` GET https://dma-api.defi.wiki/redoc ``` ååºæ°æ®: |
+åæ°åç§° | æ¯å¦å¿é¡» | æ°æ®ç±»å | æè¿° | åå¼èå´ | | --------
+--- | -------- | -------- | -------------- | ----------------------------------
+-------------------------- | | id | true | string | è®¢åid | | | user_id |
+true | long | è´¦æ· ID | | | volume | true | string | è®¢åæ°é | | |
+deal_volume | false | string | æäº¤æ°é | | | deal_money | true | string |
+å·²æäº¤éé¢ | | | fee | true | string | æç»­è´¹ | | | price | true |
+string | éä»·åæåä»·æ ¼ | | | status | false | string | è®¢åç¶æ | 0
+æ 1 ï¼æ°è®¢å, 3 ï¼é¨åæäº¤ | | type | true | string | è®¢åç±»å |
+buy-marketï¼å¸ä»·ä¹°, sell-marketï¼å¸ä»·å, buy-limitï¼éä»·ä¹°, sell-
 limitï¼éä»·å | | source | true | string | è®¢åæ¥æº | api | | symbol |
 true | string | äº¤æå¯¹ | btcbitcny, eoseth, ethbtc ... | | ctime | true |
 string | è®¢ååå»ºæ¶é´ | æ¶é´ååº | | mtime | true | string |
 æåæäº¤æ¶é´ | | ååºä¾å­: ``` { "code": '0', "msg": "suc", "data":
 [ { "symbol": "ethbtc", "fee": "0.00100000", "avg_price": "0.07231094",
 "source": 1, "type": "buy-limit", "mtime": 1524823324000, "volume": "1.000",
 "user_id": 10278, "price": "0.07231094", "ctime": 1524823301000, "deal_volume":
```

