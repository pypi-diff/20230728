# Comparing `tmp/remotemanager-0.9.6.tar.gz` & `tmp/remotemanager-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.6.tar", last modified: Thu Jul 27 15:22:59 2023, max compression
+gzip compressed data, was "remotemanager-0.9.7.tar", last modified: Fri Jul 28 13:16:39 2023, max compression
```

## Comparing `remotemanager-0.9.6.tar` & `remotemanager-0.9.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 15:22:59.005945 remotemanager-0.9.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-27 12:24:05.000000 remotemanager-0.9.6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-27 12:24:05.000000 remotemanager-0.9.6/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.6/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:10.000000 remotemanager-0.9.6/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.6/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:57.000000 remotemanager-0.9.6/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    55330 2023-07-27 14:22:14.000000 remotemanager-0.9.6/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-26 09:18:44.000000 remotemanager-0.9.6/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.6/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    23093 2023-07-26 09:18:44.000000 remotemanager-0.9.6/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.6/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:27.000000 remotemanager-0.9.6/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.6/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.6/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.6/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.6/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.6/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.6/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.6/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.6/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:31.000000 remotemanager-0.9.6/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:27.000000 remotemanager-0.9.6/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.6/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.6/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:22:59.005945 remotemanager-0.9.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-28 13:16:39.780554 remotemanager-0.9.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-28 12:51:04.000000 remotemanager-0.9.7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.772554 remotemanager-0.9.7/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-28 12:51:04.000000 remotemanager-0.9.7/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.7/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:10.000000 remotemanager-0.9.7/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.7/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.7/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:57.000000 remotemanager-0.9.7/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    55665 2023-07-28 12:51:04.000000 remotemanager-0.9.7/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10839 2023-07-28 11:41:58.000000 remotemanager-0.9.7/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.7/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    23111 2023-07-28 11:41:58.000000 remotemanager-0.9.7/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.7/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:27.000000 remotemanager-0.9.7/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.776554 remotemanager-0.9.7/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.7/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.7/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.7/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.7/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.7/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.7/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.7/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.7/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.7/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:31.000000 remotemanager-0.9.7/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:27.000000 remotemanager-0.9.7/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.780554 remotemanager-0.9.7/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.7/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.7/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.7/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:16:39.772554 remotemanager-0.9.7/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-28 13:16:39.000000 remotemanager-0.9.7/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 13:16:39.780554 remotemanager-0.9.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.7/setup.py
```

### Comparing `remotemanager-0.9.6/LICENSE` & `remotemanager-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/PKG-INFO` & `remotemanager-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.6
+Version: 0.9.7
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.6/README.md` & `remotemanager-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/pyproject.toml` & `remotemanager-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.6"
+current_version = "0.9.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.6/remotemanager/connection/cmd.py` & `remotemanager-0.9.7/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/computers/base.py` & `remotemanager-0.9.7/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/computers/example.py` & `remotemanager-0.9.7/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/computers/options.py` & `remotemanager-0.9.7/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.7/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/testing_object.py` & `remotemanager-0.9.7/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/connection/url.py` & `remotemanager-0.9.7/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/dataset/dataset.py` & `remotemanager-0.9.7/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -770,15 +770,20 @@
                 runner.jobscript.__getattribute__(target),
                 runner.runfile.__getattribute__(target),
                 runner.resultfile.__getattribute__(target),
                 runner.errorfile.__getattribute__(target),
             ]
 
             # need extra files, within their remote/local dir
-            for file in runner.extra_files["send"] + runner.extra_files["recv"]:
+            extras = runner.extra_files["recv"]
+            if remote_check:
+                for file in runner.extra_files["send"]:
+                    extras.append(os.path.split(file)[-1])
+
+            for file in extras:
                 targets.append(f"{runner.__getattribute__(fld)}/{file}")
 
         # minimize length
         targets = list(set(targets))
 
         return targets
 
