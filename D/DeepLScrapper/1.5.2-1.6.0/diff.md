# Comparing `tmp/DeepLScrapper-1.5.2.tar.gz` & `tmp/DeepLScrapper-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.5.2.tar", last modified: Thu Jul 27 21:47:44 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.6.0.tar", last modified: Thu Jul 27 22:34:57 2023, max compression
```

## Comparing `DeepLScrapper-1.5.2.tar` & `DeepLScrapper-1.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/DeepLScrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/DeepLScrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/DeepLScrapper/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.126063 DeepLScrapper-1.6.0/DeepLScrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/DeepLScrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/DeepLScrapper/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 22:34:57.000000 DeepLScrapper-1.6.0/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:34:57.130063 DeepLScrapper-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 22:34:48.000000 DeepLScrapper-1.6.0/setup.py
```

### Comparing `DeepLScrapper-1.5.2/DeepLScrapper.egg-info/PKG-INFO` & `DeepLScrapper-1.6.0/DeepLScrapper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.5.2
+Version: 1.6.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -59,24 +59,24 @@
 from DeepLScrapper import DeepLScrapper
 
 # Initialize the translator with a custom rate limit delay of 5 seconds
 translator = DeepLScrapper(rate_limit_delay=5)
 
 try:
     # Translate text from English to German
-    translation = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 1:", translation)
 
     # Translate the same text again to test caching
-    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 2 (Cached):", translation_cached)
 
     # Translate multiple texts in bulk
     texts = ['How are you?', 'Goodbye!', 'Welcome back.']
-    bulk_translations = translator.translate(texts, source_lang='en', target_lang='fr')
+    bulk_translations = translator.translate(texts, source_lang='en', target_lang='el')
     print("Bulk Translations:", bulk_translations)
 
     # Test language validation with an invalid language code
     try:
         invalid_translation = translator.translate('Hello, World!', source_lang='en', target_lang='invalid')
         print("Invalid Translation:", invalid_translation)
     except ValueError as e:
@@ -96,23 +96,26 @@
     translator.close()
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
+- fake_useragent
+- sqlite3
 
 ## Version History
 
-
+- 1.6.0
+    - Added a translation memory feature. The class now stores previously translated texts in the database, reducing redundant requests to DeepL and speeding up translations for repeated texts.
 - 1.5.[0-2]
     - Restructured the project
     - Fixed the issue to using the library
     - Updated the documentation regarding the changes
-- 1.[3-5].0
+- 1.[1-4].0
     - Initial release
     - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `DeepLScrapper-1.5.2/LICENSE` & `DeepLScrapper-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.5.2/PKG-INFO` & `DeepLScrapper-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.5.2
+Version: 1.6.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -59,24 +59,24 @@
 from DeepLScrapper import DeepLScrapper
 
 # Initialize the translator with a custom rate limit delay of 5 seconds
 translator = DeepLScrapper(rate_limit_delay=5)
 
 try:
     # Translate text from English to German
-    translation = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 1:", translation)
 
     # Translate the same text again to test caching
-    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 2 (Cached):", translation_cached)
 
     # Translate multiple texts in bulk
     texts = ['How are you?', 'Goodbye!', 'Welcome back.']
-    bulk_translations = translator.translate(texts, source_lang='en', target_lang='fr')
+    bulk_translations = translator.translate(texts, source_lang='en', target_lang='el')
     print("Bulk Translations:", bulk_translations)
 
     # Test language validation with an invalid language code
     try:
         invalid_translation = translator.translate('Hello, World!', source_lang='en', target_lang='invalid')
         print("Invalid Translation:", invalid_translation)
     except ValueError as e:
@@ -96,23 +96,26 @@
     translator.close()
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
+- fake_useragent
+- sqlite3
 
 ## Version History
 
-
+- 1.6.0
+    - Added a translation memory feature. The class now stores previously translated texts in the database, reducing redundant requests to DeepL and speeding up translations for repeated texts.
 - 1.5.[0-2]
     - Restructured the project
     - Fixed the issue to using the library
     - Updated the documentation regarding the changes
-- 1.[3-5].0
+- 1.[1-4].0
     - Initial release
     - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `DeepLScrapper-1.5.2/README.md` & `DeepLScrapper-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 from DeepLScrapper import DeepLScrapper
 
 # Initialize the translator with a custom rate limit delay of 5 seconds
 translator = DeepLScrapper(rate_limit_delay=5)
 
 try:
     # Translate text from English to German
-    translation = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 1:", translation)
 
     # Translate the same text again to test caching
-    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='el')
+    translation_cached = translator.translate('Hello, World!', source_lang='en', target_lang='de')
     print("Translation 2 (Cached):", translation_cached)
 
     # Translate multiple texts in bulk
     texts = ['How are you?', 'Goodbye!', 'Welcome back.']
-    bulk_translations = translator.translate(texts, source_lang='en', target_lang='fr')
+    bulk_translations = translator.translate(texts, source_lang='en', target_lang='el')
     print("Bulk Translations:", bulk_translations)
 
     # Test language validation with an invalid language code
     try:
         invalid_translation = translator.translate('Hello, World!', source_lang='en', target_lang='invalid')
         print("Invalid Translation:", invalid_translation)
     except ValueError as e:
@@ -79,23 +79,26 @@
     translator.close()
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
+- fake_useragent
+- sqlite3
 
 ## Version History
 
-
+- 1.6.0
+    - Added a translation memory feature. The class now stores previously translated texts in the database, reducing redundant requests to DeepL and speeding up translations for repeated texts.
 - 1.5.[0-2]
     - Restructured the project
     - Fixed the issue to using the library
     - Updated the documentation regarding the changes
-- 1.[3-5].0
+- 1.[1-4].0
     - Initial release
     - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `DeepLScrapper-1.5.2/setup.py` & `DeepLScrapper-1.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeepLScrapper',
-    version='1.5.2',
+    version='1.6.0',
     description='An unofficial Python library for translating text using DeepL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Olger Chotza',
     author_email='olgerdev@icloud.com',
     packages=find_packages(),
     install_requires=[
         'selenium',
         'beautifulsoup4',
-        'fake-useragent'
+        'fake-useragent',
+        'sqlite3'
     ],
     python_requires='>=3.9',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
```

