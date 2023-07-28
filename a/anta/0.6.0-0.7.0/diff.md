# Comparing `tmp/anta-0.6.0.tar.gz` & `tmp/anta-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anta-0.6.0.tar", last modified: Fri Jul  7 10:29:38 2023, max compression
+gzip compressed data, was "anta-0.7.0.tar", last modified: Fri Jul 28 10:41:05 2023, max compression
```

## Comparing `anta-0.6.0.tar` & `anta-0.7.0.tar`

### file list

```diff
@@ -1,85 +1,77 @@
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.622272 anta-0.6.0/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    11345 2022-07-20 14:15:12.000000 anta-0.6.0/LICENSE
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       21 2023-03-31 08:52:22.000000 anta-0.6.0/MANIFEST.in
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    18259 2023-07-07 10:29:38.621614 anta-0.6.0/PKG-INFO
--rwxr-xr-x   0 guillaumemulocher   (501) staff       (20)     3789 2023-07-07 10:29:22.000000 anta-0.6.0/README.md
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.583246 anta-0.6.0/anta/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1102 2023-07-06 12:52:04.000000 anta-0.6.0/anta/__init__.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.586721 anta-0.6.0/anta/cli/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4082 2023-07-06 16:02:24.000000 anta-0.6.0/anta/cli/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      284 2023-07-07 09:53:40.000000 anta-0.6.0/anta/cli/console.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.587368 anta-0.6.0/anta/cli/debug/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-04-27 09:11:04.000000 anta-0.6.0/anta/cli/debug/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3571 2023-07-07 09:53:40.000000 anta-0.6.0/anta/cli/debug/commands.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.589091 anta-0.6.0/anta/cli/exec/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-02-14 08:55:44.000000 anta-0.6.0/anta/cli/exec/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3308 2023-07-04 13:25:37.000000 anta-0.6.0/anta/cli/exec/commands.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7155 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/exec/utils.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.590189 anta-0.6.0/anta/cli/get/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-03-31 09:09:54.000000 anta-0.6.0/anta/cli/get/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3708 2023-07-06 12:52:04.000000 anta-0.6.0/anta/cli/get/commands.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1748 2023-04-27 09:11:04.000000 anta-0.6.0/anta/cli/get/utils.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.591713 anta-0.6.0/anta/cli/nrfu/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-07-03 15:42:22.000000 anta-0.6.0/anta/cli/nrfu/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4799 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/nrfu/commands.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4573 2023-07-07 08:14:08.000000 anta-0.6.0/anta/cli/nrfu/utils.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4343 2023-07-06 16:02:24.000000 anta-0.6.0/anta/cli/utils.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3780 2023-07-07 08:14:08.000000 anta-0.6.0/anta/decorators.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    13884 2023-07-07 09:53:40.000000 anta-0.6.0/anta/device.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.593011 anta-0.6.0/anta/inventory/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7250 2023-07-07 08:14:08.000000 anta-0.6.0/anta/inventory/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      252 2023-07-03 15:42:22.000000 anta-0.6.0/anta/inventory/exceptions.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2368 2023-07-06 12:52:04.000000 anta-0.6.0/anta/inventory/models.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3249 2023-07-06 12:52:04.000000 anta-0.6.0/anta/loader.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    12824 2023-07-07 08:14:08.000000 anta-0.6.0/anta/models.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.594030 anta-0.6.0/anta/reporter/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    10362 2023-07-06 12:52:04.000000 anta-0.6.0/anta/reporter/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1305 2023-04-27 09:11:04.000000 anta-0.6.0/anta/reporter/models.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.594816 anta-0.6.0/anta/result_manager/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7677 2023-07-06 16:02:24.000000 anta-0.6.0/anta/result_manager/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4163 2023-07-06 12:52:04.000000 anta-0.6.0/anta/result_manager/models.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2894 2023-07-07 08:14:08.000000 anta-0.6.0/anta/runner.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.615466 anta-0.6.0/anta/tests/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tests/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    15959 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/aaa.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1498 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/configuration.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1629 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/connectivity.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     6469 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/field_notices.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8554 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/hardware.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    15459 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/interfaces.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    10182 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/logging.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     9689 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/mlag.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3228 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/multicast.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2341 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/profiles.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.617133 anta-0.6.0/anta/tests/routing/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-22 08:02:04.000000 anta-0.6.0/anta/tests/routing/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    11774 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/bgp.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4579 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/generic.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3640 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/routing/ospf.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    12534 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/security.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5452 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/snmp.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3646 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/software.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8447 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/stp.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7616 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/system.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2293 2023-07-06 16:02:24.000000 anta-0.6.0/anta/tests/vxlan.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.619181 anta-0.6.0/anta/tools/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2023-04-27 09:11:04.000000 anta-0.6.0/anta/tools/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1716 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/get_value.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      614 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/misc.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      795 2023-07-03 15:42:22.000000 anta-0.6.0/anta/tools/pydantic.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.585390 anta-0.6.0/anta.egg-info/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)    18259 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/PKG-INFO
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1514 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        1 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/entry_points.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      495 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/requires.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        5 2023-07-07 10:29:38.000000 anta-0.6.0/anta.egg-info/top_level.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5816 2023-07-07 10:29:22.000000 anta-0.6.0/pyproject.toml
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2023-07-07 10:29:38.622343 anta-0.6.0/setup.cfg
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.619891 anta-0.6.0/tests/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/__init__.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.620489 anta-0.6.0/tests/data/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/data/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7834 2023-07-03 15:42:22.000000 anta-0.6.0/tests/data/json_data.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-07 10:29:38.620997 anta-0.6.0/tests/units/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-07-20 14:15:12.000000 anta-0.6.0/tests/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.815518 anta-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-28 10:40:55.000000 anta-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 10:40:55.000000 anta-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-28 10:41:05.815518 anta-0.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-28 10:40:55.000000 anta-0.7.0/anta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/exec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/get/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/cli/nrfu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/nrfu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-28 10:40:55.000000 anta-0.7.0/anta/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-28 10:40:55.000000 anta-0.7.0/anta/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-28 10:40:55.000000 anta-0.7.0/anta/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-28 10:40:55.000000 anta-0.7.0/anta/inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-28 10:40:55.000000 anta-0.7.0/anta/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-07-28 10:40:55.000000 anta-0.7.0/anta/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-28 10:40:55.000000 anta-0.7.0/anta/reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-28 10:40:55.000000 anta-0.7.0/anta/reporter/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/result_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-07-28 10:40:55.000000 anta-0.7.0/anta/result_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-28 10:40:55.000000 anta-0.7.0/anta/result_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-28 10:40:55.000000 anta-0.7.0/anta/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/field_notices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/mlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/multicast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tests/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/routing/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tests/vxlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.811518 anta-0.7.0/anta/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/get_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-28 10:40:55.000000 anta-0.7.0/anta/tools/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:41:05.807518 anta-0.7.0/anta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 10:41:05.000000 anta-0.7.0/anta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-28 10:40:55.000000 anta-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:41:05.815518 anta-0.7.0/setup.cfg
```

### Comparing `anta-0.6.0/LICENSE` & `anta-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/PKG-INFO` & `anta-0.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.6.0
+Version: 0.7.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -204,15 +204,15 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://www.anta.ninja
 Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/anta/issues
-Project-URL: Contributing, https://github.com/arista-netdevops-community/anta/blob/master/CONTRIBUTING.md
+Project-URL: Contributing, https://www.anta.ninja/main/contribution/
 Keywords: test,anta,Arista,network,automation,networking,devops,netdevops
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -224,80 +224,9 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: doc
 License-File: LICENSE
