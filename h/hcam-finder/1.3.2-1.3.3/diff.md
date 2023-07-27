# Comparing `tmp/hcam_finder-1.3.2.tar.gz` & `tmp/hcam_finder-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_finder-1.3.2.tar", last modified: Mon Jul 24 10:17:19 2023, max compression
+gzip compressed data, was "hcam_finder-1.3.3.tar", last modified: Thu Jul 27 22:12:18 2023, max compression
```

## Comparing `hcam_finder-1.3.2.tar` & `hcam_finder-1.3.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.402256 hcam_finder-1.3.2/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.2/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 10:17:19.402558 hcam_finder-1.3.2/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.2/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.390494 hcam_finder-1.3.2/docs/
--rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/docs/Makefile
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.384782 hcam_finder-1.3.2/docs/_build/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.384888 hcam_finder-1.3.2/docs/_build/html/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.392786 hcam_finder-1.3.2/docs/_build/html/_images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.2/docs/_build/html/_images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/_build/html/_images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/_build/html/_images/main.png
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.393797 hcam_finder-1.3.2/docs/_build/html/_static/
--rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/file.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.2/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.2/docs/conf.py
--rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.2/docs/hcam_finder.rst
--rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/hipercam.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.395518 hcam_finder-1.3.2/docs/images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.2/docs/images/main.png
--rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/index.rst
--rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/docs/make.bat
--rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.2/docs/modules.rst
--rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/ultracam.rst
--rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/docs/ultraspec.rst
--rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/docs/usage.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.397333 hcam_finder-1.3.2/hcam_finder/
--rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-24 10:17:05.000000 hcam_finder-1.3.2/hcam_finder/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     2462 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/hcam_finder/config.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.400687 hcam_finder-1.3.2/hcam_finder/data/
--rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.2/hcam_finder/data/Lato-Black.ttf
--rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.2/hcam_finder/data/Lato-Regular.ttf
--rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.2/hcam_finder/data/README.rst
--rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/data/config
--rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/data/configspec.ini
--rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.2/hcam_finder/data/guider_hole_arcseconds.txt
--rw-r--r--   0 sl         (501) staff       (20)    21032 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/finders.py
--rw-r--r--   0 sl         (501) staff       (20)     2808 2023-07-24 10:14:58.000000 hcam_finder-1.3.2/hcam_finder/finding_chart.py
--rw-r--r--   0 sl         (501) staff       (20)    10362 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/hcam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.2/hcam_finder/panstarrs.py
--rw-r--r--   0 sl         (501) staff       (20)     2414 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/hcam_finder/shapes.py
--rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.2/hcam_finder/skyview.py
--rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.2/hcam_finder/ucam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.2/hcam_finder/uspec_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.2/hcam_finder/ztf.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.398487 hcam_finder-1.3.2/hcam_finder.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-24 10:17:19.000000 hcam_finder-1.3.2/hcam_finder.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.401047 hcam_finder-1.3.2/scripts/
--rw-r--r--   0 sl         (501) staff       (20)    12564 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/hfinder
--rw-r--r--   0 sl         (501) staff       (20)    10866 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/ufinder
--rw-r--r--   0 sl         (501) staff       (20)    11371 2023-07-24 10:01:37.000000 hcam_finder-1.3.2/scripts/usfinder
--rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-24 10:17:19.403109 hcam_finder-1.3.2/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-24 10:17:05.000000 hcam_finder-1.3.2/setup.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-24 10:17:19.401466 hcam_finder-1.3.2/tests/
--rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/tests/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.2/tests/test_hcam_finder.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607489 hcam_finder-1.3.3/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.3/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-27 22:12:18.607561 hcam_finder-1.3.3/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.3/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.597465 hcam_finder-1.3.3/docs/
+-rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/docs/Makefile
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.594638 hcam_finder-1.3.3/docs/_build/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.594742 hcam_finder-1.3.3/docs/_build/html/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.599620 hcam_finder-1.3.3/docs/_build/html/_images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.3/docs/_build/html/_images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/_build/html/_images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/_build/html/_images/main.png
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.600475 hcam_finder-1.3.3/docs/_build/html/_static/
+-rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/plus.png
+-rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.3/docs/conf.py
+-rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.3/docs/hcam_finder.rst
+-rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/hipercam.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.602696 hcam_finder-1.3.3/docs/images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/images/main.png
+-rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/index.rst
+-rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/docs/make.bat
+-rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.3/docs/modules.rst
+-rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/ultracam.rst
+-rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/ultraspec.rst
+-rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/usage.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.604174 hcam_finder-1.3.3/hcam_finder/
+-rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-27 22:12:08.000000 hcam_finder-1.3.3/hcam_finder/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     2379 2023-07-24 10:46:18.000000 hcam_finder-1.3.3/hcam_finder/config.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.606811 hcam_finder-1.3.3/hcam_finder/data/
+-rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.3/hcam_finder/data/Lato-Black.ttf
+-rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.3/hcam_finder/data/Lato-Regular.ttf
+-rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.3/hcam_finder/data/README.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/data/config
+-rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/data/configspec.ini
+-rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.3/hcam_finder/data/guider_hole_arcseconds.txt
+-rw-r--r--   0 sl         (501) staff       (20)    21032 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/finders.py
+-rw-r--r--   0 sl         (501) staff       (20)     2804 2023-07-24 10:43:37.000000 hcam_finder-1.3.3/hcam_finder/finding_chart.py
+-rw-r--r--   0 sl         (501) staff       (20)    10394 2023-07-27 22:08:20.000000 hcam_finder-1.3.3/hcam_finder/hcam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.3/hcam_finder/panstarrs.py
+-rw-r--r--   0 sl         (501) staff       (20)     2358 2023-07-24 10:46:20.000000 hcam_finder-1.3.3/hcam_finder/shapes.py
+-rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.3/hcam_finder/skyview.py
+-rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.3/hcam_finder/ucam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/hcam_finder/uspec_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.3/hcam_finder/ztf.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.604843 hcam_finder-1.3.3/hcam_finder.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607163 hcam_finder-1.3.3/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)    12541 2023-07-24 14:23:43.000000 hcam_finder-1.3.3/scripts/hfinder
+-rw-r--r--   0 sl         (501) staff       (20)    10843 2023-07-24 14:23:41.000000 hcam_finder-1.3.3/scripts/ufinder
+-rw-r--r--   0 sl         (501) staff       (20)    11348 2023-07-24 14:23:57.000000 hcam_finder-1.3.3/scripts/usfinder
+-rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-27 22:12:18.607791 hcam_finder-1.3.3/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-27 22:12:08.000000 hcam_finder-1.3.3/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607387 hcam_finder-1.3.3/tests/
+-rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/tests/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/tests/test_hcam_finder.py
```

### Comparing `hcam_finder-1.3.2/CONTRIBUTING.rst` & `hcam_finder-1.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/LICENSE` & `hcam_finder-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/PKG-INFO` & `hcam_finder-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam_finder
-Version: 1.3.2
+Version: 1.3.3
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.2/README.rst` & `hcam_finder-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/Makefile` & `hcam_finder-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/_build/html/_images/compo.png` & `hcam_finder-1.3.3/docs/_build/html/_images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/_build/html/_images/inst.png` & `hcam_finder-1.3.3/docs/_build/html/_images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/_build/html/_images/main.png` & `hcam_finder-1.3.3/docs/_build/html/_images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/conf.py` & `hcam_finder-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/hcam_finder.rst` & `hcam_finder-1.3.3/docs/hcam_finder.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/hipercam.rst` & `hcam_finder-1.3.3/docs/hipercam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/images/compo.png` & `hcam_finder-1.3.3/docs/images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/images/inst.png` & `hcam_finder-1.3.3/docs/images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/images/main.png` & `hcam_finder-1.3.3/docs/images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/make.bat` & `hcam_finder-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/ultracam.rst` & `hcam_finder-1.3.3/docs/ultracam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/docs/usage.rst` & `hcam_finder-1.3.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/config.py` & `hcam_finder-1.3.3/hcam_finder/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # read in config
 from __future__ import absolute_import, print_function, division
 import configobj
