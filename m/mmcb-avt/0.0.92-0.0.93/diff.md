# Comparing `tmp/mmcb-avt-0.0.92.tar.gz` & `tmp/mmcb-avt-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.92.tar", last modified: Sat May 27 08:08:05 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.93.tar", last modified: Fri Jul 28 13:45:42 2023, max compression
```

## Comparing `mmcb-avt-0.0.92.tar` & `mmcb-avt-0.0.93.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.315344 mmcb-avt-0.0.92/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.92/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 08:08:05.314521 mmcb-avt-0.0.92/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.92/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.92/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-27 08:08:05.315523 mmcb-avt-0.0.92/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2593 2023-05-27 08:07:41.000000 mmcb-avt-0.0.92/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.284690 mmcb-avt-0.0.92/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.307148 mmcb-avt-0.0.92/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.92/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-27 07:42:26.000000 mmcb-avt-0.0.92/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-05-27 07:52:17.000000 mmcb-avt-0.0.92/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.92/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.92/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-17 14:29:51.000000 mmcb-avt-0.0.92/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.92/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.92/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.92/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.92/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.92/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.92/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.92/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.92/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.92/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 07:52:28.000000 mmcb-avt-0.0.92/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.92/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.92/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.92/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.92/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.312584 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      694 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      228 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.313412 mmcb-avt-0.0.92/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.92/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.291082 mmcb-avt-0.0.93/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.93/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-28 13:45:42.290212 mmcb-avt-0.0.93/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.93/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.93/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-28 13:45:42.291291 mmcb-avt-0.0.93/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-28 13:44:24.000000 mmcb-avt-0.0.93/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.244313 mmcb-avt-0.0.93/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.278929 mmcb-avt-0.0.93/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.93/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.93/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32436 2023-05-27 08:13:04.000000 mmcb-avt-0.0.93/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.93/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.93/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.93/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.93/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.93/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.93/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.93/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.93/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.93/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.93/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.93/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.93/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.93/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.93/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.93/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.93/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.93/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.288231 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      694 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.288992 mmcb-avt-0.0.93/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.93/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.92/LICENSE` & `mmcb-avt-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/PKG-INFO` & `mmcb-avt-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.92
+Version: 0.0.93
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.92/README.md` & `mmcb-avt-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/setup.py` & `mmcb-avt-0.0.93/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.92",
+    version="0.0.93",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.92/src/mmcb/common.py` & `mmcb-avt-0.0.93/src/mmcb/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 DEVICE_CACHE = os.path.expanduser('~/.cache.json')
 
 
 UNIT = types.SimpleNamespace(
     calculated_dew_point='DP\u00b0C',
-    flow_rate='l/s',
+    flow_rate='lps',
     pressure='hPa',
     relative_humidity='RH%',
     strain='arbitrary',
     temperature='\u00b0C',
     vacuum='kPa',
 )
