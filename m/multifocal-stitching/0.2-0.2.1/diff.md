# Comparing `tmp/multifocal-stitching-0.2.tar.gz` & `tmp/multifocal-stitching-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multifocal-stitching-0.2.tar", last modified: Fri Jul 28 02:54:48 2023, max compression
+gzip compressed data, was "multifocal-stitching-0.2.1.tar", last modified: Fri Jul 28 19:57:33 2023, max compression
```

## Comparing `multifocal-stitching-0.2.tar` & `multifocal-stitching-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.2/LICENSE
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5505 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3485 2023-07-28 02:47:25.000000 multifocal-stitching-0.2/README.md
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1564 2023-07-27 23:56:41.000000 multifocal-stitching-0.2/pyproject.toml
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/setup.cfg
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/multifocal_stitching/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      125 2023-07-28 00:32:08.000000 multifocal-stitching-0.2/src/multifocal_stitching/__init__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2098 2023-07-28 01:56:05.000000 multifocal-stitching-0.2/src/multifocal_stitching/__main__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1391 2023-07-28 02:36:42.000000 multifocal-stitching-0.2/src/multifocal_stitching/merge_imgs.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     4976 2023-07-28 00:32:48.000000 multifocal-stitching-0.2/src/multifocal_stitching/stitching.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3640 2023-07-28 02:50:35.000000 multifocal-stitching-0.2/src/multifocal_stitching/utils.py
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5505 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      480 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/SOURCES.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/dependency_links.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       91 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/requires.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-28 02:54:48.000000 multifocal-stitching-0.2/src/multifocal_stitching.egg-info/top_level.txt
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 02:54:48.440049 multifocal-stitching-0.2/tests/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3843 2023-07-28 02:35:08.000000 multifocal-stitching-0.2/tests/test_stitching.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2023-07-27 03:00:46.000000 multifocal-stitching-0.2.1/LICENSE
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     6170 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     4125 2023-07-28 03:14:36.000000 multifocal-stitching-0.2.1/README.md
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1600 2023-07-28 19:56:40.000000 multifocal-stitching-0.2.1/pyproject.toml
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/setup.cfg
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/src/
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/src/multifocal_stitching/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      165 2023-07-28 16:05:55.000000 multifocal-stitching-0.2.1/src/multifocal_stitching/__init__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     2092 2023-07-28 18:46:08.000000 multifocal-stitching-0.2.1/src/multifocal_stitching/__main__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1370 2023-07-28 16:17:04.000000 multifocal-stitching-0.2.1/src/multifocal_stitching/merge_imgs.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     4989 2023-07-28 19:28:10.000000 multifocal-stitching-0.2.1/src/multifocal_stitching/stitching.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3640 2023-07-28 02:50:35.000000 multifocal-stitching-0.2.1/src/multifocal_stitching/utils.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     6170 2023-07-28 19:57:33.000000 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      480 2023-07-28 19:57:33.000000 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-07-28 19:57:33.000000 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      119 2023-07-28 19:57:33.000000 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/requires.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       21 2023-07-28 19:57:33.000000 multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/top_level.txt
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-07-28 19:57:33.762454 multifocal-stitching-0.2.1/tests/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3843 2023-07-28 18:13:04.000000 multifocal-stitching-0.2.1/tests/test_stitching.py
```

### Comparing `multifocal-stitching-0.2/LICENSE` & `multifocal-stitching-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.2/PKG-INFO` & `multifocal-stitching-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multifocal-stitching
-Version: 0.2
+Version: 0.2.1
 Summary: Algorithms and tools for stitching microscopy images taken at different focal lengths
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -20,36 +20,60 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: webapp
 License-File: LICENSE
 
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+This package aims to:
+- Accurately compute translation parameters between two images taken with a
+  translation and focus change
+- Be tolerant of high levels of noise and blurriness caused by the focus change
+
+This package does not:
+- Account for other non-translational camera models
+- Calculate subpixel-level stitching coordinates
+- Perform focus stacking or blending of images in any manner
+
+### Examples
+
+Matching using low-frequency features:
+
 <img src="assets/image1.png" width="90%"/>
 
+Matching using high-frequency features:
+
 <img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
