# Comparing `tmp/geeViz-2023.7.4.tar.gz` & `tmp/geeViz-2023.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.7.4.tar", last modified: Mon Jul 24 21:31:26 2023, max compression
+gzip compressed data, was "geeViz-2023.7.5.tar", last modified: Fri Jul 28 17:23:01 2023, max compression
```

## Comparing `geeViz-2023.7.4.tar` & `geeViz-2023.7.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.911134 geeViz-2023.7.4/
--rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.7.4/LICENSE
--rw-rw-rw-   0        0        0     3851 2023-07-24 21:31:26.910134 geeViz-2023.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.784470 geeViz-2023.7.4/geeViz/
--rw-rw-rw-   0        0        0      127 2023-07-24 21:29:30.000000 geeViz-2023.7.4/geeViz/__init__.py
--rw-rw-rw-   0        0        0    23538 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.861264 geeViz-2023.7.4/geeViz/examples/
--rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      127 2023-07-24 21:29:23.000000 geeViz-2023.7.4/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/foliumViewerExample.py
--rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/gee2PandasExample.ipynb
--rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14302 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11478 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12263 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/foliumView.py
--rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/gcpLib.py
--rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/gee2Pandas.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.864255 geeViz-2023.7.4/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.866250 geeViz-2023.7.4/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.7.4/geeViz/geeView/css/style.min.css
--rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/foliumView.html
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.896171 geeViz-2023.7.4/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.7.4/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.904148 geeViz-2023.7.4/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.7.4/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0    22679 2023-07-19 18:17:03.000000 geeViz-2023.7.4/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    16069 2023-07-19 18:14:04.000000 geeViz-2023.7.4/geeViz/geeView.py
--rw-rw-rw-   0        0        0   175797 2023-07-24 21:29:01.000000 geeViz-2023.7.4/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.7.4/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 21:31:26.807407 geeViz-2023.7.4/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3851 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 21:31:26.000000 geeViz-2023.7.4/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 21:31:26.911134 geeViz-2023.7.4/setup.cfg
--rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.224322 geeViz-2023.7.5/
+-rw-rw-rw-   0        0        0      574 2023-07-24 21:19:20.000000 geeViz-2023.7.5/LICENSE
+-rw-rw-rw-   0        0        0     3851 2023-07-28 17:23:01.221329 geeViz-2023.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-07-18 20:28:01.000000 geeViz-2023.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:00.907172 geeViz-2023.7.5/geeViz/
+-rw-rw-rw-   0        0        0      127 2023-07-28 17:18:20.000000 geeViz-2023.7.5/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    23538 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    96153 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.120598 geeViz-2023.7.5/geeViz/examples/
+-rw-rw-rw-   0        0        0     5467 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11883 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     8037 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4424 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6284 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9586 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15557 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12631 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19522 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      127 2023-07-28 17:18:12.000000 geeViz-2023.7.5/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   225731 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5771 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16613 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    43661 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5779 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14302 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11478 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    18431 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12263 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     9196 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8218 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18777 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1063 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6317 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     8783 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    10077 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.155503 geeViz-2023.7.5/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.158528 geeViz-2023.7.5/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    30585 2023-07-19 17:12:21.000000 geeViz-2023.7.5/geeViz/geeView/css/style.min.css
+-rw-rw-rw-   0        0        0    10024 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/foliumView.html
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.202384 geeViz-2023.7.5/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0     8352 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   232219 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   231399 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      652 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3455 2023-07-19 17:06:25.000000 geeViz-2023.7.5/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:01.218336 geeViz-2023.7.5/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   528516 2023-07-19 17:12:21.000000 geeViz-2023.7.5/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0     1465 2023-07-28 17:17:53.000000 geeViz-2023.7.5/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    16877 2023-07-28 17:13:30.000000 geeViz-2023.7.5/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   175797 2023-07-24 21:29:01.000000 geeViz-2023.7.5/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2023-07-18 20:07:28.000000 geeViz-2023.7.5/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:23:00.954043 geeViz-2023.7.5/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3851 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 17:23:00.000000 geeViz-2023.7.5/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:23:01.224322 geeViz-2023.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-18 20:28:01.000000 geeViz-2023.7.5/setup.py
```

### Comparing `geeViz-2023.7.4/LICENSE` & `geeViz-2023.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/PKG-INFO` & `geeViz-2023.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.4/README.md` & `geeViz-2023.7.5/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/assetManagerLib.py` & `geeViz-2023.7.5/geeViz/assetManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/changeDetectionLib.py` & `geeViz-2023.7.5/geeViz/changeDetectionLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/CCDCViz.py` & `geeViz-2023.7.5/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.7.5/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.7.5/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.7.5/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/foliumViewerExample.py` & `geeViz-2023.7.5/geeViz/examples/foliumViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/gee2PandasExample.ipynb` & `geeViz-2023.7.5/geeViz/examples/gee2PandasExample.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/geeViewExample.py` & `geeViz-2023.7.5/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.7.5/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.7.5/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.7.5/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.7.5/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.7.5/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.7.5/geeViz/examples/lcmsViewerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.7.5/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.7.5/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.7.5/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/examples/timeLapseExample.py` & `geeViz-2023.7.5/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/foliumView.py` & `geeViz-2023.7.5/geeViz/foliumView.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/gcpLib.py` & `geeViz-2023.7.5/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/gee2Pandas.py` & `geeViz-2023.7.5/geeViz/gee2Pandas.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/css/style.min.css` & `geeViz-2023.7.5/geeViz/geeView/css/style.min.css`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/foliumView.html` & `geeViz-2023.7.5/geeViz/geeView/foliumView.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.7.5/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/GEE.png` & `geeViz-2023.7.5/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.7.5/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.7.5/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.7.5/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.7.5/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.7.5/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.7.5/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.7.5/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.7.5/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/index.html` & `geeViz-2023.7.5/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.7.5/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.7.5/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView/js/load.min.js` & `geeViz-2023.7.5/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/geeView.py` & `geeViz-2023.7.5/geeViz/geeView.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 from IPython.display import IFrame,display, HTML
 if sys.version_info[0] < 3:
     import SimpleHTTPServer, SocketServer
 else:
     import http.server, socketserver 
 creds_path = ee.oauth.get_credentials_path()
 IS_COLAB = "google.colab" in sys.modules
+IS_WORKBENCH = os.getenv("DL_ANACONDA_HOME") != None
 if IS_COLAB:
   from google.colab.output import eval_js
+
 ######################################################################
 # Functions to handle various initialization/authentication workflows to try to get a user an initialized instance of ee
 
 # Function to have user input a project id if one is still needed
 def getProject():
     provided_project = '{}.proj_id'.format(creds_path)
     provided_project = os.path.normpath(provided_project)
@@ -124,15 +126,17 @@
     except NameError:
         return False      # Probably standard Python interpreter
 ######################################################################
 # Function for cleaning trailing .... in accessToken
 def cleanAccessToken(accessToken):
     while accessToken[-1] == '.': accessToken = accessToken[:-1]
     return accessToken
-
+# Function to get domain base without any folders
+def baseDomain(domain):
+    return domain.split('.com')[0]+'.com'
 # Function for using default GEE refresh token to get an access token for geeView
 def refreshToken(refresh_token_path = ee.oauth.get_credentials_path()):
     try:
         refresh_token=json.load(open(refresh_token_path))['refresh_token']
     except Exception as e:
         print('Could not find refresh token at:',refresh_token_path)
         refresh_token = ''
@@ -199,14 +203,16 @@
         self.idDictList = []
         self.mapCommandList  = []
         self.ee_run_name = 'runGeeViz'
 
         self.isNotebook = is_notebook()
         self.isColab = "google.colab" in sys.modules
 
+        self.proxy_url = None
+
         self.refreshTokenPath = ee.oauth.get_credentials_path()
         self.serviceKeyPath = None
         self.queryWindowMode = 'sidePane'
         
     #Function for adding a layer to the map
     def addLayer(self,image,viz = {},name= None,visible= True):
         if name == None:
@@ -317,14 +323,22 @@
         if IS_COLAB:
             proxy_js = "google.colab.kernel.proxyPort({})".format(self.port)
             proxy_url = eval_js(proxy_js)
             geeView_proxy_url = '{}geeView/?accessToken={}'.format(proxy_url,self.accessToken)
             print('Colab Proxy URL:',geeView_proxy_url)
             viewerFrame = IFrame(src=geeView_proxy_url, width='100%', height='{}px'.format(iframe_height))
             display(viewerFrame)
+        if IS_WORKBENCH:
+            if self.proxy_url == None:
+                self.proxy_url = input('Please enter current URL Workbench Notebook is running from (e.g. https://code-dot-region.notebooks.googleusercontent.com/): ')
+            self.proxy_url = baseDomain(self.proxy_url)
+            geeView_proxy_url = '{}/proxy/{}/geeView/?accessToken={}'.format(self.proxy_url,self.port,self.accessToken)
+            print('Workbench Proxy URL:',geeView_proxy_url)
+            viewerFrame = IFrame(src=geeView_proxy_url, width='100%', height='{}px'.format(iframe_height))
+            display(viewerFrame)
         elif not self.isNotebook or open_browser:
             webbrowser.open('http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken),new = 1)
         elif open_browser == False and open_iframe:
             self.IFrame = IFrame(src='http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken), width='100%', height='{}px'.format(iframe_height))
         else:
             self.IFrame = IFrame(src='http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken), width='100%', height='{}px'.format(iframe_height))
             display(self.IFrame)
```

### Comparing `geeViz-2023.7.4/geeViz/getImagesLib.py` & `geeViz-2023.7.5/geeViz/getImagesLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/migrateGEEAssets.py` & `geeViz-2023.7.5/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/phEEnoViz.py` & `geeViz-2023.7.5/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz/taskManagerLib.py` & `geeViz-2023.7.5/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/geeViz.egg-info/PKG-INFO` & `geeViz-2023.7.5/geeViz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geeViz-2023.7.4/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.7.5/geeViz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geeViz-2023.7.4/setup.py` & `geeViz-2023.7.5/setup.py`

 * *Files identical despite different names*

