# Comparing `tmp/alibabacloud_dingtalk-2.0.27.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.27.tar", last modified: Wed Jul 26 02:26:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.28.tar", last modified: Fri Jul 28 02:23:10 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.27.tar` & `alibabacloud_dingtalk-2.0.28.tar`

### file list

```diff
@@ -1,381 +1,385 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/
--rw-r--r--   0 root         (0) root         (0)    20402 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   205984 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   590436 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106288 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23872 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33155 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    75811 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97319 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   141560 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33901 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106806 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65686 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   381194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   542779 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19158 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32757 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/
+-rw-r--r--   0 root         (0) root         (0)    20467 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   205984 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   590436 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   485844 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   747999 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97319 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   141560 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33901 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106806 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65686 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92278 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   381194 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   542779 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12717 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-07-28 02:23:10.000000 alibabacloud_dingtalk-2.0.28/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.27/ChangeLog.md` & `alibabacloud_dingtalk-2.0.28/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-26 Version: 2.0.27
+- Update AddOfficialAccountFollower.
+
 2023-07-21 Version: 2.0.26
 - Update AddOfficialAccountFollower.
 
 2023-07-19 Version: 2.0.25
 - Update AddOfficialAccountFollower.
 
 2023-07-17 Version: 2.0.24
```

### Comparing `alibabacloud_dingtalk-2.0.27/LICENSE` & `alibabacloud_dingtalk-2.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/PKG-INFO` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dingtalk
-Version: 2.0.27
+Name: alibabacloud-dingtalk
+Version: 2.0.28
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.27/README-CN.md` & `alibabacloud_dingtalk-2.0.28/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/README.md` & `alibabacloud_dingtalk-2.0.28/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,116 @@
         self,
         request: dingtalkedu__1__0_models.AddSchoolConfigRequest,
     ) -> dingtalkedu__1__0_models.AddSchoolConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.AddSchoolConfigHeaders()
         return await self.add_school_config_with_options_async(request, headers, runtime)
 
