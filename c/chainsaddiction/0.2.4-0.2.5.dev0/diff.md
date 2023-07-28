# Comparing `tmp/chainsaddiction-0.2.4.tar.gz` & `tmp/chainsaddiction-0.2.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsaddiction-0.2.4.tar", last modified: Mon Jul  3 19:28:34 2023, max compression
+gzip compressed data, was "chainsaddiction-0.2.5.dev0.tar", last modified: Fri Jul 28 13:09:09 2023, max compression
```

## Comparing `chainsaddiction-0.2.4.tar` & `chainsaddiction-0.2.5.dev0.tar`

### file list

```diff
@@ -1,272 +1,275 @@
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.091040 chainsaddiction-0.2.4/
--rw-r--r--   0 pmind      (502) staff       (20)      235 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/.gitignore
--rw-r--r--   0 pmind      (502) staff       (20)       96 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/.gitmodules
--rw-r--r--   0 pmind      (502) staff       (20)      336 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/.readthedocs.yaml
--rw-r--r--   0 pmind      (502) staff       (20)      387 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/CHANGELOG.md
--rw-r--r--   0 pmind      (502) staff       (20)     1487 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/LICENSE
--rw-r--r--   0 pmind      (502) staff       (20)       58 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/MANIFEST.in
--rw-r--r--   0 pmind      (502) staff       (20)     1938 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-03 19:28:34.090579 chainsaddiction-0.2.4/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     1223 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/README.md
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.717789 chainsaddiction-0.2.4/docs/
--rw-r--r--   0 pmind      (502) staff       (20)      584 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      791 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/make.bat
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.722085 chainsaddiction-0.2.4/docs/source/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.724496 chainsaddiction-0.2.4/docs/source/api/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.733572 chainsaddiction-0.2.4/docs/source/api/c/
--rw-r--r--   0 pmind      (502) staff       (20)      483 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/basics.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1792 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/dataset.rst
--rw-r--r--   0 pmind      (502) staff       (20)      279 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)      116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/internal.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.740144 chainsaddiction-0.2.4/docs/source/api/c/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)      200 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     5120 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-hmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)     4161 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-params.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1952 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-probs.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2260 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/api/c/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)      337 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.743869 chainsaddiction-0.2.4/docs/source/api/python/
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/python/index.rst
--rw-r--r--   0 pmind      (502) staff       (20)     2123 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/api/python/poishmm.rst
--rw-r--r--   0 pmind      (502) staff       (20)      805 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/api/python/utils.rst
--rw-r--r--   0 pmind      (502) staff       (20)     1897 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/conf.py
--rw-r--r--   0 pmind      (502) staff       (20)     2229 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/docs/source/getting-started.rst
--rw-r--r--   0 pmind      (502) staff       (20)      526 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/docs/source/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.753147 chainsaddiction-0.2.4/docs/source/usrguide/
--rw-r--r--   0 pmind      (502) staff       (20)     1442 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/usrguide/examples.rst
--rw-r--r--   0 pmind      (502) staff       (20)      198 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/docs/source/usrguide/index.rst
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.755857 chainsaddiction-0.2.4/include/
--rw-r--r--   0 pmind      (502) staff       (20)      464 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/include/chainsaddiction.h
--rw-r--r--   0 pmind      (502) staff       (20)      159 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/include/libvmath.h
--rw-r--r--   0 pmind      (502) staff       (20)     1079 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/pyproject.toml
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/requirements-dev.txt
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-07-03 19:28:34.091168 chainsaddiction-0.2.4/setup.cfg
--rw-r--r--   0 pmind      (502) staff       (20)     1458 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/setup.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.689972 chainsaddiction-0.2.4/src/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.768633 chainsaddiction-0.2.4/src/chainsaddiction/
--rw-r--r--   0 pmind      (502) staff       (20)      249 2023-07-02 14:18:19.000000 chainsaddiction-0.2.4/src/chainsaddiction/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     2028 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)     1953 2023-07-03 18:58:10.000000 chainsaddiction-0.2.4/src/chainsaddiction/dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)      301 2023-07-03 18:58:31.000000 chainsaddiction-0.2.4/src/chainsaddiction/err.h
--rw-r--r--   0 pmind      (502) staff       (20)      861 2023-07-03 18:59:33.000000 chainsaddiction-0.2.4/src/chainsaddiction/libma.c
--rw-r--r--   0 pmind      (502) staff       (20)     1831 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/libma.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.788627 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/
--rw-r--r--   0 pmind      (502) staff       (20)     1240 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      543 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/__init__.pyi
--rw-r--r--   0 pmind      (502) staff       (20)     4383 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)     2212 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     1844 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.c
--rw-r--r--   0 pmind      (502) staff       (20)     2153 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.h
--rw-r--r--   0 pmind      (502) staff       (20)     4864 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)     2099 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     4534 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)     2116 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      965 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)     1132 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)     9737 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.c
--rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     2417 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-object.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.799414 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1594 2023-07-02 11:49:32.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/Makefile
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.814244 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)      222 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/params-3s
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr1
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr2
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr3
--rw-r--r--   0 pmind      (502) staff       (20)      119 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr4
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/ppr5
--rw-r--r--   0 pmind      (502) staff       (20)      135 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
--rw-r--r--   0 pmind      (502) staff       (20)      896 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     4808 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.c
--rw-r--r--   0 pmind      (502) staff       (20)      294 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.h
--rw-r--r--   0 pmind      (502) staff       (20)     6676 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
--rw-r--r--   0 pmind      (502) staff       (20)      546 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
--rw-r--r--   0 pmind      (502) staff       (20)     1239 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.c
--rw-r--r--   0 pmind      (502) staff       (20)      220 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.h
--rw-r--r--   0 pmind      (502) staff       (20)      699 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.c
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.h
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/py.typed
--rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/read.c
--rw-r--r--   0 pmind      (502) staff       (20)     1561 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/read.h
--rw-r--r--   0 pmind      (502) staff       (20)      196 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/restrict.h
--rw-r--r--   0 pmind      (502) staff       (20)      337 2023-07-03 19:27:22.000000 chainsaddiction-0.2.4/src/chainsaddiction/scalar.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.823988 chainsaddiction-0.2.4/src/chainsaddiction/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      822 2023-07-02 14:18:30.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      593 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2464 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.c
--rw-r--r--   0 pmind      (502) staff       (20)      626 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.h
--rw-r--r--   0 pmind      (502) staff       (20)     3103 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.c
--rw-r--r--   0 pmind      (502) staff       (20)      397 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.h
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/typing.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.834888 chainsaddiction-0.2.4/src/chainsaddiction/utils/
--rw-r--r--   0 pmind      (502) staff       (20)      430 2023-07-02 11:08:18.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      207 2023-06-30 09:02:51.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/__init__.pyi
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.839293 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     1116 2023-07-02 14:25:01.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      169 2023-07-02 13:06:36.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2280 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.c
--rw-r--r--   0 pmind      (502) staff       (20)      248 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.h
--rw-r--r--   0 pmind      (502) staff       (20)     4882 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.c
--rw-r--r--   0 pmind      (502) staff       (20)      795 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.h
--rw-r--r--   0 pmind      (502) staff       (20)     3119 2023-07-01 19:30:23.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.c
--rw-r--r--   0 pmind      (502) staff       (20)     1467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.773143 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/
--rw-r--r--   0 pmind      (502) staff       (20)     3851 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     7974 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/SOURCES.txt
--rw-r--r--   0 pmind      (502) staff       (20)        1 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/dependency_links.txt
--rw-r--r--   0 pmind      (502) staff       (20)        6 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/requires.txt
--rw-r--r--   0 pmind      (502) staff       (20)       22 2023-07-03 19:28:33.000000 chainsaddiction-0.2.4/src/chainsaddiction.egg-info/top_level.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.908062 chainsaddiction-0.2.4/src/vmath/
--rw-r--r--   0 pmind      (502) staff       (20)      659 2023-07-02 10:49:38.000000 chainsaddiction-0.2.4/src/vmath/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      773 2023-07-02 10:49:20.000000 chainsaddiction-0.2.4/src/vmath/alloc.h
--rw-r--r--   0 pmind      (502) staff       (20)      440 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/config.h
--rw-r--r--   0 pmind      (502) staff       (20)     1473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/core.c
--rw-r--r--   0 pmind      (502) staff       (20)      932 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/core.h
--rw-r--r--   0 pmind      (502) staff       (20)     4047 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/print.h
--rw-r--r--   0 pmind      (502) staff       (20)     1349 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)     2907 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)      682 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/stats.c
--rw-r--r--   0 pmind      (502) staff       (20)     1008 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/stats.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.924279 chainsaddiction-0.2.4/src/vmath/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      807 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)     1294 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/tests/runtest.c
--rw-r--r--   0 pmind      (502) staff       (20)     2573 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_rnd.c
--rw-r--r--   0 pmind      (502) staff       (20)      344 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_rnd.h
--rw-r--r--   0 pmind      (502) staff       (20)     1108 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_stats.c
--rw-r--r--   0 pmind      (502) staff       (20)      273 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_stats.h
--rw-r--r--   0 pmind      (502) staff       (20)    23250 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)     1182 2023-07-02 20:06:40.000000 chainsaddiction-0.2.4/src/vmath/tests/test_vmath.h
--rw-r--r--   0 pmind      (502) staff       (20)    13402 2023-07-02 19:08:05.000000 chainsaddiction-0.2.4/src/vmath/vmath.c
--rw-r--r--   0 pmind      (502) staff       (20)    18516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/src/vmath/vmath.h
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.932782 chainsaddiction-0.2.4/tests/
--rw-r--r--   0 pmind      (502) staff       (20)      142 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/Makefile
--rw-r--r--   0 pmind      (502) staff       (20)      179 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/README
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.949621 chainsaddiction-0.2.4/tests/data/
--rw-r--r--   0 pmind      (502) staff       (20)     1299 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N100
--rw-r--r--   0 pmind      (502) staff       (20)     6535 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N500
--rw-r--r--   0 pmind      (502) staff       (20)      967 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/S4_N50_MID
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.950674 chainsaddiction-0.2.4/tests/data/centroids/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.973070 chainsaddiction-0.2.4/tests/data/centroids/2s/
--rw-r--r--   0 pmind      (502) staff       (20)        8 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68467 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       43 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    68421 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    72888 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.991444 chainsaddiction-0.2.4/tests/data/centroids/3s/
--rw-r--r--   0 pmind      (502) staff       (20)       12 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      187 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102650 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       64 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   102555 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   105803 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.010329 chainsaddiction-0.2.4/tests/data/centroids/4s/
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      356 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135537 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)       85 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   135631 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   141473 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.032920 chainsaddiction-0.2.4/tests/data/centroids/5s/
--rw-r--r--   0 pmind      (502) staff       (20)       44 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      553 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      100 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      489 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170825 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)      107 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)   170730 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)   176569 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)     3010 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)     6164 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/centroids/centroids
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.034250 chainsaddiction-0.2.4/tests/data/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.043233 chainsaddiction-0.2.4/tests/data/earthquakes/2s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4872 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     4826 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     5138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       27 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)       93 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       42 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/2s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.057134 chainsaddiction-0.2.4/tests/data/earthquakes/3s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7304 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7249 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     7516 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       50 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      210 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       65 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/3s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.069407 chainsaddiction-0.2.4/tests/data/earthquakes/4s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9724 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9672 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)     9894 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       71 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      368 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       88 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/4s/local-decoding.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.082521 chainsaddiction-0.2.4/tests/data/earthquakes/5s/
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/global-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-delta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      493 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-gamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)       39 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/init-lambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12138 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lalpha.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12048 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lbeta.txt
--rw-r--r--   0 pmind      (502) staff       (20)    12274 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lcsp.txt
--rw-r--r--   0 pmind      (502) staff       (20)       76 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/ldelta.txt
--rw-r--r--   0 pmind      (502) staff       (20)      571 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/lgamma.txt
--rw-r--r--   0 pmind      (502) staff       (20)      110 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/llambda.txt
--rw-r--r--   0 pmind      (502) staff       (20)      214 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/5s/local-decoding.txt
--rw-r--r--   0 pmind      (502) staff       (20)      315 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/earthquakes/earthquakes
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/empty
--rw-r--r--   0 pmind      (502) staff       (20)       31 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_2s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_3s
--rw-r--r--   0 pmind      (502) staff       (20)       98 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_4s
--rw-r--r--   0 pmind      (502) staff       (20)      104 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/params_4s_MID
--rw-r--r--   0 pmind      (502) staff       (20)      206 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/test_15_100_50
--rw-r--r--   0 pmind      (502) staff       (20)       10 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/data/wrong_format
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.083673 chainsaddiction-0.2.4/tests/params/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:33.698583 chainsaddiction-0.2.4/tests/params/earthquakes/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.086097 chainsaddiction-0.2.4/tests/params/earthquakes/3/
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      127 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/3/random.p
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-07-03 19:28:34.089852 chainsaddiction-0.2.4/tests/params/earthquakes/4/
--rw-r--r--   0 pmind      (502) staff       (20)      250 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/linear.p
--rw-r--r--   0 pmind      (502) staff       (20)      228 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/quantile.p
--rw-r--r--   0 pmind      (502) staff       (20)      232 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/earthquakes/4/random.p
--rw-r--r--   0 pmind      (502) staff       (20)      199 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/params/params-4s
--rw-r--r--   0 pmind      (502) staff       (20)      862 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/test-ext-earthquakes.py
--rw-r--r--   0 pmind      (502) staff       (20)     1069 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/test-utils.py
--rw-r--r--   0 pmind      (502) staff       (20)     1084 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tests/utils.py
--rw-r--r--   0 pmind      (502) staff       (20)      101 2023-06-20 13:23:44.000000 chainsaddiction-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.411768 chainsaddiction-0.2.5.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.415768 chainsaddiction-0.2.5.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.415768 chainsaddiction-0.2.5.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.415768 chainsaddiction-0.2.5.dev0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.415768 chainsaddiction-0.2.5.dev0/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.415768 chainsaddiction-0.2.5.dev0/docs/source/api/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/internal.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.419768 chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-hmm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-probs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/c/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.419768 chainsaddiction-0.2.5.dev0/docs/source/api/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/python/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/python/poishmm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/api/python/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.419768 chainsaddiction-0.2.5.dev0/docs/source/usrguide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/usrguide/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/docs/source/usrguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.419768 chainsaddiction-0.2.5.dev0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/include/chainsaddiction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/include/libvmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:09:09.455768 chainsaddiction-0.2.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.411768 chainsaddiction-0.2.5.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.423768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/dataset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/err.h
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/libma.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/libma.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.427768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-em.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-em.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-fwbw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-fwbw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-hmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-hmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-params.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-params.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-probs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-probs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-object.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.427768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.427768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/earthquakes.lprobs
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/params-3s
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/params-4s
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/ppr1
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/ppr2
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/ppr3
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/ppr4
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/ppr5
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/data/std3s.poisparams
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/runtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-em.c
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-em.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-hmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-hmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-params.c
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-params.h
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-probs.c
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-probs.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/read.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/read.h
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/scalar.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.431768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/runtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-dataset.c
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-dataset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-read.c
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-read.h
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.431768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.431768 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/runtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/test-utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/test-utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils-module.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils-module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.423768 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-28 13:09:09.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-28 13:09:09.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:09:09.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 13:09:09.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:09:09.000000 chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.435768 chainsaddiction-0.2.5.dev0/src/vmath/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/core.c
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/print.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/rnd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/stats.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.435768 chainsaddiction-0.2.5.dev0/src/vmath/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/runtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_rnd.c
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23250 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_vmath.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/tests/test_vmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/vmath.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/src/vmath/vmath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.435768 chainsaddiction-0.2.5.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 13:08:49.000000 chainsaddiction-0.2.5.dev0/tests/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.435768 chainsaddiction-0.2.5.dev0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/S4_N100
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/S4_N500
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/S4_N50_MID
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.435768 chainsaddiction-0.2.5.dev0/tests/data/centroids/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.439768 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68467 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68421 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.439768 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102650 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   102555 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   105803 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.443768 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   135537 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   135631 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   141473 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.447768 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   170825 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   170730 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   176569 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/local-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/centroids/centroids
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.447768 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.447768 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/ldelta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lgamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/llambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.447768 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/ldelta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lgamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/llambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/ldelta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lgamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/llambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/local-decoding.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/global-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/init-delta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/init-gamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/init-lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lalpha.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lbeta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lcsp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/ldelta.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lgamma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/llambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/local-decoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/earthquakes/earthquakes
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/empty
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/params_2s
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/params_3s
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/params_4s
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/params_4s_MID
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/test_15_100_50
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/data/wrong_format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/tests/params/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.411768 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/3/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/3/linear.p
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/3/quantile.p
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/3/random.p
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:09:09.451768 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/4/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/4/linear.p
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/4/quantile.p
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/earthquakes/4/random.p
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/params/params-4s
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/test-ext-earthquakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/test-utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 13:08:50.000000 chainsaddiction-0.2.5.dev0/tox.ini
```

### Comparing `chainsaddiction-0.2.4/LICENSE` & `chainsaddiction-0.2.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/Makefile` & `chainsaddiction-0.2.5.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/PKG-INFO` & `chainsaddiction-0.2.5.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.4
+Version: 0.2.5.dev0
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -42,46 +42,45 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![build](https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml/badge.svg)](
+https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml)
+
 # ChainsAddiction
 
 ChainsAddiction is an easy to use tool for time series analysis using
 discrete-time Hidden Markov Models. It is written in `C` as a `numpy`-based
 Python extension module.
 
 
 ## Installation
