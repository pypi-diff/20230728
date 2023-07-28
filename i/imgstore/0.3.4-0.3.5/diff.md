# Comparing `tmp/imgstore-0.3.4.tar.gz` & `tmp/imgstore-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgstore-0.3.4.tar", last modified: Mon Jun 19 08:59:56 2023, max compression
+gzip compressed data, was "imgstore-0.3.5.tar", last modified: Fri Jul 28 10:07:04 2023, max compression
```

## Comparing `imgstore-0.3.4.tar` & `imgstore-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-19 08:59:51.000000 imgstore-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 08:59:51.000000 imgstore-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-19 08:59:56.219705 imgstore-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-19 08:59:51.000000 imgstore-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    48533 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   861959 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/graffiti.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore/tests/data/store_mp4/
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.npz
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/data/store_mp4/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/test_imgstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-19 08:59:51.000000 imgstore-0.3.4/imgstore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:59:56.219705 imgstore-0.3.4/imgstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 08:59:56.000000 imgstore-0.3.4/imgstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 08:59:56.219705 imgstore-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-19 08:59:51.000000 imgstore-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-28 10:06:58.000000 imgstore-0.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 10:06:58.000000 imgstore-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-28 10:07:04.209751 imgstore-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-28 10:06:58.000000 imgstore-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/imgstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48778 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/imgstore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/imgstore/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   861959 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/graffiti.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/imgstore/tests/data/store_mp4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/store_mp4/000000.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/store_mp4/000000.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/store_mp4/000001.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/store_mp4/000001.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/data/store_mp4/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/test_imgstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-28 10:06:58.000000 imgstore-0.3.5/imgstore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:07:04.209751 imgstore-0.3.5/imgstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 10:07:04.000000 imgstore-0.3.5/imgstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 10:07:04.209751 imgstore-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-28 10:06:58.000000 imgstore-0.3.5/setup.py
```

### Comparing `imgstore-0.3.4/LICENSE.txt` & `imgstore-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/PKG-INFO` & `imgstore-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgstore
-Version: 0.3.4
+Version: 0.3.5
 Summary: IMGStore houses your video frames
 Home-page: https://github.com/loopbio/imgstore
 Author: John Stowers, Santi Villalba
 Author-email: john@loopbio.com, santi@loopbio.com
 License: BSD 3 clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -159,18 +159,27 @@
 
 Once you have a python (virtual) environment with a recent and reliable OpenCV build,
 you can install IMGStore from pip
 
 `$ pip install imgstore`
 
 After installing imgstore from any location, you should check it's tests pass to guarantee that
-you have a trustworthy OpenCV version
+you have a trustworthy OpenCV version.
+
+If you must install opencv from pip, such as for only reading imgstores, you can
+use the following command to install the latest 4.8 version
+
+`$ pip install "opencv-python < 4.9"`
 
 ## Post install testing
 
+Test libraries are not installed by default. To do so, install pytest
+
+`$ pip install "pytest < 8"`
+
 You should always run the command `imgstore-test` after installing imgstore. If your
 environment is working correctly you should see a lot of text printed, followed by the
 text `==== 66 passed, ..... ======`
 
 To test against the package without installing first, run `python -m pytest`
 
 Note: by running pytest through it's python module interface, the interpreter adds `pwd` to
```

### Comparing `imgstore-0.3.4/README.md` & `imgstore-0.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -137,18 +137,27 @@
 
 Once you have a python (virtual) environment with a recent and reliable OpenCV build,
 you can install IMGStore from pip
 
 `$ pip install imgstore`
 
 After installing imgstore from any location, you should check it's tests pass to guarantee that
-you have a trustworthy OpenCV version
+you have a trustworthy OpenCV version.
+
+If you must install opencv from pip, such as for only reading imgstores, you can
+use the following command to install the latest 4.8 version
+
+`$ pip install "opencv-python < 4.9"`
 
 ## Post install testing
 
+Test libraries are not installed by default. To do so, install pytest
+
+`$ pip install "pytest < 8"`
+
 You should always run the command `imgstore-test` after installing imgstore. If your
 environment is working correctly you should see a lot of text printed, followed by the
 text `==== 66 passed, ..... ======`
 
 To test against the package without installing first, run `python -m pytest`
 
 Note: by running pytest through it's python module interface, the interpreter adds `pwd` to
```

### Comparing `imgstore-0.3.4/imgstore/align.py` & `imgstore-0.3.5/imgstore/align.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/apps.py` & `imgstore-0.3.5/imgstore/apps.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/index.py` & `imgstore-0.3.5/imgstore/index.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/stores.py` & `imgstore-0.3.5/imgstore/stores.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 from .constants import DEVNULL, STORE_MD_FILENAME, STORE_LOCK_FILENAME, STORE_MD_KEY, \
     STORE_INDEX_FILENAME, EXTRA_DATA_FILE_EXTENSIONS, FRAME_MD as _FRAME_MD
 from .util import ImageCodecProcessor, JsonCustomEncoder, FourCC, ensure_color,\
     ensure_grayscale, motif_extra_data_h5_to_df, motif_extra_data_json_to_df, motif_extra_data_h5_attrs
 from .index import ImgStoreIndex
 
 
+def _get_tzlocal_zone():
+    # tzlocal is probbably the worst API I have ever used at maintaining backwards
+    # compatibility.
+    try:
+        return tzlocal.get_localzone().zone
+    except AttributeError:
+        return tzlocal.get_localzone_name()
+
+
 _VERBOSE_DEBUG_GETS = False
 _VERBOSE_DEBUG_CHUNKS = False
 _VERBOSE_VERY = False  # overrides the other and prints all logs to stdout
 
 
 def _extract_store_metadata(full_path):
     with open(full_path, 'r') as f:
