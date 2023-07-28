# Comparing `tmp/dispersenn2-0.0.2.tar.gz` & `tmp/dispersenn2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispersenn2-0.0.2.tar", max compression
+gzip compressed data, was "dispersenn2-0.0.3.tar", max compression
```

## Comparing `dispersenn2-0.0.2.tar` & `dispersenn2-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      366 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/__init__.py
--rw-r--r--   0        0        0     2129 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/check_params.py
--rw-r--r--   0        0        0    13167 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/data_generation.py
--rw-r--r--   0        0        0    23908 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/disperseNN2.py
--rw-r--r--   0        0        0     7097 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/process_input.py
--rw-r--r--   0        0        0     3824 2023-07-25 00:18:01.284112 dispersenn2-0.0.2/dispersenn2/read_input.py
--rw-r--r--   0        0        0      575 2023-07-25 20:39:09.049643 dispersenn2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 dispersenn2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-28 19:39:37.121430 dispersenn2-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-27 22:45:44.334779 dispersenn2-0.0.3/dispersenn2/check_params.py
+-rw-r--r--   0        0        0    13167 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/data_generation.py
+-rw-r--r--   0        0        0    24917 2023-07-28 20:57:42.467508 dispersenn2-0.0.3/dispersenn2/disperseNN2.py
+-rw-r--r--   0        0        0     7097 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/process_input.py
+-rw-r--r--   0        0        0     3824 2023-07-27 20:51:57.445326 dispersenn2-0.0.3/dispersenn2/read_input.py
+-rw-r--r--   0        0        0      575 2023-07-28 20:58:14.295946 dispersenn2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 dispersenn2-0.0.3/PKG-INFO
```

### Comparing `dispersenn2-0.0.2/dispersenn2/check_params.py` & `dispersenn2-0.0.3/dispersenn2/check_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 
 def check_params(args):
     # avoid overwriting saved weights or other output files
     if args.train is True:
         if os.path.exists(
             args.out + "/Train/disperseNN2_" + str(args.seed) + "_model.hdf5"
-        ):
+        ) and args.force is False:
             print("saved model with specified output name already \
-                   exists (i.e. --out)")
+                   exists. To force overwrite, use --force.")
             exit()
     if args.predict is True and args.empirical is None:
         if os.path.exists(args.out
                           + "/Test/predictions_"
                           + str(args.seed)
-                          + ".txt"):
+                          + ".txt") and args.force is False:
             print(
-                "saved predictions with specified output name already exists \
-                (i.e. --out + --seed)"
+                "saved predictions with specified output name already exists. \
+                To force overwrite, use --force."
             )
             exit()
 
     # other checks
     if (
         args.train is False
         and args.predict is False
```

### Comparing `dispersenn2-0.0.2/dispersenn2/data_generation.py` & `dispersenn2-0.0.3/dispersenn2/data_generation.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.2/dispersenn2/disperseNN2.py` & `dispersenn2-0.0.3/dispersenn2/disperseNN2.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 import os
 import sys
 import random
 import argparse
 from sklearn.model_selection import train_test_split
 from dispersenn2.check_params import check_params
-from dispersenn2.read_input import list2dict, read_list, read_locs, dict_from_preprocessed
+from dispersenn2.read_input import list2dict
+from dispersenn2.read_input import read_list
+from dispersenn2.read_input import read_locs
+from dispersenn2.read_input import dict_from_preprocessed
 from dispersenn2.process_input import project_locs, vcf2genos
 import gpustat
 import itertools
 import numpy as np
 import matplotlib.pyplot as plt
 
 
@@ -114,15 +117,15 @@
     default=0.2,
     type=float,
     help="proportion of training set (after holding out test data) \
     to use for validation during training.",
 )
 parser.add_argument(
     "--batch_size",
-    default=1,
+    default=10,
     type=int,
     help="batch size for training")
 parser.add_argument(
     "--max_epochs", default=1000, type=int, help="max epochs for training"
 )
 parser.add_argument(
     "--patience",
@@ -155,15 +158,16 @@
     default=None,
 )
 parser.add_argument("--seed", default=None, type=int, help="random seed.")
 parser.add_argument(
     "--gpu",
     default="-1",
     type=str,
-    help="index of gpu. To avoid GPUs, skip this flag or say '-1'. \
+    help="gpu index (uses a single GPU). To avoid GPUs, \
+    skip this flag or say '-1'. \
     To use any available GPU say 'any' ",
 )
 parser.add_argument(
     "--plot_history",
     default=False,
     type=str,
     help="plot training history? default: False",
@@ -231,14 +235,21 @@
 parser.add_argument(
     "--pairs_encode",
     help="number of pairs (<= pairs_encode) to use for gradient \
     in the first part of the network",
     type=int,
     default=None,
 )
+parser.add_argument(
+    "--force",
+    action="store_true",
+    default=False,
+    help="force overwrite of existing data: \
+    including existing model, or predictions"
+)
 args = parser.parse_args()
 check_params(args)
 if len(sys.argv) == 1:
     parser.print_help()
     sys.exit(1)
 
 
@@ -255,39 +266,36 @@
         ratios = map(
             lambda gpu: float(gpu.entry["memory.used"])
             / float(gpu.entry["memory.total"]),
             stats,
         )
         bestGPU = min(zip(ids, ratios), key=lambda x: x[1])[0]
         os.environ["CUDA_VISIBLE_DEVICES"] = str(bestGPU)
-    threads = int(
-        np.floor(args.threads / 2)
-    )  # in practice it uses double the specified threads
+    if args.threads > 1:
+        args.threads = int(
+            np.floor(args.threads / 2)
+        )  # in practice it uses double the specified threads
     tf.config.threading.set_intra_op_parallelism_threads(
-        threads
+        args.threads
     )  # limits (and sets) threads used during training
     tf.config.threading.set_inter_op_parallelism_threads(
-        threads
+        args.threads
     )  # this one is needed too.
 
     # allocate gpu memory dynamically
     # gpu_devices = tf.config.experimental.list_physical_devices('GPU')
     # for gpu in gpu_devices:
     #     tf.config.experimental.set_memory_growth(gpu, True)
 
     # update conv+pool iterations based on number of SNPs
     num_conv_iterations = int(np.floor(np.log10(args.num_snps)) - 1)
     if num_conv_iterations < 0:
         num_conv_iterations = 0
 
     # organize pairs of individuals
-    if args.pairs is None:
-        args.pairs = int((args.n * (args.n - 1)) / 2)
-    if args.pairs_encode is None:
-        args.pairs_encode = int((args.n * (args.n - 1)) / 2)
     combinations = list(itertools.combinations(range(args.n), 2))
     combinations = random.sample(combinations, args.pairs)
     combinations_encode = random.sample(combinations, args.pairs_encode)
     combinations = list2dict(combinations)
     combinations_encode = list2dict(combinations_encode)
 
     # load inputs
@@ -438,28 +446,28 @@
     total_sims = len(trees)
 
     # separate training and test data
     train, test = train_test_split(np.arange(total_sims),
                                    test_size=args.hold_out)
 
     # loop through training targets to get mean and sd
-    if os.path.isfile(args.out + "/Train/training_params.npy"):
+    if os.path.isfile(args.out + "/preprocess_params.npy"):
         n, num_snps, meanSig, sdSig = np.load(
-            args.out + "/Train/training_params.npy")
+            args.out + "/preprocess_params.npy")
     else:
         targets = []
         for i in train:
             with open(target_paths[i]) as infile:
                 arr = np.log(float(infile.readline().strip()))
             targets.append(arr)
         meanSig = np.mean(targets)
         sdSig = np.std(targets)
         os.makedirs(args.out + "/Train", exist_ok=True)
         np.save(
-            args.out + "/Train/training_params",
+            args.out + "/preprocess_params",
             [args.n, args.num_snps, meanSig, sdSig]
         )
 
     # make directories
     os.makedirs(os.path.join(args.out,
                              "Train/Targets",
                              str(args.seed)),
@@ -482,15 +490,15 @@
                 exist_ok=True)
     os.makedirs(os.path.join(args.out,
                              "Test/Locs",
                              str(args.seed)),
                 exist_ok=True)
 
     # process
