# Comparing `tmp/horusdemodlib-0.3.7.tar.gz` & `tmp/horusdemodlib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horusdemodlib-0.3.7.tar", max compression
+gzip compressed data, was "horusdemodlib-0.3.9.tar", max compression
```

## Comparing `horusdemodlib-0.3.7.tar` & `horusdemodlib-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    26526 2021-12-01 08:57:31.001051 horusdemodlib-0.3.7/LICENSE
--rwxr-xr-x   0        0        0       22 2022-06-26 00:37:35.684849 horusdemodlib-0.3.7/horusdemodlib/__init__.py
--rw-r--r--   0        0        0     3059 2022-02-20 01:08:48.413213 horusdemodlib-0.3.7/horusdemodlib/checksums.py
--rw-r--r--   0        0        0    15371 2022-04-10 02:03:39.746822 horusdemodlib-0.3.7/horusdemodlib/decoder.py
--rw-r--r--   0        0        0     9634 2022-02-05 03:34:32.587491 horusdemodlib-0.3.7/horusdemodlib/delegates.py
--rw-r--r--   0        0        0    13226 2021-12-01 08:57:31.002106 horusdemodlib-0.3.7/horusdemodlib/demod.py
--rw-r--r--   0        0        0     7290 2022-02-05 03:46:24.818314 horusdemodlib-0.3.7/horusdemodlib/demodstats.py
--rw-r--r--   0        0        0    12398 2022-06-26 00:33:29.206712 horusdemodlib-0.3.7/horusdemodlib/habitat.py
--rw-r--r--   0        0        0     4764 2021-12-01 08:57:31.002338 horusdemodlib-0.3.7/horusdemodlib/horusudp.py
--rw-r--r--   0        0        0    11558 2022-02-20 01:06:28.197840 horusdemodlib-0.3.7/horusdemodlib/payloads.py
--rw-r--r--   0        0        0    16017 2022-06-26 00:32:22.585989 horusdemodlib-0.3.7/horusdemodlib/sondehubamateur.py
--rw-r--r--   0        0        0    10714 2022-06-26 01:02:24.918186 horusdemodlib-0.3.7/horusdemodlib/uploader.py
--rw-r--r--   0        0        0      403 2022-06-26 00:37:41.631211 horusdemodlib-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      692 2022-06-26 01:03:18.515983 horusdemodlib-0.3.7/setup.py
--rw-r--r--   0        0        0      673 2022-06-26 01:03:18.516120 horusdemodlib-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    26526 2021-12-01 08:57:31.001051 horusdemodlib-0.3.9/LICENSE
+-rwxr-xr-x   0        0        0       22 2022-09-16 08:48:29.638888 horusdemodlib-0.3.9/horusdemodlib/__init__.py
+-rw-r--r--   0        0        0     3059 2022-02-20 01:08:48.413213 horusdemodlib-0.3.9/horusdemodlib/checksums.py
+-rw-r--r--   0        0        0    15371 2022-09-16 10:09:47.558137 horusdemodlib-0.3.9/horusdemodlib/decoder.py
+-rw-r--r--   0        0        0     9634 2022-02-05 03:34:32.587491 horusdemodlib-0.3.9/horusdemodlib/delegates.py
+-rw-r--r--   0        0        0    13226 2021-12-01 08:57:31.002106 horusdemodlib-0.3.9/horusdemodlib/demod.py
+-rw-r--r--   0        0        0     7290 2022-02-05 03:46:24.818314 horusdemodlib-0.3.9/horusdemodlib/demodstats.py
+-rw-r--r--   0        0        0    12398 2022-09-16 10:08:33.594118 horusdemodlib-0.3.9/horusdemodlib/habitat.py
+-rw-r--r--   0        0        0     5075 2022-09-16 06:16:49.833796 horusdemodlib-0.3.9/horusdemodlib/horusudp.py
+-rw-r--r--   0        0        0    11558 2022-02-20 01:06:28.197840 horusdemodlib-0.3.9/horusdemodlib/payloads.py
+-rw-r--r--   0        0        0    16233 2022-09-16 10:08:41.222759 horusdemodlib-0.3.9/horusdemodlib/sondehubamateur.py
+-rw-r--r--   0        0        0    11216 2022-09-17 09:50:19.333960 horusdemodlib-0.3.9/horusdemodlib/uploader.py
+-rw-r--r--   0        0        0      403 2022-09-17 09:50:37.769811 horusdemodlib-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      692 2022-09-17 09:51:53.340681 horusdemodlib-0.3.9/setup.py
+-rw-r--r--   0        0        0      673 2022-09-17 09:51:53.340838 horusdemodlib-0.3.9/PKG-INFO
```

### Comparing `horusdemodlib-0.3.7/LICENSE` & `horusdemodlib-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/checksums.py` & `horusdemodlib-0.3.9/horusdemodlib/checksums.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/decoder.py` & `horusdemodlib-0.3.9/horusdemodlib/decoder.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/delegates.py` & `horusdemodlib-0.3.9/horusdemodlib/delegates.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/demod.py` & `horusdemodlib-0.3.9/horusdemodlib/demod.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/demodstats.py` & `horusdemodlib-0.3.9/horusdemodlib/demodstats.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/habitat.py` & `horusdemodlib-0.3.9/horusdemodlib/habitat.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/horusudp.py` & `horusdemodlib-0.3.9/horusdemodlib/horusudp.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,19 @@
         
         if 'battery_voltage' in telemetry:
             packet['batt_voltage'] = telemetry['battery_voltage']
 
         if 'speed' in telemetry:
             packet['speed'] = telemetry['speed']
 
