# Comparing `tmp/APIConnect-2.0.2.tar.gz` & `tmp/APIConnect-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIConnect-2.0.2.tar", last modified: Fri May 19 16:53:15 2023, max compression
+gzip compressed data, was "APIConnect-2.0.3.tar", last modified: Fri Jul 28 13:21:20 2023, max compression
```

## Comparing `APIConnect-2.0.2.tar` & `APIConnect-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.320442 APIConnect-2.0.2/
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.285652 APIConnect-2.0.2/APIConnect/
--rw-r--r--   0 saurabh    (502) staff       (20)    66126 2023-05-19 14:30:01.000000 APIConnect-2.0.2/APIConnect/APIConnect.py
--rw-r--r--   0 saurabh    (502) staff       (20)     1877 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/api_constants.py
--rw-r--r--   0 saurabh    (502) staff       (20)     3234 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/api_utils.py
--rw-r--r--   0 saurabh    (502) staff       (20)     6501 2023-03-16 11:10:11.000000 APIConnect-2.0.2/APIConnect/http.py
--rw-r--r--   0 saurabh    (502) staff       (20)     5379 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/login_helper.py
--rw-r--r--   0 saurabh    (502) staff       (20)     3788 2023-03-23 11:20:24.000000 APIConnect-2.0.2/APIConnect/order.py
--rw-r--r--   0 saurabh    (502) staff       (20)     4696 2023-05-03 11:18:05.000000 APIConnect-2.0.2/APIConnect/validator.py
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.289817 APIConnect-2.0.2/APIConnect.egg-info/
--rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/PKG-INFO
--rw-r--r--   0 saurabh    (502) staff       (20)     1022 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh    (502) staff       (20)        1 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh    (502) staff       (20)       33 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/requires.txt
--rw-r--r--   0 saurabh    (502) staff       (20)       56 2023-05-19 16:53:15.000000 APIConnect-2.0.2/APIConnect.egg-info/top_level.txt
--rw-r--r--   0 saurabh    (502) staff       (20)     1140 2023-03-16 11:10:11.000000 APIConnect-2.0.2/LICENSE.txt
--rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-05-19 16:53:15.319292 APIConnect-2.0.2/PKG-INFO
--rw-r--r--   0 saurabh    (502) staff       (20)       40 2023-03-16 11:10:11.000000 APIConnect-2.0.2/README
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.290363 APIConnect-2.0.2/conf/
--rw-r--r--   0 saurabh    (502) staff       (20)      354 2023-05-19 10:57:43.000000 APIConnect-2.0.2/conf/settings.ini
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.304233 APIConnect-2.0.2/constants/
--rw-r--r--   0 saurabh    (502) staff       (20)      173 2023-05-03 11:18:05.000000 APIConnect-2.0.2/constants/action.py
--rw-r--r--   0 saurabh    (502) staff       (20)      363 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/asset_type.py
--rw-r--r--   0 saurabh    (502) staff       (20)      278 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/chart_exchange.py
--rw-r--r--   0 saurabh    (502) staff       (20)      624 2023-05-19 10:58:48.000000 APIConnect-2.0.2/constants/constants.py
--rw-r--r--   0 saurabh    (502) staff       (20)      222 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/duration.py
--rw-r--r--   0 saurabh    (502) staff       (20)      193 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/eod_Interval.py
--rw-r--r--   0 saurabh    (502) staff       (20)      242 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/exchange.py
--rw-r--r--   0 saurabh    (502) staff       (20)      247 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/intraday_interval.py
--rw-r--r--   0 saurabh    (502) staff       (20)      244 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/order_type.py
--rw-r--r--   0 saurabh    (502) staff       (20)      238 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/product_code.py
--rw-r--r--   0 saurabh    (502) staff       (20)      236 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/results_stocks_news_category.py
--rw-r--r--   0 saurabh    (502) staff       (20)     8275 2023-05-03 11:18:05.000000 APIConnect-2.0.2/constants/router.py
--rw-r--r--   0 saurabh    (502) staff       (20)      224 2023-03-16 11:10:11.000000 APIConnect-2.0.2/constants/streaming_constants.py
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.306627 APIConnect-2.0.2/exceptions/
--rw-r--r--   0 saurabh    (502) staff       (20)      180 2023-03-16 11:10:11.000000 APIConnect-2.0.2/exceptions/api_exception.py
--rw-r--r--   0 saurabh    (502) staff       (20)      384 2023-03-16 11:10:11.000000 APIConnect-2.0.2/exceptions/validation_exception.py
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.312050 APIConnect-2.0.2/feed/
--rw-r--r--   0 saurabh    (502) staff       (20)     5961 2023-05-19 14:29:36.000000 APIConnect-2.0.2/feed/feed.py
--rw-r--r--   0 saurabh    (502) staff       (20)     1577 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/livenews_feed.py
--rw-r--r--   0 saurabh    (502) staff       (20)     2046 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/orders_feed.py
--rw-r--r--   0 saurabh    (502) staff       (20)     2091 2023-03-16 11:10:11.000000 APIConnect-2.0.2/feed/quotes_feed.py
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.315244 APIConnect-2.0.2/resources/
--rw-r--r--   0 saurabh    (502) staff       (20)     1123 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/chart_response_formatter.py
--rw-r--r--   0 saurabh    (502) staff       (20)     4635 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/live_news_resource.py
--rw-r--r--   0 saurabh    (502) staff       (20)      901 2023-03-16 11:10:11.000000 APIConnect-2.0.2/resources/watchlist_resource.py
-drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-05-19 16:53:15.317730 APIConnect-2.0.2/services/
--rw-r--r--   0 saurabh    (502) staff       (20)     9382 2023-05-03 11:18:05.000000 APIConnect-2.0.2/services/live_news_service.py
--rw-r--r--   0 saurabh    (502) staff       (20)     9505 2023-05-03 11:18:05.000000 APIConnect-2.0.2/services/watchlist_service.py
--rw-r--r--   0 saurabh    (502) staff       (20)       38 2023-05-19 16:53:15.320667 APIConnect-2.0.2/setup.cfg
--rw-r--r--   0 saurabh    (502) staff       (20)     1173 2023-05-19 10:55:02.000000 APIConnect-2.0.2/setup.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.762078 APIConnect-2.0.3/
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.721094 APIConnect-2.0.3/APIConnect/
+-rw-r--r--   0 saurabh    (502) staff       (20)    67027 2023-07-28 13:03:00.000000 APIConnect-2.0.3/APIConnect/APIConnect.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     1877 2023-06-06 12:14:39.000000 APIConnect-2.0.3/APIConnect/api_constants.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     3276 2023-07-28 04:33:50.000000 APIConnect-2.0.3/APIConnect/api_utils.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     6501 2023-06-06 12:14:39.000000 APIConnect-2.0.3/APIConnect/http.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     5379 2023-06-06 12:14:39.000000 APIConnect-2.0.3/APIConnect/login_helper.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     3788 2023-06-06 12:14:39.000000 APIConnect-2.0.3/APIConnect/order.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     4696 2023-06-06 12:14:39.000000 APIConnect-2.0.3/APIConnect/validator.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.725479 APIConnect-2.0.3/APIConnect.egg-info/
+-rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-07-28 13:21:20.000000 APIConnect-2.0.3/APIConnect.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh    (502) staff       (20)     1146 2023-07-28 13:21:20.000000 APIConnect-2.0.3/APIConnect.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)        1 2023-07-28 13:21:20.000000 APIConnect-2.0.3/APIConnect.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)       33 2023-07-28 13:21:20.000000 APIConnect-2.0.3/APIConnect.egg-info/requires.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)       56 2023-07-28 13:21:20.000000 APIConnect-2.0.3/APIConnect.egg-info/top_level.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)     1140 2023-06-06 12:14:39.000000 APIConnect-2.0.3/LICENSE.txt
+-rw-r--r--   0 saurabh    (502) staff       (20)      833 2023-07-28 13:21:20.761551 APIConnect-2.0.3/PKG-INFO
+-rw-r--r--   0 saurabh    (502) staff       (20)       40 2023-06-06 12:14:39.000000 APIConnect-2.0.3/README
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.726302 APIConnect-2.0.3/conf/
+-rw-r--r--   0 saurabh    (502) staff       (20)      354 2023-07-28 04:40:09.000000 APIConnect-2.0.3/conf/settings.ini
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.744639 APIConnect-2.0.3/constants/
+-rw-r--r--   0 saurabh    (502) staff       (20)      173 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/action.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      363 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/asset_type.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      278 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/chart_exchange.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      624 2023-07-28 04:37:30.000000 APIConnect-2.0.3/constants/constants.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      222 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/duration.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      193 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/eod_Interval.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      242 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/exchange.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      247 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/intraday_interval.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      244 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/order_type.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      238 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/product_code.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      236 2023-06-06 12:14:39.000000 APIConnect-2.0.3/constants/results_stocks_news_category.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     8423 2023-07-28 04:33:50.000000 APIConnect-2.0.3/constants/router.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      326 2023-07-28 04:33:50.000000 APIConnect-2.0.3/constants/streaming_constants.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.747039 APIConnect-2.0.3/exceptions/
+-rw-r--r--   0 saurabh    (502) staff       (20)      180 2023-06-06 12:14:39.000000 APIConnect-2.0.3/exceptions/api_exception.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      384 2023-06-06 12:14:39.000000 APIConnect-2.0.3/exceptions/validation_exception.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.753884 APIConnect-2.0.3/feed/
+-rw-r--r--   0 saurabh    (502) staff       (20)     2574 2023-07-28 04:33:50.000000 APIConnect-2.0.3/feed/depth_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     6532 2023-07-28 13:19:20.000000 APIConnect-2.0.3/feed/feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     1577 2023-06-06 12:14:39.000000 APIConnect-2.0.3/feed/livenews_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2159 2023-07-28 04:33:50.000000 APIConnect-2.0.3/feed/miniQuote_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2046 2023-06-06 12:14:39.000000 APIConnect-2.0.3/feed/orders_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2091 2023-06-06 12:14:39.000000 APIConnect-2.0.3/feed/quotes_feed.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     2212 2023-07-28 04:33:50.000000 APIConnect-2.0.3/feed/reduced_quotes_feed.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.757508 APIConnect-2.0.3/resources/
+-rw-r--r--   0 saurabh    (502) staff       (20)     1123 2023-06-06 12:14:39.000000 APIConnect-2.0.3/resources/chart_response_formatter.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     4635 2023-06-06 12:14:39.000000 APIConnect-2.0.3/resources/live_news_resource.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      892 2023-07-28 04:33:50.000000 APIConnect-2.0.3/resources/quote_resource.py
+-rw-r--r--   0 saurabh    (502) staff       (20)      901 2023-06-06 12:14:39.000000 APIConnect-2.0.3/resources/watchlist_resource.py
+drwxr-xr-x   0 saurabh    (502) staff       (20)        0 2023-07-28 13:21:20.760561 APIConnect-2.0.3/services/
+-rw-r--r--   0 saurabh    (502) staff       (20)     9382 2023-06-06 12:14:39.000000 APIConnect-2.0.3/services/live_news_service.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     1225 2023-07-28 04:33:50.000000 APIConnect-2.0.3/services/quote_service.py
+-rw-r--r--   0 saurabh    (502) staff       (20)     9505 2023-06-06 12:14:39.000000 APIConnect-2.0.3/services/watchlist_service.py
+-rw-r--r--   0 saurabh    (502) staff       (20)       38 2023-07-28 13:21:20.762226 APIConnect-2.0.3/setup.cfg
+-rw-r--r--   0 saurabh    (502) staff       (20)     1173 2023-07-28 13:20:14.000000 APIConnect-2.0.3/setup.py
```

### Comparing `APIConnect-2.0.2/APIConnect/APIConnect.py` & `APIConnect-2.0.3/APIConnect/APIConnect.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 from constants.order_type import OrderTypeEnum
 from constants.product_code import ProductCodeENum
 from constants.router import Router
 from feed.feed import Feed
 from feed.livenews_feed import LiveNewsFeed
 from feed.orders_feed import OrdersFeed
 from feed.quotes_feed import QuotesFeed
