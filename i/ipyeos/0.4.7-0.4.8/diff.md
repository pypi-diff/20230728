# Comparing `tmp/ipyeos-0.4.7.tar.gz` & `tmp/ipyeos-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyeos-0.4.7.tar", last modified: Fri Jul 28 04:47:32 2023, max compression
+gzip compressed data, was "ipyeos-0.4.8.tar", last modified: Fri Jul 28 07:50:44 2023, max compression
```

## Comparing `ipyeos-0.4.7.tar` & `ipyeos-0.4.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.289138 ipyeos-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-28 04:47:20.000000 ipyeos-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-28 04:47:20.000000 ipyeos-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-28 04:47:32.289138 ipyeos-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-07-28 04:47:20.000000 ipyeos-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.265138 ipyeos-0.4.7/ipyeos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-28 04:47:32.000000 ipyeos-0.4.7/ipyeos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.273138 ipyeos-0.4.7/pysrc/
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/args.py
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/block_log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7229 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)    20161 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/chain.py
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/chain_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17253 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/chainapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    37974 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/chaintester.py
--rw-r--r--   0 runner    (1001) docker     (122)   108136 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/database.py
--rw-r--r--   0 runner    (1001) docker     (122)    76191 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/database_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/debug_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     7043 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/eos.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/exec_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.277138 ipyeos-0.4.7/pysrc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/Apply.py
--rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 runner    (1001) docker     (122)   157707 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/PushActions.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/interfaces/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/ipykernel_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/ipython_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/log.py
--rw-r--r--   0 runner    (1001) docker     (122)    13232 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/native_modules.py
--rw-r--r--   0 runner    (1001) docker     (122)    55895 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/net.py
--rw-r--r--   0 runner    (1001) docker     (122)    15699 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/node.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/node_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8128 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/packer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/resource_limit.py
--rw-r--r--   0 runner    (1001) docker     (122)     7869 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/rpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6296 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    53096 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)    10657 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/state_history.py
--rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.281138 ipyeos-0.4.7/pysrc/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/deposit_withdraw_prototype.py
--rw-r--r--   0 runner    (1001) docker     (122)     6482 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_eosio_system.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_kv.py
--rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_micropython.py
--rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_powerup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_producers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4543 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_rex.py
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/trace_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/transaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     5384 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/uvicorn_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     8621 2023-07-28 04:47:20.000000 ipyeos-0.4.7/pysrc/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-28 04:47:20.000000 ipyeos-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-28 04:47:32.289138 ipyeos-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-28 04:47:20.000000 ipyeos-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 04:47:32.289138 ipyeos-0.4.7/src/
--rw-r--r--   0 runner    (1001) docker     (122)   340418 2023-07-28 04:47:29.000000 ipyeos-0.4.7/src/_block_log.cpp
--rw-r--r--   0 runner    (1001) docker     (122)  1048098 2023-07-28 04:47:29.000000 ipyeos-0.4.7/src/_chain.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   428264 2023-07-28 04:47:29.000000 ipyeos-0.4.7/src/_chainapi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   403163 2023-07-28 04:47:30.000000 ipyeos-0.4.7/src/_database.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   523398 2023-07-28 04:47:30.000000 ipyeos-0.4.7/src/_eos.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-28 04:47:20.000000 ipyeos-0.4.7/src/_ipyeos.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   346686 2023-07-28 04:47:30.000000 ipyeos-0.4.7/src/_snapshot.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   295599 2023-07-28 04:47:30.000000 ipyeos-0.4.7/src/_state_history.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   302882 2023-07-28 04:47:31.000000 ipyeos-0.4.7/src/_trace_api.cpp
--rw-r--r--   0 runner    (1001) docker     (122)   353667 2023-07-28 04:47:31.000000 ipyeos-0.4.7/src/_transaction.cpp
--rw-r--r--   0 runner    (1001) docker     (122)  1608077 2023-07-28 04:47:31.000000 ipyeos-0.4.7/src/_vm_api.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    26733 2023-07-28 04:47:20.000000 ipyeos-0.4.7/src/_vm_api_.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.554438 ipyeos-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-28 07:50:31.000000 ipyeos-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-28 07:50:31.000000 ipyeos-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-28 07:50:44.554438 ipyeos-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-07-28 07:50:31.000000 ipyeos-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.530438 ipyeos-0.4.8/ipyeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-28 07:50:44.000000 ipyeos-0.4.8/ipyeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.538438 ipyeos-0.4.8/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/args.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/block_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7229 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20161 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/chain_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17253 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/chainapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37974 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/chaintester.py
+-rw-r--r--   0 runner    (1001) docker     (122)   108136 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76191 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/database_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/debug_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7043 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/eos.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/exec_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.542438 ipyeos-0.4.8/pysrc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/Apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/ApplyRequest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   157707 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/IPCChainTester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/PushActions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/interfaces/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/ipykernel_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/ipython_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13232 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/native_modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55895 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/net.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15699 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8128 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/packer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/resource_limit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7869 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6296 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53096 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10657 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/state_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.542438 ipyeos-0.4.8/pysrc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/deposit_withdraw_prototype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6482 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_eosio_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_micropython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_powerup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_producers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4543 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_rex.py
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/trace_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5384 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/uvicorn_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8621 2023-07-28 07:50:31.000000 ipyeos-0.4.8/pysrc/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-28 07:50:31.000000 ipyeos-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-28 07:50:44.554438 ipyeos-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-28 07:50:31.000000 ipyeos-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 07:50:44.554438 ipyeos-0.4.8/src/
+-rw-r--r--   0 runner    (1001) docker     (122)   340418 2023-07-28 07:50:41.000000 ipyeos-0.4.8/src/_block_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)  1046586 2023-07-28 07:50:41.000000 ipyeos-0.4.8/src/_chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   428264 2023-07-28 07:50:41.000000 ipyeos-0.4.8/src/_chainapi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   403163 2023-07-28 07:50:42.000000 ipyeos-0.4.8/src/_database.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   523398 2023-07-28 07:50:42.000000 ipyeos-0.4.8/src/_eos.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-28 07:50:31.000000 ipyeos-0.4.8/src/_ipyeos.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   346686 2023-07-28 07:50:42.000000 ipyeos-0.4.8/src/_snapshot.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   295599 2023-07-28 07:50:42.000000 ipyeos-0.4.8/src/_state_history.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   302882 2023-07-28 07:50:43.000000 ipyeos-0.4.8/src/_trace_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   353667 2023-07-28 07:50:43.000000 ipyeos-0.4.8/src/_transaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)  1608077 2023-07-28 07:50:44.000000 ipyeos-0.4.8/src/_vm_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26733 2023-07-28 07:50:31.000000 ipyeos-0.4.8/src/_vm_api_.cpp
```

### Comparing `ipyeos-0.4.7/LICENSE` & `ipyeos-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/PKG-INFO` & `ipyeos-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.7
+Version: 0.4.8
 Summary: IPYEOS project
 Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -179,15 +179,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.7**.whl
+python3 -m pip install dist/pyeos-0.4.8**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.7/README.md` & `ipyeos-0.4.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.7**.whl
+python3 -m pip install dist/pyeos-0.4.8**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.7/ipyeos.egg-info/PKG-INFO` & `ipyeos-0.4.8/ipyeos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.7
+Version: 0.4.8
 Summary: IPYEOS project
 Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -179,15 +179,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.7**.whl