-import pkg_resources
+import importlib
 import os
 import validate
 
 
-def check_user_dir(g, app_name='hfinder'):
+def check_user_dir(g, app_name="hfinder"):
     """
     Check directories exist for saving apps/configs etc. Create if not.
     """
-    direc = os.path.expanduser('~/.' + app_name)
+    direc = os.path.expanduser("~/." + app_name)
     if not os.path.exists(direc):
         try:
             os.mkdir(direc)
         except Exception as err:
-            g.clog.warn('Failed to make directory ' + str(err))
+            g.clog.warn("Failed to make directory " + str(err))
 
 
-def load_config(g, app_name='hfinder', env_var='HCAM_FINDER_CONF'):
+def load_config(g, app_name="hfinder", env_var="HCAM_FINDER_CONF"):
     """
     Populate application level globals from config file
     """
-    configspec_file = pkg_resources.resource_filename('hcam_finder',
-                                                      'data/configspec.ini')
+    configspec_file = str(
+        importlib.resources.files("hcam_finder") / "data/configspec.ini"
+    )
     # try and load config file.
     # look in the following locations in order
     # - HCAM_FINDER_CONF environment variable
     # - ~/.hfinder directory
     # - package resources
     paths = []
     if env_var in os.environ:
         paths.append(os.environ[env_var])
