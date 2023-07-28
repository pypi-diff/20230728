# Comparing `tmp/screw_thread_lib-0.0.1.tar.gz` & `tmp/screw_thread_lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screw_thread_lib-0.0.1.tar", last modified: Mon Jun 12 20:37:47 2023, max compression
+gzip compressed data, was "screw_thread_lib-0.0.2.tar", last modified: Fri Jul 28 16:42:51 2023, max compression
```

## Comparing `screw_thread_lib-0.0.1.tar` & `screw_thread_lib-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:37:47.311272 screw_thread_lib-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-31 00:26:55.000000 screw_thread_lib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      662 2023-06-12 20:37:47.311272 screw_thread_lib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-31 01:06:38.000000 screw_thread_lib-0.0.1/README.md
--rw-rw-rw-   0        0        0      111 2021-01-22 15:42:11.000000 screw_thread_lib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      526 2023-06-12 20:37:47.318277 screw_thread_lib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       69 2021-01-22 15:35:30.000000 screw_thread_lib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:37:47.291491 screw_thread_lib-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 20:37:47.302169 screw_thread_lib-0.0.1/src/screw_thread_lib/
--rw-rw-rw-   0        0        0       31 2023-05-31 01:13:28.000000 screw_thread_lib-0.0.1/src/screw_thread_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:37:47.310272 screw_thread_lib-0.0.1/src/screw_thread_lib/data/
--rw-rw-rw-   0        0        0     2926 2023-06-12 14:08:55.000000 screw_thread_lib-0.0.1/src/screw_thread_lib/data/ASME_B11.py
--rw-rw-rw-   0        0        0       45 2023-06-12 14:09:08.000000 screw_thread_lib-0.0.1/src/screw_thread_lib/data/__init__.py
--rw-rw-rw-   0        0        0    11288 2023-06-12 14:08:51.000000 screw_thread_lib-0.0.1/src/screw_thread_lib/threads.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:37:47.307716 screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/
--rw-rw-rw-   0        0        0      662 2023-06-12 20:37:47.000000 screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-06-12 20:37:47.000000 screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:37:47.000000 screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 20:37:47.000000 screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 16:42:51.193868 screw_thread_lib-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-31 00:26:55.000000 screw_thread_lib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      662 2023-07-28 16:42:51.194201 screw_thread_lib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-31 01:06:38.000000 screw_thread_lib-0.0.2/README.md
+-rw-rw-rw-   0        0        0      111 2021-01-22 15:42:11.000000 screw_thread_lib-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      526 2023-07-28 16:42:51.196184 screw_thread_lib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       69 2021-01-22 15:35:30.000000 screw_thread_lib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:42:51.132939 screw_thread_lib-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 16:42:51.169687 screw_thread_lib-0.0.2/src/screw_thread_lib/
+-rw-rw-rw-   0        0        0       47 2023-07-11 13:57:03.000000 screw_thread_lib-0.0.2/src/screw_thread_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:42:51.191607 screw_thread_lib-0.0.2/src/screw_thread_lib/data/
+-rw-rw-rw-   0        0        0     3300 2023-07-28 16:40:05.000000 screw_thread_lib-0.0.2/src/screw_thread_lib/data/ASME_B11.py
+-rw-rw-rw-   0        0        0       45 2023-06-12 14:09:08.000000 screw_thread_lib-0.0.2/src/screw_thread_lib/data/__init__.py
+-rw-rw-rw-   0        0        0    15832 2023-07-11 14:12:00.000000 screw_thread_lib-0.0.2/src/screw_thread_lib/threads.py
+drwxrwxrwx   0        0        0        0 2023-07-28 16:42:51.178496 screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-07-28 16:42:51.000000 screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-07-28 16:42:51.000000 screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 16:42:51.000000 screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 16:42:51.000000 screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/top_level.txt
```

### Comparing `screw_thread_lib-0.0.1/LICENSE` & `screw_thread_lib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `screw_thread_lib-0.0.1/PKG-INFO` & `screw_thread_lib-0.0.2/src/screw_thread_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: screw_thread_lib
-Version: 0.0.1
+Name: screw-thread-lib
+Version: 0.0.2
 Summary: A package for computing the strength of threaded fastener assemblies.
 Home-page: https://github.com/denavit/ScrewThreadLib
 Author: Mark Denavit
 Author-email: mdenavit@utk.edu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `screw_thread_lib-0.0.1/setup.cfg` & `screw_thread_lib-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6372 6577 5f74 6872 6561 645f   = screw_thread_
 00000020: 6c69 620d 0a76 6572 7369 6f6e 203d 2030  lib..version = 0
