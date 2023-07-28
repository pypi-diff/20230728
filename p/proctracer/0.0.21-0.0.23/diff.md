# Comparing `tmp/proctracer-0.0.21.tar.gz` & `tmp/proctracer-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.21.tar", last modified: Thu Jul 27 06:23:07 2023, max compression
+gzip compressed data, was "proctracer-0.0.23.tar", last modified: Fri Jul 28 11:09:25 2023, max compression
```

## Comparing `proctracer-0.0.21.tar` & `proctracer-0.0.23.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.21/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.21/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3670 2023-07-27 06:23:07.071091 proctracer-0.0.21/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2245 2023-07-26 19:58:26.000000 proctracer-0.0.21/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 06:22:52.000000 proctracer-0.0.21/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.21/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6367 2023-07-27 05:46:38.000000 proctracer-0.0.21/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5635 2023-07-27 05:41:06.000000 proctracer-0.0.21/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2743 2023-07-27 06:09:24.000000 proctracer-0.0.21/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.21/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-07-27 05:38:46.000000 proctracer-0.0.21/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     5153 2023-07-27 06:22:36.000000 proctracer-0.0.21/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 06:13:03.000000 proctracer-0.0.21/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3670 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-27 06:23:07.071091 proctracer-0.0.21/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4895 2023-07-26 19:20:43.000000 proctracer-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.930890 proctracer-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 11:09:16.000000 proctracer-0.0.23/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 11:09:16.000000 proctracer-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 11:09:25.930890 proctracer-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-28 11:09:16.000000 proctracer-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.926890 proctracer-0.0.23/proctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.930890 proctracer-0.0.23/proctracer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5153 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/proctracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.926890 proctracer-0.0.23/proctracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 11:09:25.930890 proctracer-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-28 11:09:16.000000 proctracer-0.0.23/setup.py
```

### Comparing `proctracer-0.0.21/LICENSE.md` & `proctracer-0.0.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/README.md` & `proctracer-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/__init__.py` & `proctracer-0.0.23/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.23/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.23/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.23/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.23/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/plugin_base.py` & `proctracer-0.0.23/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.23/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.23/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.23/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.23/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer/proctracer.py` & `proctracer-0.0.23/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.23/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.21/setup.py` & `proctracer-0.0.23/setup.py`

 * *Files identical despite different names*

