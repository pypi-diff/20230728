# Comparing `tmp/pulumi_splunk-1.3.0a1690264914.tar.gz` & `tmp/pulumi_splunk-1.3.0a1690564639.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1690264914.tar", last modified: Tue Jul 25 06:12:54 2023, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1690564639.tar", last modified: Fri Jul 28 17:21:32 2023, max compression
```

## Comparing `pulumi_splunk-1.3.0a1690264914.tar` & `pulumi_splunk-1.3.0a1690564639.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   506277 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:12:54.324838 pulumi_splunk-1.3.0a1690264914/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-25 06:12:54.000000 pulumi_splunk-1.3.0a1690264914/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90731 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38600 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45752 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154784 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42002 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29483 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18863 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73136 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43975 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   514411 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:21:32.451825 pulumi_splunk-1.3.0a1690564639/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-28 17:21:32.000000 pulumi_splunk-1.3.0a1690564639/setup.py
```

### Comparing `pulumi_splunk-1.3.0a1690264914/PKG-INFO` & `pulumi_splunk-1.3.0a1690564639/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1690264914
+Version: 1.3.0a1690564639
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_splunk-1.3.0a1690264914/README.md` & `pulumi_splunk-1.3.0a1690564639/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/configs_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/saved_searches.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_custom_details: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key_override: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
@@ -227,14 +230,17 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_custom_details: The PagerDuty custom details information.
+        :param pulumi.Input[str] action_pagerduty_integration_key: The PagerDuty integration Key.
+        :param pulumi.Input[str] action_pagerduty_integration_key_override: The PagerDuty integration Key override.
         :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
@@ -450,14 +456,20 @@
             pulumi.set(__self__, "action_jira_service_desk_param_jira_issue_type", action_jira_service_desk_param_jira_issue_type)
         if action_jira_service_desk_param_jira_priority is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_priority", action_jira_service_desk_param_jira_priority)
         if action_jira_service_desk_param_jira_project is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_project", action_jira_service_desk_param_jira_project)
         if action_jira_service_desk_param_jira_summary is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_summary", action_jira_service_desk_param_jira_summary)
+        if action_pagerduty_custom_details is not None:
+            pulumi.set(__self__, "action_pagerduty_custom_details", action_pagerduty_custom_details)
+        if action_pagerduty_integration_key is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_key", action_pagerduty_integration_key)
+        if action_pagerduty_integration_key_override is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_key_override", action_pagerduty_integration_key_override)
         if action_pagerduty_integration_url is not None:
             pulumi.set(__self__, "action_pagerduty_integration_url", action_pagerduty_integration_url)
         if action_pagerduty_integration_url_override is not None:
             pulumi.set(__self__, "action_pagerduty_integration_url_override", action_pagerduty_integration_url_override)
         if action_populate_lookup_command is not None:
             pulumi.set(__self__, "action_populate_lookup_command", action_populate_lookup_command)
         if action_populate_lookup_dest is not None:
