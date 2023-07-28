# Comparing `tmp/tradingcomdados-1.2.4.tar.gz` & `tmp/tradingcomdados-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.2.4.tar", last modified: Tue Jul 11 15:05:28 2023, max compression
+gzip compressed data, was "tradingcomdados-1.2.5.tar", last modified: Fri Jul 28 18:20:37 2023, max compression
```

## Comparing `tradingcomdados-1.2.4.tar` & `tradingcomdados-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.158914 tradingcomdados-1.2.4/
--rw-rw-rw-   0        0        0     1702 2023-07-11 15:05:28.157914 tradingcomdados-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.4/README.md
--rw-rw-rw-   0        0        0      452 2023-07-11 15:05:14.000000 tradingcomdados-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 15:05:28.159915 tradingcomdados-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.146754 tradingcomdados-1.2.4/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.4/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-07-11 15:01:25.000000 tradingcomdados-1.2.4/tradingcomdados/alternative_data.py
--rw-rw-rw-   0        0        0    11046 2023-07-11 14:55:53.000000 tradingcomdados-1.2.4/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.2.4/tradingcomdados/portfolio.py
--rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.4/tradingcomdados/ta_indicators.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.4/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:05:28.156916 tradingcomdados-1.2.4/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-07-11 15:05:24.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 15:05:24.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 15:05:25.000000 tradingcomdados-1.2.4/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:37.475493 tradingcomdados-1.2.5/
+-rw-rw-rw-   0        0        0     1702 2023-07-28 18:20:37.467488 tradingcomdados-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.5/README.md
+-rw-rw-rw-   0        0        0      452 2023-07-28 18:19:15.000000 tradingcomdados-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:20:37.475493 tradingcomdados-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:37.382644 tradingcomdados-1.2.5/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.5/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-07-11 15:01:25.000000 tradingcomdados-1.2.5/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    14523 2023-07-21 01:16:21.000000 tradingcomdados-1.2.5/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     6915 2023-07-11 00:58:03.000000 tradingcomdados-1.2.5/tradingcomdados/portfolio.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.5/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.5/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:37.467488 tradingcomdados-1.2.5/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-07-28 18:20:35.000000 tradingcomdados-1.2.5/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-28 18:20:35.000000 tradingcomdados-1.2.5/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:20:35.000000 tradingcomdados-1.2.5/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-28 18:20:35.000000 tradingcomdados-1.2.5/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 18:20:35.000000 tradingcomdados-1.2.5/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.2.4/PKG-INFO` & `tradingcomdados-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.4
+Version: 1.2.5
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

