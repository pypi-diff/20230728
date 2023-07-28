# Comparing `tmp/lsg-converter-0.0.6.tar.gz` & `tmp/lsg-converter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsg-converter-0.0.6.tar", last modified: Fri Jul 28 17:12:57 2023, max compression
+gzip compressed data, was "lsg-converter-0.0.7.tar", last modified: Fri Jul 28 17:46:29 2023, max compression
```

## Comparing `lsg-converter-0.0.6.tar` & `lsg-converter-0.0.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1077 2023-03-02 12:20:29.000000 lsg-converter-0.0.6/LICENSE.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/PKG-INFO
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7168 2023-07-28 16:56:26.000000 lsg-converter-0.0.6/README.md
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.855597 lsg-converter-0.0.6/lsg_converter/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       24 2022-10-31 20:40:24.000000 lsg-converter-0.0.6/lsg_converter/__init__.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/albert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:49:02.000000 lsg-converter-0.0.6/lsg_converter/albert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5308 2022-10-31 16:52:49.000000 lsg-converter-0.0.6/lsg_converter/albert/convert_albert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    36914 2023-07-28 15:41:05.000000 lsg-converter-0.0.6/lsg_converter/albert/modeling_lsg_albert.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/bart/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:49.000000 lsg-converter-0.0.6/lsg_converter/bart/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5413 2022-11-20 15:18:14.000000 lsg-converter-0.0.6/lsg_converter/bart/convert_bart_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40250 2023-07-28 15:44:07.000000 lsg-converter-0.0.6/lsg_converter/bart/modeling_lsg_bart.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/barthez/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:51.000000 lsg-converter-0.0.6/lsg_converter/barthez/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5406 2022-10-31 16:53:17.000000 lsg-converter-0.0.6/lsg_converter/barthez/convert_barthez_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39836 2023-07-28 15:54:24.000000 lsg-converter-0.0.6/lsg_converter/barthez/modeling_lsg_barthez.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/bert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:52.000000 lsg-converter-0.0.6/lsg_converter/bert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5199 2022-10-31 16:53:26.000000 lsg-converter-0.0.6/lsg_converter/bert/convert_bert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45492 2023-07-28 15:48:23.000000 lsg-converter-0.0.6/lsg_converter/bert/modeling_lsg_bert.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/camembert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:54.000000 lsg-converter-0.0.6/lsg_converter/camembert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5126 2022-10-31 16:53:32.000000 lsg-converter-0.0.6/lsg_converter/camembert/convert_camembert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44870 2023-07-28 15:51:36.000000 lsg-converter-0.0.6/lsg_converter/camembert/modeling_lsg_camembert.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     9506 2023-07-28 16:50:20.000000 lsg-converter-0.0.6/lsg_converter/conversion_utils.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3877 2022-11-01 12:15:56.000000 lsg-converter-0.0.6/lsg_converter/converter.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/distilbert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:55.000000 lsg-converter-0.0.6/lsg_converter/distilbert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     4846 2022-10-31 16:53:41.000000 lsg-converter-0.0.6/lsg_converter/distilbert/convert_distilbert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    34352 2023-07-28 16:45:25.000000 lsg-converter-0.0.6/lsg_converter/distilbert/modeling_lsg_distilbert.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      893 2022-07-26 20:06:00.000000 lsg-converter-0.0.6/lsg_converter/dummy_conversion.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/electra/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:57.000000 lsg-converter-0.0.6/lsg_converter/electra/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5332 2022-10-31 16:53:46.000000 lsg-converter-0.0.6/lsg_converter/electra/convert_electra_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45379 2023-07-28 15:22:34.000000 lsg-converter-0.0.6/lsg_converter/electra/modeling_lsg_electra.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/mbart/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:58.000000 lsg-converter-0.0.6/lsg_converter/mbart/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5402 2022-10-31 16:53:54.000000 lsg-converter-0.0.6/lsg_converter/mbart/convert_mbart_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40302 2023-07-28 15:36:34.000000 lsg-converter-0.0.6/lsg_converter/mbart/modeling_lsg_mbart.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/pegasus/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:00.000000 lsg-converter-0.0.6/lsg_converter/pegasus/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3879 2022-10-31 16:54:01.000000 lsg-converter-0.0.6/lsg_converter/pegasus/convert_pegasus_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    42693 2023-07-28 15:58:33.000000 lsg-converter-0.0.6/lsg_converter/pegasus/modeling_lsg_pegasus.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/roberta/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:01.000000 lsg-converter-0.0.6/lsg_converter/roberta/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5073 2022-10-31 16:54:07.000000 lsg-converter-0.0.6/lsg_converter/roberta/convert_roberta_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44672 2023-07-28 16:01:01.000000 lsg-converter-0.0.6/lsg_converter/roberta/modeling_lsg_roberta.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/lsg_converter/xlm_roberta/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:03.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5142 2022-10-31 16:54:13.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45052 2023-07-28 16:03:37.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter.egg-info/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/PKG-INFO
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1803 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        1 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       32 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/requires.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       14 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/top_level.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      126 2023-07-28 17:02:36.000000 lsg-converter-0.0.6/pyproject.toml
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      672 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/setup.cfg
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.927497 lsg-converter-0.0.7/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1077 2023-03-02 12:20:29.000000 lsg-converter-0.0.7/LICENSE.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:46:29.927497 lsg-converter-0.0.7/PKG-INFO
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7168 2023-07-28 16:56:26.000000 lsg-converter-0.0.7/README.md
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       24 2022-10-31 20:40:24.000000 lsg-converter-0.0.7/lsg_converter/__init__.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/albert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:49:02.000000 lsg-converter-0.0.7/lsg_converter/albert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5308 2022-10-31 16:52:49.000000 lsg-converter-0.0.7/lsg_converter/albert/convert_albert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    36914 2023-07-28 15:41:05.000000 lsg-converter-0.0.7/lsg_converter/albert/modeling_lsg_albert.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/bart/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:49.000000 lsg-converter-0.0.7/lsg_converter/bart/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5413 2022-11-20 15:18:14.000000 lsg-converter-0.0.7/lsg_converter/bart/convert_bart_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40250 2023-07-28 15:44:07.000000 lsg-converter-0.0.7/lsg_converter/bart/modeling_lsg_bart.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/barthez/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:51.000000 lsg-converter-0.0.7/lsg_converter/barthez/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5406 2022-10-31 16:53:17.000000 lsg-converter-0.0.7/lsg_converter/barthez/convert_barthez_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39836 2023-07-28 15:54:24.000000 lsg-converter-0.0.7/lsg_converter/barthez/modeling_lsg_barthez.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/bert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:52.000000 lsg-converter-0.0.7/lsg_converter/bert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5199 2022-10-31 16:53:26.000000 lsg-converter-0.0.7/lsg_converter/bert/convert_bert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45492 2023-07-28 15:48:23.000000 lsg-converter-0.0.7/lsg_converter/bert/modeling_lsg_bert.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/camembert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:54.000000 lsg-converter-0.0.7/lsg_converter/camembert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5126 2022-10-31 16:53:32.000000 lsg-converter-0.0.7/lsg_converter/camembert/convert_camembert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44509 2023-07-28 17:44:27.000000 lsg-converter-0.0.7/lsg_converter/camembert/modeling_lsg_camembert.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     9506 2023-07-28 16:50:20.000000 lsg-converter-0.0.7/lsg_converter/conversion_utils.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3877 2022-11-01 12:15:56.000000 lsg-converter-0.0.7/lsg_converter/converter.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/distilbert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:55.000000 lsg-converter-0.0.7/lsg_converter/distilbert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     4846 2022-10-31 16:53:41.000000 lsg-converter-0.0.7/lsg_converter/distilbert/convert_distilbert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    34352 2023-07-28 16:45:25.000000 lsg-converter-0.0.7/lsg_converter/distilbert/modeling_lsg_distilbert.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      893 2022-07-26 20:06:00.000000 lsg-converter-0.0.7/lsg_converter/dummy_conversion.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/electra/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:57.000000 lsg-converter-0.0.7/lsg_converter/electra/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5332 2022-10-31 16:53:46.000000 lsg-converter-0.0.7/lsg_converter/electra/convert_electra_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45379 2023-07-28 15:22:34.000000 lsg-converter-0.0.7/lsg_converter/electra/modeling_lsg_electra.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/mbart/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:58.000000 lsg-converter-0.0.7/lsg_converter/mbart/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5402 2022-10-31 16:53:54.000000 lsg-converter-0.0.7/lsg_converter/mbart/convert_mbart_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40302 2023-07-28 15:36:34.000000 lsg-converter-0.0.7/lsg_converter/mbart/modeling_lsg_mbart.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/pegasus/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:00.000000 lsg-converter-0.0.7/lsg_converter/pegasus/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3879 2022-10-31 16:54:01.000000 lsg-converter-0.0.7/lsg_converter/pegasus/convert_pegasus_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    42693 2023-07-28 15:58:33.000000 lsg-converter-0.0.7/lsg_converter/pegasus/modeling_lsg_pegasus.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter/roberta/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:01.000000 lsg-converter-0.0.7/lsg_converter/roberta/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5073 2022-10-31 16:54:07.000000 lsg-converter-0.0.7/lsg_converter/roberta/convert_roberta_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44310 2023-07-28 17:38:57.000000 lsg-converter-0.0.7/lsg_converter/roberta/modeling_lsg_roberta.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.927497 lsg-converter-0.0.7/lsg_converter/xlm_roberta/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:03.000000 lsg-converter-0.0.7/lsg_converter/xlm_roberta/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5142 2022-10-31 16:54:13.000000 lsg-converter-0.0.7/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44690 2023-07-28 17:39:18.000000 lsg-converter-0.0.7/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:46:29.923497 lsg-converter-0.0.7/lsg_converter.egg-info/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:46:29.000000 lsg-converter-0.0.7/lsg_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1803 2023-07-28 17:46:29.000000 lsg-converter-0.0.7/lsg_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        1 2023-07-28 17:46:29.000000 lsg-converter-0.0.7/lsg_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       32 2023-07-28 17:46:29.000000 lsg-converter-0.0.7/lsg_converter.egg-info/requires.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       14 2023-07-28 17:46:29.000000 lsg-converter-0.0.7/lsg_converter.egg-info/top_level.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      126 2023-07-28 17:02:36.000000 lsg-converter-0.0.7/pyproject.toml
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      672 2023-07-28 17:46:29.927497 lsg-converter-0.0.7/setup.cfg
```

### Comparing `lsg-converter-0.0.6/LICENSE.txt` & `lsg-converter-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/PKG-INFO` & `lsg-converter-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsg-converter
-Version: 0.0.6
+Version: 0.0.7
 Summary: To convert HuggingFace models to their LSG variant
 Home-page: https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 Author: Charles Condevaux
 Author-email: charles.condevaux@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsg-converter-0.0.6/README.md` & `lsg-converter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/albert/convert_albert_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/albert/convert_albert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/albert/modeling_lsg_albert.py` & `lsg-converter-0.0.7/lsg_converter/albert/modeling_lsg_albert.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/bart/convert_bart_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/bart/convert_bart_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/bart/modeling_lsg_bart.py` & `lsg-converter-0.0.7/lsg_converter/bart/modeling_lsg_bart.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/barthez/convert_barthez_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/barthez/convert_barthez_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/barthez/modeling_lsg_barthez.py` & `lsg-converter-0.0.7/lsg_converter/barthez/modeling_lsg_barthez.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/bert/convert_bert_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/bert/convert_bert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/bert/modeling_lsg_bert.py` & `lsg-converter-0.0.7/lsg_converter/bert/modeling_lsg_bert.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/camembert/convert_camembert_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/camembert/convert_camembert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/camembert/modeling_lsg_camembert.py` & `lsg-converter-0.0.7/lsg_converter/camembert/modeling_lsg_camembert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1040,16 +1040,14 @@
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGCamembertLMHeadModel` as a standalone, add `is_decoder=True.`")
 
         self.roberta = LSGCamembertModel(config, add_pooling_layer=False)
         self.lm_head = CamembertLMHead(config)
 
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGCamembertForMaskedLM(LSGCamembertPreTrainedModel, CamembertForMaskedLM):
     """
@@ -1067,17 +1065,14 @@
             logger.warning(
                 "If you want to use `LSGCamembertForMaskedLM` make sure `config.is_decoder=False` for "
                 "bi-directional self-attention."
             )
 
         self.roberta = LSGCamembertModel(config, add_pooling_layer=False)
         self.lm_head = CamembertLMHead(config)
-        
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGCamembertForSequenceClassification(LSGCamembertPreTrainedModel, CamembertForSequenceClassification):
     """
```

