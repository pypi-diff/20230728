# Comparing `tmp/aio_dt_protocol-1.1.1.tar.gz` & `tmp/aio_dt_protocol-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-1.1.1.tar", last modified: Wed Jun  7 06:21:54 2023, max compression
+gzip compressed data, was "aio_dt_protocol-1.2.0.tar", last modified: Fri Jul 28 18:21:24 2023, max compression
```

## Comparing `aio_dt_protocol-1.1.1.tar` & `aio_dt_protocol-1.2.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:54.130775 aio_dt_protocol-1.1.1/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     8670 2023-06-07 06:21:54.131773 aio_dt_protocol-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7926 2023-06-07 06:11:50.000000 aio_dt_protocol-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.541980 aio_dt_protocol-1.1.1/aio_dt_protocol/
--rw-rw-rw-   0        0        0      503 2023-06-07 06:18:44.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/__init__.py
--rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/actions.py
--rw-rw-rw-   0        0        0    56559 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/browser.py
--rw-rw-rw-   0        0        0    16933 2023-06-07 06:00:16.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/connection.py
--rw-rw-rw-   0        0        0    25804 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/data.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.558974 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.571970 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/
--rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/background_service.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.584966 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/__init__.py
--rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/browser.py
--rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.608958 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/__init__.py
--rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/css.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.621952 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/
--rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/__init__.py
--rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/device_orientation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.663937 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/
--rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/__init__.py
--rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom.py
--rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom_element.py
--rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.683930 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/
--rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/__init__.py
--rw-rw-rw-   0        0        0    24489 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/emulation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.709921 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/
--rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/__init__.py
--rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/fetch.py
--rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.750906 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/
--rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/__init__.py
--rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/input.py
--rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.763901 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/log.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.786893 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/__init__.py
--rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/network.py
--rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.819882 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/overlay.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.849871 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/
--rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/__init__.py
--rw-rw-rw-   0        0        0    33682 2023-05-24 16:56:23.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/page.py
--rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.901852 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/__init__.py
--rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/runtime.py
--rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.920846 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/
--rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/system_info.py
--rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/types.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:54.128773 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/
--rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/__init__.py
--rw-rw-rw-   0        0        0    17276 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/target.py
--rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/types.py
--rw-rw-rw-   0        0        0     3753 2023-05-26 18:01:07.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     9252 2023-06-07 06:00:16.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/extend_connection.py
--rw-rw-rw-   0        0        0     5683 2023-05-27 18:33:35.000000 aio_dt_protocol-1.1.1/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:21:53.557976 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     8670 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2504 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-07 06:21:53.000000 aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 06:21:54.133772 aio_dt_protocol-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8069 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7302 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.894969 aio_dt_protocol-1.2.0/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      503 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    56344 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    17231 2023-07-28 18:01:34.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    25802 2023-07-28 10:14:12.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.900966 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.903965 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.906964 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.909963 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.911963 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.915961 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.918960 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    24981 2023-07-04 09:40:58.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.921959 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.924958 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.927957 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.930956 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.933955 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.936954 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    32632 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.939953 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.942952 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    16832 2023-07-25 17:35:03.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     4207 2023-07-28 15:07:56.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     9483 2023-07-03 05:36:05.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0    12324 2023-07-09 14:14:30.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/js.py
+-rw-rw-rw-   0        0        0     7136 2023-07-28 15:10:54.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.899967 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     8069 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:21:24.946950 aio_dt_protocol-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-07-28 15:29:36.000000 aio_dt_protocol-1.2.0/setup.py
```

### Comparing `aio_dt_protocol-1.1.1/LICENSE` & `aio_dt_protocol-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/PKG-INFO` & `aio_dt_protocol-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,74 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 1.1.1
+Version: 1.2.0
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/markdown
+Provides-Extra: ujson
 License-File: LICENSE
 
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
 Запуски проводятся только в ОС Windows и Linux.
 
-### Установка
-```shell
-pip install aio-dt-protocol
-```
-
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
+### Установка
+```shell
+pip install aio-dt-protocol
+```
+Или установить сразу вместе с [ujson](https://github.com/ultrajson/ultrajson)
+```shell
+pip install aio-dt-protocol[ujson]
+```
+
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
 from aio_dt_protocol import BrowserName
-from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
-    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
-    # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=PROFILE_NAME
-        )
-        msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
-
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.waitFirstTab(callback=action_printer)
-    conn = await browser.waitFirstTab()
-
+    # browser, conn = await Browser.run(callback=action_printer)
+    
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    # ? Иначе, запуск нового браузера.
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=PROFILE_NAME
+    )
+    
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
     
     # ? Эмуляция клика в поисковую строку
@@ -110,15 +105,15 @@
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
 1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
 2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
 
-Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции(слушателя), после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -156,37 +151,29 @@
     await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser, BrowserName, find_instances
+from aio_dt_protocol import Browser, BrowserName
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
     # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=""
-        )
-        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=""
+    )
     
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
```

### Comparing `aio_dt_protocol-1.1.1/README.md` & `aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,74 @@
+Metadata-Version: 2.1
+Name: aio-dt-protocol
+Version: 1.2.0
+Summary: Asynchronous wrapper over Chromium browser debugger protocol.
+Home-page: https://github.com/PieceOfGood/aio_dt_protocol
+Author: PieceOfGood
+Author-email: 78sanchezz@gmail.com
+License: BSD 3-Clause
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Description-Content-Type: text/markdown
+Provides-Extra: ujson
+License-File: LICENSE
+
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
 Запуски проводятся только в ОС Windows и Linux.
 
