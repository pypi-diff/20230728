# Comparing `tmp/fretboardgtr-0.1.0.dev1.tar.gz` & `tmp/fretboardgtr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fretboardgtr-0.1.0.dev1.tar", last modified: Fri Feb 17 11:33:00 2023, max compression
+gzip compressed data, was "fretboardgtr-0.2.0.tar", last modified: Fri Jul 28 15:45:26 2023, max compression
```

## Comparing `fretboardgtr-0.1.0.dev1.tar` & `fretboardgtr-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43220 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.459103 fretboardgtr-0.1.0.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.459103 fretboardgtr-0.1.0.dev1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.459103 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/constants.md
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/converters.md
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/elements.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/exporters.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/fretboard.md
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/fretboards.md
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/note_colors.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/notes_creators.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/api_documentation/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.463103 fretboardgtr-0.1.0.dev1/docs/source/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/assets/black_logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/assets/black_logo_square@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/assets/white_logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/assets/white_logo_square@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.463103 fretboardgtr-0.1.0.dev1/docs/source/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/get-started/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/get-started/get-started.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.463103 fretboardgtr-0.1.0.dev1/fretboardgtr/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.463103 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/background.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/fret_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/frets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/neck_dots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/nut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/elements/tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/fretboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    16488 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/note_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/notes_creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/fretboardgtr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.463103 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43220 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-17 11:33:00.000000 fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:00.467103 fretboardgtr-0.1.0.dev1/tests/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_fret_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_frets.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_neck_dots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_nut.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/elements/test_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_fretboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_fretboard_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_notes_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-02-17 11:32:51.000000 fretboardgtr-0.1.0.dev1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.173941 fretboardgtr-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-07-28 15:45:26.173941 fretboardgtr-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/docs/source/api_documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/constants.md
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/converters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/exporters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/fretboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/fretboards.md
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/note_colors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/notes_creators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/api_documentation/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/docs/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/assets/black_logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/assets/black_logo_square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/assets/white_logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/assets/white_logo_square@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/docs/source/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/get-started/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/get-started/get-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/get-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.165941 fretboardgtr-0.2.0/fretboardgtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.169941 fretboardgtr-0.2.0/fretboardgtr/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/fret_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/frets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/neck_dots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/nut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/elements/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.169941 fretboardgtr-0.2.0/fretboardgtr/fretboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/fretboards/vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/note_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/notes_creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/fretboardgtr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.169941 fretboardgtr-0.2.0/fretboardgtr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43215 2023-07-28 15:45:26.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-28 15:45:26.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:45:26.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:45:25.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-28 15:45:26.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 15:45:26.000000 fretboardgtr-0.2.0/fretboardgtr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:45:26.173941 fretboardgtr-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.169941 fretboardgtr-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.169941 fretboardgtr-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:45:26.173941 fretboardgtr-0.2.0/tests/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_fret_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_frets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_neck_dots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_nut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/elements/test_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_fretboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_fretboard_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_notes_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-28 15:45:11.000000 fretboardgtr-0.2.0/tests/test_utils.py
```

### Comparing `fretboardgtr-0.1.0.dev1/CONTRIBUTING.md` & `fretboardgtr-0.2.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -124,28 +124,48 @@
 
 ## Tips
 
 To run a subset of tests :
 ```
 python -m pytest tests.test_fretboardgtr
 ```
-## Deploying
+## Deploying and bump2version
 
 A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run:
+Make sure all your changes are committed.
 
 ```
-bump2version patch # possible: major / minor / patch / release_candidate / dev
-git push
+bump2version patch # possible: major / minor / patch
+```
+
+Will bump for example 0.1.0 to 0.2.0-dev0.
+
+We can then use :
+
+```
+bump2version dev
+```
+
+To bump  0.2.0-dev0 to 0.2.0-dev1 and so on.
+
+If you want to commit and tag directly the pre-release you can
+run for example :
+
+```
+bump2version dev --commit --tag
+```
+
+When a release is ready we then run (on a clean repo):
+
+```
+bump2version release --commit --tag
 git push --tags
 ```
 