+    def assign_class_with_options(
+        self,
+        request: dingtalkedu__1__0_models.AssignClassRequest,
+        headers: dingtalkedu__1__0_models.AssignClassHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.AssignClassResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.class_id):
+            body['classId'] = request.class_id
+        if not UtilClient.is_unset(request.is_finish):
+            body['isFinish'] = request.is_finish
+        if not UtilClient.is_unset(request.operator):
+            body['operator'] = request.operator
+        if not UtilClient.is_unset(request.student_id):
+            body['studentId'] = request.student_id
+        if not UtilClient.is_unset(request.task_id):
+            body['taskId'] = request.task_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AssignClass',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/students/classes/assign',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.AssignClassResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def assign_class_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.AssignClassRequest,
+        headers: dingtalkedu__1__0_models.AssignClassHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.AssignClassResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.class_id):
+            body['classId'] = request.class_id
+        if not UtilClient.is_unset(request.is_finish):
+            body['isFinish'] = request.is_finish
+        if not UtilClient.is_unset(request.operator):
+            body['operator'] = request.operator
+        if not UtilClient.is_unset(request.student_id):
+            body['studentId'] = request.student_id
+        if not UtilClient.is_unset(request.task_id):
+            body['taskId'] = request.task_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AssignClass',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/students/classes/assign',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.AssignClassResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def assign_class(
+        self,
+        request: dingtalkedu__1__0_models.AssignClassRequest,
+    ) -> dingtalkedu__1__0_models.AssignClassResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.AssignClassHeaders()
+        return self.assign_class_with_options(request, headers, runtime)
+
+    async def assign_class_async(
+        self,
+        request: dingtalkedu__1__0_models.AssignClassRequest,
+    ) -> dingtalkedu__1__0_models.AssignClassResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.AssignClassHeaders()
+        return await self.assign_class_with_options_async(request, headers, runtime)
+
     def batch_create_with_options(
         self,
         request: dingtalkedu__1__0_models.BatchCreateRequest,
         headers: dingtalkedu__1__0_models.BatchCreateHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.BatchCreateResponse:
         UtilClient.validate_model(request)
@@ -5691,14 +5793,210 @@
         return self.get_share_roles_with_options(headers, runtime)
 
     async def get_share_roles_async(self) -> dingtalkedu__1__0_models.GetShareRolesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkedu__1__0_models.GetShareRolesHeaders()
         return await self.get_share_roles_with_options_async(headers, runtime)
 
+    def get_task_list_with_options(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskListRequest,
+        headers: dingtalkedu__1__0_models.GetTaskListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetTaskListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator):
+            query['operator'] = request.operator
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_year):
+            query['taskYear'] = request.task_year
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTaskList',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/lists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetTaskListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_task_list_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskListRequest,
+        headers: dingtalkedu__1__0_models.GetTaskListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetTaskListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator):
+            query['operator'] = request.operator
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_year):
+            query['taskYear'] = request.task_year
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTaskList',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/lists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetTaskListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_task_list(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskListRequest,
+    ) -> dingtalkedu__1__0_models.GetTaskListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetTaskListHeaders()
+        return self.get_task_list_with_options(request, headers, runtime)
+
+    async def get_task_list_async(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskListRequest,
+    ) -> dingtalkedu__1__0_models.GetTaskListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetTaskListHeaders()
+        return await self.get_task_list_with_options_async(request, headers, runtime)
+
+    def get_task_student_list_with_options(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskStudentListRequest,
+        headers: dingtalkedu__1__0_models.GetTaskStudentListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetTaskStudentListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator):
+            query['operator'] = request.operator
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_id):
+            query['taskId'] = request.task_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTaskStudentList',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/students/lists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetTaskStudentListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_task_student_list_with_options_async(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskStudentListRequest,
+        headers: dingtalkedu__1__0_models.GetTaskStudentListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkedu__1__0_models.GetTaskStudentListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator):
+            query['operator'] = request.operator
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.task_id):
+            query['taskId'] = request.task_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetTaskStudentList',
+            version='edu_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/edu/newGrades/tasks/students/lists',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkedu__1__0_models.GetTaskStudentListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_task_student_list(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskStudentListRequest,
+    ) -> dingtalkedu__1__0_models.GetTaskStudentListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetTaskStudentListHeaders()
+        return self.get_task_student_list_with_options(request, headers, runtime)
+
+    async def get_task_student_list_async(
+        self,
+        request: dingtalkedu__1__0_models.GetTaskStudentListRequest,
+    ) -> dingtalkedu__1__0_models.GetTaskStudentListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkedu__1__0_models.GetTaskStudentListHeaders()
+        return await self.get_task_student_list_with_options_async(request, headers, runtime)
+
     def init_courses_of_class_with_options(
         self,
         class_id: str,
         request: dingtalkedu__1__0_models.InitCoursesOfClassRequest,
         headers: dingtalkedu__1__0_models.InitCoursesOfClassHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkedu__1__0_models.InitCoursesOfClassResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,14 +489,169 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddSchoolConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AssignClassHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class AssignClassRequest(TeaModel):
+    def __init__(
+        self,
+        class_id: int = None,
+        is_finish: bool = None,
+        operator: str = None,
+        student_id: int = None,
+        task_id: int = None,
+    ):
+        self.class_id = class_id
+        self.is_finish = is_finish
+        self.operator = operator
+        self.student_id = student_id
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.class_id is not None:
+            result['classId'] = self.class_id
+        if self.is_finish is not None:
+            result['isFinish'] = self.is_finish
+        if self.operator is not None:
+            result['operator'] = self.operator
+        if self.student_id is not None:
+            result['studentId'] = self.student_id
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('classId') is not None:
+            self.class_id = m.get('classId')
+        if m.get('isFinish') is not None:
+            self.is_finish = m.get('isFinish')
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        if m.get('studentId') is not None:
+            self.student_id = m.get('studentId')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class AssignClassResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class AssignClassResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AssignClassResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AssignClassResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchCreateHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -11380,14 +11535,424 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetShareRolesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTaskListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetTaskListRequest(TeaModel):
+    def __init__(
+        self,
+        operator: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        task_year: int = None,
+    ):
+        self.operator = operator
+        self.page_number = page_number
+        self.page_size = page_size
+        self.task_year = task_year
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator is not None:
+            result['operator'] = self.operator
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.task_year is not None:
+            result['taskYear'] = self.task_year
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('taskYear') is not None:
+            self.task_year = m.get('taskYear')
+        return self
+
+
+class GetTaskListResponseBodyTaskList(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        task_id: int = None,
+        task_year: int = None,
+    ):
+        self.name = name
+        self.task_id = task_id
+        self.task_year = task_year
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        if self.task_year is not None:
+            result['taskYear'] = self.task_year
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        if m.get('taskYear') is not None:
+            self.task_year = m.get('taskYear')
+        return self
+
+
+class GetTaskListResponseBody(TeaModel):
+    def __init__(
+        self,
+        count: int = None,
+        task_list: List[GetTaskListResponseBodyTaskList] = None,
+    ):
+        self.count = count
+        self.task_list = task_list
+
+    def validate(self):
+        if self.task_list:
+            for k in self.task_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.count is not None:
+            result['count'] = self.count
+        result['taskList'] = []
+        if self.task_list is not None:
+            for k in self.task_list:
+                result['taskList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('count') is not None:
+            self.count = m.get('count')
+        self.task_list = []
+        if m.get('taskList') is not None:
+            for k in m.get('taskList'):
+                temp_model = GetTaskListResponseBodyTaskList()
+                self.task_list.append(temp_model.from_map(k))
+        return self
+
+
+class GetTaskListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTaskListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetTaskListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetTaskStudentListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetTaskStudentListRequest(TeaModel):
+    def __init__(
+        self,
+        operator: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        task_id: int = None,
+    ):
+        self.operator = operator
+        self.page_number = page_number
+        self.page_size = page_size
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator is not None:
+            result['operator'] = self.operator
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class GetTaskStudentListResponseBodyStudentList(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        sexuality: str = None,
+        student_id: int = None,
+    ):
+        self.name = name
+        self.sexuality = sexuality
+        self.student_id = student_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.sexuality is not None:
+            result['sexuality'] = self.sexuality
+        if self.student_id is not None:
+            result['studentId'] = self.student_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('sexuality') is not None:
+            self.sexuality = m.get('sexuality')
+        if m.get('studentId') is not None:
+            self.student_id = m.get('studentId')
+        return self
+
+
+class GetTaskStudentListResponseBody(TeaModel):
+    def __init__(
+        self,
+        count: int = None,
+        student_list: List[GetTaskStudentListResponseBodyStudentList] = None,
+        task_id: int = None,
+    ):
+        self.count = count
+        self.student_list = student_list
+        self.task_id = task_id
+
+    def validate(self):
+        if self.student_list:
+            for k in self.student_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.count is not None:
+            result['count'] = self.count
+        result['studentList'] = []
+        if self.student_list is not None:
+            for k in self.student_list:
+                result['studentList'].append(k.to_map() if k else None)
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('count') is not None:
+            self.count = m.get('count')
+        self.student_list = []
+        if m.get('studentList') is not None:
+            for k in m.get('studentList'):
+                temp_model = GetTaskStudentListResponseBodyStudentList()
+                self.student_list.append(temp_model.from_map(k))
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class GetTaskStudentListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTaskStudentListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetTaskStudentListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class InitCoursesOfClassHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.28/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dingtalk
-Version: 2.0.27
+Name: alibabacloud_dingtalk
+Version: 2.0.28
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.28/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 alibabacloud_dingtalk/ats_1_0/models.py
 alibabacloud_dingtalk/attendance_1_0/__init__.py
 alibabacloud_dingtalk/attendance_1_0/client.py
 alibabacloud_dingtalk/attendance_1_0/models.py
 alibabacloud_dingtalk/badge_1_0/__init__.py
 alibabacloud_dingtalk/badge_1_0/client.py
 alibabacloud_dingtalk/badge_1_0/models.py
+alibabacloud_dingtalk/bay_max_1_0/__init__.py
+alibabacloud_dingtalk/bay_max_1_0/client.py
+alibabacloud_dingtalk/bay_max_1_0/models.py
 alibabacloud_dingtalk/bizfinance_1_0/__init__.py
 alibabacloud_dingtalk/bizfinance_1_0/client.py
 alibabacloud_dingtalk/bizfinance_1_0/models.py
 alibabacloud_dingtalk/blackboard_1_0/__init__.py
 alibabacloud_dingtalk/blackboard_1_0/client.py
 alibabacloud_dingtalk/blackboard_1_0/models.py
 alibabacloud_dingtalk/calendar_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.27/setup.py` & `alibabacloud_dingtalk-2.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 26/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

