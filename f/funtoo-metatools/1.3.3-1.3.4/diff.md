# Comparing `tmp/funtoo-metatools-1.3.3.tar.gz` & `tmp/funtoo-metatools-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-metatools-1.3.3.tar", last modified: Thu Jul 13 22:10:46 2023, max compression
+gzip compressed data, was "funtoo-metatools-1.3.4.tar", last modified: Fri Jul 28 20:54:17 2023, max compression
```

## Comparing `funtoo-metatools-1.3.3.tar` & `funtoo-metatools-1.3.4.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.825162 funtoo-metatools-1.3.3/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12021 2023-07-13 22:10:34.000000 funtoo-metatools-1.3.3/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-07-13 22:09:26.000000 funtoo-metatools-1.3.3/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.3/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-06-21 02:46:04.000000 funtoo-metatools-1.3.3/bin/blos-check
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5765 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.3/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.3/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.3/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.3/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25579 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    24204 2023-07-10 01:16:20.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9207 2023-07-10 01:39:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8445 2023-07-10 01:39:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2065 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-03 19:14:35.000000 funtoo-metatools-1.3.3/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/blos.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1287 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.3/metatools/cmd.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5554 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.3/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8962 2023-07-10 01:51:18.000000 funtoo-metatools-1.3.3/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27292 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    35014 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21796 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-06-21 02:40:21.000000 funtoo-metatools-1.3.3/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17658 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.3/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-07-13 22:10:42.000000 funtoo-metatools-1.3.3/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/yaml_util.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/zmq/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:08:14.000000 funtoo-metatools-1.3.3/metatools/zmq/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/app_core.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/key_monkey.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_breezyops.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-07-13 22:10:46.825162 funtoo-metatools-1.3.3/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-07-13 22:10:42.000000 funtoo-metatools-1.3.3/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.3/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12702 2023-07-28 20:54:01.000000 funtoo-metatools-1.3.4/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.4/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1492 2023-07-24 19:21:40.000000 funtoo-metatools-1.3.4/ROADMAP.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-07-28 20:49:44.000000 funtoo-metatools-1.3.4/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.313351 funtoo-metatools-1.3.4/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.4/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-06-21 02:46:04.000000 funtoo-metatools-1.3.4/bin/blos-check
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      105 2023-07-28 18:26:02.000000 funtoo-metatools-1.3.4/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5765 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.4/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.4/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.4/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.4/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.313351 funtoo-metatools-1.3.4/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.4/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.317350 funtoo-metatools-1.3.4/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25579 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    24226 2023-07-19 20:46:06.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9207 2023-07-10 01:39:44.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11198 2023-07-19 21:01:27.000000 funtoo-metatools-1.3.4/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.321351 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-28 20:54:17.000000 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2077 2023-07-28 20:54:17.000000 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-07-28 20:54:17.000000 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-07-28 20:54:17.000000 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-07-28 20:54:17.000000 funtoo-metatools-1.3.4/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-03 19:14:35.000000 funtoo-metatools-1.3.4/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.321351 funtoo-metatools-1.3.4/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/blos.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1287 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.4/metatools/cmd.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5554 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.4/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.4/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8962 2023-07-10 01:51:18.000000 funtoo-metatools-1.3.4/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27465 2023-07-28 18:28:53.000000 funtoo-metatools-1.3.4/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    35014 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.4/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21796 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.4/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-06-21 02:40:21.000000 funtoo-metatools-1.3.4/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17658 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.4/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-07-28 20:54:13.000000 funtoo-metatools-1.3.4/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/metatools/zmq/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:08:14.000000 funtoo-metatools-1.3.4/metatools/zmq/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.4/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-07-28 20:54:17.325351 funtoo-metatools-1.3.4/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-07-28 20:54:13.000000 funtoo-metatools-1.3.4/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.4/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.4/subpop.yaml
```

### Comparing `funtoo-metatools-1.3.3/.pre-commit-config.yaml` & `funtoo-metatools-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/ChangeLog.rst` & `funtoo-metatools-1.3.4/ChangeLog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+metatools 1.3.4
+===============
+
+Released on July 28, 2023.
+
+This is a maintenance/general update release.
+
+* A hopefully (and I believe) "final fix" for HTTP 304
+  responses not being properly handled. For some reason,
+  I was not reading this code correctly and it should
+  now be totally fixed.
+
+* Adding of a ``ROADMAP.rst`` to remind me of things to
+  work on.
+
+* Catch ``ssl.SSLError`` as it appears httpx doesn't
+  catch this exception, so we must catch it and handle
+  it. This fixes an issue where invalid/expired SSL
+  certs would cause a traceback rather than a "fallback"
+  behavior.
+
+* FL-11447: merge invakid404's improvements to support
+  git-sourced rust crates.
+
 metatools 1.3.3
 ===============
 
 Released on July 13, 2023.
 
 This is a maintenance/general update release.
 