```

### Comparing `mmcb-avt-0.0.92/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.93/src/mmcb/configure_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,41 +81,42 @@
         """
         Read in a configuration CSV file that describes the test setup.
 
         Each line of the CSV files defines a single sensor.
 
         The CSV fields are:
 
-        (1) sensor_type - Mandatory field. See mapping variable below for details.
-        (2) sensor_name - Mandatory field.
-        (3) qmux_i2c
+        (1) sensor_type - Mandatory field. See mapping variable below for
+        details.(2) sensor_name - Mandatory field.(3) qmux_i2c
 
-        The I2C address of the Qwiic multiplexer the sensor is attached to. Leave
-        this field empty if the sensor is connected directly to the I2C bus.
+        The I2C address of the Qwiic multiplexer the sensor is attached to.
+        Leave this field empty if the sensor is connected directly to the I2C
+        bus.
 
         (4) qmux_chan
 
-        The Qwiic multiplexer channel the sensor is attached to. Leave this field
-        empty if the sensor is connected directly to the I2C bus.
+        The Qwiic multiplexer channel the sensor is attached to. Leave this
+        field empty if the sensor is connected directly to the I2C bus.
 
         (5) i2c_addr
 
         The I2C address of the sensor.
 
-        This field supports two configurations: (a) Each multiplexer channel may
-        host a chain of sensors with I2C addresses unique to the multiplexer
-        channel, or (b) a sensor directly connected to the I2C bus.
+        This field supports two configurations: (a) Each multiplexer channel
+        may host a chain of sensors with I2C addresses unique to the
+        multiplexer channel, or (b) a sensor directly connected to the I2C
+        bus.
 
-        If omitted, this value will be assumed to be the default I2C address of
-        the sensor_type.
+        If omitted, this value will be assumed to be the default I2C address
+        of the sensor_type.
 
         (6) thermocouple_type
 
-        Only applicable to thermocouples. Leave this field empty for other sensor
-        types.
+        Only applicable to thermocouples. Leave this field empty for other
+        sensor types.
 
         (7) analogue_input
 
         Only applicable to sensor types read via an ADS1015 12-bit ADC and
         analogue multiplexer.
 
         Example configuration file:
@@ -127,25 +128,25 @@
         ntc,    ntc,            0x71, 5,,,2
         tc,     TCk1_env,       0x71, 6, 0x67, K
         tc,     TCk2_M1_vc,     0x71, 6, 0x66, K
         tc,     TCt1_M4_vc,     0x71, 6, 0x65, T
         tc,     TCk3_M2_vc,     0x71, 7, 0x66, K
         tc,     TCk3_M3_vc,     0x71, 7, 0x65, K
 
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         args
             configuration_file : string
                 file that exists
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         returns
             sensors : list of class instances
             e.g.
                 [Hyt221(), Hyt221(), Hyt221(), SmcZse30A01F(), AtlasNtc(),
                  Mcp9601(), Mcp9601(), Mcp9601(), Mcp9601(), Mcp9601()]
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         """
         # sensor_type to class mapping
         mapping = {
             'bme680': sensors.Bme680,
             'hyt221': sensors.Hyt221,
             'nau7802': sensors.Nau7802,
             'ntc': sensors.AtlasNtc,
@@ -702,35 +703,35 @@
         (0, 1, 2, 2, 2, 3, 3)
 
         Changes would be indicated thus:
 
         ((True, ...), (True, ...), (True, ...), (False, ...), (False, ...),
         (True, ...), (False, ...))
 
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         args
             number_sequence : generator
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         yields : tuple (bool, int)
-            (True, ...) if the current number in the sequence differed from its
-            predecessor, (False, ...) otherwise.
-        --------------------------------------------------------------------------
+            (True, ...) if the current number in the sequence differed from
+            its predecessor, (False, ...) otherwise.
+        ----------------------------------------------------------------------
         """
         last = None
 
         for number in number_sequence:
             if number != last:
                 yield True, last
                 last = number
             else:
                 yield False, last
 
-    ##############################################################################
+    ##########################################################################
     # dew point
-    ##############################################################################
+    ##########################################################################
 
     def calculate_dew_points(self, data_for_current_timestamp):
         """
         Calculate dew point data from a dictionary of sensor values.
 
         Dew points are only calculated for sensors that supply both relative
         humidity and temperature; there's no mixing of data from different
@@ -739,33 +740,33 @@
         Note that the internal _dew_point method which this method relies
         upon, returns values low values clamped to -71 degrees Celsius, which
         is the figure for the dry air supply in the cleanroom. This is to
         cope with some sensors reporting zero RH% in dry conditions due to
         limited resolution, which would in turn lead to dew point figures
         that would be impossible to realise in the test environment.
 
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         args
             data_for_current_timestamp : dict
                 e.g.
                 {'timestamp': 1651224444.4431129,
                  'hyt221_ch0_M1_temperature': 20.277421717634134,
                  'hyt221_ch0_M1_relative_humidity': 0.0,
                  'hyt221_ch1_env_temperature': 20.60977842885918,
                  'hyt221_ch1_env_relative_humidity': 0.0, ...}
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         returns
             dew_point_calculations: dict
                 e.g.
                 {'bme_ambient_calculated_dew_point': 7.317889854346651,
                  'hyt221_ch2_calculated_dew_point': -71,
                  'hyt221_ch1_env_calculated_dew_point': -71,
                  'hyt221_ch0_M1_calculated_dew_point': -71,
                  'sht_ambient_calculated_dew_point': 8.439206561314366}
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         """
         dew_point_calculations = {}
 
         rhu = '_relative_humidity'
         tdc = '_temperature'
         # find all keys containing relative humidity or temperature
         columns_of_interest = {
@@ -814,26 +815,26 @@
         w = 0.7858 (vapor pressure in mbar)
 
         In [25]: math.pow(10, (t * u)/(t + v) + w)
         Out[25]: 23.521463268069194
 
         For low temperature and low pressure with accuracy, use Goff-Gratch.
 
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         args
             tdc : float
                 temperature degrees Celsius
             rhp : float
                 relative humidity percentage
             arden_buck : bool
                 choice of algorithm
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         returns : float
             dew point degrees Celsius
-        --------------------------------------------------------------------------
+        ----------------------------------------------------------------------
         """
         # constants
         # a = 6.1121 # mbar
         b = 18.678
         c = 257.14  # °C
         d = 234.5  # °C
```

### Comparing `mmcb-avt-0.0.92/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.93/src/mmcb/dat2plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,22 @@
     returns : no explicit return
             plot written to local filestore
     --------------------------------------------------------------------------
     """
     lwi = 0.5
     lal = 1
 
-    y_axis_label_prefix = {'°C': 'temperature (°C)',
-                           'RH%': 'relative humidity (RH%)',
-                           'DP°C': 'calculated dew point (°C)',
-                           'kPa': 'vacuum (kPa)',
-                           'l/s': 'flow rate (l/s)',
-                           'hPa': 'pressure (hPa)'}
+    y_axis_label_prefix = {
+        '°C': 'temperature (°C)',
+       'RH%': 'relative humidity (RH%)',
+       'DP°C': 'calculated dew point (°C)',
+       'kPa': 'vacuum (kPa)',
+       'lps': 'flow rate (l/s)',
+       'hPa': 'pressure (hPa)',
+    }
 
     num_plots = len(unique_units)
     # for 3 subplots a 12 x 8 size works well, use this as a basis for other
     # numbers of plots
     y_size = (8 / 3) * num_plots
 
     fig, axes = plt.subplots(nrows=num_plots, ncols=1, sharex=True, figsize=(12, y_size))
@@ -165,19 +167,22 @@
             A separate subplot is created for each unit in this set.
             e.g. {'DP°C', 'hPa', 'RH%', 'kPa', '°C'}
     --------------------------------------------------------------------------
     returns : no explicit return
             plot written to local filestore
     --------------------------------------------------------------------------
     """
-    y_axis_label_prefix = {'°C': 'temperature (°C)',
-                           'RH%': 'relative humidity (RH%)',
-                           'DP°C': 'calculated dew point (°C)',
-                           'kPa': 'vacuum (kPa)',
-                           'hPa': 'pressure (hPa)'}
+    y_axis_label_prefix = {
+        '°C': 'temperature (°C)',
+       'RH%': 'relative humidity (RH%)',
+       'DP°C': 'calculated dew point (°C)',
+       'kPa': 'vacuum (kPa)',
+       'lps': 'flow rate (l/s)',
+       'hPa': 'pressure (hPa)',
+    }
 
     num_plots = len(unique_units)
 
     # for 3 subplots a 12 x 12 size works well, use this as a basis for other
     # numbers of plots
     y_size = 4.5 * num_plots
```

### Comparing `mmcb-avt-0.0.92/src/mmcb/dat2root.py` & `mmcb-avt-0.0.93/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/detect.py` & `mmcb-avt-0.0.93/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/dmm.py` & `mmcb-avt-0.0.93/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.93/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/iv.py` & `mmcb-avt-0.0.93/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/lexicon.py` & `mmcb-avt-0.0.93/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/liveplot.py` & `mmcb-avt-0.0.93/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/log2dat.py` & `mmcb-avt-0.0.93/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/peltier.py` & `mmcb-avt-0.0.93/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/psuset.py` & `mmcb-avt-0.0.93/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/psustat.py` & `mmcb-avt-0.0.93/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/sense.py` & `mmcb-avt-0.0.93/src/mmcb/sense.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,9 +360,9 @@
                     data_columns=True
                 )
 
                 time.sleep(5)
 
 
 ##############################################################################
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
```

### Comparing `mmcb-avt-0.0.92/src/mmcb/sensors.py` & `mmcb-avt-0.0.93/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.93/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/sequence.py` & `mmcb-avt-0.0.93/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb/ult80.py` & `mmcb-avt-0.0.93/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.92/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.93/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.92
+Version: 0.0.93
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.92/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.93/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

