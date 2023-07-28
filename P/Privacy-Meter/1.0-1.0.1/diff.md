# Comparing `tmp/privacy_meter-1.0.tar.gz` & `tmp/Privacy-Meter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/privacy_meter-1.0.tar", last modified: Fri May 13 08:53:27 2022, max compression
+gzip compressed data, was "Privacy-Meter-1.0.1.tar", last modified: Fri Jul 28 14:17:26 2023, max compression
```

## Comparing `privacy_meter-1.0.tar` & `Privacy-Meter-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 aadyaamaddi   (501) staff       (20)        0 2022-05-13 08:53:27.000000 privacy_meter-1.0/
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     1562 2022-05-13 08:53:27.000000 privacy_meter-1.0/PKG-INFO
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     1115 2022-02-23 02:03:32.000000 privacy_meter-1.0/LICENSE
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)      107 2022-05-12 12:50:40.000000 privacy_meter-1.0/requirements.txt
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)       89 2022-05-13 03:15:30.000000 privacy_meter-1.0/MANIFEST.in
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     2858 2022-05-13 04:26:18.000000 privacy_meter-1.0/README.md
-drwxr-xr-x   0 aadyaamaddi   (501) staff       (20)        0 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter/
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)    26561 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/audit_report.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)    13145 2022-05-12 12:57:04.000000 privacy_meter-1.0/privacy_meter/information_source_signal.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     6896 2022-05-12 12:10:57.000000 privacy_meter-1.0/privacy_meter/audit.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     2107 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/constants.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)        0 2022-05-12 08:01:35.000000 privacy_meter-1.0/privacy_meter/__init__.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)      927 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/hypothesis_test.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)    16971 2022-05-12 12:57:04.000000 privacy_meter-1.0/privacy_meter/model.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     9092 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/dataset.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)    28051 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/metric.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)      567 2022-05-12 08:01:36.000000 privacy_meter-1.0/privacy_meter/utils.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     2692 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/metric_result.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     3853 2022-05-12 12:37:07.000000 privacy_meter-1.0/privacy_meter/information_source.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     1126 2022-05-13 04:32:49.000000 privacy_meter-1.0/setup.py
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     1071 2022-05-13 04:26:18.000000 privacy_meter-1.0/project_description.md
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)       38 2022-05-13 08:53:27.000000 privacy_meter-1.0/setup.cfg
-drwxr-xr-x   0 aadyaamaddi   (501) staff       (20)        0 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter.egg-info/
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)     1562 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter.egg-info/PKG-INFO
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)      570 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter.egg-info/SOURCES.txt
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)       14 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter.egg-info/top_level.txt
--rw-r--r--   0 aadyaamaddi   (501) staff       (20)        1 2022-05-13 08:53:27.000000 privacy_meter-1.0/privacy_meter.egg-info/dependency_links.txt
+drwxr-xr-x   0 hongyan   (1000) hongyan   (1000)        0 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     1115 2023-02-07 09:02:13.000000 Privacy-Meter-1.0.1/LICENSE
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)       89 2023-02-07 09:02:13.000000 Privacy-Meter-1.0.1/MANIFEST.in
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     9586 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/PKG-INFO
+drwxr-xr-x   0 hongyan   (1000) hongyan   (1000)        0 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/Privacy_Meter.egg-info/
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     9586 2023-07-28 14:17:26.000000 Privacy-Meter-1.0.1/Privacy_Meter.egg-info/PKG-INFO
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)      630 2023-07-28 14:17:26.000000 Privacy-Meter-1.0.1/Privacy_Meter.egg-info/SOURCES.txt
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)        1 2023-07-28 14:17:26.000000 Privacy-Meter-1.0.1/Privacy_Meter.egg-info/dependency_links.txt
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)       14 2023-07-28 14:17:26.000000 Privacy-Meter-1.0.1/Privacy_Meter.egg-info/top_level.txt
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     9045 2023-07-28 14:12:19.000000 Privacy-Meter-1.0.1/README.md
+drwxr-xr-x   0 hongyan   (1000) hongyan   (1000)        0 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/privacy_meter/
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)        0 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/__init__.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     8134 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/audit.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)    32319 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/audit_report.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     2174 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/constants.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     9744 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/dataset.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     7614 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/hypothesis_test.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     3778 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/information_source.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)    19533 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/information_source_signal.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)    41756 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/metric.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     5190 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/metric_result.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)    30625 2023-07-28 14:12:19.000000 Privacy-Meter-1.0.1/privacy_meter/model.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)      735 2023-07-18 04:28:24.000000 Privacy-Meter-1.0.1/privacy_meter/utils.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)      227 2023-02-20 02:58:35.000000 Privacy-Meter-1.0.1/requirements.txt
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)       38 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/setup.cfg
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     1232 2023-07-28 14:17:22.000000 Privacy-Meter-1.0.1/setup.py
+drwxr-xr-x   0 hongyan   (1000) hongyan   (1000)        0 2023-07-28 14:17:26.578693 Privacy-Meter-1.0.1/tests/
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     1153 2023-02-21 08:20:14.000000 Privacy-Meter-1.0.1/tests/test_datasets.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)      380 2023-02-21 08:20:11.000000 Privacy-Meter-1.0.1/tests/test_models.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     2918 2023-07-28 14:12:19.000000 Privacy-Meter-1.0.1/tests/test_train.py
+-rw-r--r--   0 hongyan   (1000) hongyan   (1000)     4819 2023-02-21 08:20:21.000000 Privacy-Meter-1.0.1/tests/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `privacy_meter-1.0/LICENSE` & `Privacy-Meter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `privacy_meter-1.0/privacy_meter/audit_report.py` & `Privacy-Meter-1.0.1/privacy_meter/audit_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,101 @@
 import os
 import subprocess
 from abc import ABC, abstractmethod
-from typing import List, Union, Tuple, Dict
-import json
+from datetime import date
+from typing import Dict, List, Tuple, Union
 
 import jinja2
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sn
-import matplotlib.pyplot as plt
-from datetime import date
 from PIL import Image
 from scipy import interpolate
 
 from privacy_meter.constants import InferenceGame
 from privacy_meter.information_source import InformationSource
 from privacy_meter.information_source_signal import DatasetSample
-from privacy_meter.metric_result import MetricResult
-
+from privacy_meter.metric_result import CombinedMetricResult, MetricResult
 
 ########################################################################################################################
 # GLOBAL SETTINGS
 ########################################################################################################################
 
 # Temporary parameter pointing to the report_file directory (for compatibility)
 REPORT_FILES_DIR = "report_files"
 
 # Configure jinja for LaTex
 latex_jinja_env = jinja2.Environment(
-    block_start_string='\BLOCK{',
-    block_end_string='}',
-    variable_start_string='\VAR{',
-    variable_end_string='}',
-    comment_start_string='\#{',
-    comment_end_string='}',
-    line_statement_prefix='%%',
-    line_comment_prefix='%#',
+    block_start_string="\BLOCK{",
+    block_end_string="}",
+    variable_start_string="\VAR{",
+    variable_end_string="}",
+    comment_start_string="\#{",
+    comment_end_string="}",
+    line_statement_prefix="%%",
+    line_comment_prefix="%#",
     trim_blocks=True,
     autoescape=False,
-    loader=jinja2.FileSystemLoader(os.path.abspath('.'))
+    loader=jinja2.FileSystemLoader(os.path.abspath(".")),
 )
 
