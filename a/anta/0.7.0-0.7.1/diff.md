# Comparing `tmp/anta-0.7.0.tar.gz` & `tmp/anta-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anta-0.7.0.tar", last modified: Fri Jul 28 10:41:05 2023, max compression
+gzip compressed data, was "anta-0.7.1.tar", last modified: Fri Jul 28 11:20:48 2023, max compression
```

## Comparing `anta-0.7.0.tar` & `anta-0.7.1.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.815518 anta-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-28 10:40:55.000000 anta-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 10:40:55.000000 anta-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-28 10:41:05.815518 anta-0.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-28 10:40:55.000000 anta-0.7.0/anta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/debug/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/cli/nrfu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-28 10:40:55.000000 anta-0.7.0/anta/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-28 10:40:55.000000 anta-0.7.0/anta/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-28 10:40:55.000000 anta-0.7.0/anta/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-07-28 10:40:55.000000 anta-0.7.0/anta/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/reporter/
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-28 10:40:55.000000 anta-0.7.0/anta/reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-28 10:40:55.000000 anta-0.7.0/anta/reporter/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/result_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-28 10:40:55.000000 anta-0.7.0/anta/result_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-28 10:40:55.000000 anta-0.7.0/anta/result_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-28 10:40:55.000000 anta-0.7.0/anta/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/aaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/field_notices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/mlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/multicast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tests/routing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/software.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/vxlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/get_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-28 10:40:55.000000 anta-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:41:05.815518 anta-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.732905 anta-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-28 11:20:38.000000 anta-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 11:20:38.000000 anta-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-28 11:20:48.732905 anta-0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-28 11:20:38.000000 anta-0.7.1/anta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta/cli/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/exec/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/exec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/get/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/get/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/cli/nrfu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/nrfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/nrfu/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/nrfu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-28 11:20:38.000000 anta-0.7.1/anta/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-28 11:20:38.000000 anta-0.7.1/anta/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-28 11:20:38.000000 anta-0.7.1/anta/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-28 11:20:38.000000 anta-0.7.1/anta/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 11:20:38.000000 anta-0.7.1/anta/inventory/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-28 11:20:38.000000 anta-0.7.1/anta/inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-28 11:20:38.000000 anta-0.7.1/anta/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-07-28 11:20:38.000000 anta-0.7.1/anta/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-28 11:20:38.000000 anta-0.7.1/anta/reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-28 11:20:38.000000 anta-0.7.1/anta/reporter/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/result_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-28 11:20:38.000000 anta-0.7.1/anta/result_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-28 11:20:38.000000 anta-0.7.1/anta/result_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-28 11:20:38.000000 anta-0.7.1/anta/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/field_notices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/mlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/multicast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.728905 anta-0.7.1/anta/tests/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/routing/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/routing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/routing/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tests/vxlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.732905 anta-0.7.1/anta/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tools/get_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-28 11:20:38.000000 anta-0.7.1/anta/tools/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.724905 anta-0.7.1/anta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 11:20:48.000000 anta-0.7.1/anta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:20:48.732905 anta-0.7.1/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4102 2023-07-28 11:20:38.000000 anta-0.7.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-07-28 11:20:38.000000 anta-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:20:48.732905 anta-0.7.1/setup.cfg
```

### Comparing `anta-0.7.0/LICENSE` & `anta-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/PKG-INFO` & `anta-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.7.0
+Version: 0.7.1
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -226,7 +226,87 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
+
+[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/main/LICENSE)
+[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
+![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+![coverage](https://raw.githubusercontent.com/arista-netdevops-community/anta/coverage-badge/latest-release-coverage.svg)
+
+# Arista Network Test Automation (ANTA) Framework
+
+ANTA is Python framework that automates tests for Arista devices.
+
+- ANTA provides a [set of tests](api/tests.md) to validate the state of your network
+- ANTA can be used to:
+    - Automate NRFU (Network Ready For Use) test on a preproduction network
+    - Automate tests on a live network (periodically or on demand)
+- ANTA can be used with:
+    - The [ANTA CLI](cli/overview.md)
+    - As a [Python library](advanced_usages/as-python-lib.md) in your own application
+
+![anta nrfu](imgs/anta-nrfu.svg)
+
+```bash
+# Install ANTA CLI
+$ pip install anta
+
+# Run ANTA CLI
+$ anta --help
+Usage: anta [OPTIONS] COMMAND [ARGS]...
+
+  Arista Network Test Automation (ANTA) CLI
+
+Options:
+  --version                       Show the version and exit.
+  --username TEXT                 Username to connect to EOS  [env var:
+                                  ANTA_USERNAME; required]
+  --password TEXT                 Password to connect to EOS  [env var:
+                                  ANTA_PASSWORD; required]
+  --timeout INTEGER               Global connection timeout  [env var:
+                                  ANTA_TIMEOUT; default: 5]
+  --insecure                      Disable SSH Host Key validation  [env var:
+                                  ANTA_INSECURE]
+  --enable                        Add enable mode towards the devices if
+                                  required to connect  [env var: ANTA_ENABLE]
+  --enable-password TEXT          Enable password if required to connect,
+                                  --enable MUST be set  [env var:
+                                  ANTA_ENABLE_PASSWORD]
+  -i, --inventory FILE            Path to the inventory YAML file  [env var:
+                                  ANTA_INVENTORY; required]
+  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
+                                  ANTA logging level  [env var:
+                                  ANTA_LOG_LEVEL; default: INFO]
+  --ignore-status                 Always exit with success  [env var:
+                                  ANTA_IGNORE_STATUS]
+  --ignore-error                  Only report failures and not errors  [env
+                                  var: ANTA_IGNORE_ERROR]
+  --help                          Show this message and exit.
+
+Commands:
+  debug  Debug commands for building ANTA
+  exec   Execute commands to inventory devices
+  get    Get data from/to ANTA
+  nrfu   Run NRFU against inventory devices
+```
+
+!!! info
+    `username`, `password`, `enable`, and `enable-password` values are the same for all devices
+
+
+## Documentation
+
+The documentation is published on [ANTA package website](https://www.anta.ninja)
+
+## Contribution guide
+
+Contributions are welcome. Please refer to the [contribution guide](https://www.anta.ninja/main/contribution/)
+
+## Credits
+
+Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.7.0/anta/__init__.py` & `anta-0.7.1/anta/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/__init__.py` & `anta-0.7.1/anta/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/debug/commands.py` & `anta-0.7.1/anta/cli/debug/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/exec/commands.py` & `anta-0.7.1/anta/cli/exec/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/exec/utils.py` & `anta-0.7.1/anta/cli/exec/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/get/commands.py` & `anta-0.7.1/anta/cli/get/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/get/utils.py` & `anta-0.7.1/anta/cli/get/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/nrfu/commands.py` & `anta-0.7.1/anta/cli/nrfu/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/nrfu/utils.py` & `anta-0.7.1/anta/cli/nrfu/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/cli/utils.py` & `anta-0.7.1/anta/cli/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/decorators.py` & `anta-0.7.1/anta/decorators.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/device.py` & `anta-0.7.1/anta/device.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/inventory/__init__.py` & `anta-0.7.1/anta/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/inventory/models.py` & `anta-0.7.1/anta/inventory/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/loader.py` & `anta-0.7.1/anta/loader.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/models.py` & `anta-0.7.1/anta/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/reporter/__init__.py` & `anta-0.7.1/anta/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/reporter/models.py` & `anta-0.7.1/anta/reporter/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/result_manager/__init__.py` & `anta-0.7.1/anta/result_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/result_manager/models.py` & `anta-0.7.1/anta/result_manager/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/runner.py` & `anta-0.7.1/anta/runner.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/aaa.py` & `anta-0.7.1/anta/tests/aaa.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/configuration.py` & `anta-0.7.1/anta/tests/configuration.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/connectivity.py` & `anta-0.7.1/anta/tests/connectivity.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/field_notices.py` & `anta-0.7.1/anta/tests/field_notices.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/hardware.py` & `anta-0.7.1/anta/tests/hardware.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/interfaces.py` & `anta-0.7.1/anta/tests/interfaces.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/logging.py` & `anta-0.7.1/anta/tests/logging.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/mlag.py` & `anta-0.7.1/anta/tests/mlag.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/multicast.py` & `anta-0.7.1/anta/tests/multicast.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/profiles.py` & `anta-0.7.1/anta/tests/profiles.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/routing/bgp.py` & `anta-0.7.1/anta/tests/routing/bgp.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/routing/generic.py` & `anta-0.7.1/anta/tests/routing/generic.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/routing/ospf.py` & `anta-0.7.1/anta/tests/routing/ospf.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/security.py` & `anta-0.7.1/anta/tests/security.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/snmp.py` & `anta-0.7.1/anta/tests/snmp.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/software.py` & `anta-0.7.1/anta/tests/software.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/stp.py` & `anta-0.7.1/anta/tests/stp.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/system.py` & `anta-0.7.1/anta/tests/system.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tests/vxlan.py` & `anta-0.7.1/anta/tests/vxlan.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tools/get_value.py` & `anta-0.7.1/anta/tools/get_value.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tools/misc.py` & `anta-0.7.1/anta/tools/misc.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta/tools/pydantic.py` & `anta-0.7.1/anta/tools/pydantic.py`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/anta.egg-info/PKG-INFO` & `anta-0.7.1/anta.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.7.0
+Version: 0.7.1
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -226,7 +226,87 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
+
+[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/main/LICENSE)
+[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
+![PyPI - Downloads/month](https://img.shields.io/pypi/dm/eos-downloader)
+![coverage](https://raw.githubusercontent.com/arista-netdevops-community/anta/coverage-badge/latest-release-coverage.svg)
+
+# Arista Network Test Automation (ANTA) Framework
+
+ANTA is Python framework that automates tests for Arista devices.
+
+- ANTA provides a [set of tests](api/tests.md) to validate the state of your network
+- ANTA can be used to:
+    - Automate NRFU (Network Ready For Use) test on a preproduction network
+    - Automate tests on a live network (periodically or on demand)
+- ANTA can be used with:
+    - The [ANTA CLI](cli/overview.md)
+    - As a [Python library](advanced_usages/as-python-lib.md) in your own application
+
+![anta nrfu](imgs/anta-nrfu.svg)
+
+```bash
+# Install ANTA CLI
+$ pip install anta
+
+# Run ANTA CLI
+$ anta --help
+Usage: anta [OPTIONS] COMMAND [ARGS]...
+
+  Arista Network Test Automation (ANTA) CLI
+
+Options:
+  --version                       Show the version and exit.
+  --username TEXT                 Username to connect to EOS  [env var:
+                                  ANTA_USERNAME; required]
+  --password TEXT                 Password to connect to EOS  [env var:
+                                  ANTA_PASSWORD; required]
+  --timeout INTEGER               Global connection timeout  [env var:
+                                  ANTA_TIMEOUT; default: 5]
+  --insecure                      Disable SSH Host Key validation  [env var:
+                                  ANTA_INSECURE]
+  --enable                        Add enable mode towards the devices if
+                                  required to connect  [env var: ANTA_ENABLE]
+  --enable-password TEXT          Enable password if required to connect,
+                                  --enable MUST be set  [env var:
+                                  ANTA_ENABLE_PASSWORD]
+  -i, --inventory FILE            Path to the inventory YAML file  [env var:
+                                  ANTA_INVENTORY; required]
+  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
+                                  ANTA logging level  [env var:
+                                  ANTA_LOG_LEVEL; default: INFO]
+  --ignore-status                 Always exit with success  [env var:
+                                  ANTA_IGNORE_STATUS]
+  --ignore-error                  Only report failures and not errors  [env
+                                  var: ANTA_IGNORE_ERROR]
+  --help                          Show this message and exit.
+
+Commands:
+  debug  Debug commands for building ANTA
+  exec   Execute commands to inventory devices
+  get    Get data from/to ANTA
+  nrfu   Run NRFU against inventory devices
+```
+
+!!! info
+    `username`, `password`, `enable`, and `enable-password` values are the same for all devices
+
+
+## Documentation
+
+The documentation is published on [ANTA package website](https://www.anta.ninja)
+
+## Contribution guide
+
+Contributions are welcome. Please refer to the [contribution guide](https://www.anta.ninja/main/contribution/)
+
+## Credits
+
+Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.7.0/anta.egg-info/SOURCES.txt` & `anta-0.7.1/anta.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 anta/tests/routing/__init__.py
 anta/tests/routing/bgp.py
 anta/tests/routing/generic.py
 anta/tests/routing/ospf.py
 anta/tools/__init__.py
 anta/tools/get_value.py
 anta/tools/misc.py
-anta/tools/pydantic.py
+anta/tools/pydantic.py
+docs/README.md
```

### Comparing `anta-0.7.0/anta.egg-info/requires.txt` & `anta-0.7.1/anta.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `anta-0.7.0/pyproject.toml` & `anta-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # content of pyproject.toml
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anta"
-version = "v0.7.0"
-readme = "README.md"
+version = "v0.7.1"
+readme = "docs/README.md"
 authors = [{ name = "Khelil Sator", email = "ksator@arista.com" }]
 maintainers = [
   { name = "Khelil Sator", email = "ksator@arista.com" },
   { name = "Matthieu Tâche", email = "mtache@arista.com" },
   { name = "Khelil Sator", email = "ksator@arista.com" },
   { name = "Guillaume Mulocher", email = "gmulocher@arista.com" },
 ]
@@ -102,15 +102,15 @@
 include = ["anta*"]
 namespaces = false
 
 ################################
 # Version
 ################################
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump: Version {old_version} -> {new_version}"
 commit = true
 # No tag
 tag = false
 push = false
```