-### Установка
-```shell
-pip install aio-dt-protocol
-```
-
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
+### Установка
+```shell
+pip install aio-dt-protocol
+```
+Или установить сразу вместе с [ujson](https://github.com/ultrajson/ultrajson)
+```shell
+pip install aio-dt-protocol[ujson]
+```
+
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
 from aio_dt_protocol import BrowserName
-from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
-    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
-    # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=PROFILE_NAME
-        )
-        msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
-
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.waitFirstTab(callback=action_printer)
-    conn = await browser.waitFirstTab()
-
+    # browser, conn = await Browser.run(callback=action_printer)
+    
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    # ? Иначе, запуск нового браузера.
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=PROFILE_NAME
+    )
+    
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
     
     # ? Эмуляция клика в поисковую строку
@@ -91,15 +105,15 @@
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
 1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
 2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
 
-Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции(слушателя), после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -137,37 +151,29 @@
     await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser, BrowserName, find_instances
+from aio_dt_protocol import Browser, BrowserName
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
     # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=""
-        )
-        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=""
+    )
     
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
@@ -179,8 +185,8 @@
     await conn.Browser.close()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 
-```
+```
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/actions.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/browser.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,51 @@
 from inspect import iscoroutinefunction
 from typing import List, Dict, Union, Optional, Tuple, Literal
 from collections.abc import Sequence
 from enum import Enum
 from .connection import Connection
 from .data import TargetConnectionInfo, TargetConnectionType, CommonCallback
 from .exceptions import FlagArgumentContainError, NoTargetWithGivenIdFound
-from .utils import get_request, find_browser_executable_path, log, async_util_call
+from .utils import (
+    get_request,
+    find_browser_executable_path,
+    log,
+    async_util_call,
+    find_instances,
+    prepare_url
+)
 
 
 class Browser:
 
