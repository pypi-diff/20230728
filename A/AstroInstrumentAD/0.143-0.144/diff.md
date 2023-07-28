# Comparing `tmp/AstroInstrumentAD-0.143.tar.gz` & `tmp/AstroInstrumentAD-0.144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AstroInstrumentAD-0.143.tar", last modified: Fri Jul 28 13:09:15 2023, max compression
+gzip compressed data, was "AstroInstrumentAD-0.144.tar", last modified: Fri Jul 28 14:17:28 2023, max compression
```

## Comparing `AstroInstrumentAD-0.143.tar` & `AstroInstrumentAD-0.144.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.213669 AstroInstrumentAD-0.143/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.212869 AstroInstrumentAD-0.143/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16218 2023-07-28 13:08:16.000000 AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 13:09:15.213531 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 13:09:15.000000 AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.143/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      738 2023-07-28 13:09:15.213727 AstroInstrumentAD-0.143/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 11:28:37.000000 AstroInstrumentAD-0.143/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 13:09:15.213934 AstroInstrumentAD-0.143/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1713 2023-07-28 13:08:34.000000 AstroInstrumentAD-0.143/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.769009 AstroInstrumentAD-0.144/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.768188 AstroInstrumentAD-0.144/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    16791 2023-07-28 14:15:46.000000 AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-28 14:17:28.768878 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-28 14:17:28.000000 AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.144/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-28 14:17:28.769073 AstroInstrumentAD-0.144/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.144/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-28 14:17:28.769300 AstroInstrumentAD-0.144/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1711 2023-07-28 14:17:08.000000 AstroInstrumentAD-0.144/setup.py
```

### Comparing `AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,36 @@
         
         self.config={
         'telescope_diameter':39, #m
         'wavefront_outer_scale':46, #m
         'median_seeing':.68, #arcsec
         'median_seeing_wl':.5, #um
         'simulation_scale':0.01, #arcsec/pixel, default is 0.01
+        'HA_intervals':21, #number of intervals in the HA range to simulate
         'relative_plate_PA_angle':0, #deg, relative angle of the plate/apertures and PA=0. For PA=0 along aperture semi major axis, set to 90 deg
         'centring':0.5, #either 0.5 for mid index, or HA index
         'latitude':-24.6272, #deg
         'temperature':10, #deg C
         'humidity':14.5, #%
         'pressure':750.0 #mBa
         }
         
         self.config.update(kwargs)
         
-    def load_wavelengths(self,wavelengths):
+    def load_wavelengths(self,wavelengths=[]):
         """
 
         """
         self.output['wavelengths']=np.array(wavelengths)
 
-    def load_hour_angles(self,HA_range,declination):
+    def load_hour_angles(self,HA_start=0,HA_end=1,declination=-30):
         """
         
         """
+        HA_range=np.linspace(HA_start,HA_end,self.config['HA_intervals'])
         self.input['HA_range']=HA_range
         self.input['declination']=declination
 
         #latitude needs to be negative for now
         lat = float(self.config['latitude']) * np.pi/180
         dec = declination*np.pi/180
         
@@ -57,39 +59,39 @@
         self.output['airmasses']=np.array(airmasses)
 
         self.input['ZA_range']=diff_func.airmass_to_ZA(airmasses)
         
         para_angles=diff_func.parallatic_angle(np.array(HA_range),dec,lat)
         self.output['raw_para_angles']=np.array(para_angles) #actual PAs    
         
-    def calculate_integration_shifts(self, guide_waveref, aperture_waveref):
-        self.input['guide_waveref']=guide_waveref
-        self.input['aperture_waveref']=aperture_waveref
+    def calculate_integration_shifts(self, guide_wavelength=0, aperture_wavelength=0):
+        self.input['guide_wavelength']=guide_wavelength
+        self.input['aperture_wavelength']=aperture_wavelength
 
         airmasses=self.output['airmasses']
         wavelengths=self.output['wavelengths']
 
         #centring refers to the index of the hour angles at which we centre the aperture/guiding on a wavelength
         if float(self.config['centring']) == 0.5:
             centring_index=int((len(airmasses)-1)/2)
         else:
             centring_index=int(self.config['centring'])
 