-    paths.append(os.path.expanduser('~/.' + app_name))
-    resource_dir = pkg_resources.resource_filename('hcam_finder', 'data')
+    paths.append(os.path.expanduser("~/." + app_name))
+    resource_dir = str(importlib.resources.files("hcam_finder") / "data")
     paths.append(resource_dir)
 
     # now load config file
     config = configobj.ConfigObj({}, configspec=configspec_file)
     for loc in paths:
         try:
             with open(os.path.join(loc, "config")) as source:
@@ -46,27 +47,29 @@
         except IOError:
             pass
 
     # validate ConfigObj, filling defaults from configspec if missing from config file
     validator = validate.Validator()
     result = config.validate(validator)
     if result is not True:
-        g.clog.warn('Config file validation failed')
+        g.clog.warn("Config file validation failed")
 
     # now update globals with config
     g.cpars.update(config)
 
 
-def write_config(g, app_name='hfinder'):
+def write_config(g, app_name="hfinder"):
     """
     Dump application level globals to config file
     """
-    configspec_file = pkg_resources.resource_filename('hcam_finder',
-                                                      'data/configspec.ini')
+    configspec_file = str(
+        importlib.resources.files("hcam_finder") / "data/configspec.ini"
+    )
+
     config = configobj.ConfigObj({}, configspec=configspec_file)
     config.update(g.cpars)
-    config.filename = os.path.expanduser('~/.{}/config'.format(app_name))
+    config.filename = os.path.expanduser("~/.{}/config".format(app_name))
     if not os.path.exists(config.filename):
         try:
             config.write()
         except Exception as err:
             g.clog.warn("Could not write config file:\n" + str(err))
```

### Comparing `hcam_finder-1.3.2/hcam_finder/data/Lato-Black.ttf` & `hcam_finder-1.3.3/hcam_finder/data/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/data/Lato-Regular.ttf` & `hcam_finder-1.3.3/hcam_finder/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/data/config` & `hcam_finder-1.3.3/hcam_finder/data/config`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/data/configspec.ini` & `hcam_finder-1.3.3/hcam_finder/data/configspec.ini`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/data/guider_hole_arcseconds.txt` & `hcam_finder-1.3.3/hcam_finder/data/guider_hole_arcseconds.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/finders.py` & `hcam_finder-1.3.3/hcam_finder/finders.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/finding_chart.py` & `hcam_finder-1.3.3/hcam_finder/finding_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, absolute_import, unicode_literals, division
-import pkg_resources
+import importlib
 import six
 from os.path import expanduser
 
 if not six.PY3:
     import tkFileDialog as filedialog
 else:
     from tkinter import filedialog
@@ -72,19 +72,19 @@
             dec=dec,
             pa=pa,
             wins=wins,
             version=version,
         )
     )
     font_size = 5
-    font_file = pkg_resources.resource_filename("hcam_finder", "data/Lato-Regular.ttf")
+    font_file = importlib.resources.files("hcam_finder") / "data/Lato-Regular.ttf"
     text_x = 0.0
     while text_x / width < 0.4:
         font_size += 1
-        font = ImageFont.truetype(font_file, font_size)
+        font = ImageFont.truetype(str(font_file), font_size)
         _, _, text_x, text_y = max((font.getbbox(txt) for txt in info_msg.splitlines()))
 
     nlines = len(info_msg.splitlines()) + 1
     rect_x, rect_y = int(1.1 * text_x), nlines * int(text_y)
     rectangle = Image.new("RGBA", (rect_x, rect_y), (255, 255, 255, 200))
 
     width, height = image.size
