# Comparing `tmp/lsg-converter-0.0.5.tar.gz` & `tmp/lsg-converter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsg-converter-0.0.5.tar", last modified: Thu Mar  2 12:27:08 2023, max compression
+gzip compressed data, was "lsg-converter-0.0.6.tar", last modified: Fri Jul 28 17:12:57 2023, max compression
```

## Comparing `lsg-converter-0.0.5.tar` & `lsg-converter-0.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.024614 lsg-converter-0.0.5/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1077 2023-03-02 12:20:29.000000 lsg-converter-0.0.5/LICENSE.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7627 2023-03-02 12:27:08.024614 lsg-converter-0.0.5/PKG-INFO
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7141 2023-03-02 12:20:53.000000 lsg-converter-0.0.5/README.md
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       24 2022-10-31 20:40:24.000000 lsg-converter-0.0.5/lsg_converter/__init__.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/albert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:49:02.000000 lsg-converter-0.0.5/lsg_converter/albert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5308 2022-10-31 16:52:49.000000 lsg-converter-0.0.5/lsg_converter/albert/convert_albert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    36696 2023-03-02 12:18:26.000000 lsg-converter-0.0.5/lsg_converter/albert/modeling_lsg_albert.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/bart/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:49.000000 lsg-converter-0.0.5/lsg_converter/bart/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5413 2022-11-20 15:18:14.000000 lsg-converter-0.0.5/lsg_converter/bart/convert_bart_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39422 2023-03-02 12:18:49.000000 lsg-converter-0.0.5/lsg_converter/bart/modeling_lsg_bart.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/barthez/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:51.000000 lsg-converter-0.0.5/lsg_converter/barthez/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5406 2022-10-31 16:53:17.000000 lsg-converter-0.0.5/lsg_converter/barthez/convert_barthez_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39320 2023-03-02 12:19:04.000000 lsg-converter-0.0.5/lsg_converter/barthez/modeling_lsg_barthez.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/bert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:52.000000 lsg-converter-0.0.5/lsg_converter/bert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5199 2022-10-31 16:53:26.000000 lsg-converter-0.0.5/lsg_converter/bert/convert_bert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45544 2023-03-02 12:19:12.000000 lsg-converter-0.0.5/lsg_converter/bert/modeling_lsg_bert.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/camembert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:54.000000 lsg-converter-0.0.5/lsg_converter/camembert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5126 2022-10-31 16:53:32.000000 lsg-converter-0.0.5/lsg_converter/camembert/convert_camembert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45212 2023-03-02 12:19:17.000000 lsg-converter-0.0.5/lsg_converter/camembert/modeling_lsg_camembert.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     9498 2022-12-19 19:57:11.000000 lsg-converter-0.0.5/lsg_converter/conversion_utils.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3877 2022-11-01 12:15:56.000000 lsg-converter-0.0.5/lsg_converter/converter.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/distilbert/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:55.000000 lsg-converter-0.0.5/lsg_converter/distilbert/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     4846 2022-10-31 16:53:41.000000 lsg-converter-0.0.5/lsg_converter/distilbert/convert_distilbert_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    35071 2023-03-02 12:19:28.000000 lsg-converter-0.0.5/lsg_converter/distilbert/modeling_lsg_distilbert.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      893 2022-07-26 20:06:00.000000 lsg-converter-0.0.5/lsg_converter/dummy_conversion.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/electra/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:57.000000 lsg-converter-0.0.5/lsg_converter/electra/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5332 2022-10-31 16:53:46.000000 lsg-converter-0.0.5/lsg_converter/electra/convert_electra_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44870 2023-03-02 12:19:36.000000 lsg-converter-0.0.5/lsg_converter/electra/modeling_lsg_electra.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/mbart/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:58.000000 lsg-converter-0.0.5/lsg_converter/mbart/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5402 2022-10-31 16:53:54.000000 lsg-converter-0.0.5/lsg_converter/mbart/convert_mbart_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39310 2023-03-02 12:19:44.000000 lsg-converter-0.0.5/lsg_converter/mbart/modeling_lsg_mbart.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter/pegasus/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:00.000000 lsg-converter-0.0.5/lsg_converter/pegasus/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3879 2022-10-31 16:54:01.000000 lsg-converter-0.0.5/lsg_converter/pegasus/convert_pegasus_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    42416 2023-03-02 12:19:52.000000 lsg-converter-0.0.5/lsg_converter/pegasus/modeling_lsg_pegasus.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.024614 lsg-converter-0.0.5/lsg_converter/roberta/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:01.000000 lsg-converter-0.0.5/lsg_converter/roberta/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5073 2022-10-31 16:54:07.000000 lsg-converter-0.0.5/lsg_converter/roberta/convert_roberta_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44897 2023-03-02 12:20:01.000000 lsg-converter-0.0.5/lsg_converter/roberta/modeling_lsg_roberta.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.024614 lsg-converter-0.0.5/lsg_converter/xlm_roberta/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:03.000000 lsg-converter-0.0.5/lsg_converter/xlm_roberta/__init__.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5142 2022-10-31 16:54:13.000000 lsg-converter-0.0.5/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45246 2023-03-02 12:20:09.000000 lsg-converter-0.0.5/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py
-drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-03-02 12:27:08.020614 lsg-converter-0.0.5/lsg_converter.egg-info/
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7627 2023-03-02 12:27:08.000000 lsg-converter-0.0.5/lsg_converter.egg-info/PKG-INFO
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1803 2023-03-02 12:27:08.000000 lsg-converter-0.0.5/lsg_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        1 2023-03-02 12:27:08.000000 lsg-converter-0.0.5/lsg_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       32 2023-03-02 12:27:08.000000 lsg-converter-0.0.5/lsg_converter.egg-info/requires.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       14 2023-03-02 12:27:08.000000 lsg-converter-0.0.5/lsg_converter.egg-info/top_level.txt
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      126 2023-03-02 12:20:37.000000 lsg-converter-0.0.5/pyproject.toml
--rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      672 2023-03-02 12:27:08.024614 lsg-converter-0.0.5/setup.cfg
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1077 2023-03-02 12:20:29.000000 lsg-converter-0.0.6/LICENSE.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/PKG-INFO
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7168 2023-07-28 16:56:26.000000 lsg-converter-0.0.6/README.md
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.855597 lsg-converter-0.0.6/lsg_converter/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       24 2022-10-31 20:40:24.000000 lsg-converter-0.0.6/lsg_converter/__init__.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/albert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:49:02.000000 lsg-converter-0.0.6/lsg_converter/albert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5308 2022-10-31 16:52:49.000000 lsg-converter-0.0.6/lsg_converter/albert/convert_albert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    36914 2023-07-28 15:41:05.000000 lsg-converter-0.0.6/lsg_converter/albert/modeling_lsg_albert.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/bart/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:49.000000 lsg-converter-0.0.6/lsg_converter/bart/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5413 2022-11-20 15:18:14.000000 lsg-converter-0.0.6/lsg_converter/bart/convert_bart_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40250 2023-07-28 15:44:07.000000 lsg-converter-0.0.6/lsg_converter/bart/modeling_lsg_bart.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/barthez/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:51.000000 lsg-converter-0.0.6/lsg_converter/barthez/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5406 2022-10-31 16:53:17.000000 lsg-converter-0.0.6/lsg_converter/barthez/convert_barthez_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    39836 2023-07-28 15:54:24.000000 lsg-converter-0.0.6/lsg_converter/barthez/modeling_lsg_barthez.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/bert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:52.000000 lsg-converter-0.0.6/lsg_converter/bert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5199 2022-10-31 16:53:26.000000 lsg-converter-0.0.6/lsg_converter/bert/convert_bert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45492 2023-07-28 15:48:23.000000 lsg-converter-0.0.6/lsg_converter/bert/modeling_lsg_bert.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/camembert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:54.000000 lsg-converter-0.0.6/lsg_converter/camembert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5126 2022-10-31 16:53:32.000000 lsg-converter-0.0.6/lsg_converter/camembert/convert_camembert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44870 2023-07-28 15:51:36.000000 lsg-converter-0.0.6/lsg_converter/camembert/modeling_lsg_camembert.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     9506 2023-07-28 16:50:20.000000 lsg-converter-0.0.6/lsg_converter/conversion_utils.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3877 2022-11-01 12:15:56.000000 lsg-converter-0.0.6/lsg_converter/converter.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/distilbert/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:55.000000 lsg-converter-0.0.6/lsg_converter/distilbert/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     4846 2022-10-31 16:53:41.000000 lsg-converter-0.0.6/lsg_converter/distilbert/convert_distilbert_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    34352 2023-07-28 16:45:25.000000 lsg-converter-0.0.6/lsg_converter/distilbert/modeling_lsg_distilbert.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      893 2022-07-26 20:06:00.000000 lsg-converter-0.0.6/lsg_converter/dummy_conversion.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/electra/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:57.000000 lsg-converter-0.0.6/lsg_converter/electra/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5332 2022-10-31 16:53:46.000000 lsg-converter-0.0.6/lsg_converter/electra/convert_electra_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45379 2023-07-28 15:22:34.000000 lsg-converter-0.0.6/lsg_converter/electra/modeling_lsg_electra.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/mbart/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:50:58.000000 lsg-converter-0.0.6/lsg_converter/mbart/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5402 2022-10-31 16:53:54.000000 lsg-converter-0.0.6/lsg_converter/mbart/convert_mbart_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    40302 2023-07-28 15:36:34.000000 lsg-converter-0.0.6/lsg_converter/mbart/modeling_lsg_mbart.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/pegasus/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:00.000000 lsg-converter-0.0.6/lsg_converter/pegasus/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     3879 2022-10-31 16:54:01.000000 lsg-converter-0.0.6/lsg_converter/pegasus/convert_pegasus_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    42693 2023-07-28 15:58:33.000000 lsg-converter-0.0.6/lsg_converter/pegasus/modeling_lsg_pegasus.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter/roberta/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:01.000000 lsg-converter-0.0.6/lsg_converter/roberta/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5073 2022-10-31 16:54:07.000000 lsg-converter-0.0.6/lsg_converter/roberta/convert_roberta_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    44672 2023-07-28 16:01:01.000000 lsg-converter-0.0.6/lsg_converter/roberta/modeling_lsg_roberta.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/lsg_converter/xlm_roberta/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        0 2022-10-31 20:51:03.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/__init__.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     5142 2022-10-31 16:54:13.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)    45052 2023-07-28 16:03:37.000000 lsg-converter-0.0.6/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py
+drwxrwxr-x   0 ccondevaux  (1001) ccondevaux  (1001)        0 2023-07-28 17:12:57.859597 lsg-converter-0.0.6/lsg_converter.egg-info/
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     7654 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)     1803 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)        1 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       32 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/requires.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)       14 2023-07-28 17:12:57.000000 lsg-converter-0.0.6/lsg_converter.egg-info/top_level.txt
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      126 2023-07-28 17:02:36.000000 lsg-converter-0.0.6/pyproject.toml
+-rw-rw-r--   0 ccondevaux  (1001) ccondevaux  (1001)      672 2023-07-28 17:12:57.863597 lsg-converter-0.0.6/setup.cfg
```

### Comparing `lsg-converter-0.0.5/LICENSE.txt` & `lsg-converter-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/PKG-INFO` & `lsg-converter-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsg-converter
-Version: 0.0.5
+Version: 0.0.6
 Summary: To convert HuggingFace models to their LSG variant
 Home-page: https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 Author: Charles Condevaux
 Author-email: charles.condevaux@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # LSG Attention: Extrapolation of pretrained Transformers to long sequences
 
 ArXiv [paper](https://arxiv.org/abs/2210.15497) \
 Accepted as a conference paper in PAKDD 2023.
 
 
-Requires `transformers >= 4.23.1`
+Requires `transformers >= 4.29.1`
 
 Optional package to convert models:
 ```bash
 pip install lsg-converter
 ```
 
 * [Compatible models](#compatible-models)
@@ -61,14 +61,15 @@
 | Longformer-base            | 3.22 s/step      | 34.38 Gb                | 32.83 Gb                |
 | BigBird-RoBERTa-base       | 2.85 s/step      | 38.13 Gb                | 38.13 Gb (no effect)    |
 | LSG-RoBERTa 256/0          | 1.40 s/step      | 32.92 Gb                | 24.80 Gb                |
 | LSG-RoBERTa 128/128 (norm) | 1.51 s/step      | 33.80 Gb                | 27.52 Gb                |
 | LSG-RoBERTa 32/32 (norm)   | 1.20 s/step      | 24.53 Gb                | 22.53 Gb                |
 
 
+![attn](img/benchmark.png)
 
 # Convert checkpoint to LSG 
 
 Models can be converted with or without the `lsg-converter` package.
 
 ## With package
```

### Comparing `lsg-converter-0.0.5/README.md` & `lsg-converter-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # LSG Attention: Extrapolation of pretrained Transformers to long sequences
 
 ArXiv [paper](https://arxiv.org/abs/2210.15497) \
 Accepted as a conference paper in PAKDD 2023.
 
 
-Requires `transformers >= 4.23.1`
+Requires `transformers >= 4.29.1`
 
 Optional package to convert models:
 ```bash
 pip install lsg-converter
 ```
 
 * [Compatible models](#compatible-models)
@@ -47,14 +47,15 @@
 | Longformer-base            | 3.22 s/step      | 34.38 Gb                | 32.83 Gb                |
 | BigBird-RoBERTa-base       | 2.85 s/step      | 38.13 Gb                | 38.13 Gb (no effect)    |
 | LSG-RoBERTa 256/0          | 1.40 s/step      | 32.92 Gb                | 24.80 Gb                |
 | LSG-RoBERTa 128/128 (norm) | 1.51 s/step      | 33.80 Gb                | 27.52 Gb                |
 | LSG-RoBERTa 32/32 (norm)   | 1.20 s/step      | 24.53 Gb                | 22.53 Gb                |
 
 
+![attn](img/benchmark.png)
 
 # Convert checkpoint to LSG 
 
 Models can be converted with or without the `lsg-converter` package.
 
 ## With package
```

### Comparing `lsg-converter-0.0.5/lsg_converter/albert/convert_albert_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/albert/convert_albert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/albert/modeling_lsg_albert.py` & `lsg-converter-0.0.6/lsg_converter/albert/modeling_lsg_albert.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,27 +184,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in AlbertModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
+
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
 
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -834,15 +840,14 @@
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
     """
 
     config_class = LSGAlbertConfig
     load_tf_weights = load_tf_weights_in_albert
     base_model_prefix = "albert"
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def _init_weights(self, module):
         """Initialize the weights."""
         if isinstance(module, nn.Linear):
             # Slightly different from the TF version which uses truncated_normal for initialization
             # cf https://github.com/pytorch/pytorch/pull/5617
             module.weight.data.normal_(mean=0.0, std=self.config.initializer_range)
@@ -877,29 +882,31 @@
 
         # Initialize weights and apply final processing
         self.post_init()
 
     
 class LSGAlbertForPreTraining(LSGAlbertPreTrainedModel, AlbertForPreTraining):
 
+    _tied_weights_keys = ["predictions.decoder.bias", "predictions.decoder.weight"]
+
     def __init__(self, config):
 
         LSGAlbertPreTrainedModel.__init__(self, config)
 
         self.albert = LSGAlbertModel(config)
         self.predictions = AlbertMLMHead(config)
         self.sop_classifier = AlbertSOPHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGAlbertForMaskedLM(LSGAlbertPreTrainedModel, AlbertForMaskedLM):
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["predictions.decoder.bias", "predictions.decoder.weight"]
 
     def __init__(self, config):
         LSGAlbertPreTrainedModel.__init__(self, config)
 
         self.albert = LSGAlbertModel(config, add_pooling_layer=False)
         self.predictions = AlbertMLMHead(config)
 
@@ -921,16 +928,14 @@
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGAlbertForTokenClassification(LSGAlbertPreTrainedModel, AlbertForTokenClassification):
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-
     def __init__(self, config):
 
         LSGAlbertPreTrainedModel.__init__(self, config)
         self.num_labels = config.num_labels
 
         self.albert = LSGAlbertModel(config, add_pooling_layer=False)
         classifier_dropout_prob = (
@@ -943,16 +948,14 @@
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGAlbertForQuestionAnswering(LSGAlbertPreTrainedModel, AlbertForQuestionAnswering):
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-
     def __init__(self, config):
 
         LSGAlbertPreTrainedModel.__init__(self, config)
         self.num_labels = config.num_labels
 
         self.albert = LSGAlbertModel(config, add_pooling_layer=False)
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/bart/convert_bart_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/bart/convert_bart_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/bart/modeling_lsg_bart.py` & `lsg-converter-0.0.6/lsg_converter/bart/modeling_lsg_bart.py`

 * *Files 2% similar despite different names*

```diff
@@ -639,14 +639,19 @@
             dropout=config.attention_dropout,
         )
 
         
 class LSGBartPretrainedModel(BartPretrainedModel):
 
     config_class = LSGBartConfig
+    base_model_prefix = "model"
+    supports_gradient_checkpointing = True
+    _keys_to_ignore_on_load_unexpected = ["encoder.version", "decoder.version"]
+    _no_split_modules = [r"BartEncoderLayer", r"BartDecoderLayer"]
+    _skip_keys_device_placement = "past_key_values"
 
     def _set_gradient_checkpointing(self, module, value=False):
 
         if isinstance(module, (BartDecoder, BartEncoder, LSGBartEncoder)):
             module.gradient_checkpointing = value
 
 
@@ -832,16 +837,21 @@
                     f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
                 )
 
         for idx, encoder_layer in enumerate(self.layers):
             if output_hidden_states:
                 encoder_states = encoder_states + (hidden_states,)
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            dropout_probability = random.uniform(0, 1)
-            if self.training and (dropout_probability < self.layerdrop):  # skip the layer
+            to_drop = False
+            if self.training:
+                dropout_probability = torch.rand([])
+                if dropout_probability < self.layerdrop:  # skip the layer
+                    to_drop = True
+
+            if to_drop:
                 layer_outputs = (None, None)
             else:
                 if self.gradient_checkpointing and self.training:
 
                     def create_custom_forward(module):
                         def custom_forward(*inputs):
                             return module(*inputs, output_attentions)
@@ -875,14 +885,16 @@
         return BaseModelOutput(
             last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions
         )
 
 
 class LSGBartModel(LSGBartPretrainedModel, BartModel):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config):
 
         LSGBartPretrainedModel.__init__(self, config)
 
         padding_idx, vocab_size = config.pad_token_id, config.vocab_size
         self.shared = nn.Embedding(vocab_size, config.d_model, padding_idx)
 
@@ -980,29 +992,32 @@
             encoder_attentions=encoder_outputs.attentions,
         )
 
 
 class LSGBartForConditionalGeneration(LSGBartPretrainedModel, BartForConditionalGeneration):
     
     base_model_prefix = "model"
-    _keys_to_ignore_on_load_missing = [r"final_logits_bias", r"lm_head\.weight"]
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight", "lm_head.weight"]
+    _keys_to_ignore_on_load_missing = ["final_logits_bias"]
 
     def __init__(self, config):
 
         LSGBartPretrainedModel.__init__(self, config)
         self.model = LSGBartModel(config)
         self.register_buffer("final_logits_bias", torch.zeros((1, self.model.shared.num_embeddings)))
         self.lm_head = nn.Linear(config.d_model, self.model.shared.num_embeddings, bias=False)
     
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGBartForSequenceClassification(LSGBartPretrainedModel, BartForSequenceClassification):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config: LSGBartConfig, **kwargs):
 
         LSGBartPretrainedModel.__init__(self, config, **kwargs)
         self.model = LSGBartModel(config)
         self.classification_head = BartClassificationHead(
             config.d_model,
             config.d_model,
@@ -1011,14 +1026,16 @@
         )
         self.model._init_weights(self.classification_head.dense)
         self.model._init_weights(self.classification_head.out_proj)
 
 
 class LSGBartForQuestionAnswering(LSGBartPretrainedModel, BartForQuestionAnswering):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config: LSGBartConfig):
 
         LSGBartPretrainedModel.__init__(self, config)
 
         config.num_labels = 2
         self.num_labels = config.num_labels
 
@@ -1026,14 +1043,17 @@
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
 
         self.model._init_weights(self.qa_outputs)
 
 
 class LSGBartForCausalLM(LSGBartPretrainedModel, BartForCausalLM):
 
+    _keys_to_ignore_on_load_missing = ["lm_head.weight"]
+    _tied_weights_keys = ["lm_head.weight"]
+
     def __init__(self, config: LSGBartConfig):
 
         LSGBartPretrainedModel.__init__(self, config)
         BartForCausalLM.__init__(self, config)
 
 
 def str_to_class(classname):
```

### Comparing `lsg-converter-0.0.5/lsg_converter/barthez/convert_barthez_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/barthez/convert_barthez_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/barthez/modeling_lsg_barthez.py` & `lsg-converter-0.0.6/lsg_converter/barthez/modeling_lsg_barthez.py`

 * *Files 2% similar despite different names*

```diff
@@ -641,14 +641,17 @@
 
 
 class LSGMBartPretrainedModel(MBartPreTrainedModel):
 
     config_class = LSGMBartConfig
     base_model_prefix = "model"
     supports_gradient_checkpointing = True
+    _keys_to_ignore_on_load_unexpected = ["encoder.version", "decoder.version"]
+    _no_split_modules = [r"BartEncoderLayer", r"BartDecoderLayer"]
+    _skip_keys_device_placement = "past_key_values"
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (MBartDecoder, MBartEncoder, LSGMBartEncoder)):
             module.gradient_checkpointing = value
 
 
 class LSGMBartEncoder(LSGMBartPretrainedModel, MBartEncoder):
@@ -825,15 +828,15 @@
                     f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
                 )
 
         for idx, encoder_layer in enumerate(self.layers):
             if output_hidden_states:
                 encoder_states = encoder_states + (hidden_states,)
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            dropout_probability = random.uniform(0, 1)
+            dropout_probability = torch.rand([])
             if self.training and (dropout_probability < self.layerdrop):  # skip the layer
                 layer_outputs = (None, None)
             else:
                 if self.gradient_checkpointing and self.training:
 
                     def create_custom_forward(module):
                         def custom_forward(*inputs):
@@ -870,14 +873,16 @@
         return BaseModelOutput(
             last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions
         )
 
 
 class LSGMBartModel(LSGMBartPretrainedModel, MBartModel):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
 
         padding_idx, vocab_size = config.pad_token_id, config.vocab_size
         self.shared = nn.Embedding(vocab_size, config.d_model, padding_idx)
 
@@ -973,34 +978,32 @@
             encoder_attentions=encoder_outputs.attentions,
         )
 
 
 class LSGMBartForConditionalGeneration(LSGMBartPretrainedModel, MBartForConditionalGeneration):
     
     base_model_prefix = "model"
-    _keys_to_ignore_on_load_missing = [
-        r"final_logits_bias",
-        r"encoder.version",
-        r"decoder.version",
-        r"lm_head.weight",
-    ]
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight", "lm_head.weight"]
+    _keys_to_ignore_on_load_missing = ["final_logits_bias"]
 
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
         self.model = LSGMBartModel(config)
         self.register_buffer("final_logits_bias", torch.zeros((1, self.model.shared.num_embeddings)))
         self.lm_head = nn.Linear(config.d_model, self.model.shared.num_embeddings, bias=False)
     
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGMBartForSequenceClassification(LSGMBartPretrainedModel, MBartForSequenceClassification):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config, **kwargs):
 
         LSGMBartPretrainedModel.__init__(self, config, **kwargs)
         self.model = LSGMBartModel(config)
         self.classification_head = MBartClassificationHead(
             config.d_model,
             config.d_model,
@@ -1009,14 +1012,16 @@
         )
         self.model._init_weights(self.classification_head.dense)
         self.model._init_weights(self.classification_head.out_proj)
 
 
 class LSGMBartForQuestionAnswering(LSGMBartPretrainedModel, MBartForQuestionAnswering):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
 
         config.num_labels = 2
         self.num_labels = config.num_labels
 
@@ -1024,14 +1029,16 @@
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
 
         self.model._init_weights(self.qa_outputs)
 
 
 class LSGMBartForCausalLM(LSGMBartPretrainedModel, MBartForCausalLM):
 
+    _tied_weights_keys = ["lm_head.weight"]
+    
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
         MBartForCausalLM.__init__(self, config)
 
 
 def str_to_class(classname):
```

### Comparing `lsg-converter-0.0.5/lsg_converter/bert/convert_bert_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/bert/convert_bert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/bert/modeling_lsg_bert.py` & `lsg-converter-0.0.6/lsg_converter/bert/modeling_lsg_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,27 +185,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in BertModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
+
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
 
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -987,16 +993,14 @@
 
 class LSGBertModel(LSGBertPreTrainedModel, BertModel):
     """
     This class overrides :class:`~transformers.BertModel`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-
     def __init__(self, config, add_pooling_layer=True):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.config = config
 
         self.embeddings = LSGBertEmbeddings(config)
@@ -1027,29 +1031,30 @@
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(extended_attention_mask.dtype).min
 
         return extended_attention_mask
 
 
 class LSGBertForPreTraining(LSGBertPreTrainedModel, BertForPreTraining):
 
+    _tied_weights_keys = ["predictions.decoder.bias", "cls.predictions.decoder.weight"]
+
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.bert = LSGBertModel(config)
         self.cls = BertPreTrainingHeads(config)
         
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGBertLMHeadModel(LSGBertPreTrainedModel, BertLMHeadModel):
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"predictions.decoder.bias"]
+    _tied_weights_keys = ["predictions.decoder.bias", "cls.predictions.decoder.weight"]
 
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         if not config.is_decoder:
             logger.warning("If you want to use `BertLMHeadModel` as a standalone, add `is_decoder=True.`")
@@ -1063,17 +1068,15 @@
 
 class LSGBertForMaskedLM(LSGBertPreTrainedModel, BertForMaskedLM):
     """
     This class overrides :class:`~transformers.BertForMaskedLM`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"predictions.decoder.bias"]
+    _tied_weights_keys = ["predictions.decoder.bias", "cls.predictions.decoder.weight"]
 
     def __init__(self, config):
 
         LSGBertPreTrainedModel.__init__(self, config)
 
         if config.is_decoder:
             logger.warning(
@@ -1103,16 +1106,14 @@
 
 class LSGBertForSequenceClassification(LSGBertPreTrainedModel, BertForSequenceClassification):
     """
     This class overrides :class:`~transformers.BertForSequenceClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
         self.config = config
 
@@ -1129,16 +1130,14 @@
         
 class LSGBertForMultipleChoice(LSGBertPreTrainedModel, BertForMultipleChoice):
     """
     This class overrides :class:`~transformers.BertForMultipleChoice`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.bert = LSGBertModel(config)
         classifier_dropout = (
             config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
@@ -1152,17 +1151,14 @@
 
 class LSGBertForTokenClassification(LSGBertPreTrainedModel, BertForTokenClassification):
     """
     This class overrides :class:`~transformers.BertForTokenClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
 
         self.bert = LSGBertModel(config, add_pooling_layer=False)
@@ -1178,17 +1174,14 @@
 
 class LSGBertForQuestionAnswering(LSGBertPreTrainedModel, BertForQuestionAnswering):
     """
     This class overrides :class:`~transformers.BertForQuestionAnswering`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    config_class = LSGBertConfig
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-
     def __init__(self, config):
         
         LSGBertPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
 
         self.bert = LSGBertModel(config, add_pooling_layer=False)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/camembert/convert_camembert_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/camembert/convert_camembert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/camembert/modeling_lsg_camembert.py` & `lsg-converter-0.0.6/lsg_converter/camembert/modeling_lsg_camembert.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,27 +184,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in CamembertModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
+
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
 
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -970,28 +976,29 @@
 class LSGCamembertPreTrainedModel(CamembertPreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
     """
 
     config_class = LSGCamembertConfig
+    base_model_prefix = "roberta"
+    supports_gradient_checkpointing = True
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (CamembertEncoder, LSGCamembertEncoder)):
             module.gradient_checkpointing = value
 
 
 class LSGCamembertModel(LSGCamembertPreTrainedModel, CamembertModel):
     """
     This class overrides :class:`~transformers.CamembertModel`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    config_class = LSGCamembertConfig
-
+    _no_split_modules = []
 
     def __init__(self, config, add_pooling_layer=True):
         
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         self.embeddings = LSGCamembertEmbeddings(config)
         self.encoder = LSGCamembertEncoder(config)
@@ -1021,17 +1028,15 @@
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(extended_attention_mask.dtype).min
 
         return extended_attention_mask
 
 
 class LSGCamembertForCausalLM(LSGCamembertPreTrainedModel, CamembertForCausalLM):
 
-    _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGCamembertLMHeadModel` as a standalone, add `is_decoder=True.`")
@@ -1048,17 +1053,15 @@
 
 class LSGCamembertForMaskedLM(LSGCamembertPreTrainedModel, CamembertForMaskedLM):
     """
     This class overrides :class:`~transformers.CamembertForMaskedLM`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         if config.is_decoder:
             logger.warning(
@@ -1078,16 +1081,14 @@
 
 class LSGCamembertForSequenceClassification(LSGCamembertPreTrainedModel, CamembertForSequenceClassification):
     """
     This class overrides :class:`~transformers.CamembertForSequenceClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
         self.config = config
 
@@ -1100,16 +1101,14 @@
 
 class LSGCamembertForMultipleChoice(LSGCamembertPreTrainedModel, CamembertForMultipleChoice):
     """
     This class overrides :class:`~transformers.CamembertForMultipleChoice`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         self.roberta = LSGCamembertModel(config)
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
         self.classifier = nn.Linear(config.hidden_size, 1)
@@ -1120,17 +1119,14 @@
 
 class LSGCamembertForTokenClassification(LSGCamembertPreTrainedModel, CamembertForTokenClassification):
     """
     This class overrides :class:`~transformers.CamembertForTokenClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGCamembertPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
 
         self.roberta = LSGCamembertModel(config, add_pooling_layer=False)
@@ -1146,17 +1142,14 @@
 
 class LSGCamembertForQuestionAnswering(LSGCamembertPreTrainedModel, CamembertForQuestionAnswering):
     """
     This class overrides :class:`~transformers.CamembertForQuestionAnswering`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGCamembertPreTrainedModel.__init__(self, config)
         
         self.num_labels = config.num_labels
 
         self.roberta = LSGCamembertModel(config, add_pooling_layer=False)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/conversion_utils.py` & `lsg-converter-0.0.6/lsg_converter/conversion_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         for name in auto_map.keys():
 
             if name == "AutoConfig":
                 continue
 
             model = getattr(sys.modules["transformers"], name)
             print("\n\n" + "="*5 + " " + name + " " + "="*5 + "\n")
-            model = model.from_pretrained(lsg_path, trust_remote_code=True, is_decoder="Causal" in name)
+            model = model.from_pretrained(lsg_path, trust_remote_code=True, is_decoder="Causal" in name).train()
             
             if gradient_checkpointing:
                 model.gradient_checkpointing_enable()
 
             if "QuestionAnswering" in name:
                 tokens = tokenizer("context", long_text, return_tensors="pt", truncation=True)
                 inputs_embeds = torch.randn(1, max_length, hidden_size)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/converter.py` & `lsg-converter-0.0.6/lsg_converter/converter.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/distilbert/convert_distilbert_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/distilbert/convert_distilbert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/distilbert/modeling_lsg_distilbert.py` & `lsg-converter-0.0.6/lsg_converter/distilbert/modeling_lsg_distilbert.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,27 +229,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in RobertaModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
+
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
 
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -773,15 +779,15 @@
             x = torch.nn.functional.pad(x.transpose(-1, -2), (0, pad_length), value=0.).transpose(-1, -2)
             attn_mask = torch.nn.functional.pad(attn_mask, (0, pad_length), value=mask_value)
 
         if self.mask_first_token:
             attn_mask[..., 0] = mask_value
 
         attn_mask = torch.finfo(x.dtype).min*(1 - attn_mask).unsqueeze(1).unsqueeze(1)
-
+        
         encoder_outputs = super().forward(
             x=x,
             attn_mask=attn_mask,
             head_mask=head_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict
@@ -818,44 +824,20 @@
 
         self.embeddings = LSGEmbeddings(config)  # Embeddings
         self.transformer = LSGTransformer(config)  # Encoder
         self.num_global_tokens = config.num_global_tokens
         # Initialize weights and apply final processing
         self.post_init()
 
-    def forward(
-        self,
-        input_ids: Optional[torch.Tensor] = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        head_mask: Optional[torch.Tensor] = None,
-        inputs_embeds: Optional[torch.Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[BaseModelOutput, Tuple[torch.Tensor, ...]]:
-
-        
-        if input_ids is None and inputs_embeds is not None:
-            inputs_embeds = self.embeddings(None, inputs_embeds)
-            if attention_mask is None:
-                n, t, d = inputs_embeds.size()
-                attention_mask = torch.ones(n, t - self.num_global_tokens, device=inputs_embeds.device)
-
-        return super().forward(
-            input_ids=input_ids, 
-            attention_mask=attention_mask, 
-            head_mask=head_mask, 
-            inputs_embeds=inputs_embeds, 
-            output_attentions=output_attentions, 
-            output_hidden_states=output_hidden_states, 
-            return_dict=return_dict
-            )
 
 class LSGDistilBertForMaskedLM(LSGDistilBertPreTrainedModel, DistilBertForMaskedLM):
 
+    _keys_to_ignore_on_load_missing = ["vocab_projector.weight"]
+    _tied_weights_keys = ["vocab_projector.weight"]
+    
     def __init__(self, config):
 
         LSGDistilBertPreTrainedModel.__init__(self, config)
 
         self.activation = get_activation(config.activation)
         
         self.distilbert = LSGDistilBertModel(config)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/dummy_conversion.py` & `lsg-converter-0.0.6/lsg_converter/dummy_conversion.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/electra/convert_electra_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/electra/convert_electra_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/electra/modeling_lsg_electra.py` & `lsg-converter-0.0.6/lsg_converter/electra/modeling_lsg_electra.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,27 +185,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in ElectraModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
 
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
+
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -1047,14 +1053,17 @@
 
 class LSGElectraForMaskedLM(LSGElectraPreTrainedModel, ElectraForMaskedLM):
     """
     This class overrides :class:`~transformers.ElectraForMaskedLM`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
+    _keys_to_ignore_on_load_missing = ["generator_lm_head.weight"]
+    _tied_weights_keys = ["generator_lm_head.weight"]
+
     config_class = LSGElectraConfig
 
     def __init__(self, config):
 
         LSGElectraPreTrainedModel.__init__(self, config)
 
         self.electra = LSGElectraModel(config)
@@ -1104,14 +1113,17 @@
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGElectraForCausalLM(LSGElectraPreTrainedModel, ElectraForCausalLM):
 
+    _keys_to_ignore_on_load_missing = ["generator_lm_head.weight"]
+    _tied_weights_keys = ["generator_lm_head.weight"]
+
     def __init__(self, config):
 
         LSGElectraPreTrainedModel.__init__(self, config)
 
         if not config.is_decoder:
             logger.warning("If you want to use `ElectraForCausalLM` as a standalone, add `is_decoder=True.`")
```

### Comparing `lsg-converter-0.0.5/lsg_converter/mbart/convert_mbart_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/mbart/convert_mbart_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/mbart/modeling_lsg_mbart.py` & `lsg-converter-0.0.6/lsg_converter/mbart/modeling_lsg_mbart.py`

 * *Files 2% similar despite different names*

```diff
@@ -825,16 +825,21 @@
                     f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
                 )
 
         for idx, encoder_layer in enumerate(self.layers):
             if output_hidden_states:
                 encoder_states = encoder_states + (hidden_states,)
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            dropout_probability = random.uniform(0, 1)
-            if self.training and (dropout_probability < self.layerdrop):  # skip the layer
+            to_drop = False
+            if self.training:
+                dropout_probability = torch.rand([])
+                if dropout_probability < self.layerdrop:  # skip the layer
+                    to_drop = True
+
+            if to_drop:
                 layer_outputs = (None, None)
             else:
                 if self.gradient_checkpointing and self.training:
 
                     def create_custom_forward(module):
                         def custom_forward(*inputs):
                             return module(*inputs, output_attentions)
@@ -870,14 +875,17 @@
         return BaseModelOutput(
             last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions
         )
 
 
 class LSGMBartModel(LSGMBartPretrainedModel, MBartModel):
 
+    _keys_to_ignore_on_load_missing = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
 
         padding_idx, vocab_size = config.pad_token_id, config.vocab_size
         self.shared = nn.Embedding(vocab_size, config.d_model, padding_idx)
 
@@ -978,29 +986,35 @@
     
     base_model_prefix = "model"
     _keys_to_ignore_on_load_missing = [
         r"final_logits_bias",
         r"encoder.version",
         r"decoder.version",
         r"lm_head.weight",
+        "encoder.embed_tokens.weight",
+        "decoder.embed_tokens.weight",
     ]
+    _tied_weights_keys = ["model.encoder.embed_tokens.weight", "model.decoder.embed_tokens.weight", "lm_head.weight"]
 
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
         self.model = LSGMBartModel(config)
         self.register_buffer("final_logits_bias", torch.zeros((1, self.model.shared.num_embeddings)))
         self.lm_head = nn.Linear(config.d_model, self.model.shared.num_embeddings, bias=False)
     
         # Initialize weights and apply final processing
         self.post_init()
 
 
 class LSGMBartForSequenceClassification(LSGMBartPretrainedModel, MBartForSequenceClassification):
 
+    _keys_to_ignore_on_load_missing = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+    _tied_weights_keys = ["model.encoder.embed_tokens.weight", "model.decoder.embed_tokens.weight"]
+
     def __init__(self, config, **kwargs):
 
         LSGMBartPretrainedModel.__init__(self, config, **kwargs)
         self.model = LSGMBartModel(config)
         self.classification_head = MBartClassificationHead(
             config.d_model,
             config.d_model,
@@ -1009,14 +1023,17 @@
         )
         self.model._init_weights(self.classification_head.dense)
         self.model._init_weights(self.classification_head.out_proj)
 
 
 class LSGMBartForQuestionAnswering(LSGMBartPretrainedModel, MBartForQuestionAnswering):
 
+    _keys_to_ignore_on_load_missing = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+    _tied_weights_keys = ["model.encoder.embed_tokens.weight", "model.decoder.embed_tokens.weight"]
+
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
 
         config.num_labels = 2
         self.num_labels = config.num_labels
 
@@ -1024,14 +1041,17 @@
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
 
         self.model._init_weights(self.qa_outputs)
 
 
 class LSGMBartForCausalLM(LSGMBartPretrainedModel, MBartForCausalLM):
 
+    _keys_to_ignore_on_load_missing = ["lm_head.weight"]
+    _tied_weights_keys = ["lm_head.weight"]
+
     def __init__(self, config):
 
         LSGMBartPretrainedModel.__init__(self, config)
         MBartForCausalLM.__init__(self, config)
 
 
 def str_to_class(classname):
```

### Comparing `lsg-converter-0.0.5/lsg_converter/pegasus/convert_pegasus_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/pegasus/convert_pegasus_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/pegasus/modeling_lsg_pegasus.py` & `lsg-converter-0.0.6/lsg_converter/pegasus/modeling_lsg_pegasus.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,14 +674,16 @@
             dropout=config.attention_dropout,
         )
 
         
 class LSGPegasusPreTrainedModel(PegasusPreTrainedModel):
 
     config_class = LSGPegasusConfig
+    base_model_prefix = "model"
+    supports_gradient_checkpointing = True
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (PegasusDecoder, PegasusEncoder, LSGPegasusEncoder)):
             module.gradient_checkpointing = value
 
 
 class LSGPegasusEncoder(LSGPegasusPreTrainedModel, PegasusEncoder):
@@ -876,16 +878,21 @@
             assert head_mask.size()[0] == (
                 len(self.layers)
             ), f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
         for idx, encoder_layer in enumerate(self.layers):
             if output_hidden_states:
                 encoder_states = encoder_states + (hidden_states,)
             # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
-            dropout_probability = random.uniform(0, 1)
-            if self.training and (dropout_probability < self.layerdrop):  # skip the layer
+            to_drop = False
+            if self.training:
+                dropout_probability = torch.rand([])
+                if dropout_probability < self.layerdrop:  # skip the layer
+                    to_drop = True
+
+            if to_drop:
                 layer_outputs = (None, None)
             else:
                 if self.gradient_checkpointing and self.training:
 
                     def create_custom_forward(module):
                         def custom_forward(*inputs):
                             return module(*inputs, output_attentions)
@@ -921,14 +928,16 @@
         return BaseModelOutput(
             last_hidden_state=hidden_states, hidden_states=encoder_states, attentions=all_attentions
         )
 
 
 class LSGPegasusModel(LSGPegasusPreTrainedModel, PegasusModel):
 
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight"]
+
     def __init__(self, config: LSGPegasusConfig):
 
         LSGPegasusPreTrainedModel.__init__(self, config)
 
         padding_idx, vocab_size = config.pad_token_id, config.vocab_size
         self.shared = nn.Embedding(vocab_size, config.d_model, padding_idx)
         self.pass_global_tokens_to_decoder = config.pass_global_tokens_to_decoder
@@ -1028,21 +1037,16 @@
             encoder_attentions=encoder_outputs.attentions,
         )
 
 
 class LSGPegasusForConditionalGeneration(LSGPegasusPreTrainedModel, PegasusForConditionalGeneration):
 
     base_model_prefix = "model"
-    _keys_to_ignore_on_load_missing = [
-        r"final_logits_bias",
-        r"encoder\.version",
-        r"decoder\.version",
-        r"lm_head\.weight",
-        r"embed_positions\.weight",
-    ]
+    _keys_to_ignore_on_load_missing = ["final_logits_bias"]
+    _tied_weights_keys = ["encoder.embed_tokens.weight", "decoder.embed_tokens.weight", "lm_head.weight"]
 
     def __init__(self, config: LSGPegasusConfig):
 
         LSGPegasusPreTrainedModel.__init__(self, config)
         self.model = LSGPegasusModel(config)
         self.register_buffer("final_logits_bias", torch.zeros((1, self.model.shared.num_embeddings)))
         self.lm_head = nn.Linear(config.d_model, self.model.shared.num_embeddings, bias=False)
@@ -1061,14 +1065,16 @@
     def __init__(self, config):
         LSGPegasusPreTrainedModel.__init__(self, config)
         PegasusDecoderWrapper.__init__(self, config)
 
 
 class LSGPegasusForCausalLM(LSGPegasusPreTrainedModel, PegasusForCausalLM):
 
+    _tied_weights_keys = ["lm_head.weight"]
+
     def __init__(self, config):
 
         LSGPegasusPreTrainedModel.__init__(self, config)
         config = copy.deepcopy(config)
         config.is_decoder = True
         config.is_encoder_decoder = False
         self.model = LSGPegasusDecoderWrapper(config)
```

### Comparing `lsg-converter-0.0.5/lsg_converter/roberta/convert_roberta_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/roberta/convert_roberta_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/roberta/modeling_lsg_roberta.py` & `lsg-converter-0.0.6/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from logging import warn
 from transformers.models.roberta.modeling_roberta import *
 import torch
 import torch.nn as nn
-from transformers.models.roberta.configuration_roberta import RobertaConfig
+from transformers.models.xlm_roberta.configuration_xlm_roberta import XLMRobertaConfig
 import sys
 
 AUTO_MAP = {
-        "AutoModel": "modeling_lsg_roberta.LSGRobertaModel",
-        "AutoModelForCausalLM": "modeling_lsg_roberta.LSGRobertaForCausalLM",
-        "AutoModelForMaskedLM": "modeling_lsg_roberta.LSGRobertaForMaskedLM",
-        "AutoModelForMultipleChoice": "modeling_lsg_roberta.LSGRobertaForMultipleChoice",
-        "AutoModelForQuestionAnswering": "modeling_lsg_roberta.LSGRobertaForQuestionAnswering",
-        "AutoModelForSequenceClassification": "modeling_lsg_roberta.LSGRobertaForSequenceClassification",
-        "AutoModelForTokenClassification": "modeling_lsg_roberta.LSGRobertaForTokenClassification"
+        "AutoModel": "modeling_lsg_xlm_roberta.LSGXLMRobertaModel",
+        "AutoModelForCausalLM": "modeling_lsg_xlm_roberta.LSGXLMRobertaForCausalLM",
+        "AutoModelForMaskedLM": "modeling_lsg_xlm_roberta.LSGXLMRobertaForMaskedLM",
+        "AutoModelForMultipleChoice": "modeling_lsg_xlm_roberta.LSGXLMRobertaForMultipleChoice",
+        "AutoModelForQuestionAnswering": "modeling_lsg_xlm_roberta.LSGXLMRobertaForQuestionAnswering",
+        "AutoModelForSequenceClassification": "modeling_lsg_xlm_roberta.LSGXLMRobertaForSequenceClassification",
+        "AutoModelForTokenClassification": "modeling_lsg_xlm_roberta.LSGXLMRobertaForTokenClassification"
     }
 
-class LSGRobertaConfig(RobertaConfig):
+class LSGXLMRobertaConfig(XLMRobertaConfig):
     """
     This class overrides :class:`~transformers.RobertaConfig`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
     base_model_prefix = "lsg"
-    model_type = "roberta"
+    model_type = "xlm-roberta"
 
     def __init__(
         self,
         adaptive=True,
         base_model_prefix="lsg",
         block_size=128,
         lsh_num_pre_rounds=1,
@@ -34,15 +34,15 @@
         num_global_tokens=1,
         pool_with_global=True,
         sparse_block_size=128,
         sparsity_factor=2,
         sparsity_type="norm",
         **kwargs
         ):
-        """Constructs LSGRobertaConfig."""
+        """Constructs LSGXLMRobertaConfig."""
         super().__init__(**kwargs)
 
         self.adaptive = adaptive
         self.auto_map = AUTO_MAP
         self.base_model_prefix = base_model_prefix
         self.block_size = block_size
         self.lsh_num_pre_rounds = lsh_num_pre_rounds
@@ -184,27 +184,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in RobertaModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
+
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
 
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -892,15 +898,14 @@
 
 
 class LSGRobertaEncoder(RobertaEncoder):
 
     def __init__(self, config):
 
         super().__init__(config)
-
         self.layer = nn.ModuleList([LSGRobertaLayer(config) for _ in range(config.num_hidden_layers)])
 
         assert hasattr(config, "num_global_tokens")
         self.num_global_tokens = config.num_global_tokens
         self.pad_idx = config.pad_token_id
 
         assert hasattr(config, "block_size") and hasattr(config, "adaptive")
@@ -967,30 +972,30 @@
 
 class LSGRobertaPreTrainedModel(RobertaPreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
     """
 
-    config_class = LSGRobertaConfig
+    config_class = LSGXLMRobertaConfig
+    base_model_prefix = "roberta"
+    supports_gradient_checkpointing = True
+    _no_split_modules = []
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (RobertaEncoder, LSGRobertaEncoder)):
             module.gradient_checkpointing = value
 
 
-class LSGRobertaModel(LSGRobertaPreTrainedModel, RobertaModel):
+class LSGXLMRobertaModel(LSGRobertaPreTrainedModel, RobertaModel):
     """
     This class overrides :class:`~transformers.RobertaModel`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    config_class = LSGRobertaConfig
-
-
     def __init__(self, config, add_pooling_layer=True):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.embeddings = LSGRobertaEmbeddings(config)
         self.encoder = LSGRobertaEncoder(config)
         self.pooler = RobertaPooler(config) if add_pooling_layer else None
@@ -1017,161 +1022,152 @@
 
         extended_attention_mask = extended_attention_mask.to(dtype=self.dtype)  # fp16 compatibility
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(extended_attention_mask.dtype).min
 
         return extended_attention_mask
 
 
-class LSGRobertaForCausalLM(LSGRobertaPreTrainedModel, RobertaForCausalLM):
+class LSGXLMRobertaForCausalLM(LSGRobertaPreTrainedModel, RobertaForCausalLM):
 
-    _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGRobertaLMHeadModel` as a standalone, add `is_decoder=True.`")
 
-        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
 
         # The LM head weights require special treatment only when they are tied with the word embeddings
         self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
+class LSGXLMRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
     """
     This class overrides :class:`~transformers.RobertaForMaskedLM`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
-
+    config_class = LSGXLMRobertaConfig
     _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
     _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
     _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         if config.is_decoder:
             logger.warning(
                 "If you want to use `LSGRobertaForMaskedLM` make sure `config.is_decoder=False` for "
                 "bi-directional self-attention."
             )
 
-        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
         
         # The LM head weights require special treatment only when they are tied with the word embeddings
         self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
+class LSGXLMRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
     """
     This class overrides :class:`~transformers.RobertaForSequenceClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
         self.config = config
 
-        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.classifier = RobertaClassificationHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGRobertaForMultipleChoice(LSGRobertaPreTrainedModel, RobertaForMultipleChoice):
+class LSGXLMRobertaForMultipleChoice(LSGRobertaPreTrainedModel, RobertaForMultipleChoice):
     """
     This class overrides :class:`~transformers.RobertaForMultipleChoice`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
-
+    config_class = LSGXLMRobertaConfig
     _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
-        self.roberta = LSGRobertaModel(config)
+        self.roberta = LSGXLMRobertaModel(config)
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
         self.classifier = nn.Linear(config.hidden_size, 1)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGRobertaForTokenClassification(LSGRobertaPreTrainedModel, RobertaForTokenClassification):
+class LSGXLMRobertaForTokenClassification(LSGRobertaPreTrainedModel, RobertaForTokenClassification):
     """
     This class overrides :class:`~transformers.RobertaForTokenClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
 
-        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         classifier_dropout = (
             config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(classifier_dropout)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGRobertaForQuestionAnswering(LSGRobertaPreTrainedModel, RobertaForQuestionAnswering):
+class LSGXLMRobertaForQuestionAnswering(LSGRobertaPreTrainedModel, RobertaForQuestionAnswering):
     """
     This class overrides :class:`~transformers.RobertaForQuestionAnswering`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
 
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
         
         self.num_labels = config.num_labels
 
-        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 def str_to_class(classname):
     return getattr(sys.modules[__name__], classname)
 
 # Register model in Auto API
 try:
-    LSGRobertaConfig.register_for_auto_class()
+    LSGXLMRobertaConfig.register_for_auto_class()
     for key, value in AUTO_MAP.items():
         str_to_class(value.split(".")[-1]).register_for_auto_class(key)
 except:
     warn("AutoRegister isn't available, you'll have to manually copy modeling.py after .save_pretrained(...).")
     warn("Update to transformers >= 4.23.1 to fix.")
```

### Comparing `lsg-converter-0.0.5/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py` & `lsg-converter-0.0.6/lsg_converter/xlm_roberta/convert_xlm_roberta_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/lsg_converter/xlm_roberta/modeling_lsg_xlm_roberta.py` & `lsg-converter-0.0.6/lsg_converter/roberta/modeling_lsg_roberta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from logging import warn
 from transformers.models.roberta.modeling_roberta import *
 import torch
 import torch.nn as nn
-from transformers.models.xlm_roberta.configuration_xlm_roberta import XLMRobertaConfig
+from transformers.models.roberta.configuration_roberta import RobertaConfig
 import sys
 
 AUTO_MAP = {
-        "AutoModel": "modeling_lsg_xlm_roberta.LSGXLMRobertaModel",
-        "AutoModelForCausalLM": "modeling_lsg_xlm_roberta.LSGXLMRobertaForCausalLM",
-        "AutoModelForMaskedLM": "modeling_lsg_xlm_roberta.LSGXLMRobertaForMaskedLM",
-        "AutoModelForMultipleChoice": "modeling_lsg_xlm_roberta.LSGXLMRobertaForMultipleChoice",
-        "AutoModelForQuestionAnswering": "modeling_lsg_xlm_roberta.LSGXLMRobertaForQuestionAnswering",
-        "AutoModelForSequenceClassification": "modeling_lsg_xlm_roberta.LSGXLMRobertaForSequenceClassification",
-        "AutoModelForTokenClassification": "modeling_lsg_xlm_roberta.LSGXLMRobertaForTokenClassification"
+        "AutoModel": "modeling_lsg_roberta.LSGRobertaModel",
+        "AutoModelForCausalLM": "modeling_lsg_roberta.LSGRobertaForCausalLM",
+        "AutoModelForMaskedLM": "modeling_lsg_roberta.LSGRobertaForMaskedLM",
+        "AutoModelForMultipleChoice": "modeling_lsg_roberta.LSGRobertaForMultipleChoice",
+        "AutoModelForQuestionAnswering": "modeling_lsg_roberta.LSGRobertaForQuestionAnswering",
+        "AutoModelForSequenceClassification": "modeling_lsg_roberta.LSGRobertaForSequenceClassification",
+        "AutoModelForTokenClassification": "modeling_lsg_roberta.LSGRobertaForTokenClassification"
     }
 
-class LSGXLMRobertaConfig(XLMRobertaConfig):
+class LSGRobertaConfig(RobertaConfig):
     """
     This class overrides :class:`~transformers.RobertaConfig`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
     base_model_prefix = "lsg"
-    model_type = "xlm-roberta"
+    model_type = "roberta"
 
     def __init__(
         self,
         adaptive=True,
         base_model_prefix="lsg",
         block_size=128,
         lsh_num_pre_rounds=1,
@@ -34,15 +34,15 @@
         num_global_tokens=1,
         pool_with_global=True,
         sparse_block_size=128,
         sparsity_factor=2,
         sparsity_type="norm",
         **kwargs
         ):
-        """Constructs LSGXLMRobertaConfig."""
+        """Constructs LSGRobertaConfig."""
         super().__init__(**kwargs)
 
         self.adaptive = adaptive
         self.auto_map = AUTO_MAP
         self.base_model_prefix = base_model_prefix
         self.block_size = block_size
         self.lsh_num_pre_rounds = lsh_num_pre_rounds
@@ -184,27 +184,33 @@
         # Take the dot product between "query" and "key" to get the raw attention scores.
         attention_scores = query_layer @ key_layer.transpose(-1, -2) / math.sqrt(d)
 
         del query_layer
         del key_layer
 
         if attention_mask is not None:
-            # Apply the attention mask is (precomputed for all layers in RobertaModel forward() function)
-            attention_scores = attention_scores + attention_mask
-
             # Add causal mask
             causal_shape = (self.block_size, self.block_size) if causal_shape is None else causal_shape
             causal_mask = torch.tril(
                 torch.ones(*causal_shape, device=attention_mask.device, dtype=attention_scores.dtype), 
                 diagonal=-1
                 ) 
-            causal_mask = causal_mask.T * torch.finfo(attention_scores.dtype).min
-            attention_scores[..., -causal_shape[0]:, -causal_shape[1] + 1:] = causal_mask[:, 1:]
+            
+            # Min value
+            dtype_min = torch.tensor(
+                        torch.finfo(attention_scores.dtype).min, device=attention_scores.device, dtype=attention_scores.dtype
+                    )
 
+            # Build causal + attention_mask
+            causal_mask = torch.nn.functional.pad(causal_mask.T * dtype_min, (attention_mask.size()[-1] - self.block_size, 0), value=0)
+            attention_mask = torch.max(attention_mask + causal_mask.unsqueeze(0).unsqueeze(0).unsqueeze(0), dtype_min)
+
+            attention_scores = attention_scores + attention_mask
             del attention_mask
+            del causal_mask
 
         # Normalize the attention scores to probabilities.
         attention_probs = nn.Softmax(dim=-1)(attention_scores)
 
         # This is actually dropping out entire tokens to attend to, which might
         # seem a bit unusual, but is taken from the original Transformer paper.
         context_layer = self.dropout(attention_probs) @ value_layer
@@ -892,14 +898,15 @@
 
 
 class LSGRobertaEncoder(RobertaEncoder):
 
     def __init__(self, config):
 
         super().__init__(config)
+
         self.layer = nn.ModuleList([LSGRobertaLayer(config) for _ in range(config.num_hidden_layers)])
 
         assert hasattr(config, "num_global_tokens")
         self.num_global_tokens = config.num_global_tokens
         self.pad_idx = config.pad_token_id
 
         assert hasattr(config, "block_size") and hasattr(config, "adaptive")
@@ -966,30 +973,30 @@
 
 class LSGRobertaPreTrainedModel(RobertaPreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
     """
 
-    config_class = LSGXLMRobertaConfig
+    config_class = LSGRobertaConfig
+    base_model_prefix = "roberta"
+    supports_gradient_checkpointing = True
+    _no_split_modules = []
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (RobertaEncoder, LSGRobertaEncoder)):
             module.gradient_checkpointing = value
 
 
-class LSGXLMRobertaModel(LSGRobertaPreTrainedModel, RobertaModel):
+class LSGRobertaModel(LSGRobertaPreTrainedModel, RobertaModel):
     """
     This class overrides :class:`~transformers.RobertaModel`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
 
-    config_class = LSGXLMRobertaConfig
-
-
     def __init__(self, config, add_pooling_layer=True):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.embeddings = LSGRobertaEmbeddings(config)
         self.encoder = LSGRobertaEncoder(config)
         self.pooler = RobertaPooler(config) if add_pooling_layer else None
@@ -1016,162 +1023,150 @@
 
         extended_attention_mask = extended_attention_mask.to(dtype=self.dtype)  # fp16 compatibility
         extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(extended_attention_mask.dtype).min
 
         return extended_attention_mask
 
 
-class LSGXLMRobertaForCausalLM(LSGRobertaPreTrainedModel, RobertaForCausalLM):
+class LSGRobertaForCausalLM(LSGRobertaPreTrainedModel, RobertaForCausalLM):
 
-    config_class = LSGXLMRobertaConfig
-    _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         if not config.is_decoder:
             logger.warning("If you want to use `LSGRobertaLMHeadModel` as a standalone, add `is_decoder=True.`")
 
-        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
 
         # The LM head weights require special treatment only when they are tied with the word embeddings
         self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGXLMRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
+class LSGRobertaForMaskedLM(LSGRobertaPreTrainedModel, RobertaForMaskedLM):
     """
     This class overrides :class:`~transformers.RobertaForMaskedLM`. Please check the superclass for the appropriate
     documentation alongside usage examples.
     """
-    config_class = LSGXLMRobertaConfig
-    _keys_to_ignore_on_save = [r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_missing = [r"position_ids", r"lm_head.decoder.weight", r"lm_head.decoder.bias"]
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
+
+    _tied_weights_keys = ["lm_head.decoder.weight", "lm_head.decoder.bias"]
 
     def __init__(self, config):
 
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         if config.is_decoder:
             logger.warning(
                 "If you want to use `LSGRobertaForMaskedLM` make sure `config.is_decoder=False` for "
                 "bi-directional self-attention."
             )
 
-        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.lm_head = RobertaLMHead(config)
         
         # The LM head weights require special treatment only when they are tied with the word embeddings
         self.update_keys_to_ignore(config, ["lm_head.decoder.weight"])
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGXLMRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
+class LSGRobertaForSequenceClassification(LSGRobertaPreTrainedModel, RobertaForSequenceClassification):
     """
     This class overrides :class:`~transformers.RobertaForSequenceClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
-    config_class = LSGXLMRobertaConfig
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
         self.config = config
 
-        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.classifier = RobertaClassificationHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGXLMRobertaForMultipleChoice(LSGRobertaPreTrainedModel, RobertaForMultipleChoice):
+class LSGRobertaForMultipleChoice(LSGRobertaPreTrainedModel, RobertaForMultipleChoice):
     """
     This class overrides :class:`~transformers.RobertaForMultipleChoice`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
-    config_class = LSGXLMRobertaConfig
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
-        self.roberta = LSGXLMRobertaModel(config)
+        self.roberta = LSGRobertaModel(config)
         self.dropout = nn.Dropout(config.hidden_dropout_prob)
         self.classifier = nn.Linear(config.hidden_size, 1)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGXLMRobertaForTokenClassification(LSGRobertaPreTrainedModel, RobertaForTokenClassification):
+class LSGRobertaForTokenClassification(LSGRobertaPreTrainedModel, RobertaForTokenClassification):
     """
     This class overrides :class:`~transformers.RobertaForTokenClassification`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
-    config_class = LSGXLMRobertaConfig
+
     _keys_to_ignore_on_load_unexpected = [r"pooler"]
     _keys_to_ignore_on_load_missing = [r"position_ids"]
 
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
 
         self.num_labels = config.num_labels
 
-        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         classifier_dropout = (
             config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
         )
         self.dropout = nn.Dropout(classifier_dropout)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
-class LSGXLMRobertaForQuestionAnswering(LSGRobertaPreTrainedModel, RobertaForQuestionAnswering):
+class LSGRobertaForQuestionAnswering(LSGRobertaPreTrainedModel, RobertaForQuestionAnswering):
     """
     This class overrides :class:`~transformers.RobertaForQuestionAnswering`. Please check the superclass for the
     appropriate documentation alongside usage examples.
     """
-    config_class = LSGXLMRobertaConfig
-    _keys_to_ignore_on_load_unexpected = [r"pooler"]
-    _keys_to_ignore_on_load_missing = [r"position_ids"]
-
+    
     def __init__(self, config):
         
         LSGRobertaPreTrainedModel.__init__(self, config)
         
         self.num_labels = config.num_labels
 
-        self.roberta = LSGXLMRobertaModel(config, add_pooling_layer=False)
+        self.roberta = LSGRobertaModel(config, add_pooling_layer=False)
         self.qa_outputs = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
 
 def str_to_class(classname):
     return getattr(sys.modules[__name__], classname)
 
 # Register model in Auto API
 try:
-    LSGXLMRobertaConfig.register_for_auto_class()
+    LSGRobertaConfig.register_for_auto_class()
     for key, value in AUTO_MAP.items():
         str_to_class(value.split(".")[-1]).register_for_auto_class(key)
 except:
     warn("AutoRegister isn't available, you'll have to manually copy modeling.py after .save_pretrained(...).")
     warn("Update to transformers >= 4.23.1 to fix.")
```

### Comparing `lsg-converter-0.0.5/lsg_converter.egg-info/PKG-INFO` & `lsg-converter-0.0.6/lsg_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsg-converter
-Version: 0.0.5
+Version: 0.0.6
 Summary: To convert HuggingFace models to their LSG variant
 Home-page: https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 Author: Charles Condevaux
 Author-email: charles.condevaux@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # LSG Attention: Extrapolation of pretrained Transformers to long sequences
 
 ArXiv [paper](https://arxiv.org/abs/2210.15497) \
 Accepted as a conference paper in PAKDD 2023.
 
 
-Requires `transformers >= 4.23.1`
+Requires `transformers >= 4.29.1`
 
 Optional package to convert models:
 ```bash
 pip install lsg-converter
 ```
 
 * [Compatible models](#compatible-models)
@@ -61,14 +61,15 @@
 | Longformer-base            | 3.22 s/step      | 34.38 Gb                | 32.83 Gb                |
 | BigBird-RoBERTa-base       | 2.85 s/step      | 38.13 Gb                | 38.13 Gb (no effect)    |
 | LSG-RoBERTa 256/0          | 1.40 s/step      | 32.92 Gb                | 24.80 Gb                |
 | LSG-RoBERTa 128/128 (norm) | 1.51 s/step      | 33.80 Gb                | 27.52 Gb                |
 | LSG-RoBERTa 32/32 (norm)   | 1.20 s/step      | 24.53 Gb                | 22.53 Gb                |
 
 
+![attn](img/benchmark.png)
 
 # Convert checkpoint to LSG 
 
 Models can be converted with or without the `lsg-converter` package.
 
 ## With package
```

### Comparing `lsg-converter-0.0.5/lsg_converter.egg-info/SOURCES.txt` & `lsg-converter-0.0.6/lsg_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsg-converter-0.0.5/setup.cfg` & `lsg-converter-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lsg-converter
-version = 0.0.5
+version = 0.0.6
 author = Charles Condevaux
 author_email = charles.condevaux@gmail.com
 description = To convert HuggingFace models to their LSG variant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ccdv-ai/convert_checkpoint_to_lsg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
-	transformers>=4.23.1
+	transformers>=4.29.1
 	torch>=1.7
 
 [options.package_data]
 sample = 
 	img/attn.png
 
 [egg_info]
```