-### Prerequisites
-
-The installation of ChainsAddiction requires to following tools to be installed
-on your system:
-
-- Python >= 3.9
-- pip, setuptools
-- C compiler
-
-
 ### Install from PyPi
 
-You can install chainsaddiction from PyPi with:
+We currently provide wheels for macOS and Windows AMD 64, which you can install from PyPI via:
 
     python3 -m pip install chainsaddiction
 
-Please note that ChainsAddiction is a CPython extension module. You have to
-have set up a C compiler in order to install. Currently we provide wheels for
-macOS. So, if you are using this OS you do not need a compiler.
+Linux users have to build from source until we get that manylinux thing running.
 
 
 ### Install from source
 
-First, clone the source code by typing the following command in your terminal app.
+Before attemting to build ChainsAddiction from source, make sure you have
+
+- Python >= 3.9
+- pip, setuptools
+- C compiler
+
+installed and ready to go.
+
+Then, clone the source code by typing the following command in your terminal app.
 Replace `path/to/ca` with the path to where ChainsAddiction should be cloned:
 
     git clone https://github.com/teagum/chainsaddiction path/to/ca
 
 Second, change to the root directory of your freshly cloned code repository:
 
     cd path/to/ca
```

### Comparing `chainsaddiction-0.2.4/README.md` & `chainsaddiction-0.2.5.dev0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,38 @@
+[![build](https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml/badge.svg)](
+https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml)
+
 # ChainsAddiction
 
 ChainsAddiction is an easy to use tool for time series analysis using
 discrete-time Hidden Markov Models. It is written in `C` as a `numpy`-based
 Python extension module.
 
 
 ## Installation