### Comparing `tradingcomdados-1.2.4/README.md` & `tradingcomdados-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/setup.py` & `tradingcomdados-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/tradingcomdados/alternative_data.py` & `tradingcomdados-1.2.5/tradingcomdados/alternative_data.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/tradingcomdados/data_provider.py` & `tradingcomdados-1.2.5/tradingcomdados/data_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -92,14 +92,88 @@
 
     except:
         print(
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
 
+def _run_request_indicators(
+    data_type: str,
+    request_type: str,
+    ticker: str,
+    indicator: str,
+    date_begin: str,
+    date_end: str,
+    api_key: str,
+    endpoint: str,
+):
+    try:
+
+        header = {"X-API-Key": api_key}
+
+        def _ckeck_data_type(data_type):
+
+            if data_type == "stock" and request_type == "historical_data_indicator":
+                params = {
+                    "ticker": ticker,
+                    "indicador": indicator,
+                    "dataInicio": date_begin,
+                    "dataFim": date_end,
+                }
+
+            return params
+
+        params = _ckeck_data_type(data_type)
+        res = req.get(endpoint, headers=header, params=params).json()
+
+        return res
+
+    except:
+        print(
+            "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
+        )
+
+
+def _run_request_accounting(
+    data_type: str,
+    request_type: str,
+    ticker: str,
+    item: str,
+    date_begin: str,
+    date_end: str,
+    api_key: str,
+    endpoint: str,
+):
+    try:
+
+        header = {"X-API-Key": api_key}
+
+        def _ckeck_data_type(data_type):
+
+            if data_type == "stock" and request_type == "historical_data_accounting":
+                params = {
+                    "ticker": ticker,
+                    "item": item,
+                    "dataInicio": date_begin,
+                    "dataFim": date_end,
+                }
+
+            return params
+
+        params = _ckeck_data_type(data_type)
+        res = req.get(endpoint, headers=header, params=params).json()
+
+        return res
+
+    except:
+        print(
+            "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
+        )
+
+
 def _request_type_validation(data_type, request_type, ticker):
 
     try:
         url_base = "https://api.fintz.com.br"
 
         if data_type == "stock":
 
@@ -119,14 +193,20 @@
 
                 elif request_type == "historical_data_dre":
                     endpoint = url_base + "/bolsa/b3/demonstracoes/dre"
 
                 elif request_type == "historical_data_dfc":
                     endpoint = url_base + "/bolsa/b3/demonstracoes/dfc"
 
+                elif request_type == "historical_data_indicator":
+                    endpoint = url_base + "/bolsa/b3/tm/indicadores"
+
+                elif request_type == "historical_data_accounting":
+                    endpoint = url_base + "/bolsa/b3/tm/demonstracoes"
+
                 return endpoint
 
             endpoint = _check_request_type_stock(request_type)
 
         elif data_type == "treasury":
 
             def _check_request_type_treasury(request_type, ticker):
@@ -173,15 +253,18 @@
         return print(
             "Input request_type option not found, take a look at the documentation."
         )
 
 
 def _transform_to_dataframe(res, request_type):
     try:
-        if request_type != "treasury_historical":
+        if request_type == "historical_data_indicator":
+            df = pd.DataFrame.from_dict(res)
+
+        elif request_type != "treasury_historical":
             df = pd.json_normalize(res)
 
         else:
             df = pd.DataFrame.from_dict(res["dados"])
 
         return df
 
@@ -353,7 +436,62 @@
     for i in tickers:
         temp = get_data_report(
             data_type, request_type, i, date_begin, trimester, api_key
         )
         df = pd.concat([df, temp], ignore_index=True)
 
     return df
+
+
+def get_data_indicator(
+    data_type: str,
+    request_type: str,
+    ticker: str,
+    indicator: str,
+    date_begin: str,
+    date_end: str,
+    api_key: str,
+):
+
+    """
+    Get data from API using standard parameters for the chosen ticker.
+
+    """
+
+    endpoint = _request_type_validation(data_type, request_type, ticker)
+    res = _run_request_indicators(
+        data_type,
+        request_type,
+        ticker,
+        indicator,
+        date_begin,
+        date_end,
+        api_key,
+        endpoint,
+    )
+    df = _transform_to_dataframe(res, request_type)
+
+    return df
+
+
+def get_data_accounting(
+    data_type: str,
+    request_type: str,
+    ticker: str,
+    item: str,
+    date_begin: str,
+    date_end: str,
+    api_key: str,
+):
+
+    """
+    Get data from API using standard parameters for the chosen ticker.
+
+    """
+
+    endpoint = _request_type_validation(data_type, request_type, ticker)
+    res = _run_request_accounting(
+        data_type, request_type, ticker, item, date_begin, date_end, api_key, endpoint
+    )
+    df = _transform_to_dataframe(res, request_type)
+
+    return df
```

### Comparing `tradingcomdados-1.2.4/tradingcomdados/portfolio.py` & `tradingcomdados-1.2.5/tradingcomdados/portfolio.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/tradingcomdados/ta_indicators.py` & `tradingcomdados-1.2.5/tradingcomdados/ta_indicators.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.2.5/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.2.4/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.2.5/tradingcomdados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.2.4
+Version: 1.2.5
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