+# Config the name for metric id.
+EXPLANATIONS = {
+    "metric": {
+        "shadow_metric": {
+            "name": "Shadow metric",
+            "details": "The shadow metric is a membership inference metric, that uses the algorithm described in \\cite{https://doi.org/10.48550/arxiv.1610.05820}",
+        },
+        "population_metric": {
+            "name": "Population metric",
+            "details": "[TODO] Add details in explanations.json (you can also edit citations.bib).",
+        },
+        "reference_metric": {
+            "name": "Reference metric",
+            "details": "[TODO] Add details in explanations.json (you can also edit citations.bib).",
+        },
+    },
+    "figure": {
+        "roc_curve": {
+            "name": "ROC curve",
+            "details": "shows the ROC (Receiver Operating Characteristic) curve, a graph illustrating the performance of a classification model at various decision thresholds. The AUC (Area Under the Curve), represented in blue, is a threshold-independant measure of the classifier performance.\n\nA higher AUC is an indicator of a system vulnerable to the chosen metric. For reference, a random classifier yields an AUC of 0.5, while a perfect classifier yields an AUC of 1.0",
+        },
+        "confusion_matrix": {
+            "name": "Confusion matrix",
+            "details": "shows the confusion matrix, a graph illustrating the performance of a classification model for a specific decision threshold.\n\nHigher values on the top-left to bottom-right diagonal is an indicator of a system vulnerable to the chosen metric, while higher values on the top-right to bottom-left diagonal is an indicator of a system less vulnerable to the chosen metric.",
+        },
+        "signal_histogram": {
+            "name": "Signal histogram",
+            "details": "shows the histogram of the signal used by the chosen metric, on both members and non-member samples.\n\nA clear separation between the two groups is an indicator of a system vulnerable to the chosen metric.",
+        },
+        "vulnerable_points": {
+            "name": "Vulnerable points",
+            "details": "shows points that are most vulnerable to the chosen metric.\n\nThe score depends on the chosen metric, but is always between 0 and 1, with 0 meaning low vulnerability and 1 high vulnerability.",
+        },
+    },
+}
+
 ########################################################################################################################
 # AUDIT_REPORT CLASS
 ########################################################################################################################
 
 
 class AuditReport(ABC):
     """
     An abstract class to display and/or save some elements of a metric result object.
     """
 
     @staticmethod
     @abstractmethod
     def generate_report(
-            metric_result: Union[MetricResult, List[MetricResult], dict],
-            inference_game_type: InferenceGame
+        metric_result: Union[
+            MetricResult, List[MetricResult], dict, CombinedMetricResult
+        ],
+        inference_game_type: InferenceGame,
     ):
         """
         Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_result: MetricResult object, containing data for the report.
             inference_game_type: Value from the InferenceGame ENUM type, indicating which inference game was used.
@@ -76,120 +112,179 @@
     """
     Inherits from the AuditReport class, an interface class to display and/or save some elements of a metric result
     object. This particular class is used to generate a ROC (Receiver Operating Characteristic) curve.
     """
 
     @staticmethod
     def __avg_roc(
-            fpr_2d_list: List[List[float]],
-            tpr_2d_list: List[List[float]],
-            n: int = 200
+        fpr_2d_list: List[List[float]], tpr_2d_list: List[List[float]], n: int = 200
     ) -> Tuple[np.ndarray, np.ndarray]:
         """
         Private helper function, to average a ROC curve from non-aligned list.
 
         Args:
             fpr_2d_list: A 2D list of fpr values.
             tpr_2d_list: A 2D list of fpr values.
             n: Number of points in the resulting lists.
 
         Returns:
             A tuple of aligned 1D numpy arrays, fpr and tpr.
         """
-        functions = [interpolate.interp1d(fpr, tpr) for (fpr, tpr) in zip(fpr_2d_list, tpr_2d_list)]
+        functions = [
+            interpolate.interp1d(fpr, tpr)
+            for (fpr, tpr) in zip(fpr_2d_list, tpr_2d_list)
+        ]
         fpr = np.linspace(0, 1, n)
         tpr = np.mean([f(fpr) for f in functions], axis=0)
         return fpr, tpr
 
     @staticmethod
     def generate_report(
-            metric_result: Union[MetricResult, List[MetricResult], List[List[MetricResult]]],
-            inference_game_type: InferenceGame,
-            show: bool = False,
-            save: bool = True,
-            filename: str = 'roc_curve.jpg'
+        metric_result: Union[
+            MetricResult,
+            List[MetricResult],
+            List[List[MetricResult]],
+            CombinedMetricResult,
+        ],
+        inference_game_type: InferenceGame,
+        show: bool = False,
+        save: bool = True,
+        filename: str = "roc_curve.jpg",
     ):
         """
         Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_result: A list of MetricResult objects, containing data for the report.
             inference_game_type: Value from the InferenceGame ENUM type, indicating which inference game was used.
             show: Boolean specifying if the plot should be displayed on screen.
             save: Boolean specifying if the plot should be saved as a file.
             filename: File name to be used if the plot is saved as a file.
         """
 
-        # Casts type to a 2D list
+        # Check if it is the combined report:
         if not isinstance(metric_result, list):
             metric_result = [metric_result]
-        if not isinstance(metric_result[0], list):
-            metric_result = [metric_result]
-
-        # Read and store the explanation dict
-        with open(f'{REPORT_FILES_DIR}/explanations.json', 'r') as f:
-            explanations = json.load(f)
-
-        # Computes fpr, tpr and auc in different ways, depending on the available information and inference game
-        if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
-            if metric_result[0][0].predictions_proba is None:
-                fpr = [mr.fp / (mr.fp + mr.tn) for mr in metric_result[0]]
-                tpr = [mr.tp / (mr.tp + mr.fn) for mr in metric_result[0]]
-                roc_auc = np.trapz(x=fpr, y=tpr)
-            else:
-                fpr, tpr, _ = metric_result[0][0].roc
-                roc_auc = metric_result[0][0].roc_auc
-        elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
-            if metric_result[0][0].predictions_proba is None:
-                fpr = [[metric_result[i][j].fp / (metric_result[i][j].fp + metric_result[i][j].tn) for j in range(len(metric_result[0]))] for i in range(len(metric_result))]
-                tpr = [[metric_result[i][j].tp / (metric_result[i][j].tp + metric_result[i][j].fn) for j in range(len(metric_result[0]))] for i in range(len(metric_result))]
-                fpr = np.mean(fpr, axis=0)
-                tpr = np.mean(tpr, axis=0)
-                roc_auc = np.trapz(x=fpr, y=tpr)
+        if not isinstance(metric_result[0], CombinedMetricResult) and not isinstance(
+            metric_result[0][0], CombinedMetricResult
+        ):
+            # Casts type to a 2D list
+            if not isinstance(metric_result[0], list):
+                metric_result = [metric_result]
+            # Computes fpr, tpr and auc in different ways, depending on the available information and inference game
+            if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
+                if metric_result[0][0].predictions_proba is None:
+                    fpr = [mr.fp / (mr.fp + mr.tn) for mr in metric_result[0]]
+                    tpr = [mr.tp / (mr.tp + mr.fn) for mr in metric_result[0]]
+                    roc_auc = np.trapz(x=fpr, y=tpr)
+                else:
+                    fpr, tpr, _ = metric_result[0][0].roc
+                    roc_auc = metric_result[0][0].roc_auc
+            elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
+                if metric_result[0][0].predictions_proba is None:
+                    fpr = [
+                        [
+                            metric_result[i][j].fp
+                            / (metric_result[i][j].fp + metric_result[i][j].tn)
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                    tpr = [
+                        [
+                            metric_result[i][j].tp
+                            / (metric_result[i][j].tp + metric_result[i][j].fn)
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                    fpr = np.mean(fpr, axis=0)
+                    tpr = np.mean(tpr, axis=0)
+                    roc_auc = np.trapz(x=fpr, y=tpr)
+                else:
+                    fpr, tpr = ROCCurveReport.__avg_roc(
+                        fpr_2d_list=[
+                            metric_result[i][0].roc[0]
+                            for i in range(len(metric_result))
+                        ],
+                        tpr_2d_list=[
+                            metric_result[i][0].roc[1]
+                            for i in range(len(metric_result))
+                        ],
+                    )
+                    roc_auc = np.trapz(x=fpr, y=tpr)
             else:
-                fpr, tpr = ROCCurveReport.__avg_roc(
-                    fpr_2d_list=[metric_result[i][0].roc[0] for i in range(len(metric_result))],
-                    tpr_2d_list=[metric_result[i][0].roc[1] for i in range(len(metric_result))]
-                )
-                roc_auc = np.trapz(x=fpr, y=tpr)
+                raise NotImplementedError
         else:
-            raise NotImplementedError
+            # Generate report for the combined report
+            # Computes fpr, tpr and auc in different ways, depending on the available information and inference game
+            if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
+                if metric_result[0].predictions_proba is None:
+                    mr = metric_result[0]
+                    fpr = mr.fp / (mr.fp + mr.tn)
+                    tpr = mr.tp / (mr.tp + mr.fn)
+                    roc_auc = np.trapz(x=fpr, y=tpr)
+            elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
+                if metric_result[0][0].predictions_proba is None:
+                    fpr = [
+                        [
+                            metric_result[i][j].fp
+                            / (metric_result[i][j].fp + metric_result[i][j].tn)
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                    tpr = [
+                        [
+                            metric_result[i][j].tp
+                            / (metric_result[i][j].tp + metric_result[i][j].fn)
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                    fpr = np.mean(fpr, axis=0).ravel()
+                    tpr = np.mean(tpr, axis=0).ravel()
+                    roc_auc = np.trapz(x=fpr, y=tpr)
+            else:
+                raise NotImplementedError
 
         # Gets metric ID
         if isinstance(metric_result, list):
             if isinstance(metric_result[0], list):
                 metric_id = metric_result[0][0].metric_id
             else:
                 metric_id = metric_result[0].metric_id
         else:
             metric_id = metric_result.metric_id
 
         # Generate plot
         range01 = np.linspace(0, 1)
         plt.fill_between(fpr, tpr, alpha=0.15)
-        plt.plot(fpr, tpr, label=explanations["metric"][metric_id]["name"])
-        plt.plot(range01, range01, '--', label='Random guess')
+        plt.plot(fpr, tpr, label=EXPLANATIONS["metric"][metric_id]["name"])
+        plt.plot(range01, range01, "--", label="Random guess")
         plt.xlim([0, 1])
         plt.ylim([0, 1])
         plt.grid()
         plt.legend()
-        plt.xlabel('False positive rate (FPR)')
-        plt.ylabel('True positive rate (TPR)')
-        plt.title('ROC curve')
+        plt.xlabel("False positive rate (FPR)")
+        plt.ylabel("True positive rate (TPR)")
+        plt.title("ROC curve")
         plt.text(
-            0.7, 0.3,
-            f'AUC = {roc_auc:.03f}',
-            horizontalalignment='center',
-            verticalalignment='center',
-            bbox=dict(facecolor='white', alpha=0.5)
+            0.7,
+            0.3,
+            f"AUC = {roc_auc:.03f}",
+            horizontalalignment="center",
+            verticalalignment="center",
+            bbox=dict(facecolor="white", alpha=0.5),
         )
         if save:
             plt.savefig(fname=filename, dpi=1000)
         if show:
             plt.show()
+        print(f"AUC = {roc_auc:.03f}")
         plt.clf()
 
 
 ########################################################################################################################
 # CONFUSION_MATRIX_REPORT CLASS
 ########################################################################################################################
 
@@ -198,47 +293,54 @@
     """
     Inherits from the AuditReport class, an interface class to display and/or save some elements of a metric result
     object. This particular class is used to generate a confusion matrix.
     """
 
     @staticmethod
     def generate_report(
-            metric_result: Union[MetricResult, List[MetricResult]],
-            inference_game_type: InferenceGame,
-            show: bool = False,
-            save: bool = True,
-            filename: str = 'confusion_matrix.jpg'
+        metric_result: Union[MetricResult, List[MetricResult]],
+        inference_game_type: InferenceGame,
+        show: bool = False,
+        save: bool = True,
+        filename: str = "confusion_matrix.jpg",
     ):
         """
         Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_result: MetricResult object, containing data for the report.
             inference_game_type: Value from the InferenceGame ENUM type, indicating which inference game was used.
             show: Boolean specifying if the plot should be displayed on screen.
             save: Boolean specifying if the plot should be saved as a file.
             filename: File name to be used if the plot is saved as a file.
         """
 
         if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
             assert isinstance(metric_result, MetricResult)
-            cm = np.array([[metric_result.tn, metric_result.fp], [metric_result.fn, metric_result.tp]])
+            cm = np.array(
+                [
+                    [metric_result.tn, metric_result.fp],
+                    [metric_result.fn, metric_result.tp],
+                ]
+            )
         elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
             assert isinstance(metric_result, list)
-            cm = np.mean([[[mr.tn, mr.fp], [mr.fn, mr.tp]] for mr in metric_result], axis=0)
+            cm = np.mean(
+                [[[mr.tn, mr.fp], [mr.fn, mr.tp]] for mr in metric_result], axis=0
+            )
         else:
             raise NotImplementedError
 
         cm = 100 * cm / np.sum(cm)
         index = ["Non-member", "Member"]
         df_cm = pd.DataFrame(cm, index, index)
         sn.heatmap(df_cm, annot=True, cmap=plt.cm.Blues)
-        plt.xlabel('Predicted label')
-        plt.ylabel('True label')
-        plt.title('Confusion matrix (in %)')
+        plt.xlabel("Predicted label")
+        plt.ylabel("True label")
+        plt.title("Confusion matrix (in %)")
         if save:
             plt.savefig(fname=filename, dpi=1000)
         if show:
             plt.show()
         plt.clf()
 
 
@@ -251,19 +353,19 @@
     """
     Inherits from the AuditReport class, an interface class to display and/or save some elements of a metric result
     object. This particular class is used to generate a histogram of the signal values.
     """
 
     @staticmethod
     def generate_report(
-            metric_result: Union[MetricResult, List[MetricResult]],
-            inference_game_type: InferenceGame,
-            show: bool = False,
-            save: bool = True,
-            filename: str = 'signal_histogram.jpg'
+        metric_result: Union[MetricResult, List[MetricResult]],
+        inference_game_type: InferenceGame,
+        show: bool = False,
+        save: bool = True,
+        filename: str = "signal_histogram.jpg",
     ):
         """
         Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_result: MetricResult object, containing data for the report.
             inference_game_type: Value from the InferenceGame ENUM type, indicating which inference game was used.
@@ -273,51 +375,78 @@
         """
 
         if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
             values = np.array(metric_result.signal_values).ravel()
             labels = np.array(metric_result.true_labels).ravel()
             threshold = metric_result.threshold
         elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
-            values = np.concatenate([mr.signal_values for mr in metric_result]).ravel()
-            labels = np.concatenate([mr.true_labels for mr in metric_result]).ravel()
-            threshold_list = [mr.threshold for mr in metric_result]
-            threshold = None if None in threshold_list else np.mean(threshold_list)
+            if not isinstance(metric_result[0], list):
+                values = np.concatenate(
+                    [mr.signal_values for mr in metric_result]
+                ).ravel()
+                labels = np.concatenate(
+                    [mr.true_labels for mr in metric_result]
+                ).ravel()
+                threshold_list = [mr.threshold for mr in metric_result]
+                threshold = None if None in threshold_list else np.mean(threshold_list)
+            else:
+                values = np.array(
+                    [
+                        [
+                            metric_result[i][j].signal_values
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                ).ravel()
+                labels = np.array(
+                    [
+                        [
+                            metric_result[i][j].true_labels
+                            for j in range(len(metric_result[0]))
+                        ]
+                        for i in range(len(metric_result))
+                    ]
+                ).ravel()
+                threshold_list = None
+                threshold = None
+
         else:
             raise NotImplementedError
 
         histogram = sn.histplot(
-            data=pd.DataFrame({
-                'Signal': values,
-                'Membership': ['Member' if y == 1 else 'Non-member' for y in labels]
-            }),
-            x='Signal',
-            hue='Membership',
-            element='step',
-            kde=True
+            data=pd.DataFrame(
+                {
+                    "Signal": values,
+                    "Membership": [
+                        "Member" if y == 1 else "Non-member" for y in labels
+                    ],
+                }
+            ),
+            x="Signal",
+            hue="Membership",
+            element="step",
+            kde=True,
         )
 
-        if threshold is not None:
-            histogram.axvline(
-                x=threshold,
-                linestyle='--',
-                color="C{}".format(2)
-            )
+        if threshold is not None and type(threshold) == float:
+            histogram.axvline(x=threshold, linestyle="--", color="C{}".format(2))
             histogram.text(
-                x=threshold - (np.max(values) - np.min(values))/30,
-                y=.8,
-                s='Threshold',
+                x=threshold - (np.max(values) - np.min(values)) / 30,
+                y=0.8,
+                s="Threshold",
                 rotation=90,
                 color="C{}".format(2),
-                transform=histogram.get_xaxis_transform()
+                transform=histogram.get_xaxis_transform(),
             )
 
         plt.grid()
-        plt.xlabel('Signal value')
-        plt.ylabel('Number of samples')
-        plt.title('Signal histogram')
+        plt.xlabel("Signal value")
+        plt.ylabel("Number of samples")
+        plt.title("Signal histogram")
         if save:
             plt.savefig(fname=filename, dpi=1000)
         if show:
             plt.show()
         plt.clf()
 
 
@@ -330,23 +459,23 @@
     """
     Inherits from the AuditReport class, an interface class to display and/or save some elements of a metric result
     object. This particular class is used to identify the most vulnerable points.
     """
 
     @staticmethod
     def generate_report(
-            metric_results: List[MetricResult],
-            inference_game_type: InferenceGame,
-            target_info_source: InformationSource,
-            target_model_to_train_split_mapping: List[Tuple[int, str, str, str]],
-            number_of_points: int = 10,
-            save_tex: bool = False,
-            filename: str = 'vulnerable_points.tex',
-            return_raw_values: bool = True,
-            point_type: str = 'any'
+        metric_results: List[MetricResult],
+        inference_game_type: InferenceGame,
+        target_info_source: InformationSource,
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]],
+        number_of_points: int = 10,
+        save_tex: bool = False,
+        filename: str = "vulnerable_points.tex",
+        return_raw_values: bool = True,
+        point_type: str = "any",
     ):
         """Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_results: A dict of lists of MetricResult objects, containing data for the report.
             target_info_source: The InformationSource associated with the audited model training.
             target_model_to_train_split_mapping: The mapping associated with target_info_source.
@@ -371,41 +500,37 @@
 
         # If only one metric was used (i.e. we have access to the prediction probabilities)
         if len(metric_results) == 1:
             mr = metric_results[0]
             # Sort the training points that were identified as such by their prediction probabilities
             adjusted_values = np.where(
                 (np.array(mr.predicted_labels) == np.array(mr.true_labels))
-                &
-                (np.array(mr.true_labels) == 1)
-                ,
-                - mr.predictions_proba
-                ,
-                10
+                & (np.array(mr.true_labels) == 1),
+                -mr.predictions_proba,
+                10,
             )
             indices = np.argsort(adjusted_values)[:number_of_points]
             # Get the associated scores
             scores = mr.predictions_proba[indices]
 
         # If multiple metrics were used (i.e. we don't have access to the prediction probabilities)
         else:
             # Use the various metric, from the one with lowest fpr to the one with highest fpr
             fp_indices = np.argsort([mr.fp for mr in metric_results])
             for k in range(len(metric_results)):
                 mr = metric_results[fp_indices[k]]
                 # Get the training points that were identified as such
                 new_indices = np.argwhere(
                     (np.array(mr.predicted_labels) == np.array(mr.true_labels))
-                    &
-                    (np.array(mr.true_labels) == 1)
+                    & (np.array(mr.true_labels) == 1)
                 )
                 indices.extend(list(new_indices.ravel()))
                 # Get the associated scores
                 fpr = mr.fp / (mr.fp + mr.tn)