+    @classmethod
+    async def run(
+            cls,
+            debug_port: int = 9222,
+            browser_name: str = "chrome",
+            callback: CommonCallback = None,
+            **options
+    ) -> Tuple["Browser", "Connection"]:
+        if browser_instances := find_instances(debug_port, browser_name):
+            browser = Browser(debug_port=debug_port, browser_pid=browser_instances[debug_port])
+            running_state = "CONNECT TO EXISTING BROWSER"
+        else:
+            browser = Browser(
+                debug_port=debug_port,
+                browser_exe=browser_name,
+                **options
+            )
+            running_state = "CREATE NEW BROWSER"
+
+        if options.get("verbose"):
+            log(running_state)
+
+        return browser, await browser.waitFirstTab(callback=callback)
+
+
     def __init__(
             self,
             profile_path: str = "testProfile",
             dev_tool_profiles:  bool = False,
             url: Optional[Union[str, bytes]] = None,
             flags:  Optional["FlagBuilder"] = None,
             browser_path: str = "",
@@ -56,15 +88,21 @@
 
         :param dev_tool_profiles:   Если 'profile_path' указан как имя папки, а не путь,
                                     профиль с указанным именем будет создан/получен в домашней
                                     директории пользователя, из каталога 'DevTools_Profiles',
                                     если значение установлено в True. (Linux, Windows)
 
         :param url:             Адрес, которым будет инициирован старт браузера.
-                                    Со значением по умолчанию, будет открыта пустая страница.
+                                    Со значением по умолчанию, будет открыта дефолтная страница.
+                                    Пустая строка откроет пустую страницу(about:blank).
+                                    Может принимать HTML-разметку, как в виде строки, так и в
+                                    наборе байт при конвертировании в base64. Поскольку subprocess
+                                    имеет ограничения на длину принимаемых параметров, слишком
+                                    длинная строка приведёт к краху.
+                                    https://stackoverflow.com/questions/2381241/what-is-the-subprocess-popen-max-length-of-the-args-parameter
 
         :param flags:           Экземпляр `FlagBuilder()` напичканный `CMDFlags()`.
                                     https://peter.sh/experiments/chromium-command-line-switches/
 
         :param browser_path:    Путь до исполняемого файла браузера. Имеет приоритет над
                                     аргументом `browser_exe`.
 
@@ -182,44 +220,22 @@
         # https://stackoverflow.com/questions/2381241/what-is-the-subprocess-popen-max-length-of-the-args-parameter
         # data_url_len_is_high = len(url[0]) > 32_767
         data_url_len = len(url) if url else 0
         # print("url =", url)
         if data_url_len > 30_000:
             warnings.warn(f"Length data url ({data_url_len}) is approaching to critical length = 32767 symbols!")
 
-        b_name_len = len(self.browser_name)
-        # Если "app" == True:
-        _url_ = (
-            # открыть dataURL без содержимого, если в "url" ничего не передано
-            "--app=data:text/html," if url is None else
-                # иначе установить переданную разметку, если она пришла как строка
-                # и начало этой строки не содержит признаков url-адреса
-                "--app=data:text/html," + quote(url)
-                    if type(url) is str and "http" != url[:4] and self.browser_name != url[:b_name_len] else "--app=" + url
-                        # передать "как есть", раз это строка содержащая url
-                        if type(url) is str and "http" == url[:4] or self.browser_name == url[:b_name_len] else
-                            # иначе декодировать и установить её как Base64
-                            "--app=data:text/html;Base64," + url.decode()
-
-            # иначе, открыть пустую страницу, если в "url" ничего не передано
-        ) if app else "about:blank" if url is None else (
-            # иначе передать разметку как data-url, если начало этой строки
-            # не содержит признаков url-адреса
-            "data:text/html," + quote(url)
-                if type(url) is str and "http" != url[:4] and self.browser_name != url[:b_name_len] else url
-                    # или передать "как есть", раз это строка содержащая url
-                    if type(url) is str and "http" == url[:4] or self.browser_name == url[:b_name_len] else
-                        # иначе декодировать и установить её как Base64
-                        "data:text/html;Base64," + url.decode()
-        )
+        url = prepare_url(url, self.browser_name, app)
 
         self.is_headless_mode = False
-        self.browser_pid = browser_pid if browser_pid > 0 else self._run_browser(_url_, flags, position, sizes)
+        self.browser_pid = browser_pid if browser_pid > 0 else self._run_browser(url, flags, position, sizes)
 
-    def _run_browser(self, url: str, flags: "FlagBuilder", position: Optional[Tuple[int, int]] = None,
+    def _run_browser(self, url: Optional[str] = None,
+                     flags: Optional["FlagBuilder"] = None,
+                     position: Optional[Tuple[int, int]] = None,
                      sizes: Optional[Tuple[int, int]] = None) -> int:
         """
         Запускает браузер с переданными флагами.
         :param url:             Адрес. Если передан, будет загружен в первой вкладке.
         :param flags:           Флаги
         :return:                ProcessID запущенного браузера
         """
@@ -237,15 +253,16 @@
             (CMDFlags.Performance.disable_gpu_shader_disk_cache, []),
             (CMDFlags.Performance.disk_cache_dir, ["null"]),
             (CMDFlags.Performance.media_cache_dir, ["null"]),
             (CMDFlags.Render.enable_features_WebUIDarkMode, []),
             (CMDFlags.Render.force_dark_mode, []),
         )
         run_args = [ self.browser_path ]
-        flag_box.custom(url)
+        if url:
+            flag_box.custom(url)
 
         # ! Default mode
         if self.profile_path:
             flag_box.add(CMDFlags.Common.user_data_dir, self.profile_path)
             if position is not None:
                 flag_box.add(CMDFlags.Screen.window_position, *position)
             if sizes is not None:
@@ -309,15 +326,15 @@
                     "url": "https://www.yahoo.com/",
                     "webSocketDebuggerUrl": "ws://localhost:9222/devtools/page/DAB7FB6187B554E10B0BD18821265734"
                 }, { ... } ]
         """
         result = await async_util_call(
             get_request, f"http://127.0.0.1:{self.debug_port}/json/list")
 
-        if self.verbose: log("GetPageList() => " + result)
+        if self.verbose: log("getPageList() => " + result)
         return json.loads(result)
 
     async def getConnectionBy(
             self, key: Union[str, int],
             value: Union[str, int],
             match_mode: Literal["exact", "contains", "startswith"] = "exact",
             index: int = 0,
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/connection.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,22 +169,25 @@
 
         await self._send(json.dumps(data))
 
         response = await receiver.recv()
         if "error" in response:
 
             if ex := get_cdtp_error((e := response['error'])['message']):
-                raise ex(f"domain_and_method = '{domain_and_method}' | params = '{str(params)}'")
+                raise ex(
+                    f"\n\t\x1b[37mdomain_and_method: '\x1b[91m{domain_and_method}\x1b[37m'"
+                    f"\n\tparams: '\x1b[91m{str(params)}\x1b[37m'\x1b[0m"
+                )
 
             raise Exception(
-                "\x1b[36mBrowser detect error:\n" +
-                f"\x1b[37mError code: '\x1b[91m{e['code']}\n" +
-                f"\x1b[37mError message: '\x1b[91m{e['message']}\n" +
-                f"\x1b[37mdomain_and_method: '\x1b[91m{domain_and_method}\n" +
-                f"\x1b[37mparams: '\x1b[91m{params}\x1b[0m\n"
+                "\x1b[36mBrowser detect error:\x1b[37m\t\n" +
+                f"Error code: '\x1b[91m{e['code']}\x1b[37m'\t\n" +
+                f"Error message: '\x1b[91m{e['message']}\x1b[37m'\t\n" +
+                f"domain_and_method: '\x1b[91m{domain_and_method}\x1b[37m'\t\n" +
+                f"params: '\x1b[91m{params}\x1b[37m'\x1b[0m"
             )
 
         return response["result"]
 
     async def _send(self, data: str) -> None:
         if self.connected:
             await self._ws_session.send(data)
@@ -192,25 +195,24 @@
     async def _recv(self) -> None:
         while self.connected:
             try:
                 data_msg: dict = json.loads(await self._ws_session.recv())
             # ! Браузер разорвал соединение
             except ConnectionClosedError as e:
                 if self.verbose: log(f"ConnectionClosedError {e!r}")
-                await self.detach()
+                await self._detach()
                 return
 
             # Ожидающие ответов вызовы API получают ответ по id входящих сообщений.
             if sender := self.responses.pop(data_msg.get("id"), None):
                 await sender.send(data_msg)
 
             if ((method := data_msg.get("method")) == "Inspector.detached"
                     and data_msg["params"]["reason"] == "target_closed"):
-                await self.detach()
-                self.on_close_event.set()
+                await self._detach()
                 return
 
             # Если коллбэк функция была определена, она будет получать все
             #   уведомления из инстанса страницы.
             if self.callback is not None:
                 asyncio.create_task(self.callback(data_msg))
 
@@ -231,31 +233,40 @@
 
             if listeners := self._listeners_for_event.get(method):
                 p = data_msg.get("params") or {}
                 for listener, largs in listeners.items():
                     asyncio.create_task(
                         listener(       # корутина
                             p,          # её "params" — всегда передаётся
-                            *largs      # список bind-агрументов
+                            *largs      # список bind-аргументов
                         )
                     )
 
-
-
     async def waitForClose(self) -> None:
         """ Дожидается, пока не будет потеряно соединение со страницей. """
+        if self.verbose: log(f"Wait wor close connection {self.conn_id}")
         await self.on_close_event.wait()
+        if self.verbose: log(f"Wait for close connection done {self.conn_id}")
 
     async def activate(self) -> None:
         self._ws_session = await connect(self.ws_url, ping_interval=None)
         self._connected = True
         self._receiver_loop = asyncio.create_task(self._recv())
         await self.Runtime.enable()
 
-    async def detach(self) -> None:
+    async def disconnect(self) -> None:
+        """ Принудительно разрывает соединение. """
+        if not self.connected:
+            return
+        if self.verbose: log(f"[ DISCONNECT ] {self.conn_id}")
+        if not self._ws_session.closed:
+            await self._ws_session.close()
+
+
+    async def _detach(self) -> None:
         """  Отключается от страницы. Вызывается автоматически при закрытии браузера,
         или текущей страницы. Принудительный вызов не закрывает страницу,
         а лишь разрывает с ней соединение.
         """
         if not self.connected:
             return
 
@@ -263,14 +274,16 @@
         if self.verbose: log(f"[ DETACH ] {self.conn_id}")
         self._connected = False
 
         if self._on_detach_listener:
             function, args, kvargs = self._on_detach_listener
             await function(*args, **kvargs)
 
+        self.on_close_event.set()
+
     def clearOnDetach(self) -> None:
         self._on_detach_listener = tuple()
 
     def setOnDetach(self, function: Callable[[any], CoroTypeNone], *args, **kvargs) -> bool:
         """  Регистрирует асинхронный коллбэк, который будет вызван с соответствующими аргументами
         при разрыве соединения со страницей.
         """
@@ -317,16 +330,14 @@
 
     async def addListenerForEvent(
         self, event: Union[str, DomainEvent], listener: Callable[[dict, tuple], CoroTypeNone], *args) -> None:
         """ Регистрирует слушателя, который будет вызываться при генерации определённых событий
         в браузере. Список таких событий можно посмотреть в разделе "Events" почти
         у каждого домена по адресу: https://chromedevtools.github.io/devtools-protocol/
         Например: 'DOM.attributeModified'