-        centre_shift=diff_func.diff_shift(aperture_waveref,airmasses[centring_index],guide_waveref,self.config) #shift of the original aperture centre wavelength from guide wavelength
+        centre_shift=diff_func.diff_shift(aperture_wavelength,airmasses[centring_index],guide_wavelength,self.config) #shift of the original aperture centre wavelength from guide wavelength
         centring_q=self.output['raw_para_angles'][centring_index]
 
         raw_para_angles=self.output['raw_para_angles']
         para_angles=self.output['raw_para_angles'].copy()
         for i in range(0,len(para_angles)): #change in PAs from centring index
             para_angles[i]=para_angles[i]-self.output['raw_para_angles'][centring_index]
 
         shifts_para=[]
         phi=np.deg2rad(float(self.config['relative_plate_PA_angle']))
         for count,airmass in enumerate(airmasses): #for each airmass, calculate AD shift
-            shift_vals=diff_func.diff_shift(wavelengths,airmass,guide_waveref,self.config)  
+            shift_vals=diff_func.diff_shift(wavelengths,airmass,guide_wavelength,self.config)  
             airmass_shifts=[]
 
             for i in range(0,len(shift_vals)):
                 x=(shift_vals[i])*np.sin(raw_para_angles[count])-centre_shift*np.sin(centring_q)
                 y=(shift_vals[i])*np.cos(raw_para_angles[count])-centre_shift*np.cos(centring_q)
                 airmass_shifts.append([x*np.cos(phi)-y*np.sin(phi),y*np.cos(phi)+x*np.sin(phi)])
                 
@@ -109,26 +111,26 @@
         all_PSFs=[]
         all_aligned_PSFs=[]
         
         zero_shifts=np.zeros(np.shape(self.output['shifts'][0]))
 
         for i in range(0,len(self.output['airmasses'])):
             PSFs=diff_func.make_PSFs(PSF_type,self.output['wavelengths'],self.output['shifts'][i],
-                                                        self.output['airmasses'][i],self.input['major_axis'],self.config,beta=moffat_beta)
+                                                        self.output['airmasses'][i],self.input['aperture_major_axis'],self.config,beta=moffat_beta)
             aligned_PSFs=diff_func.make_PSFs(PSF_type,self.output['wavelengths'],zero_shifts,
-                                                          self.output['airmasses'][i],self.input['major_axis'],self.config,beta=moffat_beta)
+                                                          self.output['airmasses'][i],self.input['aperture_major_axis'],self.config,beta=moffat_beta)
             all_PSFs.append(PSFs)
             all_aligned_PSFs.append(aligned_PSFs)
 
         self.output['PSFs']=all_PSFs
         self.output['aligned_PSFs']=all_aligned_PSFs
         
-    def load_aperture(self,major_axis,aperture_type="hexagons",hexagon_radius=1):
-        self.input['major_axis']=major_axis
-        aperture=diff_func.make_aperture(aperture_type,major_axis,self.config,hexagon_radius=hexagon_radius)
+    def load_aperture(self,aperture_major_axis=0,aperture_type="hexagons",hexagon_radius=1):
+        self.input['aperture_major_axis']=aperture_major_axis
+        aperture=diff_func.make_aperture(aperture_type,aperture_major_axis,self.config,hexagon_radius=hexagon_radius)
         self.output['aperture']=aperture
         
     def calculate_integration_transmissions(self):
         convolved_arrays=self.output['PSFs']*self.output['aperture']
         convolved_aligned_arrays=self.output['aligned_PSFs']*self.output['aperture']
         self.output['PSFs_through_aperture']=convolved_arrays
         self.output['aligned_PSFs_through_aperture']=convolved_aligned_arrays
@@ -160,58 +162,58 @@
             plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
             plt.ylabel("Transmission Relative to No-AD")
         if y_axis=='raw':
             y_axis_data=self.output['raw_integration_transmissions']
             plt.ylabel("Raw Transmission")
             plt.plot(self.output['wavelengths'],self.output['no_AD_integration_transmissions'],color='black',linestyle='--',label='No AD Transmission, {}'.format(self.input['PSF_type']))
             
-        plt.axvline(self.input['guide_waveref'],label="Guide = {}um".format(self.input['guide_waveref']),color='black',linestyle='--',linewidth=0.5)
-        plt.axvline(self.input['aperture_waveref'],label="Aperture = {}um".format(self.input['aperture_waveref']),color='C0',linestyle='--',linewidth=0.5)
+        plt.axvline(self.input['guide_wavelength'],label="Guide = {}um".format(self.input['guide_wavelength']),color='black',linestyle='--',linewidth=0.5)
+        plt.axvline(self.input['aperture_wavelength'],label="Aperture = {}um".format(self.input['aperture_wavelength']),color='C0',linestyle='--',linewidth=0.5)
         plt.plot(self.output['wavelengths'],y_axis_data)
         plt.ylim(0,1.1)
         plt.xlabel("Wavelength (um)")
         plt.legend()
         
         fig, ax = plt.subplots(figsize=[5,5]) 
         weights = np.linspace(0, len(self.output['wavelengths'])-1,len(track_indexes))
         norm = mpl.colors.Normalize(vmin=min(weights), vmax=max(weights))
         cmap = mpl.cm.ScalarMappable(norm=norm, cmap='seismic')
