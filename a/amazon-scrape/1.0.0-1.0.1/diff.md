# Comparing `tmp/amazon_scrape-1.0.0.tar.gz` & `tmp/amazon_scrape-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-1.0.0.tar", last modified: Thu Jul 27 14:25:56 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.1.tar", last modified: Fri Jul 28 06:23:05 2023, max compression
```

## Comparing `amazon_scrape-1.0.0.tar` & `amazon_scrape-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.425020 amazon_scrape-1.0.0/
--rw-r--r--   0 finn       (501) staff       (20)     4938 2023-07-27 14:25:56.425214 amazon_scrape-1.0.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2228 2023-07-27 14:23:23.000000 amazon_scrape-1.0.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.422584 amazon_scrape-1.0.0/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4938 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.424541 amazon_scrape-1.0.0/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-1.0.0/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-27 14:22:54.000000 amazon_scrape-1.0.0/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 14:25:52.000000 amazon_scrape-1.0.0/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 14:25:56.425928 amazon_scrape-1.0.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-27 14:25:52.000000 amazon_scrape-1.0.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.084725 amazon_scrape-1.0.1/
+-rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:23:05.085188 amazon_scrape-1.0.1/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2204 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.081539 amazon_scrape-1.0.1/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:22:13.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 06:23:04.000000 amazon_scrape-1.0.1/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:23:05.084068 amazon_scrape-1.0.1/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 06:23:05.086370 amazon_scrape-1.0.1/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 06:21:42.000000 amazon_scrape-1.0.1/setup.py
```

### Comparing `amazon_scrape-1.0.0/PKG-INFO` & `amazon_scrape-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -51,16 +51,15 @@
             usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
         
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
-            --proxy_api_key PROXY_API_KEY
-                                    API Key
+            --proxy_api_key       Scraper API Key
             --pages PAGES         Number of pages to scrape
         
         
         Usage Example
         -------------
         
         .. code-block:: python
```

### Comparing `amazon_scrape-1.0.0/README.md` & `amazon_scrape-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
 
 optional arguments:
   -h, --help            show this help message and exit
   --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
   --keywords KEYWORDS   Search keywords
   --url URL             Amazon URL
-  --proxy_api_key PROXY_API_KEY
-                        API Key
+  --proxy_api_key       Scraper API Key
   --pages PAGES         Number of pages to scrape
 ```
 
 ## Usage Example
 
 ```python
 # Specify locale, keywords, API key, and number of pages to scrape
```

### Comparing `amazon_scrape-1.0.0/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.1/amazon_scrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -51,16 +51,15 @@
             usage: amazon_scraper [-h] [--locale LOCALE] [--keywords KEYWORDS] [--url URL] [--proxy_api_key PROXY_API_KEY] [--pages PAGES]
         
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
-            --proxy_api_key PROXY_API_KEY
-                                    API Key
+            --proxy_api_key       Scraper API Key
             --pages PAGES         Number of pages to scrape
         
         
         Usage Example
         -------------
         
         .. code-block:: python
```

### Comparing `amazon_scrape-1.0.0/amazon_scraper/scraper.py` & `amazon_scrape-1.0.1/amazon_scraper/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.csv_file = open('amazon_products.csv', 'w', newline='')
         self.json_file = open('amazon_products.json', 'w')
         self.writer = csv.writer(self.csv_file)
         self.json_data = []
         self.locale = locale
 
     def start_scraping(self):
-        self.writer.writerow(["product_name", "product_images", "price", "product_url", "number_of_reviews", "asin"])
+        self.writer.writerow(["product_name", "product_images", "number_of_reviews", "price", "product_url", "asin"])
         for page in range(1, self.pages + 1):
             url = self.url + "&page=" + str(page)
             headers = {"User-Agent": random.choice(self.user_agents)}
             response = requests.get(url, headers=headers)
             soup = BeautifulSoup(response.content, "html.parser")
             products = soup.find_all("div", {"class": "sg-col-inner"})
 
@@ -63,48 +63,48 @@
                 # Product images
                 images = product.find_all("img", {"class": "s-image"})
                 if images is not None:
                     images = [image['src'] for image in images]
                 else:
                     images = []
 
+                # Number of Reviews
+                number_of_reviews = product.find("span", {"class": "a-size-base"})
+                if number_of_reviews is not None:
+                    number_of_reviews = number_of_reviews.text
+                else:
+                    number_of_reviews = ''
+
                 # Price
                 price = product.find("span", {"class": "a-offscreen"})
                 if price is not None:
                     price = price.text
                 else:
                     price = ''
 
                 # Product URL
                 product_url = product.find("a", {"class": "a-link-normal"})
                 if product_url is not None:
                     product_url = f'https://www.amazon.{self.locale}' + product_url['href']
                 else:
                     product_url = ''
 
-                # Number of reviews
-                number_of_reviews = product.find("span", {"class": "a-size-base"})
-                if number_of_reviews is not None:
-                    number_of_reviews = number_of_reviews.text
-                else:
-                    number_of_reviews = ''
-
                 # ASIN
                 asin = product_url.split("/dp/")[1].split("/")[0] if "/dp/" in product_url else ''
 
                 # Write to CSV
-                self.writer.writerow([name, ", ".join(images), price, product_url, number_of_reviews, asin])
+                self.writer.writerow([name, ", ".join(images), number_of_reviews, price, product_url, asin])
 
                 # Add to JSON data
                 self.json_data.append({
                     "product_name": name,
                     "product_images": images,
+                    "number_of_reviews": number_of_reviews,
                     "price": price,
                     "product_url": product_url,
-                    "number_of_reviews": number_of_reviews,
                     "asin": asin
                 })
 
         json.dump(self.json_data, self.json_file, indent=4)
 
     def close_files(self):
         self.csv_file.close()
```

### Comparing `amazon_scrape-1.0.0/setup.py` & `amazon_scrape-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