-            !Внимание! Каждый такой слушатель должен иметь один обязательный 'data'-аргумент,
-        в который будут передаваться параметры случившегося события в виде словаря(dict).
 
         :param event:           Имя события, для которого регистируется слушатель. Например:
                                     'DOM.attributeModified'.
         :param listener:        Колбэк-функция.
         :param args:            (optional) любое кол-во агрументов, которые будут переданы
                                     в функцию последними.
         :return:        None
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/data.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional, TypeVar, Generic, Tuple, Callable, Coroutine
 from dataclasses import dataclass
 from enum import Enum
 from asyncio import Queue
 
-
 CommonCallback = Optional[Callable[[dict], Coroutine[None, None, None]]]
 T = TypeVar("T")
 
 
 @dataclass
 class GeoInfo:
     ip: str
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/background_service/background_service.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/browser.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/browser/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/css/css.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/css.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/device_orientation/device_orientation.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/dom_element.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/dom/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/emulation/emulation.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,21 @@
                         scale: Optional[float] = None,
                     screenWidth: Optional[int] = None,
                    screenHeight: Optional[int] = None,
                       positionX: Optional[int] = None,
                       positionY: Optional[int] = None,
             dontSetVisibleSize: Optional[bool] = None,
              screenOrientation: Optional[dict] = None,
-                      viewport: Optional[dict] = None
+                      viewport: Optional[dict] = None,
+                displayFeature: Optional[dict] = None,
     ) -> None:
         """
-        Переопределяет значения размеров экрана устройства (результаты мультимедийного запроса CSS,
-            относящиеся к «device-width» / «device-height», связанные с window.screen.width,
-            window.screen.height, window.innerWidth, window.innerHeight).
+        Переопределяет значения размеров экрана устройства (window.screen.width, window.screen.height,
+            window.innerWidth, window.innerHeight и результаты медиа-запросов CSS, связанные с
+            "device-width"/"device-height").
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setDeviceMetricsOverride
         :param width:               Переопределяет значение ширины viewport в пикселях(от 0 до 10_000_000).
                                         window.innerWidth
                                         0 — выключает переопределение.
         :param height:              Переопределяет значение высоты viewport в пикселях(от 0 до 10_000_000).
                                         window.innerHeight
                                         0 — выключает переопределение.
@@ -142,14 +143,16 @@
                                                                 пикселях (dip).
                                             "width": float, -> Ширина прямоугольника в независимых от устройства
                                                                 пикселях (dip).
                                             "height": float,-> Высота прямоугольника в независимых от устройства
                                                                 пикселях (dip).
                                             "scale": float  -> Коэффициент масштабирования страницы.
                                         }
+        :param displayFeature:       (optional, EXPERIMENTAL) Если установлено, отображается функция многосегментного
+                                        экрана. Если не установлено, поддержка нескольких сегментов отключена.
         :return:
         """
         args = {"width": width, "height": height, "deviceScaleFactor": deviceScaleFactor, "mobile": mobile}
         if scale is not None:
             args.update({"scale": scale})
         if screenWidth is not None:
             args.update({"screenWidth": screenWidth})