-                scores.extend([1-fpr] * new_indices.shape[0])
+                scores.extend([1 - fpr] * new_indices.shape[0])
             # Only keep number_of_points points
             indices, scores = indices[:number_of_points], scores[:number_of_points]
 
         # Map indices stored in the metric_result object to indices in the training set
         indices_to_train_indices = []
         counter = 0
         for k, v in enumerate(metric_results[0].true_labels):
@@ -416,36 +541,40 @@
         # If points are images and we are creating a LaTex file, then we read the information source to create image
         # files from the vulnerable
         if save_tex and point_type == "image":
             for k, point in enumerate(indices):
                 x = target_info_source.get_signal(
                     signal=DatasetSample(),
                     model_to_split_mapping=target_model_to_train_split_mapping,
-                    extra={"model_num": 0, "point_num": point}
+                    extra={"model_num": 0, "point_num": point},
                 )
-                Image.fromarray((x*255).astype('uint8')).save(f'point{k:03d}.jpg')
+                Image.fromarray((x * 255).astype("uint8")).save(f"point{k:03d}.jpg")
 
         # If we are creating a LaTex
         if save_tex:
-
             # Load template
-            template = latex_jinja_env.get_template(f'{REPORT_FILES_DIR}/vulnerable_points_template.tex')
+            template = latex_jinja_env.get_template(
+                f"{REPORT_FILES_DIR}/vulnerable_points_template.tex"
+            )
 
             # Render the template (i.e. generate the corresponding string)
             latex_content = template.render(
-                points=[{
-                    "index": index,
-                    "score": f'{score:.3f}',
-                    "type": point_type,
-                    "path": f"point{k:03d}.jpg" if point_type == "image" else None
-                } for (k, (index, score)) in enumerate(zip(indices, scores))]
+                points=[
+                    {
+                        "index": index,
+                        "score": f"{score:.3f}",
+                        "type": point_type,
+                        "path": f"point{k:03d}.jpg" if point_type == "image" else None,
+                    }
+                    for (k, (index, score)) in enumerate(zip(indices, scores))
+                ]
             )
 
             # Write the result (the string) to a .tex file
-            with open(filename, 'w') as f:
+            with open(filename, "w") as f:
                 f.write(latex_content)
 
         # If we required the values to be returned
         if return_raw_values:
             return indices, scores
 
 
@@ -458,25 +587,27 @@
     """
     Inherits from the AuditReport class, an interface class to display and/or save some elements of a metric result
     object. This particular class is used to generate a user-friendly report, with multiple plots and some explanations.
     """
 
     @staticmethod
     def generate_report(
-            metric_results: Dict[str, Union[MetricResult, List[MetricResult], List[List[MetricResult]]]],
-            inference_game_type: InferenceGame,
-            figures_dict: dict,
-            system_name: str,
-            call_pdflatex: bool = True,
-            show: bool = False,
-            save: bool = True,
-            filename_no_extension: str = 'report',
-            target_info_source: InformationSource = None,
-            target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            point_type: str = 'any'
+        metric_results: Dict[
+            str, Union[MetricResult, List[MetricResult], List[List[MetricResult]]]
+        ],
+        inference_game_type: InferenceGame,
+        figures_dict: dict,
+        system_name: str,
+        call_pdflatex: bool = True,
+        show: bool = False,
+        save: bool = True,
+        filename_no_extension: str = "report",
+        target_info_source: InformationSource = None,
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        point_type: str = "any",
     ):
         """
         Core function of the AuditReport class that actually generates the report.
 
         Args:
             metric_results: A dict of lists of MetricResult objects, containing data for the report.
             inference_game_type: Value from the InferenceGame ENUM type, indicating which inference game was used.
@@ -492,118 +623,129 @@
 
         for metric in metric_results:
             if not isinstance(metric_results[metric], list):
                 metric_results[metric] = [metric_results[metric]]
             if not isinstance(metric_results[metric][0], list):
                 metric_results[metric] = [[mr] for mr in metric_results[metric]]
 
-        # Read and store the explanation dict
-        with open(f'{REPORT_FILES_DIR}/explanations.json', 'r') as f:
-            explanations = json.load(f)
-
         # Generate all plots, and save their filenames
         files_dict = {}
         for metric in metric_results:
             files_dict[metric] = {}
             result = metric_results[metric]
 
             # Select one instance to display when necessary (e.g. for a confusion matrix with a PopulationMetric)
             if inference_game_type == InferenceGame.PRIVACY_LOSS_MODEL:
                 best_index = np.argmax([r.accuracy for r in result])
                 best_result = result[best_index]
             elif inference_game_type == InferenceGame.AVG_PRIVACY_LOSS_TRAINING_ALGO:
-                best_indices = np.argmax([[r2.accuracy for r2 in r1] for r1 in result], axis=1)
-                best_result = [result[k][best_index] for k, best_index in enumerate(best_indices)]
+                best_indices = np.argmax(
+                    [[r2.accuracy for r2 in r1] for r1 in result], axis=1
+                )
+                best_result = [
+                    result[k][best_index] for k, best_index in enumerate(best_indices)
+                ]
             else:
                 raise NotImplementedError
 
-            if 'roc_curve' in figures_dict[metric]:
-                figure = 'roc_curve'
-                filename = f'{metric}_{figure}.jpg'
+            if "roc_curve" in figures_dict[metric]:
+                figure = "roc_curve"
+                filename = f"{metric}_{figure}.jpg"
                 files_dict[metric][figure] = filename
                 ROCCurveReport.generate_report(
                     metric_result=result,
                     inference_game_type=inference_game_type,
-                    filename=filename
+                    filename=filename,
                 )
-            if 'confusion_matrix' in figures_dict[metric]:
-                figure = 'confusion_matrix'
-                filename = f'{metric}_{figure}.jpg'
+            if "confusion_matrix" in figures_dict[metric]:
+                figure = "confusion_matrix"
+                filename = f"{metric}_{figure}.jpg"
                 files_dict[metric][figure] = filename
                 ConfusionMatrixReport.generate_report(
                     metric_result=best_result,
                     inference_game_type=inference_game_type,
-                    filename=filename
+                    filename=filename,
                 )
-            if 'signal_histogram' in figures_dict[metric]:
-                figure = 'signal_histogram'
-                filename = f'{metric}_{figure}.jpg'
+            if "signal_histogram" in figures_dict[metric]:
+                figure = "signal_histogram"
+                filename = f"{metric}_{figure}.jpg"
                 files_dict[metric][figure] = filename
                 SignalHistogramReport.generate_report(
                     metric_result=best_result,
                     inference_game_type=inference_game_type,
-                    filename=filename
+                    filename=filename,
                 )
-            if 'vulnerable_points' in figures_dict[metric]:
+            if "vulnerable_points" in figures_dict[metric]:
                 assert target_info_source is not None
                 assert target_model_to_train_split_mapping is not None
-                figure = 'vulnerable_points'
-                filename = f'{metric}_{figure}.tex'
+                figure = "vulnerable_points"
+                filename = f"{metric}_{figure}.tex"
                 files_dict[metric][figure] = filename
                 VulnerablePointsReport.generate_report(
                     metric_results=result,
                     inference_game_type=inference_game_type,
                     save_tex=True,
                     filename=filename,
                     target_info_source=target_info_source,
                     target_model_to_train_split_mapping=target_model_to_train_split_mapping,
-                    point_type=point_type
+                    point_type=point_type,
                 )
 
         # Load template
-        template = latex_jinja_env.get_template(f'{REPORT_FILES_DIR}/report_template.tex')
+        template = latex_jinja_env.get_template(
+            f"{REPORT_FILES_DIR}/report_template.tex"
+        )
 
         # Render the template (i.e. generate the corresponding string)
         latex_content = template.render(
-            bib_file=os.path.abspath(f'{REPORT_FILES_DIR}/citations.bib'),
-            image_folder=os.path.abspath('.'),
+            bib_file=os.path.abspath(f"{REPORT_FILES_DIR}/citations.bib"),
+            image_folder=os.path.abspath("."),
             name=system_name,
-            tool_version='1.0',
+            tool_version="1.0",
             report_date=date.today().strftime("%b-%d-%Y"),
-            explanations=explanations,
+            explanations=EXPLANATIONS,
             figures_dict=figures_dict,
             files_dict=files_dict,
-            inference_game_type=inference_game_type.value
+            inference_game_type=inference_game_type.value,
         )
 
         # Write the result (the string) to a .tex file
-        with open(f'{filename_no_extension}.tex', 'w') as f:
+        with open(f"{filename_no_extension}.tex", "w") as f:
             f.write(latex_content)
 
         print(f'LaTex file created:\t{os.path.abspath(f"{filename_no_extension}.tex")}')
 
         if call_pdflatex:
-
             # Compile the .tex file to a .pdf file. Several rounds are required to get the references (to papers, to
             # page numbers, and to figure numbers)
 
-            process = subprocess.Popen(['pdflatex', os.path.abspath(f'{filename_no_extension}.tex')],
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE)
+            process = subprocess.Popen(
+                ["pdflatex", os.path.abspath(f"{filename_no_extension}.tex")],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             stdout, stderr = process.communicate()
 
-            process = subprocess.Popen(['biber', os.path.abspath(f'{filename_no_extension}')],
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE)
+            process = subprocess.Popen(
+                ["biber", os.path.abspath(f"{filename_no_extension}")],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             stdout, stderr = process.communicate()
 
-            process = subprocess.Popen(['pdflatex', os.path.abspath(f'{filename_no_extension}.tex')],
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE)
+            process = subprocess.Popen(
+                ["pdflatex", os.path.abspath(f"{filename_no_extension}.tex")],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             stdout, stderr = process.communicate()
 
-            process = subprocess.Popen(['pdflatex', os.path.abspath(f'{filename_no_extension}.tex')],
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE)
+            process = subprocess.Popen(
+                ["pdflatex", os.path.abspath(f"{filename_no_extension}.tex")],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
             stdout, stderr = process.communicate()
 
-            print(f'PDF file created:\t{os.path.abspath(f"{filename_no_extension}.pdf")}')
+            print(
+                f'PDF file created:\t{os.path.abspath(f"{filename_no_extension}.pdf")}'
+            )
```

### Comparing `privacy_meter-1.0/privacy_meter/information_source_signal.py` & `Privacy-Meter-1.0.1/privacy_meter/information_source_signal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from abc import ABC, abstractmethod
-
 from typing import List, Tuple
 
 import numpy as np
 
 from privacy_meter.dataset import Dataset
 from privacy_meter.model import Model
 
-
 ########################################################################################################################
 # SIGNAL CLASS
 ########################################################################################################################
 
 
 class Signal(ABC):
     """
     Abstract class, representing any type of signal that can be obtained from a Model and/or a Dataset.
     """
 
     @abstractmethod
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -54,20 +53,21 @@
 class DatasetSample(Signal):
     """
     Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
     Dataset.
     This particular class is used to get a given point from the Dataset.
     """
 
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -79,35 +79,44 @@
                 default_model_to_split_mapping argument.
             extra: Dictionary containing any additional parameter that should be passed to the signal object.
 
         Returns:
             The sample point from the dataset.
         """
 
-        dataset_index, split_name, input_feature, output_feature = model_to_split_mapping[extra["model_num"]]
-        x = datasets[dataset_index].get_feature(split_name, input_feature)[extra["point_num"]]
+        (
+            dataset_index,
+            split_name,
+            input_feature,
+            output_feature,
+        ) = model_to_split_mapping[extra["model_num"]]
+        x = datasets[dataset_index].get_feature(split_name, input_feature)[
+            extra["point_num"]
+        ]
         return x
 
+
 ########################################################################################################################
 # MODEL_LOGIT CLASS
 ########################################################################################################################
 
 
 class ModelLogits(Signal):
     """
     Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a Dataset.
     This particular class is used to get the output of a model.
     """
 
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -123,38 +132,103 @@
             The signal value.
         """
 
         results = []
         # Compute the signal for each model
         for k, model in enumerate(models):
             # Extract the features to be used
-            dataset_index, split_name, input_feature, output_feature = model_to_split_mapping[k]
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
             x = datasets[dataset_index].get_feature(split_name, input_feature)
             # Compute the signal
             results.append(model.get_logits(x))
         return results
 
+
+########################################################################################################################
+# MODEL_RESCALEDLOGIT CLASS
+########################################################################################################################
+
+
+class ModelNegativeRescaledLogits(Signal):
+    """
+    Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a Dataset.
+    This particular class is used to get the output of a model.
+    """
+
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
+        """Built-in call method.
+
+        Args:
+            models: List of models that can be queried.
+            datasets: List of datasets that can be queried.
+            model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
+                More specifically, for model #i:
+                model_to_split_mapping[i][0] contains the index of the dataset in the list,
+                model_to_split_mapping[i][1] contains the name of the split,
+                model_to_split_mapping[i][2] contains the name of the input feature,
+                model_to_split_mapping[i][3] contains the name of the output feature.
+                This can also be provided once and for all at the instantiation of InformationSource, through the
+                default_model_to_split_mapping argument.
+            extra: Dictionary containing any additional parameter that should be passed to the signal object.
+
+        Returns:
+            The signal value.
+        """
+
+        results = []
+        # Compute the signal for each model
+        for k, model in enumerate(models):
+            # Extract the features to be used
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
+            x = datasets[dataset_index].get_feature(split_name, input_feature)
+            # Check if output feature has been provided, else pass None
+            if output_feature is not None:
+                y = datasets[dataset_index].get_feature(split_name, output_feature)
+            else:
+                y = None
+
+            results.append(-model.get_rescaled_logits(x, y))
+        return results
+
+
 ########################################################################################################################
 # MODEL_INTERMEDIATE_OUTPUT CLASS
 ########################################################################################################################
 
 
 class ModelIntermediateOutput(Signal):
     """
     Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
     Dataset.
     This particular class is used to get the value of an intermediate layer of model.
     """
 
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -166,45 +240,52 @@
                 default_model_to_split_mapping argument.
             extra: Dictionary containing any additional parameter that should be passed to the signal object.
 
         Returns:
             The signal value.
         """
 
