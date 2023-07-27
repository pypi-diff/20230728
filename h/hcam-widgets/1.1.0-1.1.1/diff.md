# Comparing `tmp/hcam_widgets-1.1.0.tar.gz` & `tmp/hcam_widgets-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_widgets-1.1.0.tar", last modified: Fri Jul 21 10:49:41 2023, max compression
+gzip compressed data, was "hcam_widgets-1.1.1.tar", last modified: Thu Jul 27 22:10:41 2023, max compression
```

## Comparing `hcam_widgets-1.1.0.tar` & `hcam_widgets-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.676451 hcam_widgets-1.1.0/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.1.0/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.1.0/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.1.0/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-21 10:49:41.676524 hcam_widgets-1.1.0/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.1.0/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.672860 hcam_widgets-1.1.0/hcam_widgets/
--rw-r--r--   0 sl         (501) staff       (20)      246 2023-07-21 10:48:53.000000 hcam_widgets-1.1.0/hcam_widgets/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/astro.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.674804 hcam_widgets-1.1.0/hcam_widgets/compo/
--rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/compo/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)    15062 2023-05-30 12:10:48.000000 hcam_widgets-1.1.0/hcam_widgets/compo/utils.py
--rw-r--r--   0 sl         (501) staff       (20)    27122 2023-05-17 10:15:42.000000 hcam_widgets-1.1.0/hcam_widgets/compo/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.675176 hcam_widgets-1.1.0/hcam_widgets/data/
--rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/data/compo_lens_offset.csv
--rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/globals.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.676172 hcam_widgets-1.1.0/hcam_widgets/hardware/
--rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/alarms.py
--rw-r--r--   0 sl         (501) staff       (20)     4751 2023-05-10 10:21:39.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/ccds.py
--rw-r--r--   0 sl         (501) staff       (20)     9157 2023-05-15 10:45:53.000000 hcam_widgets-1.1.0/hcam_widgets/hardware/slide.py
--rw-r--r--   0 sl         (501) staff       (20)    70117 2023-05-04 13:39:14.000000 hcam_widgets-1.1.0/hcam_widgets/hcam.py
--rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.1.0/hcam_widgets/logs.py
--rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/mimic.py
--rw-r--r--   0 sl         (501) staff       (20)    20068 2021-09-13 09:33:55.000000 hcam_widgets-1.1.0/hcam_widgets/misc.py
--rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/tcs.py
--rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.1.0/hcam_widgets/tkutils.py
--rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/ucam.py
--rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.1.0/hcam_widgets/uspec.py
--rw-r--r--   0 sl         (501) staff       (20)   149251 2023-05-12 19:12:14.000000 hcam_widgets-1.1.0/hcam_widgets/widgets.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-21 10:49:41.674206 hcam_widgets-1.1.0/hcam_widgets.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)      827 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       71 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-21 10:49:41.000000 hcam_widgets-1.1.0/hcam_widgets.egg-info/top_level.txt
--rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-21 10:49:41.676766 hcam_widgets-1.1.0/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1909 2023-07-21 10:48:53.000000 hcam_widgets-1.1.0/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.543339 hcam_widgets-1.1.1/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-11-13 13:48:04.000000 hcam_widgets-1.1.1/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3303 2017-11-13 15:08:00.000000 hcam_widgets-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-11-13 13:48:04.000000 hcam_widgets-1.1.1/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-11-13 13:48:08.000000 hcam_widgets-1.1.1/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      303 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-27 22:10:41.543400 hcam_widgets-1.1.1/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2299 2018-02-15 16:29:54.000000 hcam_widgets-1.1.1/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.541643 hcam_widgets-1.1.1/hcam_widgets/
+-rw-r--r--   0 sl         (501) staff       (20)      246 2023-07-27 22:09:32.000000 hcam_widgets-1.1.1/hcam_widgets/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     8880 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/astro.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542708 hcam_widgets-1.1.1/hcam_widgets/compo/
+-rw-r--r--   0 sl         (501) staff       (20)        0 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/compo/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)    15204 2023-07-27 22:08:39.000000 hcam_widgets-1.1.1/hcam_widgets/compo/utils.py
+-rw-r--r--   0 sl         (501) staff       (20)    27122 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/compo/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542834 hcam_widgets-1.1.1/hcam_widgets/data/
+-rw-r--r--   0 sl         (501) staff       (20)     1704 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/data/compo_lens_offset.csv
+-rw-r--r--   0 sl         (501) staff       (20)     7024 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/globals.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.543242 hcam_widgets-1.1.1/hcam_widgets/hardware/
+-rw-r--r--   0 sl         (501) staff       (20)    17450 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     6312 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/alarms.py
+-rw-r--r--   0 sl         (501) staff       (20)     4751 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/ccds.py
+-rw-r--r--   0 sl         (501) staff       (20)     9157 2023-07-21 10:52:00.000000 hcam_widgets-1.1.1/hcam_widgets/hardware/slide.py
+-rw-r--r--   0 sl         (501) staff       (20)    70257 2023-07-27 21:58:00.000000 hcam_widgets-1.1.1/hcam_widgets/hcam.py
+-rw-r--r--   0 sl         (501) staff       (20)     4036 2018-02-15 16:29:54.000000 hcam_widgets-1.1.1/hcam_widgets/logs.py
+-rw-r--r--   0 sl         (501) staff       (20)      370 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/mimic.py
+-rw-r--r--   0 sl         (501) staff       (20)    20264 2023-07-27 22:08:39.000000 hcam_widgets-1.1.1/hcam_widgets/misc.py
+-rw-r--r--   0 sl         (501) staff       (20)     2087 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/tcs.py
+-rw-r--r--   0 sl         (501) staff       (20)     1880 2017-11-22 14:17:48.000000 hcam_widgets-1.1.1/hcam_widgets/tkutils.py
+-rw-r--r--   0 sl         (501) staff       (20)    22334 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/ucam.py
+-rw-r--r--   0 sl         (501) staff       (20)    36505 2021-05-26 10:14:11.000000 hcam_widgets-1.1.1/hcam_widgets/uspec.py
+-rw-r--r--   0 sl         (501) staff       (20)   149251 2023-07-27 21:10:09.000000 hcam_widgets-1.1.1/hcam_widgets/widgets.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:10:41.542393 hcam_widgets-1.1.1/hcam_widgets.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3306 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)      827 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       71 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       13 2023-07-27 22:10:41.000000 hcam_widgets-1.1.1/hcam_widgets.egg-info/top_level.txt
+-rw-r--r--   0 sl         (501) staff       (20)      313 2023-07-27 22:10:41.543620 hcam_widgets-1.1.1/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1909 2023-07-27 22:09:32.000000 hcam_widgets-1.1.1/setup.py
```

### Comparing `hcam_widgets-1.1.0/CONTRIBUTING.rst` & `hcam_widgets-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/LICENSE` & `hcam_widgets-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/PKG-INFO` & `hcam_widgets-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_widgets
-Version: 1.1.0
+Version: 1.1.1
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_widgets
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_widgets-1.1.0/README.rst` & `hcam_widgets-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/astro.py` & `hcam_widgets-1.1.1/hcam_widgets/astro.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/compo/utils.py` & `hcam_widgets-1.1.1/hcam_widgets/compo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import print_function, unicode_literals, absolute_import, division
-import pkg_resources
+import importlib
 
 # non-standard imports
 from astropy import units as u
 from astropy.coordinates.matrix_utilities import rotation_matrix
 from astropy.coordinates import CartesianRepresentation
 from astropy.utils import lazyproperty
 from scipy.interpolate import interp1d
