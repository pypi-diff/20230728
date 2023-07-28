# Comparing `tmp/tensorneko_util-0.3.0.tar.gz` & `tmp/tensorneko_util-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko_util-0.3.0.tar", last modified: Thu Jul 27 06:17:18 2023, max compression
+gzip compressed data, was "tensorneko_util-0.3.1.tar", last modified: Fri Jul 28 09:05:53 2023, max compression
```

## Comparing `tensorneko_util-0.3.0.tar` & `tensorneko_util-0.3.1.tar`

### file list

```diff
@@ -1,147 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.205324 tensorneko_util-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-27 06:17:18.205324 tensorneko_util-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 06:17:18.205324 tensorneko_util-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/setup_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.153324 tensorneko_util-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.161324 tensorneko_util-0.3.0/src/tensorneko_util/
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.165324 tensorneko_util-0.3.0/src/tensorneko_util/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/audio_lib.py
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/blocking.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/backend/visual_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.165324 tensorneko_util-0.3.0/src/tensorneko_util/debug/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/debug/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.165324 tensorneko_util-0.3.0/src/tensorneko_util/io/
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/_default_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.169324 tensorneko_util-0.3.0/src/tensorneko_util/io/audio/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/audio/audio_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/audio/audio_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2541 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/audio/audio_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.169324 tensorneko_util-0.3.0/src/tensorneko_util/io/hdf5/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/hdf5/hdf5_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/hdf5/hdf5_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.169324 tensorneko_util-0.3.0/src/tensorneko_util/io/image/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/image/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/image/image_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.169324 tensorneko_util-0.3.0/src/tensorneko_util/io/json/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.173324 tensorneko_util-0.3.0/src/tensorneko_util/io/matlab/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/matlab/mat_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/matlab/mat_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.173324 tensorneko_util-0.3.0/src/tensorneko_util/io/pickle/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/pickle/pickle_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/pickle/pickle_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.173324 tensorneko_util-0.3.0/src/tensorneko_util/io/text/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/text/text_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/text/text_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.177324 tensorneko_util-0.3.0/src/tensorneko_util/io/video/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     9333 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6013 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.177324 tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      897 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/yaml_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/yaml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.177324 tensorneko_util-0.3.0/src/tensorneko_util/notebook/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/notebook/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.181324 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/crop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.181324 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/preprocess/video.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.189324 tensorneko_util-0.3.0/src/tensorneko_util/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2787 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/bimap.py
--rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8307 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.189324 tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8674 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/bus.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.189324 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/args.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.193324 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/abstract_seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     4267 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/func.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.193324 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/eval.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/monad.py
--rw-r--r--   0 runner    (1001) docker     (122)     8379 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/option.py
--rw-r--r--   0 runner    (1001) docker     (122)     7123 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/fp/underscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     5483 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/server.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/type.py
--rw-r--r--   0 runner    (1001) docker     (122)     9444 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/util/window_merger.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 06:17:17.000000 tensorneko_util-0.3.0/src/tensorneko_util/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.193324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/color.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.197324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.197324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/web/
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/web/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/multi_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/seaborn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.197324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.157324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.197324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.197324 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (122)   246413 2023-07-27 06:15:07.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css
--rw-r--r--   0 runner    (1001) docker     (122)   979304 2023-07-27 06:15:07.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-27 06:15:07.000000 tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.161324 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-27 06:17:18.000000 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-07-27 06:17:18.000000 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 06:17:18.000000 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-27 06:17:18.000000 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-27 06:17:18.000000 tensorneko_util-0.3.0/src/tensorneko_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:18.201324 tensorneko_util-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-27 06:14:43.000000 tensorneko_util-0.3.0/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 09:05:53.143932 tensorneko_util-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/setup_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.099932 tensorneko_util-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.103932 tensorneko_util-0.3.1/src/tensorneko_util/
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/audio_lib.py
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/backend/visual_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/debug/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/_default_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.107932 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2541 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/hdf5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/hdf5/hdf5_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/image/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/json/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.111932 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/pickle_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/pickle/pickle_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/text/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/toml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/toml/toml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.115932 tensorneko_util-0.3.1/src/tensorneko_util/io/video/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9333 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6013 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/notebook/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.119932 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/crop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.123932 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3861 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/preprocess/video.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2787 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/bimap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1446 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8307 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8674 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.127932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/args.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/abstract_seq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4267 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/seq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9434 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/func.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/eval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/monad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8379 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/option.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7123 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/fp/underscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5483 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9444 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/util/window_merger.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-28 09:05:52.000000 tensorneko_util-0.3.1/src/tensorneko_util/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.131932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/color.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3189 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/multi_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/seaborn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3859 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.099932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.135932 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)   246413 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css
+-rw-r--r--   0 runner    (1001) docker     (122)   979304 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-28 09:03:33.000000 tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.103932 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-28 09:05:53.000000 tensorneko_util-0.3.1/src/tensorneko_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:05:53.139932 tensorneko_util-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-28 09:03:02.000000 tensorneko_util-0.3.1/test/test_version.py
```

### Comparing `tensorneko_util-0.3.0/LICENSE` & `tensorneko_util-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/PKG-INFO` & `tensorneko_util-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko_util
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Utils for Library TensorNeko.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko_util-0.3.0/README.md` & `tensorneko_util-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/setup.py` & `tensorneko_util-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/setup_util.py` & `tensorneko_util-0.3.1/setup_util.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/backend/_tqdm.py` & `tensorneko_util-0.3.1/src/tensorneko_util/backend/_tqdm.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/backend/blocking.py` & `tensorneko_util-0.3.1/src/tensorneko_util/backend/blocking.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/backend/parallel.py` & `tensorneko_util-0.3.1/src/tensorneko_util/backend/parallel.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/backend/visual_lib.py` & `tensorneko_util-0.3.1/src/tensorneko_util/backend/visual_lib.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/debug/parser.py` & `tensorneko_util-0.3.1/src/tensorneko_util/debug/parser.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/_default_backends.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/_default_backends.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/audio/audio_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/audio/audio_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/audio/audio_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/image/image_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/image/image_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/image/image_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_data.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_data.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/json/json_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/json/json_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/matlab/mat_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/matlab/mat_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,27 +24,35 @@
 try:
     from .hdf5 import Hdf5Reader
     h5py_available = True
 except ImportError:
     Hdf5Reader = object
     h5py_available = False
 
