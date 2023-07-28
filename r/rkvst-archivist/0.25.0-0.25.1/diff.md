# Comparing `tmp/rkvst-archivist-0.25.0.tar.gz` & `tmp/rkvst-archivist-0.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rkvst-archivist-0.25.0.tar", last modified: Thu Jul 20 10:54:47 2023, max compression
+gzip compressed data, was "rkvst-archivist-0.25.1.tar", last modified: Fri Jul 28 10:49:57 2023, max compression
```

## Comparing `rkvst-archivist-0.25.0.tar` & `rkvst-archivist-0.25.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 10:54:39.000000 rkvst-archivist-0.25.0/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.900714 rkvst-archivist-0.25.0/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/archivist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 10:52:04.000000 rkvst-archivist-0.25.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 10:54:47.000000 rkvst-archivist-0.25.0/rkvst_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 10:54:47.904713 rkvst-archivist-0.25.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.676294 rkvst-archivist-0.25.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-28 10:49:57.676294 rkvst-archivist-0.25.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.672294 rkvst-archivist-0.25.1/archivist/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-28 10:49:49.000000 rkvst-archivist-0.25.1/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.672294 rkvst-archivist-0.25.1/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.672294 rkvst-archivist-0.25.1/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.672294 rkvst-archivist-0.25.1/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/archivist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-28 10:46:53.000000 rkvst-archivist-0.25.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:49:57.676294 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 10:49:57.000000 rkvst-archivist-0.25.1/rkvst_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-28 10:49:57.676294 rkvst-archivist-0.25.1/setup.cfg
```

### Comparing `rkvst-archivist-0.25.0/LICENSE` & `rkvst-archivist-0.25.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/PKG-INFO` & `rkvst-archivist-0.25.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.25.0
+Version: 0.25.1
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
```

### Comparing `rkvst-archivist-0.25.0/README.rst` & `rkvst-archivist-0.25.1/README.rst`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/access_policies.py` & `rkvst-archivist-0.25.1/archivist/access_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from copy import deepcopy
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Generator, Optional
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 
 if TYPE_CHECKING:
-    from . import archivist
+    from .archivist import Archivist
 
 from .assets import Asset
 from .constants import (
     ACCESS_POLICIES_LABEL,
     ACCESS_POLICIES_SUBPATH,
     ASSETS_LABEL,
 )
@@ -59,15 +59,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{ACCESS_POLICIES_SUBPATH}"
         self._label = f"{self._subpath}/{ACCESS_POLICIES_LABEL}"
 
     def __str__(self) -> str:
         return f"AccessPoliciesClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/appidp.py` & `rkvst-archivist-0.25.1/archivist/appidp.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from typing import TYPE_CHECKING
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 # pylint:disable=too-few-public-methods
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 if TYPE_CHECKING:
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     APPIDP_LABEL,
     APPIDP_SUBPATH,
     APPIDP_TOKEN,
 )
 
@@ -53,15 +53,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{APPIDP_SUBPATH}"
         self._label = f"{self._subpath}/{APPIDP_LABEL}"
 
     def __str__(self) -> str:
         return f"AppIDPClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/applications.py` & `rkvst-archivist-0.25.1/archivist/applications.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 if TYPE_CHECKING:
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     APPLICATIONS_LABEL,
     APPLICATIONS_REGENERATE,
     APPLICATIONS_SUBPATH,
 )
 from .dictmerge import _deepmerge
@@ -51,15 +51,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{APPLICATIONS_SUBPATH}"
         self._label = f"{self._subpath}/{APPLICATIONS_LABEL}"
 
     def __str__(self) -> str:
         return f"ApplicationsClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/archivist.py` & `rkvst-archivist-0.25.1/archivist/archivist.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/archivistpublic.py` & `rkvst-archivist-0.25.1/archivist/archivistpublic.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/asset.py` & `rkvst-archivist-0.25.1/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/assetattachments.py` & `rkvst-archivist-0.25.1/archivist/assetattachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from typing import TYPE_CHECKING, Any, BinaryIO, Optional
 from urllib.parse import urlparse
 
 if TYPE_CHECKING:
     from requests.models import Response
 
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     ASSETATTACHMENTS_LABEL,
     ASSETATTACHMENTS_SUBPATH,
     ATTACHMENTS_LABEL,
     SEP,
 )
@@ -55,15 +55,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._public = archivist_instance.public
         self._subpath = f"{archivist_instance.root}/{ASSETATTACHMENTS_SUBPATH}"
         self._label = f"{self._subpath}/{ASSETATTACHMENTS_LABEL}"
 
     def __str__(self) -> str:
         if self._public:
```