@@ -161,26 +164,28 @@
             args.update({"positionY": positionY})
         if dontSetVisibleSize is not None:
             args.update({"dontSetVisibleSize": dontSetVisibleSize})
         if screenOrientation is not None:
             args.update({"screenOrientation": screenOrientation})
         if viewport is not None:
             args.update({"viewport": viewport})
+        if displayFeature is not None:
+            args.update({"displayFeature": displayFeature})
         await self._connection.call("Emulation.setDeviceMetricsOverride", args)
 
     async def setScrollbarsHidden(self, hidden: bool) -> None:
         """
         (EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setScrollbarsHidden
         :param hidden:              Должны ли полосы прокрутки быть всегда скрыты.
         :return:
         """
         await self._connection.call("Emulation.setScrollbarsHidden", {"hidden": hidden})
 
-    async def s(self, disabled: bool) -> None:
+    async def setDocumentCookieDisabled(self, disabled: bool) -> None:
         """
         (EXPERIMENTAL)
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setDocumentCookieDisabled
         :param disabled:            Должен ли API document.cookie быть отключен.
         :return:
         """
         await self._connection.call("Emulation.setDocumentCookieDisabled", {"disabled": disabled})
@@ -232,15 +237,16 @@
     async def setGeolocationOverride(
             self,
              latitude: Optional[float] = None,
             longitude: Optional[float] = None,
              accuracy: Optional[float] = None
     ) -> None:
         """
-        Переопределяет Положение или Ошибку Геолокации. Пропуск любого из параметров эмулирует положение недоступно.
+        Переопределяет Положение или Ошибку Геолокации. Пропуск любого из параметров эмулирует
+            "положение недоступно".
         https://chromedevtools.github.io/devtools-protocol/tot/Emulation#method-setGeolocationOverride
         :param latitude:            (optional) Широта.
         :param longitude:           (optional) Долгота.
         :param accuracy:            (optional) Точность.
         :return:
         """
         args = {}
@@ -365,9 +371,10 @@
             args.update({"acceptLanguage": acceptLanguage})
         if platform is not None:
             args.update({"platform": platform})
         if userAgentMetadata is not None:
             args.update({"userAgentMetadata": userAgentMetadata})
         await self._connection.call("Emulation.setUserAgentOverride", args)
 
+
 class EmulationEvent(DomainEvent):
     virtualTimeBudgetExpired = "Emulation.virtualTimeBudgetExpired"
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/fetch.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/fetch/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/input.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/input.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/input/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/log/log.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/network.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/network/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/overlay/overlay.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/page.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from urllib.parse import quote
 from typing import Optional, Union, Callable, Awaitable
 from ...data import DomainEvent
+from ...utils import prepare_url
 from .types import FrameTree, LifecycleEventData
 
 
 class Page:
     """
     #   https://chromedevtools.github.io/devtools-protocol/tot/Page
     """
@@ -85,15 +86,14 @@
         """
         Возвращает структуру присутствующих на странице фреймов. !!! Справедливо только в рамках одного домена.
         https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-getFrameTree
         """
         result = await self._connection.call("Page.getFrameTree")
         return FrameTree(**result.get("frameTree"))
 
-    # async def GetFrameFor
 
     async def handleJavaScriptDialog(self, accept: bool, promptText: str = "") -> None:
         """
         Подтверждает или закрывает диалоговое окно, инициированное JavaScript (alert, confirm,
             prompt или для onbeforeunload).
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-handleJavaScriptDialog
         :param accept:          'True' — принять, 'False' — отклонить диалог.
@@ -116,38 +116,17 @@
         https://chromedevtools.github.io/devtools-protocol/tot/Page#method-navigate
         :param url:                     Адрес, по которому происходит навигация.
         :param wait_for_load:           (optional) Если 'True' - ожидает состояния остановки
                                             загрузки ресурсов, если активны уведомления домена Page.
         :param wait_for_network_idle:   (optional) Если 'True' - ожидает прекращения активности сети
         :return:
         """
-        b_name_len = len(self._connection.browser_name)
-        is_url = (
-            "http" == url[:4] or
-            "chrome" == url[:6] or
-            self._connection.browser_name == url[:b_name_len] or
-            url == "about:blank"
-        )
+        url = prepare_url(url, self._connection.browser_name)
 
