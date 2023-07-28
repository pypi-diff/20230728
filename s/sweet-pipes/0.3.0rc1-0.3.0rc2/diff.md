# Comparing `tmp/sweet-pipes-0.3.0rc1.tar.gz` & `tmp/sweet-pipes-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweet-pipes-0.3.0rc1.tar", last modified: Fri Jul 28 16:48:30 2023, max compression
+gzip compressed data, was "sweet-pipes-0.3.0rc2.tar", last modified: Fri Jul 28 17:54:05 2023, max compression
```

## Comparing `sweet-pipes-0.3.0rc1.tar` & `sweet-pipes-0.3.0rc2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_captions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/coco/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/laion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/laion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/laion/laion_2b_en.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/datapipes.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/utils/fileio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/waymo_open_motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:48:30.000000 sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:48:30.448162 sweet-pipes-0.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 16:48:19.000000 sweet-pipes-0.3.0rc1/tests/test_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 17:54:05.899269 sweet-pipes-0.3.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.891270 sweet-pipes-0.3.0rc2/sweet_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_captions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/coco/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/laion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/laion/laion_2b_en.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/datapipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/utils/fileio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/datapipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 17:54:05.000000 sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:54:05.895269 sweet-pipes-0.3.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 17:53:51.000000 sweet-pipes-0.3.0rc2/tests/test_missing.py
```

### Comparing `sweet-pipes-0.3.0rc1/LICENSE` & `sweet-pipes-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/PKG-INFO` & `sweet-pipes-0.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.3.0rc1/README.md` & `sweet-pipes-0.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/setup.py` & `sweet-pipes-0.3.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_captions.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_captions.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_detection.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_detection.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/coco/coco_keypoints.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/coco/coco_keypoints.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/coco/common.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/coco/common.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_12m.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_12m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/conceptual_captions/conceptual_captions_3m.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/conceptual_captions/conceptual_captions_3m.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/laion/laion_2b_en.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/laion/laion_2b_en.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/utils/albumentations.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/utils/albumentations.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/utils/datapipes.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/utils/datapipes.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/utils/fileio.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes/waymo_open_motion/waymo_open_motion.py` & `sweet-pipes-0.3.0rc2/sweet_pipes/waymo/waymo_open_motion/datapipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from gcloud.aio.storage import Storage
 from torchdata.datapipes.iter import IterDataPipe
 from torchdata.datapipes.utils import StreamWrapper
 from tqdm import tqdm
 
 T = TypeVar("T")
 URL_TEMPLATE = (
-    "gs://waymo_open_dataset_motion_v_1_2_0/uncompressed/tf_example/"
-    "{name}/{name}_tfexample.tfrecord-{idx:05d}-of-01000"
+    "gs://waymo_open_dataset_motion_v_1_2_0/uncompressed/{format}/"
+    "{dataset_name}/{file_name}.tfrecord-{idx:05d}-of-01000"
 )
 SPLIT_TO_DATASET_NAME = {
     "train": "training",
     "validation": "validation",
     "test": "testing",
 }
 
@@ -117,30 +117,41 @@
         self.dp = dp
 
     def __iter__(self) -> Generator[T, None, None]:
         iterator = iter(self.dp)
         while True:
             try:
                 yield next(iterator)
-            except OverflowError:
-                logging.error("OverflowError encountered, skipping sample")
+            except (MemoryError, OverflowError) as e:
+                logging.error(
+                    f"{type(e).__name__} encountered. Skipping sample.  {str(e)}"
+                )
+                breakpoint()
+                pass
             except StopIteration:
                 break
 
 
 def waymo_open_motion_datapipe(
     split: Literal["train", "validation", "test"],
+    format: Literal["scenario", "tf_example"] = "tf_example",
     cache_dir: Optional[str] = None,
     shuffle: bool = False,
     shuffle_buffer_size: int = 128,
     prefetch_factor: int = 1,
     verbose: bool = False,
 ) -> IterDataPipe:
-    name = SPLIT_TO_DATASET_NAME[split]
-    tfrecord_urls = [URL_TEMPLATE.format(name=name, idx=idx) for idx in range(1000)]
+    dataset_name = SPLIT_TO_DATASET_NAME[split]
+    file_name = dataset_name if format == "scenario" else f"{dataset_name}_tfexample"
+    tfrecord_urls = [
+        URL_TEMPLATE.format(
+            format=format, dataset_name=dataset_name, file_name=file_name, idx=idx
+        )
+        for idx in range(1000)
+    ]
 
     dp = IterableWrapper(tfrecord_urls)
     if shuffle:
         # Shuffle the order of the TFRecord files.  This costs us nothing, since we
         # already have all of the URLs in memory.  We will shuffle again later, once
         # the samples have been loaded, using a small buffer for memory constraints.
         dp.shuffle()
@@ -151,20 +162,22 @@
         prefetch_factor=prefetch_factor,
         verbose=verbose,
     )
     dp = dp.load_from_tfrecord()
     dp = OverflowErrorHandler(dp)
     if shuffle:
         # Shuffle the loaded samples.  We use a small buffer to (hopefully) avoid
-        # out-of-memory errors.  The entire dataset is
+        # out-of-memory errors.  The entire dataset is on the order or 1 TiB (depends
+        # on whether you're using 'scenario' or 'tf_example' format), so we can
+        # only shuffle a small fraction of the data in memory.
         dp = dp.shuffle(buffer_size=shuffle_buffer_size)
 
     return dp
 
 
 if __name__ == "__main__":
     from torchdata.datapipes.iter import IterableWrapper
     from tqdm import tqdm
 
-    dp = waymo_open_motion_datapipe(split="train", verbose=True)
+    dp = waymo_open_motion_datapipe(split="train", prefetch_factor=2, verbose=True)
     for x in tqdm(dp):
         pass
```

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/PKG-INFO` & `sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweet-pipes
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: project_description
 Home-page: https://github.com/fkodom/sweet-pipes
 Author: Frank Odom
 Author-email: frank.odom.iii@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sweet-pipes-0.3.0rc1/sweet_pipes.egg-info/SOURCES.txt` & `sweet-pipes-0.3.0rc2/sweet_pipes.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,10 +18,12 @@
 sweet_pipes/conceptual_captions/conceptual_captions_3m.py
 sweet_pipes/laion/__init__.py
 sweet_pipes/laion/laion_2b_en.py
 sweet_pipes/utils/__init__.py
 sweet_pipes/utils/albumentations.py
 sweet_pipes/utils/datapipes.py
 sweet_pipes/utils/fileio.py
-sweet_pipes/waymo_open_motion/__init__.py
-sweet_pipes/waymo_open_motion/waymo_open_motion.py
+sweet_pipes/waymo/__init__.py
+sweet_pipes/waymo/waymo_open_motion/__init__.py
+sweet_pipes/waymo/waymo_open_motion/datapipe.py
+sweet_pipes/waymo/waymo_open_motion/visualize.py
 tests/test_missing.py
```