-        if 'layers' not in list(extra):
+        if "layers" not in list(extra):
             raise TypeError('extra parameter "layers" is required')
 
         results = []
         # Compute the signal for each model
         for k, model in enumerate(models):
             # Extract the features to be used
-            dataset_index, split_name, input_feature, output_feature = model_to_split_mapping[k]
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
             x = datasets[dataset_index].get_feature(split_name, input_feature)
             # Compute the signal
             results.append(model.get_intermediate_outputs(extra["layers"], x))
         return results
 
+
 ########################################################################################################################
 # MODEL_LOSS CLASS
 ########################################################################################################################
 
 
 class ModelLoss(Signal):
     """
     Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
     Dataset.
     This particular class is used to get the loss of a model.
     """
 
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -220,45 +301,52 @@
             The signal value.
         """
 
         results = []
         # Compute the signal for each model
         for k, model in enumerate(models):
             # Extract the features to be used
-            dataset_index, split_name, input_feature, output_feature = model_to_split_mapping[k]
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
             x = datasets[dataset_index].get_feature(split_name, input_feature)
 
             # Check if output feature has been provided, else pass None
             if output_feature is not None:
                 y = datasets[dataset_index].get_feature(split_name, output_feature)
             else:
                 y = None
 
             # Compute the signal for each sample
             results.append(model.get_loss(x, y))
         return results
 
+
 ########################################################################################################################
 # MODEL_GRADIENT CLASS
 ########################################################################################################################
 
 
 class ModelGradient(Signal):
     """
     Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
     Dataset.
     This particular class is used to get the gradient of a model.
     """
 
-    def __call__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 model_to_split_mapping: List[Tuple[int, str, str, str]],
-                 extra: dict
-                 ):
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
         """Built-in call method.
 
         Args:
             models: List of models that can be queried.
             datasets: List of datasets that can be queried.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -274,15 +362,112 @@
             The signal value.
         """
 
         results = []
         # Compute the signal for each model
         for k, model in enumerate(models):
             # Extract the features to be used
-            dataset_index, split_name, input_feature, output_feature = model_to_split_mapping[k]
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
             x = datasets[dataset_index].get_feature(split_name, input_feature)
             y = datasets[dataset_index].get_feature(split_name, output_feature)
-            # Compute the signal for each sample
-            for (sample_x, sample_y) in zip(x, y):
-                xx, yy = np.expand_dims(sample_x, axis=0), np.expand_dims(sample_y, axis=0)
-                results.append(model.get_grad(xx, yy))
+            results.append(model.get_grad(x, y))
+        return results
+
+
+########################################################################################################################
+# Group Information
+########################################################################################################################
+
+
+class GroupInfo(Signal):
+    """
+    Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
+    Dataset.
+    This particular class is used to get the group membership of data records.
+    """
+
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
+        """Built-in call method.
+
+        Args:
+            models: List of models that can be queried.
+            datasets: List of datasets that can be queried.
+            model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
+                More specifically, for model #i:
+                model_to_split_mapping[i][0] contains the index of the dataset in the list,
+                model_to_split_mapping[i][1] contains the name of the split,
+                model_to_split_mapping[i][2] contains the name of the group feature
+                This can also be provided once and for all at the instantiation of InformationSource, through the
+                default_model_to_split_mapping argument.
+            extra: Dictionary containing any additional parameter that should be passed to the signal object.
+
+        Returns:
+            The signal value.
+        """
+
+        results = []
+        # Given the group membership for each dataset used by each model
+        for k in range(len(models)):
+            dataset_index, split_name, group_feature = model_to_split_mapping[k]
+            g = datasets[dataset_index].get_feature(split_name, group_feature)
+            results.append(g)
+        return results
+
+
+class ModelGradientNorm(Signal):
+    """
+    Inherits from the Signal class, used to represent any type of signal that can be obtained from a Model and/or a
+    Dataset.
+    This particular class is used to get the gradient norm of a model.
+    """
+
+    def __call__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        model_to_split_mapping: List[Tuple[int, str, str, str]],
+        extra: dict,
+    ):
+        """Built-in call method.
+
+        Args:
+            models: List of models that can be queried.
+            datasets: List of datasets that can be queried.
+            model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
+                More specifically, for model #i:
+                model_to_split_mapping[i][0] contains the index of the dataset in the list,
+                model_to_split_mapping[i][1] contains the name of the split,
+                model_to_split_mapping[i][2] contains the name of the input feature,
+                model_to_split_mapping[i][3] contains the name of the output feature.
+                This can also be provided once and for all at the instantiation of InformationSource, through the
+                default_model_to_split_mapping argument.
+            extra: Dictionary containing any additional parameter that should be passed to the signal object.
+
+        Returns:
+            The signal value.
+        """
+
+        results = []
+        # Compute the signal for each model
+        for k, model in enumerate(models):
+            # Extract the features to be used
+            (
+                dataset_index,
+                split_name,
+                input_feature,
+                output_feature,
+            ) = model_to_split_mapping[k]
+            x = datasets[dataset_index].get_feature(split_name, input_feature)
+            y = datasets[dataset_index].get_feature(split_name, output_feature)
+            results.append(model.get_gradnorm(x, y))
         return results
```

### Comparing `privacy_meter-1.0/privacy_meter/audit.py` & `Privacy-Meter-1.0.1/privacy_meter/audit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import os
 from datetime import datetime
 from typing import List, Union
 
-from privacy_meter.constants import MetricEnum, InferenceGame
-from privacy_meter.hypothesis_test import threshold_func
+from privacy_meter.constants import InferenceGame, MetricEnum
+from privacy_meter.hypothesis_test import linear_itp_threshold_func
 from privacy_meter.information_source import InformationSource
 from privacy_meter.information_source_signal import ModelLoss
-from privacy_meter.metric import Metric, PopulationMetric, ShadowMetric, ReferenceMetric
+from privacy_meter.metric import (
+    GroupPopulationMetric,
+    Metric,
+    PopulationMetric,
+    ReferenceMetric,
+    ShadowMetric,
+)
 from privacy_meter.metric_result import MetricResult
 
 
 class Audit:
     """
     This class orchestrates how the Metric objects and the InformationSource objects interact with one
     another. The three steps of using this class are 1) initialization 2) audit.prepare() 3) audit.run().
     """
 
     def __init__(
-            self,
-            metrics: Union[Union[MetricEnum, Metric], List[Union[MetricEnum, Metric]]],
-            inference_game_type: InferenceGame,
-            target_info_sources: Union[InformationSource, List[InformationSource]] = None,
-            reference_info_sources: Union[InformationSource, List[InformationSource]] = None,
-            fpr_tolerances: Union[float, List[float]] = None,
-            logs_directory_names: Union[str, List[str]] = None
+        self,
+        metrics: Union[Union[MetricEnum, Metric], List[Union[MetricEnum, Metric]]],
+        inference_game_type: InferenceGame,
+        target_info_sources: Union[InformationSource, List[InformationSource]] = None,
+        reference_info_sources: Union[
+            InformationSource, List[InformationSource]
+        ] = None,
+        fpr_tolerances: Union[float, List[float]] = None,
+        logs_directory_names: Union[str, List[str]] = None,
+        save_logs: bool = True,
     ):
         """
         Constructor
 
         Args:
             metrics: Metric object or list of Metric objects to be used for the audit.
             inference_game_type: The type of inference game being played: average privacy loss of a training algorithm,
@@ -35,96 +44,123 @@
                 algorithm.
             target_info_sources: InformationSource object(s), containing the Model(s) that the metric will be performed
                 on, and the corresponding Dataset(s).
             reference_info_sources: InformationSource object(s), containing the Model(s) that the metric will be fitted
                 on, and the corresponding Dataset(s).
             fpr_tolerances: FPR tolerance value(s) to be used by the audit.
             logs_directory_names: Path(s) to logging directory(ies).
+            save_logs: Whether to save the signal(s).
         """
 
         self.metrics = metrics
         self.inference_game_type = inference_game_type
         self.target_info_sources = target_info_sources
         self.reference_info_sources = reference_info_sources
         self.fpr_tolerances = fpr_tolerances
         self.logs_directory_names = logs_directory_names
+        self.save_logs = save_logs
 
         self.__init_lists()
         self.__init_logs_directories()
         self.__init_metric_objects()
 
     def __init_logs_directories(self):
         """
         Private function part of the initialization process, to specify default logging directory(ies), and create them
         if necessary.
         """
-        if self.logs_directory_names is None:
+        if self.logs_directory_names is None and self.save_logs is True:
             self.logs_directory_names = []
             for i in range(len(self.metrics)):
                 logs_dirname = os.path.join(
                     os.getcwd(),
-                    datetime.now().strftime(f'log_%Y-%m-%d_%H-%M-%S-{i:03d}')
+                    datetime.now().strftime(f"log_%Y-%m-%d_%H-%M-%S-{i:03d}"),
                 )
                 os.mkdir(logs_dirname)
                 self.logs_directory_names.append(logs_dirname)
-        else:
+        elif self.save_logs:
             for path in self.logs_directory_names:
                 if not os.path.isdir(path):
                     os.mkdir(path)
+        else:
+            self.logs_directory_names = None
 
     def __init_metric_objects(self):
         """
         Private function part of the initialization process, to create Metric objects from MetricEnum ones.
         """
         self.metric_objects = []
         for k, metric in enumerate(self.metrics):
             if type(metric) == MetricEnum:
                 # If the user wants to use default versions of metrics
                 if metric == MetricEnum.POPULATION:
-                    self.metric_objects.append(PopulationMetric(
-                        target_info_source=self.target_info_sources[k],
-                        reference_info_source=self.reference_info_sources[k],
-                        signals=[ModelLoss()],
-                        hypothesis_test_func=threshold_func,
-                        logs_dirname=self.logs_directory_names[k]
-                    ))
+                    self.metric_objects.append(
+                        PopulationMetric(
+                            target_info_source=self.target_info_sources[k],
+                            reference_info_source=self.reference_info_sources[k],
+                            signals=[ModelLoss()],
+                            hypothesis_test_func=linear_itp_threshold_func,
+                            logs_dirname=self.logs_directory_names[k],
+                        )
+                    )
                 elif metric == MetricEnum.SHADOW:
-                    self.metric_objects.append(ShadowMetric(
-                        target_info_source=self.target_info_sources[k],
-                        reference_info_source=self.reference_info_sources[k],
-                        signals=[ModelLoss()],
-                        hypothesis_test_func=None,
-                        logs_dirname=self.logs_directory_names[k]
-                    ))
+                    self.metric_objects.append(
+                        ShadowMetric(
+                            target_info_source=self.target_info_sources[k],
+                            reference_info_source=self.reference_info_sources[k],
+                            signals=[ModelLoss()],
+                            hypothesis_test_func=None,
+                            logs_dirname=self.logs_directory_names[k],
+                        )
+                    )
                 elif metric == MetricEnum.REFERENCE:
-                    self.metric_objects.append(ReferenceMetric(
-                        target_info_source=self.target_info_sources[k],
-                        reference_info_source=self.reference_info_sources[k],
-                        signals=[ModelLoss()],
-                        hypothesis_test_func=threshold_func,
-                        logs_dirname=self.logs_directory_names[k]
-                    ))
+                    self.metric_objects.append(
+                        ReferenceMetric(
+                            target_info_source=self.target_info_sources[k],
+                            reference_info_source=self.reference_info_sources[k],
+                            signals=[ModelLoss()],
+                            hypothesis_test_func=linear_itp_threshold_func,
+                            logs_dirname=self.logs_directory_names[k],
+                        )
+                    )
+                elif metric == MetricEnum.GROUPPOPULATION:
+                    self.metric_objects.append(
+                        GroupPopulationMetric(
+                            target_info_source=self.target_info_sources[k],
+                            reference_info_source=self.reference_info_sources[k],
+                            signals=[ModelLoss()],
+                            hypothesis_test_func=linear_itp_threshold_func,
+                            logs_dirname=self.logs_directory_names[k],
+                        )
+                    )
+
             else:
                 # If the user wants to pass in their custom metric object
-                metric.logs_dirname = self.logs_directory_names[k]
+                if self.save_logs:
+                    metric.logs_dirname = self.logs_directory_names[k]
                 self.metric_objects.append(metric)
 
     def __init_lists(self):
         """
         Private function part of the initialization process, to have consistent argument types.
         """
         if not isinstance(self.metrics, list):
             self.metrics = [self.metrics]
         if not isinstance(self.target_info_sources, list):
             self.target_info_sources = [self.target_info_sources]
         if not isinstance(self.reference_info_sources, list):
             self.reference_info_sources = [self.reference_info_sources]
-        if not isinstance(self.fpr_tolerances, list):
+        if (
+            not isinstance(self.fpr_tolerances, list)
+            and self.fpr_tolerances is not None
+        ):
             self.fpr_tolerances = [self.fpr_tolerances]
-        if self.logs_directory_names is not None and not isinstance(self.logs_directory_names, list):
+        if self.logs_directory_names is not None and not isinstance(
+            self.logs_directory_names, list
+        ):
             self.logs_directory_names = [self.logs_directory_names]
 
     def prepare(self):
         """
         Core function that should be called after the initialization and before the audit.run() function. Runs the
         prepare_metric function of all metric objects, which computes (or loads from memory) the signals required for
         the membership inference algorithms.
