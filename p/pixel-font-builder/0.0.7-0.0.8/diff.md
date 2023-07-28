# Comparing `tmp/pixel-font-builder-0.0.7.tar.gz` & `tmp/pixel-font-builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.7.tar", last modified: Wed Jul 26 11:13:40 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.8.tar", last modified: Fri Jul 28 12:23:34 2023, max compression
```

## Comparing `pixel-font-builder-0.0.7.tar` & `pixel-font-builder-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.413936 pixel-font-builder-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.413936 pixel-font-builder-0.0.8/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.7/LICENSE` & `pixel-font-builder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/PKG-INFO` & `pixel-font-builder-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

### Comparing `pixel-font-builder-0.0.7/README.md` & `pixel-font-builder-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/pyproject.toml` & `pixel-font-builder-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.7"
+version = "0.0.8"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.8/src/pixel_font_builder/bdf.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.8/src/pixel_font_builder/font.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.8/src/pixel_font_builder/glyph.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.8/src/pixel_font_builder/info.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.8/src/pixel_font_builder/opentype.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             'Weight': context.meta_infos.style_name,
         }
         if context.meta_infos.copyright_info is not None:
             cff_font_infos['Notice'] = context.meta_infos.copyright_info
         builder.setupCFF(cff_ps_name, cff_font_infos, glyphs, {})
 
     logger.debug("Setup 'Character Mapping'")
-    builder.setupCharacterMap(context.character_mapping)
+    builder.setupCharacterMap(context.character_mapping, allowFallback=True)
 
     logger.debug("Setup 'Horizontal Metrics'")
     horizontal_metrics = {}
     for glyph_name in glyph_order:
         advance_width = context.get_glyph(glyph_name).advance_width * context.opentype_configs.px_to_units
         if is_ttf:
             lsb = glyphs[glyph_name].xMin
```

### Comparing `pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

