# Comparing `tmp/socketlabs_injectionapi-1.4.3.tar.gz` & `tmp/socketlabs_injectionapi-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketlabs_injectionapi-1.4.3.tar", last modified: Mon May 22 19:45:02 2023, max compression
+gzip compressed data, was "socketlabs_injectionapi-1.4.4.tar", last modified: Fri Jul 28 14:59:49 2023, max compression
```

## Comparing `socketlabs_injectionapi-1.4.3.tar` & `socketlabs_injectionapi-1.4.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.771768 socketlabs_injectionapi-1.4.3/
--rw-rw-rw-   0        0        0     2324 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1086 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/LICENSE.md
--rw-rw-rw-   0        0        0      109 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14553 2023-05-22 19:45:02.770763 socketlabs_injectionapi-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    13462 2023-05-22 19:44:22.000000 socketlabs_injectionapi-1.4.3/README.md
--rw-rw-rw-   0        0        0      369 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/app.json
--rw-rw-rw-   0        0        0       42 2023-05-22 19:45:02.771768 socketlabs_injectionapi-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1520 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.708000 socketlabs_injectionapi-1.4.3/socketlabs/
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.717519 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/
--rw-rw-rw-   0        0        0      142 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/__imports__.py
--rw-rw-rw-   0        0        0       84 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/__init__.py
--rw-rw-rw-   0        0        0     2856 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/addressresult.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.728895 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/
--rw-rw-rw-   0        0        0        2 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/__init__.py
--rw-rw-rw-   0        0        0     1552 2023-05-22 19:06:05.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/apikeyparser.py
--rw-rw-rw-   0        0        0     1669 2023-05-22 19:11:14.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/apikeyparseresult.py
--rw-rw-rw-   0        0        0      730 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/httpendpoint.py
--rw-rw-rw-   0        0        0     5953 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/httprequest.py
--rw-rw-rw-   0        0        0     9700 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/injectionrequestfactory.py
--rw-rw-rw-   0        0        0     3769 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/injectionresponseparser.py
--rw-rw-rw-   0        0        0     2944 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/retryhandler.py
--rw-rw-rw-   0        0        0    12976 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/sendvalidator.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.740698 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/__init__.py
--rw-rw-rw-   0        0        0     1955 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/addressjson.py
--rw-rw-rw-   0        0        0     3541 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/attachmentjson.py
--rw-rw-rw-   0        0        0     1570 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/customheaderjson.py
--rw-rw-rw-   0        0        0     1868 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/injectionrequest.py
--rw-rw-rw-   0        0        0     2776 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/injectionresponsedto.py
--rw-rw-rw-   0        0        0     2801 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/mergedatajson.py
--rw-rw-rw-   0        0        0     1560 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/mergefieldjson.py
--rw-rw-rw-   0        0        0    13585 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/messagejson.py
--rw-rw-rw-   0        0        0     2306 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/messageresultdto.py
--rw-rw-rw-   0        0        0     1479 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/metadatajson.py
--rw-rw-rw-   0        0        0     1756 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/stringextension.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.753224 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/
--rw-rw-rw-   0        0        0      304 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/__imports__.py
--rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/__init__.py
--rw-rw-rw-   0        0        0     7486 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/attachment.py
--rw-rw-rw-   0        0        0    15482 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/basicmessage.py
--rw-rw-rw-   0        0        0    14105 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/bulkmessage.py
--rw-rw-rw-   0        0        0     3277 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/bulkrecipient.py
--rw-rw-rw-   0        0        0     1991 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/customheader.py
--rw-rw-rw-   0        0        0     2168 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/emailaddress.py
--rw-rw-rw-   0        0        0     6322 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/messagebase.py
--rw-rw-rw-   0        0        0     1936 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/metadata.py
--rw-rw-rw-   0        0        0     1364 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/proxy.py
--rw-rw-rw-   0        0        0     1594 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/retrysettings.py
--rw-rw-rw-   0        0        0     4248 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/sendresponse.py
--rw-rw-rw-   0        0        0     7080 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/sendresult.py
--rw-rw-rw-   0        0        0    10977 2023-05-22 19:06:05.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/socketlabsclient.py
--rw-rw-rw-   0        0        0       80 2023-05-22 19:44:22.000000 socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/version.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:45:02.769758 socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/
--rw-rw-rw-   0        0        0    14553 2023-05-22 19:45:02.000000 socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2023-05-22 19:45:02.000000 socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:45:02.000000 socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 19:45:02.000000 socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.467984 socketlabs_injectionapi-1.4.4/
+-rw-rw-rw-   0        0        0     2324 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.4/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1086 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/LICENSE.md
+-rw-rw-rw-   0        0        0      109 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    14553 2023-07-28 14:59:49.466979 socketlabs_injectionapi-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13462 2023-05-22 19:44:22.000000 socketlabs_injectionapi-1.4.4/README.md
+-rw-rw-rw-   0        0        0      369 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/app.json
+-rw-rw-rw-   0        0        0       42 2023-07-28 14:59:49.467984 socketlabs_injectionapi-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1520 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.076021 socketlabs_injectionapi-1.4.4/socketlabs/
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.140023 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/
+-rw-rw-rw-   0        0        0      142 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/__imports__.py
+-rw-rw-rw-   0        0        0       84 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/__init__.py
+-rw-rw-rw-   0        0        0     2856 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/addressresult.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.215556 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/
+-rw-rw-rw-   0        0        0        2 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/__init__.py
+-rw-rw-rw-   0        0        0     1552 2023-05-22 19:06:05.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/apikeyparser.py
+-rw-rw-rw-   0        0        0     1669 2023-05-22 19:11:14.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/apikeyparseresult.py
+-rw-rw-rw-   0        0        0      807 2023-07-28 14:58:50.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/httpendpoint.py
+-rw-rw-rw-   0        0        0     5953 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/httprequest.py
+-rw-rw-rw-   0        0        0     9700 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/injectionrequestfactory.py
+-rw-rw-rw-   0        0        0     3769 2023-05-22 19:06:08.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/injectionresponseparser.py
+-rw-rw-rw-   0        0        0     2944 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/retryhandler.py
+-rw-rw-rw-   0        0        0    12976 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/sendvalidator.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.328911 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1955 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/addressjson.py
+-rw-rw-rw-   0        0        0     3541 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/attachmentjson.py
+-rw-rw-rw-   0        0        0     1570 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/customheaderjson.py
+-rw-rw-rw-   0        0        0     1868 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/injectionrequest.py
+-rw-rw-rw-   0        0        0     2776 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/injectionresponsedto.py
+-rw-rw-rw-   0        0        0     2801 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/mergedatajson.py
+-rw-rw-rw-   0        0        0     1560 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/mergefieldjson.py
+-rw-rw-rw-   0        0        0    13585 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/messagejson.py
+-rw-rw-rw-   0        0        0     2306 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/messageresultdto.py
+-rw-rw-rw-   0        0        0     1479 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/metadatajson.py
+-rw-rw-rw-   0        0        0     1756 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/stringextension.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.439448 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/
+-rw-rw-rw-   0        0        0      304 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/__imports__.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/__init__.py
+-rw-rw-rw-   0        0        0     7486 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/attachment.py
+-rw-rw-rw-   0        0        0    15482 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/basicmessage.py
+-rw-rw-rw-   0        0        0    14105 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/bulkmessage.py
+-rw-rw-rw-   0        0        0     3277 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/bulkrecipient.py
+-rw-rw-rw-   0        0        0     1991 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/customheader.py
+-rw-rw-rw-   0        0        0     2168 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/emailaddress.py
+-rw-rw-rw-   0        0        0     6322 2020-07-30 21:06:54.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/messagebase.py
+-rw-rw-rw-   0        0        0     1936 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/metadata.py
+-rw-rw-rw-   0        0        0     1364 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/proxy.py
+-rw-rw-rw-   0        0        0     1594 2021-04-13 19:49:12.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/retrysettings.py
+-rw-rw-rw-   0        0        0     4248 2020-07-09 15:06:38.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/sendresponse.py
+-rw-rw-rw-   0        0        0     7080 2023-05-22 19:05:57.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/sendresult.py
+-rw-rw-rw-   0        0        0    11324 2023-07-28 14:58:50.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/socketlabsclient.py
+-rw-rw-rw-   0        0        0       80 2023-07-28 14:58:50.000000 socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 14:59:49.464981 socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/
+-rw-rw-rw-   0        0        0    14553 2023-07-28 14:59:48.000000 socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2023-07-28 14:59:48.000000 socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 14:59:48.000000 socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 14:59:48.000000 socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/top_level.txt
```

### Comparing `socketlabs_injectionapi-1.4.3/CONTRIBUTING.md` & `socketlabs_injectionapi-1.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/LICENSE.md` & `socketlabs_injectionapi-1.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/PKG-INFO` & `socketlabs_injectionapi-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketlabs_injectionapi
-Version: 1.4.3
+Version: 1.4.4
 Summary: SocketLabs Email Delivery Python client library
 Home-page: https://github.com/socketlabs/socketlabs-python
 Author: David Schrenker, Matt Reibach, Ryan Lydzinski, Praneeth Chandra
 Author-email: support@socketlabs.com
 License: MIT
 Project-URL: Organization, https://github.com/socketlabs
 Project-URL: Bug Reports, https://github.com/socketlabs/socketlabs-python/issues