-This will then deploy the package in PyPI if tests pass and a tag is set,
-otherwise it will deployed on test-pipy.
+This will then deploy the package in PyPI if tests pass and a tag is set, otherwise it will deployed on test-pipy.
 
 ## Further words
 
 ### `pre-commit`
 
 Most of the pre-commit hooks require you to do nothing but save the changes. However, some pre-commits (e.g. `pydocstyle`) are sometimes hard to respect and can slow down your workflow. Although we recommend to let all of them to have a cleaner repo, if one or more are really annoying for you, you can remove or comment them in the `.pre-commit-config.yaml` file.
```

### Comparing `fretboardgtr-0.1.0.dev1/LICENSE` & `fretboardgtr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/PKG-INFO` & `fretboardgtr-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fretboardgtr
-Version: 0.1.0.dev1
+Version: 0.2.0
 Summary: Package that make easy creation of fretboards and chords diagrams
 Author-email: Antoine Gibek <antoine.gibek@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fretboardgtr-0.1.0.dev1/README.md` & `fretboardgtr-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/Makefile` & `fretboardgtr-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/make.bat` & `fretboardgtr-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/api_documentation/elements.md` & `fretboardgtr-0.2.0/docs/source/api_documentation/elements.md`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/assets/black_logo@2x.png` & `fretboardgtr-0.2.0/docs/source/assets/black_logo@2x.png`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/assets/black_logo_square@2x.png` & `fretboardgtr-0.2.0/docs/source/assets/black_logo_square@2x.png`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/assets/white_logo@2x.png` & `fretboardgtr-0.2.0/docs/source/assets/white_logo@2x.png`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/assets/white_logo_square@2x.png` & `fretboardgtr-0.2.0/docs/source/assets/white_logo_square@2x.png`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/conf.py` & `fretboardgtr-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/docs/source/get-started/configuration.md` & `fretboardgtr-0.2.0/docs/source/get-started/configuration.md`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/__init__.py` & `fretboardgtr-0.2.0/fretboardgtr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,18 @@
     FrettedNoteConfig,
     OpenNote,
     OpenNoteConfig,
 )
 from fretboardgtr.elements.nut import Nut, NutConfig
 from fretboardgtr.elements.strings import String, StringConfig
 from fretboardgtr.elements.tuning import Tuning, TuningConfig
-from fretboardgtr.fretboard import FretBoard, VerticalFretBoard
+from fretboardgtr.fretboard import FretBoard
 from fretboardgtr.fretboards.base import FretBoardLike
 from fretboardgtr.fretboards.config import FretBoardConfig, FretBoardGeneralConfig
 from fretboardgtr.fretboards.converters import FretBoardToSVGConverter
 from fretboardgtr.fretboards.elements import FretBoardElements
-from fretboardgtr.fretboards.fretboard import FretBoardContainer
-from fretboardgtr.fretboards.vertical import VerticalFretBoardContainer
 from fretboardgtr.note_colors import NoteColors
 from fretboardgtr.notes_creators import NotesContainer
 
 __author__ = "Antoine Gibek"
 __email__ = "antoine.gibek@gmail.com"
 __version__ = version_str
```

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/base.py` & `fretboardgtr-0.2.0/fretboardgtr/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+import logging
 from typing import Any, Dict
 
 
 class ConfigIniter:
     """Mixin class that define methods read the different configurations.
 
     All the components/elements configuration must subclass this Mixin.
     Then, all the configuration can be read thank to the method (eg
     from_dict) recursively
     """
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> Any:
         kwargs = {}
-        for arg, _type in cls.__annotations__.items():
-            if arg not in _dict:
+        for arg in _dict:
+            if arg not in cls.__annotations__.keys():
+                logging.warning(
+                    f'"{arg}" key confuration was not found in {cls.__name__}'
+                )
                 continue
+            _type = cls.__annotations__[arg]
             if hasattr(_type, "from_dict"):
                 kwargs[arg] = _type.from_dict(_dict[arg])
             else:
                 kwargs[arg] = _dict[arg]
         return cls(**kwargs)
```

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/constants.py` & `fretboardgtr-0.2.0/fretboardgtr/constants.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/background.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/background.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/cross.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/cross.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/fret_number.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/fret_number.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/frets.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/frets.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/neck_dots.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/neck_dots.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/notes.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/notes.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/nut.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/nut.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/strings.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/strings.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/elements/tuning.py` & `fretboardgtr-0.2.0/fretboardgtr/elements/tuning.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/exporters.py` & `fretboardgtr-0.2.0/fretboardgtr/exporters.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/base.py` & `fretboardgtr-0.2.0/fretboardgtr/fretboards/base.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/converters.py` & `fretboardgtr-0.2.0/fretboardgtr/fretboards/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,15 @@
         return drawing
 
     def convert(self) -> svgwrite.Drawing:
         drawing = self.get_empty()
         elements = self._fretboard.get_elements()
         for key in fields(elements):
             element = getattr(elements, key.name, None)
