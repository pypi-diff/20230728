# Comparing `tmp/multifocal-stitching-0.1.1.tar.gz` & `tmp/multifocal-stitching-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multifocal-stitching-0.1.1.tar", last modified: Thu Jul 27 05:30:19 2023, max compression
+gzip compressed data, was "multifocal-stitching-0.2.tar", last modified: Fri Jul 28 02:54:48 2023, max compression
```

## Comparing `multifocal-stitching-0.1.1.tar` & `multifocal-stitching-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.1.1/LICENSE
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5037 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3015 2023-07-27 05:28:03.000000 multifocal-stitching-0.1.1/README.md
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1566 2023-07-27 05:29:05.000000 multifocal-stitching-0.1.1/pyproject.toml
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/setup.cfg
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/multifocal_stitching/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       41 2023-07-27 04:00:42.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/__init__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1166 2023-07-27 05:25:55.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/__main__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1816 2023-07-27 04:19:13.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/merge_imgs.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5107 2023-07-27 05:23:29.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/stitching.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1185 2023-07-27 04:26:53.000000 multifocal-stitching-0.1.1/src/multifocal_stitching/utils.py
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5037 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      480 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/SOURCES.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/dependency_links.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       91 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/requires.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-27 05:30:19.000000 multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/top_level.txt
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-27 05:30:19.488345 multifocal-stitching-0.1.1/tests/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1906 2023-07-27 05:07:49.000000 multifocal-stitching-0.1.1/tests/test_stitching.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.2/LICENSE
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5505 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3485 2023-07-28 02:47:25.000000 multifocal-stitching-0.2/README.md
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1564 2023-07-27 23:56:41.000000 multifocal-stitching-0.2/pyproject.toml
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/setup.cfg
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/multifocal_stitching/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      125 2023-07-28 00:32:08.000000 multifocal-stitching-0.2/src/multifocal_stitching/__init__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2098 2023-07-28 01:56:05.000000 multifocal-stitching-0.2/src/multifocal_stitching/__main__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1391 2023-07-28 02:36:42.000000 multifocal-stitching-0.2/src/multifocal_stitching/merge_imgs.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     4976 2023-07-28 00:32:48.000000 multifocal-stitching-0.2/src/multifocal_stitching/stitching.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3640 2023-07-28 02:50:35.000000 multifocal-stitching-0.2/src/multifocal_stitching/utils.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5505 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      480 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       91 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/requires.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/top_level.txt
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/tests/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3843 2023-07-28 02:35:08.000000 multifocal-stitching-0.2/tests/test_stitching.py
```

### Comparing `multifocal-stitching-0.1.1/LICENSE` & `multifocal-stitching-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.1.1/PKG-INFO` & `multifocal-stitching-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multifocal-stitching
-Version: 0.1.1
+Version: 0.2
 Summary: Algorithms and tools for stitching microscopy images taken at different focal lengths
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -28,49 +28,50 @@
 
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+<img src="assets/image1.png" width="90%"/>
 