@@ -18,14 +18,20 @@
     from ginga.util import wcs
     import ginga.canvas.types.all as ginga_types
 
     has_ginga = True
 except Exception:
     has_ginga = False
 
+try:
+    from importlib import resources as importlib_resources
+except Exception:
+    # backport for Python 3.6
+    import importlib_resources
+
 flip = np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]])
 
 # COMPO is only available on GTC, so these values are well-known
 pixel_scale = 0.08086 * u.arcsec / u.pix
 focal_plane_scale = 1.214 * u.arcsec / u.mm
 gtc_focalplane_equivalencies = [
     (u.mm, u.arcsec, lambda x: x * 1.214, lambda x: x / 1.214),
@@ -90,17 +96,18 @@
 MAX_ANGLE = 67 * u.deg  # hard stops at (67.79, -67.55) for PO, (67.4, -67.8) for IA
 
 # interpolated functions for X and Y positions - not unit aware
 x_func = interp1d(THETA, X, kind="cubic", bounds_error=False, fill_value="extrapolate")
 y_func = interp1d(THETA, Y, kind="cubic", bounds_error=False, fill_value="extrapolate")
 
 # interpolated functions for lens offset
-lens_data_file = pkg_resources.resource_filename(
-    "hcam_widgets", "data/compo_lens_offset.csv"
+lens_data_file = (
+    importlib_resources.files("hcam_widgets") / "data" / "compo_lens_offset.csv"
 )
+
 _, po_theta, lens_off = np.loadtxt(lens_data_file, delimiter=",", skiprows=1).T
 _g = interp1d(po_theta, lens_off, bounds_error=False, fill_value="extrapolate")
 
 
 @u.quantity_input(pickoff_theta=u.deg)
 def target_lens_position(pickoff_theta, guiding=False):
     """
```

### Comparing `hcam_widgets-1.1.0/hcam_widgets/compo/widgets.py` & `hcam_widgets-1.1.1/hcam_widgets/compo/widgets.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/data/compo_lens_offset.csv` & `hcam_widgets-1.1.1/hcam_widgets/data/compo_lens_offset.csv`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/globals.py` & `hcam_widgets-1.1.1/hcam_widgets/globals.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/hardware/__init__.py` & `hcam_widgets-1.1.1/hcam_widgets/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/hardware/alarms.py` & `hcam_widgets-1.1.1/hcam_widgets/hardware/alarms.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/hardware/ccds.py` & `hcam_widgets-1.1.1/hcam_widgets/hardware/ccds.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/hardware/slide.py` & `hcam_widgets-1.1.1/hcam_widgets/hardware/slide.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/hcam.py` & `hcam_widgets-1.1.1/hcam_widgets/hcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,24 @@
         # Readout speed
         tk.Label(lhs, text="Readout speed").grid(row=7, column=0, sticky=tk.W)
         self.readSpeed = w.Select(lhs, 1, ("Fast", "Slow"), self.check)
         self.readSpeed.grid(row=7, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # Exp delay
         tk.Label(lhs, text="Exposure delay (s)").grid(row=8, column=0, sticky=tk.W)
-        self.expose = w.Expose(lhs, 0.1, 0.00001, 1677.7207, self.check, width=7)
+        self.expose = w.RangedFloat(
+            lhs,
+            0.1,
+            0.00001,
+            1677.7207,
+            self.check,
+            blank=True,
+            allowzero=True,
+            width=7,
+        )
         self.expose.grid(row=8, column=1, columnspan=2, pady=2, sticky=tk.W)
 
         # num exp
         tk.Label(lhs, text="Num. exposures  ").grid(row=9, column=0, sticky=tk.W)
         self.number = w.PosInt(lhs, 0, None, False, width=7)
         self.number.grid(row=9, column=1, columnspan=2, pady=2, sticky=tk.W)
```

### Comparing `hcam_widgets-1.1.0/hcam_widgets/logs.py` & `hcam_widgets-1.1.1/hcam_widgets/logs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/misc.py` & `hcam_widgets-1.1.1/hcam_widgets/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,96 +40,94 @@
      err     : reason if telemetry not parsed OK
      state   : state of the camera. Possibilties are:
                'IDLE', 'BUSY', 'ERROR', 'ABORT', 'UNKNOWN'
      clocks  : whether the clock voltages are enabled. Possible values:
                'enabled', 'disabled'
      run     : current or last run number
     """
+
     def __init__(self, telemetry):
         """
         Parameters
         ----------
         telemetry : dict
             telemetry package from NGC
         """
         # Determine state of the camera
         self.ok = True
-        self.err = ''
-        if 'system.subStateName' not in telemetry:
-            self.err += 'could not identify state\n'
+        self.err = ""
+        if "system.subStateName" not in telemetry:
+            self.err += "could not identify state\n"
             self.state = None
         else:
-            self.state = telemetry['system.subStateName']
+            self.state = telemetry["system.subStateName"]
 
         # determine state of clocks
-        if 'cldc_0.statusName' not in telemetry:
+        if "cldc_0.statusName" not in telemetry:
             self.ok = False
-            self.err += 'could not identify clock status\n'
+            self.err += "could not identify clock status\n"
             self.clocks = None
         else:
-            self.clocks = telemetry['cldc_0.statusName']
+            self.clocks = telemetry["cldc_0.statusName"]
 
         # Find current run number (set it to 0 if we fail)
         newDataFileName = telemetry["exposure.newDataFileName"]
         exposure_state = telemetry["exposure.expStatusName"]
-        pattern = '\D*(\d*).*.fits'
+        pattern = "\D*(\d*).*.fits"
         try:
             run_number = int(re.match(pattern, newDataFileName).group(1))
-            if exposure_state in ["success", "aborted", 'inactive', 'failure']:
+            if exposure_state in ["success", "aborted", "inactive", "failure"]:
                 self.run = run_number
             elif exposure_state == "integrating":
                 self.run = run_number + 1
             else:
-                raise ValueError("unknown exposure state {}".format(
-                    exposure_state
-                ))
+                raise ValueError("unknown exposure state {}".format(exposure_state))
         except (ValueError, IndexError, AttributeError):
             self.run = 0
             self.ok = False
-            self.err += 'cannot read run number'
+            self.err += "cannot read run number"
 
 
 def overlap(xl1, yl1, nx1, ny1, xl2, yl2, nx2, ny2):
     """
     Determines whether two windows overlap
     """
-    return (xl2 < xl1+nx1 and xl2+nx2 > xl1 and
-            yl2 < yl1+ny1 and yl2+ny2 > yl1)
+    return xl2 < xl1 + nx1 and xl2 + nx2 > xl1 and yl2 < yl1 + ny1 and yl2 + ny2 > yl1
 
 
 @inlineCallbacks
 def startNodding(g, data):
-    nodPattern = data.get('appdata', {}).get('nodpattern', {})
-    if g.cpars['telins_name'] == 'GTC' and nodPattern:
+    nodPattern = data.get("appdata", {}).get("nodpattern", {})
+    if g.cpars["telins_name"] == "GTC" and nodPattern:
         session = g.session
         if session is None:
-            g.clog.warn('no WAMP session')
+            g.clog.warn("no WAMP session")
             returnValue(False)
         try:
-            yield session.call('hipercam.gtc.rpc.gtc.start_nodding')
+            yield session.call("hipercam.gtc.rpc.gtc.start_nodding")
         except Exception as err:
-            g.clog.warn('Failed to stop dither server')
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            g.clog.warn("Failed to stop dither server")
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn(msg)
             returnValue(False)
     returnValue(True)
 
 
 @inlineCallbacks
 def stopNodding(g):
-    if g.cpars['telins_name'] == 'GTC':
+    if g.cpars["telins_name"] == "GTC":
         session = g.session
         if session is None:
-            g.clog.warn('no WAMP session')
+            g.clog.warn("no WAMP session")
             returnValue(False)
         try:
-            yield session.call('hipercam.gtc.rpc.gtc.stop_nodding')
+            yield session.call("hipercam.gtc.rpc.gtc.stop_nodding")
         except Exception as err:
-            g.clog.warn('Failed to stop dither server')
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            g.clog.warn("Failed to stop dither server")
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
             g.clog.warn(msg)
             returnValue(False)
     returnValue(True)
 
 
 def saveJSON(g, data, backup=False):
     """
@@ -142,232 +140,236 @@
     The current setup in JSON compatible dictionary format.
 
     backup : bool
     If we are saving a backup on close, don't prompt for filename
     """
     if not backup:
         fname = filedialog.asksaveasfilename(
-            defaultextension='.json',
-            filetypes=[('json files', '.json'), ],
-            initialdir=g.cpars['app_directory']
-            )
+            defaultextension=".json",
+            filetypes=[
+                ("json files", ".json"),
+            ],
+            initialdir=g.cpars["app_directory"],
+        )
     else:
-        fname = os.path.join(os.path.expanduser('~/.hdriver'), 'app.json')
+        fname = os.path.join(os.path.expanduser("~/.hdriver"), "app.json")
 
     if not fname:
-        g.clog.warn('Aborted save to disk')
+        g.clog.warn("Aborted save to disk")
         return False
 
-    with open(fname, 'w') as of:
-        of.write(
-            json.dumps(data, sort_keys=True, indent=4,
-                       separators=(',', ': '))
-        )
-    g.clog.info('Saved setup to' + fname)
+    with open(fname, "w") as of:
+        of.write(json.dumps(data, sort_keys=True, indent=4, separators=(",", ": ")))
+    g.clog.info("Saved setup to" + fname)
     return True
 
 
 @inlineCallbacks
 def postJSON(g, data):
     """
     Posts the current setup to the camera and data servers.
 
     g : hcam_drivers.globals.Container
     Container with globals
 
     data : dict
     The current setup in JSON compatible dictionary format.
     """
-    g.clog.debug('Entering postJSON')
+    g.clog.debug("Entering postJSON")
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
     ok = True
     try:
-        ok, status_msg = yield session.call('hipercam.ngc.rpc.load_setup', data)
+        ok, status_msg = yield session.call("hipercam.ngc.rpc.load_setup", data)
     except Exception as err:
-        status_msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+        status_msg = err.error_message() if hasattr(err, "error_message") else str(err)
         ok = False
 
     if not ok:
-        g.clog.warn('Server response was not OK')
-        g.rlog.warn('Error: ' + status_msg)
+        g.clog.warn("Server response was not OK")
+        g.rlog.warn("Error: " + status_msg)
         returnValue(False)
 
     # now try to setup nodding server if appropriate
-    nodpattern = data.get('appdata', {}).get('nodpattern', {})
-    if g.cpars['telins_name'] == 'GTC' and nodpattern:
+    nodpattern = data.get("appdata", {}).get("nodpattern", {})
+    if g.cpars["telins_name"] == "GTC" and nodpattern:
         try:
-            ra_offsets = list(nodpattern['ra'])
-            dec_offsets = list(nodpattern['dec'])
-            yield session.call('hipercam.gtc.rpc.load_nod_pattern', ra_offsets, dec_offsets)
+            ra_offsets = list(nodpattern["ra"])
+            dec_offsets = list(nodpattern["dec"])
+            yield session.call(
+                "hipercam.gtc.rpc.load_nod_pattern", ra_offsets, dec_offsets
+            )
             ok = True
         except Exception as err:
-            status_msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+            status_msg = (
+                err.error_message() if hasattr(err, "error_message") else str(err)
+            )
             ok = False
 
         if not ok:
-            g.clog.warn('Offset Server response was not OK')
-            g.rlog.warn('Error: ' + status_msg)
+            g.clog.warn("Offset Server response was not OK")
+            g.rlog.warn("Error: " + status_msg)
             returnValue(False)
 
-    g.clog.debug('Leaving postJSON')
+    g.clog.debug("Leaving postJSON")
     returnValue(True)
 
 
 @inlineCallbacks
 def createJSON(g, full=True):
     """
     Create JSON compatible dictionary from current settings
 
     Parameters
     ----------
     g :  hcam_drivers.globals.Container
     Container with globals
     """
     data = dict()
-    if 'gps_attached' not in g.cpars:
-        data['gps_attached'] = 1
+    if "gps_attached" not in g.cpars:
+        data["gps_attached"] = 1
     else:
-        data['gps_attached'] = 1 if g.cpars['gps_attached'] else 0
+        data["gps_attached"] = 1 if g.cpars["gps_attached"] else 0
 
-    data['appdata'] = g.ipars.dumpJSON()
-    data['user'] = g.rpars.dumpJSON()
+    data["appdata"] = g.ipars.dumpJSON()
+    data["user"] = g.rpars.dumpJSON()
     if full:
-        data['hardware'] = g.ccd_hw.dumpJSON()
-        data['tcs'] = g.info.dumpJSON()
+        data["hardware"] = g.ccd_hw.dumpJSON()
+        data["tcs"] = g.info.dumpJSON()
+        data["compo"] = g.compo_hw.dumpJSON()
 
-        if g.cpars['telins_name'].lower() == 'gtc':
+        if g.cpars["telins_name"].lower() == "gtc":
             session = g.session
             if session is None:
-                g.clog.warn('no WAMP session, not fetching telescope parameters')
+                g.clog.warn("no WAMP session, not fetching telescope parameters")
             else:
                 try:
-                    telpars = yield session.call('hipercam.gtc.rpc.get_telescope_pars')
-                    data['gtc_headers'] = telpars
+                    telpars = yield session.call("hipercam.gtc.rpc.get_telescope_pars")
+                    data["gtc_headers"] = telpars
                 except Exception as err:
-                    g.clog.warn('cannot get GTC headers from telescope server')
-                    msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+                    g.clog.warn("cannot get GTC headers from telescope server")
+                    msg = (
+                        err.error_message()
+                        if hasattr(err, "error_message")
+                        else str(err)
+                    )
                     g.clog.warn(msg)
     returnValue(data)
 
 
 def jsonFromFits(fname):
     hdr = fits.getheader(fname)
 
     def full_key(key):
-        return 'HIERARCH ESO {}'.format(key)
+        return "HIERARCH ESO {}".format(key)
 
     def get(name, default=None):
         return hdr.get(full_key(name), default)
 
     app_data = dict(
-        multipliers=[1 + get('DET NSKIPS{}'.format(i+1), 0) for i in range(5)],
-        dummy_out=get('DET DUMMY', 0),
-        fastclk=get('DET FASTCLK', 0),
-        oscan=int(get('DET INCPRSCX', False)),
-        oscany=int(get('DET INCOVSCY', False)),
-        readout='Slow' if get('DET SPEED', 0) == 0 else 'Fast',
-        xbin=get('DET BINX1', 1),
-        ybin=get('DET BINY1', 1),
-        clear=int(get('DET CLRCCD', True)),
-        led_flsh=int(get('DET EXPLED', False)),
-        dwell=get('DET TEXPOSE', 0.1)/1000
+        multipliers=[1 + get("DET NSKIPS{}".format(i + 1), 0) for i in range(5)],
+        dummy_out=get("DET DUMMY", 0),
+        fastclk=get("DET FASTCLK", 0),
+        oscan=int(get("DET INCPRSCX", False)),
+        oscany=int(get("DET INCOVSCY", False)),
+        readout="Slow" if get("DET SPEED", 0) == 0 else "Fast",
+        xbin=get("DET BINX1", 1),
+        ybin=get("DET BINY1", 1),
+        clear=int(get("DET CLRCCD", True)),
+        led_flsh=int(get("DET EXPLED", False)),
+        dwell=get("DET TEXPOSE", 0.1) / 1000
         # TODO: numexp
     )
 
     user = dict(
-        Observers=hdr.get('OBSERVER', ''),
-        target=hdr.get('OBJECT', ''),
-        comment=hdr.get('RUNCOM', ''),
-        flags=hdr.get('IMAGETYP', 'data'),
-        filters=hdr.get('FILTERS', 'us,gs,rs,is,zs'),
-        ID=hdr.get('PROGRM', ''),
-        PI=hdr.get('PI', '')
-
+        Observers=hdr.get("OBSERVER", ""),
+        target=hdr.get("OBJECT", ""),
+        comment=hdr.get("RUNCOM", ""),
+        flags=hdr.get("IMAGETYP", "data"),
+        filters=hdr.get("FILTERS", "us,gs,rs,is,zs"),
+        ID=hdr.get("PROGRM", ""),
+        PI=hdr.get("PI", ""),
     )
 
-    mode = get('DET READ CURID')
+    mode = get("DET READ CURID")
     if mode == 2:
         # one window
-        app_data['app'] = 'Windows'
-        app_data['x1size'] = get('DET WIN1 NX')
-        app_data['y1size'] = get('DET WIN1 NY')
-        app_data['x1start_lowerleft'] = get('DET WIN1 XSLL')
-        app_data['x1start_lowerright'] = get('DET WIN1 XSLR')
-        app_data['x1start_upperleft'] = get('DET WIN1 XSUL')
-        app_data['x1start_upperright'] = get('DET WIN1 XSUR')
-        app_data['y1start'] = get('DET WIN1 YS') + 1
+        app_data["app"] = "Windows"
+        app_data["x1size"] = get("DET WIN1 NX")
+        app_data["y1size"] = get("DET WIN1 NY")
+        app_data["x1start_lowerleft"] = get("DET WIN1 XSLL")
+        app_data["x1start_lowerright"] = get("DET WIN1 XSLR")
+        app_data["x1start_upperleft"] = get("DET WIN1 XSUL")
+        app_data["x1start_upperright"] = get("DET WIN1 XSUR")
+        app_data["y1start"] = get("DET WIN1 YS") + 1
     elif mode == 3:
         # two window
-        app_data['app'] = 'Windows'
-        app_data['x1size'] = get('DET WIN1 NX')
-        app_data['y1size'] = get('DET WIN1 NY')
-        app_data['x1start_lowerleft'] = get('DET WIN1 XSLL')
-        app_data['x1start_lowerright'] = get('DET WIN1 XSLR')
-        app_data['x1start_upperleft'] = get('DET WIN1 XSUL')
-        app_data['x1start_upperright'] = get('DET WIN1 XSUR')
-        app_data['y1start'] = get('DET WIN1 YS') + 1
-        app_data['x2size'] = get('DET WIN2 NX')
-        app_data['y2size'] = get('DET WIN2 NY')
-        app_data['x2start_lowerleft'] = get('DET WIN2 XSLL')
-        app_data['x2start_lowerright'] = get('DET WIN2 XSLR')
-        app_data['x2start_upperleft'] = get('DET WIN2 XSUL')
-        app_data['x2start_upperright'] = get('DET WIN2 XSUR')
-        app_data['y2start'] = get('DET WIN2 YS') + 1
+        app_data["app"] = "Windows"
+        app_data["x1size"] = get("DET WIN1 NX")
+        app_data["y1size"] = get("DET WIN1 NY")
+        app_data["x1start_lowerleft"] = get("DET WIN1 XSLL")
+        app_data["x1start_lowerright"] = get("DET WIN1 XSLR")
+        app_data["x1start_upperleft"] = get("DET WIN1 XSUL")
+        app_data["x1start_upperright"] = get("DET WIN1 XSUR")
+        app_data["y1start"] = get("DET WIN1 YS") + 1
+        app_data["x2size"] = get("DET WIN2 NX")
+        app_data["y2size"] = get("DET WIN2 NY")
+        app_data["x2start_lowerleft"] = get("DET WIN2 XSLL")
+        app_data["x2start_lowerright"] = get("DET WIN2 XSLR")
+        app_data["x2start_upperleft"] = get("DET WIN2 XSUL")
+        app_data["x2start_upperright"] = get("DET WIN2 XSUR")
+        app_data["y2start"] = get("DET WIN2 YS") + 1
     elif mode == 4:
         # drift mode
-        app_data['app'] = 'Drift'
-        app_data['x1size'] = get('DET DRWIN NX')
-        app_data['y1size'] = get('DET DRWIN NY')
-        app_data['x1start_left'] = get('DET DRWIN XSL')
-        app_data['x1start_right'] = get('DET DRWIN XSR')
-        app_data['y1start'] = 1 + get('DET DRWIN YS')
+        app_data["app"] = "Drift"
+        app_data["x1size"] = get("DET DRWIN NX")
+        app_data["y1size"] = get("DET DRWIN NY")
+        app_data["x1start_left"] = get("DET DRWIN XSL")
+        app_data["x1start_right"] = get("DET DRWIN XSR")
+        app_data["y1start"] = 1 + get("DET DRWIN YS")
     else:
-        app_data['app'] = 'FullFrame'
+        app_data["app"] = "FullFrame"
 
-    setup_data = dict(
-        appdata=app_data,
-        user=user
-    )
+    setup_data = dict(appdata=app_data, user=user)
     return json.dumps(setup_data)
 
 
 @inlineCallbacks
 def insertFITSHDU(g):
     """
     Uploads a table of TCS data to the servers, which is appended onto a run.
 
     Arguments
     ---------
     g : hcam_drivers.globals.Container
         the Container object of application globals
     """
-    if not g.cpars['hcam_server_on']:
-        g.clog.warn('insertFITSHDU: servers are not active')
+    if not g.cpars["hcam_server_on"]:
+        g.clog.warn("insertFITSHDU: servers are not active")
         returnValue(False)
 
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
     run_number = yield getRunNumber(g)
     tcs_table = g.info.tcs_table
 
-    g.clog.info('Adding TCS table data to run{:04d}.fits'.format(run_number))
+    g.clog.info("Adding TCS table data to run{:04d}.fits".format(run_number))
     try:
         fd = StringIO()
-        ascii.write(tcs_table, format='ecsv', output=fd)
-        yield session.call('hipercam.ngc.rpc.add_hdu', fd.getvalue(), run_number)
+        ascii.write(tcs_table, format="ecsv", output=fd)
+        yield session.call("hipercam.ngc.rpc.add_hdu", fd.getvalue(), run_number)
     except Exception as err:
-        g.clog.warn('insertFITSHDU failed')
-        msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+        g.clog.warn("insertFITSHDU failed")
+        msg = err.error_message() if hasattr(err, "error_message") else str(err)
         g.clog.warn(msg)
     returnValue(True)
 
 
 @inlineCallbacks
 def execCommand(g, command, timeout=10):
     """
@@ -388,222 +390,228 @@
       offline            : put ESO control server in idle state and power down
       standby            : server can communicate, but child processes disabled
       reset              : resets the NGC controller front end
 
     Returns True/False according to whether the command
     succeeded or not.
     """
-    if not g.cpars['hcam_server_on']:
-        g.clog.warn('execCommand: servers are not active')
+    if not g.cpars["hcam_server_on"]:
+        g.clog.warn("execCommand: servers are not active")
         returnValue(False)
 
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
     try:
-        response = yield session.call('hipercam.ngc.rpc.{}'.format(command))
+        response = yield session.call("hipercam.ngc.rpc.{}".format(command))
         if response is not None:
             msg, ok = response
         else:
-            msg = ''
+            msg = ""
             ok = True
         g.clog.info('execCommand, command = "' + command + '"')
 
         if ok:
-            g.clog.info('Response from server was OK')
+            g.clog.info("Response from server was OK")
             returnValue(True)
         else:
-            g.clog.warn('Response from server was not OK')
-            g.clog.warn('Reason: ' + msg)
+            g.clog.warn("Response from server was not OK")
+            g.clog.warn("Reason: " + msg)
             returnValue(False)
     except Exception as err:
-        g.clog.warn('execCommand failed')
-        msg = err.error_message() if hasattr(err, 'error_message') else str(err)
+        g.clog.warn("execCommand failed")
+        msg = err.error_message() if hasattr(err, "error_message") else str(err)
         g.clog.warn(msg)
 
     returnValue(False)
 
 
 @inlineCallbacks
 def isRunActive(g):
     """
     Polls the data server to see if a run is active
     """
-    session = g.session if hasattr(g, 'session') else None
+    session = g.session if hasattr(g, "session") else None
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
-    if g.cpars['hcam_server_on']:
+    if g.cpars["hcam_server_on"]:
         try:
-            response = yield session.call('hipercam.ngc.rpc.summary')
+            response = yield session.call("hipercam.ngc.rpc.summary")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            raise DriverError('isRunActive error reading NGC status: ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            raise DriverError("isRunActive error reading NGC status: " + msg)
         tel = ReadNGCTelemetry(response)
 
         if not tel.ok:
-            raise DriverError('isRunActive error: ' + str(tel.err))
-        if tel.state == 'idle':
+            raise DriverError("isRunActive error: " + str(tel.err))
+        if tel.state == "idle":
             returnValue(False)
-        elif tel.state == 'active':
+        elif tel.state == "active":
             returnValue(True)
-        elif tel.state == 'error':
+        elif tel.state == "error":
             msg = """
             NGC is in error state.
             Try resetting it using 'start_hicam' and 'Power On'
             """
-            raise DriverError('isRunActive error\n' + msg)
+            raise DriverError("isRunActive error\n" + msg)
         else:
-            raise DriverError('isRunActive error, state = ' + tel.state)
+            raise DriverError("isRunActive error, state = " + tel.state)
     else:
-        raise DriverError('isRunActive error: servers are not active')
+        raise DriverError("isRunActive error: servers are not active")
 
 
 @inlineCallbacks
 def isPoweredOn(g):
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
-    if g.cpars['hcam_server_on']:
+    if g.cpars["hcam_server_on"]:
         try:
-            response = yield session.call('hipercam.ngc.rpc.summary')
+            response = yield session.call("hipercam.ngc.rpc.summary")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            raise DriverError('isPoweredOn error reading NGC status: ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            raise DriverError("isPoweredOn error reading NGC status: " + msg)
 
         tel = ReadNGCTelemetry(response)
         if not tel.ok:
-            raise DriverError('isPoweredOn error: ' + str(tel.err))
-        if tel.clocks == 'enabled':
+            raise DriverError("isPoweredOn error: " + str(tel.err))
+        if tel.clocks == "enabled":
             returnValue(True)
         else:
             returnValue(False)
     else:
-        raise DriverError('isPoweredOn error: servers are not active')
+        raise DriverError("isPoweredOn error: servers are not active")
 
 
 @inlineCallbacks
 def isOnline(g):
     # checks if ESO Server is in ONLINE state
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
-    if g.cpars['hcam_server_on']:
+    if g.cpars["hcam_server_on"]:
         try:
-            msg, ok = yield session.call('hipercam.ngc.rpc.status')
+            msg, ok = yield session.call("hipercam.ngc.rpc.status")
         except Exception as err:
-            msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-            raise DriverError('isOnline error: ' + msg)
+            msg = err.error_message() if hasattr(err, "error_message") else str(err)
+            raise DriverError("isOnline error: " + msg)
 
         if not ok:
-            raise DriverError('isOnline error: ' + msg)
-        if msg.lower() == 'online':
+            raise DriverError("isOnline error: " + msg)
+        if msg.lower() == "online":
             returnValue(True)
         else:
             returnValue(False)
     else:
-        raise DriverError('isOnline error: hserver is not active')
+        raise DriverError("isOnline error: hserver is not active")
 
 
 @inlineCallbacks
 def getFrameNumber(g):
     """
     Polls the data server to find the current frame number.
 
     Throws an exceotion if it cannot determine it.
     """
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
-    if not g.cpars['hcam_server_on']:
-        raise DriverError('getRunNumber error: servers are not active')
-    msg, ok = yield session.call('hipercam.ngc.rpc.status', 'DET.FRAM2.NO')
+    if not g.cpars["hcam_server_on"]:
+        raise DriverError("getRunNumber error: servers are not active")
+    msg, ok = yield session.call("hipercam.ngc.rpc.status", "DET.FRAM2.NO")
     if not ok:
-        raise DriverError('getFrameNumber error: could not get frame number ' + msg)
+        raise DriverError("getFrameNumber error: could not get frame number " + msg)
     try:
         frame_no = int(msg)
     except ValueError:
-        raise DriverError('getFrameNumber error: invalid msg ' + msg)
+        raise DriverError("getFrameNumber error: invalid msg " + msg)
     returnValue(frame_no)
 
 
 @inlineCallbacks
 def getRunNumber(g):
     """
     Polls the data server to find the current run number. Throws
     exceptions if it can't determine it.
     """
     session = g.session
     if session is None:
-        g.clog.warn('no WAMP session')
+        g.clog.warn("no WAMP session")
         returnValue(False)
 
-    if not g.cpars['hcam_server_on']:
-        raise DriverError('getRunNumber error: servers are not active')
+    if not g.cpars["hcam_server_on"]:
+        raise DriverError("getRunNumber error: servers are not active")
     try:
-        response = yield session.call('hipercam.ngc.rpc.summary')
+        response = yield session.call("hipercam.ngc.rpc.summary")
     except Exception as err:
-        msg = err.error_message() if hasattr(err, 'error_message') else str(err)
-        raise DriverError('isRunActive error reading NGC status: ' + msg)
+        msg = err.error_message() if hasattr(err, "error_message") else str(err)
+        raise DriverError("isRunActive error reading NGC status: " + msg)
     tel = ReadNGCTelemetry(response)
     if tel.ok:
         returnValue(tel.run)
     else:
-        raise DriverError('getRunNumber error: ' + str(tel.err))
+        raise DriverError("getRunNumber error: " + str(tel.err))
 
 
 def checkSimbad(g, target, maxobj=5, timeout=5):
     """
     Sends off a request to Simbad to check whether a target is recognised.
     Returns with a list of results, or raises an exception if it times out
     """
-    url = 'http://simbad.u-strasbg.fr/simbad/sim-script'
-    q = 'set limit ' + str(maxobj) + \
-        '\nformat object form1 "Target: %IDLIST(1) | %COO(A D;ICRS)"\nquery ' \
+    url = "http://simbad.u-strasbg.fr/simbad/sim-script"
+    q = (
+        "set limit "
+        + str(maxobj)
+        + '\nformat object form1 "Target: %IDLIST(1) | %COO(A D;ICRS)"\nquery '
         + target
-    query = urllib.parse.urlencode({'submit': 'submit script', 'script': q})
+    )
+    query = urllib.parse.urlencode({"submit": "submit script", "script": q})
     resp = urllib.request.urlopen(url, query.encode(), timeout)
     data = False
     error = False
     results = []
     for line in resp:
         line = line.decode()
-        if line.startswith('::data::'):
+        if line.startswith("::data::"):
             data = True
-        if line.startswith('::error::'):
+        if line.startswith("::error::"):
             error = True
-        if data and line.startswith('Target:'):
-            name, coords = line[7:].split(' | ')
+        if data and line.startswith("Target:"):
+            name, coords = line[7:].split(" | ")
             results.append(
-                {'Name': name.strip(), 'Position': coords.strip(),
-                 'Frame': 'ICRS'})
+                {"Name": name.strip(), "Position": coords.strip(), "Frame": "ICRS"}
+            )
     resp.close()
 
     if error and len(results):
-        g.clog.warn('drivers.check: Simbad: there appear to be some ' +
-                    'results but an error was unexpectedly raised.')
+        g.clog.warn(
+            "drivers.check: Simbad: there appear to be some "
+            + "results but an error was unexpectedly raised."
+        )
     return results
 
 
 class FifoThread(threading.Thread):
     """
     Adds a fifo Queue to a thread in order to store up disasters which are
     added to the fifo for later retrieval. This is to get around the problem
     that otherwise exceptions thrown from withins threaded operations are
     lost.
     """
+
     def __init__(self, name, target, fifo, args=()):
         threading.Thread.__init__(self, target=target, args=args)
         self.fifo = fifo
         self.name = name
 
     def run(self):
         """
@@ -611,10 +619,13 @@
         them in the fifo
         """
         try:
             threading.Thread.run(self)
         except Exception:
             t, v, tb = sys.exc_info()
             error = traceback.format_exception_only(t, v)[0][:-1]
-            tback = (self.name + ' Traceback (most recent call last):\n' +
-                     ''.join(traceback.format_tb(tb)))
+            tback = (
+                self.name
+                + " Traceback (most recent call last):\n"
+                + "".join(traceback.format_tb(tb))
+            )
             self.fifo.put((self.name, error, tback))
```

### Comparing `hcam_widgets-1.1.0/hcam_widgets/tcs.py` & `hcam_widgets-1.1.1/hcam_widgets/tcs.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/tkutils.py` & `hcam_widgets-1.1.1/hcam_widgets/tkutils.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/ucam.py` & `hcam_widgets-1.1.1/hcam_widgets/ucam.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/uspec.py` & `hcam_widgets-1.1.1/hcam_widgets/uspec.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets/widgets.py` & `hcam_widgets-1.1.1/hcam_widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/hcam_widgets.egg-info/PKG-INFO` & `hcam_widgets-1.1.1/hcam_widgets.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-widgets
-Version: 1.1.0
+Version: 1.1.1
 Summary: Common Tkinter widgets for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_widgets
-Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_widgets
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_widgets-1.1.0/hcam_widgets.egg-info/SOURCES.txt` & `hcam_widgets-1.1.1/hcam_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_widgets-1.1.0/setup.py` & `hcam_widgets-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_widgets",
-    version="1.1.0",
+    version="1.1.1",
     description="Common Tkinter widgets for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_widgets",
-    download_url="https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.0.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_widgets/archive/v1.1.1.tar.gz",
     packages=["hcam_widgets", "hcam_widgets.compo", "hcam_widgets.hardware"],
     package_dir={"hcam_widgets": "hcam_widgets"},
     include_package_data=True,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
     keywords="hcam_widgets",
```

