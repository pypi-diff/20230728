# Comparing `tmp/mcrit-1.0.7.tar.gz` & `tmp/mcrit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.7.tar", last modified: Tue Jun  6 15:22:58 2023, max compression
+gzip compressed data, was "mcrit-1.0.8.tar", last modified: Fri Jul 28 10:04:16 2023, max compression
```

## Comparing `mcrit-1.0.7.tar` & `mcrit-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.519425 mcrit-1.0.7/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.7/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13233 2023-06-06 15:22:58.519425 mcrit-1.0.7/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10856 2023-06-06 15:21:51.000000 mcrit-1.0.7/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.255431 mcrit-1.0.7/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.7/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.7/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.287430 mcrit-1.0.7/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.7/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.7/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.287430 mcrit-1.0.7/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-06-06 15:21:29.000000 mcrit-1.0.7/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.7/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.307430 mcrit-1.0.7/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.7/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.327429 mcrit-1.0.7/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.7/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.383428 mcrit-1.0.7/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.7/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.7/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.7/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.7/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.7/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.403428 mcrit-1.0.7/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.7/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.403428 mcrit-1.0.7/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.7/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.7/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.7/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.511426 mcrit-1.0.7/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.7/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.7/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.7/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.519425 mcrit-1.0.7/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.7/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.7/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.7/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    27557 2023-06-06 15:15:08.000000 mcrit-1.0.7/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.7/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.7/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.7/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.7/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.271431 mcrit-1.0.7/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13233 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-06-06 15:22:58.519425 mcrit-1.0.7/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-06-06 15:21:36.000000 mcrit-1.0.7/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.747138 mcrit-1.0.8/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.8/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13651 2023-07-28 10:04:16.747138 mcrit-1.0.8/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11234 2023-07-28 08:53:20.000000 mcrit-1.0.8/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.739138 mcrit-1.0.8/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.8/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.8/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.739138 mcrit-1.0.8/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.8/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.8/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.739138 mcrit-1.0.8/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-07-28 09:10:47.000000 mcrit-1.0.8/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.8/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.8/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.8/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.8/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.8/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.8/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.8/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10743 2023-07-25 13:00:59.000000 mcrit-1.0.8/mcrit/matchers/FunctionCfgMatcher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.8/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.8/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.8/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.8/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.8/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.8/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.8/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.8/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.8/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.8/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.8/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.743138 mcrit-1.0.8/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.8/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.8/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.8/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.747138 mcrit-1.0.8/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.8/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.8/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.8/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.8/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    27557 2023-06-06 15:15:08.000000 mcrit-1.0.8/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.8/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.8/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.8/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.8/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.8/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.8/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-07-28 10:04:16.739138 mcrit-1.0.8/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13651 2023-07-28 10:04:16.000000 mcrit-1.0.8/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1987 2023-07-28 10:04:16.000000 mcrit-1.0.8/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-07-28 10:04:16.000000 mcrit-1.0.8/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      145 2023-07-28 10:04:16.000000 mcrit-1.0.8/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-07-28 10:04:16.000000 mcrit-1.0.8/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-07-28 10:04:16.747138 mcrit-1.0.8/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1371 2023-07-28 08:53:27.000000 mcrit-1.0.8/setup.py
```

### Comparing `mcrit-1.0.7/LICENSE` & `mcrit-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/PKG-INFO` & `mcrit-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.7
+Version: 1.0.8
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -119,16 +119,21 @@
         
         ```
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
+        ### Reference Data 
+        
+        In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
+        
         
         ## Version History
+         * 2023-07-28 v1.0.8: IDA plugin can now display colored graphs for remote functions and do queries for PicBlockHashes (for basic blocks) for the currently viewed function.
          * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
          * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
```

### Comparing `mcrit-1.0.7/README.md` & `mcrit-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -111,16 +111,21 @@
 
 ```
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
+### Reference Data 
+
+In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
+
 
 ## Version History
+ * 2023-07-28 v1.0.8: IDA plugin can now display colored graphs for remote functions and do queries for PicBlockHashes (for basic blocks) for the currently viewed function.
  * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
  * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
  * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
```

