# Comparing `tmp/lycoris_lora-1.8.2.tar.gz` & `tmp/lycoris_lora-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.2.tar", last modified: Thu Jul 27 09:34:23 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.3.tar", last modified: Fri Jul 28 15:13:06 2023, max compression
```

## Comparing `lycoris_lora-1.8.2.tar` & `lycoris_lora-1.8.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.446088 lycoris_lora-1.8.2/
--rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.2/Algo.md
--rw-rw-rw-   0        0        0     1277 2023-07-27 09:31:21.000000 lycoris_lora-1.8.2/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.2/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.2/LICENSE.md
--rw-rw-rw-   0        0        0      348 2023-07-27 09:34:23.445588 lycoris_lora-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     7531 2023-07-27 09:30:40.000000 lycoris_lora-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.422509 lycoris_lora-1.8.2/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.2/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.2/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/experiments/compare_norm.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.2/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.2/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.2/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/experiments/loha_svd.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.2/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.2/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.2/experiments/time_test.py
--rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.2/experiments/weakre_speed.py
--rw-rw-rw-   0        0        0     4110 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/hyperdream_gen_weight.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.423513 lycoris_lora-1.8.2/lycoris/
--rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2672 2023-07-27 02:52:33.000000 lycoris_lora-1.8.2/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.426020 lycoris_lora-1.8.2/lycoris/kohya/
--rw-rw-rw-   0        0        0    42380 2023-07-27 02:15:26.000000 lycoris_lora-1.8.2/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    56362 2023-07-27 09:26:55.000000 lycoris_lora-1.8.2/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    58870 2023-07-27 09:27:06.000000 lycoris_lora-1.8.2/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    20779 2023-07-27 09:28:08.000000 lycoris_lora-1.8.2/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    41085 2023-07-27 03:12:49.000000 lycoris_lora-1.8.2/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/kohya/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.430020 lycoris_lora-1.8.2/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     7334 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/hyperlycoris.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.431019 lycoris_lora-1.8.2/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8228 2023-07-25 10:04:24.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8111 2023-07-25 10:04:17.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    10342 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    10065 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    12654 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/lokr.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.432019 lycoris_lora-1.8.2/lycoris/utils/
--rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/utils/xformers_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.443585 lycoris_lora-1.8.2/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      348 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 09:34:23.446088 lycoris_lora-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-07-27 09:34:17.000000 lycoris_lora-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.444589 lycoris_lora-1.8.2/tools/
--rw-rw-rw-   0        0        0     4087 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/tools/merge.py
--rw-rw-rw-   0        0        0    55484 2023-07-25 09:54:11.000000 lycoris_lora-1.8.2/train_hyperdream.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/
+-rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.3/Algo.md
+-rw-rw-rw-   0        0        0     1277 2023-07-27 09:31:21.000000 lycoris_lora-1.8.3/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.3/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.3/LICENSE.md
+-rw-rw-rw-   0        0        0      348 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7531 2023-07-27 09:30:40.000000 lycoris_lora-1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.382475 lycoris_lora-1.8.3/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.3/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.3/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/experiments/compare_norm.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.3/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.3/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.3/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/experiments/loha_svd.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.3/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.3/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.3/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.3/experiments/weakre_speed.py
+-rw-rw-rw-   0        0        0     4110 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/hyperdream_gen_weight.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.383476 lycoris_lora-1.8.3/lycoris/
+-rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-07-27 02:52:33.000000 lycoris_lora-1.8.3/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.385976 lycoris_lora-1.8.3/lycoris/kohya/
+-rw-rw-rw-   0        0        0    42384 2023-07-28 15:12:31.000000 lycoris_lora-1.8.3/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    56362 2023-07-27 09:26:55.000000 lycoris_lora-1.8.3/lycoris/kohya/model_utils.py
+-rw-rw-rw-   0        0        0    58870 2023-07-27 09:27:06.000000 lycoris_lora-1.8.3/lycoris/kohya/original_unet.py
+-rw-rw-rw-   0        0        0    20779 2023-07-27 09:28:08.000000 lycoris_lora-1.8.3/lycoris/kohya/sdxl_model_util.py
+-rw-rw-rw-   0        0        0    41085 2023-07-27 03:12:49.000000 lycoris_lora-1.8.3/lycoris/kohya/sdxl_original_unet.py
+-rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/kohya/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.389475 lycoris_lora-1.8.3/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     7334 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/hyperlycoris.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.390475 lycoris_lora-1.8.3/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8228 2023-07-25 10:04:24.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     8111 2023-07-25 10:04:17.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/text_encoder.py
+-rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    10342 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    10065 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    12654 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/lokr.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.391976 lycoris_lora-1.8.3/lycoris/utils/
+-rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/utils/xformers_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.404477 lycoris_lora-1.8.3/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-07-28 15:12:43.000000 lycoris_lora-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.404976 lycoris_lora-1.8.3/tools/
+-rw-rw-rw-   0        0        0     4087 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/tools/merge.py
+-rw-rw-rw-   0        0        0    55484 2023-07-25 09:54:11.000000 lycoris_lora-1.8.3/train_hyperdream.py
```

### Comparing `lycoris_lora-1.8.2/.gitignore` & `lycoris_lora-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/Algo.md` & `lycoris_lora-1.8.3/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/Change.md` & `lycoris_lora-1.8.3/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/Demo.md` & `lycoris_lora-1.8.3/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/LICENSE.md` & `lycoris_lora-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/README.md` & `lycoris_lora-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/better_conv.py` & `lycoris_lora-1.8.3/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/better_conv_extract.py` & `lycoris_lora-1.8.3/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/compare_norm.py` & `lycoris_lora-1.8.3/experiments/compare_norm.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/concept_neuron.py` & `lycoris_lora-1.8.3/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/locon_extract_test.py` & `lycoris_lora-1.8.3/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/locon_merge_test.py` & `lycoris_lora-1.8.3/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/loha_svd.py` & `lycoris_lora-1.8.3/experiments/loha_svd.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/singular_value_test.py` & `lycoris_lora-1.8.3/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/sparse_bias_test.py` & `lycoris_lora-1.8.3/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/experiments/time_test.py` & `lycoris_lora-1.8.3/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/hyperdream_gen_weight.py` & `lycoris_lora-1.8.3/hyperdream_gen_weight.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/config.py` & `lycoris_lora-1.8.3/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.3/lycoris/kohya/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         'loha': LohaModule,
         'ia3':  IA3Module,
         'lokr': LokrModule,
         'dylora': DyLoraModule,
         'glora': GLoRAModule,
     }[algo]
     
