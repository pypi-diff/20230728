# Comparing `tmp/BroadSword-0.2.0.tar.gz` & `tmp/BroadSword-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.2.0.tar", last modified: Wed Jul 26 21:07:37 2023, max compression
+gzip compressed data, was "BroadSword-0.2.1.tar", last modified: Fri Jul 28 16:51:58 2023, max compression
```

## Comparing `BroadSword-0.2.0.tar` & `BroadSword-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 21:07:25.000000 BroadSword-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-26 21:07:37.052719 BroadSword-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-26 21:07:25.000000 BroadSword-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-26 21:07:25.000000 BroadSword-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 21:07:37.056719 BroadSword-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    55658 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices_ARM64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/libmatrices_x86_64.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-26 21:07:25.000000 BroadSword-0.2.0/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:07:37.052719 BroadSword-0.2.0/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 21:07:37.000000 BroadSword-0.2.0/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:07:36.000000 BroadSword-0.2.0/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 16:51:39.000000 BroadSword-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-28 16:51:58.070477 BroadSword-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-28 16:51:39.000000 BroadSword-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 16:51:39.000000 BroadSword-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-28 16:51:58.074478 BroadSword-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.066477 BroadSword-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    57155 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-28 16:51:39.000000 BroadSword-0.2.1/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:51:58.070477 BroadSword-0.2.1/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 16:51:58.000000 BroadSword-0.2.1/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:51:57.000000 BroadSword-0.2.1/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.2.0/LICENSE` & `BroadSword-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.0/PKG-INFO` & `BroadSword-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,48 +43,45 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
-broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="XAS_Fe_Nitrogen.csv",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2",headerlines=[0,0,0]) 
 broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
 broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
 broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
-
 # broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
-# Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
-# Then add the new argument XESbandScaling into initResolution()
-# broad.printBands()
-# XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
-
 # Shift the spectra until the calculation aligns with the experimental
 broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
-# Optionally you can shift specific bands in XES.
-# Add the new argument into Shift()
-# XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
-
 # Broaden the spectra
 broad.broaden(separate=False)
-
 # Export the broadened calculated spectra
 # broad.export(filename="GeP2N4",element="N",individual=False)
+
+# Optionally you can scale and shift specific bands in XES. Use printBands() to determine where the bands are located.
+# Then add the new argument XESbandScaling into initResolution() and XESbandshift int Shift()
+#broad.printBands()
+#broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5,XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
+#broad.Shift(XESshift=19.2,XASshift=20.2,separate=False,XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
+#broad.broaden(separate=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
 def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
-# Loads the measured experimental data. Fermi energy is from the calculated ground state
+# Loads the measured experimental data. Fermi energy is from the calculated ground state.
+# Use headerlines to specify the number of lines to ignore in [XES, XANES] respectively.
 
 def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
 # Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
 # Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
@@ -93,19 +90,19 @@
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
 def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
-# separate describes whether or not to create a separate plot for XES and XAS
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def broaden(self, separate=True)
-# Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
-# separate describes whether or not to create a separate plot for XES and XAS
+# Broadens the calculated spectra.
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
 # Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
 # Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
 ### Post Script
```

### Comparing `BroadSword-0.2.0/README.md` & `BroadSword-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,48 +28,45 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
-broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="XAS_Fe_Nitrogen.csv",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2",headerlines=[0,0,0]) 
 broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
 broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
 broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
-
 # broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
-# Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
-# Then add the new argument XESbandScaling into initResolution()
-# broad.printBands()
-# XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
-
 # Shift the spectra until the calculation aligns with the experimental
 broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
-# Optionally you can shift specific bands in XES.
-# Add the new argument into Shift()
-# XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
-
 # Broaden the spectra
 broad.broaden(separate=False)
-
 # Export the broadened calculated spectra
 # broad.export(filename="GeP2N4",element="N",individual=False)