+        # Add in any field names from the custom field section
+        if "custom_field_names" in telemetry:
+            for _custom_field_name in telemetry["custom_field_names"]:
+                if _custom_field_name in telemetry:
+                    packet[_custom_field_name] = telemetry[_custom_field_name]
 
         # Set up our UDP socket
         _s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         _s.settimeout(1)
         # Set up socket for broadcast, and allow re-use of the address
         _s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
         _s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
```

### Comparing `horusdemodlib-0.3.7/horusdemodlib/payloads.py` & `horusdemodlib-0.3.9/horusdemodlib/payloads.py`

 * *Files identical despite different names*

### Comparing `horusdemodlib-0.3.7/horusdemodlib/sondehubamateur.py` & `horusdemodlib-0.3.9/horusdemodlib/sondehubamateur.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,20 @@
 
         if "raw" in telemetry:
             _output["raw"] = telemetry["raw"]
 
         if "modulation" in telemetry:
             _output["modulation"] = telemetry["modulation"]
 
+        if "modulation_detail" in telemetry:
+            _output["modulation_detail"] = telemetry["modulation_detail"]
+
+        if "baud_rate" in telemetry:
+            _output["baud_rate"] = telemetry["baud_rate"]
+
         # Add in any field names from the custom field section
         if "custom_field_names" in telemetry:
             for _custom_field_name in telemetry["custom_field_names"]:
                 if _custom_field_name in telemetry:
                     _output[_custom_field_name] = telemetry[_custom_field_name]
```

### Comparing `horusdemodlib-0.3.7/horusdemodlib/uploader.py` & `horusdemodlib-0.3.9/horusdemodlib/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     parser.add_argument("--payload-list", type=str, default="payload_id_list.txt", help="List of known payload IDs.")
     parser.add_argument("--custom-fields", type=str, default="custom_field_list.json", help="List of payload Custom Fields")
     parser.add_argument("--nodownload", action="store_true", default=False, help="Do not download new lists.")
 #   parser.add_argument("--ozimux", type=int, default=-1, help="Override user.cfg OziMux output UDP port. (NOT IMPLEMENTED)")
 #   parser.add_argument("--summary", type=int, default=-1, help="Override user.cfg UDP Summary output port. (NOT IMPLEMENTED)")
     parser.add_argument("--freq_hz", type=float, default=None, help="Receiver IQ centre frequency in Hz, used in determine the absolute frequency of a telemetry burst.")
     parser.add_argument("--freq_target_hz", type=float, default=None, help="Receiver 'target' frequency in Hz, used to add metadata to station position info.")
+    parser.add_argument("--baud_rate", type=int, default=None, help="Modulation baud rate (Hz), used to add additional metadata info.")
     parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Verbose output (set logging level to DEBUG)")
     args = parser.parse_args()
 
     if args.verbose:
         logging_level = logging.DEBUG
     else:
         logging_level = logging.INFO
@@ -180,14 +181,18 @@
                     _decoded['snr'] = _snr
 
                     # Add in frequency estimate, if we have been supplied a receiver frequency.
                     if args.freq_hz:
                         _decoded['f_centre'] = int(demod_stats.fest_mean) + int(args.freq_hz)
                         habitat_uploader.last_freq_hz = _decoded['f_centre']
 
+                    # Add in baud rate, if provided.
+                    if args.baud_rate:
+                        _decoded['baud_rate'] = int(args.baud_rate)
+
                     # Send via UDP
                     send_payload_summary(_decoded, port=user_config['summary_port'])
 
                     # Upload the string to Habitat
                     _decoded_str = "$$" + data.split('$')[-1] + '\n'
                     habitat_uploader.add(_decoded_str)
 
@@ -225,19 +230,23 @@
                     _decoded['snr'] = _snr
 
                     # Add in frequency estimate, if we have been supplied a receiver frequency.
                     if args.freq_hz:
                         _decoded['f_centre'] = int(demod_stats.fest_mean) + int(args.freq_hz)
                         habitat_uploader.last_freq_hz = _decoded['f_centre']
 
+                    # Add in baud rate, if provided.
+                    if args.baud_rate:
+                        _decoded['baud_rate'] = int(args.baud_rate)
+
                     # Send via UDP
                     send_payload_summary(_decoded, port=user_config['summary_port'])
 
-                    # Upload to Habitat
-                    habitat_uploader.add(_decoded['ukhas_str']+'\n')
+                    # Do not upload Horus Binary packets to the Habitat endpoint.
+                    # habitat_uploader.add(_decoded['ukhas_str']+'\n')
 
                     # Upload the string to Sondehub Amateur
                     sondehub_uploader.add(_decoded)
 
                     if _logfile:
                         _logfile.write(_decoded['ukhas_str']+'\n')
                         _logfile.flush()
```

### Comparing `horusdemodlib-0.3.7/setup.py` & `horusdemodlib-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['crcmod>=1.7,<2.0',
  'numpy>=1.17,<2.0',
  'python-dateutil>=2.8,<3.0',
  'requests>=2.24.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'horusdemodlib',
-    'version': '0.3.7',
+    'version': '0.3.9',
     'description': 'Project Horus HAB Telemetry Demodulators',
     'long_description': None,
     'author': 'Mark Jessop',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `horusdemodlib-0.3.7/PKG-INFO` & `horusdemodlib-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horusdemodlib
-Version: 0.3.7
+Version: 0.3.9
 Summary: Project Horus HAB Telemetry Demodulators
 License: LGPL-2.1-or-later
 Author: Mark Jessop
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

