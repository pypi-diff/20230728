# Comparing `tmp/miso2-3.0.4.tar.gz` & `tmp/miso2-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miso2-3.0.4.tar", last modified: Thu Apr 27 14:14:00 2023, max compression
+gzip compressed data, was "miso2-3.0.5.tar", last modified: Fri Jul 28 04:33:33 2023, max compression
```

## Comparing `miso2-3.0.4.tar` & `miso2-3.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.790503 miso2-3.0.4/
--rw-rw-rw-   0        0        0     1062 2023-04-17 11:49:46.000000 miso2-3.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0      838 2023-04-27 14:14:00.789497 miso2-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-17 11:49:46.000000 miso2-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.500793 miso2-3.0.4/miso/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/__init__.py
--rw-rw-rw-   0        0        0     2257 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.577591 miso2-3.0.4/miso/data/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/__init__.py
--rw-rw-rw-   0        0        0     2829 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/dataset.py
--rw-rw-rw-   0        0        0     1610 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/download.py
--rw-rw-rw-   0        0        0     7520 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/filenames_dataset.py
--rw-rw-rw-   0        0        0     3213 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_dataset.py
--rw-rw-rw-   0        0        0     2651 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_loader.py
--rw-rw-rw-   0        0        0     4074 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/image_utils.py
--rw-rw-rw-   0        0        0     8146 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/tf_generator.py
--rw-rw-rw-   0        0        0     5646 2023-04-27 08:34:09.000000 miso2-3.0.4/miso/data/training_dataset.py
--rw-rw-rw-   0        0        0     3565 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.601790 miso2-3.0.4/miso/deploy/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/__init__.py
--rw-rw-rw-   0        0        0     5993 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/inference.py
--rw-rw-rw-   0        0        0     6285 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/model_info.py
--rw-rw-rw-   0        0        0     8394 2023-04-25 22:30:59.000000 miso2-3.0.4/miso/deploy/saving.py
--rw-rw-rw-   0        0        0     5275 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/deploy/server.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.642604 miso2-3.0.4/miso/layers/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/__init__.py
--rw-rw-rw-   0        0        0     4432 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/_common_blocks.py
--rw-rw-rw-   0        0        0     2127 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/asoftmax.py
--rw-rw-rw-   0        0        0     2904 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/batch_instance_normalisation.py
--rw-rw-rw-   0        0        0     3386 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/cyclic.py
--rw-rw-rw-   0        0        0     8188 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/group_normalisation.py
--rw-rw-rw-   0        0        0     2546 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/layers/msoftmax.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.676706 miso2-3.0.4/miso/models/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/__init__.py
--rw-rw-rw-   0        0        0     4596 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/base_cyclic.py
--rw-rw-rw-   0        0        0     5798 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/factory.py
--rw-rw-rw-   0        0        0       56 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/model_zoo.py
--rw-rw-rw-   0        0        0    13297 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/models/resnet_cyclic.py
--rw-rw-rw-   0        0        0     4884 2023-04-27 12:22:14.000000 miso2-3.0.4/miso/models/transfer_learning.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.720827 miso2-3.0.4/miso/stats/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/__init__.py
--rw-rw-rw-   0        0        0     1490 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/accuracy.py
--rw-rw-rw-   0        0        0    14013 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/confusion_matrix.py
--rw-rw-rw-   0        0        0     6294 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/embedding.py
--rw-rw-rw-   0        0        0     4983 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/mislabelling.py
--rw-rw-rw-   0        0        0      909 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/most_representative.py
--rw-rw-rw-   0        0        0     1496 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/projections.py
--rw-rw-rw-   0        0        0      993 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/stats/training.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.746757 miso2-3.0.4/miso/training/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/__init__.py
--rw-rw-rw-   0        0        0     5042 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/adaptive_learning_rate.py
--rw-rw-rw-   0        0        0     3282 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/parameters.py
--rw-rw-rw-   0        0        0     5374 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/tf_augmentation.py
--rw-rw-rw-   0        0        0    25756 2023-04-27 10:48:06.000000 miso2-3.0.4/miso/training/trainer.py
--rw-rw-rw-   0        0        0     1757 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/training/training_result.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.788502 miso2-3.0.4/miso/utils/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/__init__.py
--rw-rw-rw-   0        0        0    10218 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/flowcam.py
--rw-rw-rw-   0        0        0      757 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/lock.py
--rw-rw-rw-   0        0        0      227 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/misc.py
--rw-rw-rw-   0        0        0     1455 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/rolling_buffer.py
--rw-rw-rw-   0        0        0     5300 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/singleton.py
--rw-rw-rw-   0        0        0    10056 2023-04-17 11:49:46.000000 miso2-3.0.4/miso/utils/wave.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:14:00.517763 miso2-3.0.4/miso2.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 14:14:00.000000 miso2-3.0.4/miso2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 14:14:00.790503 miso2-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-04-27 14:13:46.000000 miso2-3.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.791472 miso2-3.0.5/
+-rw-rw-rw-   0        0        0     1062 2023-04-17 11:49:46.000000 miso2-3.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0      875 2023-07-28 04:33:33.791472 miso2-3.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-07-28 04:30:30.000000 miso2-3.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.749543 miso2-3.0.5/miso/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.765126 miso2-3.0.5/miso/data/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/__init__.py
+-rw-rw-rw-   0        0        0     2829 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/dataset.py
+-rw-rw-rw-   0        0        0     1610 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/download.py
+-rw-rw-rw-   0        0        0     7520 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/filenames_dataset.py
+-rw-rw-rw-   0        0        0     3213 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/image_dataset.py
+-rw-rw-rw-   0        0        0     2651 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/image_loader.py
+-rw-rw-rw-   0        0        0     4074 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/image_utils.py
+-rw-rw-rw-   0        0        0     8146 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/tf_generator.py
+-rw-rw-rw-   0        0        0     5479 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/data/training_dataset.py
+-rw-rw-rw-   0        0        0     3565 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.767934 miso2-3.0.5/miso/deploy/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/deploy/__init__.py
+-rw-rw-rw-   0        0        0     5993 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/deploy/inference.py
+-rw-rw-rw-   0        0        0     6285 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/deploy/model_info.py
+-rw-rw-rw-   0        0        0     8394 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/deploy/saving.py
+-rw-rw-rw-   0        0        0     5275 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/deploy/server.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.772809 miso2-3.0.5/miso/layers/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/__init__.py
+-rw-rw-rw-   0        0        0     4432 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/_common_blocks.py
+-rw-rw-rw-   0        0        0     2127 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/asoftmax.py
+-rw-rw-rw-   0        0        0     2904 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/batch_instance_normalisation.py
+-rw-rw-rw-   0        0        0     3386 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/cyclic.py
+-rw-rw-rw-   0        0        0     8188 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/group_normalisation.py
+-rw-rw-rw-   0        0        0     2546 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/layers/msoftmax.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.776816 miso2-3.0.5/miso/models/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/models/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/models/base_cyclic.py
+-rw-rw-rw-   0        0        0     5798 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/models/factory.py
+-rw-rw-rw-   0        0        0       56 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/models/model_zoo.py
+-rw-rw-rw-   0        0        0    13297 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/models/resnet_cyclic.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/models/transfer_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.781815 miso2-3.0.5/miso/stats/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/__init__.py
+-rw-rw-rw-   0        0        0     1490 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/accuracy.py
+-rw-rw-rw-   0        0        0    14013 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/confusion_matrix.py
+-rw-rw-rw-   0        0        0     6294 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/embedding.py
+-rw-rw-rw-   0        0        0     4983 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/stats/mislabelling.py
+-rw-rw-rw-   0        0        0      909 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/most_representative.py
+-rw-rw-rw-   0        0        0     1496 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/projections.py
+-rw-rw-rw-   0        0        0      993 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/stats/training.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.786103 miso2-3.0.5/miso/training/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/training/__init__.py
+-rw-rw-rw-   0        0        0     5042 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/training/adaptive_learning_rate.py
+-rw-rw-rw-   0        0        0     3282 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/training/parameters.py
+-rw-rw-rw-   0        0        0     5374 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/training/tf_augmentation.py
+-rw-rw-rw-   0        0        0    25513 2023-07-28 04:31:08.000000 miso2-3.0.5/miso/training/trainer.py
+-rw-rw-rw-   0        0        0     1757 2023-07-28 04:30:30.000000 miso2-3.0.5/miso/training/training_result.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.791472 miso2-3.0.5/miso/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/__init__.py
+-rw-rw-rw-   0        0        0    10218 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/flowcam.py
+-rw-rw-rw-   0        0        0      757 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/lock.py
+-rw-rw-rw-   0        0        0      227 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/misc.py
+-rw-rw-rw-   0        0        0     1455 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/rolling_buffer.py
+-rw-rw-rw-   0        0        0     5300 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/singleton.py
+-rw-rw-rw-   0        0        0    10056 2023-04-17 11:49:46.000000 miso2-3.0.5/miso/utils/wave.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:33:33.759122 miso2-3.0.5/miso2.egg-info/
+-rw-rw-rw-   0        0        0      875 2023-07-28 04:33:33.000000 miso2-3.0.5/miso2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-07-28 04:33:33.000000 miso2-3.0.5/miso2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:33:33.000000 miso2-3.0.5/miso2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2023-07-28 04:33:33.000000 miso2-3.0.5/miso2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-28 04:33:33.000000 miso2-3.0.5/miso2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:33:33.791472 miso2-3.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-07-28 04:33:26.000000 miso2-3.0.5/setup.py
```

### Comparing `miso2-3.0.4/LICENCE.txt` & `miso2-3.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/PKG-INFO` & `miso2-3.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
+Description: # particle-classification
+        Python scripts for particle classification
+        
+        https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
+        
 Keywords: microfossil,cnn
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# particle-classification
-Python scripts for particle classification
-
-https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
```

### Comparing `miso2-3.0.4/miso/__main__.py` & `miso2-3.0.5/miso/__main__.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/dataset.py` & `miso2-3.0.5/miso/data/dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/download.py` & `miso2-3.0.5/miso/data/download.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/filenames_dataset.py` & `miso2-3.0.5/miso/data/filenames_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/image_dataset.py` & `miso2-3.0.5/miso/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/image_loader.py` & `miso2-3.0.5/miso/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/image_utils.py` & `miso2-3.0.5/miso/data/image_utils.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/tf_generator.py` & `miso2-3.0.5/miso/data/tf_generator.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/data/training_dataset.py` & `miso2-3.0.5/miso/data/training_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,22 +63,18 @@
         # Class weights
         weights = gmean(fs.cls_counts) / fs.cls_counts
         weights[weights < 0.1] = 0.1
         weights[weights > 10] = 10
         self.class_weights = weights
 
         # Create split