```

### Comparing `hcam_finder-1.3.2/hcam_finder/hcam_finder.py` & `hcam_finder-1.3.3/hcam_finder/hcam_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 if not six.PY3:
     import tkFileDialog as filedialog
 else:
     from tkinter import filedialog
 
 
 class HCAMFovSetter(FovSetter):
-
     overlay_names = ["ccd_overlay", "compo_overlay"]
 
     def window_string(self):
         g = get_root(self).globals
         wframe = g.ipars.wframe
         if g.ipars.isFF():
             winlist = []
@@ -61,16 +60,17 @@
             print("Aborted save to disk")
             return False
 
         g = get_root(self).globals
         data = dict()
         data["appdata"] = g.ipars.dumpJSON()
 
-        # add compo setup info
-        data["compo"] = g.compo_hw.dumpJSON()
+        # add compo setup info, if used
+        if g.ipars.compo():
+            data["compo"] = g.compo_hw.dumpJSON()
 
         # add user info that we should know of
         # includes target, user and proposal
         user = dict()
         user["target"] = self.targName.value()
         data["user"] = user
 
@@ -134,15 +134,15 @@
         self.ra_as_drawn, self.dec_as_drawn = ra, dec
 
         obj = self.canvas.get_object_by_tag("ccd_overlay")
         obj.move_delta(xn - xc, yn - yc)
 
         obj = self.canvas.get_object_by_tag("compo_overlay")
         obj.move_delta(xn - xc, yn - yc)
-        
+
         self.canvas.update_canvas()
 
     def _make_ccd(self, image):
         """
         Converts the current instrument settings to a ginga canvas object
         """
         # get window pair object from top widget
```

### Comparing `hcam_finder-1.3.2/hcam_finder/panstarrs.py` & `hcam_finder-1.3.3/hcam_finder/panstarrs.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/shapes.py` & `hcam_finder-1.3.3/hcam_finder/shapes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import pkg_resources
 import numpy as np
 from astropy import units as u
 
 from ginga.util import wcs
 from ginga.canvas.types.all import Polygon, Path
 from ginga.util.bezier import get_bezier
 
 from hcam_widgets.compo.utils import field_stop_centre, gtc_focalplane_equivalencies
 
 
 class CCDWin(Polygon):
-    def __init__(self, ra_ll_deg, dec_ll_deg, xs, ys,
-                 image, **params):
+    def __init__(self, ra_ll_deg, dec_ll_deg, xs, ys, image, **params):
         """
         Shape for drawing ccd window
 
         Parameters
         ----------
         ra_ll_deg : float
             lower left coordinate in ra (deg)
@@ -28,46 +26,44 @@
         image : `~ginga.AstroImage`
             image to plot Window on
         """
         points_wcs = (
             (ra_ll_deg, dec_ll_deg),
             wcs.add_offset_radec(ra_ll_deg, dec_ll_deg, xs, 0.0),
             wcs.add_offset_radec(ra_ll_deg, dec_ll_deg, xs, ys),
-            wcs.add_offset_radec(ra_ll_deg, dec_ll_deg, 0.0, ys)
+            wcs.add_offset_radec(ra_ll_deg, dec_ll_deg, 0.0, ys),
         )
         self.points = [image.radectopix(ra, dec) for (ra, dec) in points_wcs]
         super(CCDWin, self).__init__(self.points, **params)
-        self.name = params.pop('name', 'window')
+        self.name = params.pop("name", "window")
 
 
 class CompoPatrolArc(Path):
     def __init__(self, ra_ctr_deg, dec_ctr_deg, image, **params):
         """
         Shape for drawing allowed control arc, made using Bezier curves
 
         Parameters
         ----------
         ra_ctr_deg, dec_ctr_deg : float
               Tel pointing center (deg)
         image : `~ginga.AstroImage`
               image to plot Window on
         """
-        
-        theta = np.linspace(-65, 65, 40)*u.deg
+
+        theta = np.linspace(-65, 65, 40) * u.deg
 
         # circular arc, swapping dec sign
         X, Y = field_stop_centre(theta)
         points = u.Quantity([X, -Y])
         # transform to shape (N, 2) and units of degrees
         with u.set_enabled_equivalencies(gtc_focalplane_equivalencies):
             points = points.T.to_value(u.deg)
         # add offsets to pointing center
         points_wcs = [
-            wcs.add_offset_radec(ra_ctr_deg, dec_ctr_deg, p[0], p[1])
-            for p in points
+            wcs.add_offset_radec(ra_ctr_deg, dec_ctr_deg, p[0], p[1]) for p in points
         ]
 
         self.points = [image.radectopix(ra, dec) for (ra, dec) in points_wcs]
         self.bezier = get_bezier(30, self.points)
         super(CompoPatrolArc, self).__init__(self.points, **params)