@@ -137,8 +173,11 @@
         Core function that should be called after the audit.prepare() function. This actually runs the metrics'
         membership inference algorithms.
 
         Returns:
             A list of MetricResult objects (one per metric)
         """
         print(f"Results are stored in: {self.logs_directory_names}")
-        return [self.metric_objects[i].run_metric(self.fpr_tolerances) for i in range(len(self.metric_objects))]
+        return [
+            self.metric_objects[i].run_metric(self.fpr_tolerances)
+            for i in range(len(self.metric_objects))
+        ]
```

### Comparing `privacy_meter-1.0/privacy_meter/dataset.py` & `Privacy-Meter-1.0.1/privacy_meter/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from itertools import product
-from typing import Union, Dict
+from typing import Dict, Union
 
 import numpy as np
 
 ########################################################################################################################
 # DATASET CLASS
 ########################################################################################################################
 
 
 class Dataset:
     """
     Wrapper around a dictionary-like formatted dataset, with functions to run preprocessing, to define default
     input/output features, and to split a dataset easily.
     """
 
-    def __init__(self,
-                 data_dict: dict,
-                 default_input: str,
-                 default_output: str,
-                 preproc_fn_dict: dict = None,
-                 preprocessed: bool = False
-                 ):
+    def __init__(
+        self,
+        data_dict: dict,
+        default_input: str,
+        default_output: str,
+        default_group: str = None,
+        preproc_fn_dict: dict = None,
+        preprocessed: bool = False,
+    ):
         """Constructor
 
         Args:
             data_dict: Contains the dataset as a dict.
             default_input: The key of the data_dict that should be used by default to get the input of a model.
             default_output: The key of the data_dict that should be used by default to get the expected output
                 of a model.
+            default_group: The key of the data_dict that shouuld be used by default to get the group of the data points.
+                This is to contruct class dependent threshold.
             preproc_fn_dict: Contains optional preprocessing functions for each feature.
             preprocessed: Indicates if the preprocessing of preproc_fn_dict has already been applied.
         """
 
         # Store parameters
         self.data_dict = data_dict
         self.default_input = default_input
         self.default_output = default_output
+        self.default_group = default_group
         self.preproc_fn_dict = preproc_fn_dict
 
         # Store splits names and features names
         self.splits = list(self.data_dict)
         self.features = list(self.data_dict[self.splits[0]])
 
         # If preprocessing functions were passed as parameters, execute them
@@ -51,53 +56,51 @@
         Preprocessing function, executed by the constructor, based on the preproc_fn_dict attribute.
         """
         for (split, feature) in product(self.splits, self.features):
             if feature in list(self.preproc_fn_dict):
                 fn = self.preproc_fn_dict[feature]
                 self.data_dict[split][feature] = fn(self.data_dict[split][feature])
 
-    def get_feature(self,
-                    split_name: str,
-                    feature_name: str,
-                    indices: list = None
-                    ):
-
+    def get_feature(self, split_name: str, feature_name: str, indices: list = None):
         """Returns a specific feature from samples of a specific split.
 
         Args:
             split_name: Name of the split.
             feature_name: Name of the feature.
             indices: Optional list of indices. If not specified, the entire subset is returned.
 
         Returns:
             The requested feature, from samples of the requested split.
         """
 
         # Two placeholders can be used to trigger either the default input or the default output, as specified during
         # object creation
-        if feature_name == '<default_input>':
+        if feature_name == "<default_input>":
             feature_name = self.default_input
-        elif feature_name == '<default_output>':
+        elif feature_name == "<default_output>":
             feature_name = self.default_output
+        elif feature_name == "<default_group>":
+            feature_name = self.default_group
 
         # If 'indices' is not specified, returns the entire array. Else just return those indices
         if indices is None:
             return self.data_dict[split_name][feature_name]
         else:
             return self.data_dict[split_name][feature_name][indices]
 
-    def subdivide(self,
-                  num_splits: int,
-                  split_names: list = None,
-                  method: str = 'independent',
-                  split_size: Union[int, Dict[str, int]] = None,
-                  delete_original: bool = False,
-                  in_place: bool = True,
-                  return_results: bool = False
-                  ):
+    def subdivide(
+        self,
+        num_splits: int,
+        split_names: list = None,
+        method: str = "independent",
+        split_size: Union[int, Dict[str, int]] = None,
+        delete_original: bool = False,
+        in_place: bool = True,
+        return_results: bool = False,
+    ):
         """Subdivides the splits contained in split_names into sub-splits, e.g. for shadow model training.
 
         Args:
             num_splits: Number of sub-splits per original split.
             split_names: The splits to subdivide (e.g. train and test). By default, includes all splits.
             method: Either independent or random. If method is independent, then the sub-splits are a partition of the
                 original split (i.e. they contain the entire split without repetition). If method is random, then each
@@ -121,51 +124,72 @@
 
         # List of results if in_place is False
         new_datasets_dict = [{} for _ in range(num_splits)]
 
         for split in split_names:
 
             if split_size is not None:
-                parsed_split_size = split_size if isinstance(split_size, int) else split_size[split]
+                parsed_split_size = (
+                    split_size if isinstance(split_size, int) else split_size[split]
+                )
 
             # If method is random, then each sub-split is a random subset of the original split.
-            if method == 'random':
-                assert split_size is not None, 'Argument split_size is required when method is "random" or "hybrid"'
-                indices = np.random.randint(self.data_dict[split][self.features[0]].shape[0], size=(num_splits, parsed_split_size))
+            if method == "random":
+                assert (
+                    split_size is not None
+                ), 'Argument split_size is required when method is "random" or "hybrid"'
+                indices = np.random.randint(
+                    self.data_dict[split][self.features[0]].shape[0],
+                    size=(num_splits, parsed_split_size),
+                )
 
             # If method is independent, then the sub-splits are a partition of the original split.
-            elif method == 'independent':
+            elif method == "independent":
                 indices = np.arange(self.data_dict[split][self.features[0]].shape[0])
                 np.random.shuffle(indices)
                 indices = np.array_split(indices, num_splits)
 
             # If method is hybrid, then each sub-split is a random subset of the original split, with the guarantee that
             # the 1st one is not overlapping with the others
-            elif method == 'hybrid':
-                assert split_size is not None, 'Argument split_size is required when method is "random" or "hybrid"'
-                available_indices = np.arange(self.data_dict[split][self.features[0]].shape[0])
-                indices_a = np.random.choice(available_indices, size=(1, parsed_split_size), replace=False)
+            elif method == "hybrid":
+                assert (
+                    split_size is not None
+                ), 'Argument split_size is required when method is "random" or "hybrid"'
+                available_indices = np.arange(
+                    self.data_dict[split][self.features[0]].shape[0]
+                )
+                indices_a = np.random.choice(
+                    available_indices, size=(1, parsed_split_size), replace=False
+                )
                 available_indices = np.setdiff1d(available_indices, indices_a.flatten())
-                indices_b = np.random.choice(available_indices, size=(num_splits-1, parsed_split_size), replace=True)
+                indices_b = np.random.choice(
+                    available_indices,
+                    size=(num_splits - 1, parsed_split_size),
+                    replace=True,
+                )
                 indices = np.concatenate((indices_a, indices_b))
 
             else:
                 raise ValueError(f'Split method "{method}" does not exist.')
 
             for split_n in range(num_splits):
                 # Fill the dictionary if in_place is True
                 if in_place:
-                    self.data_dict[f'{split}{split_n:03d}'] = {}
+                    self.data_dict[f"{split}{split_n:03d}"] = {}
                     for feature in self.features:
-                        self.data_dict[f'{split}{split_n:03d}'][feature] = self.data_dict[split][feature][indices[split_n]]
+                        self.data_dict[f"{split}{split_n:03d}"][
+                            feature
+                        ] = self.data_dict[split][feature][indices[split_n]]
                 # Create new dictionaries if return_results is True
                 if return_results:
-                    new_datasets_dict[split_n][f'{split}'] = {}
+                    new_datasets_dict[split_n][f"{split}"] = {}
                     for feature in self.features:
-                        new_datasets_dict[split_n][f'{split}'][feature] = self.data_dict[split][feature][indices[split_n]]
+                        new_datasets_dict[split_n][f"{split}"][
+                            feature
+                        ] = self.data_dict[split][feature][indices[split_n]]
 
             # delete_original indicates if the original split should be deleted.
             if delete_original:
                 del self.data_dict[split]
 
         # Update the list of splits
         self.splits = list(self.data_dict)
@@ -173,25 +197,26 @@
         # Return new datasets if return_results is True
         if return_results:
             return [
                 Dataset(
                     data_dict=new_datasets_dict[i],
                     default_input=self.default_input,
                     default_output=self.default_output,
+                    default_group=self.default_group,
                     preproc_fn_dict=self.preproc_fn_dict,
-                    preprocessed=True
+                    preprocessed=True,
                 )
                 for i in range(num_splits)
             ]
 
     def __str__(self):
         """
         Returns a string describing the dataset.
         """
         txt = [
             f'{" DATASET OBJECT ":=^48}',
-            f'Splits            = {self.splits}',
-            f'Features          = {self.features}',
-            f'Default features  = {self.default_input} --> {self.default_output}',
-            '=' * 48
+            f"Splits            = {self.splits}",
+            f"Features          = {self.features}",
+            f"Default features  = {self.default_input} --> {self.default_output}",
+            "=" * 48,
         ]
-        return '\n'.join(txt)
+        return "\n".join(txt)
```

### Comparing `privacy_meter-1.0/privacy_meter/metric.py` & `Privacy-Meter-1.0.1/privacy_meter/metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 from abc import ABC, abstractmethod
-from typing import Callable, Optional, List, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 
-from privacy_meter.constants import *
+from privacy_meter.constants import NPZ_EXTENSION, MetricEnum, SignalSourceEnum
 from privacy_meter.information_source import InformationSource
-from privacy_meter.information_source_signal import Signal
-from privacy_meter.metric_result import MetricResult
-from privacy_meter.utils import flatten_array
+from privacy_meter.information_source_signal import GroupInfo, Signal
+from privacy_meter.metric_result import CombinedMetricResult, MetricResult
+from privacy_meter.utils import default_quantile, flatten_array
 
 ########################################################################################################################
 # METRIC CLASS
 ########################################################################################################################
 
 
 class Metric(ABC):
     """
     Interface to construct and perform a membership inference attack on a target model and dataset using auxiliary
     information specified by the user. This serves as a guideline for implementing a metric to be used for measuring
     the privacy leakage of a target model.
     """
 
     def __init__(
-            self,
-            target_info_source: InformationSource,
-            reference_info_source: InformationSource,
-            signals: List[Signal],
-            hypothesis_test_func: Optional[Callable],
-            logs_dirname: str
+        self,
+        target_info_source: InformationSource,
+        reference_info_source: InformationSource,
+        signals: List[Signal],
+        hypothesis_test_func: Optional[Callable],
+        logs_dirname: str,
     ):
         """
         Constructor
 
         Args:
             target_info_source: InformationSource, containing the Model that the metric will be performed on, and the
                 corresponding Dataset.
@@ -46,146 +46,244 @@
         self.target_info_source = target_info_source
         self.reference_info_source = reference_info_source
         self.signals = signals
         self.hypothesis_test_func = hypothesis_test_func
         self.logs_dirname = logs_dirname
 
     def _load_or_compute_signal(
-            self,
-            signal_source: SignalSourceEnum,
+        self,
+        signal_source: SignalSourceEnum,
     ):
         """
         Private helper function to load signals if they have been computed already, or compute and save signals
         if they haven't.
 
         Args:
             signal_source: Signal source to determine which information source and mapping objects need to be used.
 
         Returns:
             Signals computed using the specified information source and mapping object.
         """
-        signal_filepath = f'{self.logs_dirname}/{type(self).__name__}_{signal_source.value}'
+        if self.logs_dirname is not None:
+            signal_filepath = (
+                f"{self.logs_dirname}/{type(self).__name__}_{signal_source.value}"
+            )
+        else:
+            signal_filepath = None
 
         if signal_source == SignalSourceEnum.TARGET_MEMBER:
             info_source_obj = self.target_info_source
             mapping_obj = self.target_model_to_train_split_mapping
         elif signal_source == SignalSourceEnum.TARGET_NON_MEMBER:
             info_source_obj = self.target_info_source
             mapping_obj = self.target_model_to_test_split_mapping
-        elif signal_source == SignalSourceEnum.REFERENCE_MEMBER or signal_source == SignalSourceEnum.REFERENCE:
+        elif (
+            signal_source == SignalSourceEnum.REFERENCE_MEMBER
+            or signal_source == SignalSourceEnum.REFERENCE
+        ):
             info_source_obj = self.reference_info_source
             mapping_obj = self.reference_model_to_train_split_mapping
         elif signal_source == SignalSourceEnum.REFERENCE_NON_MEMBER:
             info_source_obj = self.reference_info_source
             mapping_obj = self.reference_model_to_test_split_mapping
         else:
             raise NotImplementedError
 
         signals = []
 
