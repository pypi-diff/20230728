# Comparing `tmp/pythclient-0.1.8.tar.gz` & `tmp/pythclient-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythclient-0.1.8.tar", last modified: Tue Jun 27 08:20:45 2023, max compression
+gzip compressed data, was "pythclient-0.1.9.tar", last modified: Fri Jul 28 02:43:39 2023, max compression
```

## Comparing `pythclient-0.1.8.tar` & `pythclient-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.933852 pythclient-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-27 08:20:27.000000 pythclient-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-27 08:20:45.933852 pythclient-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-27 08:20:27.000000 pythclient-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 08:20:27.000000 pythclient-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.929852 pythclient-0.1.8/pythclient/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/pythaccounts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/pythclient.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-27 08:20:27.000000 pythclient-0.1.8/pythclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.929852 pythclient-0.1.8/pythclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-27 08:20:45.000000 pythclient-0.1.8/pythclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 08:20:45.933852 pythclient-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-27 08:20:27.000000 pythclient-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 08:20:45.933852 pythclient-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8432 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_mapping_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_account_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_price_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_product_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_pyth_account.py
--rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_pyth_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_solana_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-27 08:20:27.000000 pythclient-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 02:43:39.679928 pythclient-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-07-28 02:43:19.000000 pythclient-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-07-28 02:43:39.679928 pythclient-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-07-28 02:43:19.000000 pythclient-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-28 02:43:19.000000 pythclient-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 02:43:39.675928 pythclient-0.1.9/pythclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/pythaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/pythclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-07-28 02:43:19.000000 pythclient-0.1.9/pythclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 02:43:39.679928 pythclient-0.1.9/pythclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-07-28 02:43:39.000000 pythclient-0.1.9/pythclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-28 02:43:39.000000 pythclient-0.1.9/pythclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 02:43:39.000000 pythclient-0.1.9/pythclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-28 02:43:39.000000 pythclient-0.1.9/pythclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-28 02:43:39.000000 pythclient-0.1.9/pythclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 02:43:39.679928 pythclient-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-07-28 02:43:19.000000 pythclient-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 02:43:39.679928 pythclient-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8545 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_mapping_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_price_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_price_account_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_price_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_price_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_product_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_pyth_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_pyth_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_solana_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-28 02:43:19.000000 pythclient-0.1.9/tests/test_utils.py
```

### Comparing `pythclient-0.1.8/LICENSE` & `pythclient-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/PKG-INFO` & `pythclient-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.8/README.md` & `pythclient-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/calendar.py` & `pythclient-0.1.9/pythclient/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         return True
 
     # all other markets (crypto)
     return True
 
 
-def get_next_market_open(asset_type: str, dt: datetime.datetime) -> str:
+def get_next_market_open(asset_type: str, dt: datetime.datetime) -> int:
     # make sure time is in NY timezone
     dt = dt.astimezone(NY_TZ)
     time = dt.time()
 
     if asset_type == "equity":
         if time < EQUITY_OPEN:
             next_market_open = dt.replace(
@@ -115,18 +115,18 @@
 
     else:
         return None
 
     while not is_market_open(asset_type, next_market_open):
         next_market_open += datetime.timedelta(days=1)
 
-    return next_market_open.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
+    return int(next_market_open.timestamp())
 
 
-def get_next_market_close(asset_type: str, dt: datetime.datetime) -> str:
+def get_next_market_close(asset_type: str, dt: datetime.datetime) -> int:
     # make sure time is in NY timezone
     dt = dt.astimezone(NY_TZ)
     time = dt.time()
 
     if asset_type == "equity":
         if dt.date() in EQUITY_EARLY_HOLIDAYS:
             if time < EQUITY_EARLY_CLOSE:
@@ -144,24 +144,20 @@
                     microsecond=0,
                 )
                 next_market_close += datetime.timedelta(days=1)
         elif dt.date() in EQUITY_HOLIDAYS:
             next_market_open = get_next_market_open(
                 asset_type, dt + datetime.timedelta(days=1)
             )
