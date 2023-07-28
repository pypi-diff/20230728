# Comparing `tmp/amazon_scrape-1.0.2.tar.gz` & `tmp/amazon_scrape-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-1.0.2.tar", last modified: Fri Jul 28 06:33:10 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.3.tar", last modified: Fri Jul 28 09:11:17 2023, max compression
```

## Comparing `amazon_scrape-1.0.2.tar` & `amazon_scrape-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.767798 amazon_scrape-1.0.2/
--rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:33:10.768176 amazon_scrape-1.0.2/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2204 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.763759 amazon_scrape-1.0.2/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4902 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 06:33:10.000000 amazon_scrape-1.0.2/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 06:33:10.766997 amazon_scrape-1.0.2/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 06:33:10.769150 amazon_scrape-1.0.2/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 06:31:54.000000 amazon_scrape-1.0.2/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.614519 amazon_scrape-1.0.3/
+-rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:11:17.614924 amazon_scrape-1.0.3/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2368 2023-07-28 09:10:39.000000 amazon_scrape-1.0.3/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.611540 amazon_scrape-1.0.3/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5107 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 09:11:17.000000 amazon_scrape-1.0.3/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 09:11:17.613782 amazon_scrape-1.0.3/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.3/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8368 2023-07-28 09:06:51.000000 amazon_scrape-1.0.3/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 09:07:22.000000 amazon_scrape-1.0.3/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 09:11:17.616136 amazon_scrape-1.0.3/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 09:07:22.000000 amazon_scrape-1.0.3/setup.py
```

### Comparing `amazon_scrape-1.0.2/PKG-INFO` & `amazon_scrape-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 1.0.2
+Version: 1.0.3
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -53,33 +53,37 @@
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
             --proxy_api_key       Scraper API Key
             --pages PAGES         Number of pages to scrape
+            -r, --review          Scrape reviews
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            ## Specify locale, keywords, API key, and number of pages to scrape
+            # Specify locale, keywords, API key, and number of pages to scrape:
             amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
         
             ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
             amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
         
             ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
             amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
             ## Specify locale and Amazon URL (will default to 20 pages):
             amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
+            ## Specify review to scrape product(s) reviews:
+            amazon_scraper --keywords "watches" --proxy_api_key "your_api_key --review
+        
         
         Create Scraper API Account
         --------------------------
         
         Sign up for a Scraper API `user account`_.
         
         .. _user account: https://www.scraperapi.com/?fp_ref=finbarrs11
```

### Comparing `amazon_scrape-1.0.2/README.md` & `amazon_scrape-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,30 +35,34 @@
 optional arguments:
   -h, --help            show this help message and exit
   --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
   --keywords KEYWORDS   Search keywords
   --url URL             Amazon URL
   --proxy_api_key       Scraper API Key
   --pages PAGES         Number of pages to scrape
+  -r, --review          Scrape reviews
 ```
 
 ## Usage Example
 
 ```python
-# Specify locale, keywords, API key, and number of pages to scrape
+# Specify locale, keywords, API key, and number of pages to scrape:
 amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
 
 ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
 amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
 
 ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
 amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
 
 ## Specify locale and Amazon URL (will default to 20 pages):
 amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+
+## Specify review to scrape product(s) reviews:
+amazon_scraper --keywords "watches" --proxy_api_key "your_api_key --review
 ```
 
 ## Create Scraper API Account
 
 Sign up for a Scraper API [user account](https://www.scraperapi.com/?fp_ref=finbarrs11).
```

### Comparing `amazon_scrape-1.0.2/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.3/amazon_scrape.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 1.0.2
+Version: 1.0.3
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -53,33 +53,37 @@
             optional arguments:
             -h, --help            show this help message and exit
             --locale LOCALE       Amazon locale (e.g., "com", "co.uk", "de", etc.)
             --keywords KEYWORDS   Search keywords
             --url URL             Amazon URL
             --proxy_api_key       Scraper API Key
             --pages PAGES         Number of pages to scrape
+            -r, --review          Scrape reviews
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
-            ## Specify locale, keywords, API key, and number of pages to scrape
+            # Specify locale, keywords, API key, and number of pages to scrape:
             amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
         
             ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
             amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
         
             ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
             amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
             ## Specify locale and Amazon URL (will default to 20 pages):
             amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
+            ## Specify review to scrape product(s) reviews:
+            amazon_scraper --keywords "watches" --proxy_api_key "your_api_key --review
+        
         
         Create Scraper API Account
         --------------------------
         
         Sign up for a Scraper API `user account`_.
         
         .. _user account: https://www.scraperapi.com/?fp_ref=finbarrs11
```

### Comparing `amazon_scrape-1.0.2/amazon_scraper/scraper.py` & `amazon_scrape-1.0.3/amazon_scraper/scraper.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,30 +25,37 @@
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36",
         "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36",
         "Mozilla/5.0 (Windows NT 5.1; rv:7.0.1) Gecko/20100101 Firefox/7.0.1",
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.140 Safari/537.36 Edge/17.17134",
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:62.0) Gecko/20100101 Firefox/62.0"
     ]
 