-        if os.path.isfile(f'{signal_filepath}{NPZ_EXTENSION}'):
-            with np.load(f'{signal_filepath}{NPZ_EXTENSION}', allow_pickle=True) as data:
-                signals = np.array(data['arr_0'][()])
+        if os.path.isfile(f"{signal_filepath}{NPZ_EXTENSION}"):
+            with np.load(
+                f"{signal_filepath}{NPZ_EXTENSION}", allow_pickle=True
+            ) as data:
+                signals = np.array(data["arr_0"][()])
         else:
             # For each signal, compute the response of the model on the dataset according to the mapping
             for signal in self.signals:
-                signals.append(
-                    info_source_obj.get_signal(signal, mapping_obj)
-                )
-            np.savez(signal_filepath, signals)
+                signals.append(info_source_obj.get_signal(signal, mapping_obj))
+            if signal_filepath is not None:
+                np.savez(signal_filepath, signals)
 
         return signals
 
-    def _set_default_mappings(
-            self,
-            unique_dataset: bool
+    def _load_or_compute_group_membership(
+        self,
+        signal_source: SignalSourceEnum,
     ):
         """
+        Private helper function to compute group membership
+        Args:
+            signal_source: Signal source to determine which information source and mapping objects need to be used.
+
+        Returns:
+            Group membership computed using the specified information source and mapping object.
+        """
+        if signal_source == SignalSourceEnum.TARGET_MEMBER:
+            info_source_obj = self.target_info_source
+            mapping_obj = self.target_model_to_train_split_mapping_group
+        elif signal_source == SignalSourceEnum.TARGET_NON_MEMBER:
+            info_source_obj = self.target_info_source
+            mapping_obj = self.target_model_to_test_split_mapping_group
+        elif (
+            signal_source == SignalSourceEnum.REFERENCE_MEMBER
+            or signal_source == SignalSourceEnum.REFERENCE
+        ):
+            info_source_obj = self.reference_info_source
+            mapping_obj = self.reference_model_to_train_split_mapping_group
+        elif signal_source == SignalSourceEnum.REFERENCE_NON_MEMBER:
+            info_source_obj = self.reference_info_source
+            mapping_obj = self.reference_model_to_test_split_mapping_group
+        else:
+            raise NotImplementedError
+
+        group_membership = info_source_obj.get_signal(GroupInfo(), mapping_obj)
+
+        return group_membership
+
+    def _set_default_mappings(self, unique_dataset: bool):
+        """
         Private helper function, to set default values for mappings between models and dataset splits.
 
         Args:
             unique_dataset: Boolean indicating if target_info_source and reference_info_source use one same dataset
                 object.
 
         """
         if unique_dataset:
             if self.target_model_to_train_split_mapping is None:
-                self.target_model_to_train_split_mapping = [(0, 'train000', '<default_input>', '<default_output>')]
+                self.target_model_to_train_split_mapping = [
+                    (0, "train000", "<default_input>", "<default_output>")
+                ]
             if self.target_model_to_test_split_mapping is None:
-                self.target_model_to_test_split_mapping = [(0, 'test000', '<default_input>', '<default_output>')]
+                self.target_model_to_test_split_mapping = [
+                    (0, "test000", "<default_input>", "<default_output>")
+                ]
             if self.reference_model_to_train_split_mapping is None:
                 self.reference_model_to_train_split_mapping = [
-                    (0, f'train{k + 1:03d}', '<default_input>', '<default_output>')
+                    (0, f"train{k + 1:03d}", "<default_input>", "<default_output>")
                     for k in range(len(self.reference_info_source.models))
                 ]
             if self.reference_model_to_test_split_mapping is None:
                 self.reference_model_to_test_split_mapping = [
-                    (0, f'test{k + 1:03d}', '<default_input>', '<default_output>')
+                    (0, f"test{k + 1:03d}", "<default_input>", "<default_output>")
                     for k in range(len(self.reference_info_source.models))
                 ]
         else:
             if self.target_model_to_train_split_mapping is None:
-                self.target_model_to_train_split_mapping = [(0, 'train', '<default_input>', '<default_output>')]
+                self.target_model_to_train_split_mapping = [
+                    (0, "train", "<default_input>", "<default_output>")
+                ]
             if self.target_model_to_test_split_mapping is None:
-                self.target_model_to_test_split_mapping = [(0, 'test', '<default_input>', '<default_output>')]
+                self.target_model_to_test_split_mapping = [
+                    (0, "test", "<default_input>", "<default_output>")
+                ]
             if self.reference_model_to_train_split_mapping is None:
                 self.reference_model_to_train_split_mapping = [
-                    (k, f'train', '<default_input>', '<default_output>')
+                    (k, "train", "<default_input>", "<default_output>")
                     for k in range(len(self.reference_info_source.models))
                 ]
             if self.reference_model_to_test_split_mapping is None:
                 self.reference_model_to_test_split_mapping = [
-                    (k, f'test', '<default_input>', '<default_output>')
+                    (k, "test", "<default_input>", "<default_output>")
+                    for k in range(len(self.reference_info_source.models))
+                ]
+
+    def _set_default_group_mappings(self, unique_dataset: bool):
+        """
+        Private helper function, to set default values for mappings between models and dataset splits for groups.
+        Args:
+            unique_dataset: Boolean indicating if target_info_source and reference_info_source use one same dataset
+                object.
+
+        """
+        if unique_dataset:
+            if self.target_model_to_train_split_mapping_group is None:
+                self.target_model_to_train_split_mapping_group = [
+                    (0, "train000", "<default_group>")
+                ]
+            if self.target_model_to_test_split_mapping_group is None:
+                self.target_model_to_test_split_mapping_group = [
+                    (0, "test000", "<default_group>")
+                ]
+            if self.reference_model_to_train_split_mapping_group is None:
+                self.reference_model_to_train_split_mapping_group = [
+                    (0, f"train{k + 1:03d}", "<default_group>")
+                    for k in range(len(self.reference_info_source.models))
+                ]
+            if self.reference_model_to_test_split_mapping_group is None:
+                self.reference_model_to_test_split_mapping_group = [
+                    (0, f"test{k + 1:03d}", "<default_group>")
+                    for k in range(len(self.reference_info_source.models))
+                ]
+        else:
+            if self.target_model_to_train_split_mapping_group is None:
+                self.target_model_to_train_split_mapping_group = [
+                    (0, "train", "<default_group>")
+                ]
+            if self.target_model_to_test_split_mapping_group is None:
+                self.target_model_to_test_split_mapping_group = [
+                    (0, "test", "<default_group>")
+                ]
+            if self.reference_model_to_train_split_mapping_group is None:
+                self.reference_model_to_train_split_mapping_group = [
+                    (k, "train", "<default_group>")
+                    for k in range(len(self.reference_info_source.models))
+                ]
+            if self.reference_model_to_test_split_mapping_group is None:
+                self.reference_model_to_test_split_mapping_group = [
+                    (k, "test", "<default_group>")
                     for k in range(len(self.reference_info_source.models))
                 ]
 
     @abstractmethod
     def prepare_metric(self):
         """
         Function to prepare data needed for running the metric on the target model and dataset, using signals computed
         on the auxiliary model(s) and dataset.
         """
         pass
 
     @abstractmethod
-    def run_metric(self, fpr_tolerance_rate_list=None) -> Union[MetricResult, List[MetricResult]]:
+    def run_metric(
+        self, fpr_tolerance_rate_list=None
+    ) -> Union[MetricResult, List[MetricResult]]:
         """
         Function to run the metric on the target model and dataset.
 
         Args:
             fpr_tolerance_rate_list (optional): List of FPR tolerance values that may be used by the threshold function
                 to compute the attack threshold for the metric.
 
         Returns:
             Result(s) of the metric.
         """
         pass
 
+
 ########################################################################################################################
 # POPULATION_METRIC CLASS
 ########################################################################################################################
 
 
 class PopulationMetric(Metric):
     """
     Inherits from the Metric class to perform the population membership inference attack which will be used as a metric
     for measuring privacy leakage of a target model.
     """
 
     def __init__(
-            self,
-            target_info_source: InformationSource,
-            reference_info_source: InformationSource,
-            signals: List[Signal],
-            hypothesis_test_func: Optional[Callable],
-            target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            unique_dataset: bool = False,
-            logs_dirname: str = None
+        self,
+        target_info_source: InformationSource,
+        reference_info_source: InformationSource,
+        signals: List[Signal],
+        hypothesis_test_func: Optional[Callable],
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        unique_dataset: bool = False,
+        logs_dirname: str = None,
     ):
         """
         Constructor
 
         Args:
             target_info_source: InformationSource, containing the Model that the metric will be performed on, and the
                 corresponding Dataset.
@@ -200,124 +298,128 @@
             reference_model_to_train_split_mapping: Mapping from the reference models to their train splits of the
                 corresponding reference dataset. By default, the code will look for a split named "train" if only one
                 reference model is provided, else for splits named "train000", "train001", "train002", etc. For the
                 population metric, at least one reference dataset should be passed.
         """
 
         # Initializes the parent metric
-        super().__init__(target_info_source=target_info_source,
-                         reference_info_source=reference_info_source,
-                         signals=signals,
-                         hypothesis_test_func=hypothesis_test_func,
-                         logs_dirname=logs_dirname)
+        super().__init__(
+            target_info_source=target_info_source,
+            reference_info_source=reference_info_source,
+            signals=signals,
+            hypothesis_test_func=hypothesis_test_func,
+            logs_dirname=logs_dirname,
+        )
 
         # Useless object, for compatibility purposes only
         self.reference_model_to_test_split_mapping = None
 
         # Logs directory
         self.logs_dirname = logs_dirname
 
         # Store the model to split mappings
         self.target_model_to_train_split_mapping = target_model_to_train_split_mapping
         self.target_model_to_test_split_mapping = target_model_to_test_split_mapping
-        self.reference_model_to_train_split_mapping = reference_model_to_train_split_mapping
+        self.reference_model_to_train_split_mapping = (
+            reference_model_to_train_split_mapping
+        )
         self._set_default_mappings(unique_dataset)
 
         # Variables used in prepare_metric and run_metric
         self.member_signals, self.non_member_signals = [], []
         self.reference_signals = []
 
     def prepare_metric(self):
         """
         Function to prepare data needed for running the metric on the target model and dataset, using signals computed
         on the auxiliary model(s) and dataset. For the population attack, the auxiliary model is the target model
         itself, and the auxiliary dataset is a random split from the target model's training data.
         """
         # Load signals if they have been computed already; otherwise, compute and save them
-        self.member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.TARGET_MEMBER))
-        self.non_member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER))
-        self.reference_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.REFERENCE))
+        self.member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_MEMBER)
+        )
+        self.non_member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER)
+        )
+        self.reference_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE)
+        )
 
     def run_metric(self, fpr_tolerance_rate_list=None) -> List[MetricResult]:
         """
         Function to run the metric on the target model and dataset.
 
         Args:
             fpr_tolerance_rate_list (optional): List of FPR tolerance values that may be used by the threshold function
                 to compute the attack threshold for the metric.
 
         Returns:
             A list of MetricResult objects, one per fpr value.
         """
-        metric_result_list = []
-        for fpr_tolerance_rate in fpr_tolerance_rate_list:
-            threshold = self.hypothesis_test_func(self.reference_signals, fpr_tolerance_rate)
-
-            member_preds = []
-            for signal in self.member_signals:
-                if signal <= threshold:
-                    member_preds.append(1)
-                else:
-                    member_preds.append(0)
-
-            non_member_preds = []
-            for signal in self.non_member_signals:
-                if signal <= threshold:
-                    non_member_preds.append(1)
-                else:
-                    non_member_preds.append(0)
-
-            predictions = np.concatenate([member_preds, non_member_preds])
-
-            true_labels = [1] * len(self.member_signals)
-            true_labels.extend([0] * len(self.non_member_signals))
-
-            signal_values = np.concatenate([self.member_signals, self.non_member_signals])
-
-            metric_result = MetricResult(
-                metric_id=MetricEnum.POPULATION.value,
-                predicted_labels=predictions,
-                true_labels=true_labels,
-                predictions_proba=None,
-                signal_values=signal_values,
-                threshold=threshold
-            )
+        # map the threshold with the alpha
+        if fpr_tolerance_rate_list is not None:
+            self.quantiles = fpr_tolerance_rate_list
+        else:
+            self.quantiles = default_quantile()
+        thresholds = self.hypothesis_test_func(
+            self.reference_signals, self.quantiles
+        ).reshape(-1, 1)
+
+        num_threshold = len(self.quantiles)
+        member_signals = self.member_signals.reshape(-1, 1).repeat(num_threshold, 1).T
+        non_member_signals = (
+            self.non_member_signals.reshape(-1, 1).repeat(num_threshold, 1).T
+        )
+        member_preds = np.less(member_signals, thresholds)
+        non_member_preds = np.less(non_member_signals, thresholds)
 
-            metric_result_list.append(metric_result)
+        predictions = np.concatenate([member_preds, non_member_preds], axis=1)
+        true_labels = np.concatenate(
+            [np.ones(len(self.member_signals)), np.zeros(len(self.non_member_signals))]
+        )
+        signal_values = np.concatenate([self.member_signals, self.non_member_signals])
+        metric_result = CombinedMetricResult(
+            metric_id=MetricEnum.REFERENCE.value,
+            predicted_labels=predictions,
+            true_labels=true_labels,
+            predictions_proba=None,
+            signal_values=signal_values,
+        )
+        return [metric_result]
 