@@ -27,15 +51,15 @@
   be inspected for error code, etc.) and the combined string of
   stdout and stderr.
 
 * For dynamic archives: ``Archive`` now has a ``work_path`` and
   an async ``create_work_path`` method. This can be used as a
   'scratch area' for temporary work. Do an::
 
-   await myarchive.create_work_path()
+    await myarchive.create_work_path()
 
   ``myarchive.work_path`` is now empty and ready for use.
 
   ``Archive`` ``.store()`` and ``.store_by_name()`` now accept
   an ``existing=`` keyword argument which can be used to point
   to an archive/file that already exists. This will allow you
   to basically say "THIS is the archive I wish to store -- I
```

### Comparing `funtoo-metatools-1.3.3/PKG-INFO` & `funtoo-metatools-1.3.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.3
+Version: 1.3.4
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.3/README.rst` & `funtoo-metatools-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/blos` & `funtoo-metatools-1.3.4/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/blos-check` & `funtoo-metatools-1.3.4/bin/blos-check`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/deepdive` & `funtoo-metatools-1.3.4/bin/deepdive`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/deepquery` & `funtoo-metatools-1.3.4/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/distfile-kit-fetch` & `funtoo-metatools-1.3.4/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/distfile-stats` & `funtoo-metatools-1.3.4/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/doit` & `funtoo-metatools-1.3.4/bin/doit`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/fastpull-daemon` & `funtoo-metatools-1.3.4/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/fastpull-daemon-ng` & `funtoo-metatools-1.3.4/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/fastpull-fixer` & `funtoo-metatools-1.3.4/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/fetch` & `funtoo-metatools-1.3.4/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/interkit-links` & `funtoo-metatools-1.3.4/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/list-kits` & `funtoo-metatools-1.3.4/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/mcafee-tool` & `funtoo-metatools-1.3.4/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/merge-gentoo-staging` & `funtoo-metatools-1.3.4/bin/merge-gentoo-staging`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/merge-kits` & `funtoo-metatools-1.3.4/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/missing-links` & `funtoo-metatools-1.3.4/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/release-yaml-test` & `funtoo-metatools-1.3.4/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/reposcan` & `funtoo-metatools-1.3.4/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/storage-test` & `funtoo-metatools-1.3.4/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/bin/test-metadata-extract` & `funtoo-metatools-1.3.4/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/deprecated/mongo_backends.py` & `funtoo-metatools-1.3.4/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/Makefile` & `funtoo-metatools-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.3.4/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.3.4/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/autogen-dev.rst` & `funtoo-metatools-1.3.4/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/autogen.rst` & `funtoo-metatools-1.3.4/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/conf.py` & `funtoo-metatools-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.3.4/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.3.4/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.3.4/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/index.rst` & `funtoo-metatools-1.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/install.rst` & `funtoo-metatools-1.3.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/intro.rst` & `funtoo-metatools-1.3.4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/docs/meta-repo.rst` & `funtoo-metatools-1.3.4/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/ebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import asyncio
 import logging
 import os
 import shutil
 import threading
 from asyncio import Task
 from collections import OrderedDict
+from collections.abc import Mapping
 from datetime import datetime
 from subprocess import getstatusoutput
 from typing import Optional, Tuple
 
 import jinja2
 
 from metatools.cmd import capture_bg
