# Comparing `tmp/sdss_cherno-0.6.2.tar.gz` & `tmp/sdss_cherno-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.6.2.tar", max compression
+gzip compressed data, was "sdss_cherno-0.6.3.tar", max compression
```

## Comparing `sdss_cherno-0.6.2.tar` & `sdss_cherno-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1504 2023-04-28 18:04:40.338639 sdss_cherno-0.6.2/LICENSE.md
--rw-r--r--   0        0        0     2723 2023-04-28 18:04:40.339034 sdss_cherno-0.6.2/README.md
--rw-r--r--   0        0        0     1251 2023-04-28 18:04:40.339429 sdss_cherno-0.6.2/cherno/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-28 18:04:40.339759 sdss_cherno-0.6.2/cherno/__main__.py
--rw-r--r--   0        0        0      747 2023-04-28 18:04:40.340146 sdss_cherno-0.6.2/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4493 2023-04-28 18:04:40.340499 sdss_cherno-0.6.2/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2023-04-28 18:04:40.340708 sdss_cherno-0.6.2/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2023-04-28 18:04:40.341112 sdss_cherno-0.6.2/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2023-04-28 18:04:40.341605 sdss_cherno-0.6.2/cherno/actor/commands/config.py
--rw-r--r--   0        0        0     8213 2023-04-28 18:04:40.342068 sdss_cherno-0.6.2/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2023-04-28 18:04:40.342558 sdss_cherno-0.6.2/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1007 2023-04-28 18:04:40.343170 sdss_cherno-0.6.2/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2023-04-28 18:04:40.343621 sdss_cherno-0.6.2/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3119 2023-04-28 18:04:40.344119 sdss_cherno-0.6.2/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2023-04-28 18:04:40.344473 sdss_cherno-0.6.2/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2023-04-28 18:04:40.344830 sdss_cherno-0.6.2/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2023-04-28 18:04:40.345393 sdss_cherno-0.6.2/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2023-04-28 18:04:40.345836 sdss_cherno-0.6.2/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10857 2023-04-28 18:04:40.346392 sdss_cherno-0.6.2/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2023-04-28 18:04:40.346871 sdss_cherno-0.6.2/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2023-04-28 18:04:40.347215 sdss_cherno-0.6.2/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     1994 2023-04-28 18:04:40.347555 sdss_cherno-0.6.2/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     1958 2023-04-28 18:04:40.347909 sdss_cherno-0.6.2/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     5688 2023-04-28 18:04:40.348383 sdss_cherno-0.6.2/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2023-04-28 18:04:40.348845 sdss_cherno-0.6.2/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2023-04-28 18:04:40.349269 sdss_cherno-0.6.2/cherno/extraction.py
--rw-r--r--   0        0        0    40346 2023-04-28 18:04:40.349909 sdss_cherno-0.6.2/cherno/guider.py
--rw-r--r--   0        0        0     4175 2023-04-28 18:04:40.350366 sdss_cherno-0.6.2/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2023-04-28 18:04:40.350707 sdss_cherno-0.6.2/cherno/maskbits.py
--rw-r--r--   0        0        0     4738 2023-04-28 18:04:40.351065 sdss_cherno-0.6.2/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2023-04-28 18:04:40.351435 sdss_cherno-0.6.2/cherno/utils.py
--rw-r--r--   0        0        0     2314 2023-04-28 18:04:40.360969 sdss_cherno-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 sdss_cherno-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-28 16:27:02.842402 sdss_cherno-0.6.3/LICENSE.md
+-rw-r--r--   0        0        0     2723 2023-07-28 16:27:02.842997 sdss_cherno-0.6.3/README.md
+-rw-r--r--   0        0        0     1251 2023-07-28 16:27:02.843575 sdss_cherno-0.6.3/cherno/__init__.py
+-rw-r--r--   0        0        0     2207 2023-07-28 16:27:02.844069 sdss_cherno-0.6.3/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2023-07-28 16:27:02.844606 sdss_cherno-0.6.3/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     4493 2023-07-28 16:27:02.845108 sdss_cherno-0.6.3/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2023-07-28 16:27:02.845392 sdss_cherno-0.6.3/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-07-28 16:27:02.846040 sdss_cherno-0.6.3/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2023-07-28 16:27:02.846591 sdss_cherno-0.6.3/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0     8213 2023-07-28 16:27:02.847066 sdss_cherno-0.6.3/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2023-07-28 16:27:02.847505 sdss_cherno-0.6.3/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1007 2023-07-28 16:27:02.847947 sdss_cherno-0.6.3/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2023-07-28 16:27:02.848467 sdss_cherno-0.6.3/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3119 2023-07-28 16:27:02.848966 sdss_cherno-0.6.3/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2023-07-28 16:27:02.849402 sdss_cherno-0.6.3/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2023-07-28 16:27:02.849828 sdss_cherno-0.6.3/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2023-07-28 16:27:02.850242 sdss_cherno-0.6.3/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2023-07-28 16:27:02.850658 sdss_cherno-0.6.3/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10857 2023-07-28 16:27:02.851126 sdss_cherno-0.6.3/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2023-07-28 16:27:02.851633 sdss_cherno-0.6.3/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2023-07-28 16:27:02.852116 sdss_cherno-0.6.3/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     2040 2023-07-28 16:27:02.852563 sdss_cherno-0.6.3/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     2005 2023-07-28 16:27:02.853011 sdss_cherno-0.6.3/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2023-07-28 16:27:02.853449 sdss_cherno-0.6.3/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2023-07-28 16:27:02.853883 sdss_cherno-0.6.3/cherno/exceptions.py
+-rw-r--r--   0        0        0    14028 2023-07-28 16:27:02.854407 sdss_cherno-0.6.3/cherno/extraction.py
+-rw-r--r--   0        0        0    42170 2023-07-28 16:27:02.855095 sdss_cherno-0.6.3/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2023-07-28 16:27:02.855592 sdss_cherno-0.6.3/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2023-07-28 16:27:02.856057 sdss_cherno-0.6.3/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2023-07-28 16:27:02.856569 sdss_cherno-0.6.3/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2023-07-28 16:27:02.857026 sdss_cherno-0.6.3/cherno/utils.py
+-rw-r--r--   0        0        0     2314 2023-07-28 16:27:02.869485 sdss_cherno-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 sdss_cherno-0.6.3/PKG-INFO
```

### Comparing `sdss_cherno-0.6.2/LICENSE.md` & `sdss_cherno-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/README.md` & `sdss_cherno-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/__init__.py` & `sdss_cherno-0.6.3/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/__main__.py` & `sdss_cherno-0.6.3/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/__init__.py` & `sdss_cherno-0.6.3/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/actor.py` & `sdss_cherno-0.6.3/cherno/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/acquire.py` & `sdss_cherno-0.6.3/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/config.py` & `sdss_cherno-0.6.3/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/guide.py` & `sdss_cherno-0.6.3/cherno/actor/commands/guide.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/offset.py` & `sdss_cherno-0.6.3/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/reprocess.py` & `sdss_cherno-0.6.3/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/scale.py` & `sdss_cherno-0.6.3/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/set.py` & `sdss_cherno-0.6.3/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/show.py` & `sdss_cherno-0.6.3/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/status.py` & `sdss_cherno-0.6.3/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/stop.py` & `sdss_cherno-0.6.3/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/commands/version.py` & `sdss_cherno-0.6.3/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/actor/exposer.py` & `sdss_cherno-0.6.3/cherno/actor/exposer.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/etc/cherno_APO.yml` & `sdss_cherno-0.6.3/cherno/etc/cherno_APO.yml`

 * *Files 3% similar despite different names*

```diff
@@ -71,28 +71,30 @@
 guider:
   cpulimit: 15
   astrometry_net_config: etc/astrometrynet_APO.cfg
   astrometry_net_use_all_regions: true
   astrometry_dir: ./astrometry
   focus_r2_threshold: 0.2
   fit_focus: true
