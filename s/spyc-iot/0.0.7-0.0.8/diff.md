# Comparing `tmp/spyc_iot-0.0.7.tar.gz` & `tmp/spyc_iot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyc_iot-0.0.7.tar", last modified: Mon Jul 24 05:53:29 2023, max compression
+gzip compressed data, was "spyc_iot-0.0.8.tar", last modified: Fri Jul 28 17:36:51 2023, max compression
```

## Comparing `spyc_iot-0.0.7.tar` & `spyc_iot-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.357733 spyc_iot-0.0.7/
--rw-rw-rw-   0        0        0     1117 2023-07-24 01:47:07.000000 spyc_iot-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      307 2023-07-24 05:53:29.357733 spyc_iot-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-14 04:24:10.000000 spyc_iot-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      417 2023-07-24 05:53:29.359750 spyc_iot-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.332798 spyc_iot-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.342771 spyc_iot-0.0.7/src/spyc_iot/
--rw-rw-rw-   0        0        0      117 2023-07-24 01:47:43.000000 spyc_iot-0.0.7/src/spyc_iot/__init__.py
--rw-rw-rw-   0        0        0     5911 2023-07-24 04:23:06.000000 spyc_iot-0.0.7/src/spyc_iot/max7219.py
--rw-rw-rw-   0        0        0      667 2023-07-14 05:55:28.000000 spyc_iot-0.0.7/src/spyc_iot/ntp.py
--rw-rw-rw-   0        0        0      240 2023-07-24 04:23:07.000000 spyc_iot-0.0.7/src/spyc_iot/time.py
--rw-rw-rw-   0        0        0      505 2023-07-14 04:50:45.000000 spyc_iot-0.0.7/src/spyc_iot/wifi.py
-drwxrwxrwx   0        0        0        0 2023-07-24 05:53:29.355736 spyc_iot-0.0.7/src/spyc_iot.egg-info/
--rw-rw-rw-   0        0        0      307 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 05:53:29.000000 spyc_iot-0.0.7/src/spyc_iot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 17:36:51.760286 spyc_iot-0.0.8/
+-rw-rw-rw-   0        0        0     1117 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      346 2023-07-28 17:36:51.761299 spyc_iot-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      456 2023-07-28 17:36:51.763874 spyc_iot-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 17:36:51.724171 spyc_iot-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 17:36:51.742233 spyc_iot-0.0.8/src/spyc_iot/
+-rw-rw-rw-   0        0        0      140 2023-07-28 17:04:14.000000 spyc_iot-0.0.8/src/spyc_iot/__init__.py
+-rw-rw-rw-   0        0        0    10065 2023-07-28 17:04:03.000000 spyc_iot-0.0.8/src/spyc_iot/bme280.py
+-rw-rw-rw-   0        0        0     5911 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/src/spyc_iot/max7219.py
+-rw-rw-rw-   0        0        0      667 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/src/spyc_iot/ntp.py
+-rw-rw-rw-   0        0        0      240 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/src/spyc_iot/time.py
+-rw-rw-rw-   0        0        0      505 2023-07-28 16:57:00.000000 spyc_iot-0.0.8/src/spyc_iot/wifi.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:36:51.758781 spyc_iot-0.0.8/src/spyc_iot.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-28 17:36:51.000000 spyc_iot-0.0.8/src/spyc_iot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-28 17:36:51.000000 spyc_iot-0.0.8/src/spyc_iot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:36:51.000000 spyc_iot-0.0.8/src/spyc_iot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 17:36:51.000000 spyc_iot-0.0.8/src/spyc_iot.egg-info/top_level.txt
```

### Comparing `spyc_iot-0.0.7/LICENSE` & `spyc_iot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spyc_iot-0.0.7/src/spyc_iot/max7219.py` & `spyc_iot-0.0.8/src/spyc_iot/max7219.py`

 * *Files identical despite different names*

### Comparing `spyc_iot-0.0.7/src/spyc_iot/ntp.py` & `spyc_iot-0.0.8/src/spyc_iot/ntp.py`

 * *Files identical despite different names*