-        return metric_result_list
 
 ########################################################################################################################
 # SHADOW_METRIC CLASS
 ########################################################################################################################
 
 
 class ShadowMetric(Metric):
     """
     Inherits from the Metric class to perform the shadow membership inference attack which will be used as a metric for
     measuring privacy leakage of a target model.
     """
 
     def __init__(
-            self,
-            target_info_source: InformationSource,
-            reference_info_source: InformationSource,
-            signals: List[Signal],
-            hypothesis_test_func: Optional[Callable],
-            target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reference_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reweight_samples: bool = True,
-            unique_dataset: bool = False,
-            logs_dirname: str = None
+        self,
+        target_info_source: InformationSource,
+        reference_info_source: InformationSource,
+        signals: List[Signal],
+        hypothesis_test_func: Optional[Callable],
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reweight_samples: bool = True,
+        unique_dataset: bool = False,
+        logs_dirname: str = None,
     ):
         """
         Constructor
-        
+
         Args:
             target_info_source: InformationSource, containing the Model that the metric will be performed on, and the
                 corresponding Dataset.
             reference_info_source: List of InformationSource(s), containing the Model(s) that the metric will be
                 fitted on, and their corresponding Dataset.
             signals: List of signals to be used.
             hypothesis_test_func: Function that will be used for computing attack threshold(s)
@@ -334,48 +436,61 @@
             reweight_samples: Boolean specifying if the metric should account for an unbalance between the number of
                 members vs non-members.
             unique_dataset: Boolean indicating if target_info_source and reference_info_source use one same dataset
                 object.
         """
 
         # Initializes the parent metric
-        super().__init__(target_info_source=target_info_source,
-                         reference_info_source=reference_info_source,
-                         signals=signals,
-                         hypothesis_test_func=hypothesis_test_func,
-                         logs_dirname=logs_dirname)
+        super().__init__(
+            target_info_source=target_info_source,
+            reference_info_source=reference_info_source,
+            signals=signals,
+            hypothesis_test_func=hypothesis_test_func,
+            logs_dirname=logs_dirname,
+        )
 
         # Logs directory
         self.logs_dirname = logs_dirname
 
         self.reweight_samples = reweight_samples
 
         # Store the model to split mappings
         self.target_model_to_train_split_mapping = target_model_to_train_split_mapping
         self.target_model_to_test_split_mapping = target_model_to_test_split_mapping
-        self.reference_model_to_train_split_mapping = reference_model_to_train_split_mapping
-        self.reference_model_to_test_split_mapping = reference_model_to_test_split_mapping
+        self.reference_model_to_train_split_mapping = (
+            reference_model_to_train_split_mapping
+        )
+        self.reference_model_to_test_split_mapping = (
+            reference_model_to_test_split_mapping
+        )
         self._set_default_mappings(unique_dataset)
 
         # Variables used in prepare_metric and run_metric
         self.member_signals, self.non_member_signals = [], []
         self.reference_member_signals, self.reference_non_member_signals = [], []
 
     def prepare_metric(self):
         """
         Function to prepare data needed for running the metric on the target model and dataset, using signals computed
         on the reference model(s) and dataset. For the shadow attack, the reference models will be a list of shadow
         models and the auxiliary dataset will contain the train-test splits of these models.
         """
         # Load signals if they have been computed already; otherwise, compute and save them
-        self.member_signals = flatten_array(self._load_or_compute_signal(signal_source=SignalSourceEnum.TARGET_MEMBER))
-        self.non_member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER))
-        self.reference_member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.REFERENCE_MEMBER))
+        self.member_signals = flatten_array(
+            self._load_or_compute_signal(signal_source=SignalSourceEnum.TARGET_MEMBER)
+        )
+        self.non_member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER)
+        )
+        self.reference_member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_MEMBER)
+        )
         self.reference_non_member_signals = flatten_array(
-            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_NON_MEMBER))
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_NON_MEMBER)
+        )
 
     def run_metric(self, fpr_tolerance_rate_list=None) -> MetricResult:
         """
         Function to run the metric on the target model and dataset.
 
         Args:
             fpr_tolerance_rate_list (optional): List of FPR tolerance values that may be used by the threshold function
@@ -383,72 +498,92 @@
 
         Returns:
             The result of the metric
         """
 
         # Create and fit a LogisticRegression object, from the members and non-members of the reference
         # InformationSource
-        clf = LogisticRegression(class_weight={
-            0: self.reference_member_signals.shape[0],
-            1: self.reference_non_member_signals.shape[0],
-        } if self.reweight_samples else None)
-        x = np.concatenate([self.reference_member_signals, self.reference_non_member_signals]).reshape(-1, 1)
-        y = np.array([1] * len(self.reference_member_signals) + [0] * len(self.reference_non_member_signals))
+        clf = LogisticRegression(
+            class_weight={
+                0: self.reference_member_signals.shape[0],
+                1: self.reference_non_member_signals.shape[0],
+            }
+            if self.reweight_samples
+            else None
+        )
+        x = np.concatenate(
+            [self.reference_member_signals, self.reference_non_member_signals]
+        ).reshape(-1, 1)
+        y = np.array(
+            [1] * len(self.reference_member_signals)
+            + [0] * len(self.reference_non_member_signals)
+        )
         clf.fit(x, y)
 
-        signal_space = np.linspace(np.array(x).ravel().min(), np.array(x).ravel().max(), 200).reshape((-1, 1))
-        i = np.max([i if v == 1 else -1 for i, v in enumerate(clf.predict(signal_space))])
-        threshold = signal_space[i:i + 2].mean()
+        signal_space = np.linspace(
+            np.array(x).ravel().min(), np.array(x).ravel().max(), 200
+        ).reshape((-1, 1))
+        i = np.max(
+            [i if v == 1 else -1 for i, v in enumerate(clf.predict(signal_space))]
+        )
+        threshold = signal_space[i : i + 2].mean()
 
         # Predict the membership status of samples in the target InformationSource
-        predictions_proba = clf.predict_proba(np.concatenate([
-            self.member_signals.reshape(-1, 1),
-            self.non_member_signals.reshape(-1, 1)
-        ]))
+        predictions_proba = clf.predict_proba(
+            np.concatenate(
+                [
+                    self.member_signals.reshape(-1, 1),
+                    self.non_member_signals.reshape(-1, 1),
+                ]
+            )
+        )
         predictions_label = np.argmax(predictions_proba, axis=1)
         predictions_proba = predictions_proba[:, 1]
 
-        true_labels = [1] * len(self.member_signals) + [0] * len(self.non_member_signals)
+        true_labels = [1] * len(self.member_signals) + [0] * len(
+            self.non_member_signals
+        )
         signal_values = np.concatenate([self.member_signals, self.non_member_signals])
 
         # Evaluate the power of this inference and display the result
         metric_result = MetricResult(
             metric_id=MetricEnum.SHADOW.value,
             predictions_proba=predictions_proba,
             predicted_labels=predictions_label,
             true_labels=true_labels,
             signal_values=signal_values,
-            threshold=threshold
+            threshold=threshold,
         )
 
         return metric_result
 
+
 ########################################################################################################################
 # REFERENCE_METRIC CLASS
 ########################################################################################################################
 
 
 class ReferenceMetric(Metric):
     """
     Inherits from the Metric class to perform the reference membership inference attack which will be used as a metric
     for measuring privacy leakage of a target model.
     """
 
     def __init__(
-            self,
-            target_info_source: InformationSource,
-            reference_info_source: InformationSource,
-            signals: List[Signal],
-            hypothesis_test_func: Optional[Callable],
-            target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
-            reference_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
-            unique_dataset: bool = False,
-            logs_dirname: str = None
+        self,
+        target_info_source: InformationSource,
+        reference_info_source: InformationSource,
+        signals: List[Signal],
+        hypothesis_test_func: Optional[Callable],
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        unique_dataset: bool = False,
+        logs_dirname: str = None,
     ):
         """
         Constructor
 
         Args:
             target_info_source: InformationSource, containing the Model that the metric will be performed on, and the
                 corresponding Dataset.
@@ -464,36 +599,38 @@
                 corresponding reference dataset. By default, the code will look for a split named "train"
             reference_model_to_test_split_mapping: Mapping from the reference models to their test splits of the
                 corresponding reference dataset. By default, the code will look for a split named "test"
             unique_dataset: Boolean indicating if target_info_source and target_info_source use one same dataset object.
         """
 
         # Initializes the parent metric
-        super().__init__(target_info_source=target_info_source,
-                         reference_info_source=reference_info_source,
-                         signals=signals,
-                         hypothesis_test_func=hypothesis_test_func,
-                         logs_dirname=logs_dirname)
+        super().__init__(
+            target_info_source=target_info_source,
+            reference_info_source=reference_info_source,
+            signals=signals,
+            hypothesis_test_func=hypothesis_test_func,
+            logs_dirname=logs_dirname,
+        )
 
         # Logs directory
         self.logs_dirname = logs_dirname
 
         # Store the model to split mappings
         self.target_model_to_train_split_mapping = target_model_to_train_split_mapping
         self.target_model_to_test_split_mapping = target_model_to_test_split_mapping
 
         # Custom default mapping for the reference metric
         if reference_model_to_train_split_mapping is None:
             self.reference_model_to_train_split_mapping = [
-                                                              (0, 'train', '<default_input>', '<default_output>')
-                                                          ] * len(self.reference_info_source.models)
+                (0, "train", "<default_input>", "<default_output>")
+            ] * len(self.reference_info_source.models)
         if reference_model_to_test_split_mapping is None:
             self.reference_model_to_test_split_mapping = [
-                                                             (0, 'test', '<default_input>', '<default_output>')
-                                                         ] * len(self.reference_info_source.models)
+                (0, "test", "<default_input>", "<default_output>")
+            ] * len(self.reference_info_source.models)
 
         self._set_default_mappings(unique_dataset)
 
         # Variables used in prepare_metric and run_metric
         self.member_signals, self.non_member_signals = [], []
         self.reference_member_signals, self.reference_non_member_signals = [], []
         self.pointwise_member_thresholds, self.pointwise_non_member_thresholds = [], []
@@ -502,61 +639,267 @@
         """
         Function to prepare data needed for running the metric on the target model and dataset, using signals computed
         on the reference model(s) and dataset. For the reference attack, the reference models will be a list of models
         trained on data from the same distribution, and the reference dataset will be the target model's train-test
         split.
         """
         # Load signals if they have been computed already; otherwise, compute and save them
-        self.member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.TARGET_MEMBER))
-        self.non_member_signals = flatten_array(self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER))
+        self.member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_MEMBER)
+        )
+        self.non_member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER)
+        )
         self.reference_member_signals = np.array(
-            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_MEMBER)[0]).transpose()
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_MEMBER)[0]
+        ).transpose()
         self.reference_non_member_signals = np.array(
-            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_NON_MEMBER)[0]).transpose()
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE_NON_MEMBER)[0]
+        ).transpose()
 
     def run_metric(self, fpr_tolerance_rate_list=None) -> List[MetricResult]:
         """
         Function to run the metric on the target model and dataset.
 
         Args:
             fpr_tolerance_rate_list (optional): List of FPR tolerance values that may be used by the threshold function
                 to compute the attack threshold for the metric.
 
         Returns:
             A list of MetricResult objects, one per fpr value.
         """
-        metric_result_list = []
-        for fpr_tolerance_rate in fpr_tolerance_rate_list:
-            member_preds = []
-            for idx, signal in enumerate(self.member_signals):
-                # Use pointwise threshold
-                threshold = self.hypothesis_test_func(self.reference_member_signals[idx], fpr_tolerance_rate)
-                if signal <= threshold:
-                    member_preds.append(1)
-                else:
-                    member_preds.append(0)
-
-            non_member_preds = []
-            for idx, signal in enumerate(self.non_member_signals):
-                # Use pointwise threshold
-                threshold = self.hypothesis_test_func(self.reference_non_member_signals[idx], fpr_tolerance_rate)
-                if signal <= threshold:
-                    non_member_preds.append(1)
-                else:
-                    non_member_preds.append(0)
-
-            predictions = np.concatenate([member_preds, non_member_preds])
-
-            true_labels = [1] * len(self.member_signals)
-            true_labels.extend([0] * len(self.non_member_signals))
-
-            signal_values = np.concatenate([self.member_signals, self.non_member_signals])
-
-            metric_result = MetricResult(metric_id=MetricEnum.REFERENCE.value,
-                                         predicted_labels=predictions,
-                                         true_labels=true_labels,
-                                         predictions_proba=None,
-                                         signal_values=signal_values)
 
-            metric_result_list.append(metric_result)
+        if fpr_tolerance_rate_list is None:
+            self.quantiles = default_quantile()
+        else:
+            self.quantiles = np.array(fpr_tolerance_rate_list)
+        reference_member_threshold = self.hypothesis_test_func(
+            self.reference_member_signals, self.quantiles
+        )
+        reference_non_member_threshold = self.hypothesis_test_func(
+            self.reference_non_member_signals, self.quantiles
+        )
 