### Comparing `mcrit-1.0.7/mcrit/Worker.py` & `mcrit-1.0.8/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/__main__.py` & `mcrit-1.0.8/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/client/McritClient.py` & `mcrit-1.0.8/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/client/McritConsole.py` & `mcrit-1.0.8/mcrit/client/McritConsole.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/config/ConfigInterface.py` & `mcrit-1.0.8/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/config/McritConfig.py` & `mcrit-1.0.8/mcrit/config/McritConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.7"
+    VERSION = "1.0.8"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.7/mcrit/config/MinHashConfig.py` & `mcrit-1.0.8/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/config/QueueConfig.py` & `mcrit-1.0.8/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.8/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/config/StorageConfig.py` & `mcrit-1.0.8/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/index/MinHashIndex.py` & `mcrit-1.0.8/mcrit/index/MinHashIndex.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/index/SearchCursor.py` & `mcrit-1.0.8/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.8/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.8/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/libs/mongoqueue.py` & `mcrit-1.0.8/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/libs/pymmh3.py` & `mcrit-1.0.8/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/libs/utility.py` & `mcrit-1.0.8/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.8/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.8/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.8/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.8/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.8/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.8/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/minhash/MinHash.py` & `mcrit-1.0.8/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/minhash/MinHasher.py` & `mcrit-1.0.8/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.8/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/queue/LocalQueue.py` & `mcrit-1.0.8/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/queue/QueueFactory.py` & `mcrit-1.0.8/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.8/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/BlocksResource.py` & `mcrit-1.0.8/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/FamilyResource.py` & `mcrit-1.0.8/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/FunctionResource.py` & `mcrit-1.0.8/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/JobResource.py` & `mcrit-1.0.8/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/MatchResource.py` & `mcrit-1.0.8/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/QueryResource.py` & `mcrit-1.0.8/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/SampleResource.py` & `mcrit-1.0.8/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/StatusResource.py` & `mcrit-1.0.8/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/application_routes.py` & `mcrit-1.0.8/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/server/utils.py` & `mcrit-1.0.8/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.8/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.8/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.8/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.8/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.8/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MatchingCache.py` & `mcrit-1.0.8/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MatchingResult.py` & `mcrit-1.0.8/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.8/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.8/mcrit/storage/MongoDbStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/SampleEntry.py` & `mcrit-1.0.8/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/StorageFactory.py` & `mcrit-1.0.8/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit/storage/StorageInterface.py` & `mcrit-1.0.8/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.7/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.8/mcrit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.7
+Version: 1.0.8
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -119,16 +119,21 @@
         
         ```
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
+        ### Reference Data 
+        
+        In July 2023, we started populating a [Github repository](https://github.com/danielplohmann/mcrit-data) which contains ready-to-use reference data for common compilers and libraries.
+        
         
         ## Version History
+         * 2023-07-28 v1.0.8: IDA plugin can now display colored graphs for remote functions and do queries for PicBlockHashes (for basic blocks) for the currently viewed function.
          * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
          * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
```

### Comparing `mcrit-1.0.7/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.8/mcrit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 mcrit/index/SearchQueryParser.py
 mcrit/index/SearchQueryTree.py
 mcrit/index/__init__.py
 mcrit/libs/__init__.py
 mcrit/libs/mongoqueue.py
 mcrit/libs/pymmh3.py
 mcrit/libs/utility.py
+mcrit/matchers/FunctionCfgMatcher.py
 mcrit/matchers/MatcherCross.py
 mcrit/matchers/MatcherInterface.py
 mcrit/matchers/MatcherQuery.py
 mcrit/matchers/MatcherQueryFunction.py
 mcrit/matchers/MatcherSample.py
 mcrit/matchers/MatcherVs.py
 mcrit/matchers/__init__.py
```

### Comparing `mcrit-1.0.7/setup.py` & `mcrit-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,20 @@
     "pymongo",
     "pyparsing>=3",
     "requests",
     "scipy",
     "smda>=1.3.0",
     "tqdm",
     "waitress",
+    "rapidfuzz"
 ]
 
 setup(
     name='mcrit',
-    version="1.0.7",
+    version="1.0.8",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