+from feed.reduced_quotes_feed import ReducedQuotesFeed
+from feed.depth_feed import DepthFeed
+from feed.miniQuote_feed import MiniQuoteFeed
 from resources.chart_response_formatter import ChartResponseFormatter
 from services.live_news_service import LiveNewsService
 from services.watchlist_service import WatchlistService
+from services.quote_service import QuoteService
 
 logging.basicConfig(filename = 'apiconnect.log',
         level=logging.DEBUG,
         format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
 LOGGER = logging.getLogger(__name__)
 
 LOG_LEVELS = {
@@ -80,27 +84,27 @@
                         errno.ENOENT, os.strerror(errno.ENOENT), conf)
             except Exception as ex:
                 LOGGER.exception("Error occurred while parsing provided configuaration file: %s", ex)
                 raise ex
         else:
             LOGGER.info("Logger initiated with default values.")
 
-        self.__version = '2.0.2'
+        self.__version = '2.0.3'
         self.__dc = downloadContract
         self.__filename = "data_" + ApiKey + '.txt'
         self.__router = Router(self.__conf)
         self.__constants = ApiConstants()
         self.__init_proxies = init_proxies
         self.__proxies = self.__init_proxies(self.__conf)
         self.__http = Http(self.__constants, self.__proxies)
         self.__constants.Filename = self.__filename
         self.__constants.ApiKey = ApiKey
         self.__login_helper = LoginHelper(self.__http, self.__router, self.__constants, self.__proxies)
         self.__api_utils = ApiUtils(self.__version, self.__http, self.__router, self.__constants)
-        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjg0NTAwMDU0LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjIiLCJhcHBpZCI6ImM0YTFmYjE1Yjk2Y2E5OGRiOWVkOTVkNmFkZmJlOWM2IiwiaXNzIjoiZW10IiwiZXhwIjoxNjg0NTIxMDAwLCJpYXQiOjE2ODQ1MDAzNTR9.XuH-LuW3STn15EjZNmh31ZqNUsl98r_8aIJfmJ_CapE"
+        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjkwNTQxNjQ3LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjMiLCJhcHBpZCI6IjFmZWZjY2Y2YmQzYzllNjFkMWNlYTFlMDY2ZWJlMDg1IiwiaXNzIjoiZW10IiwiZXhwIjoxNjkwNTY5MDAwLCJpYXQiOjE2OTA1NDE5NDd9.Cl5oqCYl4Yx4fiC_oWSsDzIe-8vgkPqWqYAP5XuLtps"
 
         if conf and self.__conf['GLOBAL'].get('AppIdKey'):
             AppIdKey = self.__conf['GLOBAL'].get('AppIdKey')
         self.__constants.AppIdKey = AppIdKey
 
         if path.exists(self.__filename):
             LOGGER.info("User data file found, loading data.")
@@ -1353,20 +1357,29 @@
         LOGGER.debug(f"getLatestCorporateActions response is : {response}")
         return response
 
     # Streaming methods
 
     def initQuotesStreaming(self) :
         return QuotesFeed(self.__feedObj)
+    
+    def initReducedQuotesStreaming(self) :
+        return ReducedQuotesFeed(self.__feedObj)
 
     def initOrdersStreaming(self, acc_id : str, user_id : str) :
         return OrdersFeed(self.__feedObj, acc_id, user_id)
 
     def initLiveNewsStreaming(self) :
         return LiveNewsFeed(self.__feedObj)
+    
+    def initDepthStreaming(self) :
+        return DepthFeed(self.__feedObj, self.__constants)
+
+    def initMiniQuoteStreaming(self) :
+        return MiniQuoteFeed(self.__feedObj)
 
     # Watchlist methods
 
     def getWatchlistGroups(self):
         LOGGER.info("getWatchlistGroups method is called.")
         service = WatchlistService(self.__router, self.__http, self.__constants)
 
@@ -1464,8 +1477,22 @@
             url = self.__router._LogoutURL().format(userid=self.__constants.eqAccId)
             rep = self.__http._PutMethod(url, {})
 
         if rep != "":
             if path.exists(self.__filename):
                 LOGGER.debug("File with account related details is removed.")
                 os.remove(self.__filename)
-            self.__constants.Data = ""
+            self.__constants.Data = ""
+
+    #Quote methods
+
+    @Validator.isRequired(['Streaming_Symbol'])
+    @Validator.ValidateInputDataTypes
+    def GetMarketDepth(self, Streaming_Symbol : str):
+        LOGGER.info("getMarketDepth method is called.")
+        service = QuoteService(self.__router, self.__http)
+
+        response = service._getMarketDepth(Streaming_Symbol)
+
+        LOGGER.debug(f'getMarketDepth response is : {response}')
+        return response
+
```

### Comparing `APIConnect-2.0.2/APIConnect/api_constants.py` & `APIConnect-2.0.3/APIConnect/api_constants.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/APIConnect/api_utils.py` & `APIConnect-2.0.3/APIConnect/api_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,22 @@
         self.LOGGER.info("Checking for new update.")
         url = self.__router._CheckUpdateURl()
         rep = self.__http._PostMethod(url, json.dumps({"lib": "EAC_PYTHON", "vsn": self.__version}))
         self.LOGGER.debug("Response received: %s", rep)
         if not rep:
             return
         elif rep['data']['sts'] is True:
+            if rep['data']['msg'] == 'OPTIONAL':
+                self.LOGGER.info("New optional update found.")
+                print("New version " + rep['data']['vsn'] + " is available. Stay up to date for better experience")
+        elif rep['data']['sts'] is False:
             if rep['data']['msg'] == 'MANDATORY':
                 print("Mandatory Update. New version " + rep['data']['vsn'] + '. Update to new version to continue.')
                 self.LOGGER.info("Mandatory Update. New version " + rep['data']['vsn'] + '. Update to new version to continue.')
                 sys.exit(0)
-            if rep['data']['msg'] == 'OPTIONAL':
-                self.LOGGER.info("New optional update found.")
-                print("New version " + rep['data']['vsn'] + " is available. Stay up to date for better experience")
 
     def _setProductCodes(self) :
         self.__constants.ProductCodesMap : dict = self.__FetchProductCodes()
 
     def __FetchProductCodes(self) -> dict:
         exch_wise_product_codes = dict()
         with open(self.__constants.Filename, 'r') as session_file :
```

### Comparing `APIConnect-2.0.2/APIConnect/http.py` & `APIConnect-2.0.3/APIConnect/http.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/APIConnect/login_helper.py` & `APIConnect-2.0.3/APIConnect/login_helper.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/APIConnect/order.py` & `APIConnect-2.0.3/APIConnect/order.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/APIConnect/validator.py` & `APIConnect-2.0.3/APIConnect/validator.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/APIConnect.egg-info/PKG-INFO` & `APIConnect-2.0.3/APIConnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: APIConnect
-Version: 2.0.2
+Version: 2.0.3
 Summary: APIs to trade from Nuvama
 Home-page: https://nuvamawealth.com/
-Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz
+Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.3.tar.gz
 Author: Nuvama
 Author-email: support@nuvama.com
 License: MIT
 Keywords: Nuvama,Open API,Trade,Nuvama Python Library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `APIConnect-2.0.2/APIConnect.egg-info/SOURCES.txt` & `APIConnect-2.0.3/APIConnect.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -25,16 +25,21 @@
 constants/order_type.py
 constants/product_code.py
 constants/results_stocks_news_category.py
 constants/router.py
 constants/streaming_constants.py
 exceptions/api_exception.py
 exceptions/validation_exception.py
+feed/depth_feed.py
 feed/feed.py
 feed/livenews_feed.py
+feed/miniQuote_feed.py
 feed/orders_feed.py
 feed/quotes_feed.py
+feed/reduced_quotes_feed.py
 resources/chart_response_formatter.py
 resources/live_news_resource.py
+resources/quote_resource.py
 resources/watchlist_resource.py
 services/live_news_service.py
+services/quote_service.py
 services/watchlist_service.py
```

### Comparing `APIConnect-2.0.2/LICENSE.txt` & `APIConnect-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/PKG-INFO` & `APIConnect-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: APIConnect
-Version: 2.0.2
+Version: 2.0.3
 Summary: APIs to trade from Nuvama
 Home-page: https://nuvamawealth.com/
-Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz
+Download-URL: https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.3.tar.gz
 Author: Nuvama
 Author-email: support@nuvama.com
 License: MIT
 Keywords: Nuvama,Open API,Trade,Nuvama Python Library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `APIConnect-2.0.2/constants/constants.py` & `APIConnect-2.0.3/constants/constants.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/constants/router.py` & `APIConnect-2.0.3/constants/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,8 +199,14 @@
     def _LoginURL(self):
         return urllib.parse.urljoin(self.baseurllogin, "accounts/loginvendor/{vendorId}/")
 
     def _TokenURL(self):
         return urllib.parse.urljoin(self.baseurllogin, "accounts/logindata/")
 
     def _LogoutURL(self):
-        return urllib.parse.urljoin(self.baseurllogin, "account/logoff/{userid}/")
+        return urllib.parse.urljoin(self.baseurllogin, "account/logoff/{userid}/")
+
+    #SnapQuote related APIs
+
+    def _MarketDepthURL(self):
+        return urllib.parse.urljoin(self.baseurlcontent, "quote/scrip/{symbol}/")
+
```

### Comparing `APIConnect-2.0.2/feed/feed.py` & `APIConnect-2.0.3/feed/feed.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 LOGGER = logging.getLogger(__name__)
 
 class Feed:
 
     def __init__(self, confObj):
         self.__conf = confObj
 
-        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjg0NTAwMDU0LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjIiLCJhcHBpZCI6ImM0YTFmYjE1Yjk2Y2E5OGRiOWVkOTVkNmFkZmJlOWM2IiwiaXNzIjoiZW10IiwiZXhwIjoxNjg0NTIxMDAwLCJpYXQiOjE2ODQ1MDAzNTR9.XuH-LuW3STn15EjZNmh31ZqNUsl98r_8aIJfmJ_CapE"
+        AppIdKey = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHAiOjAsImZmIjoiVyIsImJkIjoid2ViLXBjIiwibmJmIjoxNjkwNTQxNjQ3LCJzcmMiOiJlbXRtdyIsImF2IjoiMi4wLjMiLCJhcHBpZCI6IjFmZWZjY2Y2YmQzYzllNjFkMWNlYTFlMDY2ZWJlMDg1IiwiaXNzIjoiZW10IiwiZXhwIjoxNjkwNTY5MDAwLCJpYXQiOjE2OTA1NDE5NDd9.Cl5oqCYl4Yx4fiC_oWSsDzIe-8vgkPqWqYAP5XuLtps"
         Host="ncst.nuvamawealth.com"
         Port=9443
 
         self._appID = AppIdKey
         self.__host = Host
         self.__port = Port
 
@@ -78,19 +78,24 @@
             if resp:
                 LOGGER.debug(f"Response recevied : {resp}")
                 try:
                     resp_dict = json.loads(resp)
 
                     if resp_dict['response']["streaming_type"] == "quote3":
                         callback = self.__requestsList[StreamingConstants.QUOTE_SREAM_REQ_CODE]['callback']
+                    if resp_dict['response']["streaming_type"] == "quote":
+                        callback = self.__requestsList[StreamingConstants.REDUCED_QUOTE_SREAM_REQ_CODE]['callback']
                     elif resp_dict['response']["streaming_type"] == "orderFiler":
                         callback = self.__requestsList[StreamingConstants.ORDER_STREAM_REQ_CODE]['callback']
                     elif resp_dict['response']["streaming_type"] == "news":
                         callback = self.__requestsList[StreamingConstants.LIVENEWS_STREAM_REQ_CODE]['callback']
-
+                    elif resp_dict['response']["streaming_type"] == "quote2":
+                        callback = self.__requestsList[StreamingConstants.DEPTH_STREAM_REQ_CODE]['callback']
+                    elif resp_dict['response']["streaming_type"] == "miniquote":
+                        callback = self.__requestsList[StreamingConstants.MINI_QUOTE_STREAM_REQ_CODE]['callback']
                     callback(resp)
 
                 except json.JSONDecodeError:
                     pass
 
             else:
                 LOGGER.error("Response Blank. Socket Connection seems to be closed. Trying to reconnect...")
@@ -115,15 +120,14 @@
         except OSError:
             self.__retry_connection()
 
     def __create_connection(self):
         # New code TCP
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self._sock.settimeout(100)
-
         self._sock.connect((self.__host, self.__port)) # raises OSError
         self._sock.setblocking(True)
 
         self._socket_fs = self._sock.makefile('rw')
         LOGGER.info("Connection established with subscriber.")
 
     def __retry_connection(self):
```

### Comparing `APIConnect-2.0.2/feed/livenews_feed.py` & `APIConnect-2.0.3/feed/livenews_feed.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/feed/orders_feed.py` & `APIConnect-2.0.3/feed/orders_feed.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/feed/quotes_feed.py` & `APIConnect-2.0.3/feed/quotes_feed.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/resources/chart_response_formatter.py` & `APIConnect-2.0.3/resources/chart_response_formatter.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/resources/live_news_resource.py` & `APIConnect-2.0.3/resources/live_news_resource.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/resources/watchlist_resource.py` & `APIConnect-2.0.3/resources/watchlist_resource.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/services/live_news_service.py` & `APIConnect-2.0.3/services/live_news_service.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/services/watchlist_service.py` & `APIConnect-2.0.3/services/watchlist_service.py`

 * *Files identical despite different names*

### Comparing `APIConnect-2.0.2/setup.py` & `APIConnect-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='APIConnect',
     packages=['APIConnect', 'constants', 'exceptions', 'resources', 'services', 'feed'],
-    version='2.0.2',
+    version='2.0.3',
     license='MIT',
     description='APIs to trade from Nuvama',
     author='Nuvama',
     author_email='support@nuvama.com',
     url='https://nuvamawealth.com/',
-    download_url='https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.2.tar.gz',
+    download_url='https://www.nuvamawealth.com/ewwebimages/webfiles/download/Python_APIConnect/APIConnect-2.0.3.tar.gz',
     keywords=['Nuvama', 'Open API', 'Trade', 'Nuvama Python Library'],
     python_requires=">=3.7",
     install_requires=[
         'urllib3>=1.26.6',
         'requests>=2.26.0'
         ],
     data_files=[('conf',['conf/settings.ini'])],
```