+python3 -m pip install dist/pyeos-0.4.8**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.7/ipyeos.egg-info/SOURCES.txt` & `ipyeos-0.4.8/ipyeos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/__init__.py` & `ipyeos-0.4.8/pysrc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shlex
 import subprocess
 import sys
 import sysconfig
 
 from . import run
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 cur_dir = os.path.dirname(os.path.realpath(__file__))
 
 def run_ipyeos(custom_cmds=[]):
     return run.run_ipyeos(custom_cmds)
 
 def run_eosnode():
```

### Comparing `ipyeos-0.4.7/pysrc/__main__.py` & `ipyeos-0.4.8/pysrc/__main__.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/args.py` & `ipyeos-0.4.8/pysrc/args.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/block_log.py` & `ipyeos-0.4.8/pysrc/block_log.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/blocks.py` & `ipyeos-0.4.8/pysrc/blocks.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/chain.py` & `ipyeos-0.4.8/pysrc/chain.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/chain_exceptions.py` & `ipyeos-0.4.8/pysrc/chain_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 #  'block_time': '2023-07-14T03:20:09.500',
 #  'elapsed': 208,
 #  'net_usage': 0,
 #  'scheduled': False,
 #  'action_traces': [],
 #  'failed_dtrx_trace': None,
 
-@dataclasses.dataclass
 class TransactionException(ChainException):
     # id: str
     # block_num: int
     # block_time: str
     # elapsed: int
     # net_usage: int
     # scheduled: bool
