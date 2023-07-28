# Comparing `tmp/torchqtm-0.5.0.tar.gz` & `tmp/torchqtm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchqtm-0.5.0.tar", last modified: Thu Jul 27 15:53:08 2023, max compression
+gzip compressed data, was "torchqtm-0.6.0.tar", last modified: Fri Jul 28 01:32:07 2023, max compression
```

## Comparing `torchqtm-0.5.0.tar` & `torchqtm-0.6.0.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.741000 torchqtm-0.5.0/
--rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-06-13 15:30:45.000000 torchqtm-0.5.0/LICENSE
--rw-r--r--   0 nymath     (501) staff       (20)      154 2023-07-18 02:32:38.000000 torchqtm-0.5.0/MANIFEST.in
--rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-27 15:53:08.740711 torchqtm-0.5.0/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     3547 2023-07-13 06:59:46.000000 torchqtm-0.5.0/README.md
--rw-r--r--   0 nymath     (501) staff       (20)       38 2023-07-27 15:53:08.741086 torchqtm-0.5.0/setup.cfg
--rw-r--r--   0 nymath     (501) staff       (20)     1465 2023-07-27 15:52:47.000000 torchqtm-0.5.0/setup.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.668397 torchqtm-0.5.0/test/
--rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-13 15:30:46.000000 torchqtm-0.5.0/test/testFunctional.py
--rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-13 15:30:46.000000 torchqtm-0.5.0/test/testRolling.py
--rw-r--r--   0 nymath     (501) staff       (20)        2 2023-06-13 15:30:46.000000 torchqtm-0.5.0/test/test_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-13 15:30:46.000000 torchqtm-0.5.0/test/testfunc_.py
--rw-r--r--   0 nymath     (501) staff       (20)     1865 2023-06-28 01:46:48.000000 torchqtm-0.5.0/test/testgplearn.py
--rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-13 15:30:46.000000 torchqtm-0.5.0/test/testop.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.669989 torchqtm-0.5.0/torchqtm/
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.674790 torchqtm-0.5.0/torchqtm/_C/
--rw-r--r--   0 nymath     (501) staff       (20)   108947 2023-07-13 02:19:26.000000 torchqtm-0.5.0/torchqtm/_C/__init__.c
--rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-27 12:01:02.000000 torchqtm-0.5.0/torchqtm/_C/__init__.cpp
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_C/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_C/__init__.pyx
--rw-r--r--   0 nymath     (501) staff       (20)   289603 2023-07-27 15:53:06.000000 torchqtm-0.5.0/torchqtm/_C/_functional.cpp
--rw-r--r--   0 nymath     (501) staff       (20)     1639 2023-07-13 02:24:34.000000 torchqtm-0.5.0/torchqtm/_C/_functional.pyx
--rw-r--r--   0 nymath     (501) staff       (20)  1225596 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm/_C/_rolling.cpp
--rw-r--r--   0 nymath     (501) staff       (20)    17794 2023-07-13 02:24:43.000000 torchqtm-0.5.0/torchqtm/_C/_rolling.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      736 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_C/dtypes.pxd
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.688337 torchqtm-0.5.0/torchqtm/_libs/
--rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/algos.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    49116 2023-07-07 09:25:17.000000 torchqtm-0.5.0/torchqtm/_libs/algos.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      233 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/arrays.pxd
--rw-r--r--   0 nymath     (501) staff       (20)     5861 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/arrays.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      736 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/dtypes.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    50578 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/groupby.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     4731 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/hashing.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     3213 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/hashtable.pxd
--rw-r--r--   0 nymath     (501) staff       (20)     4586 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/hashtable.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    25989 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/index.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      753 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/indexing.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    24000 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/internals.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    16608 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/interval.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    31899 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/join.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     3800 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/khash.pxd
--rw-r--r--   0 nymath     (501) staff       (20)      139 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/lib.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    89103 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/lib.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      408 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/missing.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    13911 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/missing.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     7749 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/ops.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     2570 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/ops_dispatch.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    68857 2023-07-07 09:25:17.000000 torchqtm-0.5.0/torchqtm/_libs/parsers.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     1633 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/properties.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     1090 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/reduction.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     3391 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/reshape.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    21115 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/sparse.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     5790 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/testing.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    25374 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslib.pyx
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.699672 torchqtm-0.5.0/torchqtm/_libs/tslibs/
--rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)       85 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/base.pxd
--rw-r--r--   0 nymath     (501) staff       (20)      293 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/base.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      698 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/ccalendar.pxd
--rw-r--r--   0 nymath     (501) staff       (20)     7062 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/ccalendar.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      941 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/conversion.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    24709 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/conversion.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     2540 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/dtypes.pxd
--rw-r--r--   0 nymath     (501) staff       (20)     8866 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/dtypes.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    20468 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/fields.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      339 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/nattype.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    36931 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/nattype.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     2404 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/np_datetime.pxd
--rw-r--r--   0 nymath     (501) staff       (20)     6097 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/np_datetime.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      237 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/offsets.pxd
--rw-r--r--   0 nymath     (501) staff       (20)   127830 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/offsets.pyx
--rw-r--r--   0 nymath     (501) staff       (20)       94 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/parsing.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    36738 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/parsing.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/period.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    79266 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/period.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    29116 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/strptime.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      591 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timedeltas.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    48263 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timedeltas.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     1059 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timestamps.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    67833 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timestamps.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      452 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timezones.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    13007 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/timezones.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      351 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/tzconversion.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    18840 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/tzconversion.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     5225 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/util.pxd
--rw-r--r--   0 nymath     (501) staff       (20)    12300 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/tslibs/vectorized.pyx
--rw-r--r--   0 nymath     (501) staff       (20)      352 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/util.pxd
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.700865 torchqtm-0.5.0/torchqtm/_libs/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/window/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    59202 2023-06-18 00:34:28.000000 torchqtm-0.5.0/torchqtm/_libs/window/aggregations.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     4282 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/window/indexers.pyx
--rw-r--r--   0 nymath     (501) staff       (20)     4490 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/_libs/writers.pyx
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.704789 torchqtm-0.5.0/torchqtm/alphas/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    50043 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/alpha101.py
--rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/alphas.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.705253 torchqtm-0.5.0/torchqtm/alphas/autoalpha/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.705397 torchqtm-0.5.0/torchqtm/alphas/autoalpha/boost/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/boost/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.705512 torchqtm-0.5.0/torchqtm/alphas/autoalpha/cnn/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/cnn/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.707769 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/
--rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/_program.py
--rw-r--r--   0 nymath     (501) staff       (20)     6587 2023-06-26 08:02:51.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/fitness.py
--rw-r--r--   0 nymath     (501) staff       (20)     7231 2023-06-26 08:02:51.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/functions.py
--rw-r--r--   0 nymath     (501) staff       (20)    66960 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/genetic.py
--rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     1716 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/chatgpt.py
--rw-r--r--   0 nymath     (501) staff       (20)     1317 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/introduction.py
--rw-r--r--   0 nymath     (501) staff       (20)      700 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/ml.py
--rw-r--r--   0 nymath     (501) staff       (20)      631 2023-07-18 04:25:42.000000 torchqtm-0.5.0/torchqtm/alphas/paper.py
--rw-r--r--   0 nymath     (501) staff       (20)    28048 2023-06-19 13:01:39.000000 torchqtm-0.5.0/torchqtm/alphas/statistical.py
--rw-r--r--   0 nymath     (501) staff       (20)     9453 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/alphas/technical.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.708502 torchqtm-0.5.0/torchqtm/assets/
--rw-r--r--   0 nymath     (501) staff       (20)       57 2023-07-04 07:03:05.000000 torchqtm-0.5.0/torchqtm/assets/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1430 2023-07-07 10:17:12.000000 torchqtm-0.5.0/torchqtm/assets/_assets.py
--rw-r--r--   0 nymath     (501) staff       (20)     6981 2023-06-19 12:57:55.000000 torchqtm-0.5.0/torchqtm/base.py
--rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/config.py
--rw-r--r--   0 nymath     (501) staff       (20)      337 2023-06-25 08:39:39.000000 torchqtm-0.5.0/torchqtm/configurator.py
--rw-r--r--   0 nymath     (501) staff       (20)     6957 2023-07-11 03:47:35.000000 torchqtm-0.5.0/torchqtm/constants.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.708833 torchqtm-0.5.0/torchqtm/core/
--rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/core/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.709140 torchqtm-0.5.0/torchqtm/core/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/core/window/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     6854 2023-07-11 09:25:38.000000 torchqtm-0.5.0/torchqtm/core/window/rolling.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.710496 torchqtm-0.5.0/torchqtm/data/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:11:51.000000 torchqtm-0.5.0/torchqtm/data/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1477 2023-07-06 05:29:21.000000 torchqtm-0.5.0/torchqtm/data/bardata.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.711116 torchqtm-0.5.0/torchqtm/data/bundle/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-04 03:24:44.000000 torchqtm-0.5.0/torchqtm/data/bundle/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)       68 2023-07-04 03:26:41.000000 torchqtm-0.5.0/torchqtm/data/bundle/rqalpha.py
--rw-r--r--   0 nymath     (501) staff       (20)     7505 2023-07-14 10:02:40.000000 torchqtm-0.5.0/torchqtm/data/data_portal.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.712547 torchqtm-0.5.0/torchqtm/data/rq_data_source/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 10:32:43.000000 torchqtm-0.5.0/torchqtm/data/rq_data_source/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     3214 2023-07-04 09:31:26.000000 torchqtm-0.5.0/torchqtm/data/rq_data_source/adjust.py
--rw-r--r--   0 nymath     (501) staff       (20)    18443 2023-07-15 03:27:21.000000 torchqtm-0.5.0/torchqtm/data/rq_data_source/data_source.py
--rw-r--r--   0 nymath     (501) staff       (20)    13906 2023-07-04 09:22:00.000000 torchqtm-0.5.0/torchqtm/data/rq_data_source/readers.py
--rw-r--r--   0 nymath     (501) staff       (20)      885 2023-07-02 15:35:35.000000 torchqtm-0.5.0/torchqtm/data/sample.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.712872 torchqtm-0.5.0/torchqtm/derivatives/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:10:17.000000 torchqtm-0.5.0/torchqtm/derivatives/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.713842 torchqtm-0.5.0/torchqtm/derivatives/option/
--rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/derivatives/option/Option.py
--rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/derivatives/option/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.714509 torchqtm-0.5.0/torchqtm/derivatives/option/data/
--rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/derivatives/option/data/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/derivatives/option/data/load_data.py
--rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/derivatives/option/functional.py
--rw-r--r--   0 nymath     (501) staff       (20)      598 2023-06-19 14:11:23.000000 torchqtm-0.5.0/torchqtm/derivatives/option/main.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.714806 torchqtm-0.5.0/torchqtm/dl/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-13 16:33:51.000000 torchqtm-0.5.0/torchqtm/dl/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2486 2023-07-13 16:56:24.000000 torchqtm-0.5.0/torchqtm/dl/data_loader.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.717539 torchqtm-0.5.0/torchqtm/edbt/
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-27 14:16:32.000000 torchqtm-0.5.0/torchqtm/edbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    18994 2023-07-15 11:27:23.000000 torchqtm-0.5.0/torchqtm/edbt/algorithm.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.718383 torchqtm-0.5.0/torchqtm/edbt/gens/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:46:20.000000 torchqtm-0.5.0/torchqtm/edbt/gens/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2555 2023-07-11 09:33:34.000000 torchqtm-0.5.0/torchqtm/edbt/gens/sim_engine.py
--rw-r--r--   0 nymath     (501) staff       (20)     5386 2023-07-24 12:03:26.000000 torchqtm-0.5.0/torchqtm/edbt/run_algo.py
--rw-r--r--   0 nymath     (501) staff       (20)     3458 2023-07-11 05:26:20.000000 torchqtm-0.5.0/torchqtm/edbt/sim_params.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.721057 torchqtm-0.5.0/torchqtm/edbt/temp/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:29:06.000000 torchqtm-0.5.0/torchqtm/edbt/temp/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/edbt/temp/account.py
--rw-r--r--   0 nymath     (501) staff       (20)     2269 2023-06-27 11:29:29.000000 torchqtm-0.5.0/torchqtm/edbt/temp/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/edbt/temp/datahandler.py
--rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/edbt/temp/setup.py
--rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-27 11:29:29.000000 torchqtm-0.5.0/torchqtm/edbt/temp/test.py
--rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/edbt/temp/testsearch.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.723675 torchqtm-0.5.0/torchqtm/finance/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 14:28:45.000000 torchqtm-0.5.0/torchqtm/finance/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)   381269 2023-07-27 15:53:06.000000 torchqtm-0.5.0/torchqtm/finance/_finance_ext.cpp
--rw-r--r--   0 nymath     (501) staff       (20)     5465 2023-07-13 03:01:25.000000 torchqtm-0.5.0/torchqtm/finance/_finance_ext.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    14859 2023-07-15 09:27:50.000000 torchqtm-0.5.0/torchqtm/finance/account.py
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 02:21:33.000000 torchqtm-0.5.0/torchqtm/finance/finance_ext.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.724743 torchqtm-0.5.0/torchqtm/finance/metrics/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:15:11.000000 torchqtm-0.5.0/torchqtm/finance/metrics/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      143 2023-07-12 07:38:30.000000 torchqtm-0.5.0/torchqtm/finance/metrics/loader.py
--rw-r--r--   0 nymath     (501) staff       (20)     7566 2023-07-13 05:53:29.000000 torchqtm-0.5.0/torchqtm/finance/metrics/metric.py
--rw-r--r--   0 nymath     (501) staff       (20)     9674 2023-07-14 08:51:14.000000 torchqtm-0.5.0/torchqtm/finance/metrics/tracker.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.726173 torchqtm-0.5.0/torchqtm/finance/models/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:34.000000 torchqtm-0.5.0/torchqtm/finance/models/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      845 2023-07-12 01:43:27.000000 torchqtm-0.5.0/torchqtm/finance/models/cancel_policy.py
--rw-r--r--   0 nymath     (501) staff       (20)    11967 2023-07-11 02:59:21.000000 torchqtm-0.5.0/torchqtm/finance/models/commission.py
--rw-r--r--   0 nymath     (501) staff       (20)    20911 2023-07-13 06:01:13.000000 torchqtm-0.5.0/torchqtm/finance/models/slippage.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.727112 torchqtm-0.5.0/torchqtm/finance/orders/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:14:45.000000 torchqtm-0.5.0/torchqtm/finance/orders/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     8923 2023-07-12 08:40:39.000000 torchqtm-0.5.0/torchqtm/finance/orders/order.py
--rw-r--r--   0 nymath     (501) staff       (20)    15141 2023-07-13 06:13:29.000000 torchqtm-0.5.0/torchqtm/finance/orders/tracker.py
--rw-r--r--   0 nymath     (501) staff       (20)     2466 2023-07-06 10:00:32.000000 torchqtm-0.5.0/torchqtm/finance/portfolio.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.727848 torchqtm-0.5.0/torchqtm/finance/positions/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:19.000000 torchqtm-0.5.0/torchqtm/finance/positions/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     3384 2023-07-12 06:15:32.000000 torchqtm-0.5.0/torchqtm/finance/positions/position.py
--rw-r--r--   0 nymath     (501) staff       (20)     7633 2023-07-15 09:27:50.000000 torchqtm-0.5.0/torchqtm/finance/positions/tracker.py
--rw-r--r--   0 nymath     (501) staff       (20)     1319 2023-07-06 07:02:43.000000 torchqtm-0.5.0/torchqtm/finance/transaction.py
--rw-r--r--   0 nymath     (501) staff       (20)     2566 2023-07-06 03:42:02.000000 torchqtm-0.5.0/torchqtm/finance/zp_math.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.729689 torchqtm-0.5.0/torchqtm/op/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/op/CrossSectionalOperators.py
--rw-r--r--   0 nymath     (501) staff       (20)      241 2023-06-19 12:58:39.000000 torchqtm-0.5.0/torchqtm/op/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1354 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/op/_func.pyx
--rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/op/_numba.py
--rw-r--r--   0 nymath     (501) staff       (20)     1965 2023-06-19 12:23:32.000000 torchqtm-0.5.0/torchqtm/op/algos.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.730228 torchqtm-0.5.0/torchqtm/op/filters/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 13:07:06.000000 torchqtm-0.5.0/torchqtm/op/filters/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    22259 2023-07-27 15:52:35.000000 torchqtm-0.5.0/torchqtm/op/functional.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.730943 torchqtm-0.5.0/torchqtm/tdbt/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/tdbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    12045 2023-06-23 23:59:52.000000 torchqtm-0.5.0/torchqtm/tdbt/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/tdbt/dataset.py
--rw-r--r--   0 nymath     (501) staff       (20)     1779 2023-07-11 03:00:28.000000 torchqtm-0.5.0/torchqtm/types.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.731204 torchqtm-0.5.0/torchqtm/uniquant/
--rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/uniquant/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.738209 torchqtm-0.5.0/torchqtm/utils/
--rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/utils/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      431 2023-06-18 07:34:02.000000 torchqtm-0.5.0/torchqtm/utils/_decorators.py
--rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/utils/benchmark.py
--rw-r--r--   0 nymath     (501) staff       (20)      219 2023-07-10 09:41:27.000000 torchqtm-0.5.0/torchqtm/utils/calendar_utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     1459 2023-07-12 02:05:09.000000 torchqtm-0.5.0/torchqtm/utils/datetime_utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     9078 2023-07-11 05:35:03.000000 torchqtm-0.5.0/torchqtm/utils/exchange_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/utils/rebalance.py
--rw-r--r--   0 nymath     (501) staff       (20)      114 2023-06-27 06:55:39.000000 torchqtm-0.5.0/torchqtm/utils/standards.py
--rw-r--r--   0 nymath     (501) staff       (20)     4248 2023-06-18 06:26:04.000000 torchqtm-0.5.0/torchqtm/utils/stats.py
--rw-r--r--   0 nymath     (501) staff       (20)      221 2023-07-04 05:59:26.000000 torchqtm-0.5.0/torchqtm/utils/trading_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)     1570 2023-07-06 16:31:56.000000 torchqtm-0.5.0/torchqtm/utils/universe.py
--rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/utils/visualization.py
--rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-13 15:30:46.000000 torchqtm-0.5.0/torchqtm/utils/warnings.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-27 15:53:08.670813 torchqtm-0.5.0/torchqtm.egg-info/
--rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm.egg-info/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     5963 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm.egg-info/SOURCES.txt
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm.egg-info/dependency_links.txt
--rw-r--r--   0 nymath     (501) staff       (20)       44 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm.egg-info/requires.txt
--rw-r--r--   0 nymath     (501) staff       (20)        9 2023-07-27 15:53:08.000000 torchqtm-0.5.0/torchqtm.egg-info/top_level.txt
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.499886 torchqtm-0.6.0/
+-rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-06-13 15:30:45.000000 torchqtm-0.6.0/LICENSE
+-rw-r--r--   0 nymath     (501) staff       (20)      154 2023-07-18 02:32:38.000000 torchqtm-0.6.0/MANIFEST.in
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-28 01:32:07.499597 torchqtm-0.6.0/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     3547 2023-07-13 06:59:46.000000 torchqtm-0.6.0/README.md
+-rw-r--r--   0 nymath     (501) staff       (20)       38 2023-07-28 01:32:07.499959 torchqtm-0.6.0/setup.cfg
+-rw-r--r--   0 nymath     (501) staff       (20)     1465 2023-07-28 01:32:04.000000 torchqtm-0.6.0/setup.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.425923 torchqtm-0.6.0/test/
+-rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-13 15:30:46.000000 torchqtm-0.6.0/test/testFunctional.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-13 15:30:46.000000 torchqtm-0.6.0/test/testRolling.py
+-rw-r--r--   0 nymath     (501) staff       (20)        2 2023-06-13 15:30:46.000000 torchqtm-0.6.0/test/test_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-13 15:30:46.000000 torchqtm-0.6.0/test/testfunc_.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1865 2023-06-28 01:46:48.000000 torchqtm-0.6.0/test/testgplearn.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-13 15:30:46.000000 torchqtm-0.6.0/test/testop.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.427281 torchqtm-0.6.0/torchqtm/
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.438121 torchqtm-0.6.0/torchqtm/_C/
+-rw-r--r--   0 nymath     (501) staff       (20)   108947 2023-07-13 02:19:26.000000 torchqtm-0.6.0/torchqtm/_C/__init__.c
+-rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-27 12:01:02.000000 torchqtm-0.6.0/torchqtm/_C/__init__.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_C/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_C/__init__.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)   289603 2023-07-27 15:53:06.000000 torchqtm-0.6.0/torchqtm/_C/_functional.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)     1639 2023-07-13 02:24:34.000000 torchqtm-0.6.0/torchqtm/_C/_functional.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)  1225596 2023-07-27 15:53:08.000000 torchqtm-0.6.0/torchqtm/_C/_rolling.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)    17794 2023-07-13 02:24:43.000000 torchqtm-0.6.0/torchqtm/_C/_rolling.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      736 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_C/dtypes.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.451298 torchqtm-0.6.0/torchqtm/_libs/
+-rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/algos.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    49116 2023-07-07 09:25:17.000000 torchqtm-0.6.0/torchqtm/_libs/algos.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      233 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/arrays.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)     5861 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/arrays.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      736 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/dtypes.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    50578 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/groupby.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     4731 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/hashing.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     3213 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/hashtable.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)     4586 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/hashtable.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    25989 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/index.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      753 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/indexing.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    24000 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/internals.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    16608 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/interval.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    31899 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/join.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     3800 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/khash.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)      139 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/lib.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    89103 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/lib.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      408 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/missing.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    13911 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/missing.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     7749 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/ops.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     2570 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/ops_dispatch.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    68857 2023-07-07 09:25:17.000000 torchqtm-0.6.0/torchqtm/_libs/parsers.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     1633 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/properties.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     1090 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/reduction.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     3391 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/reshape.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    21115 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/sparse.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     5790 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/testing.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    25374 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslib.pyx
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.462816 torchqtm-0.6.0/torchqtm/_libs/tslibs/
+-rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)       85 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/base.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)      293 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/base.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      698 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/ccalendar.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)     7062 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/ccalendar.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      941 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/conversion.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    24709 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/conversion.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     2540 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/dtypes.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)     8866 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/dtypes.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    20468 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/fields.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      339 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/nattype.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    36931 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/nattype.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     2404 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/np_datetime.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)     6097 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/np_datetime.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      237 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/offsets.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)   127830 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/offsets.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)       94 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/parsing.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    36738 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/parsing.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/period.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    79266 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/period.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    29116 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/strptime.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      591 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timedeltas.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    48263 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timedeltas.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     1059 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timestamps.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    67833 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timestamps.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      452 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timezones.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    13007 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/timezones.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      351 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/tzconversion.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    18840 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/tzconversion.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     5225 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/util.pxd
+-rw-r--r--   0 nymath     (501) staff       (20)    12300 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/tslibs/vectorized.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)      352 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/util.pxd
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.463910 torchqtm-0.6.0/torchqtm/_libs/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/window/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    59202 2023-06-18 00:34:28.000000 torchqtm-0.6.0/torchqtm/_libs/window/aggregations.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     4282 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/window/indexers.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)     4490 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/_libs/writers.pyx
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.467165 torchqtm-0.6.0/torchqtm/alphas/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    50043 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/alpha101.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/alphas.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.467651 torchqtm-0.6.0/torchqtm/alphas/autoalpha/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.467801 torchqtm-0.6.0/torchqtm/alphas/autoalpha/boost/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/boost/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.467955 torchqtm-0.6.0/torchqtm/alphas/autoalpha/cnn/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/cnn/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.470456 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/
+-rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/_program.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6587 2023-06-26 08:02:51.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/fitness.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7231 2023-06-26 08:02:51.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/functions.py
+-rw-r--r--   0 nymath     (501) staff       (20)    66960 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/genetic.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1716 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/chatgpt.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1317 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/introduction.py
+-rw-r--r--   0 nymath     (501) staff       (20)      700 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/ml.py
+-rw-r--r--   0 nymath     (501) staff       (20)      631 2023-07-18 04:25:42.000000 torchqtm-0.6.0/torchqtm/alphas/paper.py
+-rw-r--r--   0 nymath     (501) staff       (20)    28048 2023-06-19 13:01:39.000000 torchqtm-0.6.0/torchqtm/alphas/statistical.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9453 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/alphas/technical.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.471111 torchqtm-0.6.0/torchqtm/assets/
+-rw-r--r--   0 nymath     (501) staff       (20)       57 2023-07-04 07:03:05.000000 torchqtm-0.6.0/torchqtm/assets/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1430 2023-07-07 10:17:12.000000 torchqtm-0.6.0/torchqtm/assets/_assets.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6981 2023-06-19 12:57:55.000000 torchqtm-0.6.0/torchqtm/base.py
+-rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/config.py
+-rw-r--r--   0 nymath     (501) staff       (20)      337 2023-06-25 08:39:39.000000 torchqtm-0.6.0/torchqtm/configurator.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6957 2023-07-11 03:47:35.000000 torchqtm-0.6.0/torchqtm/constants.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.471492 torchqtm-0.6.0/torchqtm/core/
+-rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/core/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.471922 torchqtm-0.6.0/torchqtm/core/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/core/window/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6854 2023-07-11 09:25:38.000000 torchqtm-0.6.0/torchqtm/core/window/rolling.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.474139 torchqtm-0.6.0/torchqtm/data/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:11:51.000000 torchqtm-0.6.0/torchqtm/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1477 2023-07-06 05:29:21.000000 torchqtm-0.6.0/torchqtm/data/bardata.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.474684 torchqtm-0.6.0/torchqtm/data/bundle/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-04 03:24:44.000000 torchqtm-0.6.0/torchqtm/data/bundle/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)       68 2023-07-04 03:26:41.000000 torchqtm-0.6.0/torchqtm/data/bundle/rqalpha.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7505 2023-07-14 10:02:40.000000 torchqtm-0.6.0/torchqtm/data/data_portal.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.475968 torchqtm-0.6.0/torchqtm/data/rq_data_source/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 10:32:43.000000 torchqtm-0.6.0/torchqtm/data/rq_data_source/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3214 2023-07-04 09:31:26.000000 torchqtm-0.6.0/torchqtm/data/rq_data_source/adjust.py
+-rw-r--r--   0 nymath     (501) staff       (20)    18443 2023-07-15 03:27:21.000000 torchqtm-0.6.0/torchqtm/data/rq_data_source/data_source.py
+-rw-r--r--   0 nymath     (501) staff       (20)    13906 2023-07-04 09:22:00.000000 torchqtm-0.6.0/torchqtm/data/rq_data_source/readers.py
+-rw-r--r--   0 nymath     (501) staff       (20)      885 2023-07-02 15:35:35.000000 torchqtm-0.6.0/torchqtm/data/sample.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.476298 torchqtm-0.6.0/torchqtm/derivatives/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:10:17.000000 torchqtm-0.6.0/torchqtm/derivatives/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.477290 torchqtm-0.6.0/torchqtm/derivatives/option/
+-rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/derivatives/option/Option.py
+-rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/derivatives/option/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.477753 torchqtm-0.6.0/torchqtm/derivatives/option/data/
+-rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/derivatives/option/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/derivatives/option/data/load_data.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/derivatives/option/functional.py
+-rw-r--r--   0 nymath     (501) staff       (20)      598 2023-06-19 14:11:23.000000 torchqtm-0.6.0/torchqtm/derivatives/option/main.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.478015 torchqtm-0.6.0/torchqtm/dl/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-13 16:33:51.000000 torchqtm-0.6.0/torchqtm/dl/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2486 2023-07-13 16:56:24.000000 torchqtm-0.6.0/torchqtm/dl/data_loader.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.479246 torchqtm-0.6.0/torchqtm/edbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-27 14:16:32.000000 torchqtm-0.6.0/torchqtm/edbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    18994 2023-07-15 11:27:23.000000 torchqtm-0.6.0/torchqtm/edbt/algorithm.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.479648 torchqtm-0.6.0/torchqtm/edbt/gens/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:46:20.000000 torchqtm-0.6.0/torchqtm/edbt/gens/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2555 2023-07-11 09:33:34.000000 torchqtm-0.6.0/torchqtm/edbt/gens/sim_engine.py
+-rw-r--r--   0 nymath     (501) staff       (20)     5448 2023-07-28 01:28:50.000000 torchqtm-0.6.0/torchqtm/edbt/run_algo.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3458 2023-07-11 05:26:20.000000 torchqtm-0.6.0/torchqtm/edbt/sim_params.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.481087 torchqtm-0.6.0/torchqtm/edbt/temp/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:29:06.000000 torchqtm-0.6.0/torchqtm/edbt/temp/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/edbt/temp/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2269 2023-06-27 11:29:29.000000 torchqtm-0.6.0/torchqtm/edbt/temp/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/edbt/temp/datahandler.py
+-rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/edbt/temp/setup.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-27 11:29:29.000000 torchqtm-0.6.0/torchqtm/edbt/temp/test.py
+-rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/edbt/temp/testsearch.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.484920 torchqtm-0.6.0/torchqtm/finance/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 14:28:45.000000 torchqtm-0.6.0/torchqtm/finance/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   381269 2023-07-27 15:53:06.000000 torchqtm-0.6.0/torchqtm/finance/_finance_ext.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)     5465 2023-07-13 03:01:25.000000 torchqtm-0.6.0/torchqtm/finance/_finance_ext.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    14859 2023-07-15 09:27:50.000000 torchqtm-0.6.0/torchqtm/finance/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 02:21:33.000000 torchqtm-0.6.0/torchqtm/finance/finance_ext.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.486182 torchqtm-0.6.0/torchqtm/finance/metrics/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:15:11.000000 torchqtm-0.6.0/torchqtm/finance/metrics/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      143 2023-07-12 07:38:30.000000 torchqtm-0.6.0/torchqtm/finance/metrics/loader.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7566 2023-07-13 05:53:29.000000 torchqtm-0.6.0/torchqtm/finance/metrics/metric.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9674 2023-07-14 08:51:14.000000 torchqtm-0.6.0/torchqtm/finance/metrics/tracker.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.487958 torchqtm-0.6.0/torchqtm/finance/models/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:34.000000 torchqtm-0.6.0/torchqtm/finance/models/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      845 2023-07-12 01:43:27.000000 torchqtm-0.6.0/torchqtm/finance/models/cancel_policy.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11967 2023-07-11 02:59:21.000000 torchqtm-0.6.0/torchqtm/finance/models/commission.py
+-rw-r--r--   0 nymath     (501) staff       (20)    20911 2023-07-13 06:01:13.000000 torchqtm-0.6.0/torchqtm/finance/models/slippage.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.489026 torchqtm-0.6.0/torchqtm/finance/orders/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:14:45.000000 torchqtm-0.6.0/torchqtm/finance/orders/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     8923 2023-07-12 08:40:39.000000 torchqtm-0.6.0/torchqtm/finance/orders/order.py
+-rw-r--r--   0 nymath     (501) staff       (20)    15141 2023-07-13 06:13:29.000000 torchqtm-0.6.0/torchqtm/finance/orders/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2466 2023-07-06 10:00:32.000000 torchqtm-0.6.0/torchqtm/finance/portfolio.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.490083 torchqtm-0.6.0/torchqtm/finance/positions/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:19.000000 torchqtm-0.6.0/torchqtm/finance/positions/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3384 2023-07-12 06:15:32.000000 torchqtm-0.6.0/torchqtm/finance/positions/position.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7633 2023-07-15 09:27:50.000000 torchqtm-0.6.0/torchqtm/finance/positions/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1319 2023-07-06 07:02:43.000000 torchqtm-0.6.0/torchqtm/finance/transaction.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2566 2023-07-06 03:42:02.000000 torchqtm-0.6.0/torchqtm/finance/zp_math.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.492033 torchqtm-0.6.0/torchqtm/op/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/op/CrossSectionalOperators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      241 2023-06-19 12:58:39.000000 torchqtm-0.6.0/torchqtm/op/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1354 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/op/_func.pyx
+-rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/op/_numba.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1965 2023-06-19 12:23:32.000000 torchqtm-0.6.0/torchqtm/op/algos.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.492538 torchqtm-0.6.0/torchqtm/op/filters/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 13:07:06.000000 torchqtm-0.6.0/torchqtm/op/filters/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    22245 2023-07-28 01:31:47.000000 torchqtm-0.6.0/torchqtm/op/functional.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.493229 torchqtm-0.6.0/torchqtm/tdbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/tdbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    12045 2023-06-23 23:59:52.000000 torchqtm-0.6.0/torchqtm/tdbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/tdbt/dataset.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1779 2023-07-11 03:00:28.000000 torchqtm-0.6.0/torchqtm/types.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.493506 torchqtm-0.6.0/torchqtm/uniquant/
+-rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/uniquant/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.499178 torchqtm-0.6.0/torchqtm/utils/
+-rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/utils/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      431 2023-06-18 07:34:02.000000 torchqtm-0.6.0/torchqtm/utils/_decorators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/utils/benchmark.py
+-rw-r--r--   0 nymath     (501) staff       (20)      219 2023-07-10 09:41:27.000000 torchqtm-0.6.0/torchqtm/utils/calendar_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1459 2023-07-12 02:05:09.000000 torchqtm-0.6.0/torchqtm/utils/datetime_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9078 2023-07-11 05:35:03.000000 torchqtm-0.6.0/torchqtm/utils/exchange_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/utils/rebalance.py
+-rw-r--r--   0 nymath     (501) staff       (20)      114 2023-06-27 06:55:39.000000 torchqtm-0.6.0/torchqtm/utils/standards.py
+-rw-r--r--   0 nymath     (501) staff       (20)     4248 2023-06-18 06:26:04.000000 torchqtm-0.6.0/torchqtm/utils/stats.py
+-rw-r--r--   0 nymath     (501) staff       (20)      221 2023-07-04 05:59:26.000000 torchqtm-0.6.0/torchqtm/utils/trading_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1570 2023-07-06 16:31:56.000000 torchqtm-0.6.0/torchqtm/utils/universe.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/utils/visualization.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-13 15:30:46.000000 torchqtm-0.6.0/torchqtm/utils/warnings.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-28 01:32:07.428004 torchqtm-0.6.0/torchqtm.egg-info/
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-28 01:32:07.000000 torchqtm-0.6.0/torchqtm.egg-info/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     5963 2023-07-28 01:32:07.000000 torchqtm-0.6.0/torchqtm.egg-info/SOURCES.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-07-28 01:32:07.000000 torchqtm-0.6.0/torchqtm.egg-info/dependency_links.txt
+-rw-r--r--   0 nymath     (501) staff       (20)       44 2023-07-28 01:32:07.000000 torchqtm-0.6.0/torchqtm.egg-info/requires.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        9 2023-07-28 01:32:07.000000 torchqtm-0.6.0/torchqtm.egg-info/top_level.txt
```

### Comparing `torchqtm-0.5.0/LICENSE` & `torchqtm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/PKG-INFO` & `torchqtm-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.5.0
+Version: 0.6.0
 Summary: None
 Home-page: https://github.com/nymath/torchqtm
 Download-URL: https://github.com/nymath/torchqtm/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchqtm-0.5.0/README.md` & `torchqtm-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/setup.py` & `torchqtm-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def main():
     setup(
         ext_modules=cythonize(extensions, annotate=True),
         include_dirs=[numpy.get_include()],
         name="torchqtm",
-        version="0.5.0",
+        version="0.6.0",
         author="ny",
         author_email="nymath@163.com",
         install_requires=install_requires,
         description="None",
         long_description=open('README.md', 'r').read(),
         long_description_content_type="text/markdown",
         url="https://github.com/nymath/torchqtm",
```

### Comparing `torchqtm-0.5.0/test/testRolling.py` & `torchqtm-0.6.0/test/testRolling.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/test/testgplearn.py` & `torchqtm-0.6.0/test/testgplearn.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/test/testop.py` & `torchqtm-0.6.0/test/testop.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/__init__.c` & `torchqtm-0.6.0/torchqtm/_C/__init__.c`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/__init__.cpp` & `torchqtm-0.6.0/torchqtm/_C/__init__.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/_functional.cpp` & `torchqtm-0.6.0/torchqtm/_C/_functional.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/_functional.pyx` & `torchqtm-0.6.0/torchqtm/_C/_functional.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/_rolling.cpp` & `torchqtm-0.6.0/torchqtm/_C/_rolling.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/_rolling.pyx` & `torchqtm-0.6.0/torchqtm/_C/_rolling.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_C/dtypes.pxd` & `torchqtm-0.6.0/torchqtm/_C/dtypes.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/algos.pyx` & `torchqtm-0.6.0/torchqtm/_libs/algos.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/arrays.pyx` & `torchqtm-0.6.0/torchqtm/_libs/arrays.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/dtypes.pxd` & `torchqtm-0.6.0/torchqtm/_libs/dtypes.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/groupby.pyx` & `torchqtm-0.6.0/torchqtm/_libs/groupby.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/hashing.pyx` & `torchqtm-0.6.0/torchqtm/_libs/hashing.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/hashtable.pxd` & `torchqtm-0.6.0/torchqtm/_libs/hashtable.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/hashtable.pyx` & `torchqtm-0.6.0/torchqtm/_libs/hashtable.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/index.pyx` & `torchqtm-0.6.0/torchqtm/_libs/index.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/indexing.pyx` & `torchqtm-0.6.0/torchqtm/_libs/indexing.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/internals.pyx` & `torchqtm-0.6.0/torchqtm/_libs/internals.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/interval.pyx` & `torchqtm-0.6.0/torchqtm/_libs/interval.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/join.pyx` & `torchqtm-0.6.0/torchqtm/_libs/join.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/khash.pxd` & `torchqtm-0.6.0/torchqtm/_libs/khash.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/lib.pyx` & `torchqtm-0.6.0/torchqtm/_libs/lib.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/missing.pyx` & `torchqtm-0.6.0/torchqtm/_libs/missing.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/ops.pyx` & `torchqtm-0.6.0/torchqtm/_libs/ops.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/ops_dispatch.pyx` & `torchqtm-0.6.0/torchqtm/_libs/ops_dispatch.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/parsers.pyx` & `torchqtm-0.6.0/torchqtm/_libs/parsers.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/properties.pyx` & `torchqtm-0.6.0/torchqtm/_libs/properties.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/reduction.pyx` & `torchqtm-0.6.0/torchqtm/_libs/reduction.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/reshape.pyx` & `torchqtm-0.6.0/torchqtm/_libs/reshape.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/sparse.pyx` & `torchqtm-0.6.0/torchqtm/_libs/sparse.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/testing.pyx` & `torchqtm-0.6.0/torchqtm/_libs/testing.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslib.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslib.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/__init__.py` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/ccalendar.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/ccalendar.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/ccalendar.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/ccalendar.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/conversion.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/conversion.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/conversion.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/conversion.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/dtypes.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/dtypes.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/dtypes.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/dtypes.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/fields.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/fields.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/nattype.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/nattype.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/np_datetime.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/np_datetime.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/np_datetime.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/np_datetime.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/offsets.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/offsets.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/parsing.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/parsing.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/period.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/period.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/strptime.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/strptime.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/timedeltas.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/timedeltas.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/timedeltas.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/timedeltas.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/timestamps.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/timestamps.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/timestamps.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/timestamps.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/timezones.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/timezones.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/tzconversion.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/tzconversion.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/util.pxd` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/util.pxd`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/tslibs/vectorized.pyx` & `torchqtm-0.6.0/torchqtm/_libs/tslibs/vectorized.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/window/aggregations.pyx` & `torchqtm-0.6.0/torchqtm/_libs/window/aggregations.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/window/indexers.pyx` & `torchqtm-0.6.0/torchqtm/_libs/window/indexers.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/_libs/writers.pyx` & `torchqtm-0.6.0/torchqtm/_libs/writers.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/alpha101.py` & `torchqtm-0.6.0/torchqtm/alphas/alpha101.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/alphas.py` & `torchqtm-0.6.0/torchqtm/alphas/alphas.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/_program.py` & `torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/_program.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/fitness.py` & `torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/fitness.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/functions.py` & `torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/functions.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/genetic.py` & `torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/genetic.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/autoalpha/gplearn/utils.py` & `torchqtm-0.6.0/torchqtm/alphas/autoalpha/gplearn/utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/chatgpt.py` & `torchqtm-0.6.0/torchqtm/alphas/chatgpt.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/introduction.py` & `torchqtm-0.6.0/torchqtm/alphas/introduction.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/ml.py` & `torchqtm-0.6.0/torchqtm/alphas/ml.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/paper.py` & `torchqtm-0.6.0/torchqtm/alphas/paper.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/statistical.py` & `torchqtm-0.6.0/torchqtm/alphas/statistical.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/alphas/technical.py` & `torchqtm-0.6.0/torchqtm/alphas/technical.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/assets/_assets.py` & `torchqtm-0.6.0/torchqtm/assets/_assets.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/base.py` & `torchqtm-0.6.0/torchqtm/base.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/constants.py` & `torchqtm-0.6.0/torchqtm/constants.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/core/window/rolling.py` & `torchqtm-0.6.0/torchqtm/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/bardata.py` & `torchqtm-0.6.0/torchqtm/data/bardata.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/data_portal.py` & `torchqtm-0.6.0/torchqtm/data/data_portal.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/rq_data_source/adjust.py` & `torchqtm-0.6.0/torchqtm/data/rq_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/rq_data_source/data_source.py` & `torchqtm-0.6.0/torchqtm/data/rq_data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/rq_data_source/readers.py` & `torchqtm-0.6.0/torchqtm/data/rq_data_source/readers.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/data/sample.py` & `torchqtm-0.6.0/torchqtm/data/sample.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/derivatives/option/functional.py` & `torchqtm-0.6.0/torchqtm/derivatives/option/functional.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/derivatives/option/main.py` & `torchqtm-0.6.0/torchqtm/derivatives/option/main.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/dl/data_loader.py` & `torchqtm-0.6.0/torchqtm/dl/data_loader.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/algorithm.py` & `torchqtm-0.6.0/torchqtm/edbt/algorithm.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/gens/sim_engine.py` & `torchqtm-0.6.0/torchqtm/edbt/gens/sim_engine.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/run_algo.py` & `torchqtm-0.6.0/torchqtm/edbt/run_algo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import typing
 
-import talib
+# import talib
 
 from torchqtm.edbt.algorithm import TradingAlgorithm
 from torchqtm.edbt.sim_params import SimulationParameters
 
 from torchqtm.finance.account import Account
 from torchqtm.finance.metrics.tracker import MetricsTracker
 from torchqtm.utils.calendar_utils import get_calendar
@@ -103,27 +103,28 @@
         self.sym: Equity
         self.count: int
 
     def before_trading_start(self):
         pass
 
     def handle_data(self):
-        for i in range(300):
-            prices = self.history(self.sym, 'close', 21, "daily")
-
-        short_avg = talib.SMA(prices, 5)
-        long_avg = talib.SMA(prices, 20)
-
-        current_position = self.account.get_position(self.sym)
-        if short_avg[-1] - long_avg[-1] < 0 and short_avg[-2] - long_avg[-2] > 0 and current_position.amount > 0:
-            self.order(self.sym, -100)
-
-        if short_avg[-1] - long_avg[-1] > 0 and short_avg[-2] - long_avg[-2] < 0:
-            for i in range(100):
-                self.order(self.sym, 10)
+        # for i in range(300):
+        #     prices = self.history(self.sym, 'close', 21, "daily")
+        #
+        # short_avg = talib.SMA(prices, 5)
+        # long_avg = talib.SMA(prices, 20)
+        #
+        # current_position = self.account.get_position(self.sym)
+        # if short_avg[-1] - long_avg[-1] < 0 and short_avg[-2] - long_avg[-2] > 0 and current_position.amount > 0:
+        #     self.order(self.sym, -100)
+        #
+        # if short_avg[-1] - long_avg[-1] > 0 and short_avg[-2] - long_avg[-2] < 0:
+        #     for i in range(100):
+        #         self.order(self.sym, 10)
+        pass
 
     def analyze(self):
         print(self.account.ledger.cash)
         print(self.account.ledger.portfolio_value)
 
 
 import sys
```

### Comparing `torchqtm-0.5.0/torchqtm/edbt/sim_params.py` & `torchqtm-0.6.0/torchqtm/edbt/sim_params.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/temp/account.py` & `torchqtm-0.6.0/torchqtm/edbt/temp/account.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/temp/backtest.py` & `torchqtm-0.6.0/torchqtm/edbt/temp/backtest.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/temp/datahandler.py` & `torchqtm-0.6.0/torchqtm/edbt/temp/datahandler.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/edbt/temp/test.py` & `torchqtm-0.6.0/torchqtm/edbt/temp/test.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/_finance_ext.cpp` & `torchqtm-0.6.0/torchqtm/finance/_finance_ext.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/_finance_ext.pyx` & `torchqtm-0.6.0/torchqtm/finance/_finance_ext.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/account.py` & `torchqtm-0.6.0/torchqtm/finance/account.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/metrics/metric.py` & `torchqtm-0.6.0/torchqtm/finance/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/metrics/tracker.py` & `torchqtm-0.6.0/torchqtm/finance/metrics/tracker.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/models/cancel_policy.py` & `torchqtm-0.6.0/torchqtm/finance/models/cancel_policy.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/models/commission.py` & `torchqtm-0.6.0/torchqtm/finance/models/commission.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/models/slippage.py` & `torchqtm-0.6.0/torchqtm/finance/models/slippage.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/orders/order.py` & `torchqtm-0.6.0/torchqtm/finance/orders/order.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/orders/tracker.py` & `torchqtm-0.6.0/torchqtm/finance/orders/tracker.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/portfolio.py` & `torchqtm-0.6.0/torchqtm/finance/portfolio.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/positions/position.py` & `torchqtm-0.6.0/torchqtm/finance/positions/position.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/positions/tracker.py` & `torchqtm-0.6.0/torchqtm/finance/positions/tracker.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/transaction.py` & `torchqtm-0.6.0/torchqtm/finance/transaction.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/finance/zp_math.py` & `torchqtm-0.6.0/torchqtm/finance/zp_math.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/op/_func.pyx` & `torchqtm-0.6.0/torchqtm/op/_func.pyx`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/op/_numba.py` & `torchqtm-0.6.0/torchqtm/op/_numba.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/op/algos.py` & `torchqtm-0.6.0/torchqtm/op/algos.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/op/functional.py` & `torchqtm-0.6.0/torchqtm/op/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import pandas as pd
 from sklearn.linear_model import LinearRegression
 
 from ..config import __OP_MODE__
 from typing import overload
 from .algos import rank_1d, rank_2d
 from scipy.stats import norm
-import talib
 import typing
 
 CORR_METHOD = typing.Literal["pearson", "spearman"]
 
-
 # Arithmetic Operators
 
 
 def revert_type(raw, target):
     if isinstance(target, np.ndarray):
         return raw.values
     elif isinstance(target, pd.Series):
```

### Comparing `torchqtm-0.5.0/torchqtm/tdbt/backtest.py` & `torchqtm-0.6.0/torchqtm/tdbt/backtest.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/types.py` & `torchqtm-0.6.0/torchqtm/types.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/__init__.py` & `torchqtm-0.6.0/torchqtm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/benchmark.py` & `torchqtm-0.6.0/torchqtm/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/datetime_utils.py` & `torchqtm-0.6.0/torchqtm/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/exchange_calendar.py` & `torchqtm-0.6.0/torchqtm/utils/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/rebalance.py` & `torchqtm-0.6.0/torchqtm/utils/rebalance.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/stats.py` & `torchqtm-0.6.0/torchqtm/utils/stats.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/universe.py` & `torchqtm-0.6.0/torchqtm/utils/universe.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/visualization.py` & `torchqtm-0.6.0/torchqtm/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm/utils/warnings.py` & `torchqtm-0.6.0/torchqtm/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.5.0/torchqtm.egg-info/PKG-INFO` & `torchqtm-0.6.0/torchqtm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.5.0
+Version: 0.6.0
 Summary: None
 Home-page: https://github.com/nymath/torchqtm
 Download-URL: https://github.com/nymath/torchqtm/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchqtm-0.5.0/torchqtm.egg-info/SOURCES.txt` & `torchqtm-0.6.0/torchqtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