-        if self.enabled:
-            self.loading_state.clear()
-        if self.lifecycle_events_enabled:
-            self.network_idle_state.clear()
-
-        _url_ = ("data:text/html," + quote(url)
-             # передать разметку как data-url, если начало этой строки
-             # не содержит признаков url-адреса или передать "как есть",
-             if type(url) is str and not is_url else url
-                 # раз это строка содержащая url, или переход на пустую страницу
-                 if type(url) is str and is_url else
-                     # иначе декодировать и установить её как Base64
-                     "data:text/html;Base64," + url.decode()
-             )
-
-        await self._connection.call("Page.navigate", {"url": _url_})
+        await self._connection.call("Page.navigate", {"url": url})
         if wait_for_load or wait_for_network_idle:
             await self.waitForLoad(wait_for_load, wait_for_network_idle)
 
     async def waitForLoad(self, by_load_state: bool = False, by_network_idle: bool = True) -> None:
         """ Дожидается указанного состояния.
         :param by_load_state:       Ожидать завершения загрузки страницы.
         :param by_network_idle:     Ожидать завершения активности сети.
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/page/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/runtime.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/runtime/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/system_info.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/system_info.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/system_info/types.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/domains/target/target.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,22 +88,14 @@
         Возвращает список 'targetInfo' о доступных 'targets'.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-getTargets
         :return:                [ targetInfo, targetInfo, ... ]
         """
         result = (await self._connection.call("Target.getTargets"))["targetInfos"]
         return [TargetInfo(**info) for i, info in enumerate(result)]
 
-    async def attachToBrowserTarget(self) -> str:
-        """
-        Присоединяется к target браузера, использует только режим flat sessionId.
-        https://chromedevtools.github.io/devtools-protocol/tot/Target#method-attachToBrowserTarget
-        :return:                    sessionId
-        """
-        return (await self._connection.call("Target.attachToBrowserTarget"))["sessionId"]
-
     async def attachToTarget(self, targetId: str, flatten: Optional[bool] = None) -> str:
         """
         Присоединяется к 'target' по указанному 'targetId'.
         https://chromedevtools.github.io/devtools-protocol/tot/Target#method-attachToTarget
         :param targetId:        Строка, представляющая идентификатор созданной страницы.
         :param flatten:         (optional) Разрешает "flat" доступ к сеансу с помощью указания атрибута
                                     sessionId в командах.
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,34 +37,46 @@
 
 class NoScriptWithGivenId(MyBaseException): pass
 
 class UniqueContextIdNotFound(MyBaseException): pass
 
 class InvalidRemoteObjectId(MyBaseException): pass
 
+class NotAllowedError(MyBaseException): pass
+
 class AnotherLocaleOverrideIsAlreadyInEffect(MyBaseException): pass     # ! при установке той же локали
 
 class FontFamiliesCanOnlyBeSetOnce(MyBaseException): pass               # ! при установке тех же шрифтов
 
 class GetRequestBodyBeforeRequestReceived(MyBaseException): pass        # ! получение тела до получения ответа
 
+class NoSessionWithGivenId(MyBaseException): pass        # !
+
+class NoSessionForGivenTargetId(MyBaseException): pass        # !
+
+class InvalidURLError(MyBaseException): pass        # !
+
 
 exception_store = {
     "Target crashed": TargetCrashed,
     "Position out of bounds": PositionOutOfBounds,
     "Could not find node with given id": CouldNotFindNodeWithGivenID,
     "Could not compute content quads": CouldNotComputeContentQuads,
     "No dialog is showing": NoDialogIsShowing,
     "No target with given id found": NoTargetWithGivenIdFound,
     "No script with given id": NoScriptWithGivenId,
     "uniqueContextId not found": UniqueContextIdNotFound,
     "Invalid remote object id": InvalidRemoteObjectId,
+    "Not allowed": NotAllowedError,
     "Another locale override is already in effect": AnotherLocaleOverrideIsAlreadyInEffect,
     "Font families can only be set once": FontFamiliesCanOnlyBeSetOnce,
     "Can only get response body on requests captured after headers received": GetRequestBodyBeforeRequestReceived,
+    "No session with given id": NoSessionWithGivenId,
+    "No session for given target id": NoSessionForGivenTargetId,
+    "Cannot navigate to invalid URL": InvalidURLError,
 }
 
 
 def get_cdtp_error(error_text: str) -> Optional[Type[MyBaseException]]:
     for title, ex in exception_store.items():
         if title in error_text:
             return ex
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/extend_connection.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/extend_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import base64, re
 from typing import Optional
 
 from .exceptions import EvaluateError, JavaScriptError, NullProperty
 
 
 class Extend:
-    """ Расширение для 'Page' некоторыми полезными методами.
+    """ Расширение для 'Connection' некоторыми полезными методами.
     """
     __slots__ = ("_connection", "action", "_py_call_script_id")
 
     def __init__(self, conn) -> None:
 
         from .connection import Connection
 
