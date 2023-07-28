# Comparing `tmp/inventree-wireviz-plugin-0.4.1.tar.gz` & `tmp/inventree-wireviz-plugin-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.4.1.tar", last modified: Mon Jun  5 03:41:08 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.4.2.tar", last modified: Fri Jul 28 03:37:50 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.4.1.tar` & `inventree-wireviz-plugin-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 03:41:08.000000 inventree-wireviz-plugin-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 03:40:57.000000 inventree-wireviz-plugin-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19871 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-28 03:37:50.000000 inventree-wireviz-plugin-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 03:37:38.000000 inventree-wireviz-plugin-0.4.2/setup.py
```

### Comparing `inventree-wireviz-plugin-0.4.1/LICENSE` & `inventree-wireviz-plugin-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.1/PKG-INFO` & `inventree-wireviz-plugin-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.4.1
+Version: 0.4.2
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.4.1/README.md` & `inventree-wireviz-plugin-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.1/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.4.2/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.1/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.4.2/inventree_wireviz/wireviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,19 @@
         part = self.get_part_from_instance(model_instance)
 
         if isinstance(part, Part):
             metadata = part.get_metadata('wireviz')
 
             if metadata:
                 if svg_file := metadata.get(self.HARNESS_SVG_KEY, None):
-                    context['wireviz_svg_file'] = svg_file
+                    svg_path = os.path.join(settings.MEDIA_ROOT, svg_file)
+                    
+                    # Ensure that the file really does exist
+                    if os.path.exists(svg_path):
+                        context['wireviz_svg_file'] = svg_file
 
                 if bom_data := metadata.get(self.HARNESS_BOM_KEY, None):
                     context['wireviz_bom_data'] = bom_data
 
     def get_panel_context(self, view, request, context):
         """Return context information for the Wireviz panel."""
```

### Comparing `inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.4.1
+Version: 0.4.2
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.4.1/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.4.2/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.4.1/setup.py` & `inventree-wireviz-plugin-0.4.2/setup.py`

 * *Files identical despite different names*

