# Comparing `tmp/ptzipcam-0.0.6.tar.gz` & `tmp/ptzipcam-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptzipcam-0.0.6.tar", last modified: Wed May 10 16:58:44 2023, max compression
+gzip compressed data, was "ptzipcam-0.1.0.tar", last modified: Fri Jul 28 21:16:56 2023, max compression
```

## Comparing `ptzipcam-0.0.6.tar` & `ptzipcam-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/
--rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/LICENSE
--rw-rw-r--   0 ian       (1000) ian       (1000)     3935 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/README.md
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/ptzipcam/
--rw-rw-r--   0 ian       (1000) ian       (1000)       89 2023-05-10 16:55:32.000000 ptzipcam-0.0.6/ptzipcam/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/convert.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4111 2023-04-27 22:48:11.000000 ptzipcam-0.0.6/ptzipcam/io.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/logs.py
--rw-rw-r--   0 ian       (1000) ian       (1000)    17536 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/ptz_camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/tracker.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/ui.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/video_writer.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/ptzipcam.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     3935 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       37 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/setup.cfg
--rw-rw-r--   0 ian       (1000) ian       (1000)     1472 2023-05-10 16:55:26.000000 ptzipcam-0.0.6/setup.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-07-28 21:16:56.964234 ptzipcam-0.1.0/
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/LICENSE
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3935 2023-07-28 21:16:56.964234 ptzipcam-0.1.0/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/README.md
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-07-28 21:16:56.960234 ptzipcam-0.1.0/ptzipcam/
+-rw-rw-r--   0 ian       (1000) ian       (1000)       89 2023-07-28 20:44:29.000000 ptzipcam-0.1.0/ptzipcam/__init__.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/convert.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4111 2023-04-27 22:48:11.000000 ptzipcam-0.1.0/ptzipcam/io.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/logs.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    20652 2023-07-28 20:45:30.000000 ptzipcam-0.1.0/ptzipcam/ptz_camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/tracker.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/ui.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-23 20:49:22.000000 ptzipcam-0.1.0/ptzipcam/video_writer.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-07-28 21:16:56.960234 ptzipcam-0.1.0/ptzipcam.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3935 2023-07-28 21:16:56.000000 ptzipcam-0.1.0/ptzipcam.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-07-28 21:16:56.000000 ptzipcam-0.1.0/ptzipcam.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-07-28 21:16:56.000000 ptzipcam-0.1.0/ptzipcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       37 2023-07-28 21:16:56.000000 ptzipcam-0.1.0/ptzipcam.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-07-28 21:16:56.000000 ptzipcam-0.1.0/ptzipcam.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-07-28 21:16:56.964234 ptzipcam-0.1.0/setup.cfg
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1472 2023-05-10 16:55:26.000000 ptzipcam-0.1.0/setup.py
```

### Comparing `ptzipcam-0.0.6/LICENSE` & `ptzipcam-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/PKG-INFO` & `ptzipcam-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptzipcam
-Version: 0.0.6
+Version: 0.1.0
 Summary: Package for controlling PTZ IP cameras that support ONVIF
 Author: Ian Ingram
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ptzipcam-0.0.6/README.md` & `ptzipcam-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/camera.py` & `ptzipcam-0.1.0/ptzipcam/camera.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/convert.py` & `ptzipcam-0.1.0/ptzipcam/convert.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/io.py` & `ptzipcam-0.1.0/ptzipcam/io.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/logs.py` & `ptzipcam-0.1.0/ptzipcam/logs.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/ptz_camera.py` & `ptzipcam-0.1.0/ptzipcam/ptz_camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,143 @@
-"""Tools for control of pan-tilt-zoom functionality of the camera
+"""Tools for control of pan-tilt-zoom functionality of PTZ IP camera
 
 """
-
+import logging
 import time
 
 import numpy as np
 from onvif import ONVIFCamera
 
 from camml import draw
 
+log = logging.getLogger(__name__)
+
 
 def _check_zeroness(number):
     """Almost-zero check
 
     Checks if a number is very close to zero (within a window) and if
     it is makes it less close by placing it at the edge of that
     window.
 
     Parameters
     ----------
