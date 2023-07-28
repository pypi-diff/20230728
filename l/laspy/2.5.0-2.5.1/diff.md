# Comparing `tmp/laspy-2.5.0.tar.gz` & `tmp/laspy-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laspy-2.5.0.tar", last modified: Sun Jul 23 18:51:31 2023, max compression
+gzip compressed data, was "laspy-2.5.1.tar", last modified: Fri Jul 28 21:18:02 2023, max compression
```

## Comparing `laspy-2.5.0.tar` & `laspy-2.5.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.621985 laspy-2.5.0/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1538 2021-12-18 17:55:00.000000 laspy-2.5.0/LICENSE.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       65 2022-06-28 22:25:20.000000 laspy-2.5.0/MANIFEST.in
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2764 2023-07-23 18:51:31.621985 laspy-2.5.0/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1915 2022-09-04 19:53:14.000000 laspy-2.5.0/README.md
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.597985 laspy-2.5.0/laspy/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      811 2023-07-23 17:16:38.000000 laspy-2.5.0/laspy/__init__.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.600985 laspy-2.5.0/laspy/_compression/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_compression/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2427 2023-04-19 21:00:42.000000 laspy-2.5.0/laspy/_compression/backend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      461 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_compression/format.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4325 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/_compression/laszipbackend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      932 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/_compression/lazbackend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     9754 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/_compression/lazrsbackend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8272 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_compression/selection.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      254 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_pointappender.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      613 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_pointreader.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      920 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/_pointwriter.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.600985 laspy-2.5.0/laspy/cli/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5749 2023-07-10 08:39:10.000000 laspy-2.5.0/laspy/cli/copc.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      410 2023-07-10 09:37:23.000000 laspy-2.5.0/laspy/cli/main.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      307 2023-04-17 20:35:19.000000 laspy-2.5.0/laspy/compression.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    28560 2023-06-24 07:08:30.000000 laspy-2.5.0/laspy/copc.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      351 2021-12-18 17:55:00.000000 laspy-2.5.0/laspy/errors.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1449 2021-12-18 17:55:00.000000 laspy-2.5.0/laspy/extradims.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      723 2021-12-18 17:55:00.000000 laspy-2.5.0/laspy/file.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    32940 2023-07-14 10:23:23.000000 laspy-2.5.0/laspy/header.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4732 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/lasappender.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    14482 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/lasdata.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1691 2021-12-18 17:55:00.000000 laspy-2.5.0/laspy/lasmmap.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13509 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/lasreader.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6877 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/laswriter.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12984 2023-06-24 05:55:29.000000 laspy-2.5.0/laspy/lib.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.601985 laspy-2.5.0/laspy/point/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       97 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/point/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    24032 2023-06-24 07:08:30.000000 laspy-2.5.0/laspy/point/dims.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     9023 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/point/format.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      462 2022-12-04 00:00:55.000000 laspy-2.5.0/laspy/point/packing.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13472 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/point/record.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)       77 2021-12-18 17:55:00.000000 laspy-2.5.0/laspy/typehints.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4402 2022-12-04 00:00:55.000000 laspy-2.5.0/laspy/utils.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.602985 laspy-2.5.0/laspy/vlrs/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       75 2022-05-01 12:07:55.000000 laspy-2.5.0/laspy/vlrs/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7403 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/vlrs/geotiff.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    21984 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/vlrs/known.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2184 2023-04-15 15:38:48.000000 laspy-2.5.0/laspy/vlrs/vlr.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7077 2023-04-19 20:29:59.000000 laspy-2.5.0/laspy/vlrs/vlrlist.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.598985 laspy-2.5.0/laspy.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2764 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2144 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       46 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/entry_points.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2021-12-18 17:55:18.000000 laspy-2.5.0/laspy.egg-info/not-zip-safe
--rw-r--r--   0 thomas    (1000) thomas    (1000)      246 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        6 2023-07-23 18:51:31.000000 laspy-2.5.0/laspy.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      124 2023-04-19 20:29:59.000000 laspy-2.5.0/pyproject.toml
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-07-23 18:51:31.622985 laspy-2.5.0/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1847 2023-07-10 08:39:10.000000 laspy-2.5.0/setup.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.607985 laspy-2.5.0/tests/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/__init__.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.607985 laspy-2.5.0/tests/cli/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3062 2023-07-10 09:37:23.000000 laspy-2.5.0/tests/cli/test_info.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3805 2023-05-08 18:05:24.000000 laspy-2.5.0/tests/conftest.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-23 18:51:31.620985 laspy-2.5.0/tests/data/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    32381 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/1_4_w_evlr.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8948 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/1_4_w_evlr.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4962 2022-04-24 11:45:17.000000 laspy-2.5.0/tests/data/autzen.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4970 2023-02-22 10:26:26.000000 laspy-2.5.0/tests/data/autzen_geo_proj.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)   603353 2022-12-04 00:00:55.000000 laspy-2.5.0/tests/data/autzen_trim.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    29084 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/extra.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    66354 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/extrabytes.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)   763642 2023-06-24 07:08:30.000000 laspy-2.5.0/tests/data/file_with_both_wkt_and_geotiff_vlrs.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)    59344 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/plane.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    33684 2022-12-04 00:00:55.000000 laspy-2.5.0/tests/data/simple.copc.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    36437 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/simple.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)    18217 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/simple.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    30047 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/simple1_1.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)    62888 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/simple1_3.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)   814388 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/simple1_4.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)    33716 2023-06-24 07:08:30.000000 laspy-2.5.0/tests/data/simple_with_page.copc.laz
--rw-r--r--   0 thomas    (1000) thomas    (1000)    32305 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/test1_4.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)      511 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/unregistered_extra_bytes.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)   299359 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/data/vegetation_1_3.las
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5237 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_append_mode.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3873 2022-12-04 00:00:55.000000 laspy-2.5.0/tests/test_chunk_read_write.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12128 2023-07-10 17:05:57.000000 laspy-2.5.0/tests/test_common.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1171 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_constants.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      859 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_conversion.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6005 2023-06-24 07:08:30.000000 laspy-2.5.0/tests/test_copc.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4696 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_creation.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6255 2023-06-24 07:08:30.000000 laspy-2.5.0/tests/test_crs.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    12315 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_extrabytes.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5197 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_field_views.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10969 2023-07-14 10:23:23.000000 laspy-2.5.0/tests/test_header.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      443 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_las_1_1.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    25434 2022-12-04 00:00:55.000000 laspy-2.5.0/tests/test_laspy.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      284 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_mmap.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1822 2023-04-17 21:23:04.000000 laspy-2.5.0/tests/test_modif_1_2.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1531 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_modif_1_4.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2891 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_non_seekable.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      486 2021-12-18 17:55:00.000000 laspy-2.5.0/tests/test_point_format.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5666 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_reading_1_2.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7534 2023-04-19 20:29:59.000000 laspy-2.5.0/tests/test_reading_1_4.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2344 2022-12-04 00:00:55.000000 laspy-2.5.0/tests/test_vlrs.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.575616 laspy-2.5.1/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1538 2021-12-18 17:55:00.000000 laspy-2.5.1/LICENSE.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       65 2022-06-28 22:25:20.000000 laspy-2.5.1/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2764 2023-07-28 21:18:02.575616 laspy-2.5.1/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1915 2023-07-25 21:37:04.000000 laspy-2.5.1/README.md
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.534616 laspy-2.5.1/laspy/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      811 2023-07-28 21:17:09.000000 laspy-2.5.1/laspy/__init__.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.538616 laspy-2.5.1/laspy/_compression/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_compression/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2427 2023-04-19 21:00:42.000000 laspy-2.5.1/laspy/_compression/backend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      461 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_compression/format.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4325 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/_compression/laszipbackend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      932 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/_compression/lazbackend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     9754 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/_compression/lazrsbackend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8272 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_compression/selection.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      254 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_pointappender.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      613 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_pointreader.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      920 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/_pointwriter.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.538616 laspy-2.5.1/laspy/cli/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5749 2023-07-10 08:39:10.000000 laspy-2.5.1/laspy/cli/copc.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      410 2023-07-10 09:37:23.000000 laspy-2.5.1/laspy/cli/main.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      307 2023-04-17 20:35:19.000000 laspy-2.5.1/laspy/compression.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    28560 2023-06-24 07:08:30.000000 laspy-2.5.1/laspy/copc.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      351 2021-12-18 17:55:00.000000 laspy-2.5.1/laspy/errors.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1449 2021-12-18 17:55:00.000000 laspy-2.5.1/laspy/extradims.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      723 2021-12-18 17:55:00.000000 laspy-2.5.1/laspy/file.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    32940 2023-07-14 10:23:23.000000 laspy-2.5.1/laspy/header.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4732 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/lasappender.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    14482 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/lasdata.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1691 2021-12-18 17:55:00.000000 laspy-2.5.1/laspy/lasmmap.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13509 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/lasreader.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6877 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/laswriter.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12984 2023-06-24 05:55:29.000000 laspy-2.5.1/laspy/lib.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.540616 laspy-2.5.1/laspy/point/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       97 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/point/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    24032 2023-06-24 07:08:30.000000 laspy-2.5.1/laspy/point/dims.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     9023 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/point/format.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      462 2022-12-04 00:00:55.000000 laspy-2.5.1/laspy/point/packing.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13472 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/point/record.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       77 2021-12-18 17:55:00.000000 laspy-2.5.1/laspy/typehints.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4402 2022-12-04 00:00:55.000000 laspy-2.5.1/laspy/utils.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.541616 laspy-2.5.1/laspy/vlrs/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       75 2022-05-01 12:07:55.000000 laspy-2.5.1/laspy/vlrs/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7403 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/vlrs/geotiff.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    21984 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/vlrs/known.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2184 2023-04-15 15:38:48.000000 laspy-2.5.1/laspy/vlrs/vlr.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7077 2023-04-19 20:29:59.000000 laspy-2.5.1/laspy/vlrs/vlrlist.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.536616 laspy-2.5.1/laspy.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2764 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2144 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       46 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/entry_points.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2021-12-18 17:55:18.000000 laspy-2.5.1/laspy.egg-info/not-zip-safe
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      246 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        6 2023-07-28 21:18:02.000000 laspy-2.5.1/laspy.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      124 2023-04-19 20:29:59.000000 laspy-2.5.1/pyproject.toml
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-07-28 21:18:02.575616 laspy-2.5.1/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1847 2023-07-25 21:37:04.000000 laspy-2.5.1/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.548616 laspy-2.5.1/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/__init__.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.548616 laspy-2.5.1/tests/cli/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3212 2023-07-28 21:17:09.000000 laspy-2.5.1/tests/cli/test_info.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3805 2023-05-08 18:05:24.000000 laspy-2.5.1/tests/conftest.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 21:18:02.572615 laspy-2.5.1/tests/data/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    32381 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/1_4_w_evlr.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8948 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/1_4_w_evlr.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4962 2022-04-24 11:45:17.000000 laspy-2.5.1/tests/data/autzen.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4970 2023-02-22 10:26:26.000000 laspy-2.5.1/tests/data/autzen_geo_proj.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)   603353 2022-12-04 00:00:55.000000 laspy-2.5.1/tests/data/autzen_trim.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    29084 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/extra.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    66354 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/extrabytes.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)   763642 2023-06-24 07:08:30.000000 laspy-2.5.1/tests/data/file_with_both_wkt_and_geotiff_vlrs.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    59344 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/plane.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    33684 2022-12-04 00:00:55.000000 laspy-2.5.1/tests/data/simple.copc.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    36437 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/simple.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    18217 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/simple.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    30047 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/simple1_1.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    62888 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/simple1_3.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)   814388 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/simple1_4.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    33716 2023-06-24 07:08:30.000000 laspy-2.5.1/tests/data/simple_with_page.copc.laz
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    32305 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/test1_4.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      511 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/unregistered_extra_bytes.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)   299359 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/data/vegetation_1_3.las
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5237 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_append_mode.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3873 2022-12-04 00:00:55.000000 laspy-2.5.1/tests/test_chunk_read_write.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12128 2023-07-10 17:05:57.000000 laspy-2.5.1/tests/test_common.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1171 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_constants.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      859 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_conversion.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6005 2023-06-24 07:08:30.000000 laspy-2.5.1/tests/test_copc.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4696 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_creation.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6255 2023-06-24 07:08:30.000000 laspy-2.5.1/tests/test_crs.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12315 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_extrabytes.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5197 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_field_views.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10969 2023-07-14 10:23:23.000000 laspy-2.5.1/tests/test_header.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      443 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_las_1_1.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    25434 2022-12-04 00:00:55.000000 laspy-2.5.1/tests/test_laspy.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      284 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_mmap.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1822 2023-04-17 21:23:04.000000 laspy-2.5.1/tests/test_modif_1_2.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1531 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_modif_1_4.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2891 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_non_seekable.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      486 2021-12-18 17:55:00.000000 laspy-2.5.1/tests/test_point_format.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5666 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_reading_1_2.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7534 2023-04-19 20:29:59.000000 laspy-2.5.1/tests/test_reading_1_4.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2344 2022-12-04 00:00:55.000000 laspy-2.5.1/tests/test_vlrs.py
```

### Comparing `laspy-2.5.0/LICENSE.txt` & `laspy-2.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/PKG-INFO` & `laspy-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: laspy
-Version: 2.5.0
+Version: 2.5.1
 Summary: Native Python ASPRS LAS read/write library
 Home-page: https://github.com/laspy/laspy
 Author: Grant Brown, Thomas Montaigu
 Author-email: grant.brown73@gmail.com, thomas.montaigu@laposte.net
 License: BSD
 Keywords: gis lidar las
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: lazrs
 Provides-Extra: laszip
 Provides-Extra: pyproj
 Provides-Extra: requests
 Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Laspy
 
 Laspy is a python library for reading, modifying and creating LAS LiDAR
 files.
 