```

### Comparing `socketlabs_injectionapi-1.4.3/README.md` & `socketlabs_injectionapi-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/setup.py` & `socketlabs_injectionapi-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/addressresult.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/addressresult.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/apikeyparser.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/apikeyparser.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/apikeyparseresult.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/apikeyparseresult.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/httpendpoint.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/httpendpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from urllib.parse import urlparse
+
 class HttpEndpoint(object):
     """
     The HTTP endpoint
     """
 
-    def __init__(self, host: str = None, url: str = None):
+    def __init__(self, url: str):
         """
         Create an instance of the HttpEndpoint class
         :param host: the host name
         :type host: str
         :param url: the url
         :type url: str
         """
-        self._host = host
-        self._url = url
+        parsed_url = urlparse(url)
+        self._host = parsed_url.hostname
+        self._url = parsed_url.path
+
 
     @property
     def url(self):
         """
         Get the HTTP endpoint Url
         :return the url
         :rtype str
```

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/httprequest.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/httprequest.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/injectionrequestfactory.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/injectionrequestfactory.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/injectionresponseparser.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/injectionresponseparser.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/retryhandler.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/retryhandler.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/sendvalidator.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/sendvalidator.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/addressjson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/addressjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/attachmentjson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/attachmentjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/customheaderjson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/customheaderjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/injectionrequest.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/injectionrequest.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/injectionresponsedto.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/injectionresponsedto.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/mergedatajson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/mergedatajson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/mergefieldjson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/mergefieldjson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/messagejson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/messagejson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/messageresultdto.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/messageresultdto.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/serialization/metadatajson.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/serialization/metadatajson.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/core/stringextension.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/core/stringextension.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/attachment.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/attachment.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/basicmessage.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/basicmessage.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/bulkmessage.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/bulkmessage.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/bulkrecipient.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/bulkrecipient.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/customheader.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/customheader.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/emailaddress.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/emailaddress.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/messagebase.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/messagebase.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/message/metadata.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/message/metadata.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/proxy.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/proxy.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/retrysettings.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/retrysettings.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/sendresponse.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/sendresponse.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/sendresult.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/sendresult.py`

 * *Files identical despite different names*

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs/injectionapi/socketlabsclient.py` & `socketlabs_injectionapi-1.4.4/socketlabs/injectionapi/socketlabsclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,33 @@
         :type proxy: str
         """
         self._server_id = server_id
         self._api_key = api_key
         self._http_proxy = proxy
         self._request_timeout = 120
         self._number_of_retries = 0
