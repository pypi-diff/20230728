# Comparing `tmp/stability-sdk-0.8.3.tar.gz` & `tmp/stability-sdk-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.8.3.tar", last modified: Fri Jun 30 14:18:41 2023, max compression
+gzip compressed data, was "stability-sdk-0.8.4.tar", last modified: Fri Jul 28 14:22:15 2023, max compression
```

## Comparing `stability-sdk-0.8.3.tar` & `stability-sdk-0.8.4.tar`

### file list

```diff
@@ -1,56 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.019077 stability-sdk-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55475 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    37904 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/animation_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-30 14:18:23.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 14:18:24.000000 stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.023077 stability-sdk-0.8.3/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 14:18:41.000000 stability-sdk-0.8.3/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:18:41.027077 stability-sdk-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_animator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-30 14:18:21.000000 stability-sdk-0.8.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.800111 stability-sdk-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-28 14:22:15.800111 stability-sdk-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:22:15.800111 stability-sdk-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55475 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37904 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/animation_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25770 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/finetuning/finetuning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/finetuning/finetuning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40797 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4121 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-07-28 14:21:56.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/ATTIC/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/examples/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/examples/hf_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/examples/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/_wide_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26472 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/stream_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-28 14:21:57.000000 stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tests/test_stream_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.792111 stability-sdk-0.8.4/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-28 14:22:15.000000 stability-sdk-0.8.4/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-28 14:22:15.000000 stability-sdk-0.8.4/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:22:15.000000 stability-sdk-0.8.4/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-28 14:22:15.000000 stability-sdk-0.8.4/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 14:22:15.000000 stability-sdk-0.8.4/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:22:15.796111 stability-sdk-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/tests/test_animator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-28 14:21:54.000000 stability-sdk-0.8.4/tests/test_utils.py
```

### Comparing `stability-sdk-0.8.3/LICENSE` & `stability-sdk-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/PKG-INFO` & `stability-sdk-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.8.3/README.md` & `stability-sdk-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/setup.py` & `stability-sdk-0.8.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.8.3',
+    version='0.8.4',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
     description='Python SDK for interacting with stability.ai APIs',
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/__main__.py` & `stability-sdk-0.8.4/src/stability_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/animation.py` & `stability-sdk-0.8.4/src/stability_sdk/animation.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         ]
     )
     model = param.Selector(
         default=DEFAULT_MODEL, 
         check_on_set=False, # allow old and new models without raising ValueError
         objects=[
             "stable-diffusion-v1-5", "stable-diffusion-512-v2-1", "stable-diffusion-768-v2-1", 
-            "stable-diffusion-depth-v2-0", "stable-diffusion-xl-beta-v2-2-2", "stable-diffusion-xl-1024-v0-9",
+            "stable-diffusion-depth-v2-0", "stable-diffusion-xl-beta-v2-2-2", "stable-diffusion-xl-1024-v1-0",
             "custom"
         ]
     )
     custom_model = param.String(default="", doc="Identifier of custom model to use.")
     seed = param.Integer(default=-1, doc="Provide a seed value for more deterministic behavior. Negative seed values will be replaced with a random seed (default).")
     cfg_scale = param.Number(default=7, softbounds=(0,20), doc="Classifier-free guidance scale. Strength of prompt influence on denoising process. `cfg_scale=0` gives unconditioned sampling.")
     clip_guidance = param.Selector(default='None', objects=["None", "Simple", "FastBlue", "FastGreen"], doc="CLIP-guidance preset.")
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/animation_ui.py` & `stability-sdk-0.8.4/src/stability_sdk/animation_ui.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/api.py` & `stability-sdk-0.8.4/src/stability_sdk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class Context:
     def __init__(
             self, 
             host: str="", 
             api_key: str=None, 
             stub: generation_grpc.GenerationServiceStub=None,
-            generate_engine_id: str="stable-diffusion-xl-1024-v0-9",
+            generate_engine_id: str="stable-diffusion-xl-1024-v1-0",
             inpaint_engine_id: str="stable-inpainting-512-v2-0",
             interpolate_engine_id: str="interpolation-server-v1",
             transform_engine_id: str="transform-server-v1",
             upscale_engine_id: str="esrgan-v1-x2plus",
         ):
         if not host and stub is None:
             raise Exception("Must provide either GRPC host or stub to Api")
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/client.py` & `stability-sdk-0.8.4/src/stability_sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 
 class StabilityInference:
     def __init__(
         self,
         host: str = "grpc.stability.ai:443",
         key: str = "",
-        engine: str = "stable-diffusion-xl-1024-v0-9",
+        engine: str = "stable-diffusion-xl-1024-v1-0",
         upscale_engine: str = "esrgan-v1-x2plus",
         verbose: bool = False,
         wait_for_ready: bool = True,
     ):
         """
         Initialize the client.
 
@@ -167,14 +167,17 @@
         safety: bool = True,
         classifiers: Optional[generation.ClassifierParameters] = None,
         guidance_preset: generation.GuidancePreset = generation.GUIDANCE_PRESET_NONE,
         guidance_cuts: int = 0,
         guidance_strength: Optional[float] = None,
         guidance_prompt: Union[str, generation.Prompt] = None,
         guidance_models: List[str] = None,
+        adapter_type: generation.T2IAdapter = None,
+        adapter_strength: float = 0.4,
+        adapter_init_type: generation.T2IAdapterInit = generation.T2IADAPTERINIT_IMAGE,
         style_preset: Optional[str] = None
     ) -> Generator[generation.Answer, None, None]:
         """
         Generate images from a prompt.
 
         :param prompt: Prompt to generate images from.
         :param init_image: Init image.
@@ -191,14 +194,18 @@
         :param safety: DEPRECATED/UNUSED - Cannot be disabled.
         :param classifiers: DEPRECATED/UNUSED - Has no effect on image generation.
         :param guidance_preset: Guidance preset to use. See generation.GuidancePreset for supported values.
         :param guidance_cuts: Number of cuts to use for guidance.
         :param guidance_strength: Strength of the guidance. We recommend values in range [0.0,1.0]. A good default is 0.25
         :param guidance_prompt: Prompt to use for guidance, defaults to `prompt` argument (above) if not specified.
         :param guidance_models: Models to use for guidance.