```

### Comparing `ipyeos-0.4.7/pysrc/chainapi.py` & `ipyeos-0.4.8/pysrc/chainapi.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/chaintester.py` & `ipyeos-0.4.8/pysrc/chaintester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/database.py` & `ipyeos-0.4.8/pysrc/database.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/database_objects.py` & `ipyeos-0.4.8/pysrc/database_objects.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/debug.py` & `ipyeos-0.4.8/pysrc/debug.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/debug_server.py` & `ipyeos-0.4.8/pysrc/debug_server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/eos.py` & `ipyeos-0.4.8/pysrc/eos.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/helper.py` & `ipyeos-0.4.8/pysrc/helper.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/interfaces/Apply.py` & `ipyeos-0.4.8/pysrc/interfaces/Apply.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/interfaces/ApplyRequest.py` & `ipyeos-0.4.8/pysrc/interfaces/ApplyRequest.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/interfaces/IPCChainTester.py` & `ipyeos-0.4.8/pysrc/interfaces/IPCChainTester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/interfaces/PushActions.py` & `ipyeos-0.4.8/pysrc/interfaces/PushActions.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/interfaces/ttypes.py` & `ipyeos-0.4.8/pysrc/interfaces/ttypes.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/ipykernel_embed.py` & `ipyeos-0.4.8/pysrc/ipykernel_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/ipython_embed.py` & `ipyeos-0.4.8/pysrc/ipython_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/log.py` & `ipyeos-0.4.8/pysrc/log.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/main.py` & `ipyeos-0.4.8/pysrc/main.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/native_modules.py` & `ipyeos-0.4.8/pysrc/native_modules.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/net.py` & `ipyeos-0.4.8/pysrc/net.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/node.py` & `ipyeos-0.4.8/pysrc/node.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/node_config.py` & `ipyeos-0.4.8/pysrc/node_config.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/packer.py` & `ipyeos-0.4.8/pysrc/packer.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/rate_limit.py` & `ipyeos-0.4.8/pysrc/rate_limit.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/resource_limit.py` & `ipyeos-0.4.8/pysrc/resource_limit.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/rpc.py` & `ipyeos-0.4.8/pysrc/rpc.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/rpc_server.py` & `ipyeos-0.4.8/pysrc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/run.py` & `ipyeos-0.4.8/pysrc/run.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/server.py` & `ipyeos-0.4.8/pysrc/server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/snapshot.py` & `ipyeos-0.4.8/pysrc/snapshot.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/state_history.py` & `ipyeos-0.4.8/pysrc/state_history.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/structs.py` & `ipyeos-0.4.8/pysrc/structs.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/deposit_withdraw_prototype.py` & `ipyeos-0.4.8/pysrc/tests/deposit_withdraw_prototype.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_chain.py` & `ipyeos-0.4.8/pysrc/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_eosio_system.py` & `ipyeos-0.4.8/pysrc/tests/test_eosio_system.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_kv.py` & `ipyeos-0.4.8/pysrc/tests/test_kv.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_micropython.py` & `ipyeos-0.4.8/pysrc/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_powerup.py` & `ipyeos-0.4.8/pysrc/tests/test_powerup.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_producers.py` & `ipyeos-0.4.8/pysrc/tests/test_producers.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_rex.py` & `ipyeos-0.4.8/pysrc/tests/test_rex.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/tests/test_template.py` & `ipyeos-0.4.8/pysrc/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/trace_api.py` & `ipyeos-0.4.8/pysrc/trace_api.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/transaction.py` & `ipyeos-0.4.8/pysrc/transaction.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/types.py` & `ipyeos-0.4.8/pysrc/types.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/utils.py` & `ipyeos-0.4.8/pysrc/utils.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/pysrc/worker.py` & `ipyeos-0.4.8/pysrc/worker.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/setup.py` & `ipyeos-0.4.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     packages.extend([
         'ipyeos.release.bin',
         'ipyeos.release.lib',
     ])
 
 setup(
     name="ipyeos",
-    version="0.4.7",
+    version="0.4.8",
     description="IPYEOS project",
     author='The IPYEOS Team',
     license="MIT",
     packages=packages,
     package_dir={
         'ipyeos': 'pysrc',
         'ipyeos.interfaces': 'pysrc/interfaces',
```

### Comparing `ipyeos-0.4.7/src/_block_log.cpp` & `ipyeos-0.4.8/src/_block_log.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_chain.cpp` & `ipyeos-0.4.8/src/_chain.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14776,124 +14776,80 @@
 static PyObject *__pyx_pf_6_chain_166push_transaction(CYTHON_UNUSED PyObject *__pyx_self, uint64_t __pyx_v_ptr, PyObject *__pyx_v__packed_trx, int64_t __pyx_v_block_deadline_ms, uint32_t __pyx_v_billed_cpu_time_us, bool __pyx_v_explicit_cpu_bill, uint32_t __pyx_v_subjective_cpu_bill_us, bool __pyx_v_read_only) {
   std::string __pyx_v_result;
   bool __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
-  int __pyx_t_3;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push_transaction", 0);
 
   /* "_chain.pyx":542
  * def push_transaction(uint64_t ptr, _packed_trx: bytes, int64_t block_deadline_ms, uint32_t billed_cpu_time_us, bool explicit_cpu_bill = 0, uint32_t subjective_cpu_bill_us=0, bool read_only = 0):
  *     cdef string result
  *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)             # <<<<<<<<<<<<<<
- *     if ret:
- *         return (ret, result)
+ *     return (ret, result)
+ * 
  */
   __pyx_t_1 = __Pyx_PyBytes_AsWritableString(__pyx_v__packed_trx); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(1, 542, __pyx_L1_error)
   __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v__packed_trx); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 542, __pyx_L1_error)
   __pyx_v_ret = chain(__pyx_v_ptr)->push_transaction(((char *)__pyx_t_1), __pyx_t_2, __pyx_v_block_deadline_ms, __pyx_v_billed_cpu_time_us, __pyx_v_explicit_cpu_bill, __pyx_v_subjective_cpu_bill_us, __pyx_v_read_only, __pyx_v_result);
 
   /* "_chain.pyx":543
  *     cdef string result
  *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)
- *     if ret:             # <<<<<<<<<<<<<<
- *         return (ret, result)
- *     else:
- */
-  __pyx_t_3 = (__pyx_v_ret != 0);
-  if (__pyx_t_3) {
-
-    /* "_chain.pyx":544
- *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)
- *     if ret:
- *         return (ret, result)             # <<<<<<<<<<<<<<
- *     else:
- *         return (ret, None)
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 544, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __pyx_convert_PyStr_string_to_py_std__in_string(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 544, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 544, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
-    __pyx_t_4 = 0;
-    __pyx_t_5 = 0;
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
-    goto __pyx_L0;
-
-    /* "_chain.pyx":543
- *     cdef string result
- *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)
- *     if ret:             # <<<<<<<<<<<<<<
- *         return (ret, result)
- *     else:
- */
-  }
-
-  /* "_chain.pyx":546
- *         return (ret, result)
- *     else:
- *         return (ret, None)             # <<<<<<<<<<<<<<
+ *     return (ret, result)             # <<<<<<<<<<<<<<
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:
  */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 546, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 546, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
-    __Pyx_INCREF(Py_None);
-    __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None);
-    __pyx_t_6 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
-    goto __pyx_L0;
-  }
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 543, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __pyx_convert_PyStr_string_to_py_std__in_string(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 543, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 543, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
+  __pyx_t_3 = 0;
+  __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
 
   /* "_chain.pyx":540
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  * def push_transaction(uint64_t ptr, _packed_trx: bytes, int64_t block_deadline_ms, uint32_t billed_cpu_time_us, bool explicit_cpu_bill = 0, uint32_t subjective_cpu_bill_us=0, bool read_only = 0):             # <<<<<<<<<<<<<<
  *     cdef string result
  *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("_chain.push_transaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":548
- *         return (ret, None)
+/* "_chain.pyx":545
+ *     return (ret, result)
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  */
 
 /* Python wrapper */
@@ -14940,49 +14896,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_block_log_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, 1); __PYX_ERR(1, 548, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, 1); __PYX_ERR(1, 545, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_block_num)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, 2); __PYX_ERR(1, 548, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, 2); __PYX_ERR(1, 545, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_block_from_block_log") < 0)) __PYX_ERR(1, 548, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_block_from_block_log") < 0)) __PYX_ERR(1, 545, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
-    __pyx_v_block_log_ptr = __Pyx_PyInt_As_uint64_t(values[1]); if (unlikely((__pyx_v_block_log_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
-    __pyx_v_block_num = __Pyx_PyInt_As_uint32_t(values[2]); if (unlikely((__pyx_v_block_num == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
+    __pyx_v_block_log_ptr = __Pyx_PyInt_As_uint64_t(values[1]); if (unlikely((__pyx_v_block_log_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
+    __pyx_v_block_num = __Pyx_PyInt_As_uint32_t(values[2]); if (unlikely((__pyx_v_block_num == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 545, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 548, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("push_block_from_block_log", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 545, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.push_block_from_block_log", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_168push_block_from_block_log(__pyx_self, __pyx_v_ptr, __pyx_v_block_log_ptr, __pyx_v_block_num);
 
@@ -14996,30 +14952,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push_block_from_block_log", 0);
 
-  /* "_chain.pyx":549
+  /* "_chain.pyx":546
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)             # <<<<<<<<<<<<<<
  * 
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(chain(__pyx_v_ptr)->push_block_from_block_log(((void *)__pyx_v_block_log_ptr), __pyx_v_block_num)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(chain(__pyx_v_ptr)->push_block_from_block_log(((void *)__pyx_v_block_log_ptr), __pyx_v_block_num)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":548
- *         return (ret, None)
+  /* "_chain.pyx":545
+ *     return (ret, result)
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  */
 
   /* function exit code */
@@ -15029,15 +14985,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":551
+/* "_chain.pyx":548
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):             # <<<<<<<<<<<<<<
  *     cdef string block_statistics
  *     if return_block_statistic:
  */
 
@@ -15085,55 +15041,55 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_raw_block)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, 1); __PYX_ERR(1, 551, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, 1); __PYX_ERR(1, 548, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_block_statistic)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, 2); __PYX_ERR(1, 551, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, 2); __PYX_ERR(1, 548, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_block") < 0)) __PYX_ERR(1, 551, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_block") < 0)) __PYX_ERR(1, 548, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
     __pyx_v_raw_block = ((PyObject*)values[1]);
-    __pyx_v_return_block_statistic = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_return_block_statistic == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L3_error)
+    __pyx_v_return_block_statistic = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_return_block_statistic == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 551, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("push_block", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 548, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.push_block", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_block), (&PyBytes_Type), 0, "raw_block", 1))) __PYX_ERR(1, 551, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_block), (&PyBytes_Type), 0, "raw_block", 1))) __PYX_ERR(1, 548, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_chain_170push_block(__pyx_self, __pyx_v_ptr, __pyx_v_raw_block, __pyx_v_return_block_statistic);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15154,104 +15110,104 @@
   PyObject *__pyx_t_6 = NULL;
   char const *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push_block", 0);
 
-  /* "_chain.pyx":553
+  /* "_chain.pyx":550
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):
  *     cdef string block_statistics
  *     if return_block_statistic:             # <<<<<<<<<<<<<<
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), &block_statistics)
  *         return (ret, block_statistics)
  */
   __pyx_t_1 = (__pyx_v_return_block_statistic != 0);
   if (__pyx_t_1) {
 
-    /* "_chain.pyx":554
+    /* "_chain.pyx":551
  *     cdef string block_statistics
  *     if return_block_statistic:
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), &block_statistics)             # <<<<<<<<<<<<<<
  *         return (ret, block_statistics)
  *     else:
  */
-    __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_raw_block); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 554, __pyx_L1_error)
-    __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_raw_block); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 554, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_raw_block); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 551, __pyx_L1_error)
+    __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_raw_block); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 551, __pyx_L1_error)
     __pyx_v_ret = chain(__pyx_v_ptr)->push_block(((char const *)__pyx_t_2), __pyx_t_3, (&__pyx_v_block_statistics));
 
-    /* "_chain.pyx":555
+    /* "_chain.pyx":552
  *     if return_block_statistic:
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), &block_statistics)
  *         return (ret, block_statistics)             # <<<<<<<<<<<<<<
  *     else:
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), <string *>0)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 555, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 552, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __pyx_convert_PyStr_string_to_py_std__in_string(__pyx_v_block_statistics); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 555, __pyx_L1_error)
+    __pyx_t_5 = __pyx_convert_PyStr_string_to_py_std__in_string(__pyx_v_block_statistics); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 552, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 555, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 552, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
 
-    /* "_chain.pyx":553
+    /* "_chain.pyx":550
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):
  *     cdef string block_statistics
  *     if return_block_statistic:             # <<<<<<<<<<<<<<
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), &block_statistics)
  *         return (ret, block_statistics)
  */
   }
 
-  /* "_chain.pyx":557
+  /* "_chain.pyx":554
  *         return (ret, block_statistics)
  *     else:
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), <string *>0)             # <<<<<<<<<<<<<<
  *         return (ret, None)
  * 
  */
   /*else*/ {
-    __pyx_t_7 = __Pyx_PyBytes_AsString(__pyx_v_raw_block); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 557, __pyx_L1_error)
-    __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_raw_block); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 557, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBytes_AsString(__pyx_v_raw_block); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 554, __pyx_L1_error)
+    __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_raw_block); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 554, __pyx_L1_error)
     __pyx_v_ret = chain(__pyx_v_ptr)->push_block(((char const *)__pyx_t_7), __pyx_t_3, ((std::string *)0));
 
