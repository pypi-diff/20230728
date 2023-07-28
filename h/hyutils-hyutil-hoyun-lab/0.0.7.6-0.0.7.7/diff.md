# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.7.6.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.7.6.tar", last modified: Thu Jul 20 08:18:36 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.7.7.tar", last modified: Fri Jul 28 03:34:21 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6.tar` & `hyutils-hyutil-hoyun-lab-0.0.7.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:18:36.295349 hyutils-hyutil-hoyun-lab-0.0.7.6/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-07-20 08:18:36.294101 hyutils-hyutil-hoyun-lab-0.0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 08:18:36.295838 hyutils-hyutil-hoyun-lab-0.0.7.6/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-20 08:18:17.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:18:36.270837 hyutils-hyutil-hoyun-lab-0.0.7.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:18:36.287337 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      449 2023-07-20 08:18:17.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/augmentjob.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    16190 2023-07-20 08:17:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0    11383 2023-07-20 05:28:52.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:18:36.292837 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-07-20 08:18:36.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-07-20 08:18:36.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:18:36.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-20 08:18:36.000000 hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 03:34:21.785018 hyutils-hyutil-hoyun-lab-0.0.7.7/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-07-28 03:34:21.784539 hyutils-hyutil-hoyun-lab-0.0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 03:34:21.785158 hyutils-hyutil-hoyun-lab-0.0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-28 03:31:48.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:34:21.760169 hyutils-hyutil-hoyun-lab-0.0.7.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 03:34:21.778159 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      449 2023-07-28 03:31:48.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/augmentjob.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1477 2023-07-28 03:30:43.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    16190 2023-07-20 08:17:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0    11383 2023-07-20 05:28:52.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:34:21.783159 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-07-28 03:34:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-28 03:34:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:34:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 03:34:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.7.6
+Version: 0.0.7.7
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.7.6",
+    version="0.0.7.7",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/augmentjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/augmentjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/dirjob.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # path로 지정된 경로에 있는 서브디렉토리를 포함한 모든 디렉토리에 있는 파일들을 리턴.
     for root, dirs, files in os.walk(path):
         for file in files:
             extension = os.path.splitext(file)[1]
             # 특정 확장자인 경우만 리턴함.
             if extension == ext:
                 file_path = os.path.join(root, file)
-                yield file_path, root
+                yield root, file_path, file
 
 def dirs(path):
     for file in os.listdir(path):
         if os.path.isdir(os.path.join(path, file)):
             yield file
 
 def get_entry_count(path, ext):
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.7.6
+Version: 0.0.7.7
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.7.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.7.7/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