@@ -1310,14 +1322,50 @@
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @action_jira_service_desk_param_jira_summary.setter
     def action_jira_service_desk_param_jira_summary(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action_jira_service_desk_param_jira_summary", value)
 
     @property
+    @pulumi.getter(name="actionPagerdutyCustomDetails")
+    def action_pagerduty_custom_details(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty custom details information.
+        """
+        return pulumi.get(self, "action_pagerduty_custom_details")
+
+    @action_pagerduty_custom_details.setter
+    def action_pagerduty_custom_details(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_custom_details", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKey")
+    def action_pagerduty_integration_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty integration Key.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key")
+
+    @action_pagerduty_integration_key.setter
+    def action_pagerduty_integration_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_key", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKeyOverride")
+    def action_pagerduty_integration_key_override(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty integration Key override.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key_override")
+
+    @action_pagerduty_integration_key_override.setter
+    def action_pagerduty_integration_key_override(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_key_override", value)
+
+    @property
     @pulumi.getter(name="actionPagerdutyIntegrationUrl")
     def action_pagerduty_integration_url(self) -> Optional[pulumi.Input[str]]:
         """
         The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         """
         return pulumi.get(self, "action_pagerduty_integration_url")
 
@@ -2637,14 +2685,17 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_custom_details: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key_override: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup: Optional[pulumi.Input[bool]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
@@ -2803,14 +2854,17 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_custom_details: The PagerDuty custom details information.
+        :param pulumi.Input[str] action_pagerduty_integration_key: The PagerDuty integration Key.
+        :param pulumi.Input[str] action_pagerduty_integration_key_override: The PagerDuty integration Key override.
         :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[bool] action_populate_lookup: The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
@@ -3032,14 +3086,20 @@
             pulumi.set(__self__, "action_jira_service_desk_param_jira_issue_type", action_jira_service_desk_param_jira_issue_type)
         if action_jira_service_desk_param_jira_priority is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_priority", action_jira_service_desk_param_jira_priority)
         if action_jira_service_desk_param_jira_project is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_project", action_jira_service_desk_param_jira_project)
         if action_jira_service_desk_param_jira_summary is not None:
             pulumi.set(__self__, "action_jira_service_desk_param_jira_summary", action_jira_service_desk_param_jira_summary)
+        if action_pagerduty_custom_details is not None:
+            pulumi.set(__self__, "action_pagerduty_custom_details", action_pagerduty_custom_details)
+        if action_pagerduty_integration_key is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_key", action_pagerduty_integration_key)
+        if action_pagerduty_integration_key_override is not None:
+            pulumi.set(__self__, "action_pagerduty_integration_key_override", action_pagerduty_integration_key_override)
         if action_pagerduty_integration_url is not None:
             pulumi.set(__self__, "action_pagerduty_integration_url", action_pagerduty_integration_url)
         if action_pagerduty_integration_url_override is not None:
             pulumi.set(__self__, "action_pagerduty_integration_url_override", action_pagerduty_integration_url_override)
         if action_populate_lookup is not None:
             pulumi.set(__self__, "action_populate_lookup", action_populate_lookup)
         if action_populate_lookup_command is not None:
@@ -3902,14 +3962,50 @@
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @action_jira_service_desk_param_jira_summary.setter
     def action_jira_service_desk_param_jira_summary(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action_jira_service_desk_param_jira_summary", value)
 
     @property
+    @pulumi.getter(name="actionPagerdutyCustomDetails")
+    def action_pagerduty_custom_details(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty custom details information.
+        """
+        return pulumi.get(self, "action_pagerduty_custom_details")
+
+    @action_pagerduty_custom_details.setter
+    def action_pagerduty_custom_details(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_custom_details", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKey")
+    def action_pagerduty_integration_key(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty integration Key.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key")
+
+    @action_pagerduty_integration_key.setter
+    def action_pagerduty_integration_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_key", value)
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKeyOverride")
+    def action_pagerduty_integration_key_override(self) -> Optional[pulumi.Input[str]]:
+        """
+        The PagerDuty integration Key override.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key_override")
+
+    @action_pagerduty_integration_key_override.setter
+    def action_pagerduty_integration_key_override(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action_pagerduty_integration_key_override", value)
+
+    @property
     @pulumi.getter(name="actionPagerdutyIntegrationUrl")
     def action_pagerduty_integration_url(self) -> Optional[pulumi.Input[str]]:
         """
         The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         """
         return pulumi.get(self, "action_pagerduty_integration_url")
 
@@ -5290,14 +5386,17 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_custom_details: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key_override: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
@@ -5483,14 +5582,17 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_custom_details: The PagerDuty custom details information.
+        :param pulumi.Input[str] action_pagerduty_integration_key: The PagerDuty integration Key.
+        :param pulumi.Input[str] action_pagerduty_integration_key_override: The PagerDuty integration Key override.
         :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
         :param pulumi.Input[int] action_populate_lookup_max_time: Valid values are: Integer[m|s|h|d]Sets the maximum amount of time the execution of an action takes before the action is aborted. Defaults to 5m.
@@ -5705,14 +5807,17 @@
                  action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
                  action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
                  action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_custom_details: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key: Optional[pulumi.Input[str]] = None,
+                 action_pagerduty_integration_key_override: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
                  action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
                  action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
                  action_populate_lookup_max_time: Optional[pulumi.Input[int]] = None,
@@ -5873,14 +5978,17 @@
             __props__.__dict__["action_email_width_sort_columns"] = action_email_width_sort_columns
             __props__.__dict__["action_jira_service_desk_param_account"] = action_jira_service_desk_param_account
             __props__.__dict__["action_jira_service_desk_param_jira_description"] = action_jira_service_desk_param_jira_description
             __props__.__dict__["action_jira_service_desk_param_jira_issue_type"] = action_jira_service_desk_param_jira_issue_type
             __props__.__dict__["action_jira_service_desk_param_jira_priority"] = action_jira_service_desk_param_jira_priority
             __props__.__dict__["action_jira_service_desk_param_jira_project"] = action_jira_service_desk_param_jira_project
             __props__.__dict__["action_jira_service_desk_param_jira_summary"] = action_jira_service_desk_param_jira_summary
+            __props__.__dict__["action_pagerduty_custom_details"] = action_pagerduty_custom_details
+            __props__.__dict__["action_pagerduty_integration_key"] = action_pagerduty_integration_key
+            __props__.__dict__["action_pagerduty_integration_key_override"] = action_pagerduty_integration_key_override
             __props__.__dict__["action_pagerduty_integration_url"] = action_pagerduty_integration_url
             __props__.__dict__["action_pagerduty_integration_url_override"] = action_pagerduty_integration_url_override
             __props__.__dict__["action_populate_lookup_command"] = action_populate_lookup_command
             __props__.__dict__["action_populate_lookup_dest"] = action_populate_lookup_dest
             __props__.__dict__["action_populate_lookup_hostname"] = action_populate_lookup_hostname
             __props__.__dict__["action_populate_lookup_max_results"] = action_populate_lookup_max_results
             __props__.__dict__["action_populate_lookup_max_time"] = action_populate_lookup_max_time
@@ -6050,14 +6158,17 @@
             action_email_width_sort_columns: Optional[pulumi.Input[bool]] = None,
             action_jira_service_desk_param_account: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_description: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_issue_type: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_priority: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_project: Optional[pulumi.Input[str]] = None,
             action_jira_service_desk_param_jira_summary: Optional[pulumi.Input[str]] = None,
+            action_pagerduty_custom_details: Optional[pulumi.Input[str]] = None,
+            action_pagerduty_integration_key: Optional[pulumi.Input[str]] = None,
+            action_pagerduty_integration_key_override: Optional[pulumi.Input[str]] = None,
             action_pagerduty_integration_url: Optional[pulumi.Input[str]] = None,
             action_pagerduty_integration_url_override: Optional[pulumi.Input[str]] = None,
             action_populate_lookup: Optional[pulumi.Input[bool]] = None,
             action_populate_lookup_command: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_dest: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_hostname: Optional[pulumi.Input[str]] = None,
             action_populate_lookup_max_results: Optional[pulumi.Input[int]] = None,
@@ -6221,14 +6332,17 @@
         :param pulumi.Input[bool] action_email_width_sort_columns: Indicates whether columns should be sorted from least wide to most wide, left to right.Only valid if format=text.
         :param pulumi.Input[str] action_jira_service_desk_param_account: Jira Service Desk account name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_description: Jira issue description
         :param pulumi.Input[str] action_jira_service_desk_param_jira_issue_type: Jira issue type name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_priority: Jira priority of issue
         :param pulumi.Input[str] action_jira_service_desk_param_jira_project: Jira Project name
         :param pulumi.Input[str] action_jira_service_desk_param_jira_summary: Jira issue title/summary
+        :param pulumi.Input[str] action_pagerduty_custom_details: The PagerDuty custom details information.
+        :param pulumi.Input[str] action_pagerduty_integration_key: The PagerDuty integration Key.
+        :param pulumi.Input[str] action_pagerduty_integration_key_override: The PagerDuty integration Key override.
         :param pulumi.Input[str] action_pagerduty_integration_url: The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[str] action_pagerduty_integration_url_override: The pagerduty integration URL override. This integration uses Splunk's native webhooks to send events to PagerDuty.
         :param pulumi.Input[bool] action_populate_lookup: The state of the populate lookup action. Read-only attribute. Value ignored on POST. Use actions to specify a list of enabled actions. Defaults to 0.
         :param pulumi.Input[str] action_populate_lookup_command: The search command (or pipeline) which is responsible for executing the action.
         :param pulumi.Input[str] action_populate_lookup_dest: Lookup name of path of the lookup to populate
         :param pulumi.Input[str] action_populate_lookup_hostname: Sets the hostname used in the web link (url) sent in alert actions.This value accepts two forms: hostname (for example, splunkserver, splunkserver.example.com)\\n\\nprotocol://hostname:port (for example, http://splunkserver:8000, https://splunkserver.example.com:443)
         :param pulumi.Input[int] action_populate_lookup_max_results: Sets the maximum number of search results sent using alerts. Defaults to 100.
@@ -6400,14 +6514,17 @@
         __props__.__dict__["action_email_width_sort_columns"] = action_email_width_sort_columns
         __props__.__dict__["action_jira_service_desk_param_account"] = action_jira_service_desk_param_account
         __props__.__dict__["action_jira_service_desk_param_jira_description"] = action_jira_service_desk_param_jira_description
         __props__.__dict__["action_jira_service_desk_param_jira_issue_type"] = action_jira_service_desk_param_jira_issue_type
         __props__.__dict__["action_jira_service_desk_param_jira_priority"] = action_jira_service_desk_param_jira_priority
         __props__.__dict__["action_jira_service_desk_param_jira_project"] = action_jira_service_desk_param_jira_project
         __props__.__dict__["action_jira_service_desk_param_jira_summary"] = action_jira_service_desk_param_jira_summary
+        __props__.__dict__["action_pagerduty_custom_details"] = action_pagerduty_custom_details
+        __props__.__dict__["action_pagerduty_integration_key"] = action_pagerduty_integration_key
+        __props__.__dict__["action_pagerduty_integration_key_override"] = action_pagerduty_integration_key_override
         __props__.__dict__["action_pagerduty_integration_url"] = action_pagerduty_integration_url
         __props__.__dict__["action_pagerduty_integration_url_override"] = action_pagerduty_integration_url_override
         __props__.__dict__["action_populate_lookup"] = action_populate_lookup
         __props__.__dict__["action_populate_lookup_command"] = action_populate_lookup_command
         __props__.__dict__["action_populate_lookup_dest"] = action_populate_lookup_dest
         __props__.__dict__["action_populate_lookup_hostname"] = action_populate_lookup_hostname
         __props__.__dict__["action_populate_lookup_max_results"] = action_populate_lookup_max_results
@@ -6945,14 +7062,38 @@
     def action_jira_service_desk_param_jira_summary(self) -> pulumi.Output[Optional[str]]:
         """
         Jira issue title/summary
         """
         return pulumi.get(self, "action_jira_service_desk_param_jira_summary")
 
     @property
+    @pulumi.getter(name="actionPagerdutyCustomDetails")
+    def action_pagerduty_custom_details(self) -> pulumi.Output[str]:
+        """
+        The PagerDuty custom details information.
+        """
+        return pulumi.get(self, "action_pagerduty_custom_details")
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKey")
+    def action_pagerduty_integration_key(self) -> pulumi.Output[str]:
+        """
+        The PagerDuty integration Key.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key")
+
+    @property
+    @pulumi.getter(name="actionPagerdutyIntegrationKeyOverride")
+    def action_pagerduty_integration_key_override(self) -> pulumi.Output[str]:
+        """
+        The PagerDuty integration Key override.
+        """
+        return pulumi.get(self, "action_pagerduty_integration_key_override")
+
+    @property
     @pulumi.getter(name="actionPagerdutyIntegrationUrl")
     def action_pagerduty_integration_url(self) -> pulumi.Output[Optional[str]]:
         """
         The pagerduty integration URL. This integration uses Splunk's native webhooks to send events to PagerDuty.
         """
         return pulumi.get(self, "action_pagerduty_integration_url")
```

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-splunk
-Version: 1.3.0a1690264914
+Version: 1.3.0a1690564639
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi splunk
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_splunk-1.3.0a1690264914/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1690564639/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1690264914/setup.py` & `pulumi_splunk-1.3.0a1690564639/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1690264914"
-PLUGIN_VERSION = "1.3.0-alpha.1690264914+73798e57"
+VERSION = "1.3.0a1690564639"
+PLUGIN_VERSION = "1.3.0-alpha.1690564639+231b9dd6"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'splunk', PLUGIN_VERSION])
         except OSError as error:
```