-    /* "_chain.pyx":558
+    /* "_chain.pyx":555
  *     else:
  *         ret = chain(ptr).push_block(<const char *>raw_block, len(raw_block), <string *>0)
  *         return (ret, None)             # <<<<<<<<<<<<<<
  * 
  * def get_scheduled_transactions(uint64_t ptr):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 558, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyBool_FromLong(__pyx_v_ret); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 558, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None);
     __pyx_t_6 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
   }
 
-  /* "_chain.pyx":551
+  /* "_chain.pyx":548
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):             # <<<<<<<<<<<<<<
  *     cdef string block_statistics
  *     if return_block_statistic:
  */
 
@@ -15264,15 +15220,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":560
+/* "_chain.pyx":557
  *         return (ret, None)
  * 
  * def get_scheduled_transactions(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transactions()
  * 
  */
 
@@ -15314,31 +15270,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 557, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_scheduled_transactions") < 0)) __PYX_ERR(1, 560, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_scheduled_transactions") < 0)) __PYX_ERR(1, 557, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 557, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_scheduled_transactions", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 560, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_scheduled_transactions", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 557, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.get_scheduled_transactions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_172get_scheduled_transactions(__pyx_self, __pyx_v_ptr);
 
@@ -15352,29 +15308,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_scheduled_transactions", 0);
 
-  /* "_chain.pyx":561
+  /* "_chain.pyx":558
  * 
  * def get_scheduled_transactions(uint64_t ptr):
  *     return chain(ptr).get_scheduled_transactions()             # <<<<<<<<<<<<<<
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_scheduled_transactions()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 561, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_scheduled_transactions()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":560
+  /* "_chain.pyx":557
  *         return (ret, None)
  * 
  * def get_scheduled_transactions(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transactions()
  * 
  */
 
@@ -15385,15 +15341,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":563
+/* "_chain.pyx":560
  *     return chain(ptr).get_scheduled_transactions()
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  */
 
@@ -15441,55 +15397,55 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sender_id)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, 1); __PYX_ERR(1, 563, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, 1); __PYX_ERR(1, 560, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sender)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, 2); __PYX_ERR(1, 563, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, 2); __PYX_ERR(1, 560, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_scheduled_transaction") < 0)) __PYX_ERR(1, 563, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_scheduled_transaction") < 0)) __PYX_ERR(1, 560, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
     __pyx_v_sender_id = ((PyObject*)values[1]);
-    __pyx_v_sender = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+    __pyx_v_sender = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 563, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_scheduled_transaction", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 560, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.get_scheduled_transaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sender_id), (&PyBytes_Type), 0, "sender_id", 1))) __PYX_ERR(1, 563, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_sender_id), (&PyBytes_Type), 0, "sender_id", 1))) __PYX_ERR(1, 560, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_chain_174get_scheduled_transaction(__pyx_self, __pyx_v_ptr, __pyx_v_sender_id, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_sender));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15504,31 +15460,31 @@
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_scheduled_transaction", 0);
 
-  /* "_chain.pyx":564
+  /* "_chain.pyx":561
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)             # <<<<<<<<<<<<<<
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_AsString(__pyx_v_sender_id); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(1, 564, __pyx_L1_error)
-  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_sender_id); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 564, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_scheduled_transaction(((char const *)__pyx_t_1), __pyx_t_2, __pyx_v_sender)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_AsString(__pyx_v_sender_id); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(1, 561, __pyx_L1_error)
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_sender_id); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 561, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_scheduled_transaction(((char const *)__pyx_t_1), __pyx_t_2, __pyx_v_sender)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":563
+  /* "_chain.pyx":560
  *     return chain(ptr).get_scheduled_transactions()
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  */
 
@@ -15539,15 +15495,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":566
+/* "_chain.pyx":563
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  */
 
@@ -15598,58 +15554,58 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scheduled_tx_id)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 1); __PYX_ERR(1, 566, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 1); __PYX_ERR(1, 563, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 2); __PYX_ERR(1, 566, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 2); __PYX_ERR(1, 563, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_billed_cpu_time_us)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 3); __PYX_ERR(1, 566, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, 3); __PYX_ERR(1, 563, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_scheduled_transaction") < 0)) __PYX_ERR(1, 566, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "push_scheduled_transaction") < 0)) __PYX_ERR(1, 563, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
-    __pyx_v_scheduled_tx_id = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
-    __pyx_v_deadline = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
-    __pyx_v_billed_cpu_time_us = __Pyx_PyInt_As_uint32_t(values[3]); if (unlikely((__pyx_v_billed_cpu_time_us == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+    __pyx_v_scheduled_tx_id = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+    __pyx_v_deadline = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
+    __pyx_v_billed_cpu_time_us = __Pyx_PyInt_As_uint32_t(values[3]); if (unlikely((__pyx_v_billed_cpu_time_us == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 563, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 566, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("push_scheduled_transaction", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 563, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.push_scheduled_transaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_176push_scheduled_transaction(__pyx_self, __pyx_v_ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_scheduled_tx_id), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_deadline), __pyx_v_billed_cpu_time_us);
 
@@ -15663,29 +15619,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push_scheduled_transaction", 0);
 
-  /* "_chain.pyx":567
+  /* "_chain.pyx":564
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)             # <<<<<<<<<<<<<<
  * 
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->push_scheduled_transaction(__pyx_v_scheduled_tx_id, __pyx_v_deadline, __pyx_v_billed_cpu_time_us)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 567, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->push_scheduled_transaction(__pyx_v_scheduled_tx_id, __pyx_v_deadline, __pyx_v_billed_cpu_time_us)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":566
+  /* "_chain.pyx":563
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  */
 
@@ -15696,15 +15652,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":569
+/* "_chain.pyx":566
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:             # <<<<<<<<<<<<<<
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  */
 
@@ -15755,58 +15711,58 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 1); __PYX_ERR(1, 569, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 1); __PYX_ERR(1, 566, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_action)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 2); __PYX_ERR(1, 569, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 2); __PYX_ERR(1, 566, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_args)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 3); __PYX_ERR(1, 569, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, 3); __PYX_ERR(1, 566, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "pack_action_args") < 0)) __PYX_ERR(1, 569, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "pack_action_args") < 0)) __PYX_ERR(1, 566, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
-    __pyx_v_name = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
-    __pyx_v_action = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
-    __pyx_v__args = __pyx_convert_string_from_py_std__in_string(values[3]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+    __pyx_v_name = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+    __pyx_v_action = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
+    __pyx_v__args = __pyx_convert_string_from_py_std__in_string(values[3]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 566, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 569, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("pack_action_args", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 566, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.pack_action_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_178pack_action_args(__pyx_self, __pyx_v_ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_name), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_action), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v__args));
 
@@ -15822,59 +15778,59 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pack_action_args", 0);
 
-  /* "_chain.pyx":571
+  /* "_chain.pyx":568
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):             # <<<<<<<<<<<<<<
  *         return None
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  */
   __pyx_t_1 = (!(chain(__pyx_v_ptr)->pack_action_args(__pyx_v_name, __pyx_v_action, __pyx_v__args, __pyx_v_result) != 0));
   if (__pyx_t_1) {
 
-    /* "_chain.pyx":572
+    /* "_chain.pyx":569
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  *         return None             # <<<<<<<<<<<<<<
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "_chain.pyx":571
+    /* "_chain.pyx":568
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):             # <<<<<<<<<<<<<<
  *         return None
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  */
   }
 
-  /* "_chain.pyx":573
+  /* "_chain.pyx":570
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  *         return None
  *     return PyBytes_FromStringAndSize(result.data(), result.size())             # <<<<<<<<<<<<<<
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyBytes_FromStringAndSize(__pyx_v_result.data(), __pyx_v_result.size()); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 573, __pyx_L1_error)
+  __pyx_t_2 = PyBytes_FromStringAndSize(__pyx_v_result.data(), __pyx_v_result.size()); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":569
+  /* "_chain.pyx":566
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:             # <<<<<<<<<<<<<<
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  */
 
@@ -15885,15 +15841,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":575
+/* "_chain.pyx":572
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):             # <<<<<<<<<<<<<<
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  */
 
@@ -15944,58 +15900,58 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 572, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 572, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 1); __PYX_ERR(1, 575, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 1); __PYX_ERR(1, 572, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_action)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 572, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 2); __PYX_ERR(1, 575, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 2); __PYX_ERR(1, 572, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_binargs)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 572, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 3); __PYX_ERR(1, 575, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, 3); __PYX_ERR(1, 572, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unpack_action_args") < 0)) __PYX_ERR(1, 575, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "unpack_action_args") < 0)) __PYX_ERR(1, 572, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 572, __pyx_L3_error)
     __pyx_v_name = values[1];
     __pyx_v_action = values[2];
     __pyx_v__binargs = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 575, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("unpack_action_args", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 572, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.unpack_action_args", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_180unpack_action_args(__pyx_self, __pyx_v_ptr, __pyx_v_name, __pyx_v_action, __pyx_v__binargs);
 
@@ -16012,32 +15968,32 @@
   std::string __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unpack_action_args", 0);
 
-  /* "_chain.pyx":576
+  /* "_chain.pyx":573
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):
  *     return chain(ptr).unpack_action_args(name, action, _binargs)             # <<<<<<<<<<<<<<
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_name); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 576, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_v_action); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 576, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_v__binargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 576, __pyx_L1_error)
-  __pyx_t_4 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->unpack_action_args(__pyx_t_1, __pyx_t_2, __pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 576, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_name); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 573, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_v_action); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 573, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_v__binargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 573, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->unpack_action_args(__pyx_t_1, __pyx_t_2, __pyx_t_3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 573, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":575
+  /* "_chain.pyx":572
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):             # <<<<<<<<<<<<<<
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  */
 
@@ -16048,15 +16004,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":578
+/* "_chain.pyx":575
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):             # <<<<<<<<<<<<<<
  *     return chain(ptr).clear_abi_cache(account)
  * 
  */
 
@@ -16101,40 +16057,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_account)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("clear_abi_cache", 1, 2, 2, 1); __PYX_ERR(1, 578, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("clear_abi_cache", 1, 2, 2, 1); __PYX_ERR(1, 575, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "clear_abi_cache") < 0)) __PYX_ERR(1, 578, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "clear_abi_cache") < 0)) __PYX_ERR(1, 575, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
-    __pyx_v_account = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
+    __pyx_v_account = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("clear_abi_cache", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 578, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("clear_abi_cache", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 575, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.clear_abi_cache", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_182clear_abi_cache(__pyx_self, __pyx_v_ptr, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_account));
 
@@ -16148,29 +16104,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear_abi_cache", 0);
 
-  /* "_chain.pyx":579
+  /* "_chain.pyx":576
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):
  *     return chain(ptr).clear_abi_cache(account)             # <<<<<<<<<<<<<<
  * 
  * def get_producer_public_keys(uint64_t ptr):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(chain(__pyx_v_ptr)->clear_abi_cache(__pyx_v_account)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(chain(__pyx_v_ptr)->clear_abi_cache(__pyx_v_account)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":578
+  /* "_chain.pyx":575
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):             # <<<<<<<<<<<<<<
  *     return chain(ptr).clear_abi_cache(account)
  * 
  */
 
@@ -16181,15 +16137,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":581
+/* "_chain.pyx":578
  *     return chain(ptr).clear_abi_cache(account)
  * 
  * def get_producer_public_keys(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_producer_public_keys()
  * 
  */
 
@@ -16231,31 +16187,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 581, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_producer_public_keys") < 0)) __PYX_ERR(1, 581, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_producer_public_keys") < 0)) __PYX_ERR(1, 578, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 581, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 578, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_producer_public_keys", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 581, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_producer_public_keys", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 578, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.get_producer_public_keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_184get_producer_public_keys(__pyx_self, __pyx_v_ptr);
 
@@ -16269,29 +16225,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_producer_public_keys", 0);
 
-  /* "_chain.pyx":582
+  /* "_chain.pyx":579
  * 
  * def get_producer_public_keys(uint64_t ptr):
  *     return chain(ptr).get_producer_public_keys()             # <<<<<<<<<<<<<<
  * 
  * #string get_native_contract(uint64_t contract)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_producer_public_keys()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 582, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyStr_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_producer_public_keys()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":581
+  /* "_chain.pyx":578
  *     return chain(ptr).clear_abi_cache(account)
  * 
  * def get_producer_public_keys(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_producer_public_keys()
  * 
  */
 
@@ -16302,15 +16258,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":585
+/* "_chain.pyx":582
  * 
  * #string get_native_contract(uint64_t contract)
  * def get_native_contract(uint64_t ptr, contract: str) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_native_contract(contract)
  * 
  */
 
@@ -16355,46 +16311,46 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 585, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 582, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_contract)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 585, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 582, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_native_contract", 1, 2, 2, 1); __PYX_ERR(1, 585, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_native_contract", 1, 2, 2, 1); __PYX_ERR(1, 582, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_native_contract") < 0)) __PYX_ERR(1, 585, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_native_contract") < 0)) __PYX_ERR(1, 582, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 585, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 582, __pyx_L3_error)
     __pyx_v_contract = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_native_contract", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 585, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_native_contract", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 582, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.get_native_contract", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_contract), (&PyUnicode_Type), 0, "contract", 1))) __PYX_ERR(1, 585, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_contract), (&PyUnicode_Type), 0, "contract", 1))) __PYX_ERR(1, 582, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_chain_186get_native_contract(__pyx_self, __pyx_v_ptr, __pyx_v_contract);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16408,30 +16364,30 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_native_contract", 0);
 
