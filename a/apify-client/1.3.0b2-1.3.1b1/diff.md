# Comparing `tmp/apify_client-1.3.0b2.tar.gz` & `tmp/apify_client-1.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.3.0b2.tar", last modified: Mon Jul 24 08:50:24 2023, max compression
+gzip compressed data, was "apify_client-1.3.1b1.tar", last modified: Fri Jul 28 14:48:15 2023, max compression
```

## Comparing `apify_client-1.3.0b2.tar` & `apify_client-1.3.1b1.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.721164 apify_client-1.3.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-24 08:50:24.721164 apify_client-1.3.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-24 08:50:21.000000 apify_client-1.3.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:50:24.721164 apify_client-1.3.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.713163 apify_client-1.3.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.713163 apify_client-1.3.0b2/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.717164 apify_client-1.3.0b2/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.717164 apify_client-1.3.0b2/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.721164 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    46610 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 08:49:43.000000 apify_client-1.3.0b2/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:50:24.713163 apify_client-1.3.0b2/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-24 08:50:24.000000 apify_client-1.3.0b2/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-24 08:50:24.000000 apify_client-1.3.0b2/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:50:24.000000 apify_client-1.3.0b2/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-24 08:50:24.000000 apify_client-1.3.0b2/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 08:50:24.000000 apify_client-1.3.0b2/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.118427 apify_client-1.3.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-28 14:48:15.114427 apify_client-1.3.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-28 14:48:10.000000 apify_client-1.3.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:48:15.118427 apify_client-1.3.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.106427 apify_client-1.3.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.106427 apify_client-1.3.1b1/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.110427 apify_client-1.3.1b1/src/apify_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.110427 apify_client-1.3.1b1/src/apify_client/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/base/actor_job_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/base/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/base/resource_collection_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.114427 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30487 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46397 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21007 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:47:23.000000 apify_client-1.3.1b1/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:48:15.110427 apify_client-1.3.1b1/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-28 14:48:15.000000 apify_client-1.3.1b1/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 14:48:15.000000 apify_client-1.3.1b1/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:48:15.000000 apify_client-1.3.1b1/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 14:48:15.000000 apify_client-1.3.1b1/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 14:48:15.000000 apify_client-1.3.1b1/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.3.0b2/LICENSE` & `apify_client-1.3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.0b2/PKG-INFO` & `apify_client-1.3.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.3.0b2
+Version: 1.3.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.3.0b2/README.md` & `apify_client-1.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.0b2/pyproject.toml` & `apify_client-1.3.1b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 
 name = "apify_client"
 
-version = "1.3.0b2"
+version = "1.3.1b1"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
 
-    {name = "Apify Technologies s.r.o.", email = "support@apify.com" }
+    {name = "Apify Technologies s.r.o.", email = "support@apify.com"},
 
 ]
 
 keywords = ["apify", "api", "client", "scraping", "automation"]
 
 
 
@@ -43,15 +43,17 @@
 
 
 
 requires-python = ">=3.8"
 
 dependencies = [
 
-    "httpx >= 0.24.1"
+    "apify-shared ~= 1.0.0",
+
+    "httpx >= 0.24.1",
 
 ]
 
 
 
 [project.optional-dependencies]
```

### Comparing `apify_client-1.3.0b2/src/apify_client/_errors.py` & `apify_client-1.3.1b1/src/apify_client/_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import httpx
 
-from ._utils import ignore_docs
+from apify_shared.utils import ignore_docs
 
 
 class ApifyClientError(Exception):
     """Base class for errors specific to the Apify API Client."""
 
     pass
```

### Comparing `apify_client-1.3.0b2/src/apify_client/_http_client.py` & `apify_client-1.3.1b1/src/apify_client/_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,20 @@
 import sys
 from http import HTTPStatus
 from importlib import metadata
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import httpx
 
+from apify_shared.types import JSONSerializable
+from apify_shared.utils import ignore_docs, is_content_type_json, is_content_type_text, is_content_type_xml
+
 from ._errors import ApifyApiError, InvalidResponseBodyError, _is_retryable_error
 from ._logging import logger_name
-from ._types import JSONSerializable
-from ._utils import (
-    _is_content_type_json,
-    _is_content_type_text,
-    _is_content_type_xml,
-    _retry_with_exp_backoff,
-    _retry_with_exp_backoff_async,
-    ignore_docs,
-)
+from ._utils import _retry_with_exp_backoff, _retry_with_exp_backoff_async
 
 DEFAULT_BACKOFF_EXPONENTIAL_FACTOR = 2
 DEFAULT_BACKOFF_RANDOM_FACTOR = 1
 
 logger = logging.getLogger(logger_name)
 
 
@@ -66,17 +61,17 @@
             return None
 
         content_type = ''
         if 'content-type' in response.headers:
             content_type = response.headers['content-type'].split(';')[0].strip()
 
         try:
-            if _is_content_type_json(content_type):
+            if is_content_type_json(content_type):
                 return response.json()
-            elif _is_content_type_xml(content_type) or _is_content_type_text(content_type):
+            elif is_content_type_xml(content_type) or is_content_type_text(content_type):
                 return response.text
             else:
                 return response.content
         except ValueError as err:
             raise InvalidResponseBodyError(response) from err
 
     @staticmethod
```

### Comparing `apify_client-1.3.0b2/src/apify_client/_logging.py` & `apify_client-1.3.1b1/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.0b2/src/apify_client/client.py` & `apify_client-1.3.1b1/src/apify_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict, Optional, Union
 
+from apify_shared.utils import ignore_docs
+
 from ._http_client import _HTTPClient, _HTTPClientAsync