### Comparing `lsg-converter-0.0.6/lsg_converter/conversion_utils.py` & `lsg-converter-0.0.7/lsg_converter/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/converter.py` & `lsg-converter-0.0.7/lsg_converter/converter.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/distilbert/convert_distilbert_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/distilbert/convert_distilbert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/distilbert/modeling_lsg_distilbert.py` & `lsg-converter-0.0.7/lsg_converter/distilbert/modeling_lsg_distilbert.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/dummy_conversion.py` & `lsg-converter-0.0.7/lsg_converter/dummy_conversion.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/electra/convert_electra_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/electra/convert_electra_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/electra/modeling_lsg_electra.py` & `lsg-converter-0.0.7/lsg_converter/electra/modeling_lsg_electra.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/mbart/convert_mbart_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/mbart/convert_mbart_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/mbart/modeling_lsg_mbart.py` & `lsg-converter-0.0.7/lsg_converter/mbart/modeling_lsg_mbart.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/pegasus/convert_pegasus_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/pegasus/convert_pegasus_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/pegasus/modeling_lsg_pegasus.py` & `lsg-converter-0.0.7/lsg_converter/pegasus/modeling_lsg_pegasus.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/roberta/convert_roberta_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/roberta/convert_roberta_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/roberta/modeling_lsg_roberta.py` & `lsg-converter-0.0.7/lsg_converter/roberta/modeling_lsg_roberta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1037,17 +1037,14 @@
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGRobertaLMHeadModel` as a standalone, add `is_decoder=True.`")
 
         self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
 
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
-
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
     """
     This class overrides :class:`~transformers.RobertaForMaskedLM`. Please check the superclass for the appropriate
@@ -1064,17 +1061,14 @@
             logger.warning(
                 "If you want to use `LSGRobertaForMaskedLM` make sure `config.is_decoder=False` for "
                 "bi-directional self-attention."
             )
 
         self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
-        
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
     """
```