-        circle1 = plt.Circle((0, 0), self.input['major_axis']/2, color='black', fill=False, label='Major Axis')
+        circle1 = plt.Circle((0, 0), self.input['aperture_major_axis']/2, color='black', fill=False, label='Major Axis')
         ax.add_patch(circle1)    
         plt.axvline(0,color='black',linestyle='--',linewidth=0.7,label="PA = {}".format(self.config['relative_plate_PA_angle']))
-        plt.scatter(self.output['centre_shift'][0],self.output['centre_shift'][1],label='Guide = {}um'.format(self.input['guide_waveref']),color='black',marker='+')
+        plt.scatter(self.output['centre_shift'][0],self.output['centre_shift'][1],label='Guide = {}um'.format(self.input['guide_wavelength']),color='black',marker='+')
         plt.xlim(-0.4,0.4)
         plt.ylim(-0.4,0.4)
         shifts=self.output['shifts']
         for count,i in enumerate(track_indexes):
             xs,ys=[],[]
             for o in range(0,len(shifts)):
                 xs.append(shifts[o][i][0])
                 ys.append(shifts[o][i][1]) 
             plt.plot(xs,ys,marker='x',color=cmap.to_rgba(weights[count]),label="{}um".format(round(self.output['wavelengths'][i],4)))
         plt.legend()
         plt.xlabel("x (arcsec)")
         plt.ylabel("y (arcsec)")
 
-    def load_ZA(self, ZA_range):
+    def load_ZA(self, ZA_range=[]):
         """
         """
         airmasses=diff_func.ZA_to_airmass(ZA_range)
         self.output['airmasses']=airmasses
         self.input['ZA_range']=ZA_range
     
-    def calculate_snapshot_shifts(self,aperture_waveref):
-        self.input['aperture_waveref']=aperture_waveref
+    def calculate_snapshot_shifts(self,aperture_wavelength):
+        self.input['aperture_wavelength']=aperture_wavelength
     
         airmasses=self.output['airmasses']
         wavelengths=self.output['wavelengths']
         
         shifts=[]
         for count,airmass in enumerate(airmasses):
-            centre_shift=diff_func.diff_shift(aperture_waveref,airmass,1,self.config)
+            centre_shift=diff_func.diff_shift(aperture_wavelength,airmass,1,self.config)
             airmass_shifts=diff_func.diff_shift(wavelengths,airmass,1,self.config)-centre_shift
             airmass_shifts=np.append(np.resize(airmass_shifts,(len(airmass_shifts),1)),np.zeros((len(airmass_shifts),1)),axis=-1)
             shifts.append(airmass_shifts)
         self.output['shifts']=shifts
         
     def calculate_snapshot_transmissions(self):
         convolved_arrays=self.output['PSFs']*self.output['aperture']
@@ -233,45 +235,45 @@
             y_data=self.output['relative_transmissions']
             plt.axhline(y=1,label='No AD Transmission, {}'.format(self.input['PSF_type']),color='black',linestyle='--')
             plt.ylabel("Transmission Relative to No-AD")
         if y_axis=='raw':
             y_data=self.output['raw_transmissions']
             plt.ylabel("Raw Transmission")
         
-        plt.axvline(self.input['aperture_waveref'],label="Aperture = {}um".format(self.input['aperture_waveref']),color='C0',linestyle='--',linewidth=0.5)
+        plt.axvline(self.input['aperture_wavelength'],label="Aperture = {}um".format(self.input['aperture_wavelength']),color='C0',linestyle='--',linewidth=0.5)
         for count,trans in enumerate(y_data):
             plt.plot(self.output['wavelengths'],trans,label="ZA = {} deg".format(round(self.input['ZA_range'][count],1)))
         plt.ylabel("Transmission Relative to No-AD")
         plt.ylim(0,1.1)
         plt.xlabel("Wavelength (um)")
         plt.legend()   
     