@@ -514,25 +515,24 @@
 		catpkg of this BreezyBuild. We use this for writing new entries to the Distfile Integrity database for
 		to-be-fetched artifacts.
 		"""
 
 		fetch_tasks_dict = {}
 
 		for artifact in self.iter_artifacts():
-			art_type = type(artifact)
-			if art_type not in [Artifact, Archive]:
+			if isinstance(artifact, Mapping):
 				artifact = Artifact(**artifact)
 
 			# This records that the artifact is used by this catpkg, because an Artifact can be shared among multiple
 			# catpkgs. This is used for the integrity database writes:
 
 			if self not in artifact.breezybuilds:
 				artifact.breezybuilds.append(self)
 
-			if art_type is Artifact:
+			if artifact.__class__.__name__ == "Artifact":
 				async def lil_coroutine(a):
 					try:
 						status = await a.ensure_completed()
 						return a, status
 					except Exception as e:
 						pkgtools.model.log.error(e, exc_info=True)
 						raise e
```

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/fetch.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/fetch.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/github.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/github.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/golang.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/golang.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/http.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/http.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/funtoo/pkgtools/rust.py` & `funtoo-metatools-1.3.4/funtoo/pkgtools/rust.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import glob
 import os
 import subprocess
 import toml
 import asyncio
 import hashlib
 import shutil
+import urllib
+from collections import defaultdict
 
 from subpop.util import AttrDict
 
 from metatools.cmd import run_shell
 
+# TODO: although this is currently working, it's not recommended.
+#       we should look into using non-dyne references to these classes more.
+# from funtoo.pkgtools.ebuild import Artifact, Archive
+import dyne.org.funtoo.metatools.pkgtools as pkgtools
+
 
 async def add_crates_bundle(
 	hub,
 	pkginfo,
 	cargo_lock_data=None,
 	cargo_lock_path=None,
 	src_artifact=None,
@@ -66,25 +73,25 @@
 
 		src_dir = glob.glob(os.path.join(src_artifact.extract_path, src_dir_glob))[0]
 
 		cargo_lock_path = os.path.join(src_dir, "Cargo.lock")
 		if not os.path.exists(cargo_lock_path):
 			cargo_cmd = subprocess.Popen(["cargo", "update"], cwd=src_dir).wait()
 
-		crates, pkginfo["crates_bundle"].crates_attrs = generate_crates_metadata(
+		crates, pkginfo["crates_bundle"].crates_artifacts = await generate_crates_metadata(
 			lock_path=cargo_lock_path
 		)
 
 		src_artifact.cleanup()
 	elif cargo_lock_data:
-		crates, pkginfo["crates_bundle"].crates_attrs = generate_crates_metadata(
+		crates, pkginfo["crates_bundle"].crates_artifacts = await generate_crates_metadata(
 			lock_data=cargo_lock_data
 		)
 	elif cargo_lock_path:
-		crates, pkginfo["crates_bundle"].crates_attrs = generate_crates_metadata(
+		crates, pkginfo["crates_bundle"].crates_artifacts = await generate_crates_metadata(
 			lock_path=cargo_lock_path
 		)
 	else:
 		raise ValueError("No source of `Cargo.lock` provided.")
 
 	crates_hash = hashlib.sha512(crates.encode("utf-8")).hexdigest()
 
@@ -135,34 +142,96 @@
 
 	if crates_archive:
 		return crates_archive
 
 	crates_archive = hub.Archive(crates_bundle.final_name)
 	await crates_archive.initialize(f"funtoo-crates-bundle-{pkginfo['name']}")
 
-	crates_artifacts = [
-		hub.pkgtools.ebuild.Artifact(**crate_attrs)
-		for crate_attrs in crates_bundle.crates_attrs
-	]
+	crates_artifacts = crates_bundle.crates_artifacts
 
 	# Fetch crates in parallel
-	await asyncio.gather(*[artifact.fetch() for artifact in crates_artifacts])
+	await asyncio.gather(*[artifact.ensure_completed() for artifact in crates_artifacts])
 
 	for artifact in crates_artifacts:
 		shutil.copy(
 			artifact.blos_object.blob.path,
 			os.path.join(crates_archive.top_path, artifact.final_name),
 		)
 
 	await crates_archive.store(key=crates_bundle["key"])
 
 	return crates_archive
 
 
-def generate_crates_metadata(lock_path=None, lock_data=None):
+async def fetch_git_dependency(url, crates):
+	parsed_url = urllib.parse.urlparse(url)
+
+	ref = parsed_url.fragment
+	repo_url = parsed_url._replace(fragment="", query="").geturl()
+
+	repo_name = urllib.parse.quote(repo_url, safe="")
+
+	archive_name = f"{repo_name}-{ref}.tar.xz"
+	archive_key = AttrDict({"git_url": repo_url, "ref": ref})
+
+	# archive, _ = Archive.find(key=archive_key, final_name=archive_name)
+	archive, _ = pkgtools.ebuild.Archive.find(key=archive_key, final_name=archive_name)
+	if archive is None:
+		# archive = Archive(final_name=archive_name)
+		archive = pkgtools.ebuild.Archive(final_name=archive_name)
+
+		dir_name = f"{repo_name}-{ref}"
+		await archive.initialize(dir_name)
+
+		await run_shell(f"git clone --depth=1 {repo_url} {archive.top_path}")
+		await run_shell(
+			f"(cd {archive.top_path} && git fetch origin {ref} && git reset --hard {ref})"
+		)
+		await run_shell(
+			f"(cd {archive.top_path} && git submodule update --init --recursive)"
+		)
+
+		crate_locations = {}
+		for cargo_path in glob.glob(
+				os.path.join(archive.top_path, "**/Cargo.toml"), recursive=True
+		):
+			with open(cargo_path, "r") as cargo_file:
+				cargo_data = cargo_file.read()
+
+			cargo_data = toml.loads(cargo_data)
+
+			cargo_package_data = cargo_data.get("package", None)
+			if cargo_package_data is None:
+				continue
+
+			cargo_package_name = cargo_package_data.get("name", None)
+			if cargo_package_name is None:
+				continue
+
+			crate_locations[cargo_package_name] = os.path.relpath(
+				os.path.dirname(cargo_path), os.path.dirname(archive.top_path)
+			)
+
+		cargo_config_content = f"[patch.'{repo_url}']\n"
+		for crate in crates:
+			crate_location = crate_locations[crate]
+
+			cargo_config_content += f"{crate} = {{ path = \"{os.path.join('%CRATES_DIR%', crate_location)}\" }}\n"
+
+		with open(
+				os.path.join(archive.top_path, "funtoo_config.toml"), "w"
+		) as config_file:
+			config_file.write(cargo_config_content)
+
+		await archive.store(key=archive_key)
+
+	return archive
+
+
+async def generate_crates_metadata(lock_path=None, lock_data=None):
 	"""
 	This function generates crates data for the CRATES variable used in ebuilds, and also returns a
 	list of attributes to use to create new Artifacts for all crates that need to be downloaded to
 	build the project.
 	:param lock_path: If provided, open this Cargo.lock file and read its contents (string)
 	:param lock_data: If provided, this is a string containing the contents of Cargo.lock
 	:return: a tuple containing a string to use in CRATES, plus a list of attributes to use to