+<img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
 Ensure the images to be stitched are sequentially named in `dir`.
 
 ```
 python -m multifocal_stitching -h
-usage: __main__.py [-h] [-v] [-s STITCHING_RESULT] [-d RESULT_DIR] [-r] [--ext EXT] [--no_merge]
-                   [--workers WORKERS] [--min_overlap MIN_OVERLAP]
-                   [--early_term_thresh EARLY_TERM_THRESH] [--use_wins USE_WINS [USE_WINS ...]]
-                   [--peak_cutoff_std PEAK_CUTOFF_STD] [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
-                   [--filter_radius FILTER_RADIUS [FILTER_RADIUS ...]]
+usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
+                   [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
+                   [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
+                   [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
+                   [--filter_radii FILTER_RADII [FILTER_RADII ...]]
+                   [--stitching_result STITCHING_RESULT] [--result_dir RESULT_DIR]
+                   [--resize_factor RESIZE_FACTOR] [--save_gif]
                    dir
 
 positional arguments:
   dir                   Base directory
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         Increase output verbosity (default: False)
-  -s STITCHING_RESULT, --stitching_result STITCHING_RESULT
-                        Stitching result csv file (default: stitching_result.csv)
-  -d RESULT_DIR, --result_dir RESULT_DIR
-                        Directory to save merged files (default: merged)
-  -r, --exclude_reverse
-                        Whether to additionally include img2 on top of img1 (default: False)
   --ext EXT             Filename extension of images (default: .jpg)
+  --imgs IMGS [IMGS ...]
+                        Stitch only provided images in provided order, otherwise will run in batch
+                        mode over all images in directory (default: None)
   --no_merge            Disable generating merged images (default: False)
   --workers WORKERS     Number of CPU threads to use in FFT (default: 2)
   --min_overlap MIN_OVERLAP
                         Set lower limit for overlapping region as a fraction of total image area
                         (default: 0.125)
   --early_term_thresh EARLY_TERM_THRESH
                         Stop searching when correlation is above this value (default: 0.7)
@@ -78,17 +79,24 @@
                         Whether to try using Hanning window (default: (0,))
   --peak_cutoff_std PEAK_CUTOFF_STD
                         Number of standard deviations below max value to use for peak finding
                         (default: 1)
   --peaks_dist_threshold PEAKS_DIST_THRESHOLD
                         Distance to consider as part of same cluster when finding peak centroid
                         (default: 25)
-  --filter_radius FILTER_RADIUS [FILTER_RADIUS ...]
+  --filter_radii FILTER_RADII [FILTER_RADII ...]
                         Low-pass filter radii to try, smaller matches coarser/out-of-focus features
                         (default: (100, 50, 20))
+  --stitching_result STITCHING_RESULT
+                        Stitching result csv file (default: stitching_result.csv)
+  --result_dir RESULT_DIR
+                        Directory to save merged files (default: merged)
+  --resize_factor RESIZE_FACTOR
+                        Whether to resize the images saved by a factor (default: 1)
+  --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
 ### Examples
 
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
```

### Comparing `multifocal-stitching-0.1.1/README.md` & `multifocal-stitching-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+<img src="assets/image1.png" width="90%"/>
 
+<img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
 Ensure the images to be stitched are sequentially named in `dir`.
 
 ```
 python -m multifocal_stitching -h
-usage: __main__.py [-h] [-v] [-s STITCHING_RESULT] [-d RESULT_DIR] [-r] [--ext EXT] [--no_merge]
-                   [--workers WORKERS] [--min_overlap MIN_OVERLAP]
-                   [--early_term_thresh EARLY_TERM_THRESH] [--use_wins USE_WINS [USE_WINS ...]]
-                   [--peak_cutoff_std PEAK_CUTOFF_STD] [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
-                   [--filter_radius FILTER_RADIUS [FILTER_RADIUS ...]]
+usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
+                   [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
+                   [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
+                   [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
+                   [--filter_radii FILTER_RADII [FILTER_RADII ...]]
+                   [--stitching_result STITCHING_RESULT] [--result_dir RESULT_DIR]
+                   [--resize_factor RESIZE_FACTOR] [--save_gif]
                    dir
 
 positional arguments:
   dir                   Base directory
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         Increase output verbosity (default: False)
-  -s STITCHING_RESULT, --stitching_result STITCHING_RESULT
-                        Stitching result csv file (default: stitching_result.csv)
-  -d RESULT_DIR, --result_dir RESULT_DIR
-                        Directory to save merged files (default: merged)
-  -r, --exclude_reverse
-                        Whether to additionally include img2 on top of img1 (default: False)
   --ext EXT             Filename extension of images (default: .jpg)
+  --imgs IMGS [IMGS ...]
+                        Stitch only provided images in provided order, otherwise will run in batch
+                        mode over all images in directory (default: None)
   --no_merge            Disable generating merged images (default: False)
   --workers WORKERS     Number of CPU threads to use in FFT (default: 2)
   --min_overlap MIN_OVERLAP
                         Set lower limit for overlapping region as a fraction of total image area
                         (default: 0.125)
   --early_term_thresh EARLY_TERM_THRESH
                         Stop searching when correlation is above this value (default: 0.7)
@@ -50,17 +51,24 @@
                         Whether to try using Hanning window (default: (0,))
   --peak_cutoff_std PEAK_CUTOFF_STD
                         Number of standard deviations below max value to use for peak finding
                         (default: 1)
   --peaks_dist_threshold PEAKS_DIST_THRESHOLD
                         Distance to consider as part of same cluster when finding peak centroid
                         (default: 25)
-  --filter_radius FILTER_RADIUS [FILTER_RADIUS ...]
+  --filter_radii FILTER_RADII [FILTER_RADII ...]
                         Low-pass filter radii to try, smaller matches coarser/out-of-focus features
                         (default: (100, 50, 20))
+  --stitching_result STITCHING_RESULT
+                        Stitching result csv file (default: stitching_result.csv)
+  --result_dir RESULT_DIR
+                        Directory to save merged files (default: merged)
+  --resize_factor RESIZE_FACTOR
+                        Whether to resize the images saved by a factor (default: 1)
+  --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
 ### Examples
 
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
```