-
     number : float
-
         A number to be checked for closeness to zero
 
     Returns
     -------
-
     number : float
-
         The "fixed" number
 
     """
     e = .001
 
-    if number < e and number > -e:
+    if -e < number < e:
         return 0
     else:
         return number
 
 
 class MotorController():
+    """Base class for motor controllers
+
+    """
+    # pylint: disable='too-few-public-methods'
 
     def __init__(self,
                  pid_gains,
                  orientation,
                  example_frame):
+        """Constructor for MotorController class
+
+        """
 
         self.pid_gains = pid_gains
         self.orientation = orientation
 
         self.frame_width = example_frame.shape[1]
         self.frame_height = example_frame.shape[0]
 
         self.total_frame_pixels = self.frame_width * self.frame_height
 
-    def calc_errors(self,
-                    target_lbox):
-        xc, yc = draw.box_to_coords(target_lbox['box'],
-                                    return_kind='center')
-        ret = draw.box_to_coords(target_lbox['box'])
-        self.box_x, self.box_y, self.box_width, self.box_height = ret
-        x_err = self.frame_width/2 - xc
-        y_err = self.frame_height/2 - yc
-
-        # normalize errors
-        x_err = x_err/self.frame_width
-        y_err = y_err/self.frame_height
+    def _calc_errors(self,
+                     target_lbox):
+        """Calculate errors from box coordinates
+
+        Given a labeled box that is the bounding box of a detected
+        target, this function calculates an error for each of x and y
+        (pan and tilt) based on the offset of the centroid of the
+        bounding box from the center of the frame.
+
+        """
+        if target_lbox:
+            x_c, y_c = draw.box_to_coords(target_lbox['box'],
+                                          return_kind='center')
+            ret = draw.box_to_coords(target_lbox['box'])
+            self.box_x, self.box_y, self.box_width, self.box_height = ret
+            x_err = self.frame_width/2 - x_c
+            y_err = self.frame_height/2 - y_c
+
+            # normalize errors
+            x_err = x_err/self.frame_width
+            y_err = y_err/self.frame_height
+        else:
+            x_err = 0.0
+            y_err = 0.0
 
         return x_err, y_err
 
-    def update(self, x_err, y_err, zoom_command):
+    def update(self, target_lbox, zoom_command):
+        """Update the camera commands
+
+        Generates commands for pan, tilt, and zoom given the current
+        target_lbox (which is None when no detection) and the current
+        zoom_command.
+
+        Parameters
+        ----------
+        target_lbox :
+
+        zoom_command : float
+            Current zoom_command
+
+        Returns
+        -------
+        x_velocity :
+
+        y_velocity :
+
+        zoom_command :
+
+        """
+        errors = self._calc_errors(target_lbox)
+        x_err, y_err = errors
+
         if self.orientation == 'down':
             x_err = -x_err
             y_err = -y_err
 
         x_velocity = self._calc_command(x_err, self.pid_gains[0])
         y_velocity = self._calc_command(y_err, self.pid_gains[1])
-        zoom_command = self._calc_zoom_command(x_err, y_err, zoom_command)
+        zoom_command = self._calc_zoom_command(target_lbox,
+                                               x_err,
+                                               y_err,
+                                               zoom_command)
+
+        log.debug('x_err: %.2f || y_err: %.2f', x_err, y_err)
+        log.debug('x_vel: %.2f || y_vel: %.2f', x_velocity, y_velocity)
+        log.debug('zoom_command: %.2f', zoom_command)
 
         return (x_velocity, y_velocity, zoom_command)
 
     def _ensure_command_in_bounds(self, command):
+        """Util to force command is within necessary bounds
+
+        """
         if command >= 1.0:
             command = 1.0
         if command <= -1.0:
             command = -1.0
 
         return command
 
@@ -99,118 +151,130 @@
         be pursued.
 
         """
         command = k * err
         command = self._ensure_command_in_bounds(command)
         return command
 
