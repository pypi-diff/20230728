# Comparing `tmp/cloudquery-plugin-sdk-0.0.4.tar.gz` & `tmp/cloudquery-plugin-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-sdk-0.0.4.tar", last modified: Fri Jul 28 08:16:11 2023, max compression
+gzip compressed data, was "cloudquery-plugin-sdk-0.0.5.tar", last modified: Fri Jul 28 08:29:10 2023, max compression
```

## Comparing `cloudquery-plugin-sdk-0.0.4.tar` & `cloudquery-plugin-sdk-0.0.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.227083 cloudquery-plugin-sdk-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 08:16:11.227083 cloudquery-plugin-sdk-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.215082 cloudquery-plugin-sdk-0.0.4/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/markdown_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/memdb/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/memdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/memdb/memdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/message/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/message/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/message/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.219082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/date32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/float64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/int64.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/scalar_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/table_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/serve/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/serve/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.223082 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/types/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:16:11.227083 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:16:11.000000 cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 08:16:11.227083 cloudquery-plugin-sdk-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 08:15:48.000000 cloudquery-plugin-sdk-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.872885 cloudquery-plugin-sdk-0.0.5/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/markdown_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/memdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/memdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/memdb/memdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.876885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.880885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/message/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/message/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/message/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.880885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.880885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/date32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/float64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/int64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/scalar_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.880885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/table_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.880885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/serve/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 08:29:10.000000 cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 08:29:10.884885 cloudquery-plugin-sdk-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 08:28:49.000000 cloudquery-plugin-sdk-0.0.5/setup.py
```

### Comparing `cloudquery-plugin-sdk-0.0.4/PKG-INFO` & `cloudquery-plugin-sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/generator.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/generator.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/docs/markdown_templates.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/docs/markdown_templates.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/memdb/memdb.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/memdb/memdb.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/internal/servers/plugin_v3/plugin.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/internal/servers/plugin_v3/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/plugin/plugin.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/binary.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/binary.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/bool.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/bool.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/date32.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/date32.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/float64.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/float64.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/int64.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/int64.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scalar/uuid.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scalar/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/scheduler.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/scheduler/table_resolver.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/scheduler/table_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/column.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/column.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/resource.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/resource.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/schema/table.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/schema/table.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/serve/plugin.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/serve/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery/sdk/types/uuid.py` & `cloudquery-plugin-sdk-0.0.5/cloudquery/sdk/types/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/PKG-INFO` & `cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.4/cloudquery_plugin_sdk.egg-info/SOURCES.txt` & `cloudquery-plugin-sdk-0.0.5/cloudquery_plugin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.4/setup.py` & `cloudquery-plugin-sdk-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "cloudquery-plugin-sdk"
 
 description = "CloudQuery Plugin SDK for Python"
 
 dependencies = [
-    "plugin-pb-python==0.0.13",
+    "cloudquery-plugin-pb==0.0.14",
     "pyarrow==12.0.1",
     "Jinja2==3.1.2",
     "structlog==23.1.0",
 ]
 url = "https://github.com/cloudquery/plugin-sdk-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
@@ -32,15 +32,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.4",
+    version="0.0.5",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

