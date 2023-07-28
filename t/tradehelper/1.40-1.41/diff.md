# Comparing `tmp/tradehelper-1.40.tar.gz` & `tmp/tradehelper-1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradehelper-1.40.tar", last modified: Thu Jun  2 06:40:24 2022, max compression
+gzip compressed data, was "tradehelper-1.41.tar", last modified: Fri Jul 28 03:07:02 2023, max compression
```

## Comparing `tradehelper-1.40.tar` & `tradehelper-1.41.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2022-06-02 06:40:24.790476 tradehelper-1.40/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      240 2022-06-02 06:40:24.790476 tradehelper-1.40/PKG-INFO
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       38 2022-06-02 06:40:24.790476 tradehelper-1.40/setup.cfg
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      365 2022-06-02 06:39:29.000000 tradehelper-1.40/setup.py
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2022-06-02 06:40:24.790476 tradehelper-1.40/tradehelper/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      149 2022-06-02 06:39:05.000000 tradehelper-1.40/tradehelper/__init__.py
--rw-rw-r--   0 aarav     (1000) aarav     (1000)    19283 2022-06-02 06:36:56.000000 tradehelper-1.40/tradehelper/tradehelp.py
-drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2022-06-02 06:40:24.790476 tradehelper-1.40/tradehelper.egg-info/
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      240 2022-06-02 06:40:24.000000 tradehelper-1.40/tradehelper.egg-info/PKG-INFO
--rw-rw-r--   0 aarav     (1000) aarav     (1000)      231 2022-06-02 06:40:24.000000 tradehelper-1.40/tradehelper.egg-info/SOURCES.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)        1 2022-06-02 06:40:24.000000 tradehelper-1.40/tradehelper.egg-info/dependency_links.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       31 2022-06-02 06:40:24.000000 tradehelper-1.40/tradehelper.egg-info/requires.txt
--rw-rw-r--   0 aarav     (1000) aarav     (1000)       12 2022-06-02 06:40:24.000000 tradehelper-1.40/tradehelper.egg-info/top_level.txt
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-07-28 03:07:02.666106 tradehelper-1.41/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-07-28 03:07:02.666106 tradehelper-1.41/PKG-INFO
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       38 2023-07-28 03:07:02.666106 tradehelper-1.41/setup.cfg
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      366 2023-07-28 03:04:49.000000 tradehelper-1.41/setup.py
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-07-28 03:07:02.666106 tradehelper-1.41/tradehelper/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      149 2022-06-02 06:39:05.000000 tradehelper-1.41/tradehelper/__init__.py
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)    19321 2023-07-28 02:04:28.000000 tradehelper-1.41/tradehelper/tradehelp.py
+drwxrwxr-x   0 aarav     (1000) aarav     (1000)        0 2023-07-28 03:07:02.666106 tradehelper-1.41/tradehelper.egg-info/
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      196 2023-07-28 03:07:02.000000 tradehelper-1.41/tradehelper.egg-info/PKG-INFO
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)      231 2023-07-28 03:07:02.000000 tradehelper-1.41/tradehelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)        1 2023-07-28 03:07:02.000000 tradehelper-1.41/tradehelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       31 2023-07-28 03:07:02.000000 tradehelper-1.41/tradehelper.egg-info/requires.txt
+-rw-rw-r--   0 aarav     (1000) aarav     (1000)       12 2023-07-28 03:07:02.000000 tradehelper-1.41/tradehelper.egg-info/top_level.txt
```

### Comparing `tradehelper-1.40/tradehelper/tradehelp.py` & `tradehelper-1.41/tradehelper/tradehelp.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,28 +134,28 @@
             if 'strategy_name' in args:
                 if 'daily_execution_id' in args:
                     data = {
                         'strategy_name': args["strategy_name"],
                         'symbol': instrument.symbol,
                         'entry_date': entry_time,
                         'order_id': order_id,
-                        'qty': args["quantity"] * 25,
+                        'qty': args["quantity"] ,
                         'option_type': instrument.option_type,
                         'entry_price': ltp,
                         'signal': signal,
                         'status': status,
                         'daily_execution_id': args["daily_execution_id"],
                     }
                 else:
                     data = {
                         'strategy_name': args["strategy_name"],
                         'symbol': instrument.symbol,
                         'entry_date': entry_time,
                         'order_id': order_id,
-                        'qty': args["quantity"] * 25,
+                        'qty': args["quantity"] ,
                         'option_type': instrument.option_type,
                         'entry_price': ltp,
                         'signal': signal,
                         'status': status,
                     }
                 response = requests.post(
                     self.base_url+"entry", headers=self.headers, data=data)
@@ -166,15 +166,15 @@
 
     def exit(self, args, execution_id, exit_time, order_id, ltp, remarks, profit, loss, mtm, mtm_high, mtm_low):
         try:
             data = {
                 'execution_id':  execution_id,
                 'exit_date': exit_time,
                 'exit_order_id': order_id,
-                'exit_qty': args["quantity"] * 25,
+                'exit_qty': args["quantity"] ,
                 'exit_price': ltp,
                 'exit_status': 'complete',
                 'remarks': remarks,
                 'profit': profit,
                 'loss': loss,
                 'mtm': mtm,
                 'mtm_high':  mtm_high,
@@ -201,17 +201,18 @@
                         'strategy_name': args["strategy_name"],
                         'type': execution_type,
                         'trading_day' : self.trading_day,
                         'api_key': args["api_key"]
                     }
                 else:
                     data = {
-                        'strategy_name': args["strategy_name"],
+                            'strategy_name': args["strategy_name"],
                             'type': execution_type,
                             'trading_day' : self.trading_day,
+                            'args': args
                     }
                 # print(data)
                 response = requests.post(
                     self.base_url+"execution", headers=self.headers, data=data)
                 response_json = (response.json())
                 # print(response_json)
                 return int(response_json['daily_execution_id'])
@@ -262,15 +263,15 @@
         else:
             # ((current_val - previous_val) * coeff) + previous_val where coeff = 2 / (period + 1)
             df[target] = con.ewm(span=period, adjust=False).mean()
 
         df[target].fillna(0, inplace=True)
         return df
 
-    def ATR(df, period, ohlc=['open', 'high', 'low', 'close']):
+    def ATR(self,df, period, ohlc=['open', 'high', 'low', 'close']):
         """
         Function to compute Average True Range (ATR)
         Args :
             df : Pandas DataFrame which contains ['date', 'open', 'high', 'low', 'close', 'volume'] columns
             period : Integer indicates the period of computation in terms of number of candles
             ohlc: List defining OHLC Column names (default ['Open', 'High', 'low', 'Close'])
         Returns :
```