-    def _calc_zoom_command(self, x_err, y_err, zoom_command):
+    def _calc_zoom_command(self, target_lbox, x_err, y_err, zoom_command):
+        """Calculate the next zoom command
+
+        Not implemented in the base class. But should be implemented
+        to effect zoom control based on position/size of target_lbox.
+
+        """
         raise NotImplementedError
 
 
 class CalmMotorController(MotorController):
+    """MotorController with calm movements/behaviors
+
+    In certain instances, the desire is not for rapid and exacting
+    tracking but for tracking that doesn't distract from the scene
+    through quick movements and jitteriness.  This subclass is
+    intended to be that sort of calm tracker.
+
+    """
 
     def __init__(self,
                  pid_gains,
                  orientation,
-                 example_frame,
-                 zoom_pickup=.01):
+                 example_frame):
 
         super().__init__(pid_gains,
                          orientation,
                          example_frame)
 
-        self.zoom_pickup = zoom_pickup
-        self.ZOOM_STOP_RATIO = .7
-        self.STOP_RANGE = .1
+        self.zoom_stop_ratio = .6
+        self.stop_range = .1
 
     def _calc_command(self, err, k):
         """Override controller command method
 
         The meat here is that the controller stops moving axis under
         control if error is inside of some range.  This range is
         currently hardcoded but maybe should be given as an argument
         to the constructor.
 
         """
 
-        if np.abs(err) < self.STOP_RANGE:
+        if np.abs(err) < self.stop_range:
             command = 0
         else:
             command = k * err
 
         command = self._ensure_command_in_bounds(command)
 
         return command
 
-    def _calc_zoom_command(self, x_err, y_err, zoom_command):
+    def _calc_zoom_command(self, target_lbox, x_err, y_err, zoom_command):
         """Calculate the zoom command give pan/tilt errors
 
+        This is where most of the behavior of the tracking is
+        implemented.
+
         """
 
-        if x_err != 0.0 and y_err != 0.0:
+        if (x_err <= 0.5 and y_err <= 0.5
+           and target_lbox):
             target_bb_pixels = self.box_width * self.box_height
 
-            # if x_err < 50 and y_err < 50:
-            # if x_err != 0 and x_err < 50 and y_err < 50:
-            if (target_bb_pixels / self.total_frame_pixels) < .3:
-                zoom_command += self.zoom_pickup
-                if zoom_command >= 1.0:
-                    zoom_command = 1.0
-                # zoom_command = 1.0
+            box_ratio = target_bb_pixels / self.total_frame_pixels
+            log.debug('Ratio of box to whole %.2f', box_ratio)
+
+            if box_ratio < .3:
+                zoom_command = 1.0
             else:
                 zoom_command = 0.0
 
-            ratio = self.ZOOM_STOP_RATIO
-            filling_much_of_width = self.box_width >= ratio * self.frame_width
-            filling_much_of_height = self.box_height >= ratio * self.frame_height
-            if filling_much_of_width or filling_much_of_height:
+            ratio = self.zoom_stop_ratio
+            spans_much_width = self.box_width >= ratio * self.frame_width
+            spans_much_height = self.box_height >= ratio * self.frame_height
+            if spans_much_width or spans_much_height:
                 zoom_command = 0.0
 
-            margin = 100
-            if((self.box_y + self.box_height) >= (self.frame_height - margin)
+            margin = 20
+            if ((self.box_y + self.box_height) >= (self.frame_height - margin)
                or (self.box_y <= margin)):
-                zoom_command = 0.0
+                zoom_command = -1.0
 
         return zoom_command
 
 
 class TwitchyMotorController(MotorController):
 
     def __init__(self,
                  pid_gains,
                  orientation,
-                 example_frame,
-                 zoom_pickup=.01):
+                 example_frame):
 
         super().__init__(pid_gains,
                          orientation,
                          example_frame)
 
