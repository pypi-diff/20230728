# Comparing `tmp/tap_googleads-0.1.5.tar.gz` & `tmp/tap_googleads-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_googleads-0.1.5.tar", max compression
+gzip compressed data, was "tap_googleads-0.1.6.tar", max compression
```

## Comparing `tap_googleads-0.1.5.tar` & `tap_googleads-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      718 2023-07-26 16:07:00.181819 tap_googleads-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-06 18:20:33.330671 tap_googleads-0.1.5/tap_googleads/__init__.py
--rw-r--r--   0        0        0      539 2023-01-06 18:20:33.330671 tap_googleads-0.1.5/tap_googleads/auth.py
--rw-r--r--   0        0        0     5400 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/client.py
--rw-r--r--   0        0        0     2238 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/ad_group.json
--rw-r--r--   0        0        0     1218 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/ad_group_performance.json
--rw-r--r--   0        0        0      477 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign.json
--rw-r--r--   0        0        0     1640 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_label.json
--rw-r--r--   0        0        0     1659 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance.json
--rw-r--r--   0        0        0     2309 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json
--rw-r--r--   0        0        0     2305 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_gender_and_device.json
--rw-r--r--   0        0        0     1780 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_location.json
--rw-r--r--   0        0        0     1541 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/conversion_by_location.json
--rw-r--r--   0        0        0     1659 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/customer.json
--rw-r--r--   0        0        0     1682 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/schemas/customer_hierarchy.json
--rw-r--r--   0        0        0      838 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/schemas/geo_target_constant.json
--rw-r--r--   0        0        0    15532 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/streams.py
--rw-r--r--   0        0        0     3432 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tap.py
--rw-r--r--   0        0        0       36 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/tests/__init__.py
--rw-r--r--   0        0        0      711 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tests/test_core.py
--rw-r--r--   0        0        0     3314 2023-07-26 16:06:23.011371 tap_googleads-0.1.5/tap_googleads/tests/test_customer_not_found.py
--rw-r--r--   0        0        0      733 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/tests/test_utils.py
--rw-r--r--   0        0        0      982 2023-01-06 18:20:33.340671 tap_googleads-0.1.5/tap_googleads/utils.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 tap_googleads-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      718 2023-07-28 20:58:23.698739 tap_googleads-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 15:56:11.893149 tap_googleads-0.1.6/tap_googleads/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-21 15:56:11.893149 tap_googleads-0.1.6/tap_googleads/auth.py
+-rw-r--r--   0        0        0     5400 2023-07-28 18:08:13.202238 tap_googleads-0.1.6/tap_googleads/client.py
+-rw-r--r--   0        0        0     2238 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/ad_group.json
+-rw-r--r--   0        0        0     1218 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/ad_group_performance.json
+-rw-r--r--   0        0        0      477 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/campaign.json
+-rw-r--r--   0        0        0     1640 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/campaign_label.json
+-rw-r--r--   0        0        0     1748 2023-07-28 20:53:53.028832 tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance.json
+-rw-r--r--   0        0        0     2309 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json
+-rw-r--r--   0        0        0     2305 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_gender_and_device.json
+-rw-r--r--   0        0        0     1780 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_location.json
+-rw-r--r--   0        0        0     1541 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/conversion_by_location.json
+-rw-r--r--   0        0        0     1659 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/customer.json
+-rw-r--r--   0        0        0     1682 2023-07-28 18:08:13.202238 tap_googleads-0.1.6/tap_googleads/schemas/customer_hierarchy.json
+-rw-r--r--   0        0        0      838 2023-07-28 18:05:45.252305 tap_googleads-0.1.6/tap_googleads/schemas/geo_target_constant.json
+-rw-r--r--   0        0        0    15571 2023-07-28 20:53:53.028832 tap_googleads-0.1.6/tap_googleads/streams.py
+-rw-r--r--   0        0        0     3432 2023-07-28 18:08:13.202238 tap_googleads-0.1.6/tap_googleads/tap.py
+-rw-r--r--   0        0        0       36 2023-07-21 15:56:11.903149 tap_googleads-0.1.6/tap_googleads/tests/__init__.py
+-rw-r--r--   0        0        0      721 2023-07-28 20:53:53.028832 tap_googleads-0.1.6/tap_googleads/tests/test_core.py
+-rw-r--r--   0        0        0     3324 2023-07-28 20:53:53.028832 tap_googleads-0.1.6/tap_googleads/tests/test_customer_not_found.py
+-rw-r--r--   0        0        0      733 2023-07-21 15:56:11.903149 tap_googleads-0.1.6/tap_googleads/tests/test_utils.py
+-rw-r--r--   0        0        0      982 2023-07-21 15:56:11.903149 tap_googleads-0.1.6/tap_googleads/utils.py
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 tap_googleads-0.1.6/PKG-INFO
```

### Comparing `tap_googleads-0.1.5/pyproject.toml` & `tap_googleads-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-googleads"
-version = "0.1.5"
+version = "0.1.6"
 description = "`tap-googleads` is a Singer tap for GoogleAds, built with the Meltano SDK for Singer Taps."
 authors = ["AutoIDM"]
 keywords = [
     "ELT",
     "GoogleAds",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_googleads-0.1.5/tap_googleads/auth.py` & `tap_googleads-0.1.6/tap_googleads/auth.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/client.py` & `tap_googleads-0.1.6/tap_googleads/client.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/ad_group.json` & `tap_googleads-0.1.6/tap_googleads/schemas/ad_group.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/ad_group_performance.json` & `tap_googleads-0.1.6/tap_googleads/schemas/ad_group_performance.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/campaign_label.json` & `tap_googleads-0.1.6/tap_googleads/schemas/campaign_label.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance.json` & `tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666667%*

 * *Differences: {"'properties'": "{'metrics': {'properties': {'conversions': OrderedDict([('type', 'number')])}}}"}*

```diff
@@ -33,14 +33,17 @@
             "properties": {
                 "averageCpc": {
                     "type": "number"
                 },
                 "clicks": {
                     "type": "string"
                 },
+                "conversions": {
+                    "type": "number"
+                },
                 "costMicros": {
                     "type": "string"
                 },
                 "ctr": {
                     "type": "number"
                 },
                 "impressions": {
```

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json` & `tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_age_range_and_device.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_gender_and_device.json` & `tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_gender_and_device.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/campaign_performance_by_location.json` & `tap_googleads-0.1.6/tap_googleads/schemas/campaign_performance_by_location.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/conversion_by_location.json` & `tap_googleads-0.1.6/tap_googleads/schemas/conversion_by_location.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/customer.json` & `tap_googleads-0.1.6/tap_googleads/schemas/customer.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/customer_hierarchy.json` & `tap_googleads-0.1.6/tap_googleads/schemas/customer_hierarchy.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/schemas/geo_target_constant.json` & `tap_googleads-0.1.6/tap_googleads/schemas/geo_target_constant.json`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/streams.py` & `tap_googleads-0.1.6/tap_googleads/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,15 @@
                  , campaign.status
                  , campaign.start_date
                  , campaign.end_date
                  , campaign.advertising_channel_type
                  , campaign.advertising_channel_sub_type
                  , segments.device
                  , segments.date
+                 , metrics.conversions
                  , metrics.impressions
                  , metrics.clicks
                  , metrics.ctr
                  , metrics.average_cpc
                  , metrics.cost_micros 
             FROM campaign 
             WHERE segments.date {self.between_filter}
```

### Comparing `tap_googleads-0.1.5/tap_googleads/tap.py` & `tap_googleads-0.1.6/tap_googleads/tap.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/tests/test_core.py` & `tap_googleads-0.1.6/tap_googleads/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 
 from singer_sdk.testing import get_standard_tap_tests
 from tap_googleads.tap import TapGoogleAds
 
 
 SAMPLE_CONFIG = {
-    "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d"),
+    "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ"),
     "client_id": "12345",
     "client_secret": "12345",
     "developer_token": "12345",
     "refresh_token": "12345",
     "customer_id": "12345",
     "login_customer_id": "12345",
 }
```

### Comparing `tap_googleads-0.1.5/tap_googleads/tests/test_customer_not_found.py` & `tap_googleads-0.1.6/tap_googleads/tests/test_customer_not_found.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tap_googleads.tap
 import pytest
 import json
 
 import responses
 
 SAMPLE_CONFIG = {
-    "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d"),
+    "start_date": datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ"),
     "client_id": "12345",
     "client_secret": "12345",
     "developer_token": "12345",
     "refresh_token": "12345",
     "customer_id": "12345",
     "login_customer_id": "12345",
 }
```

### Comparing `tap_googleads-0.1.5/tap_googleads/tests/test_utils.py` & `tap_googleads-0.1.6/tap_googleads/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/tap_googleads/utils.py` & `tap_googleads-0.1.6/tap_googleads/utils.py`

 * *Files identical despite different names*

### Comparing `tap_googleads-0.1.5/PKG-INFO` & `tap_googleads-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-googleads
-Version: 0.1.5
+Version: 0.1.6
 Summary: `tap-googleads` is a Singer tap for GoogleAds, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,GoogleAds
 Author: AutoIDM
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