### Comparing `rkvst-archivist-0.25.0/archivist/assets.py` & `rkvst-archivist-0.25.1/archivist/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,44 +21,47 @@
 
 """
 
 from __future__ import annotations
 
 from copy import deepcopy
 from logging import getLogger
-from typing import Any, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-from . import archivist, confirmer
+from . import confirmer
 from .asset import Asset
 from .constants import (
     ASSET_BEHAVIOURS,
     ASSETS_LABEL,
     ASSETS_SUBPATH,
     CONFIRMATION_STATUS,
 )
 from .dictmerge import _deepmerge
 from .errors import ArchivistBadFieldError, ArchivistNotFoundError
 from .utils import selector_signature
 
+if TYPE_CHECKING:
+    from .archivist import Archivist
+
 LOGGER = getLogger(__name__)
 
 
 class _AssetsPublic:
     """AssetsReader
 
     Access to assets entities using CRUD interface. This class is usually
     accessed as an attribute of the Archivist or Public class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._public = archivist_instance.public
         self._subpath = f"{archivist_instance.root}/{ASSETS_SUBPATH}"
 
     def __str__(self) -> str:
         return "AssetsPublic()"
 
@@ -93,15 +96,15 @@
     accessed as an attribute of the Archivist or Public class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         super().__init__(archivist_instance)
         self._label = f"{self._subpath}/{ASSETS_LABEL}"
         self.pending_count: int = 0
 
     def __str__(self) -> str:
         return f"AssetsRestricted({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/attachments.py` & `rkvst-archivist-0.25.1/archivist/attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from os import path
 from typing import TYPE_CHECKING, Any, BinaryIO, Optional
 
 if TYPE_CHECKING:
     from requests.models import Response
 
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     ATTACHMENTS_LABEL,
     ATTACHMENTS_SUBPATH,
 )
 from .dictmerge import _deepmerge
 from .utils import get_url
@@ -63,15 +63,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{ATTACHMENTS_SUBPATH}"
         self._label = f"{self._subpath}/{ATTACHMENTS_LABEL}"
 
     def __str__(self) -> str:
         return f"AttachmentsClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/cmds/runner/main.py` & `rkvst-archivist-0.25.1/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/cmds/template/main.py` & `rkvst-archivist-0.25.1/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/cmds/template/run.py` & `rkvst-archivist-0.25.1/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/compliance.py` & `rkvst-archivist-0.25.1/archivist/compliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     COMPLIANCE_LABEL,
     COMPLIANCE_SUBPATH,
 )
 
 LOGGER = getLogger(__name__)
@@ -54,15 +54,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{COMPLIANCE_SUBPATH}"
         self._label = f"{self._subpath}/{COMPLIANCE_LABEL}"
 
     def __str__(self) -> str:
         return f"ComplianceClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/compliance_policies.py` & `rkvst-archivist-0.25.1/archivist/compliance_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from copy import deepcopy
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
     from .compliance_policy_requests import (
         CompliancePolicyCurrentOutstanding,
         CompliancePolicyDynamicTolerance,
         CompliancePolicyPeriodOutstanding,
         CompliancePolicyRichness,
         CompliancePolicySince,
     )
@@ -71,15 +71,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{COMPLIANCE_POLICIES_SUBPATH}"
         self._label = f"{self._subpath}/{COMPLIANCE_POLICIES_LABEL}"
 
     def __str__(self) -> str:
         return f"CompliancePoliciesClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/compliance_policy_requests.py` & `rkvst-archivist-0.25.1/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/compliance_policy_type.py` & `rkvst-archivist-0.25.1/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/composite.py` & `rkvst-archivist-0.25.1/archivist/composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 
 LOGGER = getLogger(__name__)
 
 
 class _CompositeClient:
     """CompositeClient
@@ -42,15 +42,15 @@
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     These mthods are not unittested and provided as a convenience.
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
 
     def __str__(self) -> str:
         return f"CompositeClient({self._archivist.url})"
 
     def estate_info(self):
         """