+try:
+    from .toml import TomlReader
+    toml_available = True
+except ImportError:
+    TomlReader = object
+    toml_available = False
+
 
 class Reader:
 
     def __init__(self):
         self.image = ImageReader
         self.text = TextReader
         self.json = JsonReader
         self.video = VideoReader
         self.audio = AudioReader
         self.pickle = PickleReader
         self._mat = None
         self._yaml = None
         self._h5 = None
+        self._toml = None
 
     @property
     def mat(self) -> Type[MatReader]:
         if scipy_available:
             if self._mat is None:
                 self._mat = MatReader
             return self._mat
@@ -64,7 +72,16 @@
     def h5(self) -> Type[Hdf5Reader]:
         if h5py_available:
             if self._h5 is None:
                 self._h5 = Hdf5Reader
             return self._h5
         else:
             raise ImportError("To use the hdf5 reader, please install h5py.")
+
+    @property
+    def toml(self) -> Type[TomlReader]:
+        if toml_available:
+            if self._toml is None:
+                self._toml = TomlReader
+            return self._toml
+        else:
+            raise ImportError("To use the toml reader, please install toml.")
```

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/text/text_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/text/text_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/text/text_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_data.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_data.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/video/video_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/video/video_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,27 +24,35 @@
 try:
     from .hdf5 import Hdf5Writer
     h5py_available = True
 except ImportError:
     Hdf5Writer = object
     h5py_available = False
 
+try:
+    from .toml import TomlWriter
+    toml_available = True
+except ImportError:
+    TomlWriter = object
+    toml_available = False
+
 
 class Writer:
 
     def __init__(self):
         self.image = ImageWriter
         self.text = TextWriter
         self.json = JsonWriter
         self.video = VideoWriter
         self.audio = AudioWriter
         self.pickle = PickleWriter
         self._mat = None
         self._yaml = None
         self._h5 = None
+        self._toml = None
 
     @property
     def mat(self) -> Type[MatWriter]:
         if scipy_available:
             if self._mat is None:
                 self._mat = MatWriter
             return self._mat
@@ -64,7 +72,16 @@
     def h5(self) -> Type[Hdf5Writer]:
         if h5py_available:
             if self._h5 is None:
                 self._h5 = Hdf5Writer
             return self._h5
         else:
             raise ImportError("To use the hdf5 writer, please install h5py.")
+
+    @property
+    def toml(self) -> Type[TomlWriter]:
+        if toml_available:
+            if self._toml is None:
+                self._toml = TomlWriter
+            return self._toml
+        else:
+            raise ImportError("To use the toml writer, please install toml.")
```

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/yaml_reader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/io/yaml/yaml_writer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/io/yaml/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/notebook/display.py` & `tensorneko_util-0.3.1/src/tensorneko_util/notebook/display.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/crop.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/_utils.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/_utils.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/abstract_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/anime_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/facexzoo_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/face_detector/opencv_face_detector.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/ffmpeg.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/image.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/image.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/preprocess/video.py` & `tensorneko_util-0.3.1/src/tensorneko_util/preprocess/video.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/__init__.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/average_meter.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/average_meter.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/bimap.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/bimap.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/dispatched_misc.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/dispatcher.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/dispatcher.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/downloader.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/downloader.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/bus.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/bus.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/eventbus/event.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/eventbus/event.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/args.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/args.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/abstract_seq.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/abstract_seq.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/seq.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/seq.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/array/stream.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/array/stream.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/func.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/func.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/eval.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/eval.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/monad/option.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/monad/option.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/fp/underscore.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/fp/underscore.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/misc.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/ref.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/ref.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/server.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/singleton.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/singleton.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/timer.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/timer.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/type.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/util/window_merger.py` & `tensorneko_util-0.3.1/src/tensorneko_util/util/window_merger.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/__init__.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/server.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/image_browser/web/index.html` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/image_browser/web/index.html`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/multi_plots.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/multi_plots.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/tensorboard.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/tensorboard.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/component.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/component.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/server.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/server.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/view.py` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/view.py`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.a66e147e.css`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/assets/index.dd94979e.js`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util/visualization/watcher/web/dist/index.html` & `tensorneko_util-0.3.1/src/tensorneko_util/visualization/watcher/web/dist/index.html`

 * *Files identical despite different names*

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util.egg-info/PKG-INFO` & `tensorneko_util-0.3.1/src/tensorneko_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko-util
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Utils for Library TensorNeko.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko_util-0.3.0/src/tensorneko_util.egg-info/SOURCES.txt` & `tensorneko_util-0.3.1/src/tensorneko_util.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 src/tensorneko_util/io/matlab/mat_writer.py
 src/tensorneko_util/io/pickle/__init__.py
 src/tensorneko_util/io/pickle/pickle_reader.py
 src/tensorneko_util/io/pickle/pickle_writer.py
 src/tensorneko_util/io/text/__init__.py
 src/tensorneko_util/io/text/text_reader.py
 src/tensorneko_util/io/text/text_writer.py
+src/tensorneko_util/io/toml/__init__.py
+src/tensorneko_util/io/toml/toml_reader.py
+src/tensorneko_util/io/toml/toml_writer.py
 src/tensorneko_util/io/video/__init__.py
 src/tensorneko_util/io/video/video_data.py
 src/tensorneko_util/io/video/video_reader.py
 src/tensorneko_util/io/video/video_writer.py
 src/tensorneko_util/io/yaml/__init__.py
 src/tensorneko_util/io/yaml/yaml_reader.py
 src/tensorneko_util/io/yaml/yaml_writer.py
```

### Comparing `tensorneko_util-0.3.0/test/test_version.py` & `tensorneko_util-0.3.1/test/test_version.py`

 * *Files identical despite different names*

