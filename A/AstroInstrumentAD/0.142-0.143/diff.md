# Comparing `tmp/AstroInstrumentAD-0.142.tar.gz` & `tmp/AstroInstrumentAD-0.143.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroInstrumentAD-0.142.tar", last modified: Fri Jul 28 13:02:16 2023, max compression
+gzip compressed data, was "AstroInstrumentAD-0.143.tar", last modified: Fri Jul 28 13:09:15 2023, max compression
```

## Comparing `AstroInstrumentAD-0.142.tar` & `AstroInstrumentAD-0.143.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:02:16.517185 AstroInstrumentAD-0.142/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:02:16.516415 AstroInstrumentAD-0.142/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16057 2023-07-28 13:01:06.000000 AstroInstrumentAD-0.142/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-18 11:24:25.000000 AstroInstrumentAD-0.142/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:02:16.517061 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:02:16.000000 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 13:02:16.000000 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 13:02:16.000000 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 13:02:16.000000 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 13:02:16.000000 AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.142/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:02:16.517243 AstroInstrumentAD-0.142/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 11:28:37.000000 AstroInstrumentAD-0.142/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 13:02:16.517453 AstroInstrumentAD-0.142/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1713 2023-07-28 13:01:20.000000 AstroInstrumentAD-0.142/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.213669 AstroInstrumentAD-0.143/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.212869 AstroInstrumentAD-0.143/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16218 2023-07-28 13:08:16.000000 AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.213531 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.143/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:09:15.213727 AstroInstrumentAD-0.143/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 11:28:37.000000 AstroInstrumentAD-0.143/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 13:09:15.213934 AstroInstrumentAD-0.143/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1713 2023-07-28 13:08:34.000000 AstroInstrumentAD-0.143/setup.py
```

### Comparing `AstroInstrumentAD-0.142/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,28 +250,31 @@
         self.load_hour_angles(hour_angles,declination)
         self.load_wavelengths(wavelengths)
         self.load_aperture(major_axis)
         if guide==0 or aperture ==0:
             print("Optimising Guide/Aperture Wavelength")
             self.optimise_integration(np.arange(wavelengths[0],wavelengths[-1],0.1),np.arange(wavelengths[0],wavelengths[-1],0.1),guide_aperture="equal")
             print("Optimal Guide/Aperture = {}um (nearest 0.1um)".format(self.input['guide_waveref']))
-
+        else:
+            self.load_PSFs()
+            self.calculate_integration_shifts(guide,aperture)
+            self.calculate_integration_transmissions()
         self.integration_plots()
             
     def optimise_integration(self,guide_options,aperture_options,guide_aperture="independent"):
         if guide_aperture=="independent":
             metrics=np.zeros((len(guide_options),len(aperture_options),3))
             performance_metrics=np.zeros((len(guide_options),len(aperture_options),3))
             best_performance_metric=0
             for guide_count,guide in enumerate(guide_options):
                 for aperture_count,aperture in enumerate(aperture_options):
                     self.calculate_integration_shifts(guide,aperture)
                     self.load_PSFs()
                     self.calculate_integration_transmissions()
-                    metric=diff_func.integ_metric(self.output['relative_integration_transmissions'])
+                    metric=diff_func.integ_metrics(self.output['relative_integration_transmissions'])
                     
                     metrics[guide_count][aperture_count]=metric
                     performance_metric=metrics[guide_count][aperture_count][0]*metrics[guide_count][aperture_count][2]**2
                     performance_metrics[guide_count][aperture_count]=performance_metric
                     
                     if performance_metric > best_performance_metric:
                         best_performance_metric=performance_metric
@@ -283,15 +286,15 @@
             metrics=np.zeros((len(guide_options),3))
             performance_metrics=np.zeros((len(guide_options),3))
             best_performance_metric=0
             for guide_count,guide in enumerate(guide_options):
                 self.calculate_integration_shifts(guide,guide)
                 self.load_PSFs()
                 self.calculate_integration_transmissions()
-                metric=diff_func.integ_metric(self.output['relative_integration_transmissions'])
+                metric=diff_func.integ_metrics(self.output['relative_integration_transmissions'])
                 
                 metrics[guide_count]=metric
                 performance_metric=metrics[guide_count][0]*metrics[guide_count][2]**2
                 performance_metrics[guide_count]=performance_metric
                 
                 if performance_metric > best_performance_metric:
                     best_performance_metric=performance_metric
```

### Comparing `AstroInstrumentAD-0.142/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.142/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.142
+Version: 0.143
 Summary: # A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
```

### Comparing `AstroInstrumentAD-0.142/PKG-INFO` & `AstroInstrumentAD-0.143/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.142
+Version: 0.143
 Summary: # A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
```

### Comparing `AstroInstrumentAD-0.142/setup.py` & `AstroInstrumentAD-0.143/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.142',      # Start with a small number and increase it with every change you make
+  version = '0.143',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = '# A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
```