-  /* "_chain.pyx":586
+  /* "_chain.pyx":583
  * #string get_native_contract(uint64_t contract)
  * def get_native_contract(uint64_t ptr, contract: str) -> str:
  *     return chain(ptr).get_native_contract(contract)             # <<<<<<<<<<<<<<
  * 
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_contract); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_PyUnicode_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_native_contract(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 586, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_contract); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 583, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyUnicode_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_native_contract(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":585
+  /* "_chain.pyx":582
  * 
  * #string get_native_contract(uint64_t contract)
  * def get_native_contract(uint64_t ptr, contract: str) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_native_contract(contract)
  * 
  */
 
@@ -16442,15 +16398,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":589
+/* "_chain.pyx":586
  * 
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  * def set_native_contract(uint64_t ptr, contract: str, const string& native_contract_lib) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).set_native_contract(contract, native_contract_lib)
  * 
  */
 
@@ -16498,55 +16454,55 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 589, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_contract)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 589, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, 1); __PYX_ERR(1, 589, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, 1); __PYX_ERR(1, 586, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_native_contract_lib)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 589, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, 2); __PYX_ERR(1, 589, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, 2); __PYX_ERR(1, 586, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_native_contract") < 0)) __PYX_ERR(1, 589, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_native_contract") < 0)) __PYX_ERR(1, 586, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 589, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L3_error)
     __pyx_v_contract = ((PyObject*)values[1]);