@@ -202,15 +211,15 @@
             if 'timezone' in allmd:
                 # noinspection PyBroadException
                 try:
                     tz = ZoneInfo(allmd['timezone'])
                 except Exception:
                     pass
             if tz is None:
-                tz = ZoneInfo(tzlocal.get_localzone().zone)
+                tz = ZoneInfo(_get_tzlocal_zone())
 
             # first the filename
             m = re.match(r"""(.*)(20[\d]{6}_\d{6}).*""", os.path.basename(self._basedir))
             if m:
                 name, datestr = m.groups()
                 # ive always been careful to make the files named with the local time
                 time_tuple = time.strptime(datestr, '%Y%m%d_%H%M%S')
@@ -265,15 +274,15 @@
         self._imgdtype = imgdtype
         self._chunksize = chunksize
         self._format = fmt
 
         self._uuid = uuid.uuid4().hex
         # because fuck you python that utcnow is naieve. kind of fixed in python >3.2
         self._created_utc = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
-        self._timezone_local = ZoneInfo(tzlocal.get_localzone().zone)
+        self._timezone_local = ZoneInfo(_get_tzlocal_zone())
 
         store_md = {'imgshape': write_imgshape,
                     'imgdtype': self._imgdtype,
                     'chunksize': chunksize,
                     'format': fmt,
                     'class': self.__class__.__name__,
                     'version': self._version,
@@ -844,15 +853,15 @@
         if kwargs['mode'] == 'w':
             if 'chunksize' not in kwargs:
                 kwargs['chunksize'] = self._DEFAULT_CHUNKSIZE
             kwargs['encoding'] = kwargs.pop('encoding', None)
 
         kwargs['write_encode_encoding'] = None
 
-        if kwargs['format'].endswith('+color'):
+        if kwargs.get('format', '').endswith('+color'):
             kwargs['format'] = kwargs['format'].replace('+color', '')
 
             if kwargs['encoding']:
                 kwargs['write_encode_encoding'] = kwargs['encoding']
                 kwargs['encoding'] = None  # and so in the store it is no longer encoded
 
         _ImgStore.__init__(self, **kwargs)
```

### Comparing `imgstore-0.3.4/imgstore/tests/data/graffiti.png` & `imgstore-0.3.5/imgstore/tests/data/graffiti.png`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.mp4` & `imgstore-0.3.5/imgstore/tests/data/store_mp4/000000.mp4`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/data/store_mp4/000000.npz` & `imgstore-0.3.5/imgstore/tests/data/store_mp4/000000.npz`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.mp4` & `imgstore-0.3.5/imgstore/tests/data/store_mp4/000001.mp4`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/data/store_mp4/000001.npz` & `imgstore-0.3.5/imgstore/tests/data/store_mp4/000001.npz`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/test_imgstore.py` & `imgstore-0.3.5/imgstore/tests/test_imgstore.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/tests/test_util.py` & `imgstore-0.3.5/imgstore/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/ui.py` & `imgstore-0.3.5/imgstore/ui.py`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/imgstore/util.py` & `imgstore-0.3.5/imgstore/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,17 @@
                 self._cv2_enum_to_code[enum] = code
 
         self.autoconvert = lambda x: x
 
         # pprint.pprint(self._cv2_code_to_enum)
         # pprint.pprint(self._cv2_enum_to_code)
 
+    def __repr__(self):
+        return "<ImageCodecProcessor(%s)>" % self._default_code
+
     @classmethod
     def from_pylon_format(cls, s):
         # pylon disagrees with opencv (B & R are always switched)
         if s in {'BayerBG', 'Bayer_BG'}:
             code = 'cv_bayerrg'
         elif s in {'BayerRG', 'Bayer_RG'}:
             code = 'cv_bayerbg'
```

### Comparing `imgstore-0.3.4/imgstore.egg-info/PKG-INFO` & `imgstore-0.3.5/imgstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgstore
-Version: 0.3.4
+Version: 0.3.5
 Summary: IMGStore houses your video frames
 Home-page: https://github.com/loopbio/imgstore
 Author: John Stowers, Santi Villalba
 Author-email: john@loopbio.com, santi@loopbio.com
 License: BSD 3 clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -159,18 +159,27 @@
 
 Once you have a python (virtual) environment with a recent and reliable OpenCV build,
 you can install IMGStore from pip
 
 `$ pip install imgstore`
 
 After installing imgstore from any location, you should check it's tests pass to guarantee that
-you have a trustworthy OpenCV version
+you have a trustworthy OpenCV version.
+
+If you must install opencv from pip, such as for only reading imgstores, you can
+use the following command to install the latest 4.8 version
+
+`$ pip install "opencv-python < 4.9"`
 
 ## Post install testing
 
+Test libraries are not installed by default. To do so, install pytest
+
+`$ pip install "pytest < 8"`
+
 You should always run the command `imgstore-test` after installing imgstore. If your
 environment is working correctly you should see a lot of text printed, followed by the
 text `==== 66 passed, ..... ======`
 
 To test against the package without installing first, run `python -m pytest`
 
 Note: by running pytest through it's python module interface, the interpreter adds `pwd` to
```

### Comparing `imgstore-0.3.4/imgstore.egg-info/SOURCES.txt` & `imgstore-0.3.5/imgstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgstore-0.3.4/setup.py` & `imgstore-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name='imgstore',
     license='BSD 3 clause',
     description='IMGStore houses your video frames',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
-    version='0.3.4',
+    version='0.3.5',
     url='https://github.com/loopbio/imgstore',
     author='John Stowers, Santi Villalba',
     author_email='john@loopbio.com, santi@loopbio.com',
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
```

