# Comparing `tmp/gog_price_checker-0.1.2.tar.gz` & `tmp/gog_price_checker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.2.tar", last modified: Fri Jul 28 14:31:59 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.3.tar", last modified: Fri Jul 28 14:35:22 2023, max compression
```

## Comparing `gog_price_checker-0.1.2.tar` & `gog_price_checker-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:31:59.516597 gog_price_checker-0.1.2/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:31:59.516350 gog_price_checker-0.1.2/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)     3119 2023-07-28 13:18:52.000000 gog_price_checker-0.1.2/README.md
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:31:59.515080 gog_price_checker-0.1.2/gog_price_checker/
--rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 14:12:13.000000 gog_price_checker-0.1.2/gog_price_checker/__init__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     3235 2023-07-28 14:31:34.000000 gog_price_checker-0.1.2/gog_price_checker/__main__.py
--rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 14:07:57.000000 gog_price_checker-0.1.2/gog_price_checker/countries.py
-drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:31:59.516098 gog_price_checker-0.1.2/gog_price_checker.egg-info/
--rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:31:59.000000 gog_price_checker-0.1.2/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 14:31:59.000000 gog_price_checker-0.1.2/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 14:31:59.000000 gog_price_checker-0.1.2/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 14:31:59.000000 gog_price_checker-0.1.2/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 14:31:59.000000 gog_price_checker-0.1.2/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 14:31:59.516656 gog_price_checker-0.1.2/setup.cfg
--rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 14:31:56.000000 gog_price_checker-0.1.2/setup.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:35:22.756144 gog_price_checker-0.1.3/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:35:22.755890 gog_price_checker-0.1.3/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3119 2023-07-28 13:18:52.000000 gog_price_checker-0.1.3/README.md
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:35:22.754728 gog_price_checker-0.1.3/gog_price_checker/
+-rw-r--r--   0 alexpopov   (501) staff       (20)       26 2023-07-28 14:12:13.000000 gog_price_checker-0.1.3/gog_price_checker/__init__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3187 2023-07-28 14:34:59.000000 gog_price_checker-0.1.3/gog_price_checker/__main__.py
+-rw-r--r--   0 alexpopov   (501) staff       (20)     1865 2023-07-28 14:07:57.000000 gog_price_checker-0.1.3/gog_price_checker/countries.py
+drwxr-xr-x   0 alexpopov   (501) staff       (20)        0 2023-07-28 14:35:22.755605 gog_price_checker-0.1.3/gog_price_checker.egg-info/
+-rw-r--r--   0 alexpopov   (501) staff       (20)     3565 2023-07-28 14:35:22.000000 gog_price_checker-0.1.3/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 alexpopov   (501) staff       (20)      317 2023-07-28 14:35:22.000000 gog_price_checker-0.1.3/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)        1 2023-07-28 14:35:22.000000 gog_price_checker-0.1.3/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       71 2023-07-28 14:35:22.000000 gog_price_checker-0.1.3/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       18 2023-07-28 14:35:22.000000 gog_price_checker-0.1.3/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 alexpopov   (501) staff       (20)       38 2023-07-28 14:35:22.756212 gog_price_checker-0.1.3/setup.cfg
+-rw-r--r--   0 alexpopov   (501) staff       (20)      785 2023-07-28 14:35:08.000000 gog_price_checker-0.1.3/setup.py
```

### Comparing `gog_price_checker-0.1.2/PKG-INFO` & `gog_price_checker-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gog_price_checker-0.1.2/README.md` & `gog_price_checker-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.2/gog_price_checker/__main__.py` & `gog_price_checker-0.1.3/gog_price_checker/__main__.py`

 * *Files 3% similar despite different names*

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
@@ -90,12 +91,7 @@
 def init_parser():
     parser = ArgumentParser()
     parser.add_argument("-u", "--url", required=True, type=str, help="url to scrape")
     parser.add_argument("-n", "--normalize", action="store_true", help="normalize currencies to USD")
     parser.add_argument("-c", "--count", type=int, default=10, help="number of countries to show")
     parser.add_argument("-p", "--pretty", action="store_true", help="shows result as pretty table")
     return parser
-
-
-if __name__ == "__main__":
-    args = init_parser().parse_args()
-    main(args)
```

### Comparing `gog_price_checker-0.1.2/gog_price_checker/countries.py` & `gog_price_checker-0.1.3/gog_price_checker/countries.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.2/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.3/gog_price_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gog_price_checker-0.1.2/setup.py` & `gog_price_checker-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.2",
+    version="0.1.3",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