-    __pyx_v_native_contract_lib = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 589, __pyx_L3_error)
+    __pyx_v_native_contract_lib = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 586, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 589, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_native_contract", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 586, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.set_native_contract", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_contract), (&PyUnicode_Type), 0, "contract", 1))) __PYX_ERR(1, 589, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_contract), (&PyUnicode_Type), 0, "contract", 1))) __PYX_ERR(1, 586, __pyx_L1_error)
   __pyx_r = __pyx_pf_6_chain_188set_native_contract(__pyx_self, __pyx_v_ptr, __pyx_v_contract, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_native_contract_lib));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16560,30 +16516,30 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_native_contract", 0);
 
-  /* "_chain.pyx":590
+  /* "_chain.pyx":587
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  * def set_native_contract(uint64_t ptr, contract: str, const string& native_contract_lib) -> bool:
  *     return chain(ptr).set_native_contract(contract, native_contract_lib)             # <<<<<<<<<<<<<<
  * 
  * # def set_debug_producer_key(uint64_t ptr, string &pub_key):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_contract); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 590, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyBool_FromLong(chain(__pyx_v_ptr)->set_native_contract(__pyx_t_1, __pyx_v_native_contract_lib)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 590, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_contract); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 587, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(chain(__pyx_v_ptr)->set_native_contract(__pyx_t_1, __pyx_v_native_contract_lib)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":589
+  /* "_chain.pyx":586
  * 
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  * def set_native_contract(uint64_t ptr, contract: str, const string& native_contract_lib) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).set_native_contract(contract, native_contract_lib)
  * 
  */
 
@@ -16594,15 +16550,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_chain.pyx":595
+/* "_chain.pyx":592
  * #     chain(ptr).set_debug_producer_key(pub_key)
  * 
  * def get_debug_producer_key(uint64_t ptr) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_debug_producer_key()
  */
 
 /* Python wrapper */
@@ -16643,31 +16599,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ptr)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 595, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 592, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_debug_producer_key") < 0)) __PYX_ERR(1, 595, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_debug_producer_key") < 0)) __PYX_ERR(1, 592, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 595, __pyx_L3_error)
+    __pyx_v_ptr = __Pyx_PyInt_As_uint64_t(values[0]); if (unlikely((__pyx_v_ptr == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 592, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_debug_producer_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 595, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_debug_producer_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 592, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_chain.get_debug_producer_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6_chain_190get_debug_producer_key(__pyx_self, __pyx_v_ptr);
 
@@ -16681,27 +16637,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_debug_producer_key", 0);
 
-  /* "_chain.pyx":596
+  /* "_chain.pyx":593
  * 
  * def get_debug_producer_key(uint64_t ptr) -> str:
  *     return chain(ptr).get_debug_producer_key()             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_debug_producer_key()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 596, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_PyUnicode_string_to_py_std__in_string(chain(__pyx_v_ptr)->get_debug_producer_key()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_chain.pyx":595
+  /* "_chain.pyx":592
  * #     chain(ptr).set_debug_producer_key(pub_key)
  * 
  * def get_debug_producer_key(uint64_t ptr) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_debug_producer_key()
  */
 
   /* function exit code */
@@ -17722,147 +17678,147 @@
  *     ret = chain(ptr).push_transaction(<char *>_packed_trx, len(_packed_trx), block_deadline_ms, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us, read_only, result)
  */
   __pyx_tuple__103 = PyTuple_Pack(9, __pyx_n_s_ptr, __pyx_n_s_packed_trx, __pyx_n_s_block_deadline_ms, __pyx_n_s_billed_cpu_time_us, __pyx_n_s_explicit_cpu_bill, __pyx_n_s_subjective_cpu_bill_us, __pyx_n_s_read_only, __pyx_n_s_result, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__103)) __PYX_ERR(1, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__103);
   __Pyx_GIVEREF(__pyx_tuple__103);
   __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__103, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_transaction, 540, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(1, 540, __pyx_L1_error)
 
-  /* "_chain.pyx":548
- *         return (ret, None)
+  /* "_chain.pyx":545
+ *     return (ret, result)
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  */
-  __pyx_tuple__105 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_block_log_ptr, __pyx_n_s_block_num); if (unlikely(!__pyx_tuple__105)) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_tuple__105 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_block_log_ptr, __pyx_n_s_block_num); if (unlikely(!__pyx_tuple__105)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__105);
   __Pyx_GIVEREF(__pyx_tuple__105);
-  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__105, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_block_from_block_log, 548, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__105, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_block_from_block_log, 545, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(1, 545, __pyx_L1_error)
 
-  /* "_chain.pyx":551
+  /* "_chain.pyx":548
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):             # <<<<<<<<<<<<<<
  *     cdef string block_statistics
  *     if return_block_statistic:
  */
-  __pyx_tuple__107 = PyTuple_Pack(5, __pyx_n_s_ptr, __pyx_n_s_raw_block, __pyx_n_s_return_block_statistic, __pyx_n_s_block_statistics, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__107)) __PYX_ERR(1, 551, __pyx_L1_error)
+  __pyx_tuple__107 = PyTuple_Pack(5, __pyx_n_s_ptr, __pyx_n_s_raw_block, __pyx_n_s_return_block_statistic, __pyx_n_s_block_statistics, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__107)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__107);
   __Pyx_GIVEREF(__pyx_tuple__107);
-  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__107, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_block, 551, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(1, 551, __pyx_L1_error)
+  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__107, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_block, 548, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(1, 548, __pyx_L1_error)
 
-  /* "_chain.pyx":560
+  /* "_chain.pyx":557
  *         return (ret, None)
  * 
  * def get_scheduled_transactions(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transactions()
  * 
  */
-  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_scheduled_transactions, 560, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(1, 560, __pyx_L1_error)
+  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_scheduled_transactions, 557, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(1, 557, __pyx_L1_error)
 
-  /* "_chain.pyx":563
+  /* "_chain.pyx":560
  *     return chain(ptr).get_scheduled_transactions()
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  */
-  __pyx_tuple__110 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_sender_id, __pyx_n_s_sender); if (unlikely(!__pyx_tuple__110)) __PYX_ERR(1, 563, __pyx_L1_error)
+  __pyx_tuple__110 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_sender_id, __pyx_n_s_sender); if (unlikely(!__pyx_tuple__110)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__110);
   __Pyx_GIVEREF(__pyx_tuple__110);
-  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__110, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_scheduled_transaction, 563, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(1, 563, __pyx_L1_error)
+  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__110, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_scheduled_transaction, 560, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(1, 560, __pyx_L1_error)
 
-  /* "_chain.pyx":566
+  /* "_chain.pyx":563
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  */
-  __pyx_tuple__112 = PyTuple_Pack(4, __pyx_n_s_ptr, __pyx_n_s_scheduled_tx_id, __pyx_n_s_deadline, __pyx_n_s_billed_cpu_time_us); if (unlikely(!__pyx_tuple__112)) __PYX_ERR(1, 566, __pyx_L1_error)
+  __pyx_tuple__112 = PyTuple_Pack(4, __pyx_n_s_ptr, __pyx_n_s_scheduled_tx_id, __pyx_n_s_deadline, __pyx_n_s_billed_cpu_time_us); if (unlikely(!__pyx_tuple__112)) __PYX_ERR(1, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__112);
   __Pyx_GIVEREF(__pyx_tuple__112);
-  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__112, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_scheduled_transaction, 566, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(1, 566, __pyx_L1_error)
+  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__112, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_push_scheduled_transaction, 563, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(1, 563, __pyx_L1_error)
 