-        self.zoom_pickup = zoom_pickup
-        self.ZOOM_STOP_RATIO = .7
+        self.zoom_stop_ratio = .7
 
-    def _calc_zoom_command(self, x_err, y_err, zoom_command):
+    def _calc_zoom_command(self, target_lbox, x_err, y_err, zoom_command):
         """Calculate the zoom command give pan/tilt errors
 
         """
         if x_err != 0.0 and y_err != 0.0:
             target_bb_pixels = self.box_width * self.box_height
 
             # ratio of bb pixels over whole frame pixels is below a
             # threshold then zoom
             ratio = target_bb_pixels / self.total_frame_pixels
             error = 1 - ratio
             zoom_command = 0.05 * error
 
             # stop zoom if either dimension of bounding box is
-            length_ratio = self.ZOOM_STOP_RATIO
-            filling_much_of_width = self.box_width >= length_ratio * self.frame_width
-            filling_much_of_height = self.box_height >= length_ratio * self.frame_height
-            if filling_much_of_width or filling_much_of_height:
+            l_ratio = self.zoom_stop_ratio  # length ratio
+            spans_much_width = self.box_width >= l_ratio * self.frame_width
+            spans_much_height = self.box_height >= l_ratio * self.frame_height
+            if spans_much_width or spans_much_height:
                 zoom_command = -0.1
 
             # margin = 100
             # if((self.box_y + self.box_height) >= (self.frame_height - margin)
             #    or (self.box_y <= margin)):
             #     zoom_command = 0.0
         else:
@@ -220,25 +284,23 @@
 
 
 class BouncyZoomMotorController(MotorController):
 
     def __init__(self,
                  pid_gains,
                  orientation,
-                 example_frame,
-                 zoom_pickup=.01):
+                 example_frame):
 
         super().__init__(pid_gains,
                          orientation,
                          example_frame)
 
-        self.zoom_pickup = zoom_pickup
-        self.ZOOM_STOP_RATIO = .7
+        self.zoom_stop_ratio = .7
 
-    def _calc_zoom_command(self, x_err, y_err, zoom_command):
+    def _calc_zoom_command(self, target_lbox, x_err, y_err, zoom_command):
         """Calculate the zoom command give pan/tilt errors
 
         """
         if x_err != 0.0 and y_err != 0.0:
             target_bb_pixels = self.box_width * self.box_height
 
             # ratio of bb pixels over whole frame pixels is below a
@@ -260,34 +322,34 @@
     """Class to control PTZ on ONVIF-compliant PTZ IP Camera
 
     Allows control of the pan, tilt, and zoom of an ONVIF-compliant IP
     camera that has PTZ capability.
 
     """
     def __init__(self,
-                 ip=None,
+                 ip_address=None,
                  port='80',
                  user=None,
                  pword=None):
         """ PtzCam constructor
 
         Parameters
         ----------
-        ip : str
+        ip_address : str
            The IP address of the camera to connect to.
         port : str
            ONVIF port on the camera. This is usually 80
         user : str
            Valid username of account on the IP camera being connected to.
         pword : str
            Password for the account on the IP camera.
 
         """
 
-        mycam = ONVIFCamera(ip, port, user, pword)
+        mycam = ONVIFCamera(ip_address, port, user, pword)
         media_service = mycam.create_media_service()
         self.ptz_service = mycam.create_ptz_service()
         self.imaging_service = mycam.create_imaging_service()
 
         # on hikvision cameras there have been 3 profiles: one for each stream
         self.media_profile = media_service.GetProfiles()[0]
 