@@ -86,17 +86,17 @@
         return (await self._connection.Target.getTargetInfo()).url
 
     async def getTitle(self) -> str:
         return (await self._connection.Target.getTargetInfo()).title
 
     async def makeScreenshot(
             self,
-                 format_: str = "",
-                 quality: int = -1,
-                   clip: Optional[dict] = None,
+            format_: str = "",
+            quality: int = -1,
+            clip: Optional[dict] = None,
             fromSurface: bool = True
     ) -> bytes:
         """  Сделать скриншот. Возвращает набор байт, представляющий скриншот.
         :param format_:         jpeg или png (по умолчанию png).
         :param quality:         Качество изображения в диапазоне [0..100] (только для jpeg).
         :param clip:            {
                                     "x": "number => X offset in device independent pixels (dip).",
@@ -145,15 +145,18 @@
             returnByValue=False,
             generatePreview=False
         )
 
         return json.loads(response.value)
 
     async def injectJS(self, expression: str) -> any:
-        """ Выполняет JavaScript-выражение во фрейме верхнего уровня. """
+        """ Выполняет JavaScript-выражение во фрейме верхнего уровня.
+        Возвращает только простые типы в естественном виде, для сложных
+        используйте сериализацию в JSON, или evaluate() домена Runtime.
+        """
         try:
             response = await self._connection.Runtime.evaluate(
                 expression=expression,
                 objectGroup="console",
                 includeCommandLineAPI=True,
                 silent=False,
                 returnByValue=False,
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.2.0/aio_dt_protocol/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import subprocess
 import re
 import sys
 import urllib.request
-from typing import Optional, Dict, Callable
+from pathlib import Path
+from typing import Optional, Dict, Callable, Union
+from urllib.parse import quote
 
 
 def get_request(url: str) -> str:
     with urllib.request.urlopen(url) as response:
         return response.read().decode('utf-8')
 
 
 def find_browser_executable_path(exe="chrome") -> str:
     """ Возвращает путь до EXE. """
     if not sys.platform == "win32":
-        raise OSError("registry_read_key() is only available on Windows")
+        raise OSError("find_browser_executable_path() is only available on Windows")
 
     if exe == "chromium":
         import os
         from pathlib import Path
 
         app_data = Path(os.getenv('APPDATA')).parent
         browser_path = app_data / "Local/Chromium/Application/chrome.exe"
@@ -38,26 +40,27 @@
     return result
 
 
 def log(data: any = "", lvl: str = "[<- V ->]", eol: str = "\n") -> None:
     print(f"\x1b[32m{lvl} \x1b[38m\x1b[3m{data}\x1b[0m", end=eol)
 
 
-def save_img_as(path: str, data: bytes) -> None:
-    """ Сохраняет по пути 'path' набор байт 'data', которые можно прислать
-    из метода страницы MakeScreenshot()
+def save_img_as(path: Union[str, Path], data: bytes) -> None:
+    """ Сохраняет набор байт возвращаемый из conn.extend.makeScreenshot(), как изображение.
+    :param path:    Путь, или имя файла сохраняемого изображения.
+    :param data:    Данные изображения.
     """
     with open(path, "wb") as f:
         f.write(data)
 
 
 async def async_util_call(function: Callable, *args) -> any:
     """ Позволяет выполнять неблокирующий вызов блокирующих функций. Например:
     await async_util_call(
-        save_img_as, "ScreenShot.png", await page_instance.MakeScreenshot()
+        save_img_as, "ScreenShot.png", await conn.extend.makeScreenshot()
     )
     """
     return await asyncio.get_running_loop().run_in_executor(
         None, function, *args
     )
 
 
@@ -113,7 +116,36 @@
             if "--type=renderer" not in cmd_line and "--remote-debugging-port=" in cmd_line:
                 port = int(re.findall(r"--remote-debugging-port=(\d+)", cmd_line)[0])
                 if for_port == port: return {port: pid}
                 result[port] = pid
     else:
         raise OSError(f"Platform '{sys.platform}' — not supported")
     return {} if for_port else result