-### Prerequisites
-
-The installation of ChainsAddiction requires to following tools to be installed
-on your system:
-
-- Python >= 3.9
-- pip, setuptools
-- C compiler
-
-
 ### Install from PyPi
 
-You can install chainsaddiction from PyPi with:
+We currently provide wheels for macOS and Windows AMD 64, which you can install from PyPI via:
 
     python3 -m pip install chainsaddiction
 
-Please note that ChainsAddiction is a CPython extension module. You have to
-have set up a C compiler in order to install. Currently we provide wheels for
-macOS. So, if you are using this OS you do not need a compiler.
+Linux users have to build from source until we get that manylinux thing running.
 
 
 ### Install from source
 
-First, clone the source code by typing the following command in your terminal app.
+Before attemting to build ChainsAddiction from source, make sure you have
+
+- Python >= 3.9
+- pip, setuptools
+- C compiler
+
+installed and ready to go.
+
+Then, clone the source code by typing the following command in your terminal app.
 Replace `path/to/ca` with the path to where ChainsAddiction should be cloned:
 
     git clone https://github.com/teagum/chainsaddiction path/to/ca
 
 Second, change to the root directory of your freshly cloned code repository:
 
     cd path/to/ca
```

### Comparing `chainsaddiction-0.2.4/docs/Makefile` & `chainsaddiction-0.2.5.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/make.bat` & `chainsaddiction-0.2.5.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/c/dataset.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/c/dataset.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-hmm.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-hmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-params.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-params.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/c/poishmm/pois-probs.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/c/poishmm/pois-probs.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/c/utils.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/c/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/python/poishmm.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/python/poishmm.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/api/python/utils.rst` & `chainsaddiction-0.2.5.dev0/docs/source/api/python/utils.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/conf.py` & `chainsaddiction-0.2.5.dev0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/getting-started.rst` & `chainsaddiction-0.2.5.dev0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/index.rst` & `chainsaddiction-0.2.5.dev0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/docs/source/usrguide/examples.rst` & `chainsaddiction-0.2.5.dev0/docs/source/usrguide/examples.rst`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/pyproject.toml` & `chainsaddiction-0.2.5.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chainsaddiction"
-version = "0.2.4"
+version = "0.2.5-dev0"
 authors = [{name = "Michael Blaß", email = "mblass@posteo.net"}]
 description = "HMM with Poisson-distributed latent variables."
 keywords = ["hmm", "poisson", "hidden-markov model"]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: BSD License",
```