-        self.name = params.pop('name', 'patrol_arc')
-
+        self.name = params.pop("name", "patrol_arc")
```

### Comparing `hcam_finder-1.3.2/hcam_finder/skyview.py` & `hcam_finder-1.3.3/hcam_finder/skyview.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/ucam_finder.py` & `hcam_finder-1.3.3/hcam_finder/ucam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/uspec_finder.py` & `hcam_finder-1.3.3/hcam_finder/uspec_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder/ztf.py` & `hcam_finder-1.3.3/hcam_finder/ztf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/hcam_finder.egg-info/PKG-INFO` & `hcam_finder-1.3.3/hcam_finder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hcam-finder
-Version: 1.3.2
+Version: 1.3.3
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.2/hcam_finder.egg-info/SOURCES.txt` & `hcam_finder-1.3.3/hcam_finder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.2/scripts/hfinder` & `hcam_finder-1.3.3/scripts/hfinder`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Please see the file LICENSE.txt for details.
 #
 from __future__ import print_function, absolute_import, unicode_literals, division
 
 import logging
 from functools import partial
 import six
-from distutils.version import LooseVersion
+from packaging.version import parse
 
 import ginga
 from ginga import AstroImage
 from ginga import imap
 
 try:
     from ginga.tkw.ImageViewTk import ImageViewCanvas as CanvasView
@@ -34,15 +34,15 @@
 if not six.PY3:
     import Tkinter as tk
     import tkFileDialog as filedialog
 else:
     import tkinter as tk
     from tkinter import filedialog
 
-OLD_GINGA = LooseVersion(ginga.__version__) <= LooseVersion("2.7.1")
+OLD_GINGA = parse(ginga.__version__) <= parse("2.7.1")
 STD_FORMAT = "%(asctime)s | %(levelname)1.1s | %(filename)s:%(lineno)d (%(funcName)s) | %(message)s"
 
 
 def format_tips(font, desired_width):
     """
     Create a formatted tips string, that fits inside the desired_width
     """
@@ -302,15 +302,14 @@
     def open_file(self):
         filename = filedialog.askopenfilename(
             filetypes=[("allfiles", "*"), ("fitsfiles", "*.fits")]
         )
         self.load_file(filename)
 
     def motion(self, fitsimage, button, data_x, data_y):
-
         # Get the value under the data coordinates
         try:
             # We report the value across the pixel, even though the coords
             # change halfway across the pixel
             value = fitsimage.get_data(int(data_x + 0.5), int(data_y + 0.5))
         except Exception:
             value = None
@@ -343,15 +342,14 @@
     def quit(self):
         write_config(self.globals)
         self.destroy()
         return True
 
 
 def main():
-
     logger = logging.getLogger("example1")
     logger.setLevel(logging.INFO)
     fmt = logging.Formatter(STD_FORMAT)
     stderrHdlr = logging.StreamHandler()
     stderrHdlr.setFormatter(fmt)
     logger.addHandler(stderrHdlr)
```

### Comparing `hcam_finder-1.3.2/scripts/ufinder` & `hcam_finder-1.3.3/scripts/ufinder`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This is open-source software licensed under a BSD license.
 # Please see the file LICENSE.txt for details.
 #
 from __future__ import print_function, absolute_import, unicode_literals, division
 from functools import partial
 import logging
 import six
-from distutils.version import LooseVersion
+from packaging.version import parse
 
 import ginga
 from ginga import AstroImage
 from ginga import imap
 
 try:
     from ginga.tkw.ImageViewTk import ImageViewCanvas as CanvasView
@@ -32,15 +32,15 @@
 if not six.PY3:
     import Tkinter as tk
     import tkFileDialog as filedialog
 else:
     import tkinter as tk
     from tkinter import filedialog
 