-        if self.test_split > 0:
-            self.train_idx, self.test_idx = train_test_split(np.arange(len(self.filenames.filenames)),
-                                                             stratify=self.cls,
-                                                             test_size=self.test_split,
-                                                             random_state=self.random_seed)
-        else:
-            self.train_idx = np.arange(len(self.filenames.filenames))
-            self.test_idx = []
+        self.train_idx, self.test_idx = train_test_split(np.arange(len(self.filenames.filenames)),
+                                                         stratify=self.cls,
+                                                         test_size=self.test_split,
+                                                         random_state=self.random_seed)
 
         # Load images
         to_greyscale = False
         if self.img_type == 'k' or self.img_type == 'greyscale':
             to_greyscale = True
         # print(self.img_size)
         self.images = ImageDataset(self.filenames.filenames,
```

### Comparing `miso2-3.0.4/miso/data/utils.py` & `miso2-3.0.5/miso/data/utils.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/deploy/inference.py` & `miso2-3.0.5/miso/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/deploy/model_info.py` & `miso2-3.0.5/miso/deploy/model_info.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/deploy/saving.py` & `miso2-3.0.5/miso/deploy/saving.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/deploy/server.py` & `miso2-3.0.5/miso/deploy/server.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/_common_blocks.py` & `miso2-3.0.5/miso/layers/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/asoftmax.py` & `miso2-3.0.5/miso/layers/asoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/batch_instance_normalisation.py` & `miso2-3.0.5/miso/layers/batch_instance_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/cyclic.py` & `miso2-3.0.5/miso/layers/cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/group_normalisation.py` & `miso2-3.0.5/miso/layers/group_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/layers/msoftmax.py` & `miso2-3.0.5/miso/layers/msoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/models/base_cyclic.py` & `miso2-3.0.5/miso/models/base_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/models/factory.py` & `miso2-3.0.5/miso/models/factory.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/models/resnet_cyclic.py` & `miso2-3.0.5/miso/models/resnet_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/models/transfer_learning.py` & `miso2-3.0.5/miso/models/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/accuracy.py` & `miso2-3.0.5/miso/stats/accuracy.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/confusion_matrix.py` & `miso2-3.0.5/miso/stats/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/embedding.py` & `miso2-3.0.5/miso/stats/embedding.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/mislabelling.py` & `miso2-3.0.5/miso/stats/mislabelling.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/most_representative.py` & `miso2-3.0.5/miso/stats/most_representative.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/projections.py` & `miso2-3.0.5/miso/stats/projections.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/stats/training.py` & `miso2-3.0.5/miso/stats/training.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/training/adaptive_learning_rate.py` & `miso2-3.0.5/miso/training/adaptive_learning_rate.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/training/parameters.py` & `miso2-3.0.5/miso/training/parameters.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/training/tf_augmentation.py` & `miso2-3.0.5/miso/training/tf_augmentation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/training/trainer.py` & `miso2-3.0.5/miso/training/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Creates and trains a generic network
 """
 import os
 import skimage.io
 import warnings
+import matplotlib.pyplot as plt
+plt.switch_backend('agg')
 
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
-# from clearml import Task
-
 import time
 import datetime
 from collections import OrderedDict
 import tensorflow.keras.backend as K
 from sklearn.manifold import TSNE
 
 from miso.data.tf_generator import TFGenerator
@@ -48,26 +48,18 @@
         pass
     results = np.concatenate(results, axis=0)
     return results
 
 
 def train_image_classification_model(tp: MisoParameters):
     tf_version = int(tf.__version__[0])
-    now = datetime.datetime.now()
-
-    # ClearML task
-    # print(f"ClearML initialising")
-    # task = Task.init(project_name='MISO',
-    #                  task_name=f"{tp.name}_{now:%Y%m%d-%H%M%S}")
-    # task.connect(tp)
 
     # Hack to make RTX cards work
     if tf_version == 2:
         physical_devices = tf.config.list_physical_devices("GPU")
-        print(physical_devices)
         for device in physical_devices:
             tf.config.experimental.set_memory_growth(device, True)
     else:
         config = tf.ConfigProto()
         config.gpu_options.allow_growth = True
         session = tf.Session(config=config)
 
@@ -105,14 +97,15 @@
         tp.dataset.random_seed,
         tp.dataset.memmap_directory,
     )
     ds.load()
     tp.dataset.num_classes = ds.num_classes
 
     # Create save lodations
+    now = datetime.datetime.now()
     save_dir = os.path.join(
         tp.output.save_dir, "{0}_{1:%Y%m%d-%H%M%S}".format(tp.name, now)
     )
     os.makedirs(save_dir, exist_ok=True)
 
     # ------------------------------------------------------------------------------
     # Transfer learning
@@ -422,15 +415,14 @@
         print(" {:.3f}ms".format(diff), end="")
     inference_time = np.median(inf_times)
     print(", median: {}".format(inference_time))
     # Store results
     # - fix to make key same for tensorflow 1 and 2
     if "accuracy" in history.history:
         history.history["acc"] = history.history.pop("accuracy")
-    if "val_accuracy" in history.history:
         history.history["val_acc"] = history.history.pop("val_accuracy")
     result = TrainingResult(
         tp,
         history,
         y_true,
         y_pred,
         y_prob,
```

### Comparing `miso2-3.0.4/miso/training/training_result.py` & `miso2-3.0.5/miso/training/training_result.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/utils/flowcam.py` & `miso2-3.0.5/miso/utils/flowcam.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/utils/lock.py` & `miso2-3.0.5/miso/utils/lock.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/utils/rolling_buffer.py` & `miso2-3.0.5/miso/utils/rolling_buffer.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/utils/singleton.py` & `miso2-3.0.5/miso/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso/utils/wave.py` & `miso2-3.0.5/miso/utils/wave.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/miso2.egg-info/PKG-INFO` & `miso2-3.0.5/miso2.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
+Description: # particle-classification
+        Python scripts for particle classification
+        
+        https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
+        
 Keywords: microfossil,cnn
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# particle-classification
-Python scripts for particle classification
-
-https://stackoverflow.com/questions/53779509/upload-failed-403-invalid-or-non-existent-authentication-information-python
```

### Comparing `miso2-3.0.4/miso2.egg-info/SOURCES.txt` & `miso2-3.0.5/miso2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miso2-3.0.4/setup.py` & `miso2-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='miso2',
-    version='3.0.4',
+    version='3.0.5',
     description='Python scripts for training CNNs for particle classification',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ross Marchant',
     author_email='ross.g.marchant@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