-00000030: 2e30 2e31 0d0a 6175 7468 6f72 203d 204d  .0.1..author = M
+00000030: 2e30 2e32 0d0a 6175 7468 6f72 203d 204d  .0.2..author = M
 00000040: 6172 6b20 4465 6e61 7669 740d 0a61 7574  ark Denavit..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d64 656e  hor_email = mden
 00000060: 6176 6974 4075 746b 2e65 6475 0d0a 6465  avit@utk.edu..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 636f 6d70 7574  ckage for comput
 00000090: 696e 6720 7468 6520 7374 7265 6e67 7468  ing the strength
 000000a0: 206f 6620 7468 7265 6164 6564 2066 6173   of threaded fas
```

### Comparing `screw_thread_lib-0.0.1/src/screw_thread_lib/data/ASME_B11.py` & `screw_thread_lib-0.0.2/src/screw_thread_lib/data/ASME_B11.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # All values from ASME B1.1-2019
 
 ASME_B11_UN_2A2B_dict = {
-    '10-24':  {'series': 'UNC', 'dbsc': 0.1900, 'n': 24, 'd2bsc': 0.1629, 'D2bsc': 0.1629, 'd1bsc': 0.1404, 'D1bsc': 0.1449, 'dmax': 0.1890, 'dmin': 0.1818, 'd2max': 0.1619, 'd2min': 0.1586, 'D1min': 0.145, 'D1max': 0.155, 'D2min': 0.1629, 'D2max': 0.1672 },
-    '10-32':  {'series': 'UNF', 'dbsc': 0.1900, 'n': 32, 'd2bsc': 0.1697, 'D2bsc': 0.1697, 'd1bsc': 0.1528, 'D1bsc': 0.1562, 'dmax': 0.1891, 'dmin': 0.1831, 'd2max': 0.1688, 'd2min': 0.1658, 'D1min': 0.156, 'D1max': 0.164, 'D2min': 0.1697, 'D2max': 0.1736 },
-    '1/4-20': {'series': 'UNC', 'dbsc': 0.2500, 'n': 20, 'd2bsc': 0.2175, 'D2bsc': 0.2175, 'd1bsc': 0.1905, 'D1bsc': 0.1959, 'dmax': 0.2489, 'dmin': 0.2408, 'd2max': 0.2164, 'd2min': 0.2127, 'D1min': 0.196, 'D1max': 0.207, 'D2min': 0.2175, 'D2max': 0.2224 },
-    '1/4-28': {'series': 'UNF', 'dbsc': 0.2500, 'n': 28, 'd2bsc': 0.2268, 'D2bsc': 0.2268, 'd1bsc': 0.2075, 'D1bsc': 0.2113, 'dmax': 0.2490, 'dmin': 0.2425, 'd2max': 0.2258, 'd2min': 0.2225, 'D1min': 0.211, 'D1max': 0.220, 'D2min': 0.2268, 'D2max': 0.2311 },
-    '1/2-13': {'series': 'UNC', 'dbsc': 0.5000, 'n': 13, 'd2bsc': 0.4500, 'D2bsc': 0.4500, 'd1bsc': 0.4084, 'D1bsc': 0.4167, 'dmax': 0.4985, 'dmin': 0.4876, 'd2max': 0.4485, 'd2min': 0.4435, 'D1min': 0.417, 'D1max': 0.434, 'D2min': 0.4500, 'D2max': 0.4565 },
-    '1/2-20': {'series': 'UNF', 'dbsc': 0.5000, 'n': 20, 'd2bsc': 0.4675, 'D2bsc': 0.4675, 'd1bsc': 0.4405, 'D1bsc': 0.4459, 'dmax': 0.4987, 'dmin': 0.4906, 'd2max': 0.4662, 'd2min': 0.4619, 'D1min': 0.446, 'D1max': 0.457, 'D2min': 0.4675, 'D2max': 0.4731 },
-    '3/4-10': {'series': 'UNC', 'dbsc': 0.7500, 'n': 10, 'd2bsc': 0.6850, 'D2bsc': 0.6850, 'd1bsc': 0.6309, 'D1bsc': 0.6417, 'dmax': 0.7482, 'dmin': 0.7353, 'd2max': 0.6832, 'd2min': 0.6773, 'D1min': 0.642, 'D1max': 0.663, 'D2min': 0.6850, 'D2max': 0.6927 },
-    '3/4-16': {'series': 'UNF', 'dbsc': 0.7500, 'n': 16, 'd2bsc': 0.7094, 'D2bsc': 0.7094, 'd1bsc': 0.6756, 'D1bsc': 0.6823, 'dmax': 0.7485, 'dmin': 0.7391, 'd2max': 0.7079, 'd2min': 0.7029, 'D1min': 0.682, 'D1max': 0.696, 'D2min': 0.7094, 'D2max': 0.7159 },
-    '1-8':    {'series': 'UNC', 'dbsc': 1.0000, 'n':  8, 'd2bsc': 0.9188, 'D2bsc': 0.9188, 'd1bsc': 0.8512, 'D1bsc': 0.8647, 'dmax': 0.9980, 'dmin': 0.9830, 'd2max': 0.9168, 'd2min': 0.9101, 'D1min': 0.865, 'D1max': 0.890, 'D2min': 0.9188, 'D2max': 0.9276 },
-    '1-12':   {'series': 'UNF', 'dbsc': 1.0000, 'n': 12, 'd2bsc': 0.9459, 'D2bsc': 0.9459, 'd1bsc': 0.9008, 'D1bsc': 0.9098, 'dmax': 0.9982, 'dmin': 0.9868, 'd2max': 0.9441, 'd2min': 0.9382, 'D1min': 0.910, 'D1max': 0.928, 'D2min': 0.9459, 'D2max': 0.9535 },
-    '1-14':   {'series': 'UNS', 'dbsc': 1.0000, 'n': 14, 'd2bsc': 0.9536, 'D2bsc': 0.9536, 'd1bsc': 0.9149, 'D1bsc': 0.9227, 'dmax': 0.9984, 'dmin': 0.9881, 'd2max': 0.9520, 'd2min': 0.9467, 'D1min': 0.923, 'D1max': 0.938, 'D2min': 0.9536, 'D2max': 0.9605 },
+    '10-24':  {'series': 'UNC', 'dbsc': 0.1900, 'n': 24, 'd2bsc': 0.1629, 'D2bsc': 0.1629, 'd1bsc': 0.1404, 'D1bsc': 0.1449, 'dmax': 0.1890, 'dmin': 0.1818, 'd2max': 0.1619, 'd2min': 0.1586, 'd1max': 0.1439, 'd1min': 0.1315, 'D1min': 0.145, 'D1max': 0.155, 'D2min': 0.1629, 'D2max': 0.1672 },
+    '10-32':  {'series': 'UNF', 'dbsc': 0.1900, 'n': 32, 'd2bsc': 0.1697, 'D2bsc': 0.1697, 'd1bsc': 0.1528, 'D1bsc': 0.1562, 'dmax': 0.1891, 'dmin': 0.1831, 'd2max': 0.1688, 'd2min': 0.1658, 'd1max': 0.1553, 'd1min': 0.1455, 'D1min': 0.156, 'D1max': 0.164, 'D2min': 0.1697, 'D2max': 0.1736 },
+    '1/4-20': {'series': 'UNC', 'dbsc': 0.2500, 'n': 20, 'd2bsc': 0.2175, 'D2bsc': 0.2175, 'd1bsc': 0.1905, 'D1bsc': 0.1959, 'dmax': 0.2489, 'dmin': 0.2408, 'd2max': 0.2164, 'd2min': 0.2127, 'd1max': 0.1948, 'd1min': 0.1802, 'D1min': 0.196, 'D1max': 0.207, 'D2min': 0.2175, 'D2max': 0.2224 },
+    '1/4-28': {'series': 'UNF', 'dbsc': 0.2500, 'n': 28, 'd2bsc': 0.2268, 'D2bsc': 0.2268, 'd1bsc': 0.2075, 'D1bsc': 0.2113, 'dmax': 0.2490, 'dmin': 0.2425, 'd2max': 0.2258, 'd2min': 0.2225, 'd1max': 0.2103, 'd1min': 0.1993, 'D1min': 0.211, 'D1max': 0.220, 'D2min': 0.2268, 'D2max': 0.2311 },
+    '1/2-13': {'series': 'UNC', 'dbsc': 0.5000, 'n': 13, 'd2bsc': 0.4500, 'D2bsc': 0.4500, 'd1bsc': 0.4084, 'D1bsc': 0.4167, 'dmax': 0.4985, 'dmin': 0.4876, 'd2max': 0.4485, 'd2min': 0.4435, 'd1max': 0.4152, 'd1min': 0.3935, 'D1min': 0.417, 'D1max': 0.434, 'D2min': 0.4500, 'D2max': 0.4565 },
+    '1/2-20': {'series': 'UNF', 'dbsc': 0.5000, 'n': 20, 'd2bsc': 0.4675, 'D2bsc': 0.4675, 'd1bsc': 0.4405, 'D1bsc': 0.4459, 'dmax': 0.4987, 'dmin': 0.4906, 'd2max': 0.4662, 'd2min': 0.4619, 'd1max': 0.4446, 'd1min': 0.4294, 'D1min': 0.446, 'D1max': 0.457, 'D2min': 0.4675, 'D2max': 0.4731 },
+    '3/4-10': {'series': 'UNC', 'dbsc': 0.7500, 'n': 10, 'd2bsc': 0.6850, 'D2bsc': 0.6850, 'd1bsc': 0.6309, 'D1bsc': 0.6417, 'dmax': 0.7482, 'dmin': 0.7353, 'd2max': 0.6832, 'd2min': 0.6773, 'd1max': 0.6399, 'd1min': 0.6123, 'D1min': 0.642, 'D1max': 0.663, 'D2min': 0.6850, 'D2max': 0.6927 },
+    '3/4-16': {'series': 'UNF', 'dbsc': 0.7500, 'n': 16, 'd2bsc': 0.7094, 'D2bsc': 0.7094, 'd1bsc': 0.6756, 'D1bsc': 0.6823, 'dmax': 0.7485, 'dmin': 0.7391, 'd2max': 0.7079, 'd2min': 0.7029, 'd1max': 0.6808, 'd1min': 0.6623, 'D1min': 0.682, 'D1max': 0.696, 'D2min': 0.7094, 'D2max': 0.7159 },
+    '1-8':    {'series': 'UNC', 'dbsc': 1.0000, 'n':  8, 'd2bsc': 0.9188, 'D2bsc': 0.9188, 'd1bsc': 0.8512, 'D1bsc': 0.8647, 'dmax': 0.9980, 'dmin': 0.9830, 'd2max': 0.9168, 'd2min': 0.9101, 'd1max': 0.8627, 'd1min': 0.8289, 'D1min': 0.865, 'D1max': 0.890, 'D2min': 0.9188, 'D2max': 0.9276 },
+    '1-12':   {'series': 'UNF', 'dbsc': 1.0000, 'n': 12, 'd2bsc': 0.9459, 'D2bsc': 0.9459, 'd1bsc': 0.9008, 'D1bsc': 0.9098, 'dmax': 0.9982, 'dmin': 0.9868, 'd2max': 0.9441, 'd2min': 0.9382, 'd1max': 0.9080, 'd1min': 0.8841, 'D1min': 0.910, 'D1max': 0.928, 'D2min': 0.9459, 'D2max': 0.9535 },
+    '1-14':   {'series': 'UNS', 'dbsc': 1.0000, 'n': 14, 'd2bsc': 0.9536, 'D2bsc': 0.9536, 'd1bsc': 0.9149, 'D1bsc': 0.9227, 'dmax': 0.9984, 'dmin': 0.9881, 'd2max': 0.9520, 'd2min': 0.9467, 'd1max': 0.9211, 'd1min': 0.9003, 'D1min': 0.923, 'D1max': 0.938, 'D2min': 0.9536, 'D2max': 0.9605 },
 }
```

### Comparing `screw_thread_lib-0.0.1/src/screw_thread_lib.egg-info/PKG-INFO` & `screw_thread_lib-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: screw-thread-lib
-Version: 0.0.1
+Name: screw_thread_lib
+Version: 0.0.2
 Summary: A package for computing the strength of threaded fastener assemblies.
 Home-page: https://github.com/denavit/ScrewThreadLib
 Author: Mark Denavit
 Author-email: mdenavit@utk.edu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