+        self._http_endpoint = "https://inject.socketlabs.com/api/v1/email"
 
     @property
-    def __endpoint(self):
+    def endpoint(self):
         """
         The SocketLabs Injection API endpoint
         :return the Http Endpoint for the request
         :rtype HttpEndpoint
         """
-        return HttpEndpoint("inject.socketlabs.com", "/api/v1/email")
+        return self._http_endpoint
+
+    @endpoint.setter
+    def endpoint(self, http_endpoint: str):
+        """
+        The SocketLabs Injection API endpoint
+        :return the Http Endpoint for the request
+        :rtype HttpEndpoint
+        """
+        self._http_endpoint = http_endpoint
 
     @property
     def __proxy(self):
         """
         The Proxy you would like to use.
         :return the optional proxy to use for the request
         :rtype Proxy
@@ -87,15 +97,16 @@
         """
         Build the HttpRequest. Will add the proxy, if set
         :param authentication: the API key to include as a bearer token
         :type authentication: object
         :return the HttpRequest object to use for the request
         :rtype HttpRequest
         """
-        req = HttpRequest(HttpRequest.HttpRequestMethod.POST, self.__endpoint, self.request_timeout, authentication)
+        endpoint = HttpEndpoint(self.endpoint)
+        req = HttpRequest(HttpRequest.HttpRequestMethod.POST, endpoint, self.request_timeout, authentication)
         if self._http_proxy is not None:
             req.proxy = self._http_proxy
         return req
 
     def send(self, message):
         """
         Sends a BasicMessage message and returns the response from the Injection API.
```

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/PKG-INFO` & `socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketlabs-injectionapi
-Version: 1.4.3
+Version: 1.4.4
 Summary: SocketLabs Email Delivery Python client library
 Home-page: https://github.com/socketlabs/socketlabs-python
 Author: David Schrenker, Matt Reibach, Ryan Lydzinski, Praneeth Chandra
 Author-email: support@socketlabs.com
 License: MIT
 Project-URL: Organization, https://github.com/socketlabs
 Project-URL: Bug Reports, https://github.com/socketlabs/socketlabs-python/issues
```

### Comparing `socketlabs_injectionapi-1.4.3/socketlabs_injectionapi.egg-info/SOURCES.txt` & `socketlabs_injectionapi-1.4.4/socketlabs_injectionapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