@@ -838,14 +843,16 @@
                 except FileNotFoundError:
                     self._logger.debug(f"{local} not found")
 
         else:
             self._logger.debug("file only wipe")
             targets = self.collect_files(remote_check=False)
 
+            self._logger.info(f"targets for wipe:|{format_iterable(targets)}")
+
             if dry_run:
                 for local in targets:
                     print(f"targeting local {local} for wipe")
 
             for path in targets:
                 try:
                     os.remove(path)
@@ -897,14 +904,16 @@
 
             self.url.cmd(cmd)
 
         else:
             self._logger.debug("file only wipe")
             targets = self.collect_files(remote_check=True)
 
+            self._logger.info(f"targets for wipe:|{format_iterable(targets)}")
+
             cmd = ",".join(targets)
             cmd = f"rm -f {{{cmd}}}"
 
             if dry_run:
                 for remote in targets:
                     print(f"targeting remote {remote} for wipe")
                 return
@@ -1338,27 +1347,27 @@
             # relpath to the jobscript
             jobscript = runner.jobscript.relative_remote_path(
                 self.master_script.remote_dir
             )
             jobpath, jobfile = os.path.split(jobscript)
             # relpath to target error file
             errorpath = runner.errorfile.relative_remote_path(runner.remote_dir)
-            runline = []
+            runline = [
+                f'sed -i "s#{runner.short_uuid}_master#$sourcedir#" {jobfile} &&'
+            ]
             if runner.remote_dir != runner.run_path:
                 runline.append(f"mkdir -p {runner.run_dir} &&")
 
             runline.append(f"{submitter} {jobfile} " f"2>> {errorpath}")
 
             # get relative path to jobscript, but we must cd into it to stop any
             # run_dirs being created in the wrong remote
             if self.remote_dir != runner.remote_dir:
                 runline.insert(0, f"cd {jobpath} && ")
 
