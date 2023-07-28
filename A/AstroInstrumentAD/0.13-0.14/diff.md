# Comparing `tmp/AstroInstrumentAD-0.13.tar.gz` & `tmp/AstroInstrumentAD-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AstroInstrumentAD-0.13.tar", last modified: Tue Jun  6 11:21:24 2023, max compression
+gzip compressed data, was "AstroInstrumentAD-0.14.tar", last modified: Fri Jul 28 11:14:41 2023, max compression
```

## Comparing `AstroInstrumentAD-0.13.tar` & `AstroInstrumentAD-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    13027 2023-06-06 11:19:57.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7301 2023-06-06 09:14:03.000000 AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       25 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.13/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      628 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.13/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-06-06 11:21:24.000000 AstroInstrumentAD-0.13/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1584 2023-06-06 11:21:14.000000 AstroInstrumentAD-0.13/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 11:14:41.213680 AstroInstrumentAD-0.14/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 11:14:41.205914 AstroInstrumentAD-0.14/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16034 2023-07-18 11:24:14.000000 AstroInstrumentAD-0.14/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-18 11:24:25.000000 AstroInstrumentAD-0.14/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 11:14:41.210573 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      737 2023-07-28 11:14:41.000000 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 11:14:41.000000 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 11:14:41.000000 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 11:14:41.000000 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 11:14:41.000000 AstroInstrumentAD-0.14/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.14/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      737 2023-07-28 11:14:41.214052 AstroInstrumentAD-0.14/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       20 2023-06-06 10:14:46.000000 AstroInstrumentAD-0.14/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 11:14:41.214813 AstroInstrumentAD-0.14/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1712 2023-07-28 11:11:10.000000 AstroInstrumentAD-0.14/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.14/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
-import AstroInstrumentAD.dispersion_functions as diff_func
+import dispersion_functions as diff_func
 import matplotlib as mpl
 
 class AD_simulation:
     def __init__(self,**kwargs):
         self.input={}
         self.output={}
         
@@ -241,17 +241,72 @@
         for count,trans in enumerate(y_data):
             plt.plot(self.output['wavelengths'],trans,label="ZA = {} deg".format(round(self.input['ZA_range'][count],1)))
         plt.ylabel("Transmission Relative to No-AD")
         plt.ylim(0,1.1)
         plt.xlabel("Wavelength (um)")
         plt.legend()   
     
-    def run(self,hour_angles,declination,wavelengths,major_axis,guide,aperture,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
+    def run(self,hour_angles,declination,wavelengths,major_axis,guide=0,aperture=0,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
         self.config.update(kwargs)
         self.load_hour_angles(hour_angles,declination)
         self.load_wavelengths(wavelengths)
-        self.calculate_integration_shifts(guide,aperture)
         self.load_aperture(major_axis)
+        if guide==0 or aperture ==0:
+            print("Optimising Guide/Aperture Wavelength")
+            self.optimise_integration(np.arange(wavelengths[0],wavelengths[-1],0.1),np.arange(wavelengths[0],wavelengths[-1],0.1),guide_aperture="equal")
+            print("Optimal Guide/Aperture = {}um (nearest 0.1um)".format(self.input['guide_waveref']))
+
+        self.integration_plots()
+            
+    def optimise_integration(self,guide_options,aperture_options,guide_aperture="independent"):
+        if guide_aperture=="independent":
+            metrics=np.zeros((len(guide_options),len(aperture_options),3))
+            performance_metrics=np.zeros((len(guide_options),len(aperture_options),3))
+            best_performance_metric=0
+            for guide_count,guide in enumerate(guide_options):
+                for aperture_count,aperture in enumerate(aperture_options):
+                    self.calculate_integration_shifts(guide,aperture)
+                    self.load_PSFs()
+                    self.calculate_integration_transmissions()
+                    metric=diff_func.integ_metric(self.output['relative_integration_transmissions'])
+                    
+                    metrics[guide_count][aperture_count]=metric
+                    performance_metric=metrics[guide_count][aperture_count][0]*metrics[guide_count][aperture_count][2]**2
+                    performance_metrics[guide_count][aperture_count]=performance_metric
+                    
+                    if performance_metric > best_performance_metric:
+                        best_performance_metric=performance_metric
+                        best_guide=guide
+                        best_aperture=aperture
+                        best_metric=metric
+                        
+        if guide_aperture=="equal":
+            metrics=np.zeros((len(guide_options),3))
+            performance_metrics=np.zeros((len(guide_options),3))
+            best_performance_metric=0
+            for guide_count,guide in enumerate(guide_options):
+                self.calculate_integration_shifts(guide,guide)
+                self.load_PSFs()
+                self.calculate_integration_transmissions()
+                metric=diff_func.integ_metric(self.output['relative_integration_transmissions'])
+                
+                metrics[guide_count]=metric
+                performance_metric=metrics[guide_count][0]*metrics[guide_count][2]**2
+                performance_metrics[guide_count]=performance_metric
+                
+                if performance_metric > best_performance_metric:
+                    best_performance_metric=performance_metric
+                    best_guide=guide
+                    best_aperture=guide
+                    best_metric=metric  
+        
+        print("Optimal Metrics:")
+        print("Min Transmission = {}%".format(round(best_metric[0]*100)))
+        print("Max Transmission = {}%".format(round(100*best_metric[1])))
+        print("Throughput = {}%".format(round(100*best_metric[2])))
+         
+        self.calculate_integration_shifts(round(best_guide,5),round(best_aperture,5))
         self.load_PSFs()
         self.calculate_integration_transmissions()
-        self.integration_plots()
+ 
+        return
```

### Comparing `AstroInstrumentAD-0.13/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.14/AstroInstrumentAD/dispersion_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import math
 import numpy as np
 from astropy.modeling.models import Moffat2D
 from astropy.modeling.functional_models import Disk2D
 from matplotlib.path import Path
+import scipy
+from scipy import integrate
 
 def calculate_FWHM(wavelength,airmass,config):
     D = float(config['telescope_diameter'])
     L0 = float(config['wavefront_outer_scale'])
     median_seeing = float(config['median_seeing'])
     median_seeing_wl = float(config['median_seeing_wl'])
        
@@ -204,8 +206,17 @@
         xmax=len(PSF)
     if ymax > len(PSF):
         ymax=len(PSF)    
     
     if ymax > 0 and xmax > 0 and xmax - xmin_old > 0 and ymax - ymin_old > 0: 
         resized_data[ymin-ymin_old:ymax-ymin_old,xmin-xmin_old:xmax-xmin_old]=PSF[ymin:ymax,xmin:xmax]
     
-    return resized_data
+    return resized_data
+
+def integ_metrics(transmission):
+
+    metric=[]
+    metric.append(min(transmission))
+    metric.append(max(transmission))
+    metric.append(scipy.integrate.simpson(transmission)/(len(transmission)-1))
+
+    return metric
```

### Comparing `AstroInstrumentAD-0.13/setup.py` & `AstroInstrumentAD-0.14/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.13',      # Start with a small number and increase it with every change you make
+  version = '0.14',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
+  description = '# A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
-  author_email = 'Jay.Stephan@stfc.ac.uk',      # Type in your E-Mail
+  author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
-  keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
+  keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
           'astropy',
+          'scipy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.7',      #Specify which pyhton versions that you want to support
```