@@ -176,47 +245,69 @@
 		raise ValueError(
 			"No source of lock data provided. Please provide either `lock_path` or `lock_data`."
 		)
 
 	crates_dict = toml.loads(lock_data)
 
 	crates = ""
-	crates_attrs = []
+	crates_artifacts = []
+
+	git_crates = defaultdict(list)
 
 	for package in crates_dict["package"]:
 		if "source" not in package:
 			continue
 
-		crates = crates + package["name"] + "-" + package["version"] + "\n"
+		name = package["name"]
+		version = package["version"]
+		source = package["source"]
+
+		source_origin = "crates"
+
+		if source.startswith("git+"):
+			source_origin = "git"
+
+			url = source.lstrip("git+")
+
+			# Append ref to version so that ref changes reflect in the hash.
+			#
+			# Note that this breaks the legacy CRATES approach, which should
+			# be fine, as it doesn't support git crates either way. We do this
+			# instead of altering the hash computation to avoid recreating all
+			# existing cached archives.
+			ref = url.rsplit("#", 2)[-1]
+			version += f"-{ref}"
+
+			git_crates[url].append(name)
+
+		crates = crates + name + "-" + version + "\n"
+
+		if source_origin == "crates":
+			final_name = f"{name}-{version}.crate"
+
+			crates_artifacts.append(
+				# Artifact(
+				pkgtools.ebuild.Artifact(
+					url=(
+							"https://crates.io/api/v1/crates/"
+							+ name
+							+ "/"
+							+ version
+							+ "/download"
+					),
+					final_name=final_name,
+				)
+			)
 