+
+
+def prepare_url(url: Union[str, bytes, None], browser_name: str, app: bool = False) -> Optional[str]:
+    """ Подготавливает строку для передачи в navigate(), или в конструкторе Browser."""
+
+    # Если url == None
+    if url is None:
+        return "--app=data:text/html," if app else None
+
+    # Если передали строку
+    if type(url) is str:
+
+        # И эта строка - пустая
+        if url == "":
+            return "--app=data:text/html," if app else "about:blank"
+
+        # Но если строка не содержит признаков url-адреса, то
+        # считаем это HTML-разметкой
+        if not url.startswith(("http", browser_name)):
+            url = "data:text/html," + quote(url)
+            return "--app=" + url if app else url
+
+        # Иначе - это адрес
+        return "--app=" + url if app else url
+
+    # Иначе считаем, что это не конвертированный набор байт
+    # из base64, в котором HTML-разметка
+    url = "data:text/html;Base64," + url.decode()
+    return "--app=" + url if app else url
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,54 @@
-Metadata-Version: 2.1
-Name: aio-dt-protocol
-Version: 1.1.1
-Summary: Asynchronous wrapper over Chromium browser debugger protocol.
-Home-page: https://github.com/PieceOfGood/aio_dt_protocol
-Author: PieceOfGood
-Author-email: 78sanchezz@gmail.com
-License: BSD 3-Clause
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Асинхронная обёртка над [протоколом](https://chromedevtools.github.io/devtools-protocol/) отладчика браузера Chromium.
 
 Запуски проводятся только в ОС Windows и Linux.
 
-### Установка
-```shell
-pip install aio-dt-protocol
-```
-
 Имеет одну зависимость:
 https://github.com/aaugustin/websockets
 
 И так как всё общение через протокол основано на формате JSON, по желанию можно установить в окружение ujson:
 https://github.com/ultrajson/ultrajson
 
+### Установка
+```shell
+pip install aio-dt-protocol
+```
+Или установить сразу вместе с [ujson](https://github.com/ultrajson/ultrajson)
+```shell
+pip install aio-dt-protocol[ujson]
+```
+
 ### Примеры:
 
 ```python
 import asyncio
 from aio_dt_protocol import Browser
 from aio_dt_protocol import BrowserName
-from aio_dt_protocol import find_instances
 from aio_dt_protocol.data import KeyEvents
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 PROFILE_NAME: str = BROWSER_NAME.capitalize() + "_Profile"
 
 
 async def main() -> None:
-    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
-    # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=PROFILE_NAME
-        )
-        msg = f"[- LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
-
     # ? Будет печатать в консоль всё, что приходит по соединению со страницей.
     # ? Полезно при разработке.
     # async def action_printer(data: dict) -> None:
     #     print(data)
-    # conn = await browser.waitFirstTab(callback=action_printer)
-    conn = await browser.waitFirstTab()
-
+    # browser, conn = await Browser.run(callback=action_printer)
+    
+    # ? Если на указанном порту есть запущенный браузер, происходит подключение.
+    # ? Иначе, запуск нового браузера.
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=PROFILE_NAME
+    )
+    
     print("[- GO TO GOOGLE ... -]")
     await conn.Page.navigate("https://www.google.com", )
     print("[- EMULATE INPUT TEXT ... -]")
 
     input_node = await conn.DOM.querySelector("[type=search]")
     
     # ? Эмуляция клика в поисковую строку
@@ -110,15 +85,15 @@
     asyncio.run(main())
 ```
 
 На страницу можно легко зарегистрировать слушателей, которые будут вызываться на стороне клиентского(Python) кода. Для этого необходимо зарегистрировать вызываемую функцию в качестве такого слушателя. Это возможно выполнить двумя способами:
 1. Вручную передав методу `addBinding()` домена `Runtime` имя функции в виде строки.
 2. Воспользоваться более функциональной обёрткой первого способа, выраженной в методе `bindFunction()` соединения.
 
-Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции, после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
+Второй способ менее многословен. Под капотом он добавляет в контекст страницы утилиту `py_call()`, первым аргументом принимающую имя функции(слушателя), после чего, любое кол-во позиционных аргументов, которые ожидает эта функция, а так же позволяет прикрепить любое кол-во аргументов, передаваемых в функцию последними. Например:
 
 ```python
     html = """\
     <html lang="ru">
     <head>
         <meta charset="utf-8" />
         <title>Test application</title>
@@ -156,37 +131,29 @@
     await conn.Page.navigate(html)
 ```
 ### Headless
 Чтобы запустить браузер в безголовом(`headless`) режиме, передайте пустую строку аргументу(`profile_path`) принимающему путь к папке профиля.
 
 ```python
 import asyncio
-from aio_dt_protocol import Browser, BrowserName, find_instances
+from aio_dt_protocol import Browser, BrowserName
 from aio_dt_protocol.utils import save_img_as, async_util_call
 
 DEBUG_PORT: int = 9222
 BROWSER_NAME: str = BrowserName.CHROME
 
 
 async def main() -> None:
     # ? Если на указанном порту есть запущенный браузер, происходит подключение.
-    if browser_instances := find_instances(DEBUG_PORT, BROWSER_NAME):
-        browser = Browser(
-            debug_port=DEBUG_PORT,
-            browser_pid=browser_instances[DEBUG_PORT])
-        msg = f"[- HEADLESS CONNECT TO EXIST BROWSER ON {DEBUG_PORT} PORT -]"
-
     # ? Иначе, запуск нового браузера.
-    else:
-        browser = Browser(
-            debug_port=DEBUG_PORT, browser_exe=BROWSER_NAME,
-            profile_path=""
-        )
-        msg = f"[- HEADLESS LAUNCH NEW BROWSER ON {DEBUG_PORT} PORT -]"
-    print(msg)
+    browser, conn = await Browser.run(
+        debug_port=DEBUG_PORT,
+        browser_name=BROWSER_NAME,
+        profile_path=""
+    )
     
     print("[- WAITING PAGE -]")
     conn = await browser.waitFirstTab()
     print("[- GO TO GOOGLE -]")
     await conn.Page.navigate("https://www.google.com")
 
     print("[- MAKE SCREENSHOT -]")
@@ -198,8 +165,8 @@
     await conn.Browser.close()
     print("[- DONE -]")
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 
-```
+```
```

### Comparing `aio_dt_protocol-1.1.1/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 aio_dt_protocol/__init__.py
 aio_dt_protocol/actions.py
 aio_dt_protocol/browser.py
 aio_dt_protocol/connection.py
 aio_dt_protocol/data.py
 aio_dt_protocol/exceptions.py
 aio_dt_protocol/extend_connection.py
+aio_dt_protocol/js.py
 aio_dt_protocol/utils.py
 aio_dt_protocol.egg-info/PKG-INFO
 aio_dt_protocol.egg-info/SOURCES.txt
 aio_dt_protocol.egg-info/dependency_links.txt
 aio_dt_protocol.egg-info/requires.txt
 aio_dt_protocol.egg-info/top_level.txt
 aio_dt_protocol/domains/__init__.py
```

### Comparing `aio_dt_protocol-1.1.1/setup.py` & `aio_dt_protocol-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/PieceOfGood/aio_dt_protocol",
     license="BSD 3-Clause",
     packages=PACKAGES,
     install_requires=["websockets>=10.0.0"],
 
+    extras_require=dict(
+        ujson=["ujson"],
+    ),
+
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