-Laspy is compatible with Python  3.7+.
+Laspy is compatible with Python  3.8+.
 
 ## Features
 
 - LAS support.
 - LAZ support via `lazrs` or `laszip` backend.
 - LAS/LAZ streamed/chunked reading/writting.
 - [COPC] support over files.
```

### Comparing `laspy-2.5.0/README.md` & `laspy-2.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Laspy
 
 Laspy is a python library for reading, modifying and creating LAS LiDAR
 files.
 
-Laspy is compatible with Python  3.7+.
+Laspy is compatible with Python  3.8+.
 
 ## Features
 
 - LAS support.
 - LAZ support via `lazrs` or `laszip` backend.
 - LAS/LAZ streamed/chunked reading/writting.
 - [COPC] support over files.
```

### Comparing `laspy-2.5.0/laspy/__init__.py` & `laspy-2.5.1/laspy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 
 import logging
 
 from . import errors, file, vlrs
 from .copc import Bounds, CopcReader
 from .errors import LaspyException
 from .header import LasHeader
```

### Comparing `laspy-2.5.0/laspy/_compression/backend.py` & `laspy-2.5.1/laspy/_compression/backend.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_compression/laszipbackend.py` & `laspy-2.5.1/laspy/_compression/laszipbackend.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_compression/lazbackend.py` & `laspy-2.5.1/laspy/_compression/lazbackend.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_compression/lazrsbackend.py` & `laspy-2.5.1/laspy/_compression/lazrsbackend.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_compression/selection.py` & `laspy-2.5.1/laspy/_compression/selection.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_pointreader.py` & `laspy-2.5.1/laspy/_pointreader.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/_pointwriter.py` & `laspy-2.5.1/laspy/_pointwriter.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/cli/copc.py` & `laspy-2.5.1/laspy/cli/copc.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/copc.py` & `laspy-2.5.1/laspy/copc.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/extradims.py` & `laspy-2.5.1/laspy/extradims.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/file.py` & `laspy-2.5.1/laspy/file.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/header.py` & `laspy-2.5.1/laspy/header.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/lasappender.py` & `laspy-2.5.1/laspy/lasappender.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/lasdata.py` & `laspy-2.5.1/laspy/lasdata.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/lasmmap.py` & `laspy-2.5.1/laspy/lasmmap.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/lasreader.py` & `laspy-2.5.1/laspy/lasreader.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/laswriter.py` & `laspy-2.5.1/laspy/laswriter.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/lib.py` & `laspy-2.5.1/laspy/lib.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/point/dims.py` & `laspy-2.5.1/laspy/point/dims.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/point/format.py` & `laspy-2.5.1/laspy/point/format.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/point/record.py` & `laspy-2.5.1/laspy/point/record.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/utils.py` & `laspy-2.5.1/laspy/utils.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/vlrs/geotiff.py` & `laspy-2.5.1/laspy/vlrs/geotiff.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/vlrs/known.py` & `laspy-2.5.1/laspy/vlrs/known.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/vlrs/vlr.py` & `laspy-2.5.1/laspy/vlrs/vlr.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy/vlrs/vlrlist.py` & `laspy-2.5.1/laspy/vlrs/vlrlist.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/laspy.egg-info/PKG-INFO` & `laspy-2.5.1/laspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: laspy
-Version: 2.5.0
+Version: 2.5.1
 Summary: Native Python ASPRS LAS read/write library
 Home-page: https://github.com/laspy/laspy
 Author: Grant Brown, Thomas Montaigu
 Author-email: grant.brown73@gmail.com, thomas.montaigu@laposte.net
 License: BSD
 Keywords: gis lidar las
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: lazrs
 Provides-Extra: laszip
 Provides-Extra: pyproj
 Provides-Extra: requests
 Provides-Extra: cli
 License-File: LICENSE.txt
 
 # Laspy
 
 Laspy is a python library for reading, modifying and creating LAS LiDAR
 files.
 