### Comparing `chainsaddiction-0.2.4/setup.py` & `chainsaddiction-0.2.5.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,22 @@
         include_dirs = [
             'include',
             'src/vmath',
             'src/chainsaddiction',
             'src/chainsaddiction/utils',
             np.get_include(),
         ],
-        extra_compile_args = ['-Wall', '-Wextra'],
         language = 'c')
 
 poishmm = Extension('chainsaddiction.poishmm',
         sources = list_source_files(poishmm_src),
         include_dirs =  [
             'include',
             'src/vmath',
             'src/chainsaddiction',
             'src/chainsaddiction/poishmm',
             np.get_include()
         ],
-        extra_compile_args = ['-Wall', '-Wextra'],
         language = 'c')
 
 
 setup(ext_modules = [utils, poishmm])
```

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/dataset.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/dataset.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/dataset.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/libma.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/libma.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/libma.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/libma.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/Makefile` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/__init__.pyi` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-em.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-em.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-fwbw.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-fwbw.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-fwbw.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-hmm.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-hmm.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-params.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-params.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-params.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-probs.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/pois-probs.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/pois-probs.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-module.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-module.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-module.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/poishmm-object.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/poishmm-object.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/Makefile` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/runtest.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-em.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-em.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-hmm.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-hmm.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-hmm.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-params.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-params.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/poishmm/tests/test-pois-probs.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/poishmm/tests/test-pois-probs.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/read.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/read.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/read.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/read.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/tests/Makefile` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/tests/runtest.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-dataset.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-dataset.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-dataset.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/tests/test-read.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/tests/test-read.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/Makefile` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/tests/test-utils.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/tests/test-utils.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils-module.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils-module.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils-module.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.c` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction/utils/utils.h` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction/utils/utils.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction.egg-info/PKG-INFO` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsaddiction
-Version: 0.2.4
+Version: 0.2.5.dev0
 Summary: HMM with Poisson-distributed latent variables.
 Author-email: Michael Blaß <mblass@posteo.net>
 License: Copyright 2019 Michael Blaß michael.blass@uni-hamburg.de
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -42,46 +42,45 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![build](https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml/badge.svg)](
+https://github.com/Teagum/chainsaddiction/actions/workflows/build.yml)
+
 # ChainsAddiction
 
 ChainsAddiction is an easy to use tool for time series analysis using
 discrete-time Hidden Markov Models. It is written in `C` as a `numpy`-based
 Python extension module.
 
 
 ## Installation
-### Prerequisites
-
-The installation of ChainsAddiction requires to following tools to be installed
-on your system:
-
-- Python >= 3.9
-- pip, setuptools
-- C compiler
-
-
 ### Install from PyPi
 
-You can install chainsaddiction from PyPi with:
+We currently provide wheels for macOS and Windows AMD 64, which you can install from PyPI via:
 
     python3 -m pip install chainsaddiction
 
-Please note that ChainsAddiction is a CPython extension module. You have to
-have set up a C compiler in order to install. Currently we provide wheels for
-macOS. So, if you are using this OS you do not need a compiler.
+Linux users have to build from source until we get that manylinux thing running.
 
 
 ### Install from source
 
-First, clone the source code by typing the following command in your terminal app.
+Before attemting to build ChainsAddiction from source, make sure you have
+
+- Python >= 3.9
+- pip, setuptools
+- C compiler
+
+installed and ready to go.
+
+Then, clone the source code by typing the following command in your terminal app.
 Replace `path/to/ca` with the path to where ChainsAddiction should be cloned:
 
     git clone https://github.com/teagum/chainsaddiction path/to/ca
 
 Second, change to the root directory of your freshly cloned code repository:
 
     cd path/to/ca
```