```

### Comparing `rkvst-archivist-0.25.0/archivist/confirmer.py` & `rkvst-archivist-0.25.1/archivist/confirmer.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/constants.py` & `rkvst-archivist-0.25.1/archivist/constants.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/dictmerge.py` & `rkvst-archivist-0.25.1/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/errors.py` & `rkvst-archivist-0.25.1/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/events.py` & `rkvst-archivist-0.25.1/archivist/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,32 @@
 
 """
 
 from __future__ import annotations
 
 from copy import deepcopy
 from logging import getLogger
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-from . import archivist, confirmer
+from . import confirmer
 from .constants import (
     ASSETS_SUBPATH,
     ASSETS_WILDCARD,
     CONFIRMATION_STATUS,
     EVENTS_LABEL,
     SBOM_RELEASE,
 )
 from .dictmerge import _deepmerge
 from .errors import ArchivistBadFieldError, ArchivistNotFoundError
 from .sboms import sboms_parse
 
+if TYPE_CHECKING:
+    from .archivist import Archivist
+
 LOGGER = getLogger(__name__)
 
 
 class Event(dict):
     """Event
 
     Event object has dictionary attributes and properties.
@@ -106,15 +109,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._public = archivist_instance.public
         self._subpath = f"{archivist_instance.root}/{ASSETS_SUBPATH}"
 
     def __str__(self) -> str:
         return "EventsPublic()"
 