+        :param adapter_type: T2I adapter type, if any.
+        :param adapter_strength: Float between 0, 1 representing the proportion of unet passes into which we inject adapter weights
+        :param adapter_init_type: If T2IADAPTERINIT_IMAGE then init_image is converted into an initialising image corresponding to the adapter_type. i.e.
+        a sketch/depthmap/canny edge. If T2IADAPTERINIT_ADAPTER_IMAGE, then the init_image is treated as already a a sketch/depthmap/canny edge.
         :param style_preset: Style preset name to use (see https://platform.stability.ai/rest-api#tag/v1generation)
         :return: Generator of Answer objects.
         """
         if (prompt is None) and (init_image is None):
             raise ValueError("prompt and/or init_image must be provided")
 
         if (mask_image is not None) and (init_image is None):
@@ -243,16 +250,15 @@
         if guidance_prompt:
             if isinstance(guidance_prompt, str):
                 guidance_prompt = generation.Prompt(text=guidance_prompt)
             elif not isinstance(guidance_prompt, generation.Prompt):
                 raise ValueError("guidance_prompt must be a string or Prompt object")
         if guidance_strength == 0.0:
             guidance_strength = None
-
-
+        
         # Build our CLIP parameters
         if guidance_preset is not generation.GUIDANCE_PRESET_NONE:
             # to do: make it so user can override this
             step_parameters['sampler']=None
 
             if guidance_models:
                 guiders = [generation.Model(alias=model) for model in guidance_models]
@@ -272,25 +278,32 @@
                         models=guiders,
                         cutouts=cutouts,
                         prompt=guidance_prompt,
                     )
                 ],
             )
 
+        adapter_parameters = generation.T2IAdapterParameter(
+            adapter_type = adapter_type,
+            adapter_strength = adapter_strength,
+            adapter_init_type = adapter_init_type,
+        )
+
         transform=None
         if sampler:
             transform=generation.TransformType(diffusion=sampler)
 
         image_parameters=generation.ImageParameters(
             transform=transform,
             height=height,
             width=width,
             seed=seed,
             steps=steps,
             samples=samples,
+            adapter=adapter_parameters,
             parameters=[generation.StepParameter(**step_parameters)],
         )
 
         if style_preset and style_preset.lower() != 'none':
             extras = Struct()
             extras.update({ '$IPC': { "preset": style_preset } })
         else:
@@ -556,15 +569,15 @@
     )
     parser_generate.add_argument("--show", action="store_true", help="open artifacts using PIL")
     parser_generate.add_argument(
         "--engine",
         "-e",
         type=str,
         help="engine to use for inference",
-        default="stable-diffusion-xl-1024-v0-9",
+        default="stable-diffusion-xl-1024-v1-0",
     )
     parser_generate.add_argument(
         "--init_image",
         "-i",
         type=str,
         help="Init image",
     )
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rengines.proto\x12\x07gooseai\"\xa9\x01\n\nEngineInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\r\n\x05ready\x18\x03 \x01(\x08\x12!\n\x04type\x18\x04 \x01(\x0e\x32\x13.gooseai.EngineType\x12+\n\ttokenizer\x18\x05 \x01(\x0e\x32\x18.gooseai.EngineTokenizer\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x14\n\x12ListEnginesRequest\".\n\x07\x45ngines\x12#\n\x06\x65ngine\x18\x01 \x03(\x0b\x32\x13.gooseai.EngineInfo*Z\n\nEngineType\x12\x08\n\x04TEXT\x10\x00\x12\x0b\n\x07PICTURE\x10\x01\x12\t\n\x05\x41UDIO\x10\x02\x12\t\n\x05VIDEO\x10\x03\x12\x12\n\x0e\x43LASSIFICATION\x10\x04\x12\x0b\n\x07STORAGE\x10\x05*%\n\x0f\x45ngineTokenizer\x12\x08\n\x04GPT2\x10\x00\x12\x08\n\x04PILE\x10\x01\x32P\n\x0e\x45nginesService\x12>\n\x0bListEngines\x12\x1b.gooseai.ListEnginesRequest\x1a\x10.gooseai.Engines\"\x00\x42\x38Z6github.com/stability-ai/api-interfaces/gooseai/enginesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rengines.proto\x12\x07gooseai\"\xc0\x01\n\nEngineInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\r\n\x05ready\x18\x03 \x01(\x08\x12!\n\x04type\x18\x04 \x01(\x0e\x32\x13.gooseai.EngineType\x12+\n\ttokenizer\x18\x05 \x01(\x0e\x32\x18.gooseai.EngineTokenizer\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x15\n\rcan_fine_tune\x18\x08 \x01(\x08\"\x14\n\x12ListEnginesRequest\".\n\x07\x45ngines\x12#\n\x06\x65ngine\x18\x01 \x03(\x0b\x32\x13.gooseai.EngineInfo*Z\n\nEngineType\x12\x08\n\x04TEXT\x10\x00\x12\x0b\n\x07PICTURE\x10\x01\x12\t\n\x05\x41UDIO\x10\x02\x12\t\n\x05VIDEO\x10\x03\x12\x12\n\x0e\x43LASSIFICATION\x10\x04\x12\x0b\n\x07STORAGE\x10\x05*%\n\x0f\x45ngineTokenizer\x12\x08\n\x04GPT2\x10\x00\x12\x08\n\x04PILE\x10\x01\x32P\n\x0e\x45nginesService\x12>\n\x0bListEngines\x12\x1b.gooseai.ListEnginesRequest\x1a\x10.gooseai.Engines\"\x00\x42\x38Z6github.com/stability-ai/api-interfaces/gooseai/enginesb\x06proto3')
 
 _ENGINETYPE = DESCRIPTOR.enum_types_by_name['EngineType']
 EngineType = enum_type_wrapper.EnumTypeWrapper(_ENGINETYPE)
 _ENGINETOKENIZER = DESCRIPTOR.enum_types_by_name['EngineTokenizer']
 EngineTokenizer = enum_type_wrapper.EnumTypeWrapper(_ENGINETOKENIZER)
 TEXT = 0
 PICTURE = 1
@@ -56,20 +56,20 @@
 _sym_db.RegisterMessage(Engines)
 
 _ENGINESSERVICE = DESCRIPTOR.services_by_name['EnginesService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z6github.com/stability-ai/api-interfaces/gooseai/engines'
-  _ENGINETYPE._serialized_start=268
-  _ENGINETYPE._serialized_end=358
-  _ENGINETOKENIZER._serialized_start=360
-  _ENGINETOKENIZER._serialized_end=397
+  _ENGINETYPE._serialized_start=291
+  _ENGINETYPE._serialized_end=381
+  _ENGINETOKENIZER._serialized_start=383
+  _ENGINETOKENIZER._serialized_end=420
   _ENGINEINFO._serialized_start=27
-  _ENGINEINFO._serialized_end=196
-  _LISTENGINESREQUEST._serialized_start=198
-  _LISTENGINESREQUEST._serialized_end=218
-  _ENGINES._serialized_start=220
-  _ENGINES._serialized_end=266
-  _ENGINESSERVICE._serialized_start=399
-  _ENGINESSERVICE._serialized_end=479
+  _ENGINEINFO._serialized_end=219
+  _LISTENGINESREQUEST._serialized_start=221
+  _LISTENGINESREQUEST._serialized_end=241
+  _ENGINES._serialized_start=243
+  _ENGINES._serialized_end=289
+  _ENGINESSERVICE._serialized_start=422
+  _ENGINESSERVICE._serialized_end=502
 # @@protoc_insertion_point(module_scope)
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 import tensors_pb2 as tensors__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\x1cgoogle/protobuf/struct.proto\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xd7\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x12\x1d\n\x10step_noise_scale\x18\x07 \x01(\x02H\x06\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scaleB\x13\n\x11_step_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\xbd\x03\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x06\x88\x01\x01\x12\x15\n\x08quantize\x18\n \x01(\x08H\x07\x88\x01\x01\x42\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_initB\x10\n\x0e_weight_methodB\x0b\n\t_quantize\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"]\n\x15InterpolateParameters\x12\x0e\n\x06ratios\x18\x01 \x03(\x02\x12+\n\x04mode\x18\x02 \x01(\x0e\x32\x18.gooseai.InterpolateModeH\x00\x88\x01\x01\x42\x07\n\x05_mode\"\x9c\x03\n\x14TransformColorAdjust\x12\x17\n\nbrightness\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x15\n\x08\x63ontrast\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x10\n\x03hue\x18\x03 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsaturation\x18\x04 \x01(\x02H\x03\x88\x01\x01\x12\x16\n\tlightness\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12+\n\x0bmatch_image\x18\x06 \x01(\x0b\x32\x11.gooseai.ArtifactH\x05\x88\x01\x01\x12\x30\n\nmatch_mode\x18\x07 \x01(\x0e\x32\x17.gooseai.ColorMatchModeH\x06\x88\x01\x01\x12\x19\n\x0cnoise_amount\x18\x08 \x01(\x02H\x07\x88\x01\x01\x12\x17\n\nnoise_seed\x18\t \x01(\rH\x08\x88\x01\x01\x42\r\n\x0b_brightnessB\x0b\n\t_contrastB\x06\n\x04_hueB\r\n\x0b_saturationB\x0c\n\n_lightnessB\x0e\n\x0c_match_imageB\r\n\x0b_match_modeB\x0f\n\r_noise_amountB\r\n\x0b_noise_seed\"\x8c\x01\n\x12TransformDepthCalc\x12\x19\n\x0c\x62lend_weight\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0b\x62lur_radius\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07reverse\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x0f\n\r_blend_weightB\x0e\n\x0c_blur_radiusB\n\n\x08_reverse\"#\n\x0fTransformMatrix\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\x86\x02\n\x11TransformResample\x12(\n\x0b\x62order_mode\x18\x01 \x01(\x0e\x32\x13.gooseai.BorderMode\x12+\n\ttransform\x18\x02 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x35\n\x0eprev_transform\x18\x03 \x01(\x0b\x32\x18.gooseai.TransformMatrixH\x00\x88\x01\x01\x12\x17\n\ndepth_warp\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x18\n\x0b\x65xport_mask\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x11\n\x0f_prev_transformB\r\n\x0b_depth_warpB\x0e\n\x0c_export_mask\"}\n\x10\x43\x61meraParameters\x12(\n\x0b\x63\x61mera_type\x18\x01 \x01(\x0e\x32\x13.gooseai.CameraType\x12\x12\n\nnear_plane\x18\x02 \x01(\x02\x12\x11\n\tfar_plane\x18\x03 \x01(\x02\x12\x10\n\x03\x66ov\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x06\n\x04_fov\"\xd9\x01\n\x13TransformCameraPose\x12\x36\n\x14world_to_view_matrix\x18\x01 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x34\n\x11\x63\x61mera_parameters\x18\x02 \x01(\x0b\x32\x19.gooseai.CameraParameters\x12\x12\n\ndo_prefill\x18\x05 \x01(\x08\x12(\n\x0brender_mode\x18\x08 \x01(\x0e\x32\x13.gooseai.RenderModeJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xf1\x01\n\x13TransformParameters\x12\x35\n\x0c\x63olor_adjust\x18\x02 \x01(\x0b\x32\x1d.gooseai.TransformColorAdjustH\x00\x12\x31\n\ndepth_calc\x18\x04 \x01(\x0b\x32\x1b.gooseai.TransformDepthCalcH\x00\x12.\n\x08resample\x18\x05 \x01(\x0b\x32\x1a.gooseai.TransformResampleH\x00\x12\x33\n\x0b\x63\x61mera_pose\x18\x06 \x01(\x0b\x32\x1c.gooseai.TransformCameraPoseH\x00\x42\x0b\n\ttransform\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"A\n\x0b\x41nswerBatch\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12 \n\x07\x61nswers\x18\x02 \x03(\x0b\x32\x0f.gooseai.Answer\"\x8f\x04\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x35\n\x0binterpolate\x18\x0b \x01(\x0b\x32\x1e.gooseai.InterpolateParametersH\x00\x12\x31\n\ttransform\x18\x0c \x01(\x0b\x32\x1c.gooseai.TransformParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12-\n\x06\x65xtras\x18\xff\x0f \x01(\x0b\x32\x17.google.protobuf.StructH\x02\x88\x01\x01\x42\x08\n\x06paramsB\x0e\n\x0c_conditionerB\t\n\x07_extrasJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xf8\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t\x12\x12\n\x0e\x41RTIFACT_DEPTH\x10\n*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\x98\x02\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t\x12\x17\n\x13SAMPLER_K_DPMPP_SDE\x10\n*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*\x8c\x01\n\x0fInterpolateMode\x12\x16\n\x12INTERPOLATE_LINEAR\x10\x00\x12\x14\n\x10INTERPOLATE_RIFE\x10\x01\x12\x1a\n\x16INTERPOLATE_VAE_LINEAR\x10\x02\x12\x19\n\x15INTERPOLATE_VAE_SLERP\x10\x03\x12\x14\n\x10INTERPOLATE_FILM\x10\x04*l\n\nBorderMode\x12\x12\n\x0e\x42ORDER_REFLECT\x10\x00\x12\x14\n\x10\x42ORDER_REPLICATE\x10\x01\x12\x0f\n\x0b\x42ORDER_WRAP\x10\x02\x12\x0f\n\x0b\x42ORDER_ZERO\x10\x03\x12\x12\n\x0e\x42ORDER_PREFILL\x10\x04*O\n\x0e\x43olorMatchMode\x12\x13\n\x0f\x43OLOR_MATCH_HSV\x10\x00\x12\x13\n\x0f\x43OLOR_MATCH_LAB\x10\x01\x12\x13\n\x0f\x43OLOR_MATCH_RGB\x10\x02*=\n\nCameraType\x12\x16\n\x12\x43\x41MERA_PERSPECTIVE\x10\x00\x12\x17\n\x13\x43\x41MERA_ORTHOGRAPHIC\x10\x01*4\n\nRenderMode\x12\x0f\n\x0bRENDER_MESH\x10\x00\x12\x15\n\x11RENDER_POINTCLOUD\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42;Z9github.com/stability-ai/api-interfaces/gooseai/generationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\x1cgoogle/protobuf/struct.proto\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xd7\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x12\x1d\n\x10step_noise_scale\x18\x07 \x01(\x02H\x06\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scaleB\x13\n\x11_step_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\x8e\x01\n\x13T2IAdapterParameter\x12)\n\x0c\x61\x64\x61pter_type\x18\x01 \x01(\x0e\x32\x13.gooseai.T2IAdapter\x12\x18\n\x10\x61\x64\x61pter_strength\x18\x02 \x01(\x02\x12\x32\n\x11\x61\x64\x61pter_init_type\x18\x03 \x01(\x0e\x32\x17.gooseai.T2IAdapterInit\"\xb6\x01\n\rCAIParameters\x12>\n\x0emodel_metadata\x18\x01 \x01(\x0e\x32$.gooseai.CAIParameters.ModelMetadataH\x00\"W\n\rModelMetadata\x12\x1e\n\x1aMODEL_METADATA_UNSPECIFIED\x10\x00\x12&\n\"MODEL_METADATA_SIGN_WITH_ENGINE_ID\x10\x01\x42\x0c\n\nparameters\"H\n\x14\x46ineTuningParameters\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\t\n\x07_weight\"\x84\x05\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x06\x88\x01\x01\x12\x15\n\x08quantize\x18\n \x01(\x08H\x07\x88\x01\x01\x12\x33\n\x0e\x63\x61i_parameters\x18\x0b \x01(\x0b\x32\x16.gooseai.CAIParametersH\x08\x88\x01\x01\x12\x32\n\x07\x61\x64\x61pter\x18\x0c \x01(\x0b\x32\x1c.gooseai.T2IAdapterParameterH\t\x88\x01\x01\x12=\n\x16\x66ine_tuning_parameters\x18\r \x03(\x0b\x32\x1d.gooseai.FineTuningParametersB\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_initB\x10\n\x0e_weight_methodB\x0b\n\t_quantizeB\x11\n\x0f_cai_parametersB\n\n\x08_adapter\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"]\n\x15InterpolateParameters\x12\x0e\n\x06ratios\x18\x01 \x03(\x02\x12+\n\x04mode\x18\x02 \x01(\x0e\x32\x18.gooseai.InterpolateModeH\x00\x88\x01\x01\x42\x07\n\x05_mode\"\x9c\x03\n\x14TransformColorAdjust\x12\x17\n\nbrightness\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x15\n\x08\x63ontrast\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x10\n\x03hue\x18\x03 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsaturation\x18\x04 \x01(\x02H\x03\x88\x01\x01\x12\x16\n\tlightness\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12+\n\x0bmatch_image\x18\x06 \x01(\x0b\x32\x11.gooseai.ArtifactH\x05\x88\x01\x01\x12\x30\n\nmatch_mode\x18\x07 \x01(\x0e\x32\x17.gooseai.ColorMatchModeH\x06\x88\x01\x01\x12\x19\n\x0cnoise_amount\x18\x08 \x01(\x02H\x07\x88\x01\x01\x12\x17\n\nnoise_seed\x18\t \x01(\rH\x08\x88\x01\x01\x42\r\n\x0b_brightnessB\x0b\n\t_contrastB\x06\n\x04_hueB\r\n\x0b_saturationB\x0c\n\n_lightnessB\x0e\n\x0c_match_imageB\r\n\x0b_match_modeB\x0f\n\r_noise_amountB\r\n\x0b_noise_seed\"\x8c\x01\n\x12TransformDepthCalc\x12\x19\n\x0c\x62lend_weight\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0b\x62lur_radius\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07reverse\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x0f\n\r_blend_weightB\x0e\n\x0c_blur_radiusB\n\n\x08_reverse\"#\n\x0fTransformMatrix\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\x86\x02\n\x11TransformResample\x12(\n\x0b\x62order_mode\x18\x01 \x01(\x0e\x32\x13.gooseai.BorderMode\x12+\n\ttransform\x18\x02 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x35\n\x0eprev_transform\x18\x03 \x01(\x0b\x32\x18.gooseai.TransformMatrixH\x00\x88\x01\x01\x12\x17\n\ndepth_warp\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x18\n\x0b\x65xport_mask\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x11\n\x0f_prev_transformB\r\n\x0b_depth_warpB\x0e\n\x0c_export_mask\"}\n\x10\x43\x61meraParameters\x12(\n\x0b\x63\x61mera_type\x18\x01 \x01(\x0e\x32\x13.gooseai.CameraType\x12\x12\n\nnear_plane\x18\x02 \x01(\x02\x12\x11\n\tfar_plane\x18\x03 \x01(\x02\x12\x10\n\x03\x66ov\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x06\n\x04_fov\"\xd9\x01\n\x13TransformCameraPose\x12\x36\n\x14world_to_view_matrix\x18\x01 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x34\n\x11\x63\x61mera_parameters\x18\x02 \x01(\x0b\x32\x19.gooseai.CameraParameters\x12\x12\n\ndo_prefill\x18\x05 \x01(\x08\x12(\n\x0brender_mode\x18\x08 \x01(\x0e\x32\x13.gooseai.RenderModeJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xf1\x01\n\x13TransformParameters\x12\x35\n\x0c\x63olor_adjust\x18\x02 \x01(\x0b\x32\x1d.gooseai.TransformColorAdjustH\x00\x12\x31\n\ndepth_calc\x18\x04 \x01(\x0b\x32\x1b.gooseai.TransformDepthCalcH\x00\x12.\n\x08resample\x18\x05 \x01(\x0b\x32\x1a.gooseai.TransformResampleH\x00\x12\x33\n\x0b\x63\x61mera_pose\x18\x06 \x01(\x0b\x32\x1c.gooseai.TransformCameraPoseH\x00\x42\x0b\n\ttransform\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"A\n\x0b\x41nswerBatch\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12 \n\x07\x61nswers\x18\x02 \x03(\x0b\x32\x0f.gooseai.Answer\"\x8f\x04\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x35\n\x0binterpolate\x18\x0b \x01(\x0b\x32\x1e.gooseai.InterpolateParametersH\x00\x12\x31\n\ttransform\x18\x0c \x01(\x0b\x32\x1c.gooseai.TransformParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12-\n\x06\x65xtras\x18\xff\x0f \x01(\x0b\x32\x17.google.protobuf.StructH\x02\x88\x01\x01\x42\x08\n\x06paramsB\x0e\n\x0c_conditionerB\t\n\x07_extrasJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xf8\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t\x12\x12\n\x0e\x41RTIFACT_DEPTH\x10\n*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\x98\x02\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t\x12\x17\n\x13SAMPLER_K_DPMPP_SDE\x10\n*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*d\n\nT2IAdapter\x12\x13\n\x0fT2IADAPTER_NONE\x10\x00\x12\x15\n\x11T2IADAPTER_SKETCH\x10\x01\x12\x14\n\x10T2IADAPTER_DEPTH\x10\x02\x12\x14\n\x10T2IADAPTER_CANNY\x10\x03*L\n\x0eT2IAdapterInit\x12\x18\n\x14T2IADAPTERINIT_IMAGE\x10\x00\x12 \n\x1cT2IADAPTERINIT_ADAPTER_IMAGE\x10\x01*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*\x8c\x01\n\x0fInterpolateMode\x12\x16\n\x12INTERPOLATE_LINEAR\x10\x00\x12\x14\n\x10INTERPOLATE_RIFE\x10\x01\x12\x1a\n\x16INTERPOLATE_VAE_LINEAR\x10\x02\x12\x19\n\x15INTERPOLATE_VAE_SLERP\x10\x03\x12\x14\n\x10INTERPOLATE_FILM\x10\x04*l\n\nBorderMode\x12\x12\n\x0e\x42ORDER_REFLECT\x10\x00\x12\x14\n\x10\x42ORDER_REPLICATE\x10\x01\x12\x0f\n\x0b\x42ORDER_WRAP\x10\x02\x12\x0f\n\x0b\x42ORDER_ZERO\x10\x03\x12\x12\n\x0e\x42ORDER_PREFILL\x10\x04*O\n\x0e\x43olorMatchMode\x12\x13\n\x0f\x43OLOR_MATCH_HSV\x10\x00\x12\x13\n\x0f\x43OLOR_MATCH_LAB\x10\x01\x12\x13\n\x0f\x43OLOR_MATCH_RGB\x10\x02*=\n\nCameraType\x12\x16\n\x12\x43\x41MERA_PERSPECTIVE\x10\x00\x12\x17\n\x13\x43\x41MERA_ORTHOGRAPHIC\x10\x01*4\n\nRenderMode\x12\x0f\n\x0bRENDER_MESH\x10\x00\x12\x15\n\x11RENDER_POINTCLOUD\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42;Z9github.com/stability-ai/api-interfaces/gooseai/generationb\x06proto3')
 
 _FINISHREASON = DESCRIPTOR.enum_types_by_name['FinishReason']
 FinishReason = enum_type_wrapper.EnumTypeWrapper(_FINISHREASON)
 _ARTIFACTTYPE = DESCRIPTOR.enum_types_by_name['ArtifactType']
 ArtifactType = enum_type_wrapper.EnumTypeWrapper(_ARTIFACTTYPE)
 _MASKEDAREAINIT = DESCRIPTOR.enum_types_by_name['MaskedAreaInit']
 MaskedAreaInit = enum_type_wrapper.EnumTypeWrapper(_MASKEDAREAINIT)
@@ -31,14 +31,18 @@
 DiffusionSampler = enum_type_wrapper.EnumTypeWrapper(_DIFFUSIONSAMPLER)
 _UPSCALER = DESCRIPTOR.enum_types_by_name['Upscaler']
 Upscaler = enum_type_wrapper.EnumTypeWrapper(_UPSCALER)
 _GUIDANCEPRESET = DESCRIPTOR.enum_types_by_name['GuidancePreset']
 GuidancePreset = enum_type_wrapper.EnumTypeWrapper(_GUIDANCEPRESET)
 _MODELARCHITECTURE = DESCRIPTOR.enum_types_by_name['ModelArchitecture']
 ModelArchitecture = enum_type_wrapper.EnumTypeWrapper(_MODELARCHITECTURE)
+_T2IADAPTER = DESCRIPTOR.enum_types_by_name['T2IAdapter']
+T2IAdapter = enum_type_wrapper.EnumTypeWrapper(_T2IADAPTER)
+_T2IADAPTERINIT = DESCRIPTOR.enum_types_by_name['T2IAdapterInit']
+T2IAdapterInit = enum_type_wrapper.EnumTypeWrapper(_T2IADAPTERINIT)
 _ACTION = DESCRIPTOR.enum_types_by_name['Action']
 Action = enum_type_wrapper.EnumTypeWrapper(_ACTION)
 _CLASSIFIERMODE = DESCRIPTOR.enum_types_by_name['ClassifierMode']
 ClassifierMode = enum_type_wrapper.EnumTypeWrapper(_CLASSIFIERMODE)
 _INTERPOLATEMODE = DESCRIPTOR.enum_types_by_name['InterpolateMode']
 InterpolateMode = enum_type_wrapper.EnumTypeWrapper(_INTERPOLATEMODE)
 _BORDERMODE = DESCRIPTOR.enum_types_by_name['BorderMode']
@@ -97,14 +101,20 @@
 GUIDANCE_PRESET_SLOW = 4
 GUIDANCE_PRESET_SLOWER = 5
 GUIDANCE_PRESET_SLOWEST = 6
 MODEL_ARCHITECTURE_NONE = 0
 MODEL_ARCHITECTURE_CLIP_VIT = 1
 MODEL_ARCHITECTURE_CLIP_RESNET = 2
 MODEL_ARCHITECTURE_LDM = 3
+T2IADAPTER_NONE = 0
+T2IADAPTER_SKETCH = 1
+T2IADAPTER_DEPTH = 2
+T2IADAPTER_CANNY = 3
+T2IADAPTERINIT_IMAGE = 0
+T2IADAPTERINIT_ADAPTER_IMAGE = 1
 ACTION_PASSTHROUGH = 0
 ACTION_REGENERATE_DUPLICATE = 1
 ACTION_REGENERATE = 2
 ACTION_OBFUSCATE_DUPLICATE = 3
 ACTION_OBFUSCATE = 4
 ACTION_DISCARD = 5
 CLSFR_MODE_ZEROSHOT = 0
@@ -150,14 +160,17 @@
 _STEPPARAMETER = DESCRIPTOR.message_types_by_name['StepParameter']
 _MODEL = DESCRIPTOR.message_types_by_name['Model']
 _CUTOUTPARAMETERS = DESCRIPTOR.message_types_by_name['CutoutParameters']
 _GUIDANCESCHEDULEPARAMETERS = DESCRIPTOR.message_types_by_name['GuidanceScheduleParameters']
 _GUIDANCEINSTANCEPARAMETERS = DESCRIPTOR.message_types_by_name['GuidanceInstanceParameters']
 _GUIDANCEPARAMETERS = DESCRIPTOR.message_types_by_name['GuidanceParameters']
 _TRANSFORMTYPE = DESCRIPTOR.message_types_by_name['TransformType']
+_T2IADAPTERPARAMETER = DESCRIPTOR.message_types_by_name['T2IAdapterParameter']
+_CAIPARAMETERS = DESCRIPTOR.message_types_by_name['CAIParameters']
+_FINETUNINGPARAMETERS = DESCRIPTOR.message_types_by_name['FineTuningParameters']
 _IMAGEPARAMETERS = DESCRIPTOR.message_types_by_name['ImageParameters']
 _CLASSIFIERCONCEPT = DESCRIPTOR.message_types_by_name['ClassifierConcept']
 _CLASSIFIERCATEGORY = DESCRIPTOR.message_types_by_name['ClassifierCategory']
 _CLASSIFIERPARAMETERS = DESCRIPTOR.message_types_by_name['ClassifierParameters']
 _INTERPOLATEPARAMETERS = DESCRIPTOR.message_types_by_name['InterpolateParameters']
 _TRANSFORMCOLORADJUST = DESCRIPTOR.message_types_by_name['TransformColorAdjust']
 _TRANSFORMDEPTHCALC = DESCRIPTOR.message_types_by_name['TransformDepthCalc']
@@ -170,14 +183,15 @@
 _ANSWERMETA = DESCRIPTOR.message_types_by_name['AnswerMeta']
 _ANSWER = DESCRIPTOR.message_types_by_name['Answer']
 _ANSWERBATCH = DESCRIPTOR.message_types_by_name['AnswerBatch']
 _REQUEST = DESCRIPTOR.message_types_by_name['Request']
 _ONSTATUS = DESCRIPTOR.message_types_by_name['OnStatus']
 _STAGE = DESCRIPTOR.message_types_by_name['Stage']
 _CHAINREQUEST = DESCRIPTOR.message_types_by_name['ChainRequest']
+_CAIPARAMETERS_MODELMETADATA = _CAIPARAMETERS.enum_types_by_name['ModelMetadata']
 Token = _reflection.GeneratedProtocolMessageType('Token', (_message.Message,), {
   'DESCRIPTOR' : _TOKEN,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.Token)
   })
 _sym_db.RegisterMessage(Token)
 
@@ -275,14 +289,35 @@
 TransformType = _reflection.GeneratedProtocolMessageType('TransformType', (_message.Message,), {
   'DESCRIPTOR' : _TRANSFORMTYPE,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.TransformType)
   })
 _sym_db.RegisterMessage(TransformType)
 
+T2IAdapterParameter = _reflection.GeneratedProtocolMessageType('T2IAdapterParameter', (_message.Message,), {
+  'DESCRIPTOR' : _T2IADAPTERPARAMETER,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.T2IAdapterParameter)
+  })
+_sym_db.RegisterMessage(T2IAdapterParameter)
+
+CAIParameters = _reflection.GeneratedProtocolMessageType('CAIParameters', (_message.Message,), {
+  'DESCRIPTOR' : _CAIPARAMETERS,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.CAIParameters)
+  })
+_sym_db.RegisterMessage(CAIParameters)
+
+FineTuningParameters = _reflection.GeneratedProtocolMessageType('FineTuningParameters', (_message.Message,), {
+  'DESCRIPTOR' : _FINETUNINGPARAMETERS,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.FineTuningParameters)
+  })
+_sym_db.RegisterMessage(FineTuningParameters)
+
 ImageParameters = _reflection.GeneratedProtocolMessageType('ImageParameters', (_message.Message,), {
   'DESCRIPTOR' : _IMAGEPARAMETERS,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.ImageParameters)
   })
 _sym_db.RegisterMessage(ImageParameters)
 
@@ -422,50 +457,54 @@
 _GENERATIONSERVICE = DESCRIPTOR.services_by_name['GenerationService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/stability-ai/api-interfaces/gooseai/generation'
   _TRANSFORMMATRIX.fields_by_name['data']._options = None
   _TRANSFORMMATRIX.fields_by_name['data']._serialized_options = b'\020\001'
-  _FINISHREASON._serialized_start=6413
-  _FINISHREASON._serialized_end=6482
-  _ARTIFACTTYPE._serialized_start=6485
-  _ARTIFACTTYPE._serialized_end=6733
-  _MASKEDAREAINIT._serialized_start=6735
-  _MASKEDAREAINIT._serialized_end=6838
-  _WEIGHTMETHOD._serialized_start=6840
-  _WEIGHTMETHOD._serialized_end=6893
-  _DIFFUSIONSAMPLER._serialized_start=6896
-  _DIFFUSIONSAMPLER._serialized_end=7176
-  _UPSCALER._serialized_start=7178
-  _UPSCALER._serialized_end=7248
-  _GUIDANCEPRESET._serialized_start=7251
-  _GUIDANCEPRESET._serialized_end=7467
-  _MODELARCHITECTURE._serialized_start=7470
-  _MODELARCHITECTURE._serialized_end=7615
-  _ACTION._serialized_start=7618
-  _ACTION._serialized_end=7780
-  _CLASSIFIERMODE._serialized_start=7782
-  _CLASSIFIERMODE._serialized_end=7850
-  _INTERPOLATEMODE._serialized_start=7853
-  _INTERPOLATEMODE._serialized_end=7993
-  _BORDERMODE._serialized_start=7995
-  _BORDERMODE._serialized_end=8103
-  _COLORMATCHMODE._serialized_start=8105
-  _COLORMATCHMODE._serialized_end=8184
-  _CAMERATYPE._serialized_start=8186
-  _CAMERATYPE._serialized_end=8247
-  _RENDERMODE._serialized_start=8249
-  _RENDERMODE._serialized_end=8301
-  _ASSETACTION._serialized_start=8303
-  _ASSETACTION._serialized_end=8364
-  _ASSETUSE._serialized_start=8367
-  _ASSETUSE._serialized_end=8496
-  _STAGEACTION._serialized_start=8498
-  _STAGEACTION._serialized_end=8585
+  _FINISHREASON._serialized_start=7016
+  _FINISHREASON._serialized_end=7085
+  _ARTIFACTTYPE._serialized_start=7088
+  _ARTIFACTTYPE._serialized_end=7336
+  _MASKEDAREAINIT._serialized_start=7338
+  _MASKEDAREAINIT._serialized_end=7441
+  _WEIGHTMETHOD._serialized_start=7443
+  _WEIGHTMETHOD._serialized_end=7496
+  _DIFFUSIONSAMPLER._serialized_start=7499
+  _DIFFUSIONSAMPLER._serialized_end=7779
+  _UPSCALER._serialized_start=7781
+  _UPSCALER._serialized_end=7851
+  _GUIDANCEPRESET._serialized_start=7854
+  _GUIDANCEPRESET._serialized_end=8070
+  _MODELARCHITECTURE._serialized_start=8073
+  _MODELARCHITECTURE._serialized_end=8218
+  _T2IADAPTER._serialized_start=8220
+  _T2IADAPTER._serialized_end=8320
+  _T2IADAPTERINIT._serialized_start=8322
+  _T2IADAPTERINIT._serialized_end=8398
+  _ACTION._serialized_start=8401
+  _ACTION._serialized_end=8563
+  _CLASSIFIERMODE._serialized_start=8565
+  _CLASSIFIERMODE._serialized_end=8633
+  _INTERPOLATEMODE._serialized_start=8636
+  _INTERPOLATEMODE._serialized_end=8776
+  _BORDERMODE._serialized_start=8778
+  _BORDERMODE._serialized_end=8886
+  _COLORMATCHMODE._serialized_start=8888
+  _COLORMATCHMODE._serialized_end=8967
+  _CAMERATYPE._serialized_start=8969
+  _CAMERATYPE._serialized_end=9030
+  _RENDERMODE._serialized_start=9032
+  _RENDERMODE._serialized_end=9084
+  _ASSETACTION._serialized_start=9086
+  _ASSETACTION._serialized_end=9147
+  _ASSETUSE._serialized_start=9150
+  _ASSETUSE._serialized_end=9279
+  _STAGEACTION._serialized_start=9281
+  _STAGEACTION._serialized_end=9368
   _TOKEN._serialized_start=74
   _TOKEN._serialized_end=121
   _TOKENS._serialized_start=123
   _TOKENS._serialized_end=207
   _ARTIFACT._serialized_start=210
   _ARTIFACT._serialized_end=581
   _PROMPTPARAMETERS._serialized_start=583
@@ -488,50 +527,58 @@
   _GUIDANCESCHEDULEPARAMETERS._serialized_end=2074
   _GUIDANCEINSTANCEPARAMETERS._serialized_start=2077
   _GUIDANCEINSTANCEPARAMETERS._serialized_end=2356
   _GUIDANCEPARAMETERS._serialized_start=2358
   _GUIDANCEPARAMETERS._serialized_end=2484
   _TRANSFORMTYPE._serialized_start=2486
   _TRANSFORMTYPE._serialized_end=2596
-  _IMAGEPARAMETERS._serialized_start=2599
-  _IMAGEPARAMETERS._serialized_end=3044
-  _CLASSIFIERCONCEPT._serialized_start=3046
-  _CLASSIFIERCONCEPT._serialized_end=3120
-  _CLASSIFIERCATEGORY._serialized_start=3123
-  _CLASSIFIERCATEGORY._serialized_end=3367
-  _CLASSIFIERPARAMETERS._serialized_start=3370
-  _CLASSIFIERPARAMETERS._serialized_end=3554
-  _INTERPOLATEPARAMETERS._serialized_start=3556
-  _INTERPOLATEPARAMETERS._serialized_end=3649
-  _TRANSFORMCOLORADJUST._serialized_start=3652
-  _TRANSFORMCOLORADJUST._serialized_end=4064
-  _TRANSFORMDEPTHCALC._serialized_start=4067
-  _TRANSFORMDEPTHCALC._serialized_end=4207
-  _TRANSFORMMATRIX._serialized_start=4209
-  _TRANSFORMMATRIX._serialized_end=4244
-  _TRANSFORMRESAMPLE._serialized_start=4247
-  _TRANSFORMRESAMPLE._serialized_end=4509
-  _CAMERAPARAMETERS._serialized_start=4511
-  _CAMERAPARAMETERS._serialized_end=4636
-  _TRANSFORMCAMERAPOSE._serialized_start=4639
-  _TRANSFORMCAMERAPOSE._serialized_end=4856
-  _TRANSFORMPARAMETERS._serialized_start=4859
-  _TRANSFORMPARAMETERS._serialized_end=5100
-  _ASSETPARAMETERS._serialized_start=5102
-  _ASSETPARAMETERS._serialized_end=5209
-  _ANSWERMETA._serialized_start=5212
-  _ANSWERMETA._serialized_end=5360
-  _ANSWER._serialized_start=5363
-  _ANSWER._serialized_end=5532
-  _ANSWERBATCH._serialized_start=5534
-  _ANSWERBATCH._serialized_end=5599
-  _REQUEST._serialized_start=5602
-  _REQUEST._serialized_end=6129
-  _ONSTATUS._serialized_start=6131
-  _ONSTATUS._serialized_end=6250
-  _STAGE._serialized_start=6252
-  _STAGE._serialized_end=6344
-  _CHAINREQUEST._serialized_start=6346
-  _CHAINREQUEST._serialized_end=6411
-  _GENERATIONSERVICE._serialized_start=8588
-  _GENERATIONSERVICE._serialized_end=8719
+  _T2IADAPTERPARAMETER._serialized_start=2599
+  _T2IADAPTERPARAMETER._serialized_end=2741
+  _CAIPARAMETERS._serialized_start=2744
+  _CAIPARAMETERS._serialized_end=2926
+  _CAIPARAMETERS_MODELMETADATA._serialized_start=2825
+  _CAIPARAMETERS_MODELMETADATA._serialized_end=2912
+  _FINETUNINGPARAMETERS._serialized_start=2928
+  _FINETUNINGPARAMETERS._serialized_end=3000
+  _IMAGEPARAMETERS._serialized_start=3003
+  _IMAGEPARAMETERS._serialized_end=3647
+  _CLASSIFIERCONCEPT._serialized_start=3649
+  _CLASSIFIERCONCEPT._serialized_end=3723
+  _CLASSIFIERCATEGORY._serialized_start=3726
+  _CLASSIFIERCATEGORY._serialized_end=3970
+  _CLASSIFIERPARAMETERS._serialized_start=3973
+  _CLASSIFIERPARAMETERS._serialized_end=4157
+  _INTERPOLATEPARAMETERS._serialized_start=4159
+  _INTERPOLATEPARAMETERS._serialized_end=4252
+  _TRANSFORMCOLORADJUST._serialized_start=4255
+  _TRANSFORMCOLORADJUST._serialized_end=4667
+  _TRANSFORMDEPTHCALC._serialized_start=4670
+  _TRANSFORMDEPTHCALC._serialized_end=4810
+  _TRANSFORMMATRIX._serialized_start=4812
+  _TRANSFORMMATRIX._serialized_end=4847
+  _TRANSFORMRESAMPLE._serialized_start=4850
+  _TRANSFORMRESAMPLE._serialized_end=5112
+  _CAMERAPARAMETERS._serialized_start=5114
+  _CAMERAPARAMETERS._serialized_end=5239
+  _TRANSFORMCAMERAPOSE._serialized_start=5242
+  _TRANSFORMCAMERAPOSE._serialized_end=5459
+  _TRANSFORMPARAMETERS._serialized_start=5462
+  _TRANSFORMPARAMETERS._serialized_end=5703
+  _ASSETPARAMETERS._serialized_start=5705
+  _ASSETPARAMETERS._serialized_end=5812
+  _ANSWERMETA._serialized_start=5815
+  _ANSWERMETA._serialized_end=5963
+  _ANSWER._serialized_start=5966
+  _ANSWER._serialized_end=6135
+  _ANSWERBATCH._serialized_start=6137
+  _ANSWERBATCH._serialized_end=6202
+  _REQUEST._serialized_start=6205
+  _REQUEST._serialized_end=6732
+  _ONSTATUS._serialized_start=6734
+  _ONSTATUS._serialized_end=6853
+  _STAGE._serialized_start=6855
+  _STAGE._serialized_end=6947
+  _CHAINREQUEST._serialized_start=6949
+  _CHAINREQUEST._serialized_end=7014
+  _GENERATIONSERVICE._serialized_start=9371
+  _GENERATIONSERVICE._serialized_end=9502
 # @@protoc_insertion_point(module_scope)
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/project/project_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,41 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import generation_pb2 as generation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rproject.proto\x12\x07gooseai\x1a\x10generation.proto\"\x91\x02\n\x0cProjectAsset\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12%\n\x03use\x18\x03 \x01(\x0e\x32\x18.gooseai.ProjectAssetUse\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x04\x12\x12\n\ncreated_at\x18\x06 \x01(\x04\x12\x12\n\nupdated_at\x18\x07 \x01(\x04\x12!\n\x07request\x18\x08 \x01(\x0b\x32\x10.gooseai.Request\x12-\n\x04tags\x18\t \x03(\x0b\x32\x1f.gooseai.ProjectAsset.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x02\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x10\n\x08owner_id\x18\x03 \x01(\t\x12&\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectAccess\x12&\n\x06status\x18\x05 \x01(\x0e\x32\x16.gooseai.ProjectStatus\x12\x0c\n\x04size\x18\x06 \x01(\x04\x12#\n\x04\x66ile\x18\x07 \x01(\x0b\x32\x15.gooseai.ProjectAsset\x12\x12\n\ncreated_at\x18\x08 \x01(\x04\x12\x12\n\nupdated_at\x18\t \x01(\x04\x12%\n\x06\x61ssets\x18\n \x03(\x0b\x32\x15.gooseai.ProjectAsset\"\xcc\x01\n\x14\x43reateProjectRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12&\n\x06\x61\x63\x63\x65ss\x18\x03 \x01(\x0e\x32\x16.gooseai.ProjectAccess\x12&\n\x06status\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectStatus\x12(\n\x04\x66ile\x18\x05 \x01(\x0b\x32\x15.gooseai.ProjectAssetH\x01\x88\x01\x01\x42\x0b\n\t_owner_idB\x07\n\x05_file\"\x87\x02\n\x14UpdateProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12+\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectAccessH\x02\x88\x01\x01\x12+\n\x06status\x18\x05 \x01(\x0e\x32\x16.gooseai.ProjectStatusH\x03\x88\x01\x01\x12(\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x15.gooseai.ProjectAssetH\x04\x88\x01\x01\x42\x0b\n\t_owner_idB\x08\n\x06_titleB\t\n\x07_accessB\t\n\x07_statusB\x07\n\x05_file\"8\n\x12ListProjectRequest\x12\x15\n\x08owner_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"C\n\x11GetProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"F\n\x14\x44\x65leteProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"\xf8\x02\n\x12QueryAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05since\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05until\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05limit\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tstart_key\x18\x06 \x01(\tH\x04\x88\x01\x01\x12%\n\x03use\x18\x07 \x03(\x0e\x32\x18.gooseai.ProjectAssetUse\x12)\n\x08sort_dir\x18\x08 \x01(\x0e\x32\x17.gooseai.ProjectSortDir\x12\x33\n\x04tags\x18\t \x03(\x0b\x32%.gooseai.QueryAssetsRequest.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0b\n\t_owner_idB\x08\n\x06_sinceB\x08\n\x06_untilB\x08\n\x06_limitB\x0c\n\n_start_key\"`\n\x13QueryAssetsResponse\x12%\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x15.gooseai.ProjectAsset\x12\x15\n\x08last_key\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_last_key\"\xb5\x01\n\x10TagAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\t\x12\x31\n\x04tags\x18\x04 \x03(\x0b\x32#.gooseai.TagAssetsRequest.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0b\n\t_owner_id\"D\n\x11TagAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t\"i\n\x12UntagAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\t\x12\x10\n\x08tag_keys\x18\x04 \x03(\tB\x0b\n\t_owner_id\"F\n\x13UntagAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t\"X\n\x13\x44\x65leteAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\tB\x0b\n\t_owner_id\"G\n\x14\x44\x65leteAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t*F\n\rProjectAccess\x12\x1a\n\x16PROJECT_ACCESS_PRIVATE\x10\x00\x12\x19\n\x15PROJECT_ACCESS_PUBLIC\x10\x01*c\n\rProjectStatus\x12\x1b\n\x17PROJECT_STATUS_INACTIVE\x10\x00\x12\x19\n\x15PROJECT_STATUS_ACTIVE\x10\x01\x12\x1a\n\x16PROJECT_STATUS_DELETED\x10\x02*\xb0\x01\n\x0fProjectAssetUse\x12\x1f\n\x1bPROJECT_ASSET_USE_UNDEFINED\x10\x00\x12\x1b\n\x17PROJECT_ASSET_USE_INPUT\x10\x01\x12\x1c\n\x18PROJECT_ASSET_USE_OUTPUT\x10\x02\x12\"\n\x1ePROJECT_ASSET_USE_INTERMEDIATE\x10\x03\x12\x1d\n\x19PROJECT_ASSET_USE_PROJECT\x10\x04*g\n\x0eProjectSortDir\x12 \n\x1cPROJECT_SORT_DIR_UNSPECIFIED\x10\x00\x12\x18\n\x14PROJECT_SORT_DIR_ASC\x10\x01\x12\x19\n\x15PROJECT_SORT_DIR_DESC\x10\x02\x32\xe6\x04\n\x0eProjectService\x12;\n\x06\x43reate\x12\x1d.gooseai.CreateProjectRequest\x1a\x10.gooseai.Project\"\x00\x12;\n\x06Update\x12\x1d.gooseai.UpdateProjectRequest\x1a\x10.gooseai.Project\"\x00\x12\x39\n\x04List\x12\x1b.gooseai.ListProjectRequest\x1a\x10.gooseai.Project\"\x00\x30\x01\x12\x35\n\x03Get\x12\x1a.gooseai.GetProjectRequest\x1a\x10.gooseai.Project\"\x00\x12;\n\x06\x44\x65lete\x12\x1d.gooseai.DeleteProjectRequest\x1a\x10.gooseai.Project\"\x00\x12\x44\n\tTagAssets\x12\x19.gooseai.TagAssetsRequest\x1a\x1a.gooseai.TagAssetsResponse\"\x00\x12J\n\x0bUntagAssets\x12\x1b.gooseai.UntagAssetsRequest\x1a\x1c.gooseai.UntagAssetsResponse\"\x00\x12J\n\x0bQueryAssets\x12\x1b.gooseai.QueryAssetsRequest\x1a\x1c.gooseai.QueryAssetsResponse\"\x00\x12M\n\x0c\x44\x65leteAssets\x12\x1c.gooseai.DeleteAssetsRequest\x1a\x1d.gooseai.DeleteAssetsResponse\"\x00\x42\x38Z6github.com/stability-ai/api-interfaces/gooseai/projectb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rproject.proto\x12\x07gooseai\x1a\x10generation.proto\"\x91\x02\n\x0cProjectAsset\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12%\n\x03use\x18\x03 \x01(\x0e\x32\x18.gooseai.ProjectAssetUse\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x04\x12\x12\n\ncreated_at\x18\x06 \x01(\x04\x12\x12\n\nupdated_at\x18\x07 \x01(\x04\x12!\n\x07request\x18\x08 \x01(\x0b\x32\x10.gooseai.Request\x12-\n\x04tags\x18\t \x03(\x0b\x32\x1f.gooseai.ProjectAsset.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xac\x02\n\x07Project\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x10\n\x08owner_id\x18\x03 \x01(\t\x12&\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectAccess\x12&\n\x06status\x18\x05 \x01(\x0e\x32\x16.gooseai.ProjectStatus\x12\x0c\n\x04size\x18\x06 \x01(\x04\x12#\n\x04\x66ile\x18\x07 \x01(\x0b\x32\x15.gooseai.ProjectAsset\x12\x12\n\ncreated_at\x18\x08 \x01(\x04\x12\x12\n\nupdated_at\x18\t \x01(\x04\x12%\n\x06\x61ssets\x18\n \x03(\x0b\x32\x15.gooseai.ProjectAsset\x12\"\n\x04type\x18\x0b \x01(\x0e\x32\x14.gooseai.ProjectType\"\xf0\x01\n\x14\x43reateProjectRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12&\n\x06\x61\x63\x63\x65ss\x18\x03 \x01(\x0e\x32\x16.gooseai.ProjectAccess\x12&\n\x06status\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectStatus\x12(\n\x04\x66ile\x18\x05 \x01(\x0b\x32\x15.gooseai.ProjectAssetH\x01\x88\x01\x01\x12\"\n\x04type\x18\x06 \x01(\x0e\x32\x14.gooseai.ProjectTypeB\x0b\n\t_owner_idB\x07\n\x05_file\"\xb9\x02\n\x14UpdateProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05title\x18\x03 \x01(\tH\x01\x88\x01\x01\x12+\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0e\x32\x16.gooseai.ProjectAccessH\x02\x88\x01\x01\x12+\n\x06status\x18\x05 \x01(\x0e\x32\x16.gooseai.ProjectStatusH\x03\x88\x01\x01\x12(\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x15.gooseai.ProjectAssetH\x04\x88\x01\x01\x12\'\n\x04type\x18\x07 \x01(\x0e\x32\x14.gooseai.ProjectTypeH\x05\x88\x01\x01\x42\x0b\n\t_owner_idB\x08\n\x06_titleB\t\n\x07_accessB\t\n\x07_statusB\x07\n\x05_fileB\x07\n\x05_type\"8\n\x12ListProjectRequest\x12\x15\n\x08owner_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"C\n\x11GetProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"F\n\x14\x44\x65leteProjectRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_owner_id\"\xf8\x02\n\x12QueryAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\x05since\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05until\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05limit\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tstart_key\x18\x06 \x01(\tH\x04\x88\x01\x01\x12%\n\x03use\x18\x07 \x03(\x0e\x32\x18.gooseai.ProjectAssetUse\x12)\n\x08sort_dir\x18\x08 \x01(\x0e\x32\x17.gooseai.ProjectSortDir\x12\x33\n\x04tags\x18\t \x03(\x0b\x32%.gooseai.QueryAssetsRequest.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0b\n\t_owner_idB\x08\n\x06_sinceB\x08\n\x06_untilB\x08\n\x06_limitB\x0c\n\n_start_key\"`\n\x13QueryAssetsResponse\x12%\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x15.gooseai.ProjectAsset\x12\x15\n\x08last_key\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0b\n\t_last_key\"\xb5\x01\n\x10TagAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\t\x12\x31\n\x04tags\x18\x04 \x03(\x0b\x32#.gooseai.TagAssetsRequest.TagsEntry\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0b\n\t_owner_id\"D\n\x11TagAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t\"i\n\x12UntagAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\t\x12\x10\n\x08tag_keys\x18\x04 \x03(\tB\x0b\n\t_owner_id\"F\n\x13UntagAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t\"X\n\x13\x44\x65leteAssetsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x08owner_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x11\n\tasset_ids\x18\x03 \x03(\tB\x0b\n\t_owner_id\"G\n\x14\x44\x65leteAssetsResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08owner_id\x18\x02 \x01(\t\x12\x11\n\tasset_ids\x18\x03 \x03(\t*F\n\rProjectAccess\x12\x1a\n\x16PROJECT_ACCESS_PRIVATE\x10\x00\x12\x19\n\x15PROJECT_ACCESS_PUBLIC\x10\x01*c\n\rProjectStatus\x12\x1b\n\x17PROJECT_STATUS_INACTIVE\x10\x00\x12\x19\n\x15PROJECT_STATUS_ACTIVE\x10\x01\x12\x1a\n\x16PROJECT_STATUS_DELETED\x10\x02*\xb0\x01\n\x0fProjectAssetUse\x12\x1f\n\x1bPROJECT_ASSET_USE_UNDEFINED\x10\x00\x12\x1b\n\x17PROJECT_ASSET_USE_INPUT\x10\x01\x12\x1c\n\x18PROJECT_ASSET_USE_OUTPUT\x10\x02\x12\"\n\x1ePROJECT_ASSET_USE_INTERMEDIATE\x10\x03\x12\x1d\n\x19PROJECT_ASSET_USE_PROJECT\x10\x04*g\n\x0eProjectSortDir\x12 \n\x1cPROJECT_SORT_DIR_UNSPECIFIED\x10\x00\x12\x18\n\x14PROJECT_SORT_DIR_ASC\x10\x01\x12\x19\n\x15PROJECT_SORT_DIR_DESC\x10\x02*F\n\x0bProjectType\x12\x1c\n\x18PROJECT_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15PROJECT_TYPE_TRAINING\x10\x01\x32\xe6\x04\n\x0eProjectService\x12;\n\x06\x43reate\x12\x1d.gooseai.CreateProjectRequest\x1a\x10.gooseai.Project\"\x00\x12;\n\x06Update\x12\x1d.gooseai.UpdateProjectRequest\x1a\x10.gooseai.Project\"\x00\x12\x39\n\x04List\x12\x1b.gooseai.ListProjectRequest\x1a\x10.gooseai.Project\"\x00\x30\x01\x12\x35\n\x03Get\x12\x1a.gooseai.GetProjectRequest\x1a\x10.gooseai.Project\"\x00\x12;\n\x06\x44\x65lete\x12\x1d.gooseai.DeleteProjectRequest\x1a\x10.gooseai.Project\"\x00\x12\x44\n\tTagAssets\x12\x19.gooseai.TagAssetsRequest\x1a\x1a.gooseai.TagAssetsResponse\"\x00\x12J\n\x0bUntagAssets\x12\x1b.gooseai.UntagAssetsRequest\x1a\x1c.gooseai.UntagAssetsResponse\"\x00\x12J\n\x0bQueryAssets\x12\x1b.gooseai.QueryAssetsRequest\x1a\x1c.gooseai.QueryAssetsResponse\"\x00\x12M\n\x0c\x44\x65leteAssets\x12\x1c.gooseai.DeleteAssetsRequest\x1a\x1d.gooseai.DeleteAssetsResponse\"\x00\x42\x38Z6github.com/stability-ai/api-interfaces/gooseai/projectb\x06proto3')
 
 _PROJECTACCESS = DESCRIPTOR.enum_types_by_name['ProjectAccess']
 ProjectAccess = enum_type_wrapper.EnumTypeWrapper(_PROJECTACCESS)
 _PROJECTSTATUS = DESCRIPTOR.enum_types_by_name['ProjectStatus']
 ProjectStatus = enum_type_wrapper.EnumTypeWrapper(_PROJECTSTATUS)
 _PROJECTASSETUSE = DESCRIPTOR.enum_types_by_name['ProjectAssetUse']
 ProjectAssetUse = enum_type_wrapper.EnumTypeWrapper(_PROJECTASSETUSE)
 _PROJECTSORTDIR = DESCRIPTOR.enum_types_by_name['ProjectSortDir']
 ProjectSortDir = enum_type_wrapper.EnumTypeWrapper(_PROJECTSORTDIR)
+_PROJECTTYPE = DESCRIPTOR.enum_types_by_name['ProjectType']
+ProjectType = enum_type_wrapper.EnumTypeWrapper(_PROJECTTYPE)
 PROJECT_ACCESS_PRIVATE = 0
 PROJECT_ACCESS_PUBLIC = 1
 PROJECT_STATUS_INACTIVE = 0
 PROJECT_STATUS_ACTIVE = 1
 PROJECT_STATUS_DELETED = 2
 PROJECT_ASSET_USE_UNDEFINED = 0
 PROJECT_ASSET_USE_INPUT = 1
 PROJECT_ASSET_USE_OUTPUT = 2
 PROJECT_ASSET_USE_INTERMEDIATE = 3
 PROJECT_ASSET_USE_PROJECT = 4
 PROJECT_SORT_DIR_UNSPECIFIED = 0
 PROJECT_SORT_DIR_ASC = 1
 PROJECT_SORT_DIR_DESC = 2
+PROJECT_TYPE_UNSPECIFIED = 0
+PROJECT_TYPE_TRAINING = 1
 
 
 _PROJECTASSET = DESCRIPTOR.message_types_by_name['ProjectAsset']
 _PROJECTASSET_TAGSENTRY = _PROJECTASSET.nested_types_by_name['TagsEntry']
 _PROJECT = DESCRIPTOR.message_types_by_name['Project']
 _CREATEPROJECTREQUEST = DESCRIPTOR.message_types_by_name['CreateProjectRequest']
 _UPDATEPROJECTREQUEST = DESCRIPTOR.message_types_by_name['UpdateProjectRequest']
@@ -195,54 +199,56 @@
   DESCRIPTOR._serialized_options = b'Z6github.com/stability-ai/api-interfaces/gooseai/project'
   _PROJECTASSET_TAGSENTRY._options = None
   _PROJECTASSET_TAGSENTRY._serialized_options = b'8\001'
   _QUERYASSETSREQUEST_TAGSENTRY._options = None
   _QUERYASSETSREQUEST_TAGSENTRY._serialized_options = b'8\001'
   _TAGASSETSREQUEST_TAGSENTRY._options = None
   _TAGASSETSREQUEST_TAGSENTRY._serialized_options = b'8\001'
-  _PROJECTACCESS._serialized_start=2332
-  _PROJECTACCESS._serialized_end=2402
-  _PROJECTSTATUS._serialized_start=2404
-  _PROJECTSTATUS._serialized_end=2503
-  _PROJECTASSETUSE._serialized_start=2506
-  _PROJECTASSETUSE._serialized_end=2682
-  _PROJECTSORTDIR._serialized_start=2684
-  _PROJECTSORTDIR._serialized_end=2787
+  _PROJECTACCESS._serialized_start=2454
+  _PROJECTACCESS._serialized_end=2524
+  _PROJECTSTATUS._serialized_start=2526
+  _PROJECTSTATUS._serialized_end=2625
+  _PROJECTASSETUSE._serialized_start=2628
+  _PROJECTASSETUSE._serialized_end=2804
+  _PROJECTSORTDIR._serialized_start=2806
+  _PROJECTSORTDIR._serialized_end=2909
+  _PROJECTTYPE._serialized_start=2911
+  _PROJECTTYPE._serialized_end=2981
   _PROJECTASSET._serialized_start=45
   _PROJECTASSET._serialized_end=318
   _PROJECTASSET_TAGSENTRY._serialized_start=275
   _PROJECTASSET_TAGSENTRY._serialized_end=318
   _PROJECT._serialized_start=321
-  _PROJECT._serialized_end=585
-  _CREATEPROJECTREQUEST._serialized_start=588
-  _CREATEPROJECTREQUEST._serialized_end=792
-  _UPDATEPROJECTREQUEST._serialized_start=795
-  _UPDATEPROJECTREQUEST._serialized_end=1058
-  _LISTPROJECTREQUEST._serialized_start=1060
-  _LISTPROJECTREQUEST._serialized_end=1116
-  _GETPROJECTREQUEST._serialized_start=1118
-  _GETPROJECTREQUEST._serialized_end=1185
-  _DELETEPROJECTREQUEST._serialized_start=1187
-  _DELETEPROJECTREQUEST._serialized_end=1257
-  _QUERYASSETSREQUEST._serialized_start=1260
-  _QUERYASSETSREQUEST._serialized_end=1636
+  _PROJECT._serialized_end=621
+  _CREATEPROJECTREQUEST._serialized_start=624
+  _CREATEPROJECTREQUEST._serialized_end=864
+  _UPDATEPROJECTREQUEST._serialized_start=867
+  _UPDATEPROJECTREQUEST._serialized_end=1180
+  _LISTPROJECTREQUEST._serialized_start=1182
+  _LISTPROJECTREQUEST._serialized_end=1238
+  _GETPROJECTREQUEST._serialized_start=1240
+  _GETPROJECTREQUEST._serialized_end=1307
+  _DELETEPROJECTREQUEST._serialized_start=1309
+  _DELETEPROJECTREQUEST._serialized_end=1379
+  _QUERYASSETSREQUEST._serialized_start=1382
+  _QUERYASSETSREQUEST._serialized_end=1758
   _QUERYASSETSREQUEST_TAGSENTRY._serialized_start=275
   _QUERYASSETSREQUEST_TAGSENTRY._serialized_end=318
-  _QUERYASSETSRESPONSE._serialized_start=1638
-  _QUERYASSETSRESPONSE._serialized_end=1734
-  _TAGASSETSREQUEST._serialized_start=1737
-  _TAGASSETSREQUEST._serialized_end=1918
+  _QUERYASSETSRESPONSE._serialized_start=1760
+  _QUERYASSETSRESPONSE._serialized_end=1856
+  _TAGASSETSREQUEST._serialized_start=1859
+  _TAGASSETSREQUEST._serialized_end=2040
   _TAGASSETSREQUEST_TAGSENTRY._serialized_start=275
   _TAGASSETSREQUEST_TAGSENTRY._serialized_end=318
-  _TAGASSETSRESPONSE._serialized_start=1920
-  _TAGASSETSRESPONSE._serialized_end=1988
-  _UNTAGASSETSREQUEST._serialized_start=1990
-  _UNTAGASSETSREQUEST._serialized_end=2095
-  _UNTAGASSETSRESPONSE._serialized_start=2097
-  _UNTAGASSETSRESPONSE._serialized_end=2167
-  _DELETEASSETSREQUEST._serialized_start=2169
-  _DELETEASSETSREQUEST._serialized_end=2257
-  _DELETEASSETSRESPONSE._serialized_start=2259
-  _DELETEASSETSRESPONSE._serialized_end=2330
-  _PROJECTSERVICE._serialized_start=2790
-  _PROJECTSERVICE._serialized_end=3404
+  _TAGASSETSRESPONSE._serialized_start=2042
+  _TAGASSETSRESPONSE._serialized_end=2110
+  _UNTAGASSETSREQUEST._serialized_start=2112
+  _UNTAGASSETSREQUEST._serialized_end=2217
+  _UNTAGASSETSRESPONSE._serialized_start=2219
+  _UNTAGASSETSRESPONSE._serialized_end=2289
+  _DELETEASSETSREQUEST._serialized_start=2291
+  _DELETEASSETSREQUEST._serialized_end=2379
+  _DELETEASSETSRESPONSE._serialized_start=2381
+  _DELETEASSETSRESPONSE._serialized_end=2452
+  _PROJECTSERVICE._serialized_start=2984
+  _PROJECTSERVICE._serialized_end=3598
 # @@protoc_insertion_point(module_scope)
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/protobuf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from collections import OrderedDict
+from typing import BinaryIO
+from typing import OrderedDict as OrderedDictType
+from typing import Tuple, Union
+
+import numpy as np
 import torch
 from torch import Tensor
-import numpy as np
-import tensors.tensors_pb2 as tensors_pb
-from tensors.tensors_pb2 import Tensor as TensorPb
-from typing import OrderedDict, Tuple, Union, BinaryIO
+
+import tensorizer.tensors_pb2 as tensors_pb
+from tensorizer.tensors_pb2 import Tensor as TensorPb
 
 DtypePbs = {
     torch.float32: tensors_pb.DT_FLOAT32,
     torch.float64: tensors_pb.DT_FLOAT64,
     torch.float16: tensors_pb.DT_FLOAT16,
     torch.bfloat16: tensors_pb.DT_BFLOAT16,
     torch.complex32: tensors_pb.DT_COMPLEX32,
@@ -62,90 +67,93 @@
     tensors_pb.DT_QUINT8: np.uint8,
     tensors_pb.DT_QINT8: np.int8,
     tensors_pb.DT_QINT32: np.int32,
     tensors_pb.DT_QUINT4_2: np.uint8,
 }
 
 
-def serialize_tensor(t: Tensor, attribute: tensors_pb.AttributeType = None) -> \
-        tensors_pb.Tensor:
+def serialize_tensor(
+    t: Tensor, attribute: tensors_pb.AttributeType = None
+) -> tensors_pb.Tensor:
     assert isinstance(t, Tensor)
-    assert attribute is None or attribute in [tensors_pb.AT_PARAMETER,
-                                              tensors_pb.AT_BUFFER]
+    assert attribute is None or attribute in [
+        tensors_pb.AT_PARAMETER,
+        tensors_pb.AT_BUFFER,
+    ]
 
     extra_opts = {}
     if attribute is not None:
-        extra_opts = {'attr_type': attribute}
+        extra_opts = {"attr_type": attribute}
 
     return tensors_pb.Tensor(
         dtype=DtypePbs[t.dtype],
         shape=t.shape,
         data=t.cpu().detach().numpy().tobytes(),
-        **extra_opts
+        **extra_opts,
     )
 
 
-def deserialize_tensor(t: tensors_pb.Tensor) -> \
-        Union[Tensor, Tuple[Tensor, 'tensors_pb.AttributeType']]:
+def deserialize_tensor(
+    t: tensors_pb.Tensor,
+) -> Union[Tensor, Tuple[Tensor, "tensors_pb.AttributeType"]]:
     mv = bytearray(t.data)
-    tensor = torch.as_tensor(np.ndarray.__new__(np.memmap,
-                                                t.shape,
-                                                dtype=PbNpyDtypes[t.dtype],
-                                                buffer=mv,
-                                                offset=0))
+    tensor = torch.as_tensor(
+        np.ndarray.__new__(
+            np.memmap, t.shape, dtype=PbNpyDtypes[t.dtype], buffer=mv, offset=0
+        )
+    )
     if t.HasField("attr_type"):
         return tensor, t.attr_type
     else:
         return tensor
 
 
 def serialize_model(model: torch.nn.Module, file_stream: BinaryIO) -> None:
     modules = list()
     for module_name, module in model.named_modules():
         print(module_name)
         attributes = list()
         for name, param in module.named_parameters(recurse=False):
             v = param.cpu().detach()
             param_attr = tensors_pb.Attribute(
-                name=name,
-                tensor=serialize_tensor(v, tensors_pb.AT_PARAMETER)
+                name=name, tensor=serialize_tensor(v, tensors_pb.AT_PARAMETER)
             )
             attributes.append(param_attr)
         for name, buffer in module.named_buffers(recurse=False):
             v = buffer.cpu().detach()
             buffer_attr = tensors_pb.Attribute(
-                name=name,
-                tensor=serialize_tensor(v, tensors_pb.AT_BUFFER)
+                name=name, tensor=serialize_tensor(v, tensors_pb.AT_BUFFER)
             )
             attributes.append(buffer_attr)
         module_attr = tensors_pb.Attribute(
-            name=module_name,
-            module=tensors_pb.Module(
-                attributes=attributes
-            )
+            name=module_name, module=tensors_pb.Module(attributes=attributes)
         )
         modules.append(module_attr)
     model_proto = tensors_pb.Module(  # models are just modules as attributes
         name="",
         attributes=modules,
     )
     file_stream.write(model_proto.SerializeToString())
 
 
 def deserialize_model(model: torch.nn.Module, file_stream: BinaryIO) -> None:
     model_proto = tensors_pb.Module()
     model_proto.ParseFromString(file_stream.read())
 
-    modules: OrderedDict[str, torch.nn.Module] = OrderedDict()
+    modules: OrderedDictType[str, torch.nn.Module] = OrderedDict()
     for name, module in model.named_modules():
         modules[name] = module
 
     for module_attr in model_proto.attributes:
         module = modules[module_attr.name]
         for attr in module_attr.module.attributes:
             if attr.tensor.HasField("attr_type"):
                 if attr.tensor.attr_type == tensors_pb.AT_PARAMETER:
-                    module._parameters[attr.name] = deserialize_tensor(attr.tensor)[0]
+                    module._parameters[attr.name] = deserialize_tensor(
+                        attr.tensor
+                    )[0]
                 elif attr.tensor.attr_type == tensors_pb.AT_BUFFER:
-                    module._buffers[attr.name] = deserialize_tensor(attr.tensor)[0]
+                    module._buffers[attr.name] = deserialize_tensor(
+                        attr.tensor
+                    )[0]
                 else:
                     raise ValueError("Unknown attribute type")
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/tensorizer/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.8.4/src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_tensorizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
-import tensorizer
+from tensorizer import tensorizer
+
 import unittest
 import torch
 
 class TestTensorizer(unittest.TestCase):
     def test_tensorizer_gptj(self):
         from transformers import GPTJConfig, GPTJForCausalLM
         # instantiate dummy model config
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk/matrix.py` & `stability-sdk-0.8.4/src/stability_sdk/matrix.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk/utils.py` & `stability-sdk-0.8.4/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.8.4/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.8.3/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.8.4/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,24 +17,36 @@
 src/stability_sdk.egg-info/top_level.txt
 src/stability_sdk/interfaces/__init__.py
 src/stability_sdk/interfaces/gooseai/__init__.py
 src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
 src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
 src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
 src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+src/stability_sdk/interfaces/gooseai/finetuning/finetuning_pb2.py
+src/stability_sdk/interfaces/gooseai/finetuning/finetuning_pb2_grpc.py
 src/stability_sdk/interfaces/gooseai/generation/__init__.py
 src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
 src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
 src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
 src/stability_sdk/interfaces/gooseai/project/project_pb2.py
 src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-src/stability_sdk/interfaces/src/tensorizer/__init__.py
-src/stability_sdk/interfaces/src/tensorizer/protobuf.py
-src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
-src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_protobuf.py
+src/stability_sdk/interfaces/src/tensorizer/ATTIC/test_tensorizer.py
+src/stability_sdk/interfaces/src/tensorizer/examples/__init__.py
+src/stability_sdk/interfaces/src/tensorizer/examples/deserialize.py
+src/stability_sdk/interfaces/src/tensorizer/examples/hf_serialization.py
+src/stability_sdk/interfaces/src/tensorizer/examples/serialize.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/__init__.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/_wide_pipes.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/protobuf.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/serialization.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/stream_io.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/tensors_pb2.py
+src/stability_sdk/interfaces/src/tensorizer/tensorizer/utils.py
 src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
 src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+src/stability_sdk/interfaces/src/tensorizer/tests/test_serialization.py
+src/stability_sdk/interfaces/src/tensorizer/tests/test_stream_io.py
 tests/test_animator.py
 tests/test_api.py
 tests/test_client.py
 tests/test_utils.py
```

### Comparing `stability-sdk-0.8.3/tests/test_animator.py` & `stability-sdk-0.8.4/tests/test_animator.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/tests/test_api.py` & `stability-sdk-0.8.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/tests/test_client.py` & `stability-sdk-0.8.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.3/tests/test_utils.py` & `stability-sdk-0.8.4/tests/test_utils.py`

 * *Files identical despite different names*