-    def __init__(self, locale="co.uk", keyword=None, url=None, api_key=None, pages=20):
+    def __init__(self, locale="co.uk", keyword=None, url=None, api_key=None, pages=20, review=False):
         base_url = f"https://www.amazon.{locale}/s"
         if keyword:
             self.url = f"http://api.scraperapi.com?api_key={api_key}&url={base_url}?k={keyword}"
         else:
             self.url = f"http://api.scraperapi.com?api_key={api_key}&url={url}"
         self.api_key = api_key
         self.pages = pages
-        self.csv_file = open('amazon_products.csv', 'w', newline='')
-        self.json_file = open('amazon_products.json', 'w')
-        self.writer = csv.writer(self.csv_file)
-        self.json_data = []
+        self.review = review
+        self.product_csv_file = open('amazon_products.csv', 'w', newline='')
+        self.product_json_file = open('amazon_products.json', 'w')
+        self.review_csv_file = open('amazon_reviews.csv', 'w', newline='') if review else None
+        self.review_json_file = open('amazon_reviews.json', 'w') if review else None
+        self.product_writer = csv.writer(self.product_csv_file)
+        self.review_writer = csv.writer(self.review_csv_file) if review else None
+        self.product_json_data = []
+        self.review_json_data = []
         self.locale = locale
 
     def start_scraping(self):
-        self.writer.writerow(["product_name", "product_images", "number_of_reviews", "price", "product_url", "asin"])
+        self.product_writer.writerow(["product_name", "product_images", "number_of_reviews", "price", "product_url", "asin"])
+        if self.review:
+            self.review_writer.writerow(["product_name", "product_reviews", "product_url", "asin"])
         for page in range(1, self.pages + 1):
             url = self.url + "&page=" + str(page)
             headers = {"User-Agent": random.choice(self.user_agents)}
             response = requests.get(url, headers=headers)
             soup = BeautifulSoup(response.content, "html.parser")
             products = soup.find_all("div", {"class": "sg-col-inner"})
 
@@ -88,40 +95,67 @@
                 else:
                     product_url = ''
 
                 # ASIN
                 asin = product_url.split("/dp/")[1].split("/")[0] if "/dp/" in product_url else ''
 
                 # Write to CSV
-                self.writer.writerow([name, ", ".join(images), number_of_reviews, price, product_url, asin])
+                self.product_writer.writerow([name, ", ".join(images), number_of_reviews, price, product_url, asin])
 
                 # Add to JSON data
-                self.json_data.append({
+                self.product_json_data.append({
                     "product_name": name,
                     "product_images": images,
                     "number_of_reviews": number_of_reviews,
                     "price": price,
                     "product_url": product_url,
                     "asin": asin
                 })
 
-        json.dump(self.json_data, self.json_file, indent=4)
+                # Product reviews
+                if self.review:
+                    product_reviews = []
+                    review_url = f'https://www.amazon.{self.locale}/product-reviews/{asin}'
+                    review_response = requests.get(review_url, headers=headers)
+                    review_soup = BeautifulSoup(review_response.content, "html.parser")
+                    reviews = review_soup.find_all("span", {"data-hook": "review-body"})
+                    for review in reviews:
+                        product_reviews.append(review.text.strip())
+
+                    # Write to CSV
+                    self.review_writer.writerow([name, ", ".join(product_reviews), product_url, asin])
+
+                    # Add to JSON data
+                    self.review_json_data.append({
+                        "product_name": name,
+                        "product_reviews": product_reviews,
+                        "product_url": product_url,
+                        "asin": asin
+                    })
+
+        json.dump(self.product_json_data, self.product_json_file, indent=4)
+        if self.review:
+            json.dump(self.review_json_data, self.review_json_file, indent=4)
 
     def close_files(self):
-        self.csv_file.close()
-        self.json_file.close()
+        self.product_csv_file.close()
+        self.product_json_file.close()
+        if self.review:
+            self.review_csv_file.close()
+            self.review_json_file.close()
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--locale', type=str, default='co.uk', help='Amazon locale (e.g., "com", "co.uk", "de", etc.)')
     parser.add_argument('--keywords', type=str, help='Search keywords')
     parser.add_argument('--url', type=str, help='Amazon URL')
     parser.add_argument('--proxy_api_key', type=str, help='API Key')
     parser.add_argument('--pages', type=int, default=20, help='Number of pages to scrape')
+    parser.add_argument('-r', '--review', action='store_true', help='Scrape reviews')
     args = parser.parse_args()
 
-    scraper = AmazonScraper(args.locale, args.keywords, args.url, args.proxy_api_key, args.pages)
+    scraper = AmazonScraper(args.locale, args.keywords, args.url, args.proxy_api_key, args.pages, args.review)
     scraper.start_scraping()
     scraper.close_files()
 
 if __name__ == '__main__':
     main()
```

### Comparing `amazon_scrape-1.0.2/setup.py` & `amazon_scrape-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

