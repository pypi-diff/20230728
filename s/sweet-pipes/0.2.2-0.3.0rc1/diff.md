# Comparing `tmp/sweet-pipes-0.2.2.tar.gz` & `tmp/sweet-pipes-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweet-pipes-0.2.2.tar", last modified: Fri Mar 10 03:12:26 2023, max compression
+gzip compressed data, was "sweet-pipes-0.3.0rc1.tar", last modified: Fri Jul 28 16:48:30 2023, max compression
```

## Comparing `sweet-pipes-0.2.2.tar` & `sweet-pipes-0.3.0rc1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/coco/coco_captions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/coco/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/coco/coco_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/coco/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes/laion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/laion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/laion/laion_2b_en.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/utils/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/utils/datapipes.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/sweet_pipes/utils/fileio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/sweet_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-10 03:12:26.000000 sweet-pipes-0.2.2/sweet_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-10 03:12:26.000000 sweet-pipes-0.2.2/sweet_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 03:12:26.000000 sweet-pipes-0.2.2/sweet_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-10 03:12:26.000000 sweet-pipes-0.2.2/sweet_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-10 03:12:26.000000 sweet-pipes-0.2.2/sweet_pipes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:12:26.955353 sweet-pipes-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-10 03:12:13.000000 sweet-pipes-0.2.2/tests/test_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_captions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/laion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/laion/laion_2b_en.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/datapipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/fileio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/waymo_open_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/tests/test_missing.py
```

### Comparing `sweet-pipes-0.2.2/LICENSE` & `sweet-pipes-0.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/PKG-INFO` & `sweet-pipes-0.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.2.2
+Version: 0.3.0rc1
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.2.2/README.md` & `sweet-pipes-0.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/setup.py` & `sweet-pipes-0.3.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     description="project_description",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "aiohttp[spedups]",
         "albumentations",
         "dill",
+        "gcloud-aio-storage",
         "Pillow",
+        "protobuf",
         "pyarrow",
         "pycocotools",
         "torchdata>=0.4.1",
         "wget",
     ],
     extras_require=extras_require,
     classifiers=[
```

### Comparing `sweet-pipes-0.2.2/sweet_pipes/coco/coco_captions.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_captions.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/coco/coco_detection.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_detection.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/coco/coco_keypoints.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_keypoints.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/coco/common.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/coco/common.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_12m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_3m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/laion/laion_2b_en.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/laion/laion_2b_en.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/utils/albumentations.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/utils/albumentations.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/utils/datapipes.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/utils/datapipes.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes/utils/fileio.py` & `sweet-pipes-0.3.0rc1/sweet_pipes/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.2.2/sweet_pipes.egg-info/PKG-INFO` & `sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.2.2
+Version: 0.3.0rc1
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.2.2/sweet_pipes.egg-info/SOURCES.txt` & `sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,8 +18,10 @@
 sweet_pipes/conceptual_captions/conceptual_captions_3m.py
 sweet_pipes/laion/__init__.py
 sweet_pipes/laion/laion_2b_en.py
 sweet_pipes/utils/__init__.py
 sweet_pipes/utils/albumentations.py
 sweet_pipes/utils/datapipes.py
 sweet_pipes/utils/fileio.py
+sweet_pipes/waymo_open_motion/__init__.py
+sweet_pipes/waymo_open_motion/waymo_open_motion.py
 tests/test_missing.py
```