-    load_dl_modules()  # (to get data generator)    
+    load_dl_modules()  # (to get data generator)
     for i in range(total_sims):
         if i in test:
             split = "Test"
         else:
             split = "Train"
         targetfile = os.path.join(
             args.out, split, "Targets", str(args.seed), str(i) + ".target"
@@ -543,20 +551,35 @@
     print("reading input paths", flush=True)
     targets, genos, locs = dict_from_preprocessed(args.out + "/Train/")
     total_sims = len(targets)
 
     # grab n and num_snps from preprocessed dir
     if args.training_mean_sd is None:
         args.n, args.num_snps, meanSig, sdSig = np.load(
-            args.out + "/Train/training_params.npy"
+            args.out + "/preprocess_params.npy"
         )
     else:
         args.n, args.num_snps, meanSid, sdSig = np.load(args.training_mean_sd)
     args.n, args.num_snps = int(args.n), int(args.num_snps)
 
+    # save training params:
+    if args.pairs is None:
+        args.pairs = int((args.n * (args.n - 1)) / 2)
+    if args.pairs_encode is None:
+        args.pairs_encode = int(args.pairs)
+    np.save(
+        args.out + "/Train/training_params_" + str(args.seed),
+        [args.seed,
+         args.max_epochs,
+         args.validation_split,
+         args.learning_rate,
+         args.pairs,
+         args.pairs_encode]
+    )
+
     # split into val,train sets
     sim_ids = np.arange(0, total_sims)
     train, val = train_test_split(sim_ids, test_size=args.validation_split)
     if (
         len(val) * args.num_samples % args.batch_size != 0
         or len(train) * args.num_samples % args.batch_size != 0
     ):
@@ -599,20 +622,25 @@
     return
 
 
 def predict():
     # grab mean and sd from training distribution
     if args.training_mean_sd is None:
         args.n, args.num_snps, meanSig, sdSig = np.load(
-            args.out + "/Train/training_params.npy"
+            args.out + "/preprocess_params.npy"
         )
     else:
         args.n, args.num_snps, meanSid, sdSig = np.load(args.training_mean_sd)
     args.n, args.num_snps = int(args.n), int(args.num_snps)
 
+    # grab num pairs from saved training params
+    params = np.load(args.out + "/Train/training_params_"
+                     + str(args.seed) + ".npy")
+    args.pairs, args.num_pairs = int(params[4]), int(params[5])
+
     # load inputs
     targets, genos, locs = dict_from_preprocessed(args.out + "/Test/")
     total_sims = len(targets)
 
     # organize "partition" to hand to data generator
     partition = {}
     if args.num_pred is None:
@@ -664,20 +692,25 @@
     return
 
 
 def empirical():
     # grab mean and sd from training distribution
     if args.training_mean_sd is None:
         args.n, args.num_snps, meanSig, sdSig = np.load(
-            args.out + "/Train/training_params.npy"
+            args.out + "/preprocess_params.npy"
         )
     else:
         args.n, args.num_snps, meanSid, sdSig = np.load(args.training_mean_sd)
     args.n, args.num_snps = int(args.n), int(args.num_snps)
 
+    # grab num pairs from saved training params
+    params = np.load(args.out + "/Train/training_params_"
+                     + str(args.seed) + ".npy")
+    args.pairs, args.num_pairs = int(params[4]), int(params[5])
+
     # project locs
     locs = read_locs(args.empirical + ".locs")
     locs = np.array(locs)
     if len(locs) != args.n:
         print("length of locs file doesn't match n")
         exit()
     locs = project_locs(locs)
@@ -743,16 +776,17 @@
     ax1 = fig.add_axes([0, 0, 0.4, 1])
     ax1.plot(epochs, val_loss, color="blue", lw=0.5, label="val_loss")
     ax1.set_xlabel("Epoch")
     ax1.plot(epochs, loss, color="red", lw=0.5, label="loss")
     ax1.legend()
     fig.savefig(args.plot_history + "_plot.pdf", bbox_inches="tight")
 
+
 def run():
-    
+
     # main #
     np.random.seed(args.seed)
 
     # pre-process
     if args.preprocess is True:
         print("starting pre-processing pipeline")
         preprocess()
```

### Comparing `dispersenn2-0.0.2/dispersenn2/process_input.py` & `dispersenn2-0.0.3/dispersenn2/process_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.2/dispersenn2/read_input.py` & `dispersenn2-0.0.3/dispersenn2/read_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.2/pyproject.toml` & `dispersenn2-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "disperseNN2"
-version = "0.0.2"
+version = "0.0.3"
 description = "Neural net for estimating dispersal distance"
 authors = ["chriscrsmith <chriscs@uoregon.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 gpustat = "^1.1"
```

### Comparing `dispersenn2-0.0.2/PKG-INFO` & `dispersenn2-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispersenn2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neural net for estimating dispersal distance
 Author: chriscrsmith
 Author-email: chriscs@uoregon.edu
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,11 +21,13 @@
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # disperseNN2
 
 [![Documentation Status](https://readthedocs.org/projects/dispersenn2/badge/?version=latest)](https://dispersenn2.readthedocs.io/en/latest/?badge=latest)
 
-New architecture for estimating dispersal rate from georeferenced SNPs. For details see our preprint (LINK).
+`disperseNN2` is a machine learning framework for predicting &#963;, the expected per generation displacement distance between offspring and their parent(s), from genetic variation data.
+`disperseNN2` replaces our previous method, `disperseNN`, by introducing
+a novel architecture. For details see our preprint (LINK).
 
-For instructions, see the [docs page](https://dispersenn2.readthedocs.io/en/latest/).
+For installation and usage instructions, see the [docs page](https://dispersenn2.readthedocs.io/en/latest/).
```

