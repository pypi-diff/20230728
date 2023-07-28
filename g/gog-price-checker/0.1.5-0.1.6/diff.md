# Comparing `tmp/gog_price_checker-0.1.5.tar.gz` & `tmp/gog_price_checker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.5.tar", last modified: Fri Jul 28 15:24:14 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.6.tar", last modified: Fri Jul 28 15:32:58 2023, max compression
```

## Comparing `gog_price_checker-0.1.5.tar` & `gog_price_checker-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/gog_price_checker/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/gog_price_checker/countries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/gog_price_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 15:24:14.000000 gog_price_checker-0.1.5/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:24:14.209272 gog_price_checker-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 15:23:59.000000 gog_price_checker-0.1.5/setup.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.740218 gog_price_checker-0.1.6/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:32:58.740061 gog_price_checker-0.1.6/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3286 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/README.md
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.738902 gog_price_checker-0.1.6/gog_price_checker/
+-rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/gog_price_checker/__init__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3227 2023-07-28 15:30:50.000000 gog_price_checker-0.1.6/gog_price_checker/__main__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 15:15:44.000000 gog_price_checker-0.1.6/gog_price_checker/countries.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 15:32:58.739813 gog_price_checker-0.1.6/gog_price_checker.egg-info/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3732 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 15:32:58.000000 gog_price_checker-0.1.6/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 15:32:58.740279 gog_price_checker-0.1.6/setup.cfg
+-rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 15:32:25.000000 gog_price_checker-0.1.6/setup.py
```

### Comparing `gog_price_checker-0.1.5/PKG-INFO` & `gog_price_checker-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
@@ -81,7 +83,9 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
+
+
```

### Comparing `gog_price_checker-0.1.5/README.md` & `gog_price_checker-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.5/gog_price_checker/__main__.py` & `gog_price_checker-0.1.6/gog_price_checker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     else:
         for i, price in enumerate(sorted_prices):
             if i == count:
                 break
             print(f"{price[0]}: {price[1][0]} {price[1][1]}")
 
 
-def main(args):
+def main():
+    args = init_parser().parse_args()
     if "gogdb.org" in args.url:
         product_id = args.url.split("/")[-1]
     else:
         product_id = extract_product_id(args.url)
     request_prices(product_id, args.normalize)
     sort_prices()
     out_result(args.count, args.pretty)
@@ -93,9 +94,8 @@
     parser.add_argument("-n", "--normalize", action="store_true", help="normalize currencies to USD")
     parser.add_argument("-c", "--count", type=int, default=10, help="number of countries to show")
     parser.add_argument("-p", "--pretty", action="store_true", help="shows result as pretty table")
     return parser
 
 
 if __name__ == "__main__":
-    arguments = init_parser().parse_args()
-    main(arguments)
+    main()
```

### Comparing `gog_price_checker-0.1.5/gog_price_checker/countries.py` & `gog_price_checker-0.1.6/gog_price_checker/countries.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.5/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.6/gog_price_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Game Price Checker 💵
 [![PyPI](https://img.shields.io/pypi/v/gog-price-checker)](https://pypi.org/project/gog-price-checker/)
@@ -81,7 +83,9 @@
 ## License
 
 - The **Game Price Checker** Python script is released under the [MIT License](LICENSE). Feel free to modify and distribute the script according to the terms of the license.
 
 ## Disclaimer
 
 - The author of this script is not responsible for any misuse or consequences of using the script on unauthorized websites. Always make sure you have the right to access and use the data from the websites you interact with.
+
+
```

### Comparing `gog_price_checker-0.1.5/setup.py` & `gog_price_checker-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.5",
+    version="0.1.6",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

