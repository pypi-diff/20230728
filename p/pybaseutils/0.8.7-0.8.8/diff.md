# Comparing `tmp/pybaseutils-0.8.7.tar.gz` & `tmp/pybaseutils-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaseutils-0.8.7.tar", last modified: Wed Jul 26 02:59:07 2023, max compression
+gzip compressed data, was "pybaseutils-0.8.8.tar", last modified: Thu Jul 27 03:37:17 2023, max compression
```

## Comparing `pybaseutils-0.8.7.tar` & `pybaseutils-0.8.8.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.500642 pybaseutils-0.8.7/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.7/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-26 02:59:07.500377 pybaseutils-0.8.7/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.7/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.443905 pybaseutils-0.8.7/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-07-26 02:59:03.000000 pybaseutils-0.8.7/pybaseutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/base64_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.447415 pybaseutils-0.8.7/pybaseutils/base_audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.7/pybaseutils/base_audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4930 2023-07-26 02:31:14.000000 pybaseutils-0.8.7/pybaseutils/base_audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-0.8.7/pybaseutils/base_audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.449377 pybaseutils-0.8.7/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.7/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.7/pybaseutils/config_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.452453 pybaseutils-0.8.7/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.7/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.7/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-0.8.7/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9770 2023-07-19 10:29:03.000000 pybaseutils-0.8.7/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.455471 pybaseutils-0.8.7/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12357 2023-07-26 02:57:35.000000 pybaseutils-0.8.7/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19469 2023-06-30 00:49:35.000000 pybaseutils-0.8.7/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-0.8.7/pybaseutils/demo_nii.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32622 2023-07-24 08:48:54.000000 pybaseutils-0.8.7/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.456167 pybaseutils-0.8.7/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    99197 2023-07-19 08:43:17.000000 pybaseutils-0.8.7/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.7/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.460429 pybaseutils-0.8.7/pybaseutils/maker/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/maker/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5158 2023-07-14 03:43:40.000000 pybaseutils-0.8.7/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-0.8.7/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/maker/maker_voc.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.463760 pybaseutils-0.8.7/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.7/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.465159 pybaseutils-0.8.7/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.7/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.7/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/pycpp/main.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.466341 pybaseutils-0.8.7/pybaseutils/server/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-0.8.7/pybaseutils/server/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-0.8.7/pybaseutils/server/apm_server.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.7/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.7/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.467547 pybaseutils-0.8.7/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.7/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.7/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.7/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.446013 pybaseutils-0.8.7/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-26 02:59:07.000000 pybaseutils-0.8.7/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3945 2023-07-26 02:59:07.000000 pybaseutils-0.8.7/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-07-26 02:59:07.000000 pybaseutils-0.8.7/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.7/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-07-26 02:59:07.000000 pybaseutils-0.8.7/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-07-26 02:59:07.500740 pybaseutils-0.8.7/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.7/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.484453 pybaseutils-0.8.7/test_py/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      610 2023-07-18 02:51:24.000000 pybaseutils-0.8.7/test_py/apm_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.7/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.492830 pybaseutils-0.8.7/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.7/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-0.8.7/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.7/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.7/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.7/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.7/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-0.8.7/test_py/converter/FL3D_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.7/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      982 2023-07-20 09:35:42.000000 pybaseutils-0.8.7/test_py/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-0.8.7/test_py/converter/fatigue_driving.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2320 2023-07-17 02:10:53.000000 pybaseutils-0.8.7/test_py/converter/fdd_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.7/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      453 2023-07-26 02:51:16.000000 pybaseutils-0.8.7/test_py/converter/labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.7/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1259 2023-06-20 02:37:41.000000 pybaseutils-0.8.7/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      519 2023-07-13 03:25:56.000000 pybaseutils-0.8.7/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1291 2023-06-29 02:15:47.000000 pybaseutils-0.8.7/test_py/demo3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.7/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.7/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5086 2023-06-30 02:28:09.000000 pybaseutils-0.8.7/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-0.8.7/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-0.8.7/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.7/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4589 2023-07-17 09:31:14.000000 pybaseutils-0.8.7/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1690 2023-07-24 05:47:50.000000 pybaseutils-0.8.7/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      827 2023-06-30 00:39:21.000000 pybaseutils-0.8.7/test_py/demo_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.7/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.7/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.7/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      803 2023-07-19 10:31:29.000000 pybaseutils-0.8.7/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2949 2023-07-24 09:16:56.000000 pybaseutils-0.8.7/test_py/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3593 2023-06-30 00:54:49.000000 pybaseutils-0.8.7/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2919 2023-07-17 08:48:13.000000 pybaseutils-0.8.7/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.7/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.495267 pybaseutils-0.8.7/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.7/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1863 2023-07-17 02:45:08.000000 pybaseutils-0.8.7/test_py/detector/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-07-11 07:21:57.000000 pybaseutils-0.8.7/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6121 2023-07-18 07:56:37.000000 pybaseutils-0.8.7/test_py/detector/predet_labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.497018 pybaseutils-0.8.7/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.7/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.7/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.7/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-26 02:59:07.499751 pybaseutils-0.8.7/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.7/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.7/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.7/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.7/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.7/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.7/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.7/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.383916 pybaseutils-0.8.8/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.8/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-27 03:37:17.383680 pybaseutils-0.8.8/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.8/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.323702 pybaseutils-0.8.8/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-07-27 01:34:25.000000 pybaseutils-0.8.8/pybaseutils/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.327457 pybaseutils-0.8.8/pybaseutils/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.8/pybaseutils/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7139 2023-07-27 01:53:59.000000 pybaseutils-0.8.8/pybaseutils/audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-0.8.8/pybaseutils/audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9012 2023-07-26 06:40:44.000000 pybaseutils-0.8.8/pybaseutils/audio/vad_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.329172 pybaseutils-0.8.8/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.8/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.8/pybaseutils/config_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.331435 pybaseutils-0.8.8/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.8/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.8/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-0.8.8/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9770 2023-07-19 10:29:03.000000 pybaseutils-0.8.8/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.333834 pybaseutils-0.8.8/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12357 2023-07-26 02:57:35.000000 pybaseutils-0.8.8/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19555 2023-07-26 03:00:02.000000 pybaseutils-0.8.8/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-0.8.8/pybaseutils/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32622 2023-07-24 08:48:54.000000 pybaseutils-0.8.8/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.334373 pybaseutils-0.8.8/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    99197 2023-07-19 08:43:17.000000 pybaseutils-0.8.8/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.8/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.337563 pybaseutils-0.8.8/pybaseutils/maker/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/maker/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5158 2023-07-14 03:43:40.000000 pybaseutils-0.8.8/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-0.8.8/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/maker/maker_voc.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.340422 pybaseutils-0.8.8/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.8/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.341766 pybaseutils-0.8.8/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.8/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.8/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.342811 pybaseutils-0.8.8/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-0.8.8/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-0.8.8/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.8/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.8/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.343919 pybaseutils-0.8.8/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.8/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.8/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.8/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.325559 pybaseutils-0.8.8/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-27 03:37:17.000000 pybaseutils-0.8.8/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3961 2023-07-27 03:37:17.000000 pybaseutils-0.8.8/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-07-27 03:37:17.000000 pybaseutils-0.8.8/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.8/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-07-27 03:37:17.000000 pybaseutils-0.8.8/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-07-27 03:37:17.383998 pybaseutils-0.8.8/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.8/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.360462 pybaseutils-0.8.8/test_py/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      610 2023-07-18 02:51:24.000000 pybaseutils-0.8.8/test_py/apm_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.8/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.377486 pybaseutils-0.8.8/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.8/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-0.8.8/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.8/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.8/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.8/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.8/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-0.8.8/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.8/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      982 2023-07-20 09:35:42.000000 pybaseutils-0.8.8/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-0.8.8/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2320 2023-07-17 02:10:53.000000 pybaseutils-0.8.8/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.8/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      453 2023-07-26 02:51:16.000000 pybaseutils-0.8.8/test_py/converter/labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.8/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1259 2023-06-20 02:37:41.000000 pybaseutils-0.8.8/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      519 2023-07-13 03:25:56.000000 pybaseutils-0.8.8/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1291 2023-06-29 02:15:47.000000 pybaseutils-0.8.8/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.8/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.8/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5086 2023-06-30 02:28:09.000000 pybaseutils-0.8.8/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-0.8.8/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-0.8.8/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.8/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4589 2023-07-17 09:31:14.000000 pybaseutils-0.8.8/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1690 2023-07-24 05:47:50.000000 pybaseutils-0.8.8/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      827 2023-06-30 00:39:21.000000 pybaseutils-0.8.8/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.8/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.8/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.8/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      803 2023-07-19 10:31:29.000000 pybaseutils-0.8.8/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2949 2023-07-24 09:16:56.000000 pybaseutils-0.8.8/test_py/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3593 2023-06-30 00:54:49.000000 pybaseutils-0.8.8/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2919 2023-07-17 08:48:13.000000 pybaseutils-0.8.8/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.8/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.379554 pybaseutils-0.8.8/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.8/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1863 2023-07-17 02:45:08.000000 pybaseutils-0.8.8/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-07-11 07:21:57.000000 pybaseutils-0.8.8/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6121 2023-07-18 07:56:37.000000 pybaseutils-0.8.8/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.381013 pybaseutils-0.8.8/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.8/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.8/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.8/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-27 03:37:17.383146 pybaseutils-0.8.8/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.8/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.8/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.8/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.8/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.8/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.8/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.8/test_py/performance.py
```

### Comparing `pybaseutils-0.8.7/LICENCE` & `pybaseutils-0.8.8/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/PKG-INFO` & `pybaseutils-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.7
+Version: 0.8.8
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.7/README.md` & `pybaseutils-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/base64_utils.py` & `pybaseutils-0.8.8/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/base_audio/pyaudio_utils.py` & `pybaseutils-0.8.8/pybaseutils/audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/batch_utils.py` & `pybaseutils-0.8.8/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.8/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.8/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.8/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/color_utils.py` & `pybaseutils-0.8.8/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/config_utils.py` & `pybaseutils-0.8.8/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/coords_utils.py` & `pybaseutils-0.8.8/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.8/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cvutils/monitor.py` & `pybaseutils-0.8.8/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.8/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.8/pybaseutils/cvutils/video_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.8/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.8/pybaseutils/dataloader/parser_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.8/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.8/pybaseutils/dataloader/parser_voc.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         :param image_dir:
         :return:
         """
         if "." in image_id[0]:
             postfix = ""
         else:
             image_list = glob.glob(os.path.join(image_dir, "*"))
+            # image_list = [file for file in image_list if not file.endswith("json")]
             postfix = os.path.basename(image_list[0]).split(".")[1]
         return postfix
 
     def __get_image_anno_file(self, image_dir, anno_dir, image_id: str, img_postfix):
         """
         :param image_dir:
         :param anno_dir:
