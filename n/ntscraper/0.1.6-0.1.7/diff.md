# Comparing `tmp/ntscraper-0.1.6.tar.gz` & `tmp/ntscraper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.1.6.tar", last modified: Thu Jul 27 18:07:55 2023, max compression
+gzip compressed data, was "ntscraper-0.1.7.tar", last modified: Fri Jul 28 11:18:59 2023, max compression
```

## Comparing `ntscraper-0.1.6.tar` & `ntscraper-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.964204 ntscraper-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3439 2023-07-27 18:07:55.964204 ntscraper-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2513 2023-07-27 18:07:45.000000 ntscraper-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.908185 ntscraper-0.1.6/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-07-12 10:00:30.000000 ntscraper-0.1.6/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    27712 2023-07-27 18:05:03.000000 ntscraper-0.1.6/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.964204 ntscraper-0.1.6/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     3439 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 18:07:55.964204 ntscraper-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-07-27 18:05:32.000000 ntscraper-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:18:59.909497 ntscraper-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2023-07-28 11:18:59.901492 ntscraper-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2513 2023-07-27 18:07:45.000000 ntscraper-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 11:18:59.845480 ntscraper-0.1.7/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-07-12 10:00:30.000000 ntscraper-0.1.7/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    27795 2023-07-28 11:18:21.000000 ntscraper-0.1.7/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:18:59.901492 ntscraper-0.1.7/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     3439 2023-07-28 11:18:59.000000 ntscraper-0.1.7/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-28 11:18:59.000000 ntscraper-0.1.7/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:18:59.000000 ntscraper-0.1.7/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-28 11:18:59.000000 ntscraper-0.1.7/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 11:18:59.000000 ntscraper-0.1.7/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:18:59.909497 ntscraper-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-07-28 11:18:44.000000 ntscraper-0.1.7/setup.py
```

### Comparing `ntscraper-0.1.6/LICENSE.txt` & `ntscraper-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.6/PKG-INFO` & `ntscraper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.1.6/README.md` & `ntscraper-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.6/ntscraper/nitter.py` & `ntscraper-0.1.7/ntscraper/nitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,16 @@
                     for img in tweet.find("div", class_="tweet-body")
                     .find("div", class_="attachments", recursive=False)
                     .find_all("img")
                 ]
                 videos = [
                     b64decode(video["data-url"].split("/")[-1].encode("utf-8")).decode(
                         "utf-8"
-                    )
+                    ) if "data-url" in video.attrs
+                    else video.find("source")["src"]
                     for video in tweet.find("div", class_="tweet-body")
                     .find("div", class_="attachments", recursive=False)
                     .find_all("video", class_="")
                 ]
                 gifs = [
                     "https://"
                     + b64decode(
```

### Comparing `ntscraper-0.1.6/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.1.7/ntscraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.1.6/setup.py` & `ntscraper-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.1.6",
+    version="0.1.7",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