-  plot_focus: true
+  plot_focus: false
   auto_radec_min: -1
   use_astrometry_net: true
   astrometry_net_odds: 9
   gaia_connection_string: postgresql://sdss_user@sdss5-db/chernodb
   gaia_phot_g_mean_mag_max: 19
   gaia_search_radius: 0.09
   gaia_use_cross_correlation_shift: true
   gaia_cross_correlation_blur: 1
   gaia_cross_correlation_min_error: 0.6
   gaia_distance_upper_bound: 5
   fit_all_detections: true
   fit_rms_sigma: 2
-  plot_rms: true
+  plot_rms: false
+  max_delta_scale_ppm: 1000
+  max_fit_rms: 2
 
 extraction:
   output_dir: ./extraction
   method: marginal
   plot: false
   rejection_method: sigclip
   reject_sigma: 2.0
@@ -101,10 +103,10 @@
     background_sigma: 3.0
     min_npix: 15
   marginal:
     background_sigma: 5.0
     minarea: 15
     max_detections: 50
 
-default_offset: [0.0, -0.1, -432]
+default_offset: [0.0, 0.0, -420]
 
 observatory: ${OBSERVATORY}
```

### Comparing `sdss_cherno-0.6.2/cherno/etc/cherno_LCO.yml` & `sdss_cherno-0.6.3/cherno/etc/cherno_LCO.yml`

 * *Files 8% similar despite different names*

```diff
@@ -71,28 +71,30 @@
 guider:
   cpulimit: 15
   astrometry_net_config: etc/astrometrynet_LCO.cfg
   astrometry_net_use_all_regions: false
   astrometry_dir: ./astrometry
   focus_r2_threshold: 0.2
   fit_focus: false
