# Comparing `tmp/visionmetrics-0.0.3.tar.gz` & `tmp/visionmetrics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionmetrics-0.0.3.tar", last modified: Thu Jul  6 23:12:24 2023, max compression
+gzip compressed data, was "visionmetrics-0.0.4.tar", last modified: Thu Jul 27 22:16:03 2023, max compression
```

## Comparing `visionmetrics-0.0.3.tar` & `visionmetrics-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_matting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_prediction_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/caption/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/caption_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/cider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/coco_evalcap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/meteor.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/rougel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/classification/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/detection/mean_ap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/matting/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/boundary_foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/boundary_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/l1_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/matting_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/prediction_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/retrieval/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 22:16:03.112623 visionmetrics-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_matting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_prediction_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/tests/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/caption/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/caption_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/cider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/coco_evalcap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/caption/rougel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/classification/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/detection/mean_ap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/matting/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/boundary_foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/boundary_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/l1_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/matting_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/matting/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/prediction_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-27 22:12:55.000000 visionmetrics-0.0.4/visionmetrics/retrieval/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:16:03.108623 visionmetrics-0.0.4/visionmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-27 22:16:03.000000 visionmetrics-0.0.4/visionmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 22:16:03.000000 visionmetrics-0.0.4/visionmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:16:03.000000 visionmetrics-0.0.4/visionmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 22:16:03.000000 visionmetrics-0.0.4/visionmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 22:16:03.000000 visionmetrics-0.0.4/visionmetrics.egg-info/top_level.txt
```

### Comparing `visionmetrics-0.0.3/LICENSE` & `visionmetrics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/PKG-INFO` & `visionmetrics-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
+Provides-Extra: dev
 License-File: LICENSE
 
 # visionmetrics
 
 This repo contains evaluation metrics for vision tasks such as classification, object detection, image caption, and image matting. It uses [torchmetrics](https://github.com/Lightning-AI/torchmetrics) as a base library and extends it to support custom vision tasks as necessary.
 
 ## Available Metrics
```

### Comparing `visionmetrics-0.0.3/README.md` & `visionmetrics-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/setup.cfg` & `visionmetrics-0.0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 [metadata]
 name = visionmetrics
-version = 0.0.3
+version = 0.0.4
 description = Evaluation metric codes for various vision tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Microsoft
 license = MIT
 url = https://github.com/microsoft/visionmetrics
 
 [options]
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
 	numpy
 	torch
-	torchmetrics[detection]==0.11.4
+	torchmetrics[detection]~=1.0.1
 	opencv-python-headless
 	Pillow>=6.2.2
 
 [options.packages.find]
 exclude = 
 	test*
 
 [options.extras_require]
 caption = 
 	pycocoevalcap
 	pycocotools
+dev = 
+	pre-commit
+	flake8
+	isort
+	pytest
 
 [flake8]
 exclude = .git,build,dist,*venv,.idea
 max-line-length = 200
 per-file-ignores = __init__.py:F401
 
 [egg_info]
```

### Comparing `visionmetrics-0.0.3/tests/test_caption.py` & `visionmetrics-0.0.4/tests/test_caption.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/tests/test_classification.py` & `visionmetrics-0.0.4/tests/test_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             self.assertAlmostEqual(vmetric_avg_prec.item(), gts[fl_i], places=5)
 
 
 class TestROCAUC(unittest.TestCase):
     @staticmethod
     def _get_metric(predictions, targets, task='multiclass', num_classes=None, average='macro'):
         if task == 'binary':
-            metric = BinaryAUROC(num_classes=num_classes, average=average)
+            metric = BinaryAUROC()
         elif task == 'multiclass':
             metric = MulticlassAUROC(num_classes=num_classes, average=average)
         else:
             metric = MultilabelAUROC(num_labels=num_classes, average=average)
 
         metric.update(predictions, targets)
         roc_auc = metric.compute()
```

### Comparing `visionmetrics-0.0.3/tests/test_detection.py` & `visionmetrics-0.0.4/tests/test_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import unittest
 
+import torch
+
 from visionmetrics.detection import MeanAveragePrecision
 
 
 class TestDetection(unittest.TestCase):
     def test_perfect_one_image_absolute_coordinates(self):
 
         PREDICTIONS = [[[0, 1.0, 0, 0, 10, 10],
@@ -154,12 +156,12 @@
                                  [1, 0.1, 0.1, 0.5, 0.5]]]
 
         metric = MeanAveragePrecision(iou_thresholds=[0.5])
         metric.update(PREDICTIONS_REMAP_CAT_ID, TARGETS_REMAP_CAT_ID)
         result_remap_cat_id = metric.compute()
 
         for k in result.keys():
-            self.assertEqual(result[k], result_remap_cat_id[k])
+            self.assertTrue(torch.allclose(result[k], result_remap_cat_id[k]))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `visionmetrics-0.0.3/tests/test_matting.py` & `visionmetrics-0.0.4/tests/test_matting.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/tests/test_prediction_filters.py` & `visionmetrics-0.0.4/tests/test_prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/tests/test_retrieval.py` & `visionmetrics-0.0.4/tests/test_retrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 
 import torch
 
-from visionmetrics.retrieval import (RetrievalMAP, RetrievalPrecision, RetrievalPrecisionRecallCurveNPoints,
+from visionmetrics.retrieval import (RetrievalMAP, RetrievalPrecision,
+                                     RetrievalPrecisionRecallCurveNPoints,
                                      RetrievalRecall)
 
 
 class TestRetrievalPrecision(unittest.TestCase):
 
     PREDICTIONS = [torch.tensor([[5, 4, 3, 2, 1]]),
                    torch.tensor([[5, 4, 3, 2, 1]]),
@@ -40,15 +41,15 @@
                         [0, 0, 0, 0, 1.0],
                         [0.25, 0.25, 0.25, 0.25, 1.0],
                         [1.0, 1.0, 1.0],
                         [0.5, 0.5, 0.5]]
 
         for preds, target, exps, k in zip(self.PREDICTIONS, self.TARGETS, expectations, ks):
             for i in range(1, k):
-                metric = RetrievalRecall(k=i, adaptive_k=True)
+                metric = RetrievalRecall(top_k=i)
                 metric.update(preds.float(), target)
                 result = metric.compute()
                 self.assertAlmostEqual(result.item(), exps[i - 1], places=4)
 
     def test_precision_at_k(self):
         ks = [6, 8, 6, 6, 6, 6, 4, 4]
         expectations = [[1.0, 1.0, 0.66666, 0.5, 0.6],
@@ -58,15 +59,15 @@
                         [0, 0, 0, 0, 0.2],
                         [0.5, 0.25, 0.16666, 0.125, 0.3],
                         [1.0, 1.0, 1.0],
                         [0.5, 0.5, 0.5]]
 
         for preds, target, exps, k in zip(self.PREDICTIONS, self.TARGETS, expectations, ks):
             for i in range(1, k):
-                metric = RetrievalPrecision(k=i, adaptive_k=True)
+                metric = RetrievalPrecision(top_k=i, adaptive_k=True)
                 metric.update(preds.float(), target)
                 result = metric.compute()
                 self.assertAlmostEqual(result.item(), exps[i - 1], places=4)
 
     def test_mean_average_precision_at_k(self):
         targets = [torch.tensor([[1, 0, 1, 1],
                                  [1, 0, 0, 1]]),
@@ -90,23 +91,24 @@
                        torch.tensor([[4, 2, 3, 5]]),
                        torch.tensor([[2, 3, 5, 4]]),
                        torch.tensor([[2, 3, 5, 4]]),
                        torch.tensor([[2, 3, 5, 4]]),
                        torch.tensor([[2, 3, 5, 4]]),
                        torch.tensor([[2, 3, 5]]),
                        torch.tensor([[2, 3, 5, 4, 2, 3, 5, 4, 2, 3, 5, 4, 2, 3, 5, 7, 3, 4]])]
-        rank = [4, 4, 4, 4, 4, 4, 3, 3, 5, 2, 4, 4, 8]
-        expectations = [0.77777, 0.80555, 0.75, 0.91666, 1.0, 1.0, 0.91666, 0.91666, 0.91666, 0.0, 0.83333, 0.8220]
+        rank = [5, 4, 4, 4, 4, 3, 3, 5, 2, 4, 4, 8]
+        expectations = [0.77777, 0.80555, 0.75, 0.91666, 1.0, 1.0, 1.0, 0.91666, 1.0, 0.0, 0.83333, 0.9306]
 
         for preds, target, exps, k in zip(predictions, targets, expectations, rank):
             if preds.numel() == 0:
                 continue
-            metric = RetrievalMAP(k=k, adaptive_k=True)
+            metric = RetrievalMAP(top_k=k)
             metric.update(preds.float(), target)
             result = metric.compute()
+            print(result)
             self.assertAlmostEqual(result.item(), exps, places=4)
 
     def test_precision_recall_curve_n_points(self):
 
         predictions = [torch.tensor([[0.8, 0.5, 0.2],
                                      [0.8, 0.2, 0.7]]),
                        torch.tensor([[0.9, 0.0, 0.1]]),
```

### Comparing `visionmetrics-0.0.3/visionmetrics/caption/caption_eval_base.py` & `visionmetrics-0.0.4/visionmetrics/caption/caption_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/caption/coco_evalcap_utils.py` & `visionmetrics-0.0.4/visionmetrics/caption/coco_evalcap_utils.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/classification/__init__.py` & `visionmetrics-0.0.4/visionmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/classification/precision_recall.py` & `visionmetrics-0.0.4/visionmetrics/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/boundary_foreground_iou.py` & `visionmetrics-0.0.4/visionmetrics/matting/boundary_foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/boundary_mean_iou.py` & `visionmetrics-0.0.4/visionmetrics/matting/boundary_mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/foreground_iou.py` & `visionmetrics-0.0.4/visionmetrics/matting/foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/l1_error.py` & `visionmetrics-0.0.4/visionmetrics/matting/l1_error.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/matting_eval_base.py` & `visionmetrics-0.0.4/visionmetrics/matting/matting_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/matting/mean_iou.py` & `visionmetrics-0.0.4/visionmetrics/matting/mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/prediction_filters.py` & `visionmetrics-0.0.4/visionmetrics/prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics/retrieval/precision_recall.py` & `visionmetrics-0.0.4/visionmetrics/retrieval/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.3/visionmetrics.egg-info/PKG-INFO` & `visionmetrics-0.0.4/visionmetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
+Provides-Extra: dev
 License-File: LICENSE
 
 # visionmetrics
 
 This repo contains evaluation metrics for vision tasks such as classification, object detection, image caption, and image matting. It uses [torchmetrics](https://github.com/Lightning-AI/torchmetrics) as a base library and extends it to support custom vision tasks as necessary.
 
 ## Available Metrics
```

### Comparing `visionmetrics-0.0.3/visionmetrics.egg-info/SOURCES.txt` & `visionmetrics-0.0.4/visionmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