-            next_market_close = (
-                datetime.datetime.fromisoformat(next_market_open.replace("Z", "+00:00"))
-                .astimezone(NY_TZ)
-                .replace(
+            next_market_close = datetime.datetime.fromtimestamp(next_market_open).astimezone(NY_TZ).replace(
                     hour=EQUITY_CLOSE.hour,
                     minute=EQUITY_CLOSE.minute,
                     second=0,
                     microsecond=0,
                 )
-            )
         else:
             next_market_close = dt.replace(
                 hour=EQUITY_CLOSE.hour,
                 minute=EQUITY_CLOSE.minute,
                 second=0,
                 microsecond=0,
             )
@@ -185,8 +181,8 @@
         while not is_market_open(asset_type, next_market_close):
             next_market_close += datetime.timedelta(days=1)
         while is_market_open(asset_type, next_market_close):
             next_market_close += datetime.timedelta(days=1)
     else:  # crypto markets never close
         return None
 
-    return next_market_close.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
+    return int(next_market_close.timestamp())
```

### Comparing `pythclient-0.1.8/pythclient/exceptions.py` & `pythclient-0.1.9/pythclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/pythaccounts.py` & `pythclient-0.1.9/pythclient/pythaccounts.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/pythclient.py` & `pythclient-0.1.9/pythclient/pythclient.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/ratelimit.py` & `pythclient-0.1.9/pythclient/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/solana.py` & `pythclient-0.1.9/pythclient/solana.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient/utils.py` & `pythclient-0.1.9/pythclient/utils.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/pythclient.egg-info/PKG-INFO` & `pythclient-0.1.9/pythclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pythclient-0.1.8/pythclient.egg-info/SOURCES.txt` & `pythclient-0.1.9/pythclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/setup.py` & `pythclient-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiodns', 'aiohttp>=3.7.4', 'backoff', 'base58', 'dnspython', 'flake8', 'loguru', 'typing-extensions', 'pytz']
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pythclient',
-    version='0.1.8',
+    version='0.1.9',
     packages=['pythclient'],
     author='Pyth Developers',
     author_email='contact@pyth.network',
     description='A library to retrieve Pyth account structures off the Solana blockchain.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pyth-network/pyth-client-py',
```

### Comparing `pythclient-0.1.8/tests/test_calendar.py` & `pythclient-0.1.9/tests/test_calendar.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,20 @@
 FX_METAL_CLOSE_SUN_2023_6_18_16 = datetime.datetime(2023, 6, 18, 16, 0, 0, tzinfo=NY_TZ)
 FX_METAL_HOLIDAY_SUN_2023_1_1 = datetime.datetime(2023, 1, 1, tzinfo=NY_TZ)
 
 # Define constants for cryptocurrency market
 CRYPTO_OPEN_WED_2023_6_21_12 = datetime.datetime(2023, 6, 21, 12, 0, 0, tzinfo=NY_TZ)
 CRYPTO_OPEN_SUN_2023_6_18_12 = datetime.datetime(2023, 6, 18, 12, 0, 0, tzinfo=NY_TZ)
 
-def format_datetime_to_utc_iso_string(dt: datetime.datetime):
-    return dt.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
+
+def format_datetime_to_unix_timestamp(dt: datetime.datetime):
+    # Convert the datetime object to a Unix timestamp in UTC
+    timestamp = dt.astimezone(UTC_TZ).timestamp()
+    unix_timestamp_utc = int(timestamp)
+    return unix_timestamp_utc
 
 def test_is_market_open():
     # equity
     # weekday, within equity market hours
     assert is_market_open("equity", EQUITY_OPEN_WED_2023_6_21_12) == True
 
     # weekday, out of equity market hours
@@ -63,141 +67,141 @@
     assert is_market_open("crypto", CRYPTO_OPEN_SUN_2023_6_18_12) == True
 
 
 def test_get_next_market_open():
     # equity within market hours
     assert (
         get_next_market_open("equity", EQUITY_OPEN_WED_2023_6_21_12)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 22, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 22, 9, 30, 0, tzinfo=NY_TZ))
     )
 
     # equity out of market hours
     assert (
         get_next_market_open("equity", EQUITY_CLOSE_WED_2023_6_21_17)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 22, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 22, 9, 30, 0, tzinfo=NY_TZ))
     )
 
     # equity weekend
     assert (
         get_next_market_open("equity", EQUITY_CLOSE_SAT_2023_6_10_17)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 12, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 12, 9, 30, 0, tzinfo=NY_TZ))
     )
 
     # equity holiday
     assert (
         get_next_market_open("equity", EQUITY_HOLIDAY_MON_2023_6_19)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 20, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 20, 9, 30, 0, tzinfo=NY_TZ))
     )
 
     # equity early close holiday
     assert (
         get_next_market_open("equity", EQUITY_EARLY_CLOSE_OPEN_FRI_2023_11_24_14)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 11, 27, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 11, 27, 9, 30, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_open("equity", EQUITY_EARLY_CLOSE_CLOSE_FRI_2023_11_24_14)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 11, 27, 9, 30, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 11, 27, 9, 30, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal within market hours
     assert (
         get_next_market_open("fx", FX_METAL_OPEN_WED_2023_6_21_22)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 25, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 25, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_open("metal", FX_METAL_OPEN_WED_2023_6_21_22)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 25, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 25, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal out of market hours
     assert (
         get_next_market_open("fx", FX_METAL_CLOSE_SUN_2023_6_18_16)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 18, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 18, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_open("metal", FX_METAL_CLOSE_SUN_2023_6_18_16)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 18, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 18, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal holiday
     assert (
         get_next_market_open("fx", FX_METAL_HOLIDAY_SUN_2023_1_1)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 1, 2, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 1, 2, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_open("metal", FX_METAL_HOLIDAY_SUN_2023_1_1)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 1, 2, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 1, 2, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # crypto
     assert get_next_market_open("crypto", CRYPTO_OPEN_WED_2023_6_21_12) == None
     assert get_next_market_open("crypto", CRYPTO_OPEN_SUN_2023_6_18_12) == None
 
 
 def test_get_next_market_close():
     # equity within market hours
     assert (
         get_next_market_close("equity", EQUITY_OPEN_WED_2023_6_21_12)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 21, 16, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 21, 16, 0, 0, tzinfo=NY_TZ))
     )
 
     # equity out of market hours
     assert (
         get_next_market_close("equity", EQUITY_CLOSE_WED_2023_6_21_17)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 22, 16, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 22, 16, 0, 0, tzinfo=NY_TZ))
     )
 
     # equity weekend
     assert (
         get_next_market_close("equity", EQUITY_CLOSE_SAT_2023_6_10_17)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 12, 16, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 12, 16, 0, 0, tzinfo=NY_TZ))
     )
 
     # equity holiday
     assert (
         get_next_market_close("equity", EQUITY_HOLIDAY_MON_2023_6_19)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 20, 16, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 20, 16, 0, 0, tzinfo=NY_TZ))
     )
 
     # equity early close holiday
     assert (
         get_next_market_close("equity", EQUITY_EARLY_CLOSE_OPEN_FRI_2023_11_24_14)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 11, 24, 13, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 11, 24, 13, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_close("equity", EQUITY_EARLY_CLOSE_CLOSE_FRI_2023_11_24_14)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 11, 27, 16, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 11, 27, 16, 0, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal within market hours
     assert (
         get_next_market_close("fx", FX_METAL_OPEN_WED_2023_6_21_22)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_close("metal", FX_METAL_OPEN_WED_2023_6_21_22)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal out of market hours
     assert (
         get_next_market_close("fx", FX_METAL_CLOSE_SUN_2023_6_18_16)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_close("metal", FX_METAL_CLOSE_SUN_2023_6_18_16)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 6, 23, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # fx & metal holiday
     assert (
         get_next_market_close("fx", FX_METAL_HOLIDAY_SUN_2023_1_1)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 1, 6, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 1, 6, 17, 0, 0, tzinfo=NY_TZ))
     )
     assert (
         get_next_market_close("metal", FX_METAL_HOLIDAY_SUN_2023_1_1)
-        == format_datetime_to_utc_iso_string(datetime.datetime(2023, 1, 6, 17, 0, 0, tzinfo=NY_TZ))
+        == format_datetime_to_unix_timestamp(datetime.datetime(2023, 1, 6, 17, 0, 0, tzinfo=NY_TZ))
     )
 
     # crypto
     assert get_next_market_close("crypto", CRYPTO_OPEN_WED_2023_6_21_12) == None
     assert get_next_market_close("crypto", CRYPTO_OPEN_SUN_2023_6_18_12) == None
```

### Comparing `pythclient-0.1.8/tests/test_mapping_account.py` & `pythclient-0.1.9/tests/test_mapping_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_price_account.py` & `pythclient-0.1.9/tests/test_price_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_price_account_header.py` & `pythclient-0.1.9/tests/test_price_account_header.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_price_component.py` & `pythclient-0.1.9/tests/test_price_component.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_price_info.py` & `pythclient-0.1.9/tests/test_price_info.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_product_account.py` & `pythclient-0.1.9/tests/test_product_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_pyth_account.py` & `pythclient-0.1.9/tests/test_pyth_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_pyth_client.py` & `pythclient-0.1.9/tests/test_pyth_client.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_solana_account.py` & `pythclient-0.1.9/tests/test_solana_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.8/tests/test_utils.py` & `pythclient-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