-		crates_url = (
-			"https://crates.io/api/v1/crates/"
-			+ package["name"]
-			+ "/"
-			+ package["version"]
-			+ "/download"
-		)
-		crates_file = package["name"] + "-" + package["version"] + ".crate"
+	for url, contained_crates in git_crates.items():
+		git_archive = await fetch_git_dependency(url, contained_crates)
 
-		crates_attrs.append(dict(url=crates_url, final_name=crates_file))
+		crates_artifacts.append(git_archive)
 
-	return crates, crates_attrs
-
-
-async def get_crates_artifacts(lock_path):
-	"""
-	This method will extract package data from ``Cargo.lock`` and generate Artifacts for all packages it finds.
-	"""
-	crates, crates_attrs = generate_crates_metadata(lock_path=lock_path)
-
-	crates_artifacts = [
-		hub.pkgtools.ebuild.Artifact(**crate_attrs) for crate_attrs in crates_attrs
-	]
-
-	return dict(crates=crates, crates_artifacts=crates_artifacts)
+	return crates, crates_artifacts
 
 
 async def generate_crates_from_artifact(src_artifact, src_dir_glob="*"):
 	"""
 	IMPORTANT: It's now preferred to use ``add_crates_bundle`` instead, which uses dynamic archives
 	and avoids having hundreds of files in SRC_URI.
 
@@ -230,14 +321,14 @@
 	await src_artifact.fetch()
 	src_artifact.extract()
 
 	src_dir = glob.glob(os.path.join(src_artifact.extract_path, src_dir_glob))[0]
 
 	cargo_lock_path = os.path.join(src_dir, "Cargo.lock")
 	if not os.path.exists(cargo_lock_path):
-		result = await run_shell(["cargo", "update"], chdir=src_dir)
+		await run_shell(["cargo", "update"], chdir=src_dir)
 
-	artifacts = await get_crates_artifacts(cargo_lock_path)
+	crates, crates_artifacts = await generate_crates_metadata(lock_path=cargo_lock_path)
 
 	src_artifact.cleanup()
 
-	return artifacts
+	return dict(crates=crates, crates_artifacts=crates_artifacts)
```

### Comparing `funtoo-metatools-1.3.3/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.3.4/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.3
+Version: 1.3.4
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.3/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.3.4/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 ChangeLog.rst
 README.rst
+ROADMAP.rst
 VERSION
 make.sh
 setup.py
 setup.py.in
 subpop.yaml
 bin/blos
 bin/blos-check
```

### Comparing `funtoo-metatools-1.3.3/make.sh` & `funtoo-metatools-1.3.4/make.sh`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/blos.py` & `funtoo-metatools-1.3.4/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/cmd.py` & `funtoo-metatools-1.3.4/metatools/cmd.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/config/autogen.py` & `funtoo-metatools-1.3.4/metatools/config/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/config/base.py` & `funtoo-metatools-1.3.4/metatools/config/base.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/config/merge.py` & `funtoo-metatools-1.3.4/metatools/config/merge.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/context.py` & `funtoo-metatools-1.3.4/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/fastpull/core.py` & `funtoo-metatools-1.3.4/metatools/fastpull/core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/fastpull/spider.py` & `funtoo-metatools-1.3.4/metatools/fastpull/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import hashlib
 import logging
 import os
 import random
+import ssl
 import string
 import threading
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from datetime import datetime
 from json import JSONDecodeError
 from typing import Tuple, Dict
@@ -537,18 +538,21 @@
 		accept_304 = False
 		async with self.acquire_fetch_slot(request):
 			http_client = await self.acquire_http_client(request)
 			headers, auth = self.get_headers_and_auth(request)
 			# TODO: add code to explicitly close all clients, above:
 			try:
 				if extra_headers:
-					if "If-None-Match" in extra_headers or "If-Modified-Since" in headers:
-						accept_304 = True
 					headers.update(extra_headers)
 
+				for key_304 in [ "If-None-Match", "If-Modified-Since" ]:
+					if key_304 in http_client.headers or key_304 in headers:
+						accept_304 = True
+						break
+
 				response = await http_client.get(request.url, headers=headers, auth=auth, follow_redirects=True, timeout=15)
 				log.debug(f'http_fetch: GET {response.status_code} {request.url}')
 				if accept_304 and response.status_code == 304:
 					raise ContentNotModified()
 				if response.status_code != 200:
 					if response.status_code in [400, 404, 410]:
 						# No need to retry as the server has just told us that the resource does not exist.
@@ -559,27 +563,28 @@
 						err_response = response.json()
 					except JSONDecodeError:
 						err_response = response.text
 					log.error(
 						f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase} {err_response}")
 					if response.status_code == 304:
 						log.error("We should not get status 304 (not modified) but we did.")
-						log.error(f"Original request headers: {repr(http_client.headers)}")
+						log.error(f"  client request headers: {repr(http_client.headers)}")
+						log.error(f"headers passed to client: {repr(headers)} with auth: {repr(auth)}")
 						log.error(f"Extra headers:            {repr(extra_headers)}")
 					raise FetchError(request,
 									 f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase} {err_response}",
 									 retry=retry)
 				if is_json:
 					return response.headers, response.json()
 				if encoding:
 					result = response.headers, response.content.decode(encoding)
 				else:
 					result = response.headers, response.text
 				return result
-			except httpx.RequestError as re:
+			except (httpx.RequestError, ssl.SSLError) as re:
 				raise FetchError(request, f"Could not connect to {request.url}: {repr(re)}", retry=False)
 
 	@asynccontextmanager
 	async def acquire_download_slot(self):
 		"""
 		If you are inside this contextmanager, then it means you *have permission to start a download*.