-  /* "_chain.pyx":569
+  /* "_chain.pyx":566
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:             # <<<<<<<<<<<<<<
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  */
-  __pyx_tuple__114 = PyTuple_Pack(5, __pyx_n_s_ptr, __pyx_n_s_name, __pyx_n_s_action, __pyx_n_s_args, __pyx_n_s_result); if (unlikely(!__pyx_tuple__114)) __PYX_ERR(1, 569, __pyx_L1_error)
+  __pyx_tuple__114 = PyTuple_Pack(5, __pyx_n_s_ptr, __pyx_n_s_name, __pyx_n_s_action, __pyx_n_s_args, __pyx_n_s_result); if (unlikely(!__pyx_tuple__114)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__114);
   __Pyx_GIVEREF(__pyx_tuple__114);
-  __pyx_codeobj__115 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__114, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_pack_action_args, 569, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__115)) __PYX_ERR(1, 569, __pyx_L1_error)
+  __pyx_codeobj__115 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__114, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_pack_action_args, 566, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__115)) __PYX_ERR(1, 566, __pyx_L1_error)
 
-  /* "_chain.pyx":575
+  /* "_chain.pyx":572
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):             # <<<<<<<<<<<<<<
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  */
-  __pyx_tuple__116 = PyTuple_Pack(4, __pyx_n_s_ptr, __pyx_n_s_name, __pyx_n_s_action, __pyx_n_s_binargs); if (unlikely(!__pyx_tuple__116)) __PYX_ERR(1, 575, __pyx_L1_error)
+  __pyx_tuple__116 = PyTuple_Pack(4, __pyx_n_s_ptr, __pyx_n_s_name, __pyx_n_s_action, __pyx_n_s_binargs); if (unlikely(!__pyx_tuple__116)) __PYX_ERR(1, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__116);
   __Pyx_GIVEREF(__pyx_tuple__116);
-  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__116, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_unpack_action_args, 575, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(1, 575, __pyx_L1_error)
+  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__116, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_unpack_action_args, 572, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(1, 572, __pyx_L1_error)
 
-  /* "_chain.pyx":578
+  /* "_chain.pyx":575
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):             # <<<<<<<<<<<<<<
  *     return chain(ptr).clear_abi_cache(account)
  * 
  */
-  __pyx_tuple__118 = PyTuple_Pack(2, __pyx_n_s_ptr, __pyx_n_s_account); if (unlikely(!__pyx_tuple__118)) __PYX_ERR(1, 578, __pyx_L1_error)
+  __pyx_tuple__118 = PyTuple_Pack(2, __pyx_n_s_ptr, __pyx_n_s_account); if (unlikely(!__pyx_tuple__118)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__118);
   __Pyx_GIVEREF(__pyx_tuple__118);
-  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_clear_abi_cache, 578, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(1, 578, __pyx_L1_error)
+  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_clear_abi_cache, 575, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(1, 575, __pyx_L1_error)
 
-  /* "_chain.pyx":581
+  /* "_chain.pyx":578
  *     return chain(ptr).clear_abi_cache(account)
  * 
  * def get_producer_public_keys(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_producer_public_keys()
  * 
  */
-  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_producer_public_keys, 581, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(1, 581, __pyx_L1_error)
+  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_producer_public_keys, 578, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(1, 578, __pyx_L1_error)
 
-  /* "_chain.pyx":585
+  /* "_chain.pyx":582
  * 
  * #string get_native_contract(uint64_t contract)
  * def get_native_contract(uint64_t ptr, contract: str) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_native_contract(contract)
  * 
  */
-  __pyx_tuple__121 = PyTuple_Pack(2, __pyx_n_s_ptr, __pyx_n_s_contract); if (unlikely(!__pyx_tuple__121)) __PYX_ERR(1, 585, __pyx_L1_error)
+  __pyx_tuple__121 = PyTuple_Pack(2, __pyx_n_s_ptr, __pyx_n_s_contract); if (unlikely(!__pyx_tuple__121)) __PYX_ERR(1, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__121);
   __Pyx_GIVEREF(__pyx_tuple__121);
-  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__121, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_native_contract, 585, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(1, 585, __pyx_L1_error)
+  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__121, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_native_contract, 582, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(1, 582, __pyx_L1_error)
 
-  /* "_chain.pyx":589
+  /* "_chain.pyx":586
  * 
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  * def set_native_contract(uint64_t ptr, contract: str, const string& native_contract_lib) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).set_native_contract(contract, native_contract_lib)
  * 
  */
-  __pyx_tuple__123 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_contract, __pyx_n_s_native_contract_lib); if (unlikely(!__pyx_tuple__123)) __PYX_ERR(1, 589, __pyx_L1_error)
+  __pyx_tuple__123 = PyTuple_Pack(3, __pyx_n_s_ptr, __pyx_n_s_contract, __pyx_n_s_native_contract_lib); if (unlikely(!__pyx_tuple__123)) __PYX_ERR(1, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__123);
   __Pyx_GIVEREF(__pyx_tuple__123);
-  __pyx_codeobj__124 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__123, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_set_native_contract, 589, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__124)) __PYX_ERR(1, 589, __pyx_L1_error)
+  __pyx_codeobj__124 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__123, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_set_native_contract, 586, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__124)) __PYX_ERR(1, 586, __pyx_L1_error)
 
-  /* "_chain.pyx":595
+  /* "_chain.pyx":592
  * #     chain(ptr).set_debug_producer_key(pub_key)
  * 
  * def get_debug_producer_key(uint64_t ptr) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_debug_producer_key()
  */
