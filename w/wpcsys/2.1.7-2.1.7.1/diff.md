# Comparing `tmp/wpcsys-2.1.7.tar.gz` & `tmp/wpcsys-2.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.1.7.tar", last modified: Thu Jul 27 07:01:23 2023, max compression
+gzip compressed data, was "wpcsys-2.1.7.1.tar", last modified: Thu Jul 27 07:37:00 2023, max compression
```

## Comparing `wpcsys-2.1.7.tar` & `wpcsys-2.1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.951336 wpcsys-2.1.7/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.7/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    10345 2023-07-27 07:01:23.943330 wpcsys-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     9284 2023-07-27 04:47:23.000000 wpcsys-2.1.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 07:01:23.951336 wpcsys-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2138 2023-07-27 04:32:46.000000 wpcsys-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.909185 wpcsys-2.1.7/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.7/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.7/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  7585280 2023-07-27 06:48:08.000000 wpcsys-2.1.7/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  8171520 2023-07-27 07:00:23.000000 wpcsys-2.1.7/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  8180224 2023-07-27 06:59:21.000000 wpcsys-2.1.7/wpcsys/pywpc.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0       17 2023-07-27 04:53:27.000000 wpcsys-2.1.7/wpcsys/version.py
-drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.940385 wpcsys-2.1.7/wpcsys.egg-info/
--rw-rw-rw-   0        0        0    10345 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 07:37:00.152497 wpcsys-2.1.7.1/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.7.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10347 2023-07-27 07:37:00.141498 wpcsys-2.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9284 2023-07-27 04:47:23.000000 wpcsys-2.1.7.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:37:00.152497 wpcsys-2.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2023-07-27 07:30:01.000000 wpcsys-2.1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:37:00.091505 wpcsys-2.1.7.1/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.7.1/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.7.1/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  7585280 2023-07-27 07:33:29.000000 wpcsys-2.1.7.1/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8171520 2023-07-27 07:36:20.000000 wpcsys-2.1.7.1/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8180224 2023-07-27 07:35:03.000000 wpcsys-2.1.7.1/wpcsys/pywpc.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0       19 2023-07-27 07:15:56.000000 wpcsys-2.1.7.1/wpcsys/version.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:37:00.137502 wpcsys-2.1.7.1/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0    10347 2023-07-27 07:36:59.000000 wpcsys-2.1.7.1/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-27 07:36:59.000000 wpcsys-2.1.7.1/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:36:59.000000 wpcsys-2.1.7.1/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-27 07:36:59.000000 wpcsys-2.1.7.1/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 07:36:59.000000 wpcsys-2.1.7.1/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.1.7/LICENSE` & `wpcsys-2.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.7/PKG-INFO` & `wpcsys-2.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.7
+Version: 2.1.7.1
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wpcsys-2.1.7/README.rst` & `wpcsys-2.1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.7/setup.py` & `wpcsys-2.1.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     """Distribution which always forces a binary package with platform name"""
     def has_ext_modules(x):
         return True
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", "r", encoding="utf-8") as fh:
-    install_requires = fh.readlines()
-    install_requires = [str_.rstrip(' \n') for str_ in install_requires]
+# with open("requirements.txt", "r", encoding="utf-8") as fh:
+#     install_requires = fh.readlines()
+#     install_requires = [str_.rstrip(' \n') for str_ in install_requires]
 
 sut.setup(
     name="wpcsys",
     version=version,
     description='WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)',
     long_description=long_description,
     long_description_content_type='text/x-rst',
@@ -55,10 +55,15 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     distclass=BinaryDistribution,
     license='MIT',
     keywords='wpc, daq, driver, usb, ethernet, wifi, data acquisition',
 
     include_package_data=True,
-    install_requires=install_requires,
+    install_requires=['pyusb>=1.2.1', 'numpy>=1.23.0',
+                      'qasync>=0.23.0', 'matplotlib>=3.5.2',
+                      'PyQt5Designer>=5.14.1', 'PyQt5>=5.15.4', 'PyQt5-Qt5>=5.15.2',
+                      'PyQt5-sip>=12.10.1',
+                      'wpcEXEbuild>=0.0.1'],
+
     python_requires='>=3.8',
 )
```

### Comparing `wpcsys-2.1.7/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.7.1/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.7/wpcsys.egg-info/PKG-INFO` & `wpcsys-2.1.7.1/wpcsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.7
+Version: 2.1.7.1
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
```

