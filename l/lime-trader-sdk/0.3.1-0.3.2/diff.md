# Comparing `tmp/lime_trader_sdk-0.3.1.tar.gz` & `tmp/lime_trader_sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime_trader_sdk-0.3.1.tar", max compression
+gzip compressed data, was "lime_trader_sdk-0.3.2.tar", max compression
```

## Comparing `lime_trader_sdk-0.3.1.tar` & `lime_trader_sdk-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      815 2023-06-28 14:15:23.656792 lime_trader_sdk-0.3.1/README.md
--rw-r--r--   0        0        0       86 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/api/__init__.py
--rw-r--r--   0        0        0     8874 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/api/api_client.py
--rw-r--r--   0        0        0     4552 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/api/authenticated_api_client.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/api/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/api/async_api_client.py
--rw-r--r--   0        0        0     2091 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/api/async_authenticated_api_client.py
--rw-r--r--   0        0        0     2420 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/async_client.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.657792 lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_account_client.py
--rw-r--r--   0        0        0     4964 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_market_data_client.py
--rw-r--r--   0        0        0     3097 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_trading_client.py
--rw-r--r--   0        0        0     7947 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/client.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/__init__.py
--rw-r--r--   0        0        0     6775 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/account_client.py
--rw-r--r--   0        0        0     4341 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/account_feed_client.py
--rw-r--r--   0        0        0     8195 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/market_data_client.py
--rw-r--r--   0        0        0     2260 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/market_data_feed_client.py
--rw-r--r--   0        0        0     5211 2023-06-28 14:15:23.658792 lime_trader_sdk-0.3.1/lime_trader/clients/trading_client.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/constants/__init__.py
--rw-r--r--   0        0        0       21 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/constants/config.py
--rw-r--r--   0        0        0     1707 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/constants/urls.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/converters/__init__.py
--rw-r--r--   0        0        0      979 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/converters/abstract_converter.py
--rw-r--r--   0        0        0     2088 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/converters/cattr_converter.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/exceptions/__init__.py
--rw-r--r--   0        0        0      466 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/exceptions/api_error.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/handlers/__init__.py
--rw-r--r--   0        0        0     5360 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/handlers/account_feed_handler.py
--rw-r--r--   0        0        0     3272 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/handlers/market_data_feed_handler.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/__init__.py
--rw-r--r--   0        0        0     8409 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/accounts.py
--rw-r--r--   0        0        0      301 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/errors.py
--rw-r--r--   0        0        0     7798 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/market.py
--rw-r--r--   0        0        0     2311 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/page.py
--rw-r--r--   0        0        0     3054 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/token_storage.py
--rw-r--r--   0        0        0     5148 2023-06-28 14:15:23.659792 lime_trader_sdk-0.3.1/lime_trader/models/trading.py
--rw-r--r--   0        0        0        0 2023-06-28 14:15:23.660792 lime_trader_sdk-0.3.1/lime_trader/utils/__init__.py
--rw-r--r--   0        0        0     1275 2023-06-28 14:15:23.660792 lime_trader_sdk-0.3.1/lime_trader/utils/date_utils.py
--rw-r--r--   0        0        0     1480 2023-06-28 14:15:23.660792 lime_trader_sdk-0.3.1/lime_trader/utils/logging_utils.py
--rw-r--r--   0        0        0     1405 2023-06-28 14:15:23.660792 lime_trader_sdk-0.3.1/lime_trader/utils/pagination.py
--rw-r--r--   0        0        0      649 2023-06-28 14:15:23.661792 lime_trader_sdk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      815 2023-07-28 12:19:41.900092 lime_trader_sdk-0.3.2/README.md
+-rw-r--r--   0        0        0       86 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/api/__init__.py
+-rw-r--r--   0        0        0     8874 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/api/api_client.py
+-rw-r--r--   0        0        0     4552 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/api/authenticated_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/api/__init__.py
+-rw-r--r--   0        0        0     3192 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/api/async_api_client.py
+-rw-r--r--   0        0        0     2091 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/api/async_authenticated_api_client.py
+-rw-r--r--   0        0        0     2420 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/async_client.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/__init__.py
+-rw-r--r--   0        0        0     4805 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_account_client.py
+-rw-r--r--   0        0        0     4964 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_market_data_client.py
+-rw-r--r--   0        0        0     3097 2023-07-28 12:19:41.901092 lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_trading_client.py
+-rw-r--r--   0        0        0     7947 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/client.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/__init__.py
+-rw-r--r--   0        0        0     6775 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/account_client.py
+-rw-r--r--   0        0        0     4341 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/account_feed_client.py
+-rw-r--r--   0        0        0     8195 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/market_data_client.py
+-rw-r--r--   0        0        0     2260 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/market_data_feed_client.py
+-rw-r--r--   0        0        0     5211 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/clients/trading_client.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/constants/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/constants/config.py
+-rw-r--r--   0        0        0     1707 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/constants/urls.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/converters/__init__.py
+-rw-r--r--   0        0        0      979 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/converters/abstract_converter.py
+-rw-r--r--   0        0        0     2088 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/converters/cattr_converter.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.902092 lime_trader_sdk-0.3.2/lime_trader/exceptions/__init__.py
+-rw-r--r--   0        0        0      466 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/exceptions/api_error.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/handlers/__init__.py
+-rw-r--r--   0        0        0     5360 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/handlers/account_feed_handler.py
+-rw-r--r--   0        0        0     3272 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/handlers/market_data_feed_handler.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/__init__.py
+-rw-r--r--   0        0        0     8409 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/accounts.py
+-rw-r--r--   0        0        0      301 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/errors.py
+-rw-r--r--   0        0        0     7798 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/market.py
+-rw-r--r--   0        0        0     2311 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/page.py
+-rw-r--r--   0        0        0     3054 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/token_storage.py
+-rw-r--r--   0        0        0     5060 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/models/trading.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/utils/__init__.py
+-rw-r--r--   0        0        0     1275 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/utils/date_utils.py
+-rw-r--r--   0        0        0     1480 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/utils/logging_utils.py
+-rw-r--r--   0        0        0     1405 2023-07-28 12:19:41.903092 lime_trader_sdk-0.3.2/lime_trader/utils/pagination.py
+-rw-r--r--   0        0        0      649 2023-07-28 12:19:41.904092 lime_trader_sdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 lime_trader_sdk-0.3.2/PKG-INFO
```

### Comparing `lime_trader_sdk-0.3.1/README.md` & `lime_trader_sdk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/api/api_client.py` & `lime_trader_sdk-0.3.2/lime_trader/api/api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/api/authenticated_api_client.py` & `lime_trader_sdk-0.3.2/lime_trader/api/authenticated_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/api/async_api_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/api/async_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/api/async_authenticated_api_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/api/async_authenticated_api_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/async_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/async_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_account_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_market_data_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_market_data_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/async_trader/clients/async_trading_client.py` & `lime_trader_sdk-0.3.2/lime_trader/async_trader/clients/async_trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/client.py` & `lime_trader_sdk-0.3.2/lime_trader/client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/clients/account_client.py` & `lime_trader_sdk-0.3.2/lime_trader/clients/account_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/clients/account_feed_client.py` & `lime_trader_sdk-0.3.2/lime_trader/clients/account_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/clients/market_data_client.py` & `lime_trader_sdk-0.3.2/lime_trader/clients/market_data_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/clients/market_data_feed_client.py` & `lime_trader_sdk-0.3.2/lime_trader/clients/market_data_feed_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/clients/trading_client.py` & `lime_trader_sdk-0.3.2/lime_trader/clients/trading_client.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/constants/urls.py` & `lime_trader_sdk-0.3.2/lime_trader/constants/urls.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/converters/abstract_converter.py` & `lime_trader_sdk-0.3.2/lime_trader/converters/abstract_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/converters/cattr_converter.py` & `lime_trader_sdk-0.3.2/lime_trader/converters/cattr_converter.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/handlers/account_feed_handler.py` & `lime_trader_sdk-0.3.2/lime_trader/handlers/account_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/handlers/market_data_feed_handler.py` & `lime_trader_sdk-0.3.2/lime_trader/handlers/market_data_feed_handler.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/models/accounts.py` & `lime_trader_sdk-0.3.2/lime_trader/models/accounts.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/models/market.py` & `lime_trader_sdk-0.3.2/lime_trader/models/market.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/models/page.py` & `lime_trader_sdk-0.3.2/lime_trader/models/page.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/models/token_storage.py` & `lime_trader_sdk-0.3.2/lime_trader/models/token_storage.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/models/trading.py` & `lime_trader_sdk-0.3.2/lime_trader/models/trading.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     REJECTED = "rejected"
     DONE_FOR_DAY = "done_for_day"
     EXPIRED = "expired"
 
 
 class TimeInForce(enum.Enum):
     DAY = "day"
-    GOOD_TILL_CANCEL = "good_till_cancel"
-    GOOD_TILL_CROSSING = "good_till_crossing"
 
 
 class OrderType(enum.Enum):
     MARKET = "market"
     LIMIT = "limit"
     STOP = "stop"
     STOP_LIMIT = "stop_limit"
```

### Comparing `lime_trader_sdk-0.3.1/lime_trader/utils/date_utils.py` & `lime_trader_sdk-0.3.2/lime_trader/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/utils/logging_utils.py` & `lime_trader_sdk-0.3.2/lime_trader/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/lime_trader/utils/pagination.py` & `lime_trader_sdk-0.3.2/lime_trader/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `lime_trader_sdk-0.3.1/pyproject.toml` & `lime_trader_sdk-0.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lime-trader-sdk"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python wrapper for Lime Trader REST API (https://docs.lime.co/trader/)"
 authors = ["Lime Financial <support@lime.co>"]
 readme = "README.md"
 packages = [{include = "lime_trader"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `lime_trader_sdk-0.3.1/PKG-INFO` & `lime_trader_sdk-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-trader-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python wrapper for Lime Trader REST API (https://docs.lime.co/trader/)
 Author: Lime Financial
 Author-email: support@lime.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