-  plot_focus: true
+  plot_focus: false
   auto_radec_min: 2
   use_astrometry_net: true
   astrometry_net_odds: 9
   gaia_connection_string: postgresql://sdss_user@sdss5-db/chernodb
   gaia_phot_g_mean_mag_max: 19
   gaia_search_radius: 0.05
   gaia_use_cross_correlation_shift: true
   gaia_cross_correlation_blur: 1
   gaia_cross_correlation_min_error: 0.6
   gaia_distance_upper_bound: 100
   fit_all_detections: true
   fit_rms_sigma: 2
-  plot_rms: true
+  plot_rms: false
+  max_delta_scale_ppm: 1000
+  max_fit_rms: 2
 
 extraction:
   output_dir: ./extraction
   method: marginal
   plot: false
   rejection_method: sigclip
   reject_sigma: 3.0
@@ -101,10 +103,10 @@
     background_sigma: 3.0
     min_npix: 15
   marginal:
     background_sigma: 5.0
     minarea: 15
     max_detections: 50
 
-default_offset: [0, 0, -375]
+default_offset: [0, 0, -365]
 
 observatory: ${OBSERVATORY}
```

### Comparing `sdss_cherno-0.6.2/cherno/etc/schema.json` & `sdss_cherno-0.6.3/cherno/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/exceptions.py` & `sdss_cherno-0.6.3/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/extraction.py` & `sdss_cherno-0.6.3/cherno/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/guider.py` & `sdss_cherno-0.6.3/cherno/guider.py`

 * *Files 6% similar despite different names*

```diff
@@ -418,29 +418,29 @@
                 f"Only {len(solved)} cameras solved. Only fitting RA/Dec. "
                 "The rotation and scale offsets are informational-only "
                 "and not corrected."
             )
 
         fit_cameras = [d.camera_id for d in solved]
         fit_rms_sigma = config["guider"].get("fit_rms_sigma", 3)
-        guider_fit = None
+        guider_fit = False
         while True:
             tmp_guider_fit = self.fitter.fit(
                 field_ra,
                 field_dec,
                 field_pa,
                 offset=full_offset,
                 scale_rms=scale_rms,
                 only_radec=only_radec,
                 cameras=fit_cameras,
             )
 
             # If we already had a solution and this fit failed or the fit RMS is bad,
             # just use the previous fit.
-            if guider_fit is not None and (fit_rms_sigma <= 0 or not tmp_guider_fit):
+            if guider_fit is not False and (fit_rms_sigma <= 0 or not tmp_guider_fit):
                 break
 
             # Update the fit with the previous one.
             guider_fit = tmp_guider_fit
 
             # If the fit failed, exit.
             if guider_fit is False:
@@ -467,18 +467,22 @@
             fit_cameras.remove(cam_max_rms)
 
         plate_scale = defaults.PLATE_SCALE[self.observatory]
         mm_to_arcsec = 1 / plate_scale * 3600
 
         exp_no = solved[0].exposure_no  # Should be the same for all.
 
-        if not guider_fit:
-            rms = delta_ra = delta_dec = delta_rot = delta_scale = -999.0
-            ast_solution.guider_fit = None
-        else:
+        if guider_fit:
+            # If we have a guider_fit != False, the fit produced a good astrometric
+            # solution.
+            ast_solution.valid_solution = True
+
+            # Now unpack fit information. We do this even if we reject the
+            # fit below because we want the fit data in the headers, but
+            # won't apply the correction.
             delta_ra = guider_fit.delta_ra
             delta_dec = guider_fit.delta_dec
             delta_rot = guider_fit.delta_rot
             delta_scale = guider_fit.delta_scale
 
             xrms = numpy.round(guider_fit.xrms * mm_to_arcsec, 3)
             yrms = numpy.round(guider_fit.yrms * mm_to_arcsec, 3)
@@ -489,25 +493,65 @@
 
             self.command.info(guide_rms=[exp_no, xrms, yrms, rms])
 
             # Store RMS. This is used to determine acquisition convergence.
             if self.command.actor and rms > 0 and rms < 1:
                 self.command.actor.state.rms_history.append(rms)
 