-    def run(self,hour_angles,declination,wavelengths,major_axis,guide=0,aperture=0,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
+    def run(self,HA_start=0,HA_end=1,declination=-30,wavelengths=[],aperture_major_axis=[],guide_wavelength=0,aperture_wavelength=0,aperture_type="hexagons",hexagon_radius=1,PSF_type="moffat",moffat_beta=2.5,y_axis="relative",track_indexes=[0,-1],**kwargs):
         self.config.update(kwargs)
-        self.load_hour_angles(hour_angles,declination)
-        self.load_wavelengths(wavelengths)
-        self.load_aperture(major_axis)
-        if guide==0 or aperture ==0:
+        self.load_hour_angles(HA_start=HA_start,HA_end=HA_end,declination=declination)
+        self.load_wavelengths(wavelengths=wavelengths)
+        self.load_aperture(aperture_major_axis=aperture_major_axis)
+        if guide_wavelength==0 or aperture_wavelength ==0:
             print("Optimising Guide/Aperture Wavelength")
             self.optimise_integration(np.arange(wavelengths[0],wavelengths[-1],0.1),np.arange(wavelengths[0],wavelengths[-1],0.1),guide_aperture="equal")
-            print("Optimal Guide/Aperture = {}um (nearest 0.1um)".format(self.input['guide_waveref']))
+            print("Optimal Guide/Aperture = {}um (nearest 0.1um)".format(self.input['guide_wavelength']))
         else:
+            self.calculate_integration_shifts(guide_wavelength=guide_wavelength,aperture_wavelength=aperture_wavelength)
             self.load_PSFs()
-            self.calculate_integration_shifts(guide,aperture)
             self.calculate_integration_transmissions()
         self.integration_plots()
             
-    def optimise_integration(self,guide_options,aperture_options,guide_aperture="independent"):
+    def optimise_integration(self,guide_options=[],aperture_options=[],guide_aperture="independent"):
         if guide_aperture=="independent":
             metrics=np.zeros((len(guide_options),len(aperture_options),3))
             performance_metrics=np.zeros((len(guide_options),len(aperture_options),3))
             best_performance_metric=0
             for guide_count,guide in enumerate(guide_options):
                 for aperture_count,aperture in enumerate(aperture_options):
-                    self.calculate_integration_shifts(guide,aperture)
+                    self.calculate_integration_shifts(guide_wavelength=guide,aperture_wavelength=aperture)
                     self.load_PSFs()
                     self.calculate_integration_transmissions()
                     metric=diff_func.integ_metrics(self.output['relative_integration_transmissions'])
                     
                     metrics[guide_count][aperture_count]=metric
                     performance_metric=metrics[guide_count][aperture_count][0]*metrics[guide_count][aperture_count][2]**2
                     performance_metrics[guide_count][aperture_count]=performance_metric
@@ -283,15 +285,15 @@
                         best_metric=metric
                         
         if guide_aperture=="equal":
             metrics=np.zeros((len(guide_options),3))
             performance_metrics=np.zeros((len(guide_options),3))
             best_performance_metric=0
             for guide_count,guide in enumerate(guide_options):
-                self.calculate_integration_shifts(guide,guide)
+                self.calculate_integration_shifts(guide_wavelength=guide,aperture_wavelength=guide)
                 self.load_PSFs()
                 self.calculate_integration_transmissions()
                 metric=diff_func.integ_metrics(self.output['relative_integration_transmissions'])
                 
                 metrics[guide_count]=metric
                 performance_metric=metrics[guide_count][0]*metrics[guide_count][2]**2
                 performance_metrics[guide_count]=performance_metric
@@ -307,9 +309,8 @@
         print("Max Transmission = {}%".format(round(100*best_metric[1])))
         print("Throughput = {}%".format(round(100*best_metric[2])))
          
         self.calculate_integration_shifts(round(best_guide,5),round(best_aperture,5))
         self.load_PSFs()
         self.calculate_integration_transmissions()
  
-        return
-            
+        return
```

### Comparing `AstroInstrumentAD-0.143/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.144/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.143/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.144/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.143
-Summary: # A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
+Version: 0.144
+Summary: A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AstroInstrumentAD-0.143/PKG-INFO` & `AstroInstrumentAD-0.144/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.143
-Summary: # A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
+Version: 0.144
+Summary: A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AstroInstrumentAD-0.143/setup.py` & `AstroInstrumentAD-0.144/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.143',      # Start with a small number and increase it with every change you make
+  version = '0.144',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = '# A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.',   # Give a short description about your library
+  description = 'A Python package to calculate the throughput of a spectrograph impacted by atmospheric atmospheric dispersion.',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
```