### Comparing `chainsaddiction-0.2.4/src/chainsaddiction.egg-info/SOURCES.txt` & `chainsaddiction-0.2.5.dev0/src/chainsaddiction.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements-dev.txt
 setup.py
 tox.ini
+.github/workflows/release.yml
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/getting-started.rst
 docs/source/index.rst
 docs/source/api/index.rst
 docs/source/api/c/basics.rst
```

### Comparing `chainsaddiction-0.2.4/src/vmath/Makefile` & `chainsaddiction-0.2.5.dev0/src/vmath/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/alloc.h` & `chainsaddiction-0.2.5.dev0/src/vmath/alloc.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/core.c` & `chainsaddiction-0.2.5.dev0/src/vmath/core.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/core.h` & `chainsaddiction-0.2.5.dev0/src/vmath/core.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/print.h` & `chainsaddiction-0.2.5.dev0/src/vmath/print.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/rnd.c` & `chainsaddiction-0.2.5.dev0/src/vmath/rnd.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/rnd.h` & `chainsaddiction-0.2.5.dev0/src/vmath/rnd.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/stats.c` & `chainsaddiction-0.2.5.dev0/src/vmath/stats.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/stats.h` & `chainsaddiction-0.2.5.dev0/src/vmath/stats.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/Makefile` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/Makefile`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/runtest.c` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/runtest.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/test_rnd.c` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/test_rnd.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/test_stats.c` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/test_stats.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/test_vmath.c` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/test_vmath.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/tests/test_vmath.h` & `chainsaddiction-0.2.5.dev0/src/vmath/tests/test_vmath.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/vmath.c` & `chainsaddiction-0.2.5.dev0/src/vmath/vmath.c`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/src/vmath/vmath.h` & `chainsaddiction-0.2.5.dev0/src/vmath/vmath.h`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/S4_N100` & `chainsaddiction-0.2.5.dev0/tests/data/S4_N100`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/S4_N500` & `chainsaddiction-0.2.5.dev0/tests/data/S4_N500`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/S4_N50_MID` & `chainsaddiction-0.2.5.dev0/tests/data/S4_N50_MID`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/2s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/2s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/2s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/3s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/3s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/3s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/4s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/4s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/4s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/gamma.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/gamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/global-decoding.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/global-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/5s/local-decoding.txt` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/5s/local-decoding.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/centroids/centroids` & `chainsaddiction-0.2.5.dev0/tests/data/centroids/centroids`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/2s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/2s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/3s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/3s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/4s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/4s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lalpha.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lalpha.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lbeta.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lbeta.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lcsp.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lcsp.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/data/earthquakes/5s/lgamma.txt` & `chainsaddiction-0.2.5.dev0/tests/data/earthquakes/5s/lgamma.txt`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/test-ext-earthquakes.py` & `chainsaddiction-0.2.5.dev0/tests/test-ext-earthquakes.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/test-utils.py` & `chainsaddiction-0.2.5.dev0/tests/test-utils.py`

 * *Files identical despite different names*

### Comparing `chainsaddiction-0.2.4/tests/utils.py` & `chainsaddiction-0.2.5.dev0/tests/utils.py`

 * *Files identical despite different names*