-Laspy is compatible with Python  3.7+.
+Laspy is compatible with Python  3.8+.
 
 ## Features
 
 - LAS support.
 - LAZ support via `lazrs` or `laszip` backend.
 - LAS/LAZ streamed/chunked reading/writting.
 - [COPC] support over files.
```

### Comparing `laspy-2.5.0/laspy.egg-info/SOURCES.txt` & `laspy-2.5.1/laspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/setup.py` & `laspy-2.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     keywords="gis lidar las",
     author="Grant Brown, Thomas Montaigu",
     author_email="grant.brown73@gmail.com, thomas.montaigu@laposte.net",
     url="https://github.com/laspy/laspy",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["numpy"],
     extras_require={
         "dev": [
             "pytest",
             "coverage",
             "sphinx",
             "sphinx-rtd-theme",
```

### Comparing `laspy-2.5.0/tests/cli/test_info.py` & `laspy-2.5.1/tests/cli/test_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,8 +74,12 @@
     )
     assert result.exit_code != 0
     assert (
         result.output
         == """Error:
 [Errno 2] No such file or directory: 'tests/data/this_does_not_exist.las'
 """
+        or result.output  # Windows paths...
+        == """Error:
+[Errno 2] No such file or directory: 'tests\\\\data\\\\this_does_not_exist.las'
+"""
     )
```

### Comparing `laspy-2.5.0/tests/conftest.py` & `laspy-2.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/1_4_w_evlr.las` & `laspy-2.5.1/tests/data/1_4_w_evlr.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/1_4_w_evlr.laz` & `laspy-2.5.1/tests/data/1_4_w_evlr.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/autzen.las` & `laspy-2.5.1/tests/data/autzen.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/autzen_geo_proj.las` & `laspy-2.5.1/tests/data/autzen_geo_proj.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/autzen_trim.laz` & `laspy-2.5.1/tests/data/autzen_trim.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/extra.laz` & `laspy-2.5.1/tests/data/extra.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/extrabytes.las` & `laspy-2.5.1/tests/data/extrabytes.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/file_with_both_wkt_and_geotiff_vlrs.las` & `laspy-2.5.1/tests/data/file_with_both_wkt_and_geotiff_vlrs.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/plane.laz` & `laspy-2.5.1/tests/data/plane.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple.copc.laz` & `laspy-2.5.1/tests/data/simple.copc.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple.las` & `laspy-2.5.1/tests/data/simple.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple.laz` & `laspy-2.5.1/tests/data/simple.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple1_1.las` & `laspy-2.5.1/tests/data/simple1_1.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple1_3.las` & `laspy-2.5.1/tests/data/simple1_3.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple1_4.las` & `laspy-2.5.1/tests/data/simple1_4.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/simple_with_page.copc.laz` & `laspy-2.5.1/tests/data/simple_with_page.copc.laz`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/test1_4.las` & `laspy-2.5.1/tests/data/test1_4.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/data/vegetation_1_3.las` & `laspy-2.5.1/tests/data/vegetation_1_3.las`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_append_mode.py` & `laspy-2.5.1/tests/test_append_mode.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_chunk_read_write.py` & `laspy-2.5.1/tests/test_chunk_read_write.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_common.py` & `laspy-2.5.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_constants.py` & `laspy-2.5.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_conversion.py` & `laspy-2.5.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_copc.py` & `laspy-2.5.1/tests/test_copc.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_creation.py` & `laspy-2.5.1/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_crs.py` & `laspy-2.5.1/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_extrabytes.py` & `laspy-2.5.1/tests/test_extrabytes.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_field_views.py` & `laspy-2.5.1/tests/test_field_views.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_header.py` & `laspy-2.5.1/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_laspy.py` & `laspy-2.5.1/tests/test_laspy.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_modif_1_2.py` & `laspy-2.5.1/tests/test_modif_1_2.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_modif_1_4.py` & `laspy-2.5.1/tests/test_modif_1_4.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_non_seekable.py` & `laspy-2.5.1/tests/test_non_seekable.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_reading_1_2.py` & `laspy-2.5.1/tests/test_reading_1_2.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_reading_1_4.py` & `laspy-2.5.1/tests/test_reading_1_4.py`

 * *Files identical despite different names*

### Comparing `laspy-2.5.0/tests/test_vlrs.py` & `laspy-2.5.1/tests/test_vlrs.py`

 * *Files identical despite different names*

