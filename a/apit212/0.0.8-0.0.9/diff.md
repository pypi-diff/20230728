# Comparing `tmp/apit212-0.0.8.tar.gz` & `tmp/apit212-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-0.0.8.tar", last modified: Sat Jul 15 00:10:54 2023, max compression
+gzip compressed data, was "apit212-0.0.9.tar", last modified: Fri Jul 28 08:44:44 2023, max compression
```

## Comparing `apit212-0.0.8.tar` & `apit212-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.541528 apit212-0.0.8/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     7148 2023-07-15 00:10:54.539496 apit212-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6381 2023-07-15 00:10:04.000000 apit212-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.424049 apit212-0.0.8/apit212/
--rw-rw-rw-   0        0        0    18278 2023-07-15 00:05:08.000000 apit212-0.0.8/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.8/apit212/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-0.0.8/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-05 19:45:17.000000 apit212-0.0.8/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.533977 apit212-0.0.8/apit212.egg-info/
--rw-rw-rw-   0        0        0     7148 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-07-15 00:05:35.000000 apit212-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 00:10:54.541528 apit212-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-07-15 00:05:45.000000 apit212-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:44.596350 apit212-0.0.9/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     7148 2023-07-28 08:44:44.594337 apit212-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6381 2023-07-15 00:18:19.000000 apit212-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:44.522879 apit212-0.0.9/apit212/
+-rw-rw-rw-   0        0        0    18714 2023-07-28 08:40:45.000000 apit212-0.0.9/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.9/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-0.0.9/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-0.0.9/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:44.589061 apit212-0.0.9/apit212.egg-info/
+-rw-rw-rw-   0        0        0     7148 2023-07-28 08:44:44.000000 apit212-0.0.9/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-28 08:44:44.000000 apit212-0.0.9/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 08:44:44.000000 apit212-0.0.9/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-28 08:44:44.000000 apit212-0.0.9/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 08:44:44.000000 apit212-0.0.9/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-07-28 08:42:23.000000 apit212-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 08:44:44.596350 apit212-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-07-28 08:43:01.000000 apit212-0.0.9/setup.py
```

### Comparing `apit212-0.0.8/LICENSE` & `apit212-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-0.0.8/PKG-INFO` & `apit212-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-0.0.8/README.md` & `apit212-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `apit212-0.0.8/apit212/Apit212.py` & `apit212-0.0.9/apit212/Apit212.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,14 +194,26 @@
             }
 
         self.logger.info(f'finished setup...{username}')
 
     # RETURNS HEADERS AND URL
     def __getitem__(self, key):
         return self.headers
+    
+    def live_price(self, instruments: list):
+        """
+        :param instruments:
+        :return: 
+        """
+        payload = {
+        }
+        for instrument in instruments:
+            payload.update(dict({"ticker": instrument, "useAskPrice": "false"}))
+        r = requests.get(f'{self.url}/charting/v1/watchlist/batch/deviations', headers=self.headers,
+                         data=[json.dumps(payload)])
 
     # GET AUTH VALIDATE
     def auth_validate(self) -> dict:
         """
 
         :return: {'id': '********-****-****-****-************', 'accountId': ********, 'customerId': ********,
         'tradingType': 'CFD', 'customerUuid': '********-****-****-****-************', 'frontend': 'WC4',
```

### Comparing `apit212-0.0.8/apit212/apitconstant.py` & `apit212-0.0.9/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.8/apit212/cfdScrape.py` & `apit212-0.0.9/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.8/apit212.egg-info/PKG-INFO` & `apit212-0.0.9/apit212.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-0.0.8/pyproject.toml` & `apit212-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-0.0.8/setup.py` & `apit212-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