-Ensure the images to be stitched are sequentially named in `dir`.
+Ensure the images to be stitched are sequentially named in `<dir>`, then run:
+
+```
+python -m multifocal_stitching <dir>
+```
+
+Most images can be stitched successfully with the default settings. To fine-tune
+settings with the CLI:
 
 ```
 python -m multifocal_stitching -h
 usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
                    [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
                    [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
                    [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
@@ -91,13 +115,11 @@
   --result_dir RESULT_DIR
                         Directory to save merged files (default: merged)
   --resize_factor RESIZE_FACTOR
                         Whether to resize the images saved by a factor (default: 1)
   --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
-### Examples
-
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
 [build-url]: https://github.com/yuanchenyang/multifocal-stitching/actions?query=workflow%3ACI
```

### Comparing `multifocal-stitching-0.2/README.md` & `multifocal-stitching-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+This package aims to:
+- Accurately compute translation parameters between two images taken with a
+  translation and focus change
+- Be tolerant of high levels of noise and blurriness caused by the focus change
+
+This package does not:
+- Account for other non-translational camera models
+- Calculate subpixel-level stitching coordinates
+- Perform focus stacking or blending of images in any manner
+
+### Examples
+
+Matching using low-frequency features:
+
 <img src="assets/image1.png" width="90%"/>
 
+Matching using high-frequency features:
+
 <img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
-Ensure the images to be stitched are sequentially named in `dir`.
+Ensure the images to be stitched are sequentially named in `<dir>`, then run:
+
+```
+python -m multifocal_stitching <dir>
+```
+
+Most images can be stitched successfully with the default settings. To fine-tune
+settings with the CLI:
 
 ```
 python -m multifocal_stitching -h
 usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
                    [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
                    [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
                    [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
@@ -63,13 +86,11 @@
   --result_dir RESULT_DIR
                         Directory to save merged files (default: merged)
   --resize_factor RESIZE_FACTOR
                         Whether to resize the images saved by a factor (default: 1)
   --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
-### Examples
-
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
 [build-url]: https://github.com/yuanchenyang/multifocal-stitching/actions?query=workflow%3ACI
```

### Comparing `multifocal-stitching-0.2/pyproject.toml` & `multifocal-stitching-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multifocal-stitching"
-version = "0.2"
+version = "0.2.1"
 description = "Algorithms and tools for stitching microscopy images taken at different focal lengths"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "Chenyang Yuan", email = "yuanchenyang@gmail.com" }
 ]
@@ -43,14 +43,15 @@
 "Bug Tracker" = "https://github.com/yuanchenyang/multifocal-stitching/issues"
 "Documentation" = "https://github.com/yuanchenyang/multifocal-stitching"
 "Source" = "https://github.com/yuanchenyang/multifocal-stitching"
 
 [project.optional-dependencies] # Optional
 dev = ["build", "twine"]
 test = ["pytest", "pytest-cov"]
+webapp = ["gradio", "matplotlib"]
 
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = [
```

### Comparing `multifocal-stitching-0.2/src/multifocal_stitching/__main__.py` & `multifocal-stitching-0.2.1/src/multifocal_stitching/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
                             workers = args.workers,
                             peak_cutoff_std = args.peak_cutoff_std,
                             peaks_dist_threshold = args.peaks_dist_threshold,
                             filter_radii = args.filter_radii,
                             min_overlap = args.min_overlap,
                             early_term_thresh = args.early_term_thresh,
                             verbose = args.verbose)
-            dx, dy = result.coord
+            dx, dy = result.delta
             img_name1, img_name2 = map(get_name, img_names)
             writer.writerow([img_name1, img_name2, dx, dy, result.corr_coeff,
-                             result.area, result.best_r, result.best_win])
+                             result.area, result.r, result.use_win])
             if not args.no_merge:
                 if args.verbose:
                     print('Merging:', img_name1, img_name2)
                 res_dir = get_full_path(args.dir, args.result_dir, mkdir=True)
                 merge_and_save(args.dir, res_dir, img_name1, img_name2, dx, dy,
                                resize_factor=args.resize_factor,
                                save_gif=args.save_gif,)
```

### Comparing `multifocal-stitching-0.2/src/multifocal_stitching/merge_imgs.py` & `multifocal-stitching-0.2.1/src/multifocal_stitching/merge_imgs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from PIL import Image
 from typing import Tuple
 from .utils import *
 
-def merge(i1: Image, i2: Image, dx:int, dy:int) -> Tuple[Image, Image]:
+def merge(i1: Image, i2: Image, dx:int, dy:int, resize_factor:int = 1
+          ) -> Tuple[Image.Image, Image.Image]:
     assert i1.size == i2.size, "Images must be same size!"
     W, H = i1.size
     new_W, new_H = W + abs(dx), H + abs(dy)
 
     i1_x = -dx if dx < 0 else 0
     i1_y = -dy if dy < 0 else 0
     i2_x = dx if dx > 0 else 0
