# Comparing `tmp/pyvideothumbnailer-2.0.2.tar.gz` & `tmp/pyvideothumbnailer-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvideothumbnailer-2.0.2.tar", last modified: Thu Jan 26 18:14:45 2023, max compression
+gzip compressed data, was "pyvideothumbnailer-2.0.3.tar", last modified: Fri Jul 28 18:38:41 2023, max compression
```

## Comparing `pyvideothumbnailer-2.0.2.tar` & `pyvideothumbnailer-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-01-26 18:14:45.402496 pyvideothumbnailer-2.0.2/
--rw-rw-r--   0 default   (1010) default   (1010)     1522 2020-06-11 15:07:37.000000 pyvideothumbnailer-2.0.2/LICENSE
--rw-rw-r--   0 default   (1010) default   (1010)     3742 2023-01-26 18:14:45.398496 pyvideothumbnailer-2.0.2/PKG-INFO
--rw-rw-r--   0 default   (1010) default   (1010)     6422 2023-01-05 20:16:19.000000 pyvideothumbnailer-2.0.2/README
--rw-rw-r--   0 default   (1010) default   (1010)     3155 2023-01-21 20:58:38.000000 pyvideothumbnailer-2.0.2/README.md
--rw-rw-r--   0 default   (1010) default   (1010)      831 2023-01-26 18:14:31.000000 pyvideothumbnailer-2.0.2/pyproject.toml
--rw-rw-r--   0 default   (1010) default   (1010)       38 2023-01-26 18:14:45.402496 pyvideothumbnailer-2.0.2/setup.cfg
-drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-01-26 18:14:45.398496 pyvideothumbnailer-2.0.2/src/
-drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-01-26 18:14:45.398496 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer/
--rw-rw-r--   0 default   (1010) default   (1010)        0 2023-01-08 06:25:39.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer/__init__.py
--rwxrwxr-x   0 default   (1010) default   (1010)    55819 2023-01-26 18:05:43.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer/videothumbnailer.py
-drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-01-26 18:14:45.398496 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/
--rw-rw-r--   0 default   (1010) default   (1010)     3742 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/PKG-INFO
--rw-rw-r--   0 default   (1010) default   (1010)      395 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/SOURCES.txt
--rw-rw-r--   0 default   (1010) default   (1010)        1 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/dependency_links.txt
--rw-rw-r--   0 default   (1010) default   (1010)       80 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/entry_points.txt
--rw-rw-r--   0 default   (1010) default   (1010)       41 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/requires.txt
--rw-rw-r--   0 default   (1010) default   (1010)       19 2023-01-26 18:14:45.000000 pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/top_level.txt
+drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/
+-rw-rw-r--   0 default   (1010) default   (1010)     1522 2020-06-11 15:07:37.000000 pyvideothumbnailer-2.0.3/LICENSE
+-rw-rw-r--   0 default   (1010) default   (1010)     3742 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/PKG-INFO
+-rw-rw-r--   0 default   (1010) default   (1010)     6420 2023-01-26 18:25:30.000000 pyvideothumbnailer-2.0.3/README
+-rw-rw-r--   0 default   (1010) default   (1010)     3155 2023-01-21 20:58:38.000000 pyvideothumbnailer-2.0.3/README.md
+-rw-rw-r--   0 default   (1010) default   (1010)      831 2023-07-28 18:23:09.000000 pyvideothumbnailer-2.0.3/pyproject.toml
+-rw-rw-r--   0 default   (1010) default   (1010)       38 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/setup.cfg
+drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/src/
+drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer/
+-rw-rw-r--   0 default   (1010) default   (1010)        0 2023-01-08 06:25:39.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer/__init__.py
+-rw-rw-r--   0 default   (1010) default   (1010)    56134 2023-07-28 18:21:49.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer/videothumbnailer.py
+drwxrwxr-x   0 default   (1010) default   (1010)        0 2023-07-28 18:38:41.106592 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/
+-rw-rw-r--   0 default   (1010) default   (1010)     3742 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/PKG-INFO
+-rw-rw-r--   0 default   (1010) default   (1010)      395 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/SOURCES.txt
+-rw-rw-r--   0 default   (1010) default   (1010)        1 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/dependency_links.txt
+-rw-rw-r--   0 default   (1010) default   (1010)       80 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/entry_points.txt
+-rw-rw-r--   0 default   (1010) default   (1010)       41 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/requires.txt
+-rw-rw-r--   0 default   (1010) default   (1010)       19 2023-07-28 18:38:41.000000 pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/top_level.txt
```

### Comparing `pyvideothumbnailer-2.0.2/LICENSE` & `pyvideothumbnailer-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvideothumbnailer-2.0.2/PKG-INFO` & `pyvideothumbnailer-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvideothumbnailer
-Version: 2.0.2
+Version: 2.0.3
 Summary: A command line tool for creating video preview thumbnails images.
 Author-email: Harald Hetzner <57875126+hhtznr@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/hhtznr/pyvideothumbnailer
 Project-URL: Bug Tracker, https://github.com/hhtznr/pyvideothumbnailer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvideothumbnailer-2.0.2/README` & `pyvideothumbnailer-2.0.3/README`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 
 The video file name or the directory, where multiple videos are located, always need to be specified as parameter on the command line.
 
 For further reference: https://github.com/hhtznr/pyvideothumbnailer/wiki
 
 
 