-from ._utils import ignore_docs
 from .clients import (
     ActorClient,
     ActorClientAsync,
     ActorCollectionClient,
     ActorCollectionClientAsync,
     BuildClient,
     BuildClientAsync,
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/__init__.py` & `apify_client-1.3.1b1/src/apify_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/base/actor_job_base_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/actor_job_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
 import math
 import time
 from datetime import datetime, timezone
 from typing import Dict, Optional
 
+from apify_shared.consts import ActorJobStatus
+from apify_shared.utils import ignore_docs, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import _catch_not_found_or_throw, _parse_date_fields, _pluck_data, ignore_docs
-from ...consts import ActorJobStatus
+from ..._utils import _catch_not_found_or_throw, _pluck_data
 from .resource_client import ResourceClient, ResourceClientAsync
 
 DEFAULT_WAIT_FOR_FINISH_SEC = 999999
 
 # After how many seconds we give up trying in case job doesn't exist
 DEFAULT_WAIT_WHEN_JOB_NOT_EXIST_SEC = 3
 
@@ -32,15 +34,15 @@
 
             try:
                 response = self.http_client.call(
                     url=self._url(),
                     method='GET',
                     params=self._params(waitForFinish=wait_for_finish),
                 )
-                job = _parse_date_fields(_pluck_data(response.json()))
+                job = parse_date_fields(_pluck_data(response.json()))
 
                 seconds_elapsed = math.floor(((datetime.now(timezone.utc) - started_at).total_seconds()))
                 if (
                     ActorJobStatus(job['status'])._is_terminal or (wait_secs is not None and seconds_elapsed >= wait_secs)
                 ):
                     should_repeat = False
 
@@ -65,15 +67,15 @@
         response = self.http_client.call(
             url=self._url('abort'),
             method='POST',
             params=self._params(
                 gracefully=gracefully,
             ),
         )
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
 
 @ignore_docs
 class ActorJobBaseClientAsync(ResourceClientAsync):
     """Base async sub-client class for actor runs and actor builds."""
 
     async def _wait_for_finish(self, wait_secs: Optional[int] = None) -> Optional[Dict]:
@@ -89,15 +91,15 @@
 
             try:
                 response = await self.http_client.call(
                     url=self._url(),
                     method='GET',
                     params=self._params(waitForFinish=wait_for_finish),
                 )
-                job = _parse_date_fields(_pluck_data(response.json()))
+                job = parse_date_fields(_pluck_data(response.json()))
 
                 seconds_elapsed = math.floor(((datetime.now(timezone.utc) - started_at).total_seconds()))
                 if (
                     ActorJobStatus(job['status'])._is_terminal or (wait_secs is not None and seconds_elapsed >= wait_secs)
                 ):
                     should_repeat = False
 
@@ -122,8 +124,8 @@
         response = await self.http_client.call(
             url=self._url('abort'),
             method='POST',
             params=self._params(
                 gracefully=gracefully,
             ),
         )
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/base/base_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
+from apify_shared.utils import ignore_docs
+
 from ..._http_client import _HTTPClient, _HTTPClientAsync
 from ..._logging import _WithLogDetailsClient
-from ..._utils import _to_safe_id, ignore_docs
+from ..._utils import _to_safe_id
 
 # Conditional import only executed when type checking, otherwise we'd get circular dependency issues
 if TYPE_CHECKING:
     from ...client import ApifyClient, ApifyClientAsync
 
 
 class _BaseBaseClient(metaclass=_WithLogDetailsClient):
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/base/resource_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/resource_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Dict, Optional
 
+from apify_shared.utils import ignore_docs, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import _catch_not_found_or_throw, _parse_date_fields, _pluck_data, ignore_docs
+from ..._utils import _catch_not_found_or_throw, _pluck_data
 from .base_client import BaseClient, BaseClientAsync
 
 
 @ignore_docs
 class ResourceClient(BaseClient):
     """Base class for sub-clients manipulating a single resource."""
 
@@ -13,30 +15,30 @@
         try:
             response = self.http_client.call(
                 url=self.url,
                 method='GET',
                 params=self._params(),
             )
 
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     def _update(self, updated_fields: Dict) -> Dict:
         response = self.http_client.call(
             url=self._url(),
             method='PUT',
             params=self._params(),
             json=updated_fields,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def _delete(self) -> None:
         try:
             self.http_client.call(
                 url=self._url(),
                 method='DELETE',
                 params=self._params(),
@@ -54,30 +56,30 @@
         try:
             response = await self.http_client.call(
                 url=self.url,
                 method='GET',
                 params=self._params(),
             )
 
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     async def _update(self, updated_fields: Dict) -> Dict:
         response = await self.http_client.call(
             url=self._url(),
             method='PUT',
             params=self._params(),
             json=updated_fields,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def _delete(self) -> None:
         try:
             await self.http_client.call(
                 url=self._url(),
                 method='DELETE',
                 params=self._params(),
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/base/resource_collection_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/resource_collection_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _parse_date_fields, _pluck_data, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs, parse_date_fields
+
+from ..._utils import _pluck_data
 from .base_client import BaseClient, BaseClientAsync
 
 
 @ignore_docs
 class ResourceCollectionClient(BaseClient):
     """Base class for sub-clients manipulating a resource collection."""
 
     def _list(self, **kwargs: Any) -> ListPage:
         response = self.http_client.call(
             url=self._url(),
             method='GET',
             params=self._params(**kwargs),
         )
 
-        return ListPage(_parse_date_fields(_pluck_data(response.json())))
+        return ListPage(parse_date_fields(_pluck_data(response.json())))
 
     def _create(self, resource: Dict) -> Dict:
         response = self.http_client.call(
             url=self._url(),
             method='POST',
             params=self._params(),
             json=resource,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def _get_or_create(self, name: Optional[str] = None, resource: Optional[Dict] = None) -> Dict:
         response = self.http_client.call(
             url=self._url(),
             method='POST',
             params=self._params(name=name),
             json=resource,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
 
 @ignore_docs
 class ResourceCollectionClientAsync(BaseClientAsync):
     """Base class for async sub-clients manipulating a resource collection."""
 
     async def _list(self, **kwargs: Any) -> ListPage:
         response = await self.http_client.call(
             url=self._url(),
             method='GET',
             params=self._params(**kwargs),
         )
 
-        return ListPage(_parse_date_fields(_pluck_data(response.json())))
+        return ListPage(parse_date_fields(_pluck_data(response.json())))
 
     async def _create(self, resource: Dict) -> Dict:
         response = await self.http_client.call(
             url=self._url(),
             method='POST',
             params=self._params(),
             json=resource,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def _get_or_create(self, name: Optional[str] = None, resource: Optional[Dict] = None) -> Dict:
         response = await self.http_client.call(
             url=self._url(),
             method='POST',
             params=self._params(name=name),
             json=resource,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/__init__.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from typing import Any, Dict, List, Optional
 
-from ..._utils import (
-    _encode_key_value_store_record_value,
-    _encode_webhook_list_to_base64,
-    _filter_out_none_values_recursively,
-    _maybe_extract_enum_member_value,
-    _parse_date_fields,
-    _pluck_data,
-    ignore_docs,
-)
-from ...consts import ActorJobStatus, MetaOrigin
+from apify_shared.consts import ActorJobStatus, MetaOrigin
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, maybe_extract_enum_member_value, parse_date_fields
+
+from ..._utils import _encode_key_value_store_record_value, _encode_webhook_list_to_base64, _pluck_data
 from ..base import ResourceClient, ResourceClientAsync
 from .actor_version import ActorVersionClient, ActorVersionClientAsync
 from .actor_version_collection import ActorVersionCollectionClient, ActorVersionCollectionClientAsync
 from .build_collection import BuildCollectionClient, BuildCollectionClientAsync
 from .run import RunClient, RunClientAsync
 from .run_collection import RunCollectionClient, RunCollectionClientAsync
 from .webhook_collection import WebhookCollectionClient, WebhookCollectionClientAsync
@@ -141,15 +135,15 @@
             default_run_build=default_run_build,
             default_run_memory_mbytes=default_run_memory_mbytes,
             default_run_timeout_secs=default_run_timeout_secs,
             example_run_input_body=example_run_input_body,
             example_run_input_content_type=example_run_input_content_type,
         )
 
-        return self._update(_filter_out_none_values_recursively(actor_representation))
+        return self._update(filter_out_none_values_recursively(actor_representation))
 
     def delete(self) -> None:
         """Delete the actor.
 
         https://docs.apify.com/api/v2#/reference/actors/actor-object/delete-actor
         """
         return self._delete()
@@ -206,15 +200,15 @@
             url=self._url('runs'),
             method='POST',
             headers={'content-type': content_type},
             data=run_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def call(
         self,
         *,
         run_input: Optional[Any] = None,
         content_type: Optional[str] = None,
         build: Optional[str] = None,
@@ -295,15 +289,15 @@
 
         response = self.http_client.call(
             url=self._url('builds'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def builds(self) -> BuildCollectionClient:
         """Retrieve a client for the builds of this actor."""
         return BuildCollectionClient(**self._sub_resource_init_options(resource_path='builds'))
 
     def runs(self) -> RunCollectionClient:
         """Retrieve a client for the runs of this actor."""
@@ -321,16 +315,16 @@
         Returns:
             RunClient: The resource client for the last run of this actor.
         """
         return RunClient(**self._sub_resource_init_options(
             resource_id='last',
             resource_path='runs',
             params=self._params(
-                status=_maybe_extract_enum_member_value(status),
-                origin=_maybe_extract_enum_member_value(origin),
+                status=maybe_extract_enum_member_value(status),
+                origin=maybe_extract_enum_member_value(origin),
             ),
         ))
 
     def versions(self) -> ActorVersionCollectionClient:
         """Retrieve a client for the versions of this actor."""
         return ActorVersionCollectionClient(**self._sub_resource_init_options())
 
@@ -429,15 +423,15 @@
             default_run_build=default_run_build,
             default_run_memory_mbytes=default_run_memory_mbytes,
             default_run_timeout_secs=default_run_timeout_secs,
             example_run_input_body=example_run_input_body,
             example_run_input_content_type=example_run_input_content_type,
         )
 
-        return await self._update(_filter_out_none_values_recursively(actor_representation))
+        return await self._update(filter_out_none_values_recursively(actor_representation))
 
     async def delete(self) -> None:
         """Delete the actor.
 
         https://docs.apify.com/api/v2#/reference/actors/actor-object/delete-actor
         """
         return await self._delete()
@@ -494,15 +488,15 @@
             url=self._url('runs'),
             method='POST',
             headers={'content-type': content_type},
             data=run_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def call(
         self,
         *,
         run_input: Optional[Any] = None,
         content_type: Optional[str] = None,
         build: Optional[str] = None,
@@ -583,15 +577,15 @@
 
         response = await self.http_client.call(
             url=self._url('builds'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def builds(self) -> BuildCollectionClientAsync:
         """Retrieve a client for the builds of this actor."""
         return BuildCollectionClientAsync(**self._sub_resource_init_options(resource_path='builds'))
 
     def runs(self) -> RunCollectionClientAsync:
         """Retrieve a client for the runs of this actor."""
@@ -609,16 +603,16 @@
         Returns:
             RunClientAsync: The resource client for the last run of this actor.
         """
         return RunClientAsync(**self._sub_resource_init_options(
             resource_id='last',
             resource_path='runs',
             params=self._params(
-                status=_maybe_extract_enum_member_value(status),
-                origin=_maybe_extract_enum_member_value(origin),
+                status=maybe_extract_enum_member_value(status),
+                origin=maybe_extract_enum_member_value(origin),
             ),
         ))
 
     def versions(self) -> ActorVersionCollectionClientAsync:
         """Retrieve a client for the versions of this actor."""
         return ActorVersionCollectionClientAsync(**self._sub_resource_init_options())
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, List, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .actor import _get_actor_representation
 
 
 class ActorCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating actors."""
 
@@ -97,15 +99,15 @@
             default_run_build=default_run_build,
             default_run_memory_mbytes=default_run_memory_mbytes,
             default_run_timeout_secs=default_run_timeout_secs,
             example_run_input_body=example_run_input_body,
             example_run_input_content_type=example_run_input_content_type,
         )
 
-        return self._create(_filter_out_none_values_recursively(actor_representation))
+        return self._create(filter_out_none_values_recursively(actor_representation))
 
 
 class ActorCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating actors."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -196,8 +198,8 @@
             default_run_build=default_run_build,
             default_run_memory_mbytes=default_run_memory_mbytes,
             default_run_timeout_secs=default_run_timeout_secs,
             example_run_input_body=example_run_input_body,
             example_run_input_content_type=example_run_input_content_type,
         )
 
-        return await self._create(_filter_out_none_values_recursively(actor_representation))
+        return await self._create(filter_out_none_values_recursively(actor_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_env_var.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import _filter_out_none_values_recursively, ignore_docs
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceClient, ResourceClientAsync
 
 
 def _get_actor_env_var_representation(
     *,
     is_secret: Optional[bool] = None,
     name: Optional[str] = None,
@@ -57,15 +58,15 @@
         """
         actor_env_var_representation = _get_actor_env_var_representation(
             is_secret=is_secret,
             name=name,
             value=value,
         )
 
-        return self._update(_filter_out_none_values_recursively(actor_env_var_representation))
+        return self._update(filter_out_none_values_recursively(actor_env_var_representation))
 
     def delete(self) -> None:
         """Delete the actor environment variable.
 
         https://docs.apify.com/api/v2#/reference/actors/environment-variable-object/delete-environment-variable
         """
         return self._delete()
@@ -111,15 +112,15 @@
         """
         actor_env_var_representation = _get_actor_env_var_representation(
             is_secret=is_secret,
             name=name,
             value=value,
         )
 
-        return await self._update(_filter_out_none_values_recursively(actor_env_var_representation))
+        return await self._update(filter_out_none_values_recursively(actor_env_var_representation))
 
     async def delete(self) -> None:
         """Delete the actor environment variable.
 
         https://docs.apify.com/api/v2#/reference/actors/environment-variable-object/delete-environment-variable
         """
         return await self._delete()
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .actor_env_var import _get_actor_env_var_representation
 
 
 class ActorEnvVarCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating actor env vars."""
 
@@ -45,15 +47,15 @@
         """
         actor_env_var_representation = _get_actor_env_var_representation(
             is_secret=is_secret,
             name=name,
             value=value,
         )
 
-        return self._create(_filter_out_none_values_recursively(actor_env_var_representation))
+        return self._create(filter_out_none_values_recursively(actor_env_var_representation))
 
 
 class ActorEnvVarCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating actor env vars."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -92,8 +94,8 @@
         """
         actor_env_var_representation = _get_actor_env_var_representation(
             is_secret=is_secret,
             name=name,
             value=value,
         )
 
-        return await self._create(_filter_out_none_values_recursively(actor_env_var_representation))
+        return await self._create(filter_out_none_values_recursively(actor_env_var_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_version.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, List, Optional
 
-from ..._utils import _filter_out_none_values_recursively, _maybe_extract_enum_member_value, ignore_docs
-from ...consts import ActorSourceType
+from apify_shared.consts import ActorSourceType
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, maybe_extract_enum_member_value
+
 from ..base import ResourceClient, ResourceClientAsync
 from .actor_env_var import ActorEnvVarClient, ActorEnvVarClientAsync
 from .actor_env_var_collection import ActorEnvVarCollectionClient, ActorEnvVarCollectionClientAsync
 
 
 def _get_actor_version_representation(
     *,
@@ -20,15 +21,15 @@
     github_gist_url: Optional[str] = None,
 ) -> Dict:
     return {
         'versionNumber': version_number,
         'buildTag': build_tag,
         'envVars': env_vars,
         'applyEnvVarsToBuild': apply_env_vars_to_build,
-        'sourceType': _maybe_extract_enum_member_value(source_type),
+        'sourceType': maybe_extract_enum_member_value(source_type),
         'sourceFiles': source_files,
         'gitRepoUrl': git_repo_url,
         'tarballUrl': tarball_url,
         'gitHubGistUrl': github_gist_url,
     }
 
 
@@ -93,15 +94,15 @@
             source_type=source_type,
             source_files=source_files,
             git_repo_url=git_repo_url,
             tarball_url=tarball_url,
             github_gist_url=github_gist_url,
         )
 
-        return self._update(_filter_out_none_values_recursively(actor_version_representation))
+        return self._update(filter_out_none_values_recursively(actor_version_representation))
 
     def delete(self) -> None:
         """Delete the actor version.
 
         https://docs.apify.com/api/v2#/reference/actors/version-object/delete-version
         """
         return self._delete()
@@ -183,15 +184,15 @@
             source_type=source_type,
             source_files=source_files,
             git_repo_url=git_repo_url,
             tarball_url=tarball_url,
             github_gist_url=github_gist_url,
         )
 
-        return await self._update(_filter_out_none_values_recursively(actor_version_representation))
+        return await self._update(filter_out_none_values_recursively(actor_version_representation))
 
     async def delete(self) -> None:
         """Delete the actor version.
 
         https://docs.apify.com/api/v2#/reference/actors/version-object/delete-version
         """
         return await self._delete()
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/actor_version_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Dict, List, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
-from ...consts import ActorSourceType
+from apify_shared.consts import ActorSourceType
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .actor_version import _get_actor_version_representation
 
 
 class ActorVersionCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating actor versions."""
 
@@ -70,15 +72,15 @@
             source_type=source_type,
             source_files=source_files,
             git_repo_url=git_repo_url,
             tarball_url=tarball_url,
             github_gist_url=github_gist_url,
         )
 
-        return self._create(_filter_out_none_values_recursively(actor_version_representation))
+        return self._create(filter_out_none_values_recursively(actor_version_representation))
 
 
 class ActorVersionCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating actor versions."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -141,8 +143,8 @@
             source_type=source_type,
             source_files=source_files,
             git_repo_url=git_repo_url,
             tarball_url=tarball_url,
             github_gist_url=github_gist_url,
         )
 
-        return await self._create(_filter_out_none_values_recursively(actor_version_representation))
+        return await self._create(filter_out_none_values_recursively(actor_version_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/build.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ignore_docs
+from apify_shared.utils import ignore_docs
+
 from ..base import ActorJobBaseClient, ActorJobBaseClientAsync
 
 
 class BuildClient(ActorJobBaseClient):
     """Sub-client for manipulating a single actor build."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/build_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class BuildCollectionClient(ResourceCollectionClient):
     """Sub-client for listing actor builds."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/dataset.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import warnings
 from contextlib import asynccontextmanager, contextmanager
 from typing import Any, AsyncIterator, Dict, Iterator, List, Optional
 
 import httpx
 
-from ..._types import JSONSerializable
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.types import JSONSerializable
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class DatasetClient(ResourceClient):
     """Sub-client for manipulating a single dataset."""
 
     @ignore_docs
@@ -39,15 +41,15 @@
         Returns:
             dict: The updated dataset
         """
         updated_fields = {
             'name': name,
         }
 
-        return self._update(_filter_out_none_values_recursively(updated_fields))
+        return self._update(filter_out_none_values_recursively(updated_fields))
 
     def delete(self) -> None:
         """Delete the dataset.
 
         https://docs.apify.com/api/v2#/reference/datasets/dataset/delete-dataset
         """
         return self._delete()
@@ -264,23 +266,19 @@
             xml_row (str, optional): Overrides default element name that wraps each page or page function result object in xml output.
                 By default the element name is item.
             flatten (list of str, optional): A list of fields that should be flattened
 
         Returns:
             bytes: The dataset items as raw bytes
         """
-        # We need to override and then restore the warnings filter so that the warning gets printed out,
-        # Otherwise it would be silently swallowed
-        with warnings.catch_warnings():
-            warnings.simplefilter('always')
-            warnings.warn(
-                '`DatasetClient.download_items()` is deprecated, use `DatasetClient.get_items_as_bytes()` instead.',
-                DeprecationWarning,
-                stacklevel=2,
-            )
+        warnings.warn(
+            '`DatasetClient.download_items()` is deprecated, use `DatasetClient.get_items_as_bytes()` instead.',
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
         return self.get_items_as_bytes(
             item_format=item_format,
             offset=offset,
             limit=limit,
             desc=desc,
             clean=clean,
@@ -532,15 +530,15 @@
         Returns:
             dict: The updated dataset
         """
         updated_fields = {
             'name': name,
         }
 
-        return await self._update(_filter_out_none_values_recursively(updated_fields))
+        return await self._update(filter_out_none_values_recursively(updated_fields))
 
     async def delete(self) -> None:
         """Delete the dataset.
 
         https://docs.apify.com/api/v2#/reference/datasets/dataset/delete-dataset
         """
         return await self._delete()
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/dataset_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class DatasetCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating datasets."""
 
     @ignore_docs
@@ -44,15 +46,15 @@
         Args:
             name (str, optional): The name of the dataset to retrieve or create.
             schema (Dict, optional): The schema of the dataset
 
         Returns:
             dict: The retrieved or newly-created dataset.
         """
-        return self._get_or_create(name=name, resource=_filter_out_none_values_recursively({'schema': schema}))
+        return self._get_or_create(name=name, resource=filter_out_none_values_recursively({'schema': schema}))
 
 
 class DatasetCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating datasets."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -91,8 +93,8 @@
         Args:
             name (str, optional): The name of the dataset to retrieve or create.
             schema (Dict, optional): The schema of the dataset
 
         Returns:
             dict: The retrieved or newly-created dataset.
         """
-        return await self._get_or_create(name=name, resource=_filter_out_none_values_recursively({'schema': schema}))
+        return await self._get_or_create(name=name, resource=filter_out_none_values_recursively({'schema': schema}))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/key_value_store.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import warnings
 from contextlib import asynccontextmanager, contextmanager
 from typing import Any, AsyncIterator, Dict, Iterator, Optional
 
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import (
-    _catch_not_found_or_throw,
-    _encode_key_value_store_record_value,
-    _filter_out_none_values_recursively,
-    _parse_date_fields,
-    _pluck_data,
-    ignore_docs,
-)
+from ..._utils import _catch_not_found_or_throw, _encode_key_value_store_record_value, _pluck_data
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class KeyValueStoreClient(ResourceClient):
     """Sub-client for manipulating a single key-value store."""
 
     @ignore_docs
@@ -44,15 +39,15 @@
         Returns:
             dict: The updated key-value store
         """
         updated_fields = {
             'name': name,
         }
 
-        return self._update(_filter_out_none_values_recursively(updated_fields))
+        return self._update(filter_out_none_values_recursively(updated_fields))
 
     def delete(self) -> None:
         """Delete the key-value store.
 
         https://docs.apify.com/api/v2#/reference/key-value-stores/store-object/delete-store
         """
         return self._delete()
@@ -76,15 +71,15 @@
 
         response = self.http_client.call(
             url=self._url('keys'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def get_record(self, key: str, *, as_bytes: bool = False, as_file: bool = False) -> Optional[Dict]:
         """Retrieve the given record from the key-value store.
 
         https://docs.apify.com/api/v2#/reference/key-value-stores/record/get-record
 
         Args:
@@ -96,36 +91,27 @@
             dict, optional: The requested record, or None, if the record does not exist
         """
         try:
             if as_bytes and as_file:
                 raise ValueError('You cannot have both as_bytes and as_file set.')
 
             if as_bytes:
-                # We need to override and then restore the warnings filter so that the warning gets printed out,
-                # Otherwise it would be silently swallowed
-                with warnings.catch_warnings():
-                    warnings.simplefilter('always')
-                    warnings.warn(
-                        '`KeyValueStoreClient.get_record(..., as_bytes=True)` is deprecated, use `KeyValueStoreClient.get_record_as_bytes()` instead.',  # noqa: E501
-                        DeprecationWarning,
-                        stacklevel=2,
-                    )
-
+                warnings.warn(
+                    '`KeyValueStoreClient.get_record(..., as_bytes=True)` is deprecated, use `KeyValueStoreClient.get_record_as_bytes()` instead.',  # noqa: E501
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
                 return self.get_record_as_bytes(key)
 
             if as_file:
-                # We need to override and then restore the warnings filter so that the warning gets printed out,
-                # Otherwise it would be silently swallowed
-                with warnings.catch_warnings():
-                    warnings.simplefilter('always')
-                    warnings.warn(
-                        '`KeyValueStoreClient.get_record(..., as_file=True)` is deprecated, use `KeyValueStoreClient.stream_record()` instead.',
-                        DeprecationWarning,
-                        stacklevel=2,
-                    )
+                warnings.warn(
+                    '`KeyValueStoreClient.get_record(..., as_file=True)` is deprecated, use `KeyValueStoreClient.stream_record()` instead.',
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
                 return self.stream_record(key)  # type: ignore
 
             response = self.http_client.call(
                 url=self._url(f'records/{key}'),
                 method='GET',
                 params=self._params(),
             )
@@ -273,15 +259,15 @@
         Returns:
             dict: The updated key-value store
         """
         updated_fields = {
             'name': name,
         }
 
-        return await self._update(_filter_out_none_values_recursively(updated_fields))
+        return await self._update(filter_out_none_values_recursively(updated_fields))
 
     async def delete(self) -> None:
         """Delete the key-value store.
 
         https://docs.apify.com/api/v2#/reference/key-value-stores/store-object/delete-store
         """
         return await self._delete()
@@ -305,15 +291,15 @@
 
         response = await self.http_client.call(
             url=self._url('keys'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def get_record(self, key: str) -> Optional[Dict]:
         """Retrieve the given record from the key-value store.
 
         https://docs.apify.com/api/v2#/reference/key-value-stores/record/get-record
 
         Args:
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/key_value_store_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class KeyValueStoreCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating key-value stores."""
 
     @ignore_docs
@@ -44,15 +46,15 @@
         Args:
             name (str, optional): The name of the key-value store to retrieve or create.
             schema (Dict, optional): The schema of the key-value store
 
         Returns:
             dict: The retrieved or newly-created key-value store.
         """
-        return self._get_or_create(name=name, resource=_filter_out_none_values_recursively({'schema': schema}))
+        return self._get_or_create(name=name, resource=filter_out_none_values_recursively({'schema': schema}))
 
 
 class KeyValueStoreCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating key-value stores."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -91,8 +93,8 @@
         Args:
             name (str, optional): The name of the key-value store to retrieve or create.
             schema (Dict, optional): The schema of the key-value store
 
         Returns:
             dict: The retrieved or newly-created key-value store.
         """
-        return await self._get_or_create(name=name, resource=_filter_out_none_values_recursively({'schema': schema}))
+        return await self._get_or_create(name=name, resource=filter_out_none_values_recursively({'schema': schema}))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/log.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from contextlib import asynccontextmanager, contextmanager
 from typing import Any, AsyncIterator, Iterator, Optional
 
 import httpx
 
+from apify_shared.utils import ignore_docs
+
 from ..._errors import ApifyApiError
-from ..._utils import _catch_not_found_or_throw, ignore_docs
+from ..._utils import _catch_not_found_or_throw
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class LogClient(ResourceClient):
     """Sub-client for manipulating logs."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/request_queue.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Dict, List, Optional
 
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import _catch_not_found_or_throw, _filter_out_none_values_recursively, _parse_date_fields, _pluck_data, ignore_docs
+from ..._utils import _catch_not_found_or_throw, _pluck_data
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class RequestQueueClient(ResourceClient):
     """Sub-client for manipulating a single request queue."""
 
     @ignore_docs
@@ -40,15 +42,15 @@
         Returns:
             dict: The updated request queue
         """
         updated_fields = {
             'name': name,
         }
 
-        return self._update(_filter_out_none_values_recursively(updated_fields))
+        return self._update(filter_out_none_values_recursively(updated_fields))
 
     def delete(self) -> None:
         """Delete the request queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/queue/delete-request-queue
         """
         return self._delete()
@@ -68,15 +70,15 @@
 
         response = self.http_client.call(
             url=self._url('head'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def list_and_lock_head(self, *, lock_secs: int, limit: Optional[int] = None) -> Dict:
         """Retrieve a given number of unlocked requests from the beginning of the queue and lock them for a given time.
 
         https://docs.apify.com/api/v2#/reference/request-queues/queue-head-with-locks/get-head-and-lock
 
         Args:
@@ -91,15 +93,15 @@
 
         response = self.http_client.call(
             url=self._url('head/lock'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def add_request(self, request: Dict, *, forefront: Optional[bool] = None) -> Dict:
         """Add a request to the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-collection/add-request
 
         Args:
@@ -117,15 +119,15 @@
         response = self.http_client.call(
             url=self._url('requests'),
             method='POST',
             json=request,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def get_request(self, request_id: str) -> Optional[Dict]:
         """Retrieve a request from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request/get-request
 
         Args:
@@ -136,15 +138,15 @@
         """
         try:
             response = self.http_client.call(
                 url=self._url(f'requests/{request_id}'),
                 method='GET',
                 params=self._params(),
             )
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     def update_request(self, request: Dict, *, forefront: Optional[bool] = None) -> Dict:
@@ -169,15 +171,15 @@
         response = self.http_client.call(
             url=self._url(f'requests/{request_id}'),
             method='PUT',
             json=request,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def delete_request(self, request_id: str) -> None:
         """Delete a request from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request/delete-request
 
         Args:
@@ -211,15 +213,15 @@
 
         response = self.http_client.call(
             url=self._url(f'requests/{request_id}/lock'),
             method='PUT',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def delete_request_lock(self, request_id: str, *, forefront: Optional[bool] = None) -> None:
         """Delete the lock on a request.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-lock/delete-request-lock
 
         Args:
@@ -253,15 +255,15 @@
 
         response = self.http_client.call(
             url=self._url('requests/batch'),
             method='POST',
             params=request_params,
             json=requests,
         )
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def batch_delete_requests(self, requests: List[Dict[str, Any]]) -> Dict:
         """Delete given requests from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/batch-request-operations/delete-requests
 
         Args:
@@ -274,15 +276,15 @@
         response = self.http_client.call(
             url=self._url('requests/batch'),
             method='DELETE',
             params=request_params,
             json=requests,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def list_requests(self, *, limit: Optional[int] = None, exclusive_start_id: Optional[str] = None) -> Dict:
         """List requests in the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-collection/list-requests
 
         Args:
@@ -293,15 +295,15 @@
 
         response = self.http_client.call(
             url=self._url('requests'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
 
 class RequestQueueClientAsync(ResourceClientAsync):
     """Async sub-client for manipulating a single request queue."""
 
     @ignore_docs
     def __init__(self, *args: Any, client_key: Optional[str] = None, **kwargs: Any) -> None:
@@ -335,15 +337,15 @@
         Returns:
             dict: The updated request queue
         """
         updated_fields = {
             'name': name,
         }
 
-        return await self._update(_filter_out_none_values_recursively(updated_fields))
+        return await self._update(filter_out_none_values_recursively(updated_fields))
 
     async def delete(self) -> None:
         """Delete the request queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/queue/delete-request-queue
         """
         return await self._delete()
@@ -363,15 +365,15 @@
 
         response = await self.http_client.call(
             url=self._url('head'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def list_and_lock_head(self, *, lock_secs: int, limit: Optional[int] = None) -> Dict:
         """Retrieve a given number of unlocked requests from the beginning of the queue and lock them for a given time.
 
         https://docs.apify.com/api/v2#/reference/request-queues/queue-head-with-locks/get-head-and-lock
 
         Args:
@@ -386,15 +388,15 @@
 
         response = await self.http_client.call(
             url=self._url('head/lock'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def add_request(self, request: Dict, *, forefront: Optional[bool] = None) -> Dict:
         """Add a request to the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-collection/add-request
 
         Args:
@@ -412,15 +414,15 @@
         response = await self.http_client.call(
             url=self._url('requests'),
             method='POST',
             json=request,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def get_request(self, request_id: str) -> Optional[Dict]:
         """Retrieve a request from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request/get-request
 
         Args:
@@ -431,15 +433,15 @@
         """
         try:
             response = await self.http_client.call(
                 url=self._url(f'requests/{request_id}'),
                 method='GET',
                 params=self._params(),
             )
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     async def update_request(self, request: Dict, *, forefront: Optional[bool] = None) -> Dict:
@@ -464,15 +466,15 @@
         response = await self.http_client.call(
             url=self._url(f'requests/{request_id}'),
             method='PUT',
             json=request,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def delete_request(self, request_id: str) -> None:
         """Delete a request from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request/delete-request
 
         Args:
@@ -506,15 +508,15 @@
 
         response = await self.http_client.call(
             url=self._url(f'requests/{request_id}/lock'),
             method='PUT',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def delete_request_lock(self, request_id: str, *, forefront: Optional[bool] = None) -> None:
         """Delete the lock on a request.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-lock/delete-request-lock
 
         Args:
@@ -548,15 +550,15 @@
 
         response = await self.http_client.call(
             url=self._url('requests/batch'),
             method='POST',
             params=request_params,
             json=requests,
         )
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def batch_delete_requests(self, requests: List[Dict[str, Any]]) -> Dict:
         """Delete given requests from the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/batch-request-operations/delete-requests
 
         Args:
@@ -568,15 +570,15 @@
 
         response = await self.http_client.call(
             url=self._url('requests/batch'),
             method='DELETE',
             params=request_params,
             json=requests,
         )
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def list_requests(self, *, limit: Optional[int] = None, exclusive_start_id: Optional[str] = None) -> Dict:
         """List requests in the queue.
 
         https://docs.apify.com/api/v2#/reference/request-queues/request-collection/list-requests
 
         Args:
@@ -587,8 +589,8 @@
 
         response = await self.http_client.call(
             url=self._url('requests'),
             method='GET',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/request_queue_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class RequestQueueCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating request queues."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/run.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import (
-    _encode_key_value_store_record_value,
-    _filter_out_none_values_recursively,
-    _parse_date_fields,
-    _pluck_data,
-    _to_safe_id,
-    ignore_docs,
-)
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, parse_date_fields
+
+from ..._utils import _encode_key_value_store_record_value, _pluck_data, _to_safe_id
 from ..base import ActorJobBaseClient, ActorJobBaseClientAsync
 from .dataset import DatasetClient, DatasetClientAsync
 from .key_value_store import KeyValueStoreClient, KeyValueStoreClientAsync
 from .log import LogClient, LogClientAsync
 from .request_queue import RequestQueueClient, RequestQueueClientAsync
 
 
@@ -47,15 +42,15 @@
             dict: The updated run
         """
         updated_fields = {
             'statusMessage': status_message,
             'isStatusMessageTerminal': is_status_message_terminal,
         }
 
-        return self._update(_filter_out_none_values_recursively(updated_fields))
+        return self._update(filter_out_none_values_recursively(updated_fields))
 
     def abort(self, *, gracefully: Optional[bool] = None) -> Dict:
         """Abort the actor run which is starting or currently running and return its details.
 
         https://docs.apify.com/api/v2#/reference/actor-runs/abort-run/abort-run
 
         Args:
@@ -115,15 +110,15 @@
             url=self._url('metamorph'),
             method='POST',
             headers={'content-type': content_type},
             data=run_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def resurrect(
         self,
         *,
         build: Optional[str] = None,
         memory_mbytes: Optional[int] = None,
         timeout_secs: Optional[int] = None,
@@ -154,15 +149,15 @@
 
         response = self.http_client.call(
             url=self._url('resurrect'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def dataset(self) -> DatasetClient:
         """Get the client for the default dataset of the actor run.
 
         https://docs.apify.com/api/v2#/reference/actors/last-run-object-and-its-storages
 
         Returns:
@@ -241,15 +236,15 @@
             dict: The updated run
         """
         updated_fields = {
             'statusMessage': status_message,
             'isStatusMessageTerminal': is_status_message_terminal,
         }
 
-        return await self._update(_filter_out_none_values_recursively(updated_fields))
+        return await self._update(filter_out_none_values_recursively(updated_fields))
 
     async def abort(self, *, gracefully: Optional[bool] = None) -> Dict:
         """Abort the actor run which is starting or currently running and return its details.
 
         https://docs.apify.com/api/v2#/reference/actor-runs/abort-run/abort-run
 
         Args:
@@ -309,15 +304,15 @@
             url=self._url('metamorph'),
             method='POST',
             headers={'content-type': content_type},
             data=run_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def resurrect(
         self,
         *,
         build: Optional[str] = None,
         memory_mbytes: Optional[int] = None,
         timeout_secs: Optional[int] = None,
@@ -348,15 +343,15 @@
 
         response = await self.http_client.call(
             url=self._url('resurrect'),
             method='POST',
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def dataset(self) -> DatasetClientAsync:
         """Get the client for the default dataset of the actor run.
 
         https://docs.apify.com/api/v2#/reference/actors/last-run-object-and-its-storages
 
         Returns:
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/run_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _maybe_extract_enum_member_value, ignore_docs
-from ...consts import ActorJobStatus
+from apify_shared.consts import ActorJobStatus
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs, maybe_extract_enum_member_value
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class RunCollectionClient(ResourceCollectionClient):
     """Sub-client for listing actor runs."""
 
     @ignore_docs
@@ -37,15 +39,15 @@
         Returns:
             ListPage: The retrieved actor runs
         """
         return self._list(
             limit=limit,
             offset=offset,
             desc=desc,
-            status=_maybe_extract_enum_member_value(status),
+            status=maybe_extract_enum_member_value(status),
         )
 
 
 class RunCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for listing actor runs."""
 
     @ignore_docs
@@ -77,9 +79,9 @@
         Returns:
             ListPage: The retrieved actor runs
         """
         return await self._list(
             limit=limit,
             offset=offset,
             desc=desc,
-            status=_maybe_extract_enum_member_value(status),
+            status=maybe_extract_enum_member_value(status),
         )
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/schedule.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Dict, List, Optional
 
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..._errors import ApifyApiError
-from ..._utils import _catch_not_found_or_throw, _filter_out_none_values_recursively, _pluck_data_as_list, ignore_docs
+from ..._utils import _catch_not_found_or_throw, _pluck_data_as_list
 from ..base import ResourceClient, ResourceClientAsync
 
 
 def _get_schedule_representation(
     cron_expression: Optional[str] = None,
     is_enabled: Optional[bool] = None,
     is_exclusive: Optional[bool] = None,
@@ -83,15 +85,15 @@
             name=name,
             actions=actions,
             description=description,
             timezone=timezone,
             title=title,
         )
 
-        return self._update(_filter_out_none_values_recursively(schedule_representation))
+        return self._update(filter_out_none_values_recursively(schedule_representation))
 
     def delete(self) -> None:
         """Delete the schedule.
 
         https://docs.apify.com/api/v2#/reference/schedules/schedule-object/delete-schedule
         """
         self._delete()
@@ -173,15 +175,15 @@
             name=name,
             actions=actions,
             description=description,
             timezone=timezone,
             title=title,
         )
 
-        return await self._update(_filter_out_none_values_recursively(schedule_representation))
+        return await self._update(filter_out_none_values_recursively(schedule_representation))
 
     async def delete(self) -> None:
         """Delete the schedule.
 
         https://docs.apify.com/api/v2#/reference/schedules/schedule-object/delete-schedule
         """
         await self._delete()
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/schedule_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, List, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .schedule import _get_schedule_representation
 
 
 class ScheduleCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating schedules."""
 
@@ -74,15 +76,15 @@
             name=name,
             actions=actions,
             description=description,
             timezone=timezone,
             title=title,
         )
 
-        return self._create(_filter_out_none_values_recursively(schedule_representation))
+        return self._create(filter_out_none_values_recursively(schedule_representation))
 
 
 class ScheduleCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating schedules."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -150,8 +152,8 @@
             name=name,
             actions=actions,
             description=description,
             timezone=timezone,
             title=title,
         )
 
-        return await self._create(_filter_out_none_values_recursively(schedule_representation))
+        return await self._create(filter_out_none_values_recursively(schedule_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/task.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from typing import Any, Dict, List, Optional, cast
 
+from apify_shared.consts import ActorJobStatus, MetaOrigin
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, maybe_extract_enum_member_value, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import (
-    _catch_not_found_or_throw,
-    _encode_webhook_list_to_base64,
-    _filter_out_none_values_recursively,
-    _maybe_extract_enum_member_value,
-    _parse_date_fields,
-    _pluck_data,
-    ignore_docs,
-)
-from ...consts import ActorJobStatus, MetaOrigin
+from ..._utils import _catch_not_found_or_throw, _encode_webhook_list_to_base64, _pluck_data
 from ..base import ResourceClient, ResourceClientAsync
 from .run import RunClient, RunClientAsync
 from .run_collection import RunCollectionClient, RunCollectionClientAsync
 from .webhook_collection import WebhookCollectionClient, WebhookCollectionClientAsync
 
 
 def _get_task_representation(
@@ -90,15 +84,15 @@
             task_input=task_input,
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
             title=title,
         )
 
-        return self._update(_filter_out_none_values_recursively(task_representation))
+        return self._update(filter_out_none_values_recursively(task_representation))
 
     def delete(self) -> None:
         """Delete the task.
 
         https://docs.apify.com/api/v2#/reference/actor-tasks/task-object/delete-task
         """
         return self._delete()
@@ -150,15 +144,15 @@
             url=self._url('runs'),
             method='POST',
             headers={'content-type': 'application/json; charset=utf-8'},
             json=task_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     def call(
         self,
         *,
         task_input: Optional[Dict[str, Any]] = None,
         build: Optional[str] = None,
         memory_mbytes: Optional[int] = None,
@@ -248,16 +242,16 @@
         Returns:
             RunClient: The resource client for the last run of this task.
         """
         return RunClient(**self._sub_resource_init_options(
             resource_id='last',
             resource_path='runs',
             params=self._params(
-                status=_maybe_extract_enum_member_value(status),
-                origin=_maybe_extract_enum_member_value(origin),
+                status=maybe_extract_enum_member_value(status),
+                origin=maybe_extract_enum_member_value(origin),
             ),
         ))
 
     def webhooks(self) -> WebhookCollectionClient:
         """Retrieve a client for webhooks associated with this task."""
         return WebhookCollectionClient(**self._sub_resource_init_options())
 
@@ -313,15 +307,15 @@
             task_input=task_input,
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
             title=title,
         )
 
-        return await self._update(_filter_out_none_values_recursively(task_representation))
+        return await self._update(filter_out_none_values_recursively(task_representation))
 
     async def delete(self) -> None:
         """Delete the task.
 
         https://docs.apify.com/api/v2#/reference/actor-tasks/task-object/delete-task
         """
         return await self._delete()
@@ -373,15 +367,15 @@
             url=self._url('runs'),
             method='POST',
             headers={'content-type': 'application/json; charset=utf-8'},
             json=task_input,
             params=request_params,
         )
 
-        return _parse_date_fields(_pluck_data(response.json()))
+        return parse_date_fields(_pluck_data(response.json()))
 
     async def call(
         self,
         *,
         task_input: Optional[Dict[str, Any]] = None,
         build: Optional[str] = None,
         memory_mbytes: Optional[int] = None,
@@ -471,15 +465,15 @@
         Returns:
             RunClientAsync: The resource client for the last run of this task.
         """
         return RunClientAsync(**self._sub_resource_init_options(
             resource_id='last',
             resource_path='runs',
             params=self._params(
-                status=_maybe_extract_enum_member_value(status),
-                origin=_maybe_extract_enum_member_value(origin),
+                status=maybe_extract_enum_member_value(status),
+                origin=maybe_extract_enum_member_value(origin),
             ),
         ))
 
     def webhooks(self) -> WebhookCollectionClientAsync:
         """Retrieve a client for webhooks associated with this task."""
         return WebhookCollectionClientAsync(**self._sub_resource_init_options())
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/task_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .task import _get_task_representation
 
 
 class TaskCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating tasks."""
 
@@ -70,15 +72,15 @@
             task_input=task_input,
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
             title=title,
         )
 
-        return self._create(_filter_out_none_values_recursively(task_representation))
+        return self._create(filter_out_none_values_recursively(task_representation))
 
 
 class TaskCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating tasks."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -142,8 +144,8 @@
             task_input=task_input,
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
             title=title,
         )
 
-        return await self._create(_filter_out_none_values_recursively(task_representation))
+        return await self._create(filter_out_none_values_recursively(task_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/user.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ignore_docs
+from apify_shared.utils import ignore_docs
+
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class UserClient(ResourceClient):
     """Sub-client for querying user data."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from typing import Any, Dict, List, Optional
 
+from apify_shared.consts import WebhookEventType
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs, maybe_extract_enum_member_value, parse_date_fields
+
 from ..._errors import ApifyApiError
-from ..._utils import (
-    _catch_not_found_or_throw,
-    _filter_out_none_values_recursively,
-    _maybe_extract_enum_member_value,
-    _parse_date_fields,
-    _pluck_data,
-    ignore_docs,
-)
-from ...consts import WebhookEventType
+from ..._utils import _catch_not_found_or_throw, _pluck_data
 from ..base import ResourceClient, ResourceClientAsync
 from .webhook_dispatch_collection import WebhookDispatchCollectionClient, WebhookDispatchCollectionClientAsync
 
 
 def _get_webhook_representation(
     *,
     event_types: Optional[List[WebhookEventType]] = None,
@@ -42,15 +37,15 @@
         },
     }
 
     if actor_run_id is not None:
         webhook['isAdHoc'] = True
 
     if event_types is not None:
-        webhook['eventTypes'] = [_maybe_extract_enum_member_value(event_type) for event_type in event_types]
+        webhook['eventTypes'] = [maybe_extract_enum_member_value(event_type) for event_type in event_types]
 
     return webhook
 
 
 class WebhookClient(ResourceClient):
     """Sub-client for manipulating a single webhook."""
 
@@ -111,15 +106,15 @@
             actor_task_id=actor_task_id,
             actor_run_id=actor_run_id,
             ignore_ssl_errors=ignore_ssl_errors,
             do_not_retry=do_not_retry,
             is_ad_hoc=is_ad_hoc,
         )
 
-        return self._update(_filter_out_none_values_recursively(webhook_representation))
+        return self._update(filter_out_none_values_recursively(webhook_representation))
 
     def delete(self) -> None:
         """Delete the webhook.
 
         https://docs.apify.com/api/v2#/reference/webhooks/webhook-object/delete-webhook
         """
         return self._delete()
@@ -137,15 +132,15 @@
         try:
             response = self.http_client.call(
                 url=self._url('test'),
                 method='POST',
                 params=self._params(),
             )
 
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     def dispatches(self) -> WebhookDispatchCollectionClient:
@@ -221,15 +216,15 @@
             actor_task_id=actor_task_id,
             actor_run_id=actor_run_id,
             ignore_ssl_errors=ignore_ssl_errors,
             do_not_retry=do_not_retry,
             is_ad_hoc=is_ad_hoc,
         )
 
-        return await self._update(_filter_out_none_values_recursively(webhook_representation))
+        return await self._update(filter_out_none_values_recursively(webhook_representation))
 
     async def delete(self) -> None:
         """Delete the webhook.
 
         https://docs.apify.com/api/v2#/reference/webhooks/webhook-object/delete-webhook
         """
         return await self._delete()
@@ -247,15 +242,15 @@
         try:
             response = await self.http_client.call(
                 url=self._url('test'),
                 method='POST',
                 params=self._params(),
             )
 
-            return _parse_date_fields(_pluck_data(response.json()))
+            return parse_date_fields(_pluck_data(response.json()))
 
         except ApifyApiError as exc:
             _catch_not_found_or_throw(exc)
 
         return None
 
     def dispatches(self) -> WebhookDispatchCollectionClientAsync:
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Optional
 
-from apify_client.consts import WebhookEventType
+from apify_shared.consts import WebhookEventType
+from apify_shared.models import ListPage
+from apify_shared.utils import filter_out_none_values_recursively, ignore_docs
 
-from ..._utils import ListPage, _filter_out_none_values_recursively, ignore_docs
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 from .webhook import _get_webhook_representation
 
 
 class WebhookCollectionClient(ResourceCollectionClient):
     """Sub-client for manipulating webhooks."""
 
@@ -84,15 +85,15 @@
             actor_run_id=actor_run_id,
             ignore_ssl_errors=ignore_ssl_errors,
             do_not_retry=do_not_retry,
             idempotency_key=idempotency_key,
             is_ad_hoc=is_ad_hoc,
         )
 
-        return self._create(_filter_out_none_values_recursively(webhook_representation))
+        return self._create(filter_out_none_values_recursively(webhook_representation))
 
 
 class WebhookCollectionClientAsync(ResourceCollectionClientAsync):
     """Async sub-client for manipulating webhooks."""
 
     @ignore_docs
     def __init__(self, *args: Any, **kwargs: Any) -> None:
@@ -168,8 +169,8 @@
             actor_run_id=actor_run_id,
             ignore_ssl_errors=ignore_ssl_errors,
             do_not_retry=do_not_retry,
             idempotency_key=idempotency_key,
             is_ad_hoc=is_ad_hoc,
         )
 
-        return await self._create(_filter_out_none_values_recursively(webhook_representation))
+        return await self._create(filter_out_none_values_recursively(webhook_representation))
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_dispatch.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ignore_docs
+from apify_shared.utils import ignore_docs
+
 from ..base import ResourceClient, ResourceClientAsync
 
 
 class WebhookDispatchClient(ResourceClient):
     """Sub-client for querying information about a webhook dispatch."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional
 
-from ..._utils import ListPage, ignore_docs
+from apify_shared.models import ListPage
+from apify_shared.utils import ignore_docs
+
 from ..base import ResourceCollectionClient, ResourceCollectionClientAsync
 
 
 class WebhookDispatchCollectionClient(ResourceCollectionClient):
     """Sub-client for listing webhook dispatches."""
 
     @ignore_docs
```

### Comparing `apify_client-1.3.0b2/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.3.1b1/src/apify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.3.0b2
+Version: 1.3.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.3.0b2/src/apify_client.egg-info/SOURCES.txt` & `apify_client-1.3.1b1/src/apify_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 src/apify_client/__init__.py
 src/apify_client/_errors.py
 src/apify_client/_http_client.py
 src/apify_client/_logging.py
-src/apify_client/_types.py
 src/apify_client/_utils.py
 src/apify_client/client.py
 src/apify_client/consts.py
 src/apify_client/py.typed
 src/apify_client.egg-info/PKG-INFO
 src/apify_client.egg-info/SOURCES.txt
 src/apify_client.egg-info/dependency_links.txt
```

### Comparing `apify_client-1.3.0b2/src/apify_client.egg-info/requires.txt` & `apify_client-1.3.1b1/src/apify_client.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+apify-shared~=1.0.0
 httpx>=0.24.1
 
 [dev]
 autopep8~=2.0.2
 build~=0.10.0
 flake8~=6.0.0
 flake8-bugbear~=23.5.9
```