-            runline.append(f"$sourcedir/{self.repofile.name}")
-
             asynchronous = runner._run_args_temp["asynchronous"]
             if asynchronous and submitter == "bash":
                 self._logger.debug('appending "&" for async run')
                 runline.append("&")
 
             for file in runner.extra_files["send"]:
                 self.transport.queue_for_push(
```

### Comparing `remotemanager-0.9.6/remotemanager/dataset/dependency.py` & `remotemanager-0.9.7/remotemanager/dataset/dependency.py`

 * *Files 6% similar despite different names*

```diff
@@ -219,23 +219,30 @@
         global_extra = []
         for ds in ds_store:
             if ds._global_run_extra is not None:
                 global_extra.append(ds._global_run_extra)
 
         # and now a master script to kick off the chains
         # we need the export for ALL datasets
-        master_content = []
+        master_content = ["sourcedir=$PWD"]
+        # update the master targets for ALL runners
+        for ds in ds_store:
+            for runner in ds.runners:
+                master_content.append(
+                    f'sed -i "s#{runner.short_uuid}_master#$sourcedir#" '
+                    f"{runner.jobscript.name}"
+                )
 
         for ds in ds_store:
             # reuse the store as a list of runner uuids for runners_to_update
             ds_store[ds] = []
             for runner in ds.runners:
                 ready = runner.stage(
                     python=ds.url.python,
-                    repo=f"${first.main_dir_env}/{first.repofile.name}",
+                    repo=first.repofile.name,
                     global_extra="\n".join(global_extra),
                     extra=extra,
                     **run_args,
                 )
                 if not ready:
                     continue
 
@@ -244,15 +251,18 @@
                 if ds == first:
                     submitter = ds.url.submitter
                     jobscript = runner.jobscript.relative_remote_path(
                         ds.master_script.remote_dir
                     )
                     jobpath, jobfile = os.path.split(jobscript)
                     errorpath = runner.errorfile.relative_remote_path(runner.remote_dir)
-                    runline = []
+                    runline = [
+                        f'sed -i "s#{runner.short_uuid}_master#$sourcedir#" '
+                        f"{jobfile} &&"
+                    ]
                     if runner.remote_dir != runner.run_path:
                         runline.append(f"mkdir -p {runner.run_dir} &&")
 
                     runline.append(f"{submitter} {jobfile} " f"2>> {errorpath}")
 
                     if ds.remote_dir != runner.remote_dir:
                         runline.insert(0, f"cd {jobpath} && ")
```

### Comparing `remotemanager-0.9.6/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.7/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/dataset/runner.py` & `remotemanager-0.9.7/remotemanager/dataset/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,22 +505,22 @@
             argline = f'kwargs = repo.load("' f'{path}")'
         else:
             argline = f"kwargs = {self.args}"
 
         # python file writing
         # if repo is not overidden by a dependency, generate the import path here
         if repo is None:
-            repo = f"${self.parent.main_dir_env}/{self.parent.repofile.name}"
+            repo = self.parent.repofile.name
 
         errorpath = self.errorfile.relative_remote_path(self.run_path)
         dir_env_name = f"DIR_{self.short_uuid}"
         # script proper
         runscript = [
             f"import importlib.util, os",
-            f"path = os.path.expandvars('${dir_env_name}')",
+            f"path = os.path.expandvars('${dir_env_name}/{repo}')",
             f"runtime = os.path.getmtime(path)",
             f"spec = importlib.util.spec_from_file_location('repo', path)",
             f"repo = importlib.util.module_from_spec(spec)",
             f"spec.loader.exec_module(repo)\n",
             argline,
             f"result = repo.{self.parent.function.name}(**kwargs)",
             f"# if the error file mtime (created at run) has changed, don't output",
@@ -545,22 +545,22 @@
             tmp.append(self.extra)
         if extra is not None:
             tmp.append(extra)
 
         if self.run_path != self.remote_dir:
             self._logger.debug("run dir is separate to remote dir, appending extras")
             submit = (
-                f"export {dir_env_name}=$1\n"
+                f"export {dir_env_name}={self.short_uuid}_master\n"
                 f"pydir=$PWD\n"
                 f"cd {self.run_dir} && "
                 f"{python} ${{pydir}}/{self.runfile.name} 2>> {errorpath}"
             )
         else:
             submit = (
-                f"export {dir_env_name}=$1\n"
+                f"export {dir_env_name}={self.short_uuid}_master\n"
                 f"{python} {self.runfile.name} 2>> {errorpath}"
             )
             self._logger.debug(f"directly using script {submit}")
         # append the submission lines
         tmp.append(submit)
         # if this runner has children, append the lines to submit them
         for line in self._dependency_info.get("child_submit", []):
```

### Comparing `remotemanager-0.9.6/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.7/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/jupyter/magic.py` & `remotemanager-0.9.7/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/logging/__init__.py` & `remotemanager-0.9.7/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/logging/log.py` & `remotemanager-0.9.7/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/logging/utils.py` & `remotemanager-0.9.7/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/logging/verbosity.py` & `remotemanager-0.9.7/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.7/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/serialisation/serial.py` & `remotemanager-0.9.7/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.7/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.7/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/storage/database.py` & `remotemanager-0.9.7/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/storage/function.py` & `remotemanager-0.9.7/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.7/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.7/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.7/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/transport/cp.py` & `remotemanager-0.9.7/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/transport/rsync.py` & `remotemanager-0.9.7/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/transport/scp.py` & `remotemanager-0.9.7/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/transport/transport.py` & `remotemanager-0.9.7/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/utils/__init__.py` & `remotemanager-0.9.7/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/utils/flags.py` & `remotemanager-0.9.7/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager/utils/version.py` & `remotemanager-0.9.7/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.6/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.7/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.6
+Version: 0.9.7
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.6/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.7/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