-Usage: pyvideothumbnailer [-h] [--width WIDTH] [--columns COLUMNS] [--rows ROWS] [---vertical-video-columns VERTICAL_VIDEO_COLUMNS] [--vertical-video-rows VERTICAL_VIDEO_ROWS] [--spacing SPACING] [--background-color BACKGROUND_COLOR]
+Usage: pyvideothumbnailer [-h] [--width WIDTH] [--columns COLUMNS] [--rows ROWS] [--vertical-video-columns VERTICAL_VIDEO_COLUMNS] [--vertical-video-rows VERTICAL_VIDEO_ROWS] [--spacing SPACING] [--background-color BACKGROUND_COLOR]
                           [--header-font HEADER_FONT] [--header-font-size HEADER_FONT_SIZE] [--header-font-color HEADER_FONT_COLOR] [--timestamp-font TIMESTAMP_FONT] [--timestamp-font-size TIMESTAMP_FONT_SIZE] [--timestamp-font-color TIMESTAMP_FONT_COLOR]
                           [--timestamp-shadow-color TIMESTAMP_SHADOW_COLOR] [--comment-label COMMENT_LABEL] [--comment-text COMMENT_TEXT] [--skip-seconds SKIP_SECONDS] [--suffix SUFFIX] [--jpeg-quality JPEG_QUALITY] [--override-existing] [--recursive]
                           [--output-directory OUTPUT_DIRECTORY] [--raise-errors] [--verbose]
                           [filename]
 
 Positional arguments:
   filename              Video file of which to create preview thumbnails or directory, where multiple video files are located. File name in the current working directory or path. If the argument is omitted, preview thumbnails are generated for video files in
                         the current working directory.
 
 Options:
   -h, --help            show this help message and exit
   --width WIDTH         The intended width of the preview thumbnails image in px. Actual width may be slightly less due rounding upon scaling.
   --columns COLUMNS     The number of preview thumbnail columns.
   --rows ROWS           The number of preview thumbnail rows.
-  ---vertical-video-columns VERTICAL_VIDEO_COLUMNS
+  --vertical-video-columns VERTICAL_VIDEO_COLUMNS
                         The number of preview thumbnail columns in place of '--columns' in case of vertical videos.
   --vertical-video-rows VERTICAL_VIDEO_ROWS
                         The number of preview thumbnail rows in place of '--rows' in case of vertical videos.
   --spacing SPACING     The spacing between and around the preview thumbnails in px.
   --background-color BACKGROUND_COLOR
                         Name or other definition of the PIL color to use for the image background, for information on accepted values see https://pillow.readthedocs.io/en/stable/reference/ImageColor.html
   --no-header           Do not include a header with metadata and optional comment. Enabling this option will make all header settings irrelevant.
```

### Comparing `pyvideothumbnailer-2.0.2/README.md` & `pyvideothumbnailer-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyvideothumbnailer-2.0.2/pyproject.toml` & `pyvideothumbnailer-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyvideothumbnailer"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Harald Hetzner", email="57875126+hhtznr@users.noreply.github.com" },
 ]
 description = "A command line tool for creating video preview thumbnails images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyvideothumbnailer-2.0.2/src/pyvideothumbnailer/videothumbnailer.py` & `pyvideothumbnailer-2.0.3/src/pyvideothumbnailer/videothumbnailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from PIL import Image
 from PIL import ImageColor
 from PIL import ImageDraw
 from PIL import ImageFont
 
 __author__ = 'Harald Hetzner'
 __license__ = 'BSD 3-Clause License'
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 class Parameters:
     """
     Parameters of Python Video Thumbnailer.
     """
 
     DEFAULT_PATH = Path.cwd()
@@ -489,14 +489,18 @@
                     self.parameters.rows = config.getint(ConfigFile.CONFIG_SECTION_LAYOUT, 'rows')
                 if 'vertical_video_columns' in layout_options:
                     self.parameters.vertical_video_columns = config.getint(ConfigFile.CONFIG_SECTION_LAYOUT, 'vertical_video_columns')
                 if 'vertical_video_rows' in layout_options:
                     self.parameters.vertical_video_rows = config.getint(ConfigFile.CONFIG_SECTION_LAYOUT, 'vertical_video_rows')
                 if 'spacing' in layout_options:
                     self.parameters.spacing = config.getint(ConfigFile.CONFIG_SECTION_LAYOUT, 'spacing')
+                if 'background_color' in layout_options:
+                    color_value = config.get(ConfigFile.CONFIG_SECTION_LAYOUT, 'background_color')
+                    if color_value is not None and color_value != '':
+                        self.parameters.background_color= ImageColor.getrgb(color_value)
                 if 'no_header' in layout_options:
                     self.parameters.no_header = config.getboolean(ConfigFile.CONFIG_SECTION_LAYOUT, 'no_header')
                 if 'header_font' in layout_options:
                     self.parameters.header_font_name = config.get(ConfigFile.CONFIG_SECTION_LAYOUT, 'header_font')
                 if 'header_font_size' in layout_options:
                     self.parameters.header_font_size = config.getint(ConfigFile.CONFIG_SECTION_LAYOUT, 'header_font_size')
                 if 'header_font_color' in layout_options:
```

### Comparing `pyvideothumbnailer-2.0.2/src/pyvideothumbnailer.egg-info/PKG-INFO` & `pyvideothumbnailer-2.0.3/src/pyvideothumbnailer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvideothumbnailer
-Version: 2.0.2
+Version: 2.0.3
 Summary: A command line tool for creating video preview thumbnails images.
 Author-email: Harald Hetzner <57875126+hhtznr@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/hhtznr/pyvideothumbnailer
 Project-URL: Bug Tracker, https://github.com/hhtznr/pyvideothumbnailer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