@@ -322,19 +384,19 @@
     def __del__(self):
         print('[INFO] PtzCam object deletion.')
 
     def get_exposure(self):
         vst = {'VideoSourceToken': self.video_source.token}
         self.imaging_settings = self.imaging_service.GetImagingSettings(vst)
 
-        time = self.imaging_settings.Exposure.ExposureTime
+        exp_time = self.imaging_settings.Exposure.ExposureTime
         gain = self.imaging_settings.Exposure.Gain
         iris = self.imaging_settings.Exposure.Iris
 
-        return time, gain, iris
+        return exp_time, gain, iris
 
     def _send_imaging_settings(self):
         command_dict = {'VideoSourceToken': self.video_source.token,
                         'ImagingSettings': self.imaging_settings}
         self.imaging_service.SetImagingSettings(command_dict)
 
     def set_exposure_to_auto(self):
@@ -442,27 +504,24 @@
 
     def absmove_w_zoom(self, pan_pos, tilt_pos, zoom_pos):
         """Move PTZ camera to an absolute pan, tilt, zoom state.
 
         Parameters
         ----------
         pan_pos : float
-
             The desired pan position expressed as a value in accepted
             range (often -1.0 to 1.0) that maps to the actual range of
             the camera (e.g. 0-350 degrees or 0-360 degrees).
 
         tilt_pos : float
-
             The desired tilt position expressed as a value in accepted
             range (often -1.0 to 1.0) that maps to the actual range of
             the camera (e.g. 0-90 degrees or -5 to 90 degrees)
 
         zoom_pos : float
-
             The desired zoom "position" expressed as a value in
             accepted range (often 0.0 to 1.0) that maps to the actual
             zoom range of the camera.
 
         Returns
         -------
         None
@@ -516,7 +575,54 @@
         move_request = self._prep_abs_move()
         move_request.Position.Zoom.x = zoom_command
         self.ptz_service.AbsoluteMove(move_request)
 
     def stop(self):
         move_request = self._prep_abs_move()
         self.ptz_service.Stop({'ProfileToken': move_request.ProfileToken})
+
+
+class CalmNoZoomMotorController(MotorController):
+
+    def __init__(self,
+                 pid_gains,
+                 orientation,
+                 example_frame,
+                 zoom_pickup=.01):
+
+        super().__init__(pid_gains,
+                         orientation,
+                         example_frame)
+
+        # this class has not been updated to way things work now
+        raise NotImplementedError
+
+        self.zoom_pickup = zoom_pickup
+        self.ZOOM_STOP_RATIO = .7
+        self.STOP_RANGE = .1
+
+    def _calc_command(self, err, k):
+        """Override controller command method
+
+        The meat here is that the controller stops moving axis under
+        control if error is inside of some range.  This range is
+        currently hardcoded but maybe should be given as an argument
+        to the constructor.
+
+        """
+
+        if np.abs(err) < self.STOP_RANGE:
+            command = 0
+        else:
+            command = k * err
+
+        command = self._ensure_command_in_bounds(command)
+
+        return command
+
+    def _calc_zoom_command(self, x_err, y_err, zoom_command):
+        """Calculate the zoom command give pan/tilt errors
+
+        """
+        zoom_command = 0.0
+        
+        return zoom_command
```

### Comparing `ptzipcam-0.0.6/ptzipcam/tracker.py` & `ptzipcam-0.1.0/ptzipcam/tracker.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/ui.py` & `ptzipcam-0.1.0/ptzipcam/ui.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam/video_writer.py` & `ptzipcam-0.1.0/ptzipcam/video_writer.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.6/ptzipcam.egg-info/PKG-INFO` & `ptzipcam-0.1.0/ptzipcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptzipcam
-Version: 0.0.6
+Version: 0.1.0
 Summary: Package for controlling PTZ IP cameras that support ONVIF
 Author: Ian Ingram
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ptzipcam-0.0.6/setup.py` & `ptzipcam-0.1.0/setup.py`

 * *Files identical despite different names*