@@ -16,22 +17,20 @@
     res = Image.new(mode='RGB', size=(new_W, new_H))
     res.paste(i1, (i1_x, i1_y))
     res.paste(i2, (i2_x, i2_y))
 
     res_r = res.copy()
     res_r.paste(i1, (i1_x, i1_y))
 
-    return res, res_r
+    return [r.resize((new_W // resize_factor, new_H // resize_factor), Image.LANCZOS)
+            for r in (res, res_r)]
 
 def merge_and_save(base_dir:str, res_dir:str, img_name1:str, img_name2:str,
-                   dx:int, dy:int, resize_factor:int=1, save_gif:bool=False):
+                   dx:int, dy:int, save_gif:bool=False, **kwargs):
     i1, i2 = [Image.open(get_full_path(base_dir, i)) for i in (img_name1, img_name2)]
-    res = merge(i1, i2, dx, dy)
-    W, H = res[0].size
-    res_resized = [r.resize((W // resize_factor, H // resize_factor), Image.LANCZOS)
-                   for r in res]
-    for i, r in enumerate(res_resized):
+    res = merge(i1, i2, dx, dy, **kwargs)
+    for i, r in enumerate(res):
         base1, base2 = [os.path.splitext(n)[0] for n in (img_name1, img_name2)]
         r.save(get_full_path(res_dir, f'{base1}__{base2}_{i}.jpg'))
     if save_gif:
-        res_resized[0].save(get_full_path(res_dir, f'{base1}__{base2}.png'), save_all=True,
-                            append_images=res_resized[1:], duration=500, loop=0)
+        res[0].save(get_full_path(res_dir, f'{base1}__{base2}.png'), save_all=True,
+                            append_images=res[1:], duration=500, loop=0)
```

### Comparing `multifocal-stitching-0.2/src/multifocal_stitching/stitching.py` & `multifocal-stitching-0.2.1/src/multifocal_stitching/stitching.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,26 +58,26 @@
         X = np.argwhere(cutoff)
         labels = AgglomerativeClustering(
             n_clusters=None,
             linkage='single',
             distance_threshold=peaks_dist_threshold
         ).fit(X).labels_
         cents = list(centroids(X, labels))
-        yield from sorted(cents, key=lambda coord: res[tuple(coord)])
+        yield from sorted(cents, key=lambda delta: res[tuple(delta)])
     else:
         yield from np.argwhere(cutoff)
 
 StitchingResult = namedtuple(
     'StitchingResult',
-    ['corr_coeff', 'corr', 'coord', 'val', 'area', 'best_r', 'best_win']
+    ['corr_coeff', 'corr', 'freq_delta', 'delta', 'val', 'area', 'r', 'use_win']
 )
 
 def print_stitching_result(r: StitchingResult):
-    dx, dy = r.coord
-    print(f'dx:{dx: 5} dy:{dy: 5} corr:{r.corr_coeff:+f} area:{r.area: 9} r:{r.best_r: 3}')
+    dx, dy = r.delta
+    print(f'dx:{dx: 5} dy:{dy: 5} corr:{r.corr_coeff:+f} area:{r.area: 9} r:{r.r: 3}')
 
 def candidate_stitches(img1: np.ndarray, img2: np.ndarray,
                        use_wins: Tuple[int] = (0,),
                        workers: int = 2,
                        peak_cutoff_std: float = 1,
                        peaks_dist_threshold: float = 25,
                        filter_radii: Tuple[int] = (100,50,20),
@@ -111,15 +111,15 @@
             # 4. Obtain cross correlation in spatial domain by taking inverse FFT
             res = fft.ifft2(R, img1.shape, norm='ortho', workers=workers)
 
             # 5. Group peaks and find centroids of groups
             for dy, dx in get_peak_centroids(res, peak_cutoff_std, peaks_dist_threshold):
                 for dX, dY in product((dx, -X+dx), (dy, -Y+dy)):
                     coef, area = get_overlap(img1, img2, (dX, dY), min_overlap=min_overlap)
-                    result = StitchingResult(coef, res, (dX, dY), res[dY, dX], area, r, use_win)
+                    result = StitchingResult(coef, res, (dx, dy), (dX, dY), res[dY, dX], area, r, use_win)
                     if verbose:
                         print_stitching_result(result)
                     yield result
                     if coef >= early_term_thresh:
                         return
 
 def stitch(img1: np.ndarray, img2: np.ndarray, **kwargs) -> StitchingResult:
```

### Comparing `multifocal-stitching-0.2/src/multifocal_stitching/utils.py` & `multifocal-stitching-0.2.1/src/multifocal_stitching/utils.py`

 * *Files identical despite different names*

### Comparing `multifocal-stitching-0.2/src/multifocal_stitching.egg-info/PKG-INFO` & `multifocal-stitching-0.2.1/src/multifocal_stitching.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multifocal-stitching
-Version: 0.2
+Version: 0.2.1
 Summary: Algorithms and tools for stitching microscopy images taken at different focal lengths
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
 License: Copyright 2023 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -20,36 +20,60 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: webapp
 License-File: LICENSE
 
 Multifocal Image Stitching
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
+This package aims to:
+- Accurately compute translation parameters between two images taken with a
+  translation and focus change
+- Be tolerant of high levels of noise and blurriness caused by the focus change
+
+This package does not:
+- Account for other non-translational camera models
+- Calculate subpixel-level stitching coordinates
+- Perform focus stacking or blending of images in any manner
+
+### Examples
+
+Matching using low-frequency features:
+
 <img src="assets/image1.png" width="90%"/>
 
+Matching using high-frequency features:
+
 <img src="assets/image2.png" width="90%"/>
 
 ### Installation
 
 To install from [pypi](https://pypi.org/project/multifocal-stitching/):
 
 ```
 pip install multifocal-stitching
 ```
 
 ### Usage
-Ensure the images to be stitched are sequentially named in `dir`.
+Ensure the images to be stitched are sequentially named in `<dir>`, then run:
+
+```
+python -m multifocal_stitching <dir>
+```
+
+Most images can be stitched successfully with the default settings. To fine-tune
+settings with the CLI:
 
 ```
 python -m multifocal_stitching -h
 usage: __main__.py [-h] [-v] [--ext EXT] [--imgs IMGS [IMGS ...]] [--no_merge] [--workers WORKERS]
                    [--min_overlap MIN_OVERLAP] [--early_term_thresh EARLY_TERM_THRESH]
                    [--use_wins USE_WINS [USE_WINS ...]] [--peak_cutoff_std PEAK_CUTOFF_STD]
                    [--peaks_dist_threshold PEAKS_DIST_THRESHOLD]
@@ -91,13 +115,11 @@
   --result_dir RESULT_DIR
                         Directory to save merged files (default: merged)
   --resize_factor RESIZE_FACTOR
                         Whether to resize the images saved by a factor (default: 1)
   --save_gif            Whether to save a gif alternating between the merged files (default: False)
 ```
 
-### Examples
-
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://github.com/yuanchenyang/multifocal-stitching
 [build-img]: https://github.com/yuanchenyang/multifocal-stitching/workflows/CI/badge.svg?branch=master
 [build-url]: https://github.com/yuanchenyang/multifocal-stitching/actions?query=workflow%3ACI
```

### Comparing `multifocal-stitching-0.2/tests/test_stitching.py` & `multifocal-stitching-0.2.1/tests/test_stitching.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from multifocal_stitching.stitching import stitch
 from multifocal_stitching.utils import read_img, get_full_path
 from multifocal_stitching.merge_imgs import merge_and_save
 from multifocal_stitching.__main__ import main as cli
 from multifocal_stitching.__main__ import CSV_HEADER
 
 def coord_is_close(res, val, tol=5):
-    assert np.linalg.norm(np.array(res.coord) - np.array(val), 1) <= tol
+    assert np.linalg.norm(np.array(res.delta) - np.array(val), 1) <= tol
 
 class TestCLI(unittest.TestCase):
     def setUp(self):
         self.base_dir = 'tests/img_folder'
         shutil.rmtree(self.base_dir, ignore_errors=True)
         os.makedirs(self.base_dir)
         shutil.copy('tests/imgs/high_freq_features_1_small.jpg', self.base_dir)
@@ -54,15 +54,15 @@
     def setUp(self):
         self.base_dir = 'tests/imgs'
 
     def stitch_name(self, name):
         names = [f'{name}_{ext}_small.jpg' for ext in '12']
         res = stitch(*[read_img(get_full_path(self.base_dir, name)) for name in names])
         res_dir = get_full_path(self.base_dir, 'merged', mkdir=True)
-        dx, dy = res.coord
+        dx, dy = res.delta
         merge_and_save(self.base_dir, res_dir, names[0], names[1], dx, dy,
                        resize_factor=8, save_gif=True)
         return res
 
     def test_stitching_high_freq_features(self):
         res = self.stitch_name('high_freq_features')
         coord_is_close(res, (2474,495))
```