-  __pyx_codeobj__125 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_debug_producer_key, 595, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__125)) __PYX_ERR(1, 595, __pyx_L1_error)
+  __pyx_codeobj__125 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__chain_pyx, __pyx_n_s_get_debug_producer_key, 592, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__125)) __PYX_ERR(1, 592, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -19316,192 +19272,192 @@
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_transaction, __pyx_t_2) < 0) __PYX_ERR(1, 540, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":548
- *         return (ret, None)
+  /* "_chain.pyx":545
+ *     return (ret, result)
  * 
  * def push_block_from_block_log(uint64_t ptr, uint64_t block_log_ptr, uint32_t block_num) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_169push_block_from_block_log, 0, __pyx_n_s_push_block_from_block_log, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_169push_block_from_block_log, 0, __pyx_n_s_push_block_from_block_log, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_block_from_block_log, __pyx_t_4) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_block_from_block_log, __pyx_t_4) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_chain.pyx":551
+  /* "_chain.pyx":548
  *     return chain(ptr).push_block_from_block_log(<void *>block_log_ptr, block_num)
  * 
  * def push_block(uint64_t ptr, raw_block: bytes, bool return_block_statistic):             # <<<<<<<<<<<<<<
  *     cdef string block_statistics
  *     if return_block_statistic:
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 551, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_raw_block, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_171push_block, 0, __pyx_n_s_push_block, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 551, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_raw_block, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_171push_block, 0, __pyx_n_s_push_block, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_block, __pyx_t_2) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_block, __pyx_t_2) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":560
+  /* "_chain.pyx":557
  *         return (ret, None)
  * 
  * def get_scheduled_transactions(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transactions()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_173get_scheduled_transactions, 0, __pyx_n_s_get_scheduled_transactions, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 560, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_173get_scheduled_transactions, 0, __pyx_n_s_get_scheduled_transactions, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_scheduled_transactions, __pyx_t_2) < 0) __PYX_ERR(1, 560, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_scheduled_transactions, __pyx_t_2) < 0) __PYX_ERR(1, 557, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":563
+  /* "_chain.pyx":560
  *     return chain(ptr).get_scheduled_transactions()
  * 
  * def get_scheduled_transaction(uint64_t ptr, sender_id: bytes, string& sender):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 563, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_sender_id, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_175get_scheduled_transaction, 0, __pyx_n_s_get_scheduled_transaction, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 563, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_sender_id, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 560, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_175get_scheduled_transaction, 0, __pyx_n_s_get_scheduled_transaction, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_scheduled_transaction, __pyx_t_4) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_scheduled_transaction, __pyx_t_4) < 0) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_chain.pyx":566
+  /* "_chain.pyx":563
  *     return chain(ptr).get_scheduled_transaction(<const char *>sender_id, len(sender_id), sender)
  * 
  * def push_scheduled_transaction(uint64_t ptr, string& scheduled_tx_id, string& deadline, uint32_t billed_cpu_time_us):             # <<<<<<<<<<<<<<
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_177push_scheduled_transaction, 0, __pyx_n_s_push_scheduled_transaction, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 566, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_177push_scheduled_transaction, 0, __pyx_n_s_push_scheduled_transaction, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_scheduled_transaction, __pyx_t_4) < 0) __PYX_ERR(1, 566, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_push_scheduled_transaction, __pyx_t_4) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_chain.pyx":569
+  /* "_chain.pyx":566
  *     return chain(ptr).push_scheduled_transaction(scheduled_tx_id, deadline, billed_cpu_time_us)
  * 
  * def pack_action_args(uint64_t ptr, string& name, string& action, string& _args) -> Union[bytes, None]:             # <<<<<<<<<<<<<<
  *     cdef vector[char] result
  *     if not chain(ptr).pack_action_args(name, action, _args, result):
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 569, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_kp_s_Union_bytes_None) < 0) __PYX_ERR(1, 569, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_179pack_action_args, 0, __pyx_n_s_pack_action_args, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__115)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 569, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_kp_s_Union_bytes_None) < 0) __PYX_ERR(1, 566, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_179pack_action_args, 0, __pyx_n_s_pack_action_args, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__115)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pack_action_args, __pyx_t_2) < 0) __PYX_ERR(1, 569, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pack_action_args, __pyx_t_2) < 0) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":575
+  /* "_chain.pyx":572
  *     return PyBytes_FromStringAndSize(result.data(), result.size())
  * 
  * def unpack_action_args(uint64_t ptr, name, action, _binargs):             # <<<<<<<<<<<<<<
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_181unpack_action_args, 0, __pyx_n_s_unpack_action_args, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_181unpack_action_args, 0, __pyx_n_s_unpack_action_args, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unpack_action_args, __pyx_t_2) < 0) __PYX_ERR(1, 575, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_unpack_action_args, __pyx_t_2) < 0) __PYX_ERR(1, 572, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":578
+  /* "_chain.pyx":575
  *     return chain(ptr).unpack_action_args(name, action, _binargs)
  * 
  * def clear_abi_cache(uint64_t ptr, string& account):             # <<<<<<<<<<<<<<
  *     return chain(ptr).clear_abi_cache(account)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_183clear_abi_cache, 0, __pyx_n_s_clear_abi_cache, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 578, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_183clear_abi_cache, 0, __pyx_n_s_clear_abi_cache, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_clear_abi_cache, __pyx_t_2) < 0) __PYX_ERR(1, 578, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_clear_abi_cache, __pyx_t_2) < 0) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":581
+  /* "_chain.pyx":578
  *     return chain(ptr).clear_abi_cache(account)
  * 
  * def get_producer_public_keys(uint64_t ptr):             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_producer_public_keys()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_185get_producer_public_keys, 0, __pyx_n_s_get_producer_public_keys, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 581, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_185get_producer_public_keys, 0, __pyx_n_s_get_producer_public_keys, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_producer_public_keys, __pyx_t_2) < 0) __PYX_ERR(1, 581, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_producer_public_keys, __pyx_t_2) < 0) __PYX_ERR(1, 578, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":585
+  /* "_chain.pyx":582
  * 
  * #string get_native_contract(uint64_t contract)
  * def get_native_contract(uint64_t ptr, contract: str) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_native_contract(contract)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 585, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_contract, __pyx_n_s_str) < 0) __PYX_ERR(1, 585, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(1, 585, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_187get_native_contract, 0, __pyx_n_s_get_native_contract, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 585, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_contract, __pyx_n_s_str) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_187get_native_contract, 0, __pyx_n_s_get_native_contract, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_native_contract, __pyx_t_4) < 0) __PYX_ERR(1, 585, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_native_contract, __pyx_t_4) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_chain.pyx":589
+  /* "_chain.pyx":586
  * 
  * #bool set_native_contract(uint64_t contract, const string& native_contract_lib)
  * def set_native_contract(uint64_t ptr, contract: str, const string& native_contract_lib) -> bool:             # <<<<<<<<<<<<<<
  *     return chain(ptr).set_native_contract(contract, native_contract_lib)
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 589, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_contract, __pyx_n_s_str) < 0) __PYX_ERR(1, 589, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(1, 589, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_189set_native_contract, 0, __pyx_n_s_set_native_contract, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__124)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 589, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_contract, __pyx_n_s_str) < 0) __PYX_ERR(1, 586, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(1, 586, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_189set_native_contract, 0, __pyx_n_s_set_native_contract, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__124)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_native_contract, __pyx_t_2) < 0) __PYX_ERR(1, 589, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_native_contract, __pyx_t_2) < 0) __PYX_ERR(1, 586, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_chain.pyx":595
+  /* "_chain.pyx":592
  * #     chain(ptr).set_debug_producer_key(pub_key)
  * 
  * def get_debug_producer_key(uint64_t ptr) -> str:             # <<<<<<<<<<<<<<
  *     return chain(ptr).get_debug_producer_key()
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 595, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(1, 595, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_191get_debug_producer_key, 0, __pyx_n_s_get_debug_producer_key, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__125)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 595, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(1, 592, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6_chain_191get_debug_producer_key, 0, __pyx_n_s_get_debug_producer_key, NULL, __pyx_n_s_chain, __pyx_d, ((PyObject *)__pyx_codeobj__125)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_debug_producer_key, __pyx_t_4) < 0) __PYX_ERR(1, 595, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_debug_producer_key, __pyx_t_4) < 0) __PYX_ERR(1, 592, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "_chain.pyx":1
  * # cython: language_level=3, c_string_type=str, c_string_encoding=utf8             # <<<<<<<<<<<<<<
  * 
  * from typing import Union
  */
```

### Comparing `ipyeos-0.4.7/src/_chainapi.cpp` & `ipyeos-0.4.8/src/_chainapi.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_database.cpp` & `ipyeos-0.4.8/src/_database.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_eos.cpp` & `ipyeos-0.4.8/src/_eos.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_ipyeos.cpp` & `ipyeos-0.4.8/src/_ipyeos.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_snapshot.cpp` & `ipyeos-0.4.8/src/_snapshot.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_state_history.cpp` & `ipyeos-0.4.8/src/_state_history.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_trace_api.cpp` & `ipyeos-0.4.8/src/_trace_api.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_transaction.cpp` & `ipyeos-0.4.8/src/_transaction.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_vm_api.cpp` & `ipyeos-0.4.8/src/_vm_api.cpp`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.7/src/_vm_api_.cpp` & `ipyeos-0.4.8/src/_vm_api_.cpp`

 * *Files identical despite different names*

