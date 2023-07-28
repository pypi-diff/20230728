# Comparing `tmp/apify_client-1.3.1.tar.gz` & `tmp/apify_client-1.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.3.1.tar", last modified: Fri Jul 28 14:58:44 2023, max compression
+gzip compressed data, was "apify_client-1.3.1b1.tar", last modified: Fri Jul 28 14:48:15 2023, max compression
```

## Comparing `apify_client-1.3.1.tar` & `apify_client-1.3.1b1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.755310 apify_client-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-28 14:58:07.000000 apify_client-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-28 14:58:44.755310 apify_client-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-28 14:58:07.000000 apify_client-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-28 14:58:07.000000 apify_client-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:58:44.755310 apify_client-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.735309 apify_client-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.743309 apify_client-1.3.1/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.743309 apify_client-1.3.1/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.747310 apify_client-1.3.1/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.755310 apify_client-1.3.1/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30487 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    46397 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21007 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:07.000000 apify_client-1.3.1/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:58:44.743309 apify_client-1.3.1/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-28 14:58:44.000000 apify_client-1.3.1/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-28 14:58:44.000000 apify_client-1.3.1/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:58:44.000000 apify_client-1.3.1/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 14:58:44.000000 apify_client-1.3.1/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 14:58:44.000000 apify_client-1.3.1/src/apify_client.egg-info/top_level.txt
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

### Comparing `apify_client-1.3.1/LICENSE` & `apify_client-1.3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/PKG-INFO` & `apify_client-1.3.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.3.1
+Version: 1.3.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.3.1/README.md` & `apify_client-1.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/pyproject.toml` & `apify_client-1.3.1b1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,158 @@
 [project]
+
 name = "apify_client"
-version = "1.3.1"
+
+version = "1.3.1b1"
 description = "Apify API client for Python"
+
 readme = "README.md"
+
 license = {text = "Apache Software License"}
+
 authors = [
+
     {name = "Apify Technologies s.r.o.", email = "support@apify.com"},
+
 ]
+
 keywords = ["apify", "api", "client", "scraping", "automation"]
 
+
+
 classifiers = [
+
     "Development Status :: 5 - Production/Stable",
+
     "Intended Audience :: Developers",
+
     "License :: OSI Approved :: Apache Software License",
+
     "Operating System :: OS Independent",
+
     "Programming Language :: Python :: 3.8",
+
     "Programming Language :: Python :: 3.9",
+
     "Programming Language :: Python :: 3.10",
+
     "Programming Language :: Python :: 3.11",
+
     "Topic :: Software Development :: Libraries",
+
 ]
 
+
+
 requires-python = ">=3.8"
+
 dependencies = [
+
     "apify-shared ~= 1.0.0",
+
     "httpx >= 0.24.1",
+
 ]
 
+
+
 [project.optional-dependencies]
+
 dev = [
+
     "autopep8 ~= 2.0.2",
+
     "build ~= 0.10.0",
+
     "flake8 ~= 6.0.0",
+
     "flake8-bugbear ~= 23.5.9",
+
     "flake8-commas ~= 2.1.0",
+
     "flake8-comprehensions ~= 3.12.0",
+
     "flake8-datetimez ~= 20.10.0",
+
     "flake8-docstrings ~= 1.7.0",
+
     "flake8-encodings ~= 0.5.0",
+
     "flake8-isort ~= 6.0.0",
+
     "flake8-noqa ~= 1.3.1",
+
     "flake8-pytest-style ~= 1.7.2",
+
     "flake8-quotes ~= 3.3.2",
+
     "flake8-unused-arguments ~= 0.0.13",
+
     "isort ~= 5.12.0",
+
     "mypy ~= 1.3.0",
+
     "pep8-naming ~= 0.13.3",
+
     "pre-commit ~= 3.3.2",
+
     "pytest ~= 7.3.1",
+
     "pytest-asyncio ~= 0.21.0",
+
     "pytest-only ~= 2.0.0",
+
     "pytest-randomly ~= 3.12.0",
+
     "pytest-timeout ~= 2.1.0",
+
     "pytest-xdist ~= 3.3.1",
+
     "redbaron ~= 0.9.2",
+
     "sphinx ~= 6.1.3",
+
     "sphinx-autodoc-typehints ~= 1.22",
+
     "sphinx-markdown-builder == 0.5.4",
+
     "twine ~= 4.0.2",
+
 ]
 
+
+
 [project.urls]
+
 "Homepage" = "https://docs.apify.com/api/client/python/"
+
 "Documentation" = "https://docs.apify.com/api/client/python/"
+
 "Source" = "https://github.com/apify/apify-client-python"
+
 "Issue tracker" = "https://github.com/apify/apify-client-python/issues"
+
 "Changelog" = "https://github.com/apify/apify-client-python/blob/master/CHANGELOG.md"
+
 "Apify Homepage" = "https://apify.com"
 
+
+
 [build-system]
+
 requires = ["setuptools>=64.0.0", "wheel"]
+
 build-backend = "setuptools.build_meta"
 
+
+
 [tool.setuptools.packages.find]
+
 where = ["src"]
+
 include = ["apify_client*"]
 
+
+
 [tool.setuptools.package-data]
+
 apify_client = ["py.typed"]
```

### Comparing `apify_client-1.3.1/src/apify_client/_errors.py` & `apify_client-1.3.1b1/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/_http_client.py` & `apify_client-1.3.1b1/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/_logging.py` & `apify_client-1.3.1b1/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/_utils.py` & `apify_client-1.3.1b1/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/client.py` & `apify_client-1.3.1b1/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/__init__.py` & `apify_client-1.3.1b1/src/apify_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/base/actor_job_base_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/actor_job_base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/base/base_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/base/resource_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/resource_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/base/resource_collection_client.py` & `apify_client-1.3.1b1/src/apify_client/clients/base/resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/__init__.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_env_var.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_env_var_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_version.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/actor_version_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/actor_version_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/build.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/build_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/build_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/dataset.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/dataset_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/key_value_store.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/key_value_store_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/log.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/log.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/request_queue.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/request_queue_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/run.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/run_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/run_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/schedule.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/schedule_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/schedule_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/task.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/task_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/task_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/user.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/user.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_dispatch.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py` & `apify_client-1.3.1b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client/consts.py` & `apify_client-1.3.1b1/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.3.1b1/src/apify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.3.1
+Version: 1.3.1b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.3.1/src/apify_client.egg-info/SOURCES.txt` & `apify_client-1.3.1b1/src/apify_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify_client-1.3.1/src/apify_client.egg-info/requires.txt` & `apify_client-1.3.1b1/src/apify_client.egg-info/requires.txt`

 * *Files identical despite different names*