-        ast_solution.valid_solution = True
+            if guider_fit.only_radec:
+                ast_solution.fit_mode = "radec"
+
+            # Report fit RMS. First value is the global fit RMS, then one for
+            # each camera and a boolean indicating if that camera was used for the
+            # global fit. If a camera was rejected the fit RMS is set to -999.
+            fit_rms = guider_fit.fit_rms
+            fit_rms_camera = [numpy.round(fit_rms.loc[0].rms * mm_to_arcsec, 4)]
+            for cid in range(1, 7):
+                if cid in fit_rms.index:
+                    this_fit_rms = numpy.round(fit_rms.loc[cid].rms * mm_to_arcsec, 4)
+                    fit_rms_camera.append(this_fit_rms)
+                else:
+                    fit_rms_camera.append(-999.0)
+                fit_rms_camera.append(cid in guider_fit.cameras)
+
+            self.command.info(fit_rms_camera=fit_rms_camera)
+
+            # If the fit_rms of all the fit cameras is greater than a certain
+            # threshold, reject the fit. This can happen in cases when the
+            # telescope is moving during an exposure.
+            max_fit_rms = config["guider"]["max_fit_rms"]  # In arcsec
+            if guider_fit:
+                fit_rms = guider_fit.fit_rms.loc[fit_cameras, "rms"] * mm_to_arcsec
+                if numpy.all(fit_rms > max_fit_rms):
+                    self.command.warning(
+                        "The fit RMS of all the cameras exceeds "
+                        "threshold values. Rejecting fit."
+                    )
+                    ast_solution.valid_solution = False
+
+            # Check the delta_scale. If the change is too large, this is probably
+            # a misfit. Reject the fit.
+            max_delta_scale_ppm = config["guider"]["max_delta_scale_ppm"]
+            delta_scale_ppm = abs(1 - guider_fit.delta_scale) * 1e6  # Parts per million
+            if delta_scale_ppm > max_delta_scale_ppm:
+                self.command.warning("Scale change exceeds limits. Rejecting fit.")
+                ast_solution.valid_solution = False
 
+        else:
+            rms = delta_ra = delta_dec = delta_rot = delta_scale = -999.0
+            ast_solution.guider_fit = None
+            ast_solution.valid_solution = False
+
+        # Update AstrometricSolution object.
         ast_solution.delta_ra = float(delta_ra)
         ast_solution.delta_dec = float(delta_dec)
         ast_solution.delta_rot = float(delta_rot)
         ast_solution.delta_scale = float(delta_scale)
         ast_solution.rms = float(rms)
 
-        if guider_fit and guider_fit.only_radec:
-            ast_solution.fit_mode = "radec"
-
         if fit_focus:
             try:
                 fwhm_fit, x_min, a, b, c, r2 = focus_fit(
                     [d.e_data for d in data],
                     plot=config["guider"]["plot_focus"],
                 )
 
@@ -519,25 +563,14 @@
                 ast_solution.delta_focus = round(-x_min / focus_sensitivity, 1)
                 ast_solution.focus_coeff = [a, b, c]
                 ast_solution.focus_r2 = round(r2, 3)
 
             except Exception as err:
                 self.command.warning(f"Failed fitting focus curve: {err}.")
 
-        if guider_fit:
-            fit_rms = guider_fit.fit_rms
-            fit_rms_camera = [numpy.round(fit_rms.loc[0].rms * mm_to_arcsec, 4)]
-            for cid in range(1, 7):
-                rms_cam = fit_rms.loc[cid].rms if cid in fit_rms.index else -999.0
-                fit_rms_camera += [
-                    numpy.round(rms_cam * mm_to_arcsec, 4) if rms_cam != -999 else -999,
-                    cid in guider_fit.cameras,
-                ]
-            self.command.info(fit_rms_camera=fit_rms_camera)
-
         self.command.info(
             astrometry_fit=[
                 exp_no,
                 len(solved),
                 -999.0,
                 -999.0,
                 numpy.round(fwhm, 2),
@@ -976,15 +1009,15 @@
             guide_data.solved = True
             guide_data.solve_method = "gaia"
             guide_data.wcs = wcs
 
     async def write_proc_image(
         self,
         guide_data: GuideData,
-        outpath: PathLike = None,
+        outpath: PathLike | None = None,
         overwrite: bool = False,
     ):
         """Writes the proc-gimg image."""
 
         ext_data = guide_data.extraction_data
 
         proc_hdu = fits.open(str(guide_data.path)).copy()
```

### Comparing `sdss_cherno-0.6.2/cherno/lcotcc.py` & `sdss_cherno-0.6.3/cherno/lcotcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/maskbits.py` & `sdss_cherno-0.6.3/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/tcc.py` & `sdss_cherno-0.6.3/cherno/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/cherno/utils.py` & `sdss_cherno-0.6.3/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.2/pyproject.toml` & `sdss_cherno-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.6.2"
+version = "0.6.3"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
```

### Comparing `sdss_cherno-0.6.2/PKG-INFO` & `sdss_cherno-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.6.2
+Version: 0.6.3
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.9,<3.12
@@ -12,16 +12,14 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.0.0,<6.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sdss-clu (>=1.8.0,<2.0.0)
```

