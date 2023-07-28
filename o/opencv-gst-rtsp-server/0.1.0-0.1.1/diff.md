# Comparing `tmp/opencv_gst_rtsp_server-0.1.0.tar.gz` & `tmp/opencv_gst_rtsp_server-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_gst_rtsp_server-0.1.0.tar", last modified: Fri Jul 28 08:34:51 2023, max compression
+gzip compressed data, was "opencv_gst_rtsp_server-0.1.1.tar", last modified: Fri Jul 28 08:45:43 2023, max compression
```

## Comparing `opencv_gst_rtsp_server-0.1.0.tar` & `opencv_gst_rtsp_server-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      670 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/PKG-INFO
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      880 2023-07-28 08:30:13.000000 opencv_gst_rtsp_server-0.1.0/README.md
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.085573 opencv_gst_rtsp_server-0.1.0/build/
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/build/opencv_gst_rtsp_server.egg-info/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      787 2023-07-28 08:34:51.000000 opencv_gst_rtsp_server-0.1.0/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      458 2023-07-28 08:25:39.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/__init__.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/exception/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:13.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/exception/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      200 2023-07-28 04:12:31.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/exception/network_exception.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:16.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1727 2023-07-28 04:13:53.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1522 2023-07-28 04:13:59.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2315 2023-07-28 04:14:05.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:18.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      616 2023-07-28 04:14:10.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2302 2023-07-28 04:14:18.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      515 2023-07-28 04:14:22.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py
-drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/utils/
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:21.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/utils/__init__.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      334 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/utils/log_utils.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      621 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/utils/network_utils.py
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      151 2023-07-28 08:34:51.089573 opencv_gst_rtsp_server-0.1.0/setup.cfg
--rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      952 2023-07-28 08:33:51.000000 opencv_gst_rtsp_server-0.1.0/setup.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1935 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/PKG-INFO
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      880 2023-07-28 08:30:13.000000 opencv_gst_rtsp_server-0.1.1/README.md
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/build/
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/build/opencv_gst_rtsp_server.egg-info/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      787 2023-07-28 08:45:43.000000 opencv_gst_rtsp_server-0.1.1/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      458 2023-07-28 08:25:39.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/__init__.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/exception/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:13.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/exception/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      200 2023-07-28 04:12:31.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/exception/network_exception.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:16.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1727 2023-07-28 04:13:53.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1522 2023-07-28 04:13:59.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2315 2023-07-28 04:14:05.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:18.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      616 2023-07-28 04:14:10.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     2302 2023-07-28 04:14:18.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      515 2023-07-28 04:14:22.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py
+drwxrwxr-x   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/utils/
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)        0 2023-07-28 04:16:21.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/utils/__init__.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      334 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/utils/log_utils.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      621 2023-07-28 04:12:44.000000 opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/utils/network_utils.py
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)      151 2023-07-28 08:45:43.104021 opencv_gst_rtsp_server-0.1.1/setup.cfg
+-rw-rw-r--   0 nguyencobap  (1000) nguyencobap  (1000)     1063 2023-07-28 08:44:57.000000 opencv_gst_rtsp_server-0.1.1/setup.py
```

### Comparing `opencv_gst_rtsp_server-0.1.0/README.md` & `opencv_gst_rtsp_server-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt` & `opencv_gst_rtsp_server-0.1.1/build/opencv_gst_rtsp_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_frame_media_factory.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_media_factory.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_media_factory/opencv_stream_media_factory.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_frame_rtsp_server.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_rtsp_server.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/rtsp_server/opencv_stream_rtsp_server.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/opencv_gst_rtsp_server/utils/network_utils.py` & `opencv_gst_rtsp_server-0.1.1/opencv_gst_rtsp_server/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `opencv_gst_rtsp_server-0.1.0/setup.py` & `opencv_gst_rtsp_server-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import io
 from setuptools import setup, find_packages
 
+long_description = io.open("README.md", encoding="utf-8").read()
+
 setup(
     name='opencv_gst_rtsp_server',
-    version='0.1.0',    
+    version='0.1.1',
     description='Restream rtsp with opencv frame using gst-rtsp-server',
     url='https://github.com/nguyencobap/opencv_gst_rtsp_server',
     author='Nguyen Hai Nguyen',
     author_email='nguyenhainguyen97@gmail.com',
     license='MIT License',
     python_requires=">=3.5",
     packages=find_packages(),
+    long_description=long_description,
     keywords=['gstreamer', 'gst', 'opencv', 'rtsp'],
     install_requires=['opencv-python>=4.6.0.66',
                         'pycairo>=1.24.0',
                         'PyGObject>=3.44.1'
                         ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