-    preset = kwargs.get('preset', {})
+    preset = kwargs.get('preset', 'full')
     if preset not in PRESET:
         preset = read_preset(preset)
     else:
         preset = PRESET[preset]
     assert preset is not None
     LycorisNetwork.apply_preset(preset)
```

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/model_utils.py` & `lycoris_lora-1.8.3/lycoris/kohya/model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/original_unet.py` & `lycoris_lora-1.8.3/lycoris/kohya/original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/sdxl_model_util.py` & `lycoris_lora-1.8.3/lycoris/kohya/sdxl_model_util.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/sdxl_original_unet.py` & `lycoris_lora-1.8.3/lycoris/kohya/sdxl_original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/kohya/utils.py` & `lycoris_lora-1.8.3/lycoris/kohya/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/attention.py` & `lycoris_lora-1.8.3/lycoris/modules/attention.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/dylora.py` & `lycoris_lora-1.8.3/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/glokr.py` & `lycoris_lora-1.8.3/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/glora.py` & `lycoris_lora-1.8.3/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/hypernet/generater.py` & `lycoris_lora-1.8.3/lycoris/modules/hypernet/generater.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/hypernet/text_encoder.py` & `lycoris_lora-1.8.3/lycoris/modules/hypernet/text_encoder.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/ia3.py` & `lycoris_lora-1.8.3/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/locon.py` & `lycoris_lora-1.8.3/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/loha.py` & `lycoris_lora-1.8.3/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/modules/lokr.py` & `lycoris_lora-1.8.3/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris/utils/__init__.py` & `lycoris_lora-1.8.3/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.8.3/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/setup.py` & `lycoris_lora-1.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.2',
+    version='1.8.3',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-1.8.2/tools/extract_locon.py` & `lycoris_lora-1.8.3/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/tools/merge.py` & `lycoris_lora-1.8.3/tools/merge.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.2/train_hyperdream.py` & `lycoris_lora-1.8.3/train_hyperdream.py`

 * *Files identical despite different names*