+
+# Optionally you can scale and shift specific bands in XES. Use printBands() to determine where the bands are located.
+# Then add the new argument XESbandScaling into initResolution() and XESbandshift int Shift()
+#broad.printBands()
+#broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5,XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
+#broad.Shift(XESshift=19.2,XASshift=20.2,separate=False,XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
+#broad.broaden(separate=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
 def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
-# Loads the measured experimental data. Fermi energy is from the calculated ground state
+# Loads the measured experimental data. Fermi energy is from the calculated ground state.
+# Use headerlines to specify the number of lines to ignore in [XES, XANES] respectively.
 
 def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
 # Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
 # Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
@@ -78,19 +75,19 @@
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
 def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
-# separate describes whether or not to create a separate plot for XES and XAS
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def broaden(self, separate=True)
-# Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
-# separate describes whether or not to create a separate plot for XES and XAS
+# Broadens the calculated spectra.
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
 # Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
 # Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
 ### Post Script
```

### Comparing `BroadSword-0.2.0/setup.cfg` & `BroadSword-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.2.0
+version = 0.2.1
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls =
```

### Comparing `BroadSword-0.2.0/src/BroadSword/BroadSword.py` & `BroadSword-0.2.1/src/BroadSword/BroadSword.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,36 +84,62 @@
             Header lines are allowed, as long as they are specified properly in the function.
         GS_fermi : float
             Specify the fermi energy for the ground state calculated spectra. Found in .scf2
         headerlines : [int]
             Specify the number of headerlines for the XES and XANES files respectively. 
         """
 
-        with open(basedir+"/"+XES, "r") as xesFile: # Measured XES
-            df = pd.read_csv(xesFile, delimiter='\s+',header=None, skiprows=headerlines[0]) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook
-            c1 = 0
-            maxEXP = 0
-            for i in range(len(df)): 
-                ExpSXS[0][c1][0] = df[0][c1] # Energy
-                ExpSXS[1][c1][0] = df[1][c1] # Counts
-                if ExpSXS[1][c1][0] > maxEXP:
-                    maxEXP = ExpSXS[1][c1][0] # Get max value in experimental XES
-                c1 += 1
-            ExpSXSCount[0] = c1 # Length of data points
-            for i in range(ExpSXSCount[0]): # Normalize spectra
-                ExpSXS[1][i][0] = ExpSXS[1][i][0]/maxEXP
-
-        with open(basedir+"/"+XANES, "r") as xanesFile: # Measured XANES
-            df = pd.read_csv(xanesFile, delimiter='\s+',header=None, skiprows=headerlines[1])
-            c1 = 0
-            for i in range(len(df)):
-                ExpSXS[0][c1][1] = df[0][c1] # Energy
-                ExpSXS[1][c1][1] = df[1][c1] # Counts
-                c1 += 1
-            ExpSXSCount[1] = c1 # Length of data points
+        try:
+            with open(basedir+"/"+XES, "r") as xesFile: # Measured XES
+                df = pd.read_csv(xesFile, delimiter='\s+', header=None, skiprows=headerlines[0]) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook
+                c1 = 0
+                maxEXP = 0
+                for i in range(len(df)): 
+                    ExpSXS[0][c1][0] = df[0][c1] # Energy
+                    ExpSXS[1][c1][0] = df[1][c1] # Counts
+                    if ExpSXS[1][c1][0] > maxEXP:
+                        maxEXP = ExpSXS[1][c1][0] # Get max value in experimental XES
+                    c1 += 1
+                ExpSXSCount[0] = c1 # Length of data points
+                for i in range(ExpSXSCount[0]): # Normalize spectra
+                    ExpSXS[1][i][0] = ExpSXS[1][i][0]/maxEXP
+        except:
+            with open(basedir+"/"+XES, "r") as xesFile: # Measured XES
+                # This trys it as a .csv instead of a .txt
+                df = pd.read_csv(xesFile, header=None, skiprows=headerlines[0]) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook                
+                c1 = 0
+                maxEXP = 0
+                for i in range(len(df)): 
+                    ExpSXS[0][c1][0] = df[0][c1] # Energy
+                    ExpSXS[1][c1][0] = df[1][c1] # Counts
+                    if ExpSXS[1][c1][0] > maxEXP:
+                        maxEXP = ExpSXS[1][c1][0] # Get max value in experimental XES
+                    c1 += 1
+                ExpSXSCount[0] = c1 # Length of data points
+                for i in range(ExpSXSCount[0]): # Normalize spectra
+                    ExpSXS[1][i][0] = ExpSXS[1][i][0]/maxEXP
+        try:
+            with open(basedir+"/"+XANES, "r") as xanesFile: # Measured XANES
+                df = pd.read_csv(xanesFile, delimiter='\s+', header=None, skiprows=headerlines[1])
+                c1 = 0
+                for i in range(len(df)):
+                    ExpSXS[0][c1][1] = df[0][c1] # Energy
+                    ExpSXS[1][c1][1] = df[1][c1] # Counts
+                    c1 += 1
+                ExpSXSCount[1] = c1 # Length of data points
+        except:
+            with open(basedir+"/"+XANES, "r") as xanesFile: # Measured XANES
+                # This trys it as a .csv instead of a .txt
+                df = pd.read_csv(xanesFile, header=None, skiprows=headerlines[1])
+                c1 = 0
+                for i in range(len(df)):
+                    ExpSXS[0][c1][1] = df[0][c1] # Energy
+                    ExpSXS[1][c1][1] = df[1][c1] # Counts
+                    c1 += 1
+                ExpSXSCount[1] = c1 # Length of data points
         
         global CalcSXSCase
         global Fermi
         global Edge
         CalcSXSCase = 0 # Stores number of calculated inequivalent sites
         Edge = []
         Fermi = GS_fermi
```

### Comparing `BroadSword-0.2.0/src/BroadSword/libmatrices.so` & `BroadSword-0.2.1/src/BroadSword/libmatrices.so`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.0/src/BroadSword/libmatrices_ARM64.dylib` & `BroadSword-0.2.1/src/BroadSword/libmatrices_ARM64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.0/src/BroadSword/libmatrices_x86_64.dylib` & `BroadSword-0.2.1/src/BroadSword/libmatrices_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.0/src/BroadSword/matrices.c` & `BroadSword-0.2.1/src/BroadSword/matrices.c`

 * *Files identical despite different names*

### Comparing `BroadSword-0.2.0/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.2.1/src/BroadSword.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,48 +43,45 @@
 from bokeh.io import output_notebook
 output_notebook(hide_banner=True)
 
 # Create an instance of the class
 broad = Broaden()
 
 # Load the experimental and calculations
-broad.loadExp(basedir,XES="N_test_XES.txt",XANES="N_test_XAS.txt",GS_fermi=0.44996547,headerlines=[2,2])
-broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2")
+broad.loadExp(basedir,XES="N_test_XES.txt",XANES="XAS_Fe_Nitrogen.csv",GS_fermi=0.44996547,headerlines=[2,2])
+broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.176237,XANES="N1_half.txspec",ES_fermi=0.45062079,sites=1,edge="L2",headerlines=[0,0,0]) 
 broad.loadCalc(basedir,XES="N2_emis.txspec",XAS="N2_abs.txspec",GS_bindingEnergy=27.177975,XANES="N2_half.txspec",ES_fermi=0.45091878)
 broad.loadCalc(basedir,XES="N3_emis.txspec",XAS="N3_abs.txspec",GS_bindingEnergy=27.122234,XANES="N3_half.txspec",ES_fermi=0.45090808)
 broad.loadCalc(basedir,XES="N4_emis.txspec",XAS="N4_abs.txspec",GS_bindingEnergy=27.177070,XANES="N4_half.txspec",ES_fermi=0.45088602)
-
 # broad.loadCalc(basedir,XES="N1_emis.txspec",XAS="N1_abs.txspec",GS_bindingEnergy=27.177070) # Minimum required inputs to broaden a spectra.
 
 # Initialize the broadening parameters
 broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5)
-# Optionally you can scale specific bands in XEN. Use printBands() to determine where the bands are located.
-# Then add the new argument XESbandScaling into initResolution()
-# broad.printBands()
-# XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
-
 # Shift the spectra until the calculation aligns with the experimental
 broad.Shift(XESshift=19.2,XASshift=20.2,separate=False)
-# Optionally you can shift specific bands in XES.
-# Add the new argument into Shift()
-# XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
-
 # Broaden the spectra
 broad.broaden(separate=False)
-
 # Export the broadened calculated spectra
 # broad.export(filename="GeP2N4",element="N",individual=False)
+
+# Optionally you can scale and shift specific bands in XES. Use printBands() to determine where the bands are located.
+# Then add the new argument XESbandScaling into initResolution() and XESbandshift int Shift()
+#broad.printBands()
+#broad.initResolution(corelifetime=0.15,specResolution=1200,monoResolution=5000,disorder=0.5,XESscaling=0.5,XASscaling=0.5,XESbandScaling=[[0.1,0.2,0.2,0.4],[0.2,0.2,0.4,0.2],[0.3,0.2,0.1,0.5],[0.3,0.5,0.4,0.2]])
+#broad.Shift(XESshift=19.2,XASshift=20.2,separate=False,XESbandshift=[[30,33,30,20],[15,19.2,19.2,19.2],[30,33,30,20],[15,19.2,19.2,19.2]])
+#broad.broaden(separate=False)
 ```
 
 ### Functions
 Below are the functions with their input criteria. If needed the docstrings will appear in Jupyter notebook using "shift+tab"
 
 ```
 def loadExp(self, basedir, XES, XANES, GS_fermi, headerlines=[0,0]):
-# Loads the measured experimental data. Fermi energy is from the calculated ground state
+# Loads the measured experimental data. Fermi energy is from the calculated ground state.
+# Use headerlines to specify the number of lines to ignore in [XES, XANES] respectively.
 
 def loadCalc(self, basedir, XES, XAS, GS_bindingEnergy, XANES=0, ES_fermi=0,  edge="K", sites=1, headerlines=[0,0,0]):
 # Loads the calculated data. The header lines are an array describing the number of header lines in the [XES, XAS, XANES] respectively.
 # Fermis is the energy from the calculated excited state. Binding is from the ground state.
 # Specifying the edge and number of sites are only required if they differ from the K edge and you have a different number of atoms between different inequivalent atoms.
 
 def printBands(self):
@@ -93,19 +90,19 @@
 def initResolution(self, corelifetime, specResolution, monoResolution, disorder, XESscaling, XASscaling, XESbandScaling=0)
 # Specifies the broadening parameters based on instrument, general disorder, and lifetime broadening.
 # An optional variable to scale the bands individually is available
 
 def Shift(self,XESshift, XASshift, XESbandshift=0, separate=False):
 # Shifts the calculated spectra based on user input.
 # An optional variable to shift the bands individually is available
-# separate describes whether or not to create a separate plot for XES and XAS
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def broaden(self, separate=True)
-# Broadens the calculated spectra. The library path will need to specified as described in the Installation segment
-# separate describes whether or not to create a separate plot for XES and XAS
+# Broadens the calculated spectra.
+# 'separate' describes whether or not to create a separate plot for XES and XAS
 
 def export(self, filename, element, individual=False)
 # Exports the broadened data as a .csv file.
 # Set the filename and then the elemental edge, as well as if the broadened spectra for each individual inequivalent site should be export.
 # Ex: filename=C3N3, element=N, ouput would be C3N3_N_XES.csv
 ```
 ### Post Script
```

