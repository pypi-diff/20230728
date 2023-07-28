# Comparing `tmp/radiacode-0.2.0.tar.gz` & `tmp/radiacode-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiacode-0.2.0.tar", max compression
+gzip compressed data, was "radiacode-0.2.1.tar", max compression
```

## Comparing `radiacode-0.2.0.tar` & `radiacode-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-06-18 13:36:03.683282 radiacode-0.2.0/LICENSE
--rw-r--r--   0        0        0     1520 2023-06-18 13:36:03.683282 radiacode-0.2.0/README.md
--rw-r--r--   0        0        0      981 2023-06-18 13:36:03.683282 radiacode-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      147 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/__init__.py
--rw-r--r--   0        0        0      694 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/bytes_buffer.py
--rw-r--r--   0        0        0        0 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/databuf.py
--rw-r--r--   0        0        0     1573 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/spectrum.py
--rw-r--r--   0        0        0     7253 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/radiacode.py
--rw-r--r--   0        0        0        0 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/bluetooth.py
--rw-r--r--   0        0        0      954 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/usb.py
--rw-r--r--   0        0        0     2310 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/types.py
--rw-r--r--   0        0        0     1296 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/README.md
--rw-r--r--   0        0        0     1215 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/README_ru.md
--rw-r--r--   0        0        0      933 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/basic.py
--rw-r--r--   0        0        0     2711 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/narodmon.py
--rw-r--r--   0        0        0     1820 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/radiacode-exporter.py
--rw-r--r--   0        0        0     4276 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/webserver.html
--rw-r--r--   0        0        0     3509 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/webserver.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 radiacode-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-28 12:30:47.754924 radiacode-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1520 2023-07-28 12:30:47.754924 radiacode-0.2.1/README.md
+-rw-r--r--   0        0        0      981 2023-07-28 12:30:47.754924 radiacode-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/bytes_buffer.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/decoders/__init__.py
+-rw-r--r--   0        0        0     3714 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/decoders/databuf.py
+-rw-r--r--   0        0        0     1573 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/decoders/spectrum.py
+-rw-r--r--   0        0        0     7560 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/radiacode.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/transports/__init__.py
+-rw-r--r--   0        0        0     1720 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/transports/bluetooth.py
+-rw-r--r--   0        0        0      954 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/transports/usb.py
+-rw-r--r--   0        0        0     2443 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode/types.py
+-rw-r--r--   0        0        0     1296 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/README.md
+-rw-r--r--   0        0        0     1215 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/README_ru.md
+-rw-r--r--   0        0        0      933 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/basic.py
+-rw-r--r--   0        0        0     2711 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/narodmon.py
+-rw-r--r--   0        0        0     1820 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/radiacode-exporter.py
+-rw-r--r--   0        0        0     4456 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/webserver.html
+-rw-r--r--   0        0        0     3729 2023-07-28 12:30:47.754924 radiacode-0.2.1/radiacode-examples/webserver.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 radiacode-0.2.1/PKG-INFO
```

### Comparing `radiacode-0.2.0/LICENSE` & `radiacode-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/README.md` & `radiacode-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/pyproject.toml` & `radiacode-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radiacode"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library for RadiaCode-101"
 authors = ["Maxim Andreev <andreevmaxim@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cdump/radiacode"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `radiacode-0.2.0/radiacode/bytes_buffer.py` & `radiacode-0.2.1/radiacode/bytes_buffer.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode/decoders/databuf.py` & `radiacode-0.2.1/radiacode/decoders/databuf.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode/decoders/spectrum.py` & `radiacode-0.2.1/radiacode/decoders/spectrum.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode/radiacode.py` & `radiacode-0.2.1/radiacode/radiacode.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def read_request(self, command_id: Union[int, VS, VSFR]) -> BytesBuffer:
         r = self.execute(b'\x26\x08', struct.pack('<I', int(command_id)))
         retcode, flen = r.unpack('<II')
         assert retcode == 1
         assert r.size() == flen
         return r
 
-    def write_request(self, command_id: Union[int, VSFR], data: bytes) -> None:
+    def write_request(self, command_id: Union[int, VSFR], data: Optional[bytes] = None) -> None:
         r = self.execute(b'\x25\x08', struct.pack('<I', int(command_id)) + (data or b''))
         retcode = r.unpack('<I')[0]
         assert retcode == 1
         assert r.size() == 0
 
     def batch_read_vsfrs(self, vsfr_ids: List[VSFR]) -> List[int]:
         assert len(vsfr_ids)
@@ -136,14 +136,23 @@
         r = self.read_request(VS.SPECTRUM)
         return decode_RC_VS_SPECTRUM(r, self._spectrum_format_version)
 
     def spectrum_accum(self) -> Spectrum:
         r = self.read_request(VS.SPEC_ACCUM)
         return decode_RC_VS_SPECTRUM(r, self._spectrum_format_version)
 
+    def dose_reset(self) -> None:
+        self.write_request(VSFR.DOSE_RESET)
+
+    def spectrum_reset(self) -> None:
+        r = self.execute(b'\x27\x08', struct.pack('<II', int(VS.SPECTRUM), 0))
+        retcode = r.unpack('<I')[0]
+        assert retcode == 1
+        assert r.size() == 0
+
     # used in spectrum_channel_to_energy
     def energy_calib(self) -> List[float]:
         r = self.read_request(VS.ENERGY_CALIB)
         return list(r.unpack('<fff'))
 
     def set_language(self, lang='ru') -> None:
         assert lang in {'ru', 'en'}, 'unsupported lang value - use "ru" or "en"'
```

### Comparing `radiacode-0.2.0/radiacode/transports/bluetooth.py` & `radiacode-0.2.1/radiacode/transports/bluetooth.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode/transports/usb.py` & `radiacode-0.2.1/radiacode/transports/usb.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode/types.py` & `radiacode-0.2.1/radiacode/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,26 +91,28 @@
     LED3_BRT = 1348
     LEDS_ON = 1349
     ALARM_MODE = 1504
     MS_CTRL = 1536
     MS_MODE = 1537
     MS_SUB_MODE = 1538
     MS_RUN = 1539
+    DOSE_RESET = 32775
 
     def __int__(self) -> int:
         return self.value
 
 class VS(Enum):
     CONFIGURATION = 2
     TEXT_MESSAGE = 15
     DATA_BUF = 256
     SPECTRUM = 512
     ENERGY_CALIB = 514
     SPEC_ACCUM = 517
     SPEC_DIFF = 518  # TODO: what's that? Can be decoded by spectrum decoder
+    SPEC_RESET = 519 # TODO: looks like spectrum, but our spectrum decoder fails with `vlen == 7 unsupported`
     # UNKNOWN_13 = 13
     # UNKNOWN_240 = 240
 
     def __int__(self) -> int:
         return self.value
```

### Comparing `radiacode-0.2.0/radiacode-examples/README.md` & `radiacode-0.2.1/radiacode-examples/README.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode-examples/README_ru.md` & `radiacode-0.2.1/radiacode-examples/README_ru.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode-examples/basic.py` & `radiacode-0.2.1/radiacode-examples/basic.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode-examples/narodmon.py` & `radiacode-0.2.1/radiacode-examples/narodmon.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode-examples/radiacode-exporter.py` & `radiacode-0.2.1/radiacode-examples/radiacode-exporter.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.2.0/radiacode-examples/webserver.html` & `radiacode-0.2.1/radiacode-examples/webserver.html`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         <input type="radio" id="spectrum_linear" v-bind:value="false" v-model="spectrum_logarithmic">
         <label for="spectrum_linear">Linear</label>
         <input type="radio" id="spectrum_log" v-bind:value="true" v-model="spectrum_logarithmic">
         <label for="spectrum_log">Logarithmic</label>
       </fieldset>
     </div>
     <button @click="updateSpectrum">Update spectrum</button>
+    <button @click="resetSpectrum">Reset spectrum</button>
   </div>
   <div>
     <apexchart type="line" height="350" :options="ratesChartOptions" :series="rates_series"></apexchart>
     <button @click="rates_autoupdate = !rates_autoupdate">Rates autoupdate: {{ rates_autoupdate ? "ON" : "OFF" }}</button>
   </div>
 </div>
 
@@ -126,12 +127,16 @@
       this.rates_series = d.series;
     },
     updateSpectrum() {
       fetch(`/spectrum?accum=${this.spectrum_accum}`)
         .then(response => response.json())
         .then(data => (this.spectrum_duration=data.duration, this.spectrum_coef=data.coef, this.spectrum_series=data.series));
     },
+    resetSpectrum() {
+      fetch(`/spectrum/reset`, {method: 'POST'})
+        .then(r => this.updateSpectrum());
+    },
   },
 });
 </script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 options="spectrumChartOptions" :series="spectrum_series">
  ⁰ Accumulated   o Channel o Energy   o Linear o Logarithmic
 click="updateSpectrum">Update spectrum
+click="resetSpectrum">Reset spectrum
 options="ratesChartOptions" :series="rates_series">
 click="rates_autoupdate = !rates_autoupdate">Rates autoupdate: {
 { rates_autoupdate ? "ON" : "OFF" }}
```

### Comparing `radiacode-0.2.0/radiacode-examples/webserver.py` & `radiacode-0.2.1/radiacode-examples/webserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,19 @@
         {
             'coef': [spectrum.a0, spectrum.a1, spectrum.a2],
             'duration': spectrum.duration.total_seconds(),
             'series': [{'name': 'spectrum', 'data': spectrum_data}],
         },
     )
 
+async def handle_spectrum_reset(request):
+    cn = request.app.rc_conn
+    cn.spectrum_reset()
+    print('Spectrum reset')
+    return web.json_response({})
 
 async def process(app):
     max_history_size = 128
     countrate_history, doserate_history = [], []
     while True:  # noqa: WPS457
         databuf = app.rc_conn.data_buf()
         for v in databuf:
@@ -95,11 +100,12 @@
         app.rc_conn = RadiaCode()
 
     app.on_startup.append(on_startup)
     app.add_routes(
         [
             web.get('/', handle_index),
             web.get('/spectrum', handle_spectrum),
+            web.post('/spectrum/reset', handle_spectrum_reset),
             web.get('/ws', handle_ws),
         ],
     )
     web.run_app(app, host=args.listen_host, port=args.listen_port)
```

### Comparing `radiacode-0.2.0/PKG-INFO` & `radiacode-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiacode
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for RadiaCode-101
 Home-page: https://github.com/cdump/radiacode
 License: MIT
 Author: Maxim Andreev
 Author-email: andreevmaxim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

