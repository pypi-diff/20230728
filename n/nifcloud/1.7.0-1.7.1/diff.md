# Comparing `tmp/nifcloud-1.7.0.tar.gz` & `tmp/nifcloud-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifcloud-1.7.0.tar", last modified: Fri Jun 30 01:56:48 2023, max compression
+gzip compressed data, was "nifcloud-1.7.1.tar", last modified: Fri Jul 28 07:18:10 2023, max compression
```

## Comparing `nifcloud-1.7.0.tar` & `nifcloud-1.7.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 01:56:39.000000 nifcloud-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-30 01:56:48.695919 nifcloud-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-30 01:56:39.000000 nifcloud-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/_retry.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/computing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/computing/3.0/
--rw-r--r--   0 runner    (1001) docker     (123)   756272 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/computing/3.0/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/computing/3.0/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/dns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/endpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/ess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/
--rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/hatoba/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/hatoba/v1/
--rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/hatoba/v1/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/hatoba/v1/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/nas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/script/2015-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/script/2015-09-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/service-activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 01:56:48.695919 nifcloud-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-30 01:56:39.000000 nifcloud-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-28 07:18:01.000000 nifcloud-1.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-28 07:18:10.558851 nifcloud-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-28 07:18:01.000000 nifcloud-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/_retry.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/computing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/data/computing/3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   756272 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/computing/3.0/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/computing/3.0/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/dns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/data/dns/2012-12-12N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/endpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/ess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/data/ess/2010-12-01N2014-05-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/hatoba/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/hatoba/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/hatoba/v1/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/hatoba/v1/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/nas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/nas/N2016-02-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/nas/N2016-02-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/nas/N2016-02-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/rdb/2013-05-15N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/script/2015-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/script/2015-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/sdk-default-configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.550851 nifcloud-1.7.1/nifcloud/data/service-activity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/service-activity/2020-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/service-activity/2020-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud/data/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/data/storage/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/data/storage/2006-03-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.558851 nifcloud-1.7.1/nifcloud/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-28 07:18:01.000000 nifcloud-1.7.1/nifcloud/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 07:18:10.554851 nifcloud-1.7.1/nifcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-28 07:18:10.000000 nifcloud-1.7.1/nifcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-28 07:18:10.000000 nifcloud-1.7.1/nifcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 07:18:10.000000 nifcloud-1.7.1/nifcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 07:18:10.000000 nifcloud-1.7.1/nifcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 07:18:10.000000 nifcloud-1.7.1/nifcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 07:18:10.558851 nifcloud-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-28 07:18:01.000000 nifcloud-1.7.1/setup.py
```

### Comparing `nifcloud-1.7.0/LICENSE.txt` & `nifcloud-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/PKG-INFO` & `nifcloud-1.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: nifcloud
-Version: 1.7.0
+Version: 1.7.1
 Summary: Data-driven NIFCLOUD SDK for Python
 Home-page: https://github.com/nifcloud/nifcloud-sdk-python
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -40,15 +33,15 @@
 
 * :heavy_check_mark: Full support for NIFCLOUD Computing / RDB / NAS / Script / Hatoba / ESS / DNS / ObjectStorageService / ServiceActivity APIs
 * :heavy_check_mark: The nifcloud package is the foundation for the [NIFCLOUD CLI](https://github.com/nifcloud/nifcloud-cli).
 * :heavy_check_mark: AWS-SDK-compatible data-driven architecture
 
 ## Requirements
 
-* Python 2.6 or later
+- Python 3.7 or later
 
 ## How to Install
 
 ```
 pip install nifcloud
 ```
```

### Comparing `nifcloud-1.7.0/README.md` & `nifcloud-1.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 * :heavy_check_mark: Full support for NIFCLOUD Computing / RDB / NAS / Script / Hatoba / ESS / DNS / ObjectStorageService / ServiceActivity APIs
 * :heavy_check_mark: The nifcloud package is the foundation for the [NIFCLOUD CLI](https://github.com/nifcloud/nifcloud-cli).
 * :heavy_check_mark: AWS-SDK-compatible data-driven architecture
 
 ## Requirements
 
-* Python 2.6 or later
+- Python 3.7 or later
 
 ## How to Install
 
 ```
 pip install nifcloud
 ```
```

### Comparing `nifcloud-1.7.0/nifcloud/data/_retry.json` & `nifcloud-1.7.1/nifcloud/data/_retry.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/computing/3.0/service-2.json` & `nifcloud-1.7.1/nifcloud/data/computing/3.0/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/computing/3.0/waiters-2.json` & `nifcloud-1.7.1/nifcloud/data/computing/3.0/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json` & `nifcloud-1.7.1/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/endpoints.json` & `nifcloud-1.7.1/nifcloud/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json` & `nifcloud-1.7.1/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/hatoba/v1/service-2.json` & `nifcloud-1.7.1/nifcloud/data/hatoba/v1/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/hatoba/v1/waiters-2.json` & `nifcloud-1.7.1/nifcloud/data/hatoba/v1/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/service-2.json` & `nifcloud-1.7.1/nifcloud/data/nas/N2016-02-24/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/waiters-2.json` & `nifcloud-1.7.1/nifcloud/data/nas/N2016-02-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json` & `nifcloud-1.7.1/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json` & `nifcloud-1.7.1/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/script/2015-09-01/service-2.json` & `nifcloud-1.7.1/nifcloud/data/script/2015-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/service-2.json` & `nifcloud-1.7.1/nifcloud/data/service-activity/2020-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/service-2.json` & `nifcloud-1.7.1/nifcloud/data/storage/2006-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/docs/__init__.py` & `nifcloud-1.7.1/nifcloud/docs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,17 +31,18 @@
         ).replace('AWS', 'NIFCLOUD')
         method_intro.clear_text()
         method_intro.push_write(replaced_text)
 
 
 class ServiceDocumenter(service.ServiceDocumenter):
 
-    def __init__(self, service_name, session):
+    def __init__(self, service_name, session, root_docs_path):
         self._session = session
         self._service_name = service_name
+        self._root_docs_path = root_docs_path
 
         self._client = self._session.create_client(
             service_name, region_name='jp-east-1', nifcloud_access_key_id='foo',
             nifcloud_secret_access_key='bar')
         self._event_emitter = self._client.meta.events
 
         self.sections = [
```

### Comparing `nifcloud-1.7.0/nifcloud/parsers.py` & `nifcloud-1.7.1/nifcloud/parsers.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/serialize.py` & `nifcloud-1.7.1/nifcloud/serialize.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud/session.py` & `nifcloud-1.7.1/nifcloud/session.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.7.0/nifcloud.egg-info/PKG-INFO` & `nifcloud-1.7.1/nifcloud.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: nifcloud
-Version: 1.7.0
+Version: 1.7.1
 Summary: Data-driven NIFCLOUD SDK for Python
 Home-page: https://github.com/nifcloud/nifcloud-sdk-python
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -40,15 +33,15 @@
 
 * :heavy_check_mark: Full support for NIFCLOUD Computing / RDB / NAS / Script / Hatoba / ESS / DNS / ObjectStorageService / ServiceActivity APIs
 * :heavy_check_mark: The nifcloud package is the foundation for the [NIFCLOUD CLI](https://github.com/nifcloud/nifcloud-cli).
 * :heavy_check_mark: AWS-SDK-compatible data-driven architecture
 
 ## Requirements
 
-* Python 2.6 or later
+- Python 3.7 or later
 
 ## How to Install
 
 ```
 pip install nifcloud
 ```
```

### Comparing `nifcloud-1.7.0/nifcloud.egg-info/SOURCES.txt` & `nifcloud-1.7.1/nifcloud.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 nifcloud.egg-info/PKG-INFO
 nifcloud.egg-info/SOURCES.txt
 nifcloud.egg-info/dependency_links.txt
 nifcloud.egg-info/requires.txt
 nifcloud.egg-info/top_level.txt
 nifcloud/data/_retry.json
 nifcloud/data/endpoints.json
+nifcloud/data/sdk-default-configuration.json
 nifcloud/data/computing/3.0/service-2.json
 nifcloud/data/computing/3.0/waiters-2.json
 nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json
 nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json
 nifcloud/data/hatoba/v1/service-2.json
 nifcloud/data/hatoba/v1/waiters-2.json
 nifcloud/data/nas/N2016-02-24/service-2.json
```

### Comparing `nifcloud-1.7.0/setup.py` & `nifcloud-1.7.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,31 +31,24 @@
     long_description_content_type='text/markdown',
     author='FUJITSU CLOUD TECHNOLOGIES',
     url='https://github.com/nifcloud/nifcloud-sdk-python',
     packages=find_packages(exclude=['tests*']),
     package_data={'nifcloud': ['data/*.json',
                                'data/*/*/*.json']},
     include_package_data=True,
-    install_requires=['botocore==1.21.43'],
+    install_requires=['botocore==1.31.1'],
     license='Apache License 2.0',
     classifiers=(
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ),
 )
```

