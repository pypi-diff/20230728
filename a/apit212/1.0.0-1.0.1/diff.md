# Comparing `tmp/apit212-1.0.0.tar.gz` & `tmp/apit212-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-1.0.0.tar", last modified: Fri Jul 28 09:05:50 2023, max compression
+gzip compressed data, was "apit212-1.0.1.tar", last modified: Fri Jul 28 09:14:42 2023, max compression
```

## Comparing `apit212-1.0.0.tar` & `apit212-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:05:50.869788 apit212-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7148 2023-07-28 09:05:50.862140 apit212-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6381 2023-07-15 00:18:19.000000 apit212-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 09:05:50.798646 apit212-1.0.0/apit212/
--rw-rw-rw-   0        0        0    18710 2023-07-28 09:04:05.000000 apit212-1.0.0/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.0/apit212/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-1.0.0/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.0/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-07-28 09:05:50.862140 apit212-1.0.0/apit212.egg-info/
--rw-rw-rw-   0        0        0     7148 2023-07-28 09:05:50.000000 apit212-1.0.0/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-28 09:05:50.000000 apit212-1.0.0/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:05:50.000000 apit212-1.0.0/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-28 09:05:50.000000 apit212-1.0.0/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 09:05:50.000000 apit212-1.0.0/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-07-28 09:04:43.000000 apit212-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 09:05:50.869788 apit212-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-07-28 09:04:32.000000 apit212-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:42.249976 apit212-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7148 2023-07-28 09:14:42.247461 apit212-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6381 2023-07-15 00:18:19.000000 apit212-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:42.186774 apit212-1.0.1/apit212/
+-rw-rw-rw-   0        0        0    18760 2023-07-28 09:14:02.000000 apit212-1.0.1/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.1/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-1.0.1/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.1/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:14:42.247461 apit212-1.0.1/apit212.egg-info/
+-rw-rw-rw-   0        0        0     7148 2023-07-28 09:14:42.000000 apit212-1.0.1/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:14:42.000000 apit212-1.0.1/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:14:42.000000 apit212-1.0.1/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-28 09:14:42.000000 apit212-1.0.1/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 09:14:42.000000 apit212-1.0.1/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-07-28 09:13:49.000000 apit212-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:14:42.249976 apit212-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-07-28 09:13:59.000000 apit212-1.0.1/setup.py
```

### Comparing `apit212-1.0.0/LICENSE` & `apit212-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-1.0.0/PKG-INFO` & `apit212-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-1.0.0/README.md` & `apit212-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `apit212-1.0.0/apit212/Apit212.py` & `apit212-1.0.1/apit212/Apit212.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,16 @@
         payload = []
 
         for instrument in instruments:
             payload.append(dict({"ticker": instrument, "useAskPrice": "false"}))
 
         r = requests.get(f'{self.url}/charting/v1/watchlist/batch/deviations', headers=self.headers,
                          data=json.dumps([payload]))
+                         
+        return r.json
 
     # GET AUTH VALIDATE
     def auth_validate(self) -> dict:
         """
 
         :return: {'id': '********-****-****-****-************', 'accountId': ********, 'customerId': ********,
         'tradingType': 'CFD', 'customerUuid': '********-****-****-****-************', 'frontend': 'WC4',
```

### Comparing `apit212-1.0.0/apit212/apitconstant.py` & `apit212-1.0.1/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.0/apit212/cfdScrape.py` & `apit212-1.0.1/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.0/apit212.egg-info/PKG-INFO` & `apit212-1.0.1/apit212.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-1.0.0/pyproject.toml` & `apit212-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-1.0.0/setup.py` & `apit212-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