### Comparing `lsg-converter-0.0.6/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py` & `lsg-converter-0.0.7/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py` & `lsg-converter-0.0.7/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1036,17 +1036,14 @@
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGRobertaLMHeadModel` as a standalone, add `is_decoder=True.`")
 
         self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
 
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
-
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGXLMRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
     """
     This class overrides :class:`~transformers.RobertaForMaskedLM`. Please check the superclass for the appropriate
@@ -1066,17 +1063,14 @@
             logger.warning(
                 "If you want to use `LSGRobertaForMaskedLM` make sure `config.is_decoder=False` for "
                 "bi-directional self-attention."
             )
 
         self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
-        
-        # The LM head weights require special treatment only when they are tied with the word embeddings
-        self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGXLMRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
     """
```

### Comparing `lsg-converter-0.0.6/lsg_converter.egg-info/PKG-INFO` & `lsg-converter-0.0.7/lsg_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsg-converter
-Version: 0.0.6
+Version: 0.0.7
 Summary: To convert HuggingFace models to their LSG variant
 Home-page: https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 Author: Charles Condevaux
 Author-email: charles.condevaux@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsg-converter-0.0.6/lsg_converter.egg-info/SOURCES.txt` & `lsg-converter-0.0.7/lsg_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.6/setup.cfg` & `lsg-converter-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lsg-converter
-version = 0.0.6
+version = 0.0.7
 author = Charles Condevaux
 author_email = charles.condevaux@gmail.com
 description = To convert HuggingFace models to their LSG variant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 classifiers =
```