-OLD_GINGA = LooseVersion(ginga.__version__) <= LooseVersion("2.7.1")
+OLD_GINGA = parse(ginga.__version__) <= parse("2.7.1")
 STD_FORMAT = "%(asctime)s | %(levelname)1.1s | %(filename)s:%(lineno)d (%(funcName)s) | %(message)s"
 
 
 def format_tips(font, desired_width):
     """
     Create a formatted tips string, that fits inside the desired_width
     """
@@ -265,15 +265,14 @@
     def open_file(self):
         filename = filedialog.askopenfilename(
             filetypes=[("allfiles", "*"), ("fitsfiles", "*.fits")]
         )
         self.load_file(filename)
 
     def motion(self, fitsimage, button, data_x, data_y):
-
         # Get the value under the data coordinates
         try:
             # We report the value across the pixel, even though the coords
             # change halfway across the pixel
             value = fitsimage.get_data(int(data_x + 0.5), int(data_y + 0.5))
         except Exception:
             value = None
@@ -306,15 +305,14 @@
     def quit(self):
         write_config(self.globals)
         self.destroy()
         return True
 
 
 def main():
-
     logger = logging.getLogger("example1")
     logger.setLevel(logging.INFO)
     fmt = logging.Formatter(STD_FORMAT)
     stderrHdlr = logging.StreamHandler()
     stderrHdlr.setFormatter(fmt)
     logger.addHandler(stderrHdlr)
```

### Comparing `hcam_finder-1.3.2/scripts/usfinder` & `hcam_finder-1.3.3/scripts/usfinder`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This is open-source software licensed under a BSD license.
 # Please see the file LICENSE.txt for details.
 #
 from __future__ import print_function, absolute_import, unicode_literals, division
 from functools import partial
 import logging
 import six
-from distutils.version import LooseVersion
+from packaging.version import parse
 
 import ginga
 from ginga import AstroImage
 from ginga import imap
 
 try:
     from ginga.tkw.ImageViewTk import ImageViewCanvas as CanvasView
@@ -32,15 +32,15 @@
 if not six.PY3:
     import Tkinter as tk
     import tkFileDialog as filedialog
 else:
     import tkinter as tk
     from tkinter import filedialog
 
-OLD_GINGA = LooseVersion(ginga.__version__) <= LooseVersion("2.7.1")
+OLD_GINGA = parse(ginga.__version__) <= parse("2.7.1")
 STD_FORMAT = "%(asctime)s | %(levelname)1.1s | %(filename)s:%(lineno)d (%(funcName)s) | %(message)s"
 
 
 def format_tips(font, desired_width):
     """
     Create a formatted tips string, that fits inside the desired_width
     """
@@ -276,15 +276,14 @@
     def open_file(self):
         filename = filedialog.askopenfilename(
             filetypes=[("allfiles", "*"), ("fitsfiles", "*.fits")]
         )
         self.load_file(filename)
 
     def motion(self, fitsimage, button, data_x, data_y):
-
         # Get the value under the data coordinates
         try:
             # We report the value across the pixel, even though the coords
             # change halfway across the pixel
             value = fitsimage.get_data(int(data_x + 0.5), int(data_y + 0.5))
         except Exception:
             value = None
@@ -317,15 +316,14 @@
     def quit(self):
         write_config(self.globals)
         self.destroy()
         return True
 
 
 def main():
-
     logger = logging.getLogger("example1")
     logger.setLevel(logging.INFO)
     fmt = logging.Formatter(STD_FORMAT)
     stderrHdlr = logging.StreamHandler()
     stderrHdlr.setFormatter(fmt)
     logger.addHandler(stderrHdlr)
```

### Comparing `hcam_finder-1.3.2/setup.py` & `hcam_finder-1.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["ginga", "astropy", "six", "pillow", "configobj", "hcam_widgets>=1.1.0"]
+requirements = ["ginga", "astropy", "six", "pillow", "configobj", "hcam_widgets>=1.1.1"]
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 # Treat everything in scripts except README.rst as a script to be installed
 scripts = [
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_finder",
-    version="1.3.2",
+    version="1.3.3",
     description="Observation planning and finding charts for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_finder",
-    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.2.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz",
     packages=[
         "hcam_finder",
     ],
     package_dir={"hcam_finder": "hcam_finder"},
     include_package_data=True,
     scripts=scripts,
     install_requires=requirements,
```

### Comparing `hcam_finder-1.3.2/tests/test_hcam_finder.py` & `hcam_finder-1.3.3/tests/test_hcam_finder.py`

 * *Files identical despite different names*