### Comparing `multifocal-stitching-0.1.1/pyproject.toml` & `multifocal-stitching-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multifocal-stitching"
-version = "0.1.1"
+version = "0.2"
 description = "Algorithms and tools for stitching microscopy images taken at different focal lengths"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "Chenyang Yuan", email = "yuanchenyang@gmail.com" }
 ]
```

### Comparing `multifocal-stitching-0.1.1/src/multifocal_stitching.egg-info/PKG-INFO` & `multifocal-stitching-0.2/src/multifocal_stitching.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multifocal-stitching
-Version: 0.1.1
+Version: 0.2
 Summary: Algorithms and tools for stitching microscopy images taken at different focal lengths
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -28,49 +28,50 @@
 
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+<img src="assets/image1.png" width="90%"/>
 
+<img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
 Ensure the images to be stitched are sequentially named in `dir`.
 
 ```
 python -m multifocal_stitching -h
-usage: __main__.py [-h] [-v] [-s STITCHING_RESULT] [-d RESULT_DIR] [-r] [--ext EXT] [--no_merge]
-                   [--workers WORKERS] [--min_overlap MIN_OVERLAP]
-                   [--early_term_thresh EARLY_TERM_THRESH] [--use_wins USE_WINS [USE_WINS ...]]
-                   [--peak_cutoff_std PEAK_CUTOFF_STD] [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
-                   [--filter_radius FILTER_RADIUS [FILTER_RADIUS ...]]
+usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
+                   [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
+                   [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
+                   [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
+                   [--filter_radii FILTER_RADII [FILTER_RADII ...]]
+                   [--stitching_result STITCHING_RESULT] [--result_dir RESULT_DIR]
+                   [--resize_factor RESIZE_FACTOR] [--save_gif]
                    dir
 
 positional arguments:
   dir                   Base directory
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         Increase output verbosity (default: False)
-  -s STITCHING_RESULT, --stitching_result STITCHING_RESULT
-                        Stitching result csv file (default: stitching_result.csv)
-  -d RESULT_DIR, --result_dir RESULT_DIR
-                        Directory to save merged files (default: merged)
-  -r, --exclude_reverse
-                        Whether to additionally include img2 on top of img1 (default: False)
   --ext EXT             Filename extension of images (default: .jpg)
+  --imgs IMGS [IMGS ...]
+                        Stitch only provided images in provided order, otherwise will run in batch
+                        mode over all images in directory (default: None)
   --no_merge            Disable generating merged images (default: False)
   --workers WORKERS     Number of CPU threads to use in FFT (default: 2)
   --min_overlap MIN_OVERLAP
                         Set lower limit for overlapping region as a fraction of total image area
                         (default: 0.125)
   --early_term_thresh EARLY_TERM_THRESH
                         Stop searching when correlation is above this value (default: 0.7)
@@ -78,17 +79,24 @@
                         Whether to try using Hanning window (default: (0,))
   --peak_cutoff_std PEAK_CUTOFF_STD
                         Number of standard deviations below max value to use for peak finding
                         (default: 1)
   --peaks_dist_threshold PEAKS_DIST_THRESHOLD
                         Distance to consider as part of same cluster when finding peak centroid
                         (default: 25)
-  --filter_radius FILTER_RADIUS [FILTER_RADIUS ...]
+  --filter_radii FILTER_RADII [FILTER_RADII ...]
                         Low-pass filter radii to try, smaller matches coarser/out-of-focus features
                         (default: (100, 50, 20))
+  --stitching_result STITCHING_RESULT
+                        Stitching result csv file (default: stitching_result.csv)
+  --result_dir RESULT_DIR
+                        Directory to save merged files (default: merged)
+  --resize_factor RESIZE_FACTOR
+                        Whether to resize the images saved by a factor (default: 1)
+  --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
 ### Examples
 
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
```