-
-[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/master/LICENSE)
-[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
-[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
-
-# Arista Network Test Automation (ANTA) Framework
-
-__WARNING:__ Documentation is work in progress for version 0.6.0 available in Pypi.
-
-This repository is a Python package to automate tests on Arista devices.
-
-- The package name is ANTA, which stands for **Arista Network Test Automation**.
-- This package provides a set of tests to validate the state of your network.
-- This package can be imported in Python scripts:
-  - To automate NRFU (Network Ready For Use) test on a preproduction network
-  - To automate tests on a live network (periodically or on demand)
-
-This repository comes with a cli to run __Arista Network Test Automation__ (ANTA) framework using your preferred shell:
-
-```bash
-# Install ANTA CLI
-$ pip install anta
-
-# Run ANTA CLI
-$ anta
-Usage: anta [OPTIONS] COMMAND [ARGS]...
-
-  Arista Network Test Automation (ANTA) CLI
-
-Options:
-  --version                       Show the version and exit.
-  --username TEXT                 Username to connect to EOS  [env var:
-                                  ANTA_USERNAME; required]
-  --password TEXT                 Password to connect to EOS  [env var:
-                                  ANTA_PASSWORD; required]
-  --timeout INTEGER               Global connection timeout  [env var:
-                                  ANTA_TIMEOUT; default: 5]
-  --insecure                      Disable SSH Host Key validation  [env var:
-                                  ANTA_INSECURE]
-  --enable-password TEXT          Enable password if required to connect  [env
-                                  var: ANTA_ENABLE_PASSWORD]
-  -i, --inventory FILE            Path to the inventory YAML file  [env var:
-                                  ANTA_INVENTORY; required]
-  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
-                                  ANTA logging level  [env var:
-                                  ANTA_LOG_LEVEL; default: INFO]
-  --ignore-status                 Always exit with success  [env var:
-                                  ANTA_IGNORE_STATUS]
-  --ignore-error                  Only report failures and not errors  [env
-                                  var: ANTA_IGNORE_ERROR]
-  --help                          Show this message and exit.
-
-Commands:
-  debug  Debug commands for building ANTA
-  exec   Execute commands to inventory devices
-  get    Get data from/to ANTA
-  nrfu   Run NRFU against inventory devices
-```
-
-<img src="https://github.com/arista-netdevops-community/anta/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
-
-# Documentation
-
-The documentation is published on [ANTA package website](https://www.anta.ninja)
-
-# Contribution guide
-
-Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/anta/master/docs/contribution.md)
-
-# Credits
-
-Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.6.0/anta/__init__.py` & `anta-0.7.0/anta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-"""
-Arista Network Test Automation (ANTA) Framework
-"""
+"""Arista Network Test Automation (ANTA) Framework."""
 import importlib.metadata
 import os
 
-__version__ = importlib.metadata.version("anta")
+__version__ = f"v{importlib.metadata.version('anta')}"
 __credits__ = [
     "Angélique Phillipps",
     "Colin MacGiollaEáin",
     "Khelil Sator",
     "Matthieu Tâche",
     "Onur Gashi",
     "Paul Lavelle",
```

### Comparing `anta-0.6.0/anta/cli/__init__.py` & `anta-0.7.0/anta/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 import click
 
 from anta import __version__
 from anta.cli.debug import commands as debug_commands
 from anta.cli.exec import commands as exec_commands
 from anta.cli.get import commands as get_commands
 from anta.cli.nrfu import commands as check_commands
-from anta.cli.utils import parse_catalog, parse_inventory, setup_logging
+from anta.cli.utils import IgnoreRequiredWithHelp, parse_catalog, parse_inventory, requires_enable, setup_logging
 from anta.result_manager.models import TestResult
 
 
-@click.group()
+# @click.group()
+@click.group(cls=IgnoreRequiredWithHelp)
 @click.pass_context
 @click.version_option(__version__)
 @click.option(
     "--username",
     show_envvar=True,
     help="Username to connect to EOS",
     required=True,
@@ -46,17 +47,26 @@
     show_envvar=True,
     is_flag=True,
     default=False,
     help="Disable SSH Host Key validation",
     show_default=True,
 )
 @click.option(
+    "--enable",
+    show_envvar=True,
+    is_flag=True,
+    default=False,
+    help="Add enable mode towards the devices if required to connect",
+    show_default=True,
+)
+@click.option(
     "--enable-password",
     show_envvar=True,
-    help="Enable password if required to connect",
+    help="Enable password if required to connect, --enable MUST be set",
+    callback=requires_enable,
 )
 @click.option(
     "--inventory",
     "-i",
     show_envvar=True,
     required=True,
     help="Path to the inventory YAML file",
@@ -79,24 +89,24 @@
         ],
         case_sensitive=False,
     ),
     callback=setup_logging,
 )
 @click.option("--ignore-status", show_envvar=True, is_flag=True, default=False, help="Always exit with success")
 @click.option("--ignore-error", show_envvar=True, is_flag=True, default=False, help="Only report failures and not errors")
-def anta(ctx: click.Context, inventory: pathlib.Path, ignore_status: bool, ignore_error: bool, **kwargs: Dict[str, Any]) -> None:
+def anta(ctx: click.Context, inventory: pathlib.Path, ignore_status: bool, ignore_error: bool, **kwargs: Any) -> None:
     # pylint: disable=unused-argument
     """Arista Network Test Automation (ANTA) CLI"""
     ctx.ensure_object(dict)
     ctx.obj["inventory"] = parse_inventory(ctx, inventory)
     ctx.obj["ignore_status"] = ignore_status
     ctx.obj["ignore_error"] = ignore_error
 
 
-@anta.group()
+@anta.group(cls=IgnoreRequiredWithHelp)
 @click.pass_context
 @click.option(
     "--catalog",
     "-c",
     show_envvar=True,
     help="Path to the tests catalog YAML file",
     type=click.Path(file_okay=True, dir_okay=False, exists=True, readable=True),
@@ -110,41 +120,46 @@
 
 @anta.group("exec")
 def _exec() -> None:
     """Execute commands to inventory devices"""
 
 
 @anta.group("get")
-def get() -> None:
+def _get() -> None:
     """Get data from/to ANTA"""
 
 
 @anta.group("debug")
-def debug() -> None:
+def _debug() -> None:
     """Debug commands for building ANTA"""
 
 
+# Load group commands
+# Prefixing with `_` for avoiding the confusion when importing anta.cli.debug.commands as otherwise the debug group has
+# a commands attribute.
+_exec.add_command(exec_commands.clear_counters)
+_exec.add_command(exec_commands.snapshot)
+_exec.add_command(exec_commands.collect_tech_support)
+
+
+_get.add_command(get_commands.from_cvp)
+_get.add_command(get_commands.from_ansible)
+_get.add_command(get_commands.inventory)
+_get.add_command(get_commands.tags)
+
+_debug.add_command(debug_commands.run_cmd)
+_debug.add_command(debug_commands.run_template)
+
+nrfu.add_command(check_commands.table)
+nrfu.add_command(check_commands.json)
+nrfu.add_command(check_commands.text)
+nrfu.add_command(check_commands.tpl_report)
+
+
 # ANTA CLI Execution
 def cli() -> None:
-    """Load ANTA CLI"""
-    # Load group commands
-    _exec.add_command(exec_commands.clear_counters)
-    _exec.add_command(exec_commands.snapshot)
-    _exec.add_command(exec_commands.collect_tech_support)
-
-    get.add_command(get_commands.from_cvp)
-    get.add_command(get_commands.inventory)
-    get.add_command(get_commands.tags)
-
-    debug.add_command(debug_commands.run_cmd)
-    debug.add_command(debug_commands.run_template)
-
-    nrfu.add_command(check_commands.table)
-    nrfu.add_command(check_commands.json)
-    nrfu.add_command(check_commands.text)
-    nrfu.add_command(check_commands.tpl_report)
-    # Load CLI
-    anta(obj={}, auto_envvar_prefix="ANTA")
+    """Entrypoint for pyproject.toml"""
+    anta(obj={}, auto_envvar_prefix="ANTA")  # pragma: no cover
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `anta-0.6.0/anta/cli/debug/commands.py` & `anta-0.7.0/anta/cli/debug/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 
 import click
 from click import Option
 
 from anta.cli.console import console
 from anta.device import AntaDevice
 from anta.models import AntaCommand, AntaTemplate
+from anta.tools.misc import anta_log_exception
 
 logger = logging.getLogger(__name__)
 
 
+# pylint: disable-next=inconsistent-return-statements
 def get_device(ctx: click.Context, param: Option, value: str) -> List[str]:
-    # pylint: disable=unused-argument
     """
     Click option callback to get an AntaDevice instance from a string
     """
-    if value is not None:
+    # pylint: disable=unused-argument
+    try:
         return ctx.obj["inventory"][value]
-    return None
+    except KeyError as e:
+        message = f"Device {value} does not exist in Inventory"
+        anta_log_exception(e, message, logger)
+        ctx.fail(message)
 
 
 @click.command()
 @click.option("--command", "-c", type=str, required=True, help="Command to run")
 @click.option("--ofmt", type=click.Choice(["json", "text"]), default="json", help="EOS eAPI format to use. can be text or json")
 @click.option("--version", "-v", type=click.Choice(["1", "latest"]), default="latest", help="EOS eAPI version")
 @click.option("--revision", "-r", type=int, help="eAPI command revision", required=False)
```

### Comparing `anta-0.6.0/anta/cli/exec/commands.py` & `anta-0.7.0/anta/cli/exec/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,19 +25,14 @@
 @click.pass_context
 @click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
 def clear_counters(ctx: click.Context, tags: Optional[List[str]]) -> None:
     """Clear counter statistics on EOS devices"""
     asyncio.run(clear_counters_utils(ctx.obj["inventory"], tags=tags))
 
 
-def _get_snapshot_dir(ctx: click.Context, param: click.Parameter, value: str) -> Path:  # pylint: disable=unused-argument
-    """Build directory name for command snapshots, including current time"""
-    return Path(f"{value}_{datetime.now().strftime('%Y-%m-%d_%H_%M_%S')}")
-
-
 @click.command()
 @click.pass_context
 @click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
 @click.option(
     "--commands-list",
     "-c",
     help="File with list of commands to collect",
@@ -45,22 +40,23 @@
     show_envvar=True,
     type=click.Path(file_okay=True, dir_okay=False, exists=True, readable=True, path_type=Path),
 )
 @click.option(
     "--output",
     "-o",
     show_envvar=True,
-    type=click.Path(file_okay=False, dir_okay=True, exists=False, writable=True),
-    help="Directory to save commands output. Will have a suffix with the format _YEAR-MONTH-DAY_HOUR-MINUTES-SECONDS'",
-    default="anta_snapshot",
+    type=click.Path(file_okay=False, dir_okay=True, exists=False, writable=True, path_type=Path),
+    help="Directory to save commands output.",
+    default=f"anta_snapshot_{datetime.now().strftime('%Y-%m-%d_%H_%M_%S')}",
     show_default=True,
-    callback=_get_snapshot_dir,
 )
 def snapshot(ctx: click.Context, tags: Optional[List[str]], commands_list: Path, output: Path) -> None:
     """Collect commands output from devices in inventory"""
+    print(f"Collecting data for {commands_list}")
+    print(f"Output directory is {output}")
     try:
         with open(commands_list, "r", encoding="UTF-8") as file:
             file_content = file.read()
             eos_commands = safe_load(file_content)
     except FileNotFoundError:
         logger.error(f"Error reading {commands_list}")
         sys.exit(1)
@@ -68,13 +64,17 @@
 
 
 @click.command()
 @click.pass_context
 @click.option("--output", "-o", default="./tech-support", show_default=True, help="Path for tests catalog", type=click.Path(path_type=Path), required=False)
 @click.option("--latest", help="Number of scheduled show-tech to retrieve", type=int, required=False)
 @click.option(
-    "--configure/--not-configure", help="Ensure device has 'aaa authorization exec default local' configured (required for SCP)", default=False, show_default=True
+    "--configure",
+    help="Ensure devices have 'aaa authorization exec default local' configured (required for SCP on EOS). THIS WILL CHANGE THE CONFIGURATION OF YOUR NETWORK.",
+    default=False,
+    is_flag=True,
+    show_default=True,
 )
 @click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
 def collect_tech_support(ctx: click.Context, tags: Optional[List[str]], output: Path, latest: Optional[int], configure: bool) -> None:
     """Collect scheduled tech-support from EOS devices"""
     asyncio.run(collect_scheduled_show_tech(ctx.obj["inventory"], output, configure, tags=tags, latest=latest))
```

### Comparing `anta-0.6.0/anta/cli/exec/utils.py` & `anta-0.7.0/anta/cli/exec/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 import json
 import logging
 from pathlib import Path
 from typing import Dict, List, Literal, Optional
 
 from aioeapi import EapiCommandError
 
-from anta import __DEBUG__
-from anta.device import AntaDevice
+from anta.device import AntaDevice, AsyncEOSDevice
 from anta.inventory import AntaInventory
 from anta.models import AntaCommand
-from anta.tools.misc import exc_to_str
+from anta.tools.misc import anta_log_exception, exc_to_str
 
 EOS_SCHEDULED_TECH_SUPPORT = "/mnt/flash/schedule/tech-support"
 
 logger = logging.getLogger(__name__)
 
 
 async def clear_counters_utils(anta_inventory: AntaInventory, tags: Optional[List[str]] = None) -> None:
@@ -75,24 +74,24 @@
             f.write(content)
         logger.info(f"Collected command '{command}' from device {dev.name} ({dev.hw_model})")
 
     logger.info("Connecting to devices...")
     await inv.connect_inventory()
     devices = inv.get_inventory(established_only=True, tags=tags).values()
     logger.info("Collecting commands from remote devices")
-    coros = [collect(device, command, "json") for device, command in itertools.product(devices, commands["json_format"])]
-    coros += [collect(device, command, "text") for device, command in itertools.product(devices, commands["text_format"])]
+    coros = []
+    if "json_format" in commands:
+        coros += [collect(device, command, "json") for device, command in itertools.product(devices, commands["json_format"])]
+    if "text_format" in commands:
+        coros += [collect(device, command, "text") for device, command in itertools.product(devices, commands["text_format"])]
     res = await asyncio.gather(*coros, return_exceptions=True)
     for r in res:
         if isinstance(r, Exception):
             message = "Error when collecting commands"
-            if __DEBUG__:
-                logger.exception(message, exc_info=r)
-            else:
-                logger.error(f"{message}: {exc_to_str(r)}")
+            anta_log_exception(r, message, logger)
 
 
 async def collect_scheduled_show_tech(inv: AntaInventory, root_dir: Path, configure: bool, tags: Optional[List[str]] = None, latest: Optional[int] = None) -> None:
     """
     Collect scheduled show-tech on devices
     """
 
@@ -120,22 +119,30 @@
             # Check if 'aaa authorization exec default local' is present in the running-config
             command = AntaCommand(command="show running-config | include aaa authorization exec default local", ofmt="text")
             await device.collect(command=command)
 
             if command.collected and not command.text_output:
                 logger.debug(f"'aaa authorization exec default local' is not configured on device {device.name}")
                 if configure:
+                    # Otherwise mypy complains about enable
+                    assert isinstance(device, AsyncEOSDevice)
                     # TODO - @mtache - add `config` field to `AntaCommand` object to handle this use case.
-                    commands = [
-                        {"cmd": "enable", "input": device._enable_password},  # type: ignore[attr-defined] # pylint: disable=protected-access
-                        "configure terminal",
-                        "aaa authorization exec default local",
-                    ]
+                    commands = []
+                    if device.enable and device._enable_password is not None:  # type: ignore[attr-defined] # pylint: disable=protected-access
+                        commands.append({"cmd": "enable", "input": device._enable_password})  # type: ignore[attr-defined] # pylint: disable=protected-access
+                    elif device.enable:
+                        commands.append({"cmd": "enable"})
+                    commands.extend(
+                        [
+                            {"cmd": "configure terminal"},
+                            {"cmd": "aaa authorization exec default local"},
+                        ]
+                    )
+                    logger.warning(f"Configuring 'aaa authorization exec default local' on device {device.name}")
                     command = AntaCommand(command="show running-config | include aaa authorization exec default local", ofmt="text")
-                    logger.debug(f"Configuring 'aaa authorization exec default local' on device {device.name}")
                     await device.session.cli(commands=commands)  # type: ignore[attr-defined]
                     logger.info(f"Configured 'aaa authorization exec default local' on device {device.name}")
                 else:
                     logger.error(f"Unable to collect tech-support on {device.name}: configuration 'aaa authorization exec default local' is not present")
                     return
             logger.debug(f"'aaa authorization exec default local' is already configured on device {device.name}")
 
@@ -143,16 +150,13 @@
             logger.info(f"Collected {len(filenames)} scheduled tech-support from {device.name}")
 
         except EapiCommandError as e:
             logger.error(f"Unable to collect tech-support on {device.name}: {e.errmsg}")
         # In this case we want to catch all exceptions
         except Exception as e:  # pylint: disable=broad-except
             message = f"Unable to collect tech-support on device {device.name}"
-            if __DEBUG__:
-                logger.exception(message)
-            else:
-                logger.error(f"{message}: {exc_to_str(e)}")
+            anta_log_exception(e, message, logger)
 
     logger.info("Connecting to devices...")
     await inv.connect_inventory()
     devices = inv.get_inventory(established_only=True, tags=tags).values()
     await asyncio.gather(*(collect(device) for device in devices))
```

### Comparing `anta-0.6.0/anta/cli/nrfu/commands.py` & `anta-0.7.0/anta/cli/nrfu/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,28 @@
 from .utils import anta_progress_bar, print_jinja, print_json, print_settings, print_table, print_text
 
 logger = logging.getLogger(__name__)
 
 
 @click.command()
 @click.pass_context
-@click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
+@click.option("--tags", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
 @click.option("--device", "-d", help="Show a summary for this device", type=str, required=False)
 @click.option("--test", "-t", help="Show a summary for this test", type=str, required=False)
-def table(ctx: click.Context, tags: Optional[List[str]], device: Optional[str], test: Optional[str]) -> None:
+@click.option(
+    "--group-by", default=None, type=click.Choice(["device", "test"], case_sensitive=False), help="Group result by test or host. default none", required=False
+)
+def table(ctx: click.Context, tags: Optional[List[str]], device: Optional[str], test: Optional[str], group_by: str) -> None:
     """ANTA command to check network states with table result"""
     print_settings(ctx)
     results = ResultManager()
     with anta_progress_bar() as AntaTest.progress:
         asyncio.run(main(results, ctx.obj["inventory"], ctx.obj["catalog"], tags=tags))
-    print_table(results=results, device=device, test=test)
+
+    print_table(results=results, device=device, group_by=group_by, test=test)
 
     # TODO make a util method to avoid repeating the same three line
     ignore_status = ctx.obj["ignore_status"]
     ignore_error = ctx.obj["ignore_error"]
     sys.exit(return_code(results, ignore_error, ignore_status))
 
 
@@ -65,15 +69,15 @@
     sys.exit(return_code(results, ignore_error, ignore_status))
 
 
 @click.command()
 @click.pass_context
 @click.option("--tags", "-t", help="List of tags using comma as separator: tag1,tag2,tag3", type=str, required=False, callback=parse_tags)
 @click.option("--search", "-s", help="Regular expression to search in both name and test", type=str, required=False)
-@click.option("--skip-error/--no-skip-error", help="Hide tests in errors due to connectivity issue", default=False, show_default=True, required=False)
+@click.option("--skip-error", help="Hide tests in errors due to connectivity issue", default=False, is_flag=True, show_default=True, required=False)
 def text(ctx: click.Context, tags: Optional[List[str]], search: Optional[str], skip_error: bool) -> None:
     """ANTA command to check network states with text result"""
     print_settings(ctx)
     results = ResultManager()
     with anta_progress_bar() as AntaTest.progress:
         asyncio.run(main(results, ctx.obj["inventory"], ctx.obj["catalog"], tags=tags))
     print_text(results=results, search=search, skip_error=skip_error)
```

### Comparing `anta-0.6.0/anta/cli/nrfu/utils.py` & `anta-0.7.0/anta/cli/nrfu/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,56 +28,66 @@
     """Print ANTA settings before running tests"""
     message = f"Running ANTA tests:\n- {context.obj['inventory']}\n- Tests catalog contains {len(context.obj['catalog'])} tests"
     if report_template:
         message += f"\n- Report template: {report_template}"
     if report_output:
         message += f"\n- Report output: {report_output}"
     console.print(Panel.fit(message, style="cyan", title="[green]Settings"))
+    console.print()
 
 
-def print_table(results: ResultManager, device: Optional[str] = None, test: Optional[str] = None) -> None:
+def print_table(results: ResultManager, device: Optional[str] = None, test: Optional[str] = None, group_by: Optional[str] = None) -> None:
     """Print result in a table"""
     reporter = ReportTable()
+    console.print()
     if device:
-        console.print(reporter.report_summary_hosts(result_manager=results, host=device))
-    if test:
-        console.print(reporter.report_summary_tests(result_manager=results, testcase=test))
-    if device is None and test is None:
+        console.print(reporter.report_all(result_manager=results, host=device))
+    elif test:
+        console.print(reporter.report_all(result_manager=results, testcase=test))
+    elif group_by == "device":
+        console.print(reporter.report_summary_hosts(result_manager=results, host=None))
+    elif group_by == "test":
+        console.print(reporter.report_summary_tests(result_manager=results, testcase=None))
+    else:
         console.print(reporter.report_all(result_manager=results))
 
 
 def print_json(results: ResultManager, output: Optional[pathlib.Path] = None) -> None:
     """Print result in a json format"""
+    console.print()
     console.print(Panel("JSON results of all tests", style="cyan"))
     rich.print_json(results.get_results(output_format="json"))
     if output is not None:
         with open(output, "w", encoding="utf-8") as fout:
             fout.write(results.get_results(output_format="json"))
 
 
 def print_list(results: ResultManager, output: Optional[pathlib.Path] = None) -> None:
     """Print result in a list"""
+    console.print()
     console.print(Panel.fit("List results of all tests", style="cyan"))
     pprint(results.get_results(output_format="list"))
     if output is not None:
         with open(output, "w", encoding="utf-8") as fout:
             fout.write(str(results.get_results(output_format="list")))
 
 
 def print_text(results: ResultManager, search: Optional[str] = None, skip_error: bool = False) -> None:
     """Print results as simple text"""
+    console.print()
     regexp = re.compile(search if search else ".*")
     for line in results.get_results(output_format="list"):
         if any(regexp.match(entry) for entry in [line.name, line.test]) and (not skip_error or line.result != "error"):
             message = f" ({str(line.messages[0])})" if len(line.messages) > 0 else ""
             console.print(f"{line.name} :: {line.test} :: [{line.result}]{line.result.upper()}[/{line.result}]{message}", highlight=False)
 
 
 def print_jinja(results: ResultManager, template: pathlib.Path, output: Optional[pathlib.Path] = None) -> None:
     """Print result based on template."""
+    console.print()
     reporter = ReportJinja(template_path=template)
     json_data = json.loads(results.get_results(output_format="json"))
     report = reporter.render(json_data)
     console.print(report)
     if output is not None:
         with open(output, "w", encoding="utf-8") as file:
             file.write(report)
```

### Comparing `anta-0.6.0/anta/decorators.py` & `anta-0.7.0/anta/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-"""
-decorators for tests
-"""
+"""decorators for tests."""
+from __future__ import annotations
+
 from functools import wraps
-from typing import Any, Callable, Dict, List, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 
 from anta.models import AntaCommand, AntaTest
-from anta.result_manager.models import TestResult
 from anta.tools.misc import exc_to_str
 
+if TYPE_CHECKING:
+    from anta.result_manager.models import TestResult
+
 # TODO - should probably use mypy Awaitable in some places rather than this everywhere - @gmuloc
 F = TypeVar("F", bound=Callable[..., Any])
 
 
-def skip_on_platforms(platforms: List[str]) -> Callable[[F], F]:
-    """
-    Decorator factory to skip a test on a list of platforms
+def skip_on_platforms(platforms: list[str]) -> Callable[[F], F]:
+    """Return a decorator factory to skip a test on a list of platforms.
 
     Args:
-    * platforms (List[str]): the list of platforms on which the decorated test should be skipped.
+    ----
+      platforms (List[str]): the list of platforms on which the decorated test should be skipped.
 
     """
 
     def decorator(function: F) -> F:
-        """
-        Decorator to skip a test ona list of platform
-        * func (Callable): the test to be decorated
+        """Implement the decorator to skip a test ona list of platform.
+
+        Args:
+        ----
+            function (F): the test to be decorated.
         """
 
         @wraps(function)
-        async def wrapper(*args: Any, **kwargs: Dict[str, Any]) -> TestResult:
-            """
-            wrapper for func
-            """
+        async def wrapper(*args: Any, **kwargs: Any) -> TestResult:
+            """Implement the wrapper for func."""
             anta_test = args[0]
 
             if anta_test.result.result != "unset":
                 AntaTest.update_progress()
                 return anta_test.result
 
             if anta_test.device.hw_model in platforms:
@@ -47,33 +49,33 @@
 
         return cast(F, wrapper)
 
     return decorator
 
 
 def check_bgp_family_enable(family: str) -> Callable[[F], F]:
-    """
-    Decorator factory to skip a test if BGP is enabled
+    """Return a decorator factory to skip a test if BGP is enabled.
 
     Args:
-    * family (str): BGP family to check. Can be ipv4 / ipv6 / evpn / rtc
+    ----
+        family (str): BGP family to check. Can be ipv4 / ipv6 / evpn / rtc
 
     """
 
     def decorator(function: F) -> F:
-        """
-        Decorator to skip a test if an address family is not configured
-        * func (Callable): the test to be decorated
+        """Implement the decorator to skip a test if an address family is not configured.
+
+        Args:
+        ----
+            function (F): the test to be decorated.
         """
 
         @wraps(function)
-        async def wrapper(*args: Any, **kwargs: Dict[str, Any]) -> TestResult:
-            """
-            wrapper for func
-            """
+        async def wrapper(*args: Any, **kwargs: Any) -> TestResult:
+            """Implement the wrapper for func."""
             anta_test = args[0]
 
             if anta_test.result.result != "unset":
                 AntaTest.update_progress()
                 return anta_test.result
 
             if family == "ipv4":
```

### Comparing `anta-0.6.0/anta/device.py` & `anta-0.7.0/anta/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,61 +10,26 @@
 import asyncssh
 from aioeapi import Device, EapiCommandError
 from asyncssh import SSHClientConnection, SSHClientConnectionOptions
 from httpx import ConnectError, HTTPError
 
 from anta import __DEBUG__
 from anta.models import DEFAULT_TAG, AntaCommand
-from anta.tools.misc import exc_to_str
+from anta.tools.misc import anta_log_exception, exc_to_str
 
 logger = logging.getLogger(__name__)
 
 
-# For Python < 3.10, it is not possible to install a version of aio-eapi newer than 0.3.0
-# which sadly hardcodes version to 1 in its call to eAPI
-# This little piece of nasty hack patches the aio-eapi function to support using a different
-# version of the eAPI.
-# Hic Sunt Draconis.
-# Are we proud of this? No.
-# Waiting for: https://github.com/jeremyschulman/aio-eapi/issues/9
-def patched_jsoncrpc_command(self: Device, commands: List[str], ofmt: str, **kwargs: Dict[Any, Any]) -> Dict[str, Any]:
-    """
-    Used to create the JSON-RPC command dictionary object
-    """
-    version = kwargs.get("version", "latest")
-
-    cmd = {
-        "jsonrpc": "2.0",
-        "method": "runCmds",
-        "params": {
-            "version": version,
-            "cmds": commands,
-            "format": ofmt or self.EAPI_DEFAULT_OFMT,
-        },
-        "id": str(kwargs.get("req_id") or id(self)),
-    }
-    if "autoComplete" in kwargs:
-        cmd["params"]["autoComplete"] = kwargs["autoComplete"]  # type: ignore
-
-    if "expandAliases" in kwargs:
-        cmd["params"]["expandAliases"] = kwargs["expandAliases"]  # type: ignore
-
-    return cmd
-
-
-Device.jsoncrpc_command = patched_jsoncrpc_command
-
-
 class AntaDevice(ABC):
     """
     Abstract class representing a device in ANTA.
     An implementation of this class needs must override the abstract coroutines `collect()` and
     `refresh()`.
 
-    Instance attributes:
+    Attributes:
         name: Device name
         is_online: True if the device IP is reachable and a port can be open
         established: True if remote command execution succeeds
         hw_model: Hardware model of the device
         tags: List of tags for this device
     """
 
@@ -132,17 +97,17 @@
 
     @abstractmethod
     async def refresh(self) -> None:
         """
         Update attributes of an AntaDevice instance.
 
         This coroutine must update the following attributes of AntaDevice:
-        - is_online: When the device IP is reachable and a port can be open
-        - established: When a command execution succeeds
-        - hw_model: The hardware model of the device
+            - `is_online`: When the device IP is reachable and a port can be open
+            - `established`: When a command execution succeeds
+            - `hw_model`: The hardware model of the device
         """
 
     async def copy(self, sources: List[Path], destination: Path, direction: Literal["to", "from"] = "from") -> None:
         """
         Copy files to and from the device, usually through SCP.
         It is not mandatory to implement this for a valid AntaDevice subclass.
 
@@ -154,28 +119,29 @@
         raise NotImplementedError(f"copy() method has not been implemented in {self.__class__.__name__} definition")
 
 
 class AsyncEOSDevice(AntaDevice):
     """
     Implementation of AntaDevice for EOS using aio-eapi.
 
-    Instance attributes:
+    Attributes:
         name: Device name
         is_online: True if the device IP is reachable and a port can be open
         established: True if remote command execution succeeds
         hw_model: Hardware model of the device
         tags: List of tags for this device
     """
 
     def __init__(  # pylint: disable=R0913
         self,
         host: str,
         username: str,
         password: str,
         name: Optional[str] = None,
+        enable: bool = False,
         enable_password: Optional[str] = None,
         port: Optional[int] = None,
         ssh_port: Optional[int] = 22,
         tags: Optional[List[str]] = None,
         timeout: Optional[float] = None,
         insecure: bool = False,
         proto: Literal["http", "https"] = "https",
@@ -184,25 +150,27 @@
         Constructor of AsyncEOSDevice
 
         Args:
             host: Device FQDN or IP
             username: Username to connect to eAPI and SSH
             password: Password to connect to eAPI and SSH
             name: Device name
+            enable: Device needs privileged access
             enable_password: Password used to gain privileged access on EOS
-            proto: eAPI protocol. Value can be 'http' or 'https'
             port: eAPI port. Defaults to 80 is proto is 'http' or 443 if proto is 'https'.
             ssh_port: SSH port
-            insecure: Disable SSH Host Key validation
             tags: List of tags for this device
             timeout: Timeout value in seconds for outgoing connections. Default to 10 secs.
+            insecure: Disable SSH Host Key validation
+            proto: eAPI protocol. Value can be 'http' or 'https'
         """
         if name is None:
-            name = f"{host}:{port}"
+            name = f"{host}{f':{port}' if port else ''}"
         super().__init__(name, tags)
+        self.enable = enable
         self._enable_password = enable_password
         self._session: Device = Device(host=host, port=port, username=username, password=password, proto=proto, timeout=timeout)
         ssh_params: Dict[str, Any] = {}
         if insecure:
             ssh_params.update({"known_hosts": None})
         self._ssh_opts: SSHClientConnectionOptions = SSHClientConnectionOptions(host=host, port=ssh_port, username=username, password=password, **ssh_params)
 
@@ -212,14 +180,15 @@
         https://rich.readthedocs.io/en/stable/pretty.html#rich-repr-protocol
         """
         yield from super().__rich_repr__()
         yield "host", self._session.host
         yield "eapi_port", self._session.port
         yield "username", self._ssh_opts.username
         yield "password", self._ssh_opts.password
+        yield "enable", self.enable
         yield "enable_password", self._enable_password
         yield "insecure", self._ssh_opts.known_hosts is None
         if __DEBUG__:
             yield "_session", vars(self._session)
             yield "_ssh_opts", vars(self._ssh_opts)
 
     def __eq__(self, other: object) -> bool:
@@ -240,52 +209,52 @@
         of the `AntaDevice` instance if populated.
 
         Args:
             command: the command to collect
         """
         try:
             commands = []
-            if self._enable_password is not None:
+            if self.enable and self._enable_password is not None:
                 commands.append(
                     {
                         "cmd": "enable",
                         "input": str(self._enable_password),
                     }
                 )
-            else:
+            elif self.enable:
+                # No password
                 commands.append({"cmd": "enable"})
             if command.revision:
                 commands.append({"cmd": command.command, "revision": command.revision})
             else:
                 commands.append({"cmd": command.command})
             response = await self._session.cli(
                 commands=commands,
                 ofmt=command.ofmt,
                 version=command.version,
             )
             # remove first dict related to enable command
             # only applicable to json output
             if command.ofmt in ["json", "text"]:
                 # selecting only our command output
-                response = response[1]
+                response = response[-1]
             command.output = response
             logger.debug(f"{self.name}: {command}")
 
         except EapiCommandError as e:
-            logger.error(f"Command '{command.command}' failed on {self.name}: {e.errmsg}")
+            message = f"Command '{command.command}' failed on {self.name}"
+            anta_log_exception(e, message, logger)
             command.failed = e
         except (HTTPError, ConnectError) as e:
-            logger.error(f"Cannot connect to device {self.name}: {exc_to_str(e)}")
+            message = f"Cannot connect to device {self.name}"
+            anta_log_exception(e, message, logger)
             command.failed = e
         except Exception as e:  # pylint: disable=broad-exception-caught
             message = f"Exception raised while collecting command '{command.command}' on device {self.name}"
-            if __DEBUG__:
-                logger.exception(message)
-            else:
-                logger.error(message + f": {exc_to_str(e)}")
+            anta_log_exception(e, message, logger)
             command.failed = e
             logger.debug(command)
 
     async def refresh(self) -> None:
         """
         Update attributes of an AsyncEOSDevice instance.
```

### Comparing `anta-0.6.0/anta/inventory/__init__.py` & `anta-0.7.0/anta/inventory/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 Inventory Module for ANTA.
 """
 
 from __future__ import annotations
 
 import asyncio
 import logging
+from ipaddress import ip_address, ip_network
 from typing import Any, Dict, List, Optional
 
-from netaddr import IPAddress, IPNetwork
 from pydantic import ValidationError
 from yaml import safe_load
 
-from anta import __DEBUG__
 from anta.device import AntaDevice, AsyncEOSDevice
 from anta.inventory.exceptions import InventoryIncorrectSchema, InventoryRootKeyError
 from anta.inventory.models import AntaInventoryInput
-from anta.tools.misc import exc_to_str
+from anta.tools.misc import anta_log_exception
 
 logger = logging.getLogger(__name__)
 
 
 class AntaInventory(dict):  # type: ignore
     # dict[str, AntaDevice] - not working in python 3.8 hence the ignore
     """
@@ -39,36 +38,125 @@
             if (dev_type := dev.__class__.__name__) not in devs:
                 devs[dev_type] = 1
             else:
                 devs[dev_type] += 1
         return f"ANTA Inventory contains {' '.join([f'{n} devices ({t})' for t, n in devs.items()])}"
 
     @staticmethod
+    def _parse_hosts(inventory_input: AntaInventoryInput, inventory: AntaInventory, **kwargs: Any) -> None:
+        """
+        Parses the host section of an AntaInventoryInput and add the devices to the inventory
+
+        Args:
+            inventory_input (AntaInventoryInput): AntaInventoryInput used to parse the devices
+            inventory (AntaInventory): AntaInventory to add the parsed devices to
+        """
+        if inventory_input.hosts is None:
+            return
+
+        for host in inventory_input.hosts:
+            device = AsyncEOSDevice(name=host.name, host=str(host.host), port=host.port, tags=host.tags, **kwargs)
+            inventory.add_device(device)
+
+    @staticmethod
+    def _parse_networks(inventory_input: AntaInventoryInput, inventory: AntaInventory, **kwargs: Any) -> None:
+        """
+        Parses the network section of an AntaInventoryInput and add the devices to the inventory.
+
+        Args:
+            inventory_input (AntaInventoryInput): AntaInventoryInput used to parse the devices
+            inventory (AntaInventory): AntaInventory to add the parsed devices to
+
+        Raises:
+            InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
+        """
+        if inventory_input.networks is None:
+            return
+
+        for network in inventory_input.networks:
+            try:
+                for host_ip in ip_network(str(network.network)):
+                    device = AsyncEOSDevice(host=str(host_ip), tags=network.tags, **kwargs)
+                    inventory.add_device(device)
+            except ValueError as e:
+                message = "Could not parse network {network.network} in the inventory"
+                anta_log_exception(e, message, logger)
+                raise InventoryIncorrectSchema(message) from e
+
+    @staticmethod
+    def _parse_ranges(inventory_input: AntaInventoryInput, inventory: AntaInventory, **kwargs: Any) -> None:
+        """
+        Parses the range section of an AntaInventoryInput and add the devices to the inventory.
+
+        Args:
+            inventory_input (AntaInventoryInput): AntaInventoryInput used to parse the devices
+            inventory (AntaInventory): AntaInventory to add the parsed devices to
+
+        Raises:
+            InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
+        """
+        if inventory_input.ranges is None:
+            return
+
+        for range_def in inventory_input.ranges:
+            try:
+                range_increment = ip_address(str(range_def.start))
+                range_stop = ip_address(str(range_def.end))
+                while range_increment <= range_stop:  # type: ignore[operator]
+                    # mypy raise an issue about comparing IPv4Address and IPv6Address
+                    # but this is handled by the ipaddress module natively by raising a TypeError
+                    device = AsyncEOSDevice(host=str(range_increment), tags=range_def.tags, **kwargs)
+                    inventory.add_device(device)
+                    range_increment += 1
+            except ValueError as e:
+                message = f"Could not parse the following range in the inventory: {range_def.start} - {range_def.end}"
+                anta_log_exception(e, message, logger)
+                raise InventoryIncorrectSchema(message) from e
+            except TypeError as e:
+                message = f"A range in the inventory has different address families for start and end: {range_def.start} - {range_def.end}"
+                anta_log_exception(e, message, logger)
+                raise InventoryIncorrectSchema(message) from e
+
+    @staticmethod
     def parse(
-        inventory_file: str, username: str, password: str, enable_password: Optional[str] = None, timeout: Optional[float] = None, insecure: bool = False
+        inventory_file: str,
+        username: str,
+        password: str,
+        enable: bool = False,
+        enable_password: Optional[str] = None,
+        timeout: Optional[float] = None,
+        insecure: bool = False,
     ) -> AntaInventory:
         # pylint: disable=too-many-arguments
         """
-        Create an AntaInventory object from an inventory file.
-        Instantiate AntaDevice objects using the AsyncEOSDevice subclass.
+        Create an AntaInventory instance from an inventory file.
+        The inventory devices are AsyncEOSDevice instances.
 
         Args:
             inventory_file (str): Path to inventory YAML file where user has described his inputs
             username (str): Username to use to connect to devices
             password (str): Password to use to connect to devices
+            enable (bool): Whether or not the commands need to be run in enable mode towards the devices
             timeout (float, optional): timeout in seconds for every API call.
 
         Raises:
             InventoryRootKeyError: Root key of inventory is missing.
             InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
             InventoryUnknownFormat: Output format is not supported.
         """
 
         inventory = AntaInventory()
-        kwargs: Dict[str, Any] = {"username": username, "password": password, "enable_password": enable_password, "timeout": timeout, "insecure": insecure}
+        kwargs: Dict[str, Any] = {
+            "username": username,
+            "password": password,
+            "enable": enable,
+            "enable_password": enable_password,
+            "timeout": timeout,
+            "insecure": insecure,
+        }
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
         with open(inventory_file, "r", encoding="UTF-8") as file:
             data = safe_load(file)
 
         # Load data using Pydantic
         try:
@@ -77,31 +165,17 @@
             logger.error(f"Inventory root key is missing: {AntaInventory.INVENTORY_ROOT_KEY}")
             raise InventoryRootKeyError(f"Inventory root key ({AntaInventory.INVENTORY_ROOT_KEY}) is not defined in your inventory") from exc
         except ValidationError as exc:
             logger.error("Inventory data are not compliant with inventory models")
             raise InventoryIncorrectSchema(f"Inventory is not following the schema: {str(exc)}") from exc
 
         # Read data from input
-        if inventory_input.hosts is not None:
-            for host in inventory_input.hosts:
-                device = AsyncEOSDevice(name=host.name, host=str(host.host), port=host.port, tags=host.tags, **kwargs)
-                inventory.add_device(device)
-        if inventory_input.networks is not None:
-            for network in inventory_input.networks:
-                for host_ip in IPNetwork(str(network.network)):
-                    device = AsyncEOSDevice(host=str(host_ip), tags=network.tags, **kwargs)
-                    inventory.add_device(device)
-        if inventory_input.ranges is not None:
-            for range_def in inventory_input.ranges:
-                range_increment = IPAddress(str(range_def.start))
-                range_stop = IPAddress(str(range_def.end))
-                while range_increment <= range_stop:
-                    device = AsyncEOSDevice(host=str(range_increment), tags=range_def.tags, **kwargs)
-                    inventory.add_device(device)
-                    range_increment += 1
+        AntaInventory._parse_hosts(inventory_input, inventory, **kwargs)
+        AntaInventory._parse_networks(inventory_input, inventory, **kwargs)
+        AntaInventory._parse_ranges(inventory_input, inventory, **kwargs)
 
         return inventory
 
     ###########################################################################
     # Public methods
     ###########################################################################
 
@@ -163,11 +237,8 @@
         results = await asyncio.gather(
             *(device.refresh() for device in self.values()),
             return_exceptions=True,
         )
         for r in results:
             if isinstance(r, Exception):
                 message = "Error when refreshing inventory"
-                if __DEBUG__:
-                    logger.exception(message, exc_info=r)
-                else:
-                    logger.error(f"{message}: {exc_to_str(r)}")
+                anta_log_exception(r, message, logger)
```

### Comparing `anta-0.6.0/anta/inventory/models.py` & `anta-0.7.0/anta/inventory/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/loader.py` & `anta-0.7.0/anta/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     Configure logging
 
     Args:
         level (str, optional): level name to configure.
     """
     root = logging.getLogger()
     loglevel = getattr(logging, level.upper())
-    handler = RichHandler(markup=True, rich_tracebacks=True)
+    handler = RichHandler(markup=True, rich_tracebacks=True, tracebacks_show_locals=True)
     if __DEBUG__:
-        fmt_string = "[grey58]\[%(name)s][/grey58] %(message)s"  # noqa: W605 pylint: disable=anomalous-backslash-in-string
+        fmt_string = r"[grey58]\[%(name)s][/grey58] %(message)s"
     else:
         fmt_string = "%(message)s"
     formatter = logging.Formatter(fmt=fmt_string, datefmt="[%X]")
     handler.setFormatter(formatter)
     root.addHandler(handler)
     root.setLevel(loglevel)
```

### Comparing `anta-0.6.0/anta/models.py` & `anta-0.7.0/anta/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from copy import deepcopy
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Coroutine, Dict, List, Literal, Optional, TypeVar, Union
 
 from pydantic import BaseModel, ConfigDict, conint
 from rich.progress import Progress, TaskID
 
-from anta import __DEBUG__
 from anta.result_manager.models import TestResult
-from anta.tools.misc import exc_to_str
+from anta.tools.misc import anta_log_exception, exc_to_str
 
 if TYPE_CHECKING:
     from anta.device import AntaDevice
 
 F = TypeVar("F", bound=Callable[..., Any])
 DEFAULT_TAG = "all"
 
@@ -139,14 +138,16 @@
 
     The goal of this class is to handle the heavy lifting and make
     writing a test as simple as possible.
 
     TODO - complete doctstring with example
     """
 
+    # pylint: disable=too-many-instance-attributes
+
     # Mandatory class attributes
     # TODO - find a way to tell mypy these are mandatory for child classes - maybe Protocol
     name: ClassVar[str]
     description: ClassVar[str]
     categories: ClassVar[list[str]]
     # Or any child type
     commands: ClassVar[list[AntaCommand]]
@@ -158,24 +159,40 @@
     # Optional class attributes
     test_filters: ClassVar[list[AntaTestFilter]]
 
     def __init__(
         self,
         device: AntaDevice,
         template_params: list[dict[str, Any]] | None = None,
+        result_description: str | None = None,
+        result_categories: list[str] | None = None,
+        result_custom_field: str | None = None,
         # TODO document very well the order of eos_data
         eos_data: list[dict[Any, Any] | str] | None = None,
         labels: list[str] | None = None,
     ):
-        """Class constructor"""
+        """
+        AntaTest Constructor
+
+        Doc to be completed
+
+        Arguments:
+            result_custom_field (str): a free string that is included in the TestResult object
+        """
         # Accept 6 input arguments
         # pylint: disable=R0913
         self.logger: logging.Logger = logging.getLogger(f"{self.__module__}.{self.__class__.__name__}")
         self.device: AntaDevice = device
-        self.result: TestResult = TestResult(name=device.name, test=self.name, test_category=self.categories, test_description=self.description)
+        self.result: TestResult = TestResult(
+            name=device.name,
+            test=self.name,
+            categories=result_categories or self.categories,
+            description=result_description or self.description,
+            custom_field=result_custom_field,
+        )
         self.labels: List[str] = labels or []
         self.instance_commands: List[AntaCommand] = []
 
         # TODO - check optimization for deepcopy
         # Generating instance_commands from list of commands and template
         if hasattr(self.__class__, "commands") and (cmds := self.__class__.commands) is not None:
             self.instance_commands.extend(deepcopy(cmds))
@@ -227,31 +244,28 @@
         """
         Method used to collect outputs of all commands of this test class from the device of this test instance.
         """
         try:
             await self.device.collect_commands(self.instance_commands)
         except Exception as e:  # pylint: disable=broad-exception-caught
             message = f"Exception raised while collecting commands for test {self.name} (on device {self.device.name})"
-            if __DEBUG__:
-                self.logger.exception(message)
-            else:
-                self.logger.error(f"{message}: {exc_to_str(e)}")
+            anta_log_exception(e, message, self.logger)
             self.result.is_error(exc_to_str(e))
 
     @staticmethod
     def anta_test(function: F) -> Callable[..., Coroutine[Any, Any, TestResult]]:
         """
         Decorator for anta_test that handles injecting test data if given and collecting it using asyncio if missing
         """
 
         @wraps(function)
         async def wrapper(
             self: AntaTest,
             eos_data: list[dict[Any, Any] | str] | None = None,
-            **kwargs: dict[str, Any],
+            **kwargs: Any,
         ) -> TestResult:
             """
             Wraps the test function and implement (in this order):
             1. Instantiate the command outputs if `eos_data` is provided
             2. Collect missing command outputs from the device
             3. Run the test function
             4. Catches and set the result if the test function raises an exception
@@ -280,18 +294,15 @@
                     self.result.is_error(
                         "\n".join([f"{cmd.command} has failed: {exc_to_str(cmd.failed)}" if cmd.failed else f"{cmd.command} has failed" for cmd in cmds])
                     )
                     return self.result
                 function(self, **kwargs)
             except Exception as e:  # pylint: disable=broad-exception-caught
                 message = f"Exception raised for test {self.name} (on device {self.device.name})"
-                if __DEBUG__:
-                    self.logger.exception(message)
-                else:
-                    self.logger.error(f"{message}: {exc_to_str(e)}")
+                anta_log_exception(e, message, self.logger)
                 self.result.is_error(exc_to_str(e))
 
             AntaTest.update_progress()
             return self.result
 
         return wrapper
```

### Comparing `anta-0.6.0/anta/reporter/__init__.py` & `anta-0.7.0/anta/reporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         Args:
             status (str): status value to colorized
             output_type (str, optional): Which format to output code. Defaults to 'Text'.
 
         Returns:
             Any: Can be either str or Text with Style
         """
+        # TODO refactor this code as it looks quite surprising
         if len([result for result in self.colors if str(result.level).upper() == status.upper()]) == 1:
             code: ColorManager = [result for result in self.colors if str(result.level).upper() == status.upper()][0]
             return code.style_rich() if output_type == "Text" else code.string()
         return None
 
     def report_all(
         self,
@@ -112,16 +113,16 @@
         table = self._build_headers(headers=headers, table=table)
 
         for result in result_manager.get_results(output_format="list"):
             # pylint: disable=R0916
             if (host is None and testcase is None) or (host is not None and str(result.name) == host) or (testcase is not None and testcase == str(result.test)):
                 state = self._color_result(status=str(result.result), output_type="str")
                 message = self._split_list_to_txt_list(result.messages) if len(result.messages) > 0 else ""
-                test_categories = ", ".join(result.test_category)
-                table.add_row(str(result.name), result.test, state, message, result.test_description, test_categories)
+                categories = ", ".join(result.categories)
+                table.add_row(str(result.name), result.test, state, message, result.description, categories)
         return table
 
     def report_summary_tests(
         self,
         result_manager: ResultManager,
         testcase: Optional[str] = None,
         title: str = "Summary per test case",
@@ -190,15 +191,15 @@
         table = Table(title=title)
         headers = [
             "Host IP",
             "# of success",
             "# of skipped",
             "# of failure",
             "# of errors",
-            "List of failed ortest case",
+            "List of failed or error test cases",
         ]
         table = self._build_headers(headers=headers, table=table)
         for host_read in result_manager.get_hosts():
             if host is None or str(host_read) == host:
                 results = result_manager.get_result_by_host(host_read)
                 logger.debug("data to use for computation")
                 logger.debug(f"{host}: {results}")
@@ -238,16 +239,16 @@
         >>> print(data)
         [
             {
                 name: ...,
                 test: ...,
                 result: ...,
                 messages: [...]
-                test_category: ...,
-                test_description: ...,
+                categories: ...,
+                description: ...,
             }
         ]
 
         Args:
             data (List[Dict[str, Any]]): List of results from ResultManager.get_results
             trim_blocks (bool, optional): enable trim_blocks for J2 rendering. Defaults to True.
             lstrip_blocks (bool, optional): enable lstrip_blocks for J2 rendering. Defaults to True.
```

### Comparing `anta-0.6.0/anta/reporter/models.py` & `anta-0.7.0/anta/reporter/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/result_manager/__init__.py` & `anta-0.7.0/anta/result_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def __len__(self) -> int:
         """
         Implement __len__ method to count number of results.
         """
         return len(self._result_entries)
 
-    def __update_status(self, test_status: str) -> None:
+    def _update_status(self, test_status: str) -> None:
         """
         Update ResultManager status based on the table above.
         """
         if test_status not in RESULT_OPTIONS:
             raise ValueError("{test_status} is not a valid result option")
         if test_status == "error":
             self.error_status = True
@@ -115,15 +115,15 @@
         """Add a result to the list
 
         Args:
             entry (TestResult): TestResult data to add to the report
         """
         logger.debug(entry)
         self._result_entries.append(entry)
-        self.__update_status(entry.result)
+        self._update_status(entry.result)
 
     def add_test_results(self, entries: List[TestResult]) -> None:
         """Add a list of results to the list
 
         Args:
             entries (List[TestResult]): list of TestResult data to add to the report
         """
@@ -153,16 +153,18 @@
         """
         if output_format == "list":
             return list(self._result_entries)
 
         if output_format == "json":
             return json.dumps(pydantic_to_dict(self._result_entries), indent=4)
 
-        # Default return for native format.
-        return self._result_entries
+        if output_format == "native":
+            # Default return for native format.
+            return self._result_entries
+        raise ValueError(f"{output_format} is not a valid value ['list', 'json', 'native']")
 
     def get_result_by_test(self, test_name: str, output_format: str = "native") -> Any:
         """
         Get list of test result for a given test.
 
         Args:
             test_name (str): Test name to use to filter results
```

### Comparing `anta-0.6.0/anta/result_manager/models.py` & `anta-0.7.0/anta/result_manager/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Models related to anta.result_manager module."""
 
-from typing import Iterator, List
+from typing import Iterator, List, Optional
 
-from pydantic import BaseModel, RootModel, validator
+from pydantic import BaseModel, RootModel, field_validator
 
 RESULT_OPTIONS = ["unset", "success", "failure", "error", "skipped"]
 
 
 class TestResult(BaseModel):
     """
     Describe the result of a test from a single device.
 
     Attributes:
         name (str): Device name where the test has run.
         test (str): Test name runs on the device.
-        test_category (List[str]): List of test categories the test belongs to.
-        test_description (str): Test description.
+        categories (List[str]): List of categories the TestResult belongs to, by default the AntaTest categories.
+        description (str): TestResult description, by default the AntaTest description.
         results (str): Result of the test. Can be one of ["unset", "success", "failure", "error", "skipped"].
         message (str, optional): Message to report after the test if any.
+        custom_field (str, optional): Custom field to store a string for flexibility in integrating with ANTA
     """
 
     name: str
     test: str
-    test_category: List[str]
-    test_description: str
+    categories: List[str]
+    description: str
     result: str = "unset"
     messages: List[str] = []
+    custom_field: Optional[str] = None
 
     @classmethod
-    @validator("result", allow_reuse=True)
+    @field_validator("result")
     def name_must_be_in(cls, v: str) -> str:
         """
         Status validator
 
         Validate status is a supported one
 
         Args:
```

### Comparing `anta-0.6.0/anta/runner.py` & `anta-0.7.0/anta/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 """
 
 import asyncio
 import itertools
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from anta import __DEBUG__
 from anta.inventory import AntaInventory
 from anta.models import AntaTest
 from anta.result_manager import ResultManager
 from anta.result_manager.models import TestResult
-from anta.tools.misc import exc_to_str
+from anta.tools.misc import anta_log_exception
 
 logger = logging.getLogger(__name__)
 
-# Key from YAML file tranfered to AntaTemplate of the test.
-TEST_TPL_PARAMS = "template_params"
+# Keys from the ANTA test catalog file tranferred to kwargs for AntaTest initialization.
+TEST_CATALOG_PARAMS = [
+    "result_overwrite",
+    "template_params",
+]
 
 
 async def main(
     manager: ResultManager,
     inventory: AntaInventory,
     tests: List[Tuple[Callable[..., TestResult], Dict[Any, Any]]],
     tags: Optional[List[str]] = None,
@@ -29,57 +31,71 @@
 ) -> None:
     """
     Main coroutine to run ANTA.
     Use this as an entrypoint to the test framwork in your script.
 
     Args:
         manager (ResultManager): ResultManager object to populate with the test results.
-        inventory (AntaInventory): Device inventory object.
-        tests (List[...]): Test catalog. Output of anta.loader.parse_catalog().
+        inventory (AntaInventory): AntaInventory object that includes the device(s).
+        tests (List[...]): ANTA test catalog. Output of anta.loader.parse_catalog().
+        tags (Optional[List[str]]): List of tags to filter devices from the inventory. Defaults to None.
+        established_only (bool): Include only established device(s). Defaults to True.
 
     Example:
         anta.tests.routing.bgp:
         - VerifyBGPIPv4UnicastCount:
             number: 3
             template_params:
                 - vrf: default
 
+        anta.tests.connectivity:
+        - VerifyReachability:
+            result_overwrite:
+              categories:
+                - "Overwritten category 1"
+              description: "Test with overwritten description"
+              custom_field: "Test run by John Doe"
+            template_params:
+              - src: Loopback0
+                dst: 10.1.0.1
+
     Returns:
-        any: List of results.
+        any: ResultManager object gets updated with the test results.
     """
     # Accept 6 arguments here
     # pylint: disable=R0913
 
     await inventory.connect_inventory()
 
     # asyncio.gather takes an iterator of the function to run concurrently.
     # we get the cross product of the devices and tests to build that iterator.
 
     coros = []
     for device, test in itertools.product(inventory.get_inventory(established_only=established_only, tags=tags).values(), tests):
-        test_params = {k: v for k, v in test[1].items() if k != TEST_TPL_PARAMS}
-        template_params = test[1].get(TEST_TPL_PARAMS)
+        kwargs = {k: v for k, v in test[1].items() if k in TEST_CATALOG_PARAMS}
+
+        if "result_overwrite" in kwargs:
+            result_overwrite = kwargs.pop("result_overwrite")
+            result_overwrite = {"result_" + k: v for k, v in result_overwrite.items()}
+            kwargs.update(result_overwrite)
+
+        test_params = {k: v for k, v in test[1].items() if k not in TEST_CATALOG_PARAMS}
+
         try:
             # Instantiate AntaTest object
-            test_instance = test[0](device=device, template_params=template_params)
+            test_instance = test[0](device=device, **kwargs)
             coros.append(test_instance.test(eos_data=None, **test_params))
         except Exception as e:  # pylint: disable=broad-exception-caught
             message = "Error when creating ANTA tests"
-            if __DEBUG__:
-                logger.exception(message)
-            else:
-                logger.error(f"{message}: {exc_to_str(e)}")
+            anta_log_exception(e, message, logger)
 
     if AntaTest.progress is not None:
         AntaTest.nrfu_task = AntaTest.progress.add_task("Running NRFU Tests...", total=len(coros))
 
     logger.info("Running ANTA tests...")
     res = await asyncio.gather(*coros, return_exceptions=True)
     for r in res:
         if isinstance(r, Exception):
             message = "Error in main ANTA Runner"
-            if __DEBUG__:
-                logger.exception(message, exc_info=r)
-            else:
-                logger.error(f"{message}: {exc_to_str(r)}")
+            anta_log_exception(r, message, logger)
             res.remove(r)
     manager.add_test_results(res)
```

### Comparing `anta-0.6.0/anta/tests/aaa.py` & `anta-0.7.0/anta/tests/aaa.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/configuration.py` & `anta-0.7.0/anta/tests/configuration.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/connectivity.py` & `anta-0.7.0/anta/tests/connectivity.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/field_notices.py` & `anta-0.7.0/anta/tests/field_notices.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/hardware.py` & `anta-0.7.0/anta/tests/hardware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,215 +1,251 @@
 """
-Test functions related to the hardware or environement
+Test functions related to the hardware or environment
 """
 from __future__ import annotations
 
 from typing import List, Optional
 
 from anta.decorators import skip_on_platforms
 from anta.models import AntaCommand, AntaTest
 
 
 class VerifyTransceiversManufacturers(AntaTest):
     """
-    Verifies Manufacturers of all Transceivers.
+    This test verifies if all the transceivers come from approved manufacturers.
+
+    Expected Results:
+      * success: The test will pass if all transceivers are from approved manufacturers.
+      * failure: The test will fail if some transceivers are from unapproved manufacturers.
+      * skipped: The test will be skipped if a list of approved manufacturers is not provided or if it's run on a virtualized platform.
     """
 
     name = "VerifyTransceiversManufacturers"
-    description = ""
+    description = "Verifies the transceiver's manufacturer against a list of approved manufacturers."
     categories = ["hardware"]
     commands = [AntaCommand(command="show inventory", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self, manufacturers: Optional[List[str]] = None) -> None:
         """
         Run VerifyTransceiversManufacturers validation
 
         Args:
-            manufacturers: List of allowed transceivers manufacturers.
+            manufacturers: List of approved transceivers manufacturers.
         """
         if not manufacturers:
-            self.result.is_skipped(f"{self.__class__.name} was not run as no manufacturers were given")
+            self.result.is_skipped(f"{self.__class__.name} was not run because manufacturers list was not provided")
+            return
+
+        command_output = self.instance_commands[0].json_output
+        wrong_manufacturers = {interface: value["mfgName"] for interface, value in command_output["xcvrSlots"].items() if value["mfgName"] not in manufacturers}
+        if not wrong_manufacturers:
+            self.result.is_success()
         else:
-            command_output = self.instance_commands[0].json_output
-            wrong_manufacturers = {interface: value["mfgName"] for interface, value in command_output["xcvrSlots"].items() if value["mfgName"] not in manufacturers}
-            if not wrong_manufacturers:
-                self.result.is_success()
-            else:
-                self.result.is_failure("The following interfaces have transceivers from unauthorized manufacturers")
-                self.result.messages.append(str(wrong_manufacturers))
+            self.result.is_failure(f"Some transceivers are from unapproved manufacturers: {wrong_manufacturers}")
 
 
 class VerifyTemperature(AntaTest):
     """
-    Verifies device temparture is currently OK (temperatureOK).
+    This test verifies if the device temperature is within acceptable limits.
+
+    Expected Results:
+      * success: The test will pass if the device temperature is currently OK: 'temperatureOk'.
+      * failure: The test will fail if the device temperature is NOT OK.
+      * skipped: Test test will be skipped if it's run on a virtualized platform.
     """
 
     name = "VerifyTemperature"
-    description = "Verifies device temparture is currently OK (temperatureOK)"
+    description = "Verifies if the device temperature is within the acceptable range."
     categories = ["hardware"]
     commands = [AntaCommand(command="show system environment temperature", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self) -> None:
-        """Run VerifyTemperature validation"""
+        """
+        Run VerifyTemperature validation
+        """
         command_output = self.instance_commands[0].json_output
         temperature_status = command_output["systemStatus"] if "systemStatus" in command_output.keys() else ""
         if temperature_status == "temperatureOk":
             self.result.is_success()
         else:
-            self.result.is_failure(f"Device temperature is not OK, systemStatus: {temperature_status }")
+            self.result.is_failure(f"Device temperature exceeds acceptable limits. Current system status: '{temperature_status}'")
 
 
 class VerifyTransceiversTemperature(AntaTest):
     """
-    Verifies Transceivers temperature is currently OK.
+    This test verifies if all the transceivers are operating at an acceptable temperature.
+
+    Expected Results:
+          * success: The test will pass if all transceivers status are OK: 'ok'.
+          * failure: The test will fail if some transceivers are NOT OK.
+          * skipped: Test test will be skipped if it's run on a virtualized platform.
     """
 
     name = "VerifyTransceiversTemperature"
-    description = "Verifies Transceivers temperature is currently OK"
+    description = "Verifies that all transceivers are operating within the acceptable temperature range."
     categories = ["hardware"]
     commands = [AntaCommand(command="show system environment temperature transceiver", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self) -> None:
-        """Run VerifyTransceiversTemperature validation"""
+        """
+        Run VerifyTransceiversTemperature validation
+        """
         command_output = self.instance_commands[0].json_output
         sensors = command_output["tempSensors"] if "tempSensors" in command_output.keys() else ""
         wrong_sensors = {
             sensor["name"]: {
                 "hwStatus": sensor["hwStatus"],
                 "alertCount": sensor["alertCount"],
             }
             for sensor in sensors
             if sensor["hwStatus"] != "ok" or sensor["alertCount"] != 0
         }
         if not wrong_sensors:
             self.result.is_success()
         else:
-            self.result.is_failure("The following sensors do not have the correct temperature or had alarms in the past:")
-            self.result.messages.append(str(wrong_sensors))
+            self.result.is_failure(f"The following sensors are operating outside the acceptable temperature range or have raised alerts: {wrong_sensors}")
 
 
 class VerifyEnvironmentSystemCooling(AntaTest):
     """
-    Verifies the System Cooling is ok.
+    This test verifies the device's system cooling.
+
+    Expected Results:
+      * success: The test will pass if the system cooling status is OK: 'coolingOk'.
+      * failure: The test will fail if the system cooling status is NOT OK.
+      * skipped: The test will be skipped if it's run on a virtualized platform.
     """
 
     name = "VerifyEnvironmentSystemCooling"
-    description = "Verifies the fans status is OK for fans"
+    description = "Verifies the system cooling status."
     categories = ["hardware"]
     commands = [AntaCommand(command="show system environment cooling", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self) -> None:
-        """Run VerifyEnvironmentCooling validation"""
+        """
+        Run VerifyEnvironmentCooling validation
+        """
 
         command_output = self.instance_commands[0].json_output
         sys_status = command_output["systemStatus"] if "systemStatus" in command_output.keys() else ""
 
         self.result.is_success()
         if sys_status != "coolingOk":
-            self.result.is_failure(f"Device System cooling is not OK: {sys_status}")
+            self.result.is_failure(f"Device system cooling is not OK: '{sys_status}'")
 
 
 class VerifyEnvironmentCooling(AntaTest):
     """
-    Verifies the fans status is in the accepted states list.
+    This test verifies the fans status.
 
-    Default accepted states list is ['ok']
+    Expected Results:
+      * success: The test will pass if the fans status are within the accepted states list.
+      * failure: The test will fail if some fans status is not within the accepted states list.
+      * skipped: The test will be skipped if the accepted states list is not provided or if it's run on a virtualized platform.
     """
 
     name = "VerifyEnvironmentCooling"
-    description = "Verifies the fans status is OK for fans"
+    description = "Verifies if the fans status are within the accepted states list."
     categories = ["hardware"]
     commands = [AntaCommand(command="show system environment cooling", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self, accepted_states: Optional[List[str]] = None) -> None:
         """
         Run VerifyEnvironmentCooling validation
 
         Args:
-            accepted_states: Accepted states list for fan status
+            accepted_states: Accepted states list for fan status.
         """
-        if accepted_states is None:
-            accepted_states = ["ok"]
+        if not accepted_states:
+            self.result.is_skipped(f"{self.__class__.name} was not run because accepted_states list was not provided")
+            return
 
         command_output = self.instance_commands[0].json_output
         self.result.is_success()
         # First go through power supplies fans
         for power_supply in command_output.get("powerSupplySlots", []):
             for fan in power_supply.get("fans", []):
                 if (state := fan["status"]) not in accepted_states:
-                    if self.result.result == "success":
-                        self.result.is_failure(f"Some fans state are not in the accepted list: {accepted_states}.")
-                    self.result.is_failure(f"Fan {fan['label']} on PowerSupply {power_supply['label']} has state '{state}'.")
-        # Then go through Fan Trays
+                    self.result.is_failure(f"Fan {fan['label']} on PowerSupply {power_supply['label']} is: '{state}'")
+        # Then go through fan trays
         for fan_tray in command_output.get("fanTraySlots", []):
             for fan in fan_tray.get("fans", []):
                 if (state := fan["status"]) not in accepted_states:
-                    if self.result.result == "success":
-                        self.result.is_failure(f"Some fans state are not in the accepted list: {accepted_states}.")
-                    self.result.is_failure(f"Fan {fan['label']} on Fan Tray {fan_tray['label']} has state '{state}'.")
+                    self.result.is_failure(f"Fan {fan['label']} on Fan Tray {fan_tray['label']} is: '{state}'")
 
 
 class VerifyEnvironmentPower(AntaTest):
     """
-    Verifies the power supplies status is in the accepted states list
+    This test verifies the power supplies status.
 
-    The default accepted states list is ['ok']
+    Expected Results:
+      * success: The test will pass if the power supplies status are within the accepted states list.
+      * failure: The test will fail if some power supplies status is not within the accepted states list.
+      * skipped: The test will be skipped if the accepted states list is not provided or if it's run on a virtualized platform.
     """
 
     name = "VerifyEnvironmentPower"
-    description = "Verifies the power supplies status is OK"
+    description = "Verifies if the power supplies status are within the accepted states list."
     categories = ["hardware"]
     commands = [AntaCommand(command="show system environment power", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self, accepted_states: Optional[List[str]] = None) -> None:
         """
         Run VerifyEnvironmentPower validation
 
         Args:
-            accepted_states: Accepted states list for power supplies
+            accepted_states: Accepted states list for power supplies status.
         """
-        if accepted_states is None:
-            accepted_states = ["ok"]
+        if not accepted_states:
+            self.result.is_skipped(f"{self.__class__.name} was not run because accepted_states list was not provided")
+            return
+
         command_output = self.instance_commands[0].json_output
         power_supplies = command_output["powerSupplies"] if "powerSupplies" in command_output.keys() else "{}"
         wrong_power_supplies = {
             powersupply: {"state": value["state"]} for powersupply, value in dict(power_supplies).items() if value["state"] not in accepted_states
         }
         if not wrong_power_supplies:
             self.result.is_success()
         else:
-            self.result.is_failure(f"The following power supplies states are not in the accepted_states list {accepted_states}")
-            self.result.messages.append(str(wrong_power_supplies))
+            self.result.is_failure(f"The following power supplies status are not in the accepted states list: {wrong_power_supplies}")
 
 
 class VerifyAdverseDrops(AntaTest):
     """
-    Verifies there is no adverse drops on DCS7280E and DCS7500E.
+    This test verifies if there are no adverse drops on DCS7280E and DCS7500E.
+
+    Expected Results:
+      * success: The test will pass if there are no adverse drops.
+      * failure: The test will fail if there are adverse drops.
+      * skipped: The test will be skipped if it's run on a virtualized platform.
     """
 
     name = "VerifyAdverseDrops"
-    description = "Verifies there is no adverse drops on DCS7280E and DCS7500E"
+    description = "Verifies there are no adverse drops on DCS7280E and DCS7500E"
     categories = ["hardware"]
     commands = [AntaCommand(command="show hardware counter drop", ofmt="json")]
 
     @skip_on_platforms(["cEOSLab", "vEOS-lab"])
     @AntaTest.anta_test
     def test(self) -> None:
-        """Run VerifyAdverseDrops validation"""
+        """
+        Run VerifyAdverseDrops validation
+        """
         command_output = self.instance_commands[0].json_output
         total_adverse_drop = command_output["totalAdverseDrops"] if "totalAdverseDrops" in command_output.keys() else ""
         if total_adverse_drop == 0:
             self.result.is_success()
         else:
-            self.result.is_failure(f"Device TotalAdverseDrops counter is {total_adverse_drop}")
+            self.result.is_failure(f"Device totalAdverseDrops counter is: '{total_adverse_drop}'")
```

### Comparing `anta-0.6.0/anta/tests/interfaces.py` & `anta-0.7.0/anta/tests/interfaces.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/logging.py` & `anta-0.7.0/anta/tests/logging.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/mlag.py` & `anta-0.7.0/anta/tests/mlag.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/multicast.py` & `anta-0.7.0/anta/tests/multicast.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/profiles.py` & `anta-0.7.0/anta/tests/profiles.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/routing/bgp.py` & `anta-0.7.0/anta/tests/routing/bgp.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/routing/generic.py` & `anta-0.7.0/anta/tests/routing/generic.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/routing/ospf.py` & `anta-0.7.0/anta/tests/routing/ospf.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/security.py` & `anta-0.7.0/anta/tests/security.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/snmp.py` & `anta-0.7.0/anta/tests/snmp.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/software.py` & `anta-0.7.0/anta/tests/software.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tests/stp.py` & `anta-0.7.0/anta/tests/stp.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tools/get_value.py` & `anta-0.7.0/anta/tools/get_value.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta/tools/pydantic.py` & `anta-0.7.0/anta/tools/pydantic.py`

 * *Files identical despite different names*

### Comparing `anta-0.6.0/anta.egg-info/PKG-INFO` & `anta-0.7.0/anta.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.6.0
+Version: 0.7.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Khelil Sator <ksator@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -204,15 +204,15 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://www.anta.ninja
 Project-URL: Bug Tracker, https://github.com/arista-netdevops-community/anta/issues
-Project-URL: Contributing, https://github.com/arista-netdevops-community/anta/blob/master/CONTRIBUTING.md
+Project-URL: Contributing, https://www.anta.ninja/main/contribution/
 Keywords: test,anta,Arista,network,automation,networking,devops,netdevops
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -224,80 +224,9 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: doc
 License-File: LICENSE
-
-[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen.svg)](https://github.com/arista-netdevops-community/anta/blob/master/LICENSE)
-[![Linting and Testing Anta](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml/badge.svg)](https://github.com/arista-netdevops-community/anta/actions/workflows/code-testing.yml)
-[![github release](https://img.shields.io/github/release/arista-netdevops-community/anta.svg)](https://github.com/arista-netdevops-community/anta/releases/)
-
-# Arista Network Test Automation (ANTA) Framework
-
-__WARNING:__ Documentation is work in progress for version 0.6.0 available in Pypi.
-
-This repository is a Python package to automate tests on Arista devices.
-
-- The package name is ANTA, which stands for **Arista Network Test Automation**.
-- This package provides a set of tests to validate the state of your network.
-- This package can be imported in Python scripts:
-  - To automate NRFU (Network Ready For Use) test on a preproduction network
-  - To automate tests on a live network (periodically or on demand)
-
-This repository comes with a cli to run __Arista Network Test Automation__ (ANTA) framework using your preferred shell:
-
-```bash
-# Install ANTA CLI
-$ pip install anta
-
-# Run ANTA CLI
-$ anta
-Usage: anta [OPTIONS] COMMAND [ARGS]...
-
-  Arista Network Test Automation (ANTA) CLI
-
-Options:
-  --version                       Show the version and exit.
-  --username TEXT                 Username to connect to EOS  [env var:
-                                  ANTA_USERNAME; required]
-  --password TEXT                 Password to connect to EOS  [env var:
-                                  ANTA_PASSWORD; required]
-  --timeout INTEGER               Global connection timeout  [env var:
-                                  ANTA_TIMEOUT; default: 5]
-  --insecure                      Disable SSH Host Key validation  [env var:
-                                  ANTA_INSECURE]
-  --enable-password TEXT          Enable password if required to connect  [env
-                                  var: ANTA_ENABLE_PASSWORD]
-  -i, --inventory FILE            Path to the inventory YAML file  [env var:
-                                  ANTA_INVENTORY; required]
-  --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
-                                  ANTA logging level  [env var:
-                                  ANTA_LOG_LEVEL; default: INFO]
-  --ignore-status                 Always exit with success  [env var:
-                                  ANTA_IGNORE_STATUS]
-  --ignore-error                  Only report failures and not errors  [env
-                                  var: ANTA_IGNORE_ERROR]
-  --help                          Show this message and exit.
-
-Commands:
-  debug  Debug commands for building ANTA
-  exec   Execute commands to inventory devices
-  get    Get data from/to ANTA
-  nrfu   Run NRFU against inventory devices
-```
-
-<img src="https://github.com/arista-netdevops-community/anta/raw/master/docs/imgs/anta-nrfu-table-group-by-test-output.png"></img>
-
-# Documentation
-
-The documentation is published on [ANTA package website](https://www.anta.ninja)
-
-# Contribution guide
-
-Contributions are welcome. Please refer to the [contribution guide](https://raw.githubusercontent.com/arista-netdevops-community/anta/master/docs/contribution.md)
-
-# Credits
-
-Thank you to [Angélique Phillipps](https://github.com/aphillipps), [Colin MacGiollaEáin](https://github.com/colinmacgiolla), [Khelil Sator](https://github.com/ksator), [Matthieu Tache](https://github.com/mtache), [Onur Gashi](https://github.com/onurgashi), [Paul Lavelle](https://github.com/paullavelle), [Guillaume Mulocher](https://github.com/gmuloc) and [Thomas Grimonet](https://github.com/titom73) for their contributions and guidances.
```

### Comparing `anta-0.6.0/anta.egg-info/SOURCES.txt` & `anta-0.7.0/anta.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 MANIFEST.in
-README.md
 pyproject.toml
 anta/__init__.py
 anta/decorators.py
 anta/device.py
 anta/loader.py
 anta/models.py
 anta/runner.py
@@ -55,12 +54,8 @@
 anta/tests/routing/__init__.py
 anta/tests/routing/bgp.py
 anta/tests/routing/generic.py
 anta/tests/routing/ospf.py
 anta/tools/__init__.py
 anta/tools/get_value.py
 anta/tools/misc.py
-anta/tools/pydantic.py
-tests/__init__.py
-tests/data/__init__.py
-tests/data/json_data.py
-tests/units/__init__.py
+anta/tools/pydantic.py
```

