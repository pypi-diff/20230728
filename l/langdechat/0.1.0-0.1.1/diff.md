# Comparing `tmp/langdechat-0.1.0.tar.gz` & `tmp/langdechat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdechat-0.1.0.tar", last modified: Thu Jul 27 23:17:33 2023, max compression
+gzip compressed data, was "langdechat-0.1.1.tar", last modified: Fri Jul 28 08:52:13 2023, max compression
```

## Comparing `langdechat-0.1.0.tar` & `langdechat-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:17:33.107608 langdechat-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-27 23:17:33.107608 langdechat-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 03:04:42.000000 langdechat-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:17:33.107608 langdechat-0.1.0/langdechat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 03:06:16.000000 langdechat-0.1.0/langdechat/__init__.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-27 23:06:10.000000 langdechat-0.1.0/langdechat/module1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 23:17:33.107608 langdechat-0.1.0/langdechat.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-27 23:17:33.000000 langdechat-0.1.0/langdechat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-27 23:17:33.000000 langdechat-0.1.0/langdechat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 23:17:33.000000 langdechat-0.1.0/langdechat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-27 23:17:33.000000 langdechat-0.1.0/langdechat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-27 23:17:33.000000 langdechat-0.1.0/langdechat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 23:17:33.107608 langdechat-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-27 23:12:45.000000 langdechat-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:52:13.806079 langdechat-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 23:42:49.000000 langdechat-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 08:52:13.806079 langdechat-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 03:04:42.000000 langdechat-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:52:13.806079 langdechat-0.1.1/langdechat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 03:06:16.000000 langdechat-0.1.1/langdechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-28 08:34:13.000000 langdechat-0.1.1/langdechat/langeval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 08:52:13.806079 langdechat-0.1.1/langdechat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-28 08:52:13.000000 langdechat-0.1.1/langdechat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-28 08:52:13.000000 langdechat-0.1.1/langdechat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 08:52:13.000000 langdechat-0.1.1/langdechat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-28 08:52:13.000000 langdechat-0.1.1/langdechat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-28 08:52:13.000000 langdechat-0.1.1/langdechat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 08:52:13.806079 langdechat-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-28 08:50:09.000000 langdechat-0.1.1/setup.py
```

