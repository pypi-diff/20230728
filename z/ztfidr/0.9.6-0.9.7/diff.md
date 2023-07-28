# Comparing `tmp/ztfidr-0.9.6.tar.gz` & `tmp/ztfidr-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.6.tar", last modified: Thu Jul 27 16:08:16 2023, max compression
+gzip compressed data, was "ztfidr-0.9.7.tar", last modified: Fri Jul 28 18:15:26 2023, max compression
```

## Comparing `ztfidr-0.9.6.tar` & `ztfidr-0.9.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-27 16:08:16.811331 ztfidr-0.9.6/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.6/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-07-27 16:08:16.811182 ztfidr-0.9.6/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.6/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-07-27 16:08:16.811378 ztfidr-0.9.6/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-07-27 16:07:43.000000 ztfidr-0.9.6/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-27 16:08:16.810390 ztfidr-0.9.6/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      126 2023-07-27 16:07:49.000000 ztfidr-0.9.6/ztfidr/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5542 2023-07-17 14:06:04.000000 ztfidr-0.9.6/ztfidr/host.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    16159 2023-07-13 12:05:49.000000 ztfidr-0.9.6/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22999 2023-07-27 16:07:03.000000 ztfidr-0.9.6/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.6/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)    25901 2023-07-13 12:46:52.000000 ztfidr-0.9.6/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1091 2023-06-18 10:58:06.000000 ztfidr-0.9.6/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    25280 2023-06-20 08:13:19.000000 ztfidr-0.9.6/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.6/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.6/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.6/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.6/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23636 2023-07-27 15:37:39.000000 ztfidr-0.9.6/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4225 2023-07-05 21:38:13.000000 ztfidr-0.9.6/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-27 16:08:16.811010 ztfidr-0.9.6/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-07-27 16:08:16.000000 ztfidr-0.9.6/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      392 2023-07-27 16:08:16.000000 ztfidr-0.9.6/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-07-27 16:08:16.000000 ztfidr-0.9.6/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-07-27 16:08:16.000000 ztfidr-0.9.6/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.761319 ztfidr-0.9.7/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.7/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-07-28 18:15:26.761199 ztfidr-0.9.7/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.7/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-07-28 18:15:26.761358 ztfidr-0.9.7/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-07-28 18:15:08.000000 ztfidr-0.9.7/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.760447 ztfidr-0.9.7/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      126 2023-07-28 18:15:13.000000 ztfidr-0.9.7/ztfidr/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5542 2023-07-17 14:06:04.000000 ztfidr-0.9.7/ztfidr/host.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    16159 2023-07-13 12:05:49.000000 ztfidr-0.9.7/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23052 2023-07-28 18:14:33.000000 ztfidr-0.9.7/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.7/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    25901 2023-07-13 12:46:52.000000 ztfidr-0.9.7/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1091 2023-06-18 10:58:06.000000 ztfidr-0.9.7/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    25280 2023-06-20 08:13:19.000000 ztfidr-0.9.7/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.7/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.7/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.7/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.7/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23636 2023-07-27 15:37:39.000000 ztfidr-0.9.7/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4225 2023-07-05 21:38:13.000000 ztfidr-0.9.7/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-07-28 18:15:26.761042 ztfidr-0.9.7/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      392 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-07-28 18:15:26.000000 ztfidr-0.9.7/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.6/LICENSE` & `ztfidr-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/README.md` & `ztfidr-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/host.py` & `ztfidr-0.9.7/ztfidr/host.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/io.py` & `ztfidr-0.9.7/ztfidr/io.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/lightcurve.py` & `ztfidr-0.9.7/ztfidr/lightcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,14 +364,15 @@
              
         t0 = self.saltparam.t0
         if not np.isnan(t0):
             if phase_range is not None: # removes NaN
                 timerange = [t0+phase_range[0], t0+phase_range[1]]
             else:
                 timerange = None
+            modeltime = t0 + np.linspace(-15,50,100)
         else:
             timerange = None
             if incl_salt:
                 warnings.warn("t0 in saltparam is NaN, cannot show the model")
             incl_salt = False
             saltmodel = None
             autoscale_salt = False
```

### Comparing `ztfidr-0.9.6/ztfidr/linefitter.py` & `ztfidr-0.9.7/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/plotting.py` & `ztfidr-0.9.7/ztfidr/plotting.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/salt2.py` & `ztfidr-0.9.7/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/sample.py` & `ztfidr-0.9.7/ztfidr/sample.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/script.py` & `ztfidr-0.9.7/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/snid.py` & `ztfidr-0.9.7/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/spectroscopy.py` & `ztfidr-0.9.7/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/target.py` & `ztfidr-0.9.7/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/typing.py` & `ztfidr-0.9.7/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.6/ztfidr/utils.py` & `ztfidr-0.9.7/ztfidr/utils.py`

 * *Files identical despite different names*

