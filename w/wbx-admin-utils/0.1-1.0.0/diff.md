# Comparing `tmp/wbx-admin-utils-0.1.tar.gz` & `tmp/wbx-admin-utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbx-admin-utils-0.1.tar", last modified: Thu Jul 27 17:29:15 2023, max compression
+gzip compressed data, was "wbx-admin-utils-1.0.0.tar", last modified: Fri Jul 28 15:51:08 2023, max compression
```

## Comparing `wbx-admin-utils-0.1.tar` & `wbx-admin-utils-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 stcohen    (501) staff       (20)        0 2023-07-27 17:29:15.345878 wbx-admin-utils-0.1/
--rw-r--r--   0 stcohen    (501) staff       (20)      254 2023-07-27 17:29:15.345759 wbx-admin-utils-0.1/PKG-INFO
--rw-r--r--   0 stcohen    (501) staff       (20)       38 2023-07-27 17:29:15.345919 wbx-admin-utils-0.1/setup.cfg
--rw-r--r--   0 stcohen    (501) staff       (20)      345 2023-07-27 17:28:58.000000 wbx-admin-utils-0.1/setup.py
--rw-r--r--   0 stcohen    (501) staff       (20)     5589 2023-07-27 14:33:32.000000 wbx-admin-utils-0.1/wbx-user-groups.py
-drwxr-xr-x   0 stcohen    (501) staff       (20)        0 2023-07-27 17:29:15.345595 wbx-admin-utils-0.1/wbx_admin_utils.egg-info/
--rw-r--r--   0 stcohen    (501) staff       (20)      254 2023-07-27 17:29:15.000000 wbx-admin-utils-0.1/wbx_admin_utils.egg-info/PKG-INFO
--rw-r--r--   0 stcohen    (501) staff       (20)      183 2023-07-27 17:29:15.000000 wbx-admin-utils-0.1/wbx_admin_utils.egg-info/SOURCES.txt
--rw-r--r--   0 stcohen    (501) staff       (20)        1 2023-07-27 17:29:15.000000 wbx-admin-utils-0.1/wbx_admin_utils.egg-info/dependency_links.txt
--rw-r--r--   0 stcohen    (501) staff       (20)       16 2023-07-27 17:29:15.000000 wbx-admin-utils-0.1/wbx_admin_utils.egg-info/top_level.txt
+drwxr-xr-x   0 stcohen    (501) staff       (20)        0 2023-07-28 15:51:08.830675 wbx-admin-utils-1.0.0/
+-rw-r--r--   0 stcohen    (501) staff       (20)      958 2023-07-28 15:51:08.830546 wbx-admin-utils-1.0.0/PKG-INFO
+-rw-r--r--   0 stcohen    (501) staff       (20)      520 2023-07-28 11:35:28.000000 wbx-admin-utils-1.0.0/README.md
+-rw-r--r--   0 stcohen    (501) staff       (20)      607 2023-07-28 14:10:19.000000 wbx-admin-utils-1.0.0/pyproject.toml
+-rw-r--r--   0 stcohen    (501) staff       (20)       38 2023-07-28 15:51:08.830716 wbx-admin-utils-1.0.0/setup.cfg
+drwxr-xr-x   0 stcohen    (501) staff       (20)        0 2023-07-28 15:51:08.830029 wbx-admin-utils-1.0.0/wbx_admin_utils.egg-info/
+-rw-r--r--   0 stcohen    (501) staff       (20)      958 2023-07-28 15:51:08.000000 wbx-admin-utils-1.0.0/wbx_admin_utils.egg-info/PKG-INFO
+-rw-r--r--   0 stcohen    (501) staff       (20)      180 2023-07-28 15:51:08.000000 wbx-admin-utils-1.0.0/wbx_admin_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 stcohen    (501) staff       (20)        1 2023-07-28 15:51:08.000000 wbx-admin-utils-1.0.0/wbx_admin_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 stcohen    (501) staff       (20)        1 2023-07-28 15:51:08.000000 wbx-admin-utils-1.0.0/wbx_admin_utils.egg-info/top_level.txt
```