+            if element is None:
+                continue
             if isinstance(element, list):
                 for sub in element:
                     drawing = self.add_to_drawing(drawing, sub)
             else:
                 drawing = self.add_to_drawing(drawing, element)  # type: ignore
         return drawing
```

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/fretboards/elements.py` & `fretboardgtr-0.2.0/fretboardgtr/fretboards/elements.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/note_colors.py` & `fretboardgtr-0.2.0/fretboardgtr/note_colors.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr/utils.py` & `fretboardgtr-0.2.0/fretboardgtr/utils.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/PKG-INFO` & `fretboardgtr-0.2.0/fretboardgtr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fretboardgtr
-Version: 0.1.0.dev1
+Version: 0.2.0
 Summary: Package that make easy creation of fretboards and chords diagrams
 Author-email: Antoine Gibek <antoine.gibek@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fretboardgtr-0.1.0.dev1/fretboardgtr.egg-info/SOURCES.txt` & `fretboardgtr-0.2.0/fretboardgtr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 fretboardgtr/elements/strings.py
 fretboardgtr/elements/tuning.py
 fretboardgtr/fretboards/__init__.py
 fretboardgtr/fretboards/base.py
 fretboardgtr/fretboards/config.py
 fretboardgtr/fretboards/converters.py
 fretboardgtr/fretboards/elements.py
-fretboardgtr/fretboards/fretboard.py
+fretboardgtr/fretboards/horizontal.py
 fretboardgtr/fretboards/vertical.py
 tests/__init__.py
 tests/test_e2e.py
 tests/test_exporters.py
 tests/test_fretboard.py
 tests/test_fretboard_vertical.py
 tests/test_notes_creator.py
```

### Comparing `fretboardgtr-0.1.0.dev1/pyproject.toml` & `fretboardgtr-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
 ]
 keywords=['fretboardgtr', "fretboard", "chord", "guitar", "bass"]
-dependencies=["reportlab", "svglib", "svgwrite"]
+dependencies=["reportlab<=4", "svglib", "svgwrite"]
 # Dynamic for setuptools
 dynamic = ["version"]
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
```

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_background.py` & `fretboardgtr-0.2.0/tests/elements/test_background.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_fret_number.py` & `fretboardgtr-0.2.0/tests/elements/test_fret_number.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_frets.py` & `fretboardgtr-0.2.0/tests/elements/test_frets.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_neck_dots.py` & `fretboardgtr-0.2.0/tests/elements/test_neck_dots.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_notes.py` & `fretboardgtr-0.2.0/tests/elements/test_notes.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_nut.py` & `fretboardgtr-0.2.0/tests/elements/test_nut.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_strings.py` & `fretboardgtr-0.2.0/tests/elements/test_strings.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/elements/test_tuning.py` & `fretboardgtr-0.2.0/tests/elements/test_tuning.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/test_exporters.py` & `fretboardgtr-0.2.0/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `fretboardgtr-0.1.0.dev1/tests/test_fretboard.py` & `fretboardgtr-0.2.0/tests/test_fretboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     FrettedNoteConfig,
     OpenNote,
     OpenNoteConfig,
 )
 from fretboardgtr.elements.nut import Nut, NutConfig
 from fretboardgtr.elements.strings import String, StringConfig
 from fretboardgtr.elements.tuning import Tuning, TuningConfig
+from fretboardgtr.fretboard import FretBoard
 from fretboardgtr.fretboards.config import FretBoardConfig, FretBoardGeneralConfig
-from fretboardgtr.fretboards.fretboard import FretBoardContainer
 from fretboardgtr.note_colors import NoteColors
 from fretboardgtr.notes_creators import NotesContainer
 
 
 @pytest.fixture()
 def default_config():
     return FretBoardConfig(
@@ -196,51 +196,46 @@
     )
 
 
 def test_default_config(default_config: FretBoardConfig):
     assert default_config == FretBoardConfig()
 
 