```

### Comparing `funtoo-metatools-1.3.3/metatools/fetch_cache.py` & `funtoo-metatools-1.3.4/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/hashutils.py` & `funtoo-metatools-1.3.4/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/kit.py` & `funtoo-metatools-1.3.4/metatools/kit.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/kit_cache.py` & `funtoo-metatools-1.3.4/metatools/kit_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/metadata.py` & `funtoo-metatools-1.3.4/metatools/metadata.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/model.py` & `funtoo-metatools-1.3.4/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/pretty_logging.py` & `funtoo-metatools-1.3.4/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/steps.py` & `funtoo-metatools-1.3.4/metatools/steps.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/store.py` & `funtoo-metatools-1.3.4/metatools/store.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/tree.py` & `funtoo-metatools-1.3.4/metatools/tree.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/yaml_util.py` & `funtoo-metatools-1.3.4/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/zmq/app_core.py` & `funtoo-metatools-1.3.4/metatools/zmq/app_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/zmq/key_monkey.py` & `funtoo-metatools-1.3.4/metatools/zmq/key_monkey.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_breezyops.py` & `funtoo-metatools-1.3.4/metatools/zmq/zmq_msg_breezyops.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_core.py` & `funtoo-metatools-1.3.4/metatools/zmq/zmq_msg_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.3/setup.py` & `funtoo-metatools-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.3.3",
+	version="1.3.4",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
```

### Comparing `funtoo-metatools-1.3.3/setup.py.in` & `funtoo-metatools-1.3.4/setup.py.in`

 * *Files identical despite different names*

