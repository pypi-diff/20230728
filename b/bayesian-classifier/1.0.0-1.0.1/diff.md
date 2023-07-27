# Comparing `tmp/bayesian_classifier-1.0.0.tar.gz` & `tmp/bayesian_classifier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian_classifier-1.0.0.tar", last modified: Mon Feb  6 06:25:41 2023, max compression
+gzip compressed data, was "bayesian_classifier-1.0.1.tar", last modified: Thu Jul 27 23:48:12 2023, max compression
```

## Comparing `bayesian_classifier-1.0.0.tar` & `bayesian_classifier-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 06:25:41.831837 bayesian_classifier-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-06 06:25:41.831837 bayesian_classifier-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 06:25:41.831837 bayesian_classifier-1.0.0/bayesian_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/bayesian_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/bayesian_classifier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/bayesian_classifier/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/bayesian_classifier/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 06:25:41.831837 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 06:25:41.000000 bayesian_classifier-1.0.0/bayesian_classifier.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 06:25:41.831837 bayesian_classifier-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-06 06:25:30.000000 bayesian_classifier-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:12.987109 bayesian_classifier-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 23:48:12.987109 bayesian_classifier-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:12.987109 bayesian_classifier-1.0.1/bayesian_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/bayesian_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/bayesian_classifier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/bayesian_classifier/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/bayesian_classifier/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/bayesian_classifier/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:12.987109 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 23:48:12.000000 bayesian_classifier-1.0.1/bayesian_classifier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 23:48:03.000000 bayesian_classifier-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:48:12.987109 bayesian_classifier-1.0.1/setup.cfg
```

### Comparing `bayesian_classifier-1.0.0/bayesian_classifier/__main__.py` & `bayesian_classifier-1.0.1/bayesian_classifier/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 import os
 from .dataset import CSVDataset
 from .classifiers import NaiveBayes, FullBayes
+from .evaluate import evaluate_model_performance
+
 
 @click.group()
 def cli():
     pass
 
 @cli.group("naive_bayes")
 def naive_bayes_group():
@@ -35,25 +37,15 @@
     classifier = NaiveBayes()
     classifier.load(model)
     
     if not os.path.exists(dataset):
         raise Exception(f"File {dataset} not found")
 
     dataset = CSVDataset(dataset, sep)
-    correct=0
-    total=0
-    for i in range(0,len(dataset.labels)):
-        label = dataset.labels[i]
-        for sample in dataset.dataset[i]:
-            label_pred = classifier.classify(sample)
-            if label == label_pred:
-                correct+=1
-            total+=1
-    
-    print("Accuracy: {}".format(correct/total))
+    evaluate_model_performance(dataset, classifier)
 
 
 @cli.group("full_bayes")
 def full_bayes_group():
     pass
 
 @full_bayes_group.command(name="train")
@@ -80,22 +72,12 @@
     classifier = FullBayes()
     classifier.load(model)
     
     if not os.path.exists(dataset):
         raise Exception(f"File {dataset} not found")
 
     dataset = CSVDataset(dataset, sep)
-    correct=0
-    total=0
-    for i in range(0,len(dataset.labels)):
-        label = dataset.labels[i]
-        for sample in dataset.dataset[i]:
-            label_pred = classifier.classify(sample)
-            if label == label_pred:
-                correct+=1
-            total+=1
-    
-    print("Accuracy: {}".format(correct/total))
+    evaluate_model_performance(dataset, classifier)
 
 
 if __name__=="__main__":
     cli()
```

### Comparing `bayesian_classifier-1.0.0/bayesian_classifier/classifiers.py` & `bayesian_classifier-1.0.1/bayesian_classifier/classifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import abc
 import numpy
 
-
-
 class Classifier(abc.ABC):
     def __init__(self):
         pass
 
     @abc.abstractmethod
     def fit(self, dataset):
         pass
```

### Comparing `bayesian_classifier-1.0.0/bayesian_classifier/dataset.py` & `bayesian_classifier-1.0.1/bayesian_classifier/dataset.py`

 * *Files identical despite different names*