```

### Comparing `pybaseutils-0.8.7/pybaseutils/demo_nii.py` & `pybaseutils-0.8.8/pybaseutils/demo_nii.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/file_utils.py` & `pybaseutils-0.8.8/pybaseutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.8/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/font_utils.py` & `pybaseutils-0.8.8/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.8/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.8/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/image_utils.py` & `pybaseutils-0.8.8/pybaseutils/image_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/json_utils.py` & `pybaseutils-0.8.8/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/log.py` & `pybaseutils-0.8.8/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/logger.py` & `pybaseutils-0.8.8/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.8/pybaseutils/maker/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.8/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.8/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.8/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.8/pybaseutils/maker/maker_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.8/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.8/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.8/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.8/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.8/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.8/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.8/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.8/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/plot_utils.py` & `pybaseutils-0.8.8/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.8/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.8/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/server/apm_server.py` & `pybaseutils-0.8.8/pybaseutils/server/apm_server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/setup_config.py` & `pybaseutils-0.8.8/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/thread_utils.py` & `pybaseutils-0.8.8/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/time_utils.py` & `pybaseutils-0.8.8/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.8/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.8/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.8/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/word_utils.py` & `pybaseutils-0.8.8/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/worker.py` & `pybaseutils-0.8.8/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.8/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.8/pybaseutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.7
+Version: 0.8.8
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.7/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.8/pybaseutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 pybaseutils/worker.py
 pybaseutils/yaml_utils.py
 pybaseutils.egg-info/PKG-INFO
 pybaseutils.egg-info/SOURCES.txt
 pybaseutils.egg-info/dependency_links.txt
 pybaseutils.egg-info/not-zip-safe
 pybaseutils.egg-info/top_level.txt
