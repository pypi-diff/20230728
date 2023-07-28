# Comparing `tmp/krcg-bot-3.3.tar.gz` & `tmp/krcg-bot-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krcg-bot-3.3.tar", last modified: Mon Nov 14 12:00:33 2022, max compression
+gzip compressed data, was "krcg-bot-3.4.tar", last modified: Fri Jul 28 06:24:29 2023, max compression
```

## Comparing `krcg-bot-3.3.tar` & `krcg-bot-3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2022-11-14 12:00:33.992836 krcg-bot-3.3/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1239 2022-11-14 12:00:33.000000 krcg-bot-3.3/CHANGELOG.rst
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2022-11-14 12:00:33.000000 krcg-bot-3.3/LICENSE
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      252 2022-11-14 12:00:33.000000 krcg-bot-3.3/MANIFEST.in
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3761 2022-11-14 12:00:33.992894 krcg-bot-3.3/PKG-INFO
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3054 2022-11-14 12:00:33.000000 krcg-bot-3.3/README.md
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2022-11-14 12:00:33.992630 krcg-bot-3.3/krcg_bot/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    11234 2022-11-14 12:00:33.000000 krcg-bot-3.3/krcg_bot/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       27 2022-11-14 12:00:33.000000 krcg-bot-3.3/krcg_bot/__main__.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2022-11-14 12:00:33.992742 krcg-bot-3.3/krcg_bot.egg-info/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      104 2022-11-14 12:00:33.000000 krcg-bot-3.3/krcg_bot.egg-info/SOURCES.txt
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1337 2022-11-14 12:00:33.993264 krcg-bot-3.3/setup.cfg
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2022-11-14 12:00:33.000000 krcg-bot-3.3/setup.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-28 06:24:29.907990 krcg-bot-3.4/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1345 2023-07-28 06:24:29.000000 krcg-bot-3.4/CHANGELOG.rst
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2023-07-28 06:24:29.000000 krcg-bot-3.4/LICENSE
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      252 2023-07-28 06:24:29.000000 krcg-bot-3.4/MANIFEST.in
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3784 2023-07-28 06:24:29.908072 krcg-bot-3.4/PKG-INFO
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3054 2023-07-28 06:24:29.000000 krcg-bot-3.4/README.md
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-28 06:24:29.907787 krcg-bot-3.4/krcg_bot/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    11234 2023-07-28 06:24:29.000000 krcg-bot-3.4/krcg_bot/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       27 2023-07-28 06:24:29.000000 krcg-bot-3.4/krcg_bot/__main__.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2023-07-28 06:24:29.907909 krcg-bot-3.4/krcg_bot.egg-info/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      104 2023-07-28 06:24:29.000000 krcg-bot-3.4/krcg_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1369 2023-07-28 06:24:29.908522 krcg-bot-3.4/setup.cfg
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       39 2023-07-28 06:24:29.000000 krcg-bot-3.4/setup.py
```

### Comparing `krcg-bot-3.3/CHANGELOG.rst` & `krcg-bot-3.4/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.4 (2023-07-28)
+----------------
+
+- Bump KRCG (3.0)
+- Bump Discord lib discord-py-interactions (4.4.1)
+
+
 3.3 (2022-11-14)
 ----------------
 
 - Fix embed border color for powers and convictions
 - Bump KRCG (2.30)
 
 3.2 (2022-08-25)
```

### Comparing `krcg-bot-3.3/LICENSE` & `krcg-bot-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krcg-bot-3.3/PKG-INFO` & `krcg-bot-3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: krcg-bot
-Version: 3.3
+Version: 3.4
 Summary: "Discord bot for VTES cards",
 Home-page: http://github.com/lionel-panhaleux/krcg-bot
 Author: lionelpx
 Author-email: lionel.panhaleux@gmail.com
 License: "MIT"
 Keywords: vampire vtes ccg discord bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Games/Entertainment
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # KRCG Discord Bot
 
 [![PyPI version](https://badge.fury.io/py/krcg-bot.svg)](https://badge.fury.io/py/krcg-bot)
```

### Comparing `krcg-bot-3.3/README.md` & `krcg-bot-3.4/README.md`

 * *Files identical despite different names*

### Comparing `krcg-bot-3.3/krcg_bot/__init__.py` & `krcg-bot-3.4/krcg_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `krcg-bot-3.3/setup.cfg` & `krcg-bot-3.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = krcg-bot
-version = 3.3
+version = 3.4
 author = lionelpx
 author_email = lionel.panhaleux@gmail.com
 url = http://github.com/lionel-panhaleux/krcg-bot
 description = "Discord bot for VTES cards",
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "MIT"
@@ -16,22 +16,23 @@
 	Operating System :: OS Independent
 	Environment :: Plugins
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Topic :: Games/Entertainment
 
 [options]
+python_requires = >=3.8
 zip_safe = True
 include_package_data = True
 packages = find:
 setup_requires = 
 	setuptools
 install_requires = 
-	discord-py-interactions
-	krcg >= 2.30
+	discord-py-interactions >= 4.4.1
+	krcg >= 3.0
 	setuptools
 	unidecode
 
 [options.extras_require]
 dev = 
 	black
 	doc8
```