-        return metric_result_list
+        num_threshold = len(self.quantiles)
+        member_signals = self.member_signals.reshape(-1, 1).repeat(num_threshold, 1).T
+        non_member_signals = (
+            self.non_member_signals.reshape(-1, 1).repeat(num_threshold, 1).T
+        )
+        member_preds = np.less(member_signals, reference_member_threshold)
+        non_member_preds = np.less(non_member_signals, reference_non_member_threshold)
+
+        predictions = np.concatenate([member_preds, non_member_preds], axis=1)
+        true_labels = np.concatenate(
+            [np.ones(len(self.member_signals)), np.zeros(len(self.non_member_signals))]
+        )
+
+        signal_values = np.concatenate([self.member_signals, self.non_member_signals])
+
+        metric_result = CombinedMetricResult(
+            metric_id=MetricEnum.REFERENCE.value,
+            predicted_labels=predictions,
+            true_labels=true_labels,
+            predictions_proba=None,
+            signal_values=signal_values,
+        )
+
+        return [metric_result]
+
+
+########################################################################################################################
+# GroupPopulationMetric CLASS
+########################################################################################################################
+
+
+class GroupPopulationMetric(Metric):
+    """
+    Inherits from the Metric class to perform the population membership inference attack which will be used as a metric
+    for measuring privacy leakage of a target model. Compared to PopulationMetric, this new metric is designed to compute the threshold per class.
+    """
+
+    def __init__(
+        self,
+        target_info_source: InformationSource,
+        reference_info_source: InformationSource,
+        signals: List[Signal],
+        hypothesis_test_func: Optional[Callable],
+        target_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        target_model_to_test_split_mapping: List[Tuple[int, str, str, str]] = None,
+        reference_model_to_train_split_mapping: List[Tuple[int, str, str, str]] = None,
+        target_model_to_train_split_mapping_group: List[Tuple[int, str, str]] = None,
+        target_model_to_test_split_mapping_group: List[Tuple[int, str, str]] = None,
+        reference_model_to_train_split_mapping_group: List[Tuple[int, str, str]] = None,
+        unique_dataset: bool = False,
+        logs_dirname: str = None,
+    ):
+        """
+        Constructor
+
+        Args:
+            target_info_source: InformationSource, containing the Model that the metric will be performed on, and the
+                corresponding Dataset.
+            reference_info_source: List of InformationSource(s), containing the Model(s) that the metric will be
+                fitted on, and their corresponding Dataset.
+            signals: List of signals to be used.
+            hypothesis_test_func: Function that will be used for computing attack threshold(s)
+            target_model_to_train_split_mapping: Mapping from the target model to the train split of the target dataset.
+                By default, the code will look for a split named "train".
+            target_model_to_test_split_mapping: Mapping from the target model to the test split of the target dataset.
+                By default, the code will look for a split named "test".
+            reference_model_to_train_split_mapping: Mapping from the reference models to their train splits of the
+                corresponding reference dataset. By default, the code will look for a split named "train" if only one
+                reference model is provided, else for splits named "train000", "train001", "train002", etc. For the
+                population metric, at least one reference dataset should be passed.
+            target_model_to_train_split_mapping_group: Mapping from the target model to the train split of the target dataset with respect to group information.
+                By default, the code will look for a split named "train".
+            target_model_to_test_split_mapping_group: Mapping from the target model to the test split of the target dataset with respect to group information.
+                By default, the code will look for a split named "test".
+            reference_model_to_train_split_mapping_group: Mapping from the reference models to their train splits of the
+                corresponding reference dataset  with respect to group information.. By default, the code will look for a split named "train" if only one
+                reference model is provided, else for splits named "train000", "train001", "train002", etc. For the
+                population metric, at least one reference dataset should be passed.
+        """
+
+        # Initializes the parent metric
+        super().__init__(
+            target_info_source=target_info_source,
+            reference_info_source=reference_info_source,
+            signals=signals,
+            hypothesis_test_func=hypothesis_test_func,
+            logs_dirname=logs_dirname,
+        )
+
+        # Useless object, for compatibility purposes only
+        self.reference_model_to_test_split_mapping = None
+        self.reference_model_to_test_split_mapping_group = None
+
+        # Logs directory
+        self.logs_dirname = logs_dirname
+
+        # Store the model to split mappings
+        self.target_model_to_train_split_mapping = target_model_to_train_split_mapping
+        self.target_model_to_test_split_mapping = target_model_to_test_split_mapping
+        self.reference_model_to_train_split_mapping = (
+            reference_model_to_train_split_mapping
+        )
+        self.target_model_to_train_split_mapping_group = (
+            target_model_to_train_split_mapping_group
+        )
+        self.target_model_to_test_split_mapping_group = (
+            target_model_to_test_split_mapping_group
+        )
+        self.reference_model_to_train_split_mapping_group = (
+            reference_model_to_train_split_mapping_group
+        )
+
+        # get the mapping for the groups
+        self._set_default_group_mappings(unique_dataset)
+        self._set_default_mappings(unique_dataset)
+
+        # Variables used in prepare_metric and run_metric
+        self.member_signals, self.non_member_signals = [], []
+        self.reference_signals = []
+        self.member_groups, self.non_member_groups = [], []
+        self.reference_groups = []
+
+    def prepare_metric(self):
+        """
+        Function to prepare data needed for running the metric on the target model and dataset, using signals computed
+        on the auxiliary model(s) and dataset. For the population attack, the auxiliary model is the target model
+        itself, and the auxiliary dataset is a random split from the target model's training data.
+        """
+        # Load signals if they have been computed already; otherwise, compute and save them
+        self.member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_MEMBER)
+        )
+        self.non_member_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.TARGET_NON_MEMBER)
+        )
+        self.reference_signals = flatten_array(
+            self._load_or_compute_signal(SignalSourceEnum.REFERENCE)
+        )
+        self.reference_groups = flatten_array(
+            self._load_or_compute_group_membership(SignalSourceEnum.REFERENCE)
+        )
+        self.non_member_groups = flatten_array(
+            self._load_or_compute_group_membership(SignalSourceEnum.TARGET_NON_MEMBER)
+        )
+        self.member_groups = flatten_array(
+            self._load_or_compute_group_membership(SignalSourceEnum.TARGET_MEMBER)
+        )
+
+    def run_metric(self, fpr_tolerance_rate_list=None) -> List[MetricResult]:
+        """
+        Function to run the metric on the target model and dataset.
+
+        Args:
+            fpr_tolerance_rate_list (optional): List of FPR tolerance values that may be used by the threshold function
+                to compute the attack threshold for the metric.
+
+        Returns:
+            A list of MetricResult objects, one per fpr value.
+        """
+        if fpr_tolerance_rate_list is None:
+            self.quantiles = default_quantile()
+        else:
+            self.quantiles = fpr_tolerance_rate_list
+
+        num_threshold = len(self.quantiles)
+        member_preds = []
+        non_member_preds = []
+        reference_thresholds = {}
+        member_signal_list = []
+        non_member_signal_list = []
+        for g in np.unique(self.reference_groups):
+
+            thresholds = self.hypothesis_test_func(
+                self.reference_signals[self.reference_groups == g], self.quantiles
+            ).reshape(-1, 1)
+
+            member_signals = (
+                self.member_signals[self.member_groups == g]
+                .reshape(-1, 1)
+                .repeat(num_threshold, 1)
+                .T
+            )
+
+            non_member_signals = (
+                self.non_member_signals[self.non_member_groups == g]
+                .reshape(-1, 1)
+                .repeat(num_threshold, 1)
+                .T
+            )
+            member_pred = np.less(member_signals, thresholds)
+            non_member_pred = np.less(non_member_signals, thresholds)
+
+            member_signal_list.append(self.member_signals[self.member_groups == g])
+            non_member_signal_list.append(
+                self.non_member_signals[self.member_groups == g]
+            )
+            member_preds.append(member_pred)
+            non_member_preds.append(non_member_pred)
+
+            reference_thresholds[g] = thresholds
+
+        member_preds = np.concatenate(member_preds, axis=1)
+        non_member_preds = np.concatenate(non_member_preds, axis=1)
+        predictions = np.concatenate([member_preds, non_member_preds], axis=1)
+        true_labels = np.concatenate(
+            [np.ones(len(self.member_signals)), np.zeros(len(self.non_member_signals))]
+        )
+
+        member_signals = np.concatenate(
+            member_signal_list, axis=0
+        )  # reoder based on the groups
+        non_member_signals = np.concatenate(non_member_signal_list, axis=0)
+
+        signal_values = np.concatenate([member_signals, non_member_signals])
+
+        metric_result = CombinedMetricResult(
+            metric_id=MetricEnum.REFERENCE.value,
+            predicted_labels=predictions,
+            true_labels=true_labels,
+            predictions_proba=None,
+            signal_values=signal_values,
+            threshold=reference_thresholds,
+        )
+        return [metric_result]
```

### Comparing `privacy_meter-1.0/privacy_meter/utils.py` & `Privacy-Meter-1.0.1/privacy_meter/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,7 +16,16 @@
     flat_array = []
     for item in arr:
         if isinstance(item, (list, tuple, set, np.ndarray)):
             flat_array.extend(flatten_array(item))
         else:
             flat_array.append(item)
     return np.array(flat_array)
+
+
+def default_quantile():
+    """Return the default fprs
+
+    Returns:
+        arr: Numpy array, indicating the default fprs
+    """
+    return np.logspace(-5, 0, 100)
```

### Comparing `privacy_meter-1.0/privacy_meter/information_source.py` & `Privacy-Meter-1.0.1/privacy_meter/information_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import List, Tuple
 
 from privacy_meter.dataset import Dataset
-from privacy_meter.model import Model
 from privacy_meter.information_source_signal import Signal
+from privacy_meter.model import Model
 
 ########################################################################################################################
 # INFORMATION_SOURCE CLASS
 ########################################################################################################################
 
 
 class InformationSource:
     """
     Interface to dispatch Model objects, Dataset objects, and any additional objects required, to Signal objects.
     """
 
-    def __init__(self,
-                 models: List[Model],
-                 datasets: List[Dataset],
-                 default_model_to_split_mapping: List[Tuple[int, str, str, str]] = None
-                 ):
+    def __init__(
+        self,
+        models: List[Model],
+        datasets: List[Dataset],
+        default_model_to_split_mapping: List[Tuple[int, str, str, str]] = None,
+    ):
         """Constructor
 
         Args:
             models: List of models to be queried.
             datasets: List of datasets to be queried.
             default_model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -33,19 +34,20 @@
                 This can also be provided independently for each call, through the model_to_split_mapping argument of
                 the get_signal function.
         """
         self.models = models
         self.datasets = datasets
         self.default_model_to_split_mapping = default_model_to_split_mapping
 
-    def get_signal(self,
-                   signal: Signal,
-                   model_to_split_mapping: List[Tuple[int, str, str, str]] = None,
-                   extra: dict = None
-                   ):
+    def get_signal(
+        self,
+        signal: Signal,
+        model_to_split_mapping: List[Tuple[int, str, str, str]] = None,
+        extra: dict = None,
+    ):
         """Calls the signal object with the appropriate arguments: Model objects and Dataset objects specified at
         object instantiation, plus and any additional object required.
 
         Args:
             signal: The signal object to call.
             model_to_split_mapping: List of tuples, indicating how each model should query the dataset.
                 More specifically, for model #i:
@@ -63,15 +65,17 @@
 
         # If no value of model_to_split_mapping is provided, use the default value
         if model_to_split_mapping is None:
             model_to_split_mapping = self.default_model_to_split_mapping
         # If no value of model_to_split_mapping is provided and no default value is set, raise an exception
         if model_to_split_mapping is None:
             raise TypeError(
-                'At least one of self.default_model_to_split_mapping and model_to_split_mapping should be specified'
+                "At least one of self.default_model_to_split_mapping and model_to_split_mapping should be specified"
             )
 
         # Calls the signal object, and returns the value of the call
-        return signal(models=self.models,
-                      datasets=self.datasets,
-                      model_to_split_mapping=model_to_split_mapping,
-                      extra=extra)
+        return signal(
+            models=self.models,
+            datasets=self.datasets,
+            model_to_split_mapping=model_to_split_mapping,
+            extra=extra,
+        )
```

### Comparing `privacy_meter-1.0/setup.py` & `Privacy-Meter-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import io
 import os
+
 from setuptools import setup
 
-DESCRIPTION = f'Privacy Meter: An open-source library to audit data privacy in statistical and machine learning ' \
-              f'algorithms.'
+DESCRIPTION = (
+    "Privacy Meter: An open-source library to audit data privacy in statistical and machine learning "
+    "algorithms."
+)
 
 here = os.path.abspath(os.path.dirname(__file__))
-
+version = "1.0.1"
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'project_description.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
-      name='privacy_meter',
-      version='1.0',
-      description=DESCRIPTION,
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      url='https://github.com/privacytrustlab/ml_privacy_meter',
-      author_email='reza@comp.nus.edu.sg',
-      license="MIT",
-      packages=['privacy_meter'],
-      python_requires='>=3.6.0',
-      include_package_data=True,
-      classifiers=[
-            "License :: OSI Approved :: MIT License",
-            "Programming Language :: Python :: 3",
-      ],
+    name="Privacy-Meter",
+    version=version,
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    # change to the privacy_meter when the repo is renamed
+    url="https://github.com/privacytrustlab/ml_privacy_meter",
+    author_email="reza@comp.nus.edu.sg",
+    maintainer="Hongyan Chang",
+    maintainer_email="hongyan@comp.nus.edu.sg",
+    license="MIT",
+    packages=["privacy_meter"],
+    python_requires=">=3.8.0",
+    include_package_data=True,
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+    ],
 )
```