@@ -278,15 +281,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         super().__init__(archivist_instance)
         self.pending_count: int = 0
 
     def __str__(self) -> str:
         return f"EventsRestricted({self._archivist.url})"
 
     def create(
```

### Comparing `rkvst-archivist-0.25.0/archivist/locations.py` & `rkvst-archivist-0.25.1/archivist/locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from contextlib import suppress
 from copy import deepcopy
 from logging import getLogger
 from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import LOCATIONS_LABEL, LOCATIONS_SUBPATH
 from .dictmerge import _deepmerge
 from .errors import ArchivistNotFoundError
 from .utils import selector_signature
 
 LOGGER = getLogger(__name__)
@@ -65,15 +65,15 @@
     accessed as an attribute of the Archivist class.
 
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{LOCATIONS_SUBPATH}"
         self._label = f"{self._subpath}/{LOCATIONS_LABEL}"
 
     def __str__(self) -> str:
         return f"LocationsClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/logger.py` & `rkvst-archivist-0.25.1/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/parser.py` & `rkvst-archivist-0.25.1/archivist/parser.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/retry429.py` & `rkvst-archivist-0.25.1/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/runner.py` & `rkvst-archivist-0.25.1/archivist/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from .errors import ArchivistError, ArchivistInvalidOperationError
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
 # pylint:disable=missing-function-docstring
 # pylint:disable=protected-access
 if TYPE_CHECKING:
-    from . import archivist
+    from .archivist import Archivist
 
 LOGGER = getLogger(__name__)
 
 
 NOUNS = ("asset", "location", "subject")
 
 
@@ -46,15 +46,15 @@
     #
     #  use_asset_label = 1   = first positional argument
     #  use_asset_label = "asset_id"   = keyword argument
     #  use_asset_label = "-asset_id"   = keyword argument in first argumemt that is
     #                                    a dictionary
     # similarly for location and subjects labels
     #
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         super().__init__()
         self._archivist = archivist_instance
 
         # please keep in alphabetical order
         self["ASSETS_ATTACHMENT_INFO"] = {
             "action": self._archivist.attachments.info,
             "use_asset_label": "add_arg_identity",
@@ -224,15 +224,15 @@
         """
         Return whether this action uses or sets label
         """
         return self.ops(action_name).get(f"{noun}_{endpoint}_label", False)
 
 
 class _Step(dict):  # pylint:disable=too-many-instance-attributes
-    def __init__(self, archivist_instance: archivist.Archivist, **kwargs):
+    def __init__(self, archivist_instance: Archivist, **kwargs):
         super().__init__(**kwargs)
         self._archivist = archivist_instance
         self._args: list[Any] = []
         self._kwargs: dict[str, Any] = {}
         self._actions = None
         self._action = None
         self._action_name = None
@@ -393,15 +393,15 @@
 
 
 class _Runner:
     """
     ArchivistRunner takes a url, token_file.
     """
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self.entities: defaultdict
         self.deletions = {}
 
     def __str__(self) -> str:
         return f"Runner({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/sboms.py` & `rkvst-archivist-0.25.1/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/subjects.py` & `rkvst-archivist-0.25.1/archivist/subjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,28 @@
 """
 
 from __future__ import annotations
 
 from base64 import b64decode
 from json import loads as json_loads
 from logging import getLogger
-from typing import Any, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-from . import archivist, subjects_confirmer
+from . import subjects_confirmer
 from .constants import (
     SUBJECTS_LABEL,
     SUBJECTS_SELF_ID,
     SUBJECTS_SUBPATH,
 )
 from .dictmerge import _deepmerge
 
+if TYPE_CHECKING:
+    from .archivist import Archivist
+
 LOGGER = getLogger(__name__)
 
 
 class Subject(dict):
     """Subject object"""
 
 
@@ -53,15 +56,15 @@
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
     maxDiff = None
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{SUBJECTS_SUBPATH}"
         self._label = f"{self._subpath}/{SUBJECTS_LABEL}"
 
     def __str__(self) -> str:
         return f"SubjectsClient({self._archivist.url})"
 
@@ -87,15 +90,15 @@
                 display_name=display_name,
                 wallet_pub_key=wallet_pub_key,
                 tessera_pub_key=tessera_pub_key,
             ),
         )
 
     def share(
-        self, name: str, other_name: str, other_archivist: archivist.Archivist
+        self, name: str, other_name: str, other_archivist: Archivist
     ) -> Tuple[Subject, Subject]:
         """Import the self subjects from the foreign archivist connection
            from another organization - mutually share.
 
         Args:
             name (str): display_name of the foreign self subject in this archivist
             other_name (str): display_name of the self subject in other archivist
```

### Comparing `rkvst-archivist-0.25.0/archivist/subjects_confirmer.py` & `rkvst-archivist-0.25.1/archivist/subjects_confirmer.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/tenancies.py` & `rkvst-archivist-0.25.1/archivist/tenancies.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     # pylint:disable=cyclic-import      # but pylint doesn't understand this feature
-    from . import archivist
+    from .archivist import Archivist
 
 from .constants import (
     TENANCIES_LABEL,
     TENANCIES_PREFIX,
     TENANCIES_SUBPATH,
 )
 
@@ -52,15 +52,15 @@
     Args:
         archivist (Archivist): :class:`Archivist` instance
 
     """
 
     maxDiff = None
 
-    def __init__(self, archivist_instance: archivist.Archivist):
+    def __init__(self, archivist_instance: Archivist):
         self._archivist = archivist_instance
         self._subpath = f"{archivist_instance.root}/{TENANCIES_SUBPATH}"
         self._label = f"{self._subpath}/{TENANCIES_LABEL}"
 
     def __str__(self) -> str:
         return f"TenanciesClient({self._archivist.url})"
```

### Comparing `rkvst-archivist-0.25.0/archivist/timestamp.py` & `rkvst-archivist-0.25.1/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/archivist/utils.py` & `rkvst-archivist-0.25.1/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/pyproject.toml` & `rkvst-archivist-0.25.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/rkvst_archivist.egg-info/PKG-INFO` & `rkvst-archivist-0.25.1/rkvst_archivist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rkvst-archivist
-Version: 0.25.0
+Version: 0.25.1
 Summary: RKVST Client
 Home-page: https://github.com/rkvst/rkvst-python
 Author: RKVST Inc.
 Author-email: support@rkvst.com
 License: MIT
 Project-URL: Documentation, https://python.rkvst.com
 Project-URL: Source, https://github.com/rkvst/rkvst-python
```

### Comparing `rkvst-archivist-0.25.0/rkvst_archivist.egg-info/SOURCES.txt` & `rkvst-archivist-0.25.1/rkvst_archivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rkvst-archivist-0.25.0/setup.cfg` & `rkvst-archivist-0.25.1/setup.cfg`

 * *Files identical despite different names*