-def test_default_config_container(default_config):
-    vertical_fretboard = FretBoardContainer()
-    assert vertical_fretboard.config == default_config
-
-
 def load_config_from_dict(dict_config):
     config = FretBoardConfig.from_dict(dict_config)
     assert config == FretBoardConfig()
 
 
 def load_config_from_partial_dict(partial_dict_config):
     config = FretBoardConfig.from_dict(partial_dict_config)
     assert config.background.color == "blue"
     # The default is still there
     assert config.background.opacity == 0.2
 
 
 def test_fretboard_get_background(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_background()
     background = fretboard.elements.background
     # Position == (width_fret + x_start, y_start)
     assert background.position == (100, 30)
     assert background.size == (840, 250)
 
 
 def test_fretboard_get_background_new_tuning(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config, tuning=["E", "A", "D", "G"])
+    fretboard = FretBoard(config=default_config, tuning=["E", "A", "D", "G"])
     fretboard.add_background()
     background = fretboard.elements.background
     # Position == (width_fret + x_start, y_start)
     assert background.position == (100, 30)
     assert background.size == (840, 150)
 
 
 def test_fretboard_get_neck_dots(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_neck_dots()
     neck_dots = fretboard.elements.neck_dots
     assert neck_dots[0].x == 275.0
     assert neck_dots[0].y == 155.0
     for neck_dot in neck_dots:
         # Check if center of fret
         assert (
@@ -258,15 +253,15 @@
                 - (fretboard.config.general.fret_height // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_frets(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_frets()
     frets = fretboard.elements.frets
     for fret in frets:
         # Test if multiple of width
         assert (
             fret.start_position[0] % fretboard.config.general.x_start
             + fretboard.config.general.fret_width
@@ -279,15 +274,15 @@
         assert fret.end_position[1] == (
             fretboard.config.general.y_start
             + (len(fretboard.tuning) - 1) * fretboard.config.general.fret_height
         )
 
 
 def test_fretboard_get_strings(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_strings()
     strings = fretboard.elements.strings
     for string in strings:
         # Test if horizontal line
         assert string.start_position[1] == string.end_position[1]
 
         # Test if multiple of width
@@ -305,15 +300,15 @@
             fretboard.config.general.y_start
             + fretboard.config.general.fret_width
             + fretboard.config.general.last_fret * fretboard.config.general.fret_width
         )
 
 
 def test_fretboard_get_nut(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_nut()
     nut = fretboard.elements.nut
     assert nut is not None
     # Test if vertical line
     assert nut.start_position[0] == nut.end_position[0]
     # Test if start where it should
     assert (
@@ -328,22 +323,22 @@
         == fretboard.config.general.y_start
         + (len(fretboard.tuning) - 1) * fretboard.config.general.fret_height
     )
 
 
 def test_fretboard_get_nut_not_first_fret(default_config: FretBoardConfig):
     default_config.general.first_fret = 1
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_nut()
 
     assert fretboard.elements.nut is None
 
 
 def test_fretboard_get_fret_numbers(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_fret_numbers()
     fret_numbers = fretboard.elements.fret_numbers
     assert fret_numbers is not None
     assert fret_numbers[0].x == 275.0
     assert fret_numbers[0].y == 330.0
     for fret_number in fret_numbers:
         # Check if center of fret
@@ -362,15 +357,15 @@
                 - (fretboard.config.general.fret_height // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_string(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     strings = fretboard.add_strings()
     strings = fretboard.elements.strings
     for string in strings:
         # Test if horizontal line
         assert string.start_position[1] == string.end_position[1]
 
         # Test if multiple of width
@@ -388,121 +383,121 @@
             fretboard.config.general.y_start
             + fretboard.config.general.fret_width
             + fretboard.config.general.last_fret * fretboard.config.general.fret_width
         )
 
 
 def test_fretboard_get_open_note(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_open_note(position=(100, 100), note="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     assert open_note.config.color == "rgb(255,255,255)"
 
 
 def test_fretboard_get_open_note_root(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_open_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     assert open_note.config.color == "rgb(255,255,255)"
 
 
 def test_fretboard_get_open_note_root_colors(default_config: FretBoardConfig):
     default_config.general.open_color_scale = True
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_open_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_open_note_show_degree_name(default_config: FretBoardConfig):
     default_config.general.open_color_scale = True
     default_config.general.show_degree_name = True
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_open_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "1"
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_open_note_no_name(default_config: FretBoardConfig):
     default_config.general.open_color_scale = True
     default_config.general.show_degree_name = False
     default_config.general.show_note_name = False
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_open_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == ""
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_fretted_note(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_fretted_note(position=(100, 100), note="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     assert open_note.config.color == "rgb(255,255,255)"
 
 
 def test_fretboard_get_fretted_note_root_colors(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_fretted_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_fretted_note_root_no_color(default_config: FretBoardConfig):
     default_config.general.fretted_color_scale = False
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_fretted_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "C"
     assert open_note.config.color == "rgb(255,255,255)"
 
 
 def test_fretboard_get_fretted_note_show_degree_name(default_config: FretBoardConfig):
     default_config.general.show_degree_name = True
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_fretted_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == "1"
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_fretted_note_no_name(default_config: FretBoardConfig):
     default_config.general.show_degree_name = False
     default_config.general.show_note_name = False
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     open_note = fretboard._get_fretted_note(position=(100, 100), note="C", root="C")
     assert open_note.x == 100
     assert open_note.y == 100
     assert open_note.name == ""
     # RED
     assert open_note.config.color == "rgb(231, 0, 0)"
 
 
 def test_fretboard_get_notes(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_note(string_no=0, note="E", root="C")
 
     notes = fretboard.elements.notes
     for note in notes:
         assert note.y == fretboard.config.general.y_start
         # Check if placed between two frets
         assert (
@@ -512,73 +507,73 @@
                 - (fretboard.config.general.fret_width // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_notes_invalid_string(default_config: FretBoardConfig):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     with pytest.raises(ValueError):
         fretboard.add_note(string_no=7, note="E", root="C")
 
 
 def test_fretboard_get_inside_bounds(default_config):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     upper_left, lower_right = fretboard.get_inside_bounds()
     assert upper_left == (30.0, 30.0)
     assert lower_right == (940.0, 280.0)
 
 
 def test_fretboard_get_size(default_config):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     width, height = fretboard.get_size()
     assert width == 1010.0
     assert height == 380.0
 
 
 def test_init_fretboard(default_config):
-    fretboard = FretBoardContainer(config=default_config)
-    assert len(fretboard.elements) == 37
+    fretboard = FretBoard(config=default_config)
+    assert len(fretboard.elements) == 38
     assert len(fretboard.elements.strings) == 6
-    assert len(fretboard.elements.frets) == 12
+    assert len(fretboard.elements.frets) == 13
     list_of_elements = fretboard.elements.to_list()
     assert any([isinstance(obj, FretNumber) for obj in list_of_elements])
     assert any([isinstance(obj, Fret) for obj in list_of_elements])
     assert any([isinstance(obj, NeckDot) for obj in list_of_elements])
     assert any([isinstance(obj, Nut) for obj in list_of_elements])
     assert any([isinstance(obj, String) for obj in list_of_elements])
     assert any([isinstance(obj, Tuning) for obj in list_of_elements])
     assert not any([isinstance(obj, FrettedNote) for obj in list_of_elements])
     assert not any([isinstance(obj, OpenNote) for obj in list_of_elements])
 
 
 def test_init_fretboard_add_notes(default_config):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     notes_container = NotesContainer(
         root="C", notes=["C", "D", "E", "F", "G", "A", "B"]
     )
     fretboard.add_notes(notes_container)
-    assert len(fretboard.elements) == 85
+    assert len(fretboard.elements) == 86
     assert len(fretboard.elements.strings) == 6
-    assert len(fretboard.elements.frets) == 12
+    assert len(fretboard.elements.frets) == 13
     list_of_elements = fretboard.elements.to_list()
     assert any([isinstance(obj, Background) for obj in list_of_elements])
     assert any([isinstance(obj, FretNumber) for obj in list_of_elements])
     assert any([isinstance(obj, Fret) for obj in list_of_elements])
     assert any([isinstance(obj, NeckDot) for obj in list_of_elements])
     assert any([isinstance(obj, Nut) for obj in list_of_elements])
     assert any([isinstance(obj, String) for obj in list_of_elements])
     assert any([isinstance(obj, Tuning) for obj in list_of_elements])
     assert any([isinstance(obj, FrettedNote) for obj in list_of_elements])
     assert any([isinstance(obj, OpenNote) for obj in list_of_elements])
 
 
 def test_add_element(default_config):
     note = OpenNote("C", position=(0, 0))
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     fretboard.add_element(note)
 
 
 def test_add_wrong_lement(default_config):
-    fretboard = FretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config)
     with pytest.raises(ValueError):
         fretboard.add_element(1)
```

### Comparing `fretboardgtr-0.1.0.dev1/tests/test_fretboard_vertical.py` & `fretboardgtr-0.2.0/tests/test_fretboard_vertical.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     FrettedNoteConfig,
     OpenNote,
     OpenNoteConfig,
 )
 from fretboardgtr.elements.nut import Nut, NutConfig
 from fretboardgtr.elements.strings import String, StringConfig
 from fretboardgtr.elements.tuning import Tuning, TuningConfig
+from fretboardgtr.fretboard import FretBoard
 from fretboardgtr.fretboards.config import FretBoardConfig, FretBoardGeneralConfig
-from fretboardgtr.fretboards.vertical import VerticalFretBoardContainer
 from fretboardgtr.note_colors import NoteColors
 from fretboardgtr.notes_creators import NotesContainer
 
 
 @pytest.fixture()
 def default_config():
     return FretBoardConfig(
@@ -101,45 +101,35 @@
             text_color="rgb(0,0,0)",
             fontsize=20,
             fontweight="bold",
         ),
     )
 
 
-def test_default_config_container(default_config):
-    vertical_fretboard = VerticalFretBoardContainer()
-    assert vertical_fretboard.config == default_config
-
-
-def load_config_from_dict(dict_config):
-    config = FretBoardConfig.from_dict(dict_config)
-    assert config == FretBoardConfig()
-
-
 def test_fretboard_get_background(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_background()
     background = fretboard.elements.background
     # Position == (width_fret + x_start, y_start)
     assert background.position == (80, 30)[::-1]
     assert background.size == (600, 250)[::-1]
 
 
 def test_fretboard_get_background_new_tuning(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(
-        config=default_config, tuning=["E", "A", "D", "G"]
+    fretboard = FretBoard(
+        config=default_config, tuning=["E", "A", "D", "G"], vertical=True
     )
     fretboard.add_background()
     background = fretboard.elements.background
     assert background.position == (80, 30)[::-1]
     assert background.size == (600, 150)[::-1]
 
 
 def test_fretboard_get_neck_dots(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_neck_dots()
     neck_dots = fretboard.elements.neck_dots
     assert neck_dots[0].x == 155.0
     assert neck_dots[0].y == 205.0
     for neck_dot in neck_dots:
         # Check if center of fret
         assert (
@@ -157,15 +147,15 @@
                 - (fretboard.config.general.fret_height // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_frets(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_frets()
     frets = fretboard.elements.frets
     for fret in frets:
         # Test if multiple of width
         assert (
             fret.start_position[0] % fretboard.config.general.x_start
             + fretboard.config.general.fret_width
@@ -178,15 +168,15 @@
         assert fret.end_position[0] == (
             fretboard.config.general.x_start
             + (len(fretboard.tuning) - 1) * fretboard.config.general.fret_width
         )
 
 
 def test_fretboard_get_strings(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_strings()
     strings = fretboard.elements.strings
     for string in strings:
         # Test if vertical line
         assert string.start_position[0] == string.end_position[0]
 
         # Test if multiple of width
@@ -204,15 +194,15 @@
             fretboard.config.general.y_start
             + fretboard.config.general.fret_height
             + fretboard.config.general.last_fret * fretboard.config.general.fret_width
         )
 
 
 def test_fretboard_get_nut(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_nut()
     nut = fretboard.elements.nut
     assert nut is not None
     # Test if horizontal line
     assert nut.start_position[1] == nut.end_position[1]
     # Test if start where it should
     assert (
@@ -227,22 +217,22 @@
     #     fretboard.config.general.x_start
     #     + (len(fretboard.tuning) - 1) * fretboard.config.general.fret_width
     # )
 
 
 def test_fretboard_get_nut_not_first_fret(default_config: FretBoardConfig):
     default_config.general.first_fret = 1
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_nut()
 
     assert fretboard.elements.nut is None
 
 
 def test_fretboard_get_fret_numbers(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_fret_numbers()
     fret_numbers = fretboard.elements.fret_numbers
     assert fret_numbers is not None
     assert fret_numbers[0].x == 330.0
     assert fret_numbers[0].y == 205.0
     for fret_number in fret_numbers:
         # Check if center of fret
@@ -261,15 +251,15 @@
                 - (fretboard.config.general.fret_height // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_notes(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_note(string_no=0, note="E", root="C")
 
     notes = fretboard.elements.notes
     for note in notes:
         assert note.x == fretboard.config.general.x_start
         # Check if placed between two frets
         assert (
@@ -279,73 +269,73 @@
                 - (fretboard.config.general.fret_width // 2)
             )
             == 0
         )
 
 
 def test_fretboard_get_notes_invalid_string(default_config: FretBoardConfig):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     with pytest.raises(ValueError):
         fretboard.add_note(string_no=7, note="E", root="C")
 
 
 def test_fretboard_get_inside_bounds(default_config):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     upper_left, lower_right = fretboard.get_inside_bounds()
     assert upper_left == (30.0, 30.0)
     assert lower_right == (280.0, 680.0)
 
 
 def test_fretboard_get_size(default_config):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     width, height = fretboard.get_size()
     assert width == 380.0
     assert height == 730.0
 
 
 def test_init_fretboard(default_config):
-    fretboard = VerticalFretBoardContainer(config=default_config)
-    assert len(fretboard.elements) == 37
+    fretboard = FretBoard(config=default_config, vertical=True)
+    assert len(fretboard.elements) == 38
     assert len(fretboard.elements.strings) == 6
-    assert len(fretboard.elements.frets) == 12
+    assert len(fretboard.elements.frets) == 13
     list_of_elements = fretboard.elements.to_list()
     assert any([isinstance(obj, FretNumber) for obj in list_of_elements])
     assert any([isinstance(obj, Fret) for obj in list_of_elements])
     assert any([isinstance(obj, NeckDot) for obj in list_of_elements])
     assert any([isinstance(obj, Nut) for obj in list_of_elements])
     assert any([isinstance(obj, String) for obj in list_of_elements])
     assert any([isinstance(obj, Tuning) for obj in list_of_elements])
     assert not any([isinstance(obj, FrettedNote) for obj in list_of_elements])
     assert not any([isinstance(obj, OpenNote) for obj in list_of_elements])
 
 
 def test_init_fretboard_add_notes(default_config):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     notes_container = NotesContainer(
         root="C", notes=["C", "D", "E", "F", "G", "A", "B"]
     )
     fretboard.add_notes(notes_container)
-    assert len(fretboard.elements) == 85
+    assert len(fretboard.elements) == 86
     assert len(fretboard.elements.strings) == 6
-    assert len(fretboard.elements.frets) == 12
+    assert len(fretboard.elements.frets) == 13
     list_of_elements = fretboard.elements.to_list()
     assert any([isinstance(obj, Background) for obj in list_of_elements])
     assert any([isinstance(obj, FretNumber) for obj in list_of_elements])
     assert any([isinstance(obj, Fret) for obj in list_of_elements])
     assert any([isinstance(obj, NeckDot) for obj in list_of_elements])
     assert any([isinstance(obj, Nut) for obj in list_of_elements])
     assert any([isinstance(obj, String) for obj in list_of_elements])
     assert any([isinstance(obj, Tuning) for obj in list_of_elements])
     assert any([isinstance(obj, FrettedNote) for obj in list_of_elements])
     assert any([isinstance(obj, OpenNote) for obj in list_of_elements])
 
 
 def test_add_element(default_config):
     note = OpenNote("C", position=(0, 0))
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     fretboard.add_element(note)
 
 
 def test_add_wrong_lement(default_config):
-    fretboard = VerticalFretBoardContainer(config=default_config)
+    fretboard = FretBoard(config=default_config, vertical=True)
     with pytest.raises(ValueError):
         fretboard.add_element(1)
```

### Comparing `fretboardgtr-0.1.0.dev1/tests/test_utils.py` & `fretboardgtr-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