-pybaseutils/base_audio/__init__.py
-pybaseutils/base_audio/audio_utils.py
-pybaseutils/base_audio/pyaudio_utils.py
+pybaseutils/audio/__init__.py
+pybaseutils/audio/audio_utils.py
+pybaseutils/audio/pyaudio_utils.py
+pybaseutils/audio/vad_utils.py
 pybaseutils/cluster/__init__.py
 pybaseutils/cluster/kmean.py
 pybaseutils/cluster/maxmin_distance.py
 pybaseutils/cluster/similarity.py
 pybaseutils/cvutils/__init__.py
 pybaseutils/cvutils/corner_utils.py
 pybaseutils/cvutils/monitor.py
```

### Comparing `pybaseutils-0.8.7/setup.py` & `pybaseutils-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/apm_demo.py` & `pybaseutils-0.8.8/test_py/apm_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/class_names.py` & `pybaseutils-0.8.8/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/AffectNet.py` & `pybaseutils-0.8.8/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.8/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.8/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.8/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/CCPD.py` & `pybaseutils-0.8.8/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.8/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/FL3D_dataset.py` & `pybaseutils-0.8.8/test_py/converter/FL3D_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/TT100K.py` & `pybaseutils-0.8.8/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/convert_labelme2voc.py` & `pybaseutils-0.8.8/test_py/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/fatigue_driving.py` & `pybaseutils-0.8.8/test_py/converter/fatigue_driving.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/fdd_dataset.py` & `pybaseutils-0.8.8/test_py/converter/fdd_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.8/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.8/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.8/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo1.py` & `pybaseutils-0.8.8/test_py/demo1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo2.py` & `pybaseutils-0.8.8/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo3.py` & `pybaseutils-0.8.8/test_py/demo3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_async_await2.py` & `pybaseutils-0.8.8/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_copy_files.py` & `pybaseutils-0.8.8/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.8/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_ffmpy.py` & `pybaseutils-0.8.8/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_get_file_list.py` & `pybaseutils-0.8.8/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_gif.py` & `pybaseutils-0.8.8/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_gif_video.py` & `pybaseutils-0.8.8/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_labelme.py` & `pybaseutils-0.8.8/test_py/demo_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_metrics.py` & `pybaseutils-0.8.8/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_mouse.py` & `pybaseutils-0.8.8/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_pandas.py` & `pybaseutils-0.8.8/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_plot.py` & `pybaseutils-0.8.8/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_standard_image .py` & `pybaseutils-0.8.8/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_standard_video .py` & `pybaseutils-0.8.8/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_taichi.py` & `pybaseutils-0.8.8/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_video.py` & `pybaseutils-0.8.8/test_py/demo_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_video_aije.py` & `pybaseutils-0.8.8/test_py/demo_video_aije.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_voc_crop.py` & `pybaseutils-0.8.8/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_voc_vis.py` & `pybaseutils-0.8.8/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_word_similar.py` & `pybaseutils-0.8.8/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_worker1.py` & `pybaseutils-0.8.8/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/demo_worker2.py` & `pybaseutils-0.8.8/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/detector/demo.py` & `pybaseutils-0.8.8/test_py/detector/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/detector/detect_face_person.py` & `pybaseutils-0.8.8/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/detector/predet_labelme.py` & `pybaseutils-0.8.8/test_py/detector/predet_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/flask_demo/server.py` & `pybaseutils-0.8.8/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-0.8.8/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-0.8.8/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-0.8.8/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/kafka_worker.py` & `pybaseutils-0.8.8/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/men_tracemalloc.py` & `pybaseutils-0.8.8/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.7/test_py/performance.py` & `pybaseutils-0.8.8/test_py/performance.py`

 * *Files identical despite different names*

