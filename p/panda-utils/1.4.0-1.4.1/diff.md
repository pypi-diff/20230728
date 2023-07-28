# Comparing `tmp/panda_utils-1.4.0.tar.gz` & `tmp/panda_utils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.4.0.tar", last modified: Tue Jul 11 16:26:13 2023, max compression
+gzip compressed data, was "panda_utils-1.4.1.tar", last modified: Fri Jul 28 09:46:45 2023, max compression
```

## Comparing `panda_utils-1.4.0.tar` & `panda_utils-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.0/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-11 16:26:13.308351 panda_utils-1.4.0/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.0/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.0/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.0/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.0/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.0/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     4488 2023-07-08 05:09:48.000000 panda_utils-1.4.0/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      256 2023-06-13 10:12:15.000000 panda_utils-1.4.0/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      269 2023-07-09 18:02:42.000000 panda_utils-1.4.0/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    12990 2023-07-11 15:46:06.000000 panda_utils-1.4.0/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.0/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.0/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      614 2023-07-11 09:02:42.000000 panda_utils-1.4.0/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      526 2023-06-12 20:26:53.000000 panda_utils-1.4.0/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.0/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.0/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5608 2023-07-07 09:32:40.000000 panda_utils-1.4.0/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      631 2023-06-12 17:03:28.000000 panda_utils-1.4.0/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.0/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.0/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.0/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.0/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.0/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.0/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.0/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-11 16:26:13.308351 panda_utils-1.4.0/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      950 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-11 16:26:13.000000 panda_utils-1.4.0/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-11 15:59:43.000000 panda_utils-1.4.0/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.0/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-11 16:26:13.308351 panda_utils-1.4.0/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.1/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-28 09:46:45.679729 panda_utils-1.4.1/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.1/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.1/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.676396 panda_utils-1.4.1/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.1/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.1/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.1/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5056 2023-07-28 09:29:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      807 2023-07-26 20:53:08.000000 panda_utils-1.4.1/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14512 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.1/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.1/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.1/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.1/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.1/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.1/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.1/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.1/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.1/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.1/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.1/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.1/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.676396 panda_utils-1.4.1/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-28 09:44:37.000000 panda_utils-1.4.1/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.1/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-28 09:46:45.679729 panda_utils-1.4.1/setup.cfg
```

### Comparing `panda_utils-1.4.0/LICENSE` & `panda_utils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/PKG-INFO` & `panda_utils-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.4.0
+Version: 1.4.1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.0/README.md` & `panda_utils-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/__main__.py` & `panda_utils-1.4.1/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.4.1/panda_utils/assetpipeline/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import pathlib
 import shutil
 import sys
 
 import yaml
 
 from panda_utils.assetpipeline import imports
 from panda_utils.eggtree import eggparse
@@ -27,14 +28,16 @@
         self.name = self.model_name.replace("-", " ").replace("_", " ").title()
 
         self.intermediate_path = f"{OUTPUT_PARENT}/{output_phase}/models/{output_folder}/{self.model_name}"
         self.output_model_rel = f"{output_phase}/models/{output_folder}"
         self.output_model = os.path.abspath(os.path.dirname(self.intermediate_path))
         self.output_texture = os.path.abspath(f"{OUTPUT_PARENT}/{output_phase}/maps")
         self.eggs = None
+        self.path_overrides = {}
+        self.post_remove = set()
 
     def cache_eggs(self):
         if self.eggs is not None:
             return
 
         self.eggs = {}
         for file in self.files:
@@ -52,14 +55,22 @@
                 f.write(str(tree))
         self.eggs = None
 
     @property
     def files(self):
         return sorted(os.listdir())
 
+    @staticmethod
+    def get_injection_path(name):
+        injections_base_path = pathlib.Path("..", "..", "common")
+        all_injections = os.listdir(injections_base_path)
+        if name not in all_injections:
+            return None
+        return injections_base_path / name
+
     def run_action_through_config(self, action, name):
         if YAML_CONFIG_FILENAME not in self.files:
             return
 
         with open(YAML_CONFIG_FILENAME) as f:
             data = yaml.safe_load(f)
 
@@ -77,14 +88,22 @@
         if isinstance(args, dict):
             action(self, **args)
         elif isinstance(args, str):
             action(self, args)
         else:
             logger.warning("%s: Invalid configured arguments: %s (expected dict, or str)", self.name, type(args))
 
+    @staticmethod
+    def reverse_rmdir(path):
+        while not os.listdir(path):
+            path.rmdir()
+            path = path.parent
+            if path[-1] == OUTPUT_PARENT:
+                break
+
 
 def main(enable_logging=False):
     if enable_logging:
         console = logging.StreamHandler()
         console.setLevel(logging.INFO)
         formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
         console.setFormatter(formatter)
```

### Comparing `panda_utils-1.4.0/panda_utils/assetpipeline/models.py` & `panda_utils-1.4.1/panda_utils/assetpipeline/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import fnmatch
 import logging
 import os
+import pathlib
 import platform
 import re
 import shutil
 import subprocess
 from pathlib import Path
 
 from panda_utils import util
 from panda_utils.eggtree import eggparse, operations
 from panda_utils.tools.convert import bam2egg, egg2bam
 from panda_utils.tools.palettize import remove_palette_indices
 from panda_utils.util import get_data_file_path
 
 preblend_regex = re.compile(r".*\.(fbx|obj)")
+image_regex = re.compile(r".*\.(png|jpg|rgb)")
 logger = logging.getLogger("panda_utils.pipeline.models")
 
 
 def run_blender(cwd, file, script, *inputs):
     args = [util.choose_binary("blender"), "--background", "--python", get_data_file_path(script), "--", *inputs]
     if file is not None:
         args.insert(1, file)
@@ -80,16 +82,18 @@
             args.append("legacy")
     return args
 
 
 def __run_export_util(ctx, binary, input_file, output_file, flags):
     res = subprocess.run(
         [binary, *__make_blend2bam_args(binary, flags), input_file, output_file],
-        stdout=subprocess.DEVNULL, stderr=subprocess.PIPE, cwd=ctx.cwd
-        )
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.PIPE,
+        cwd=ctx.cwd,
+    )
     err = res.stderr.decode("utf-8")
     if err and "KeyError: 'nodes'" in err:
         logger.error("%s: Blender output an empty model, aborting.", ctx.name)
         ctx.valid = False
     elif err:
         logger.error("%s: Blender failed", ctx.name)
         print(err)
@@ -131,32 +135,43 @@
 def action_bam2egg(ctx):
     for file in ctx.files:
         if file.endswith(".bam"):
             logger.info("%s: Converting %s from Bam to Egg", ctx.name, file)
             bam2egg(ctx.putil_ctx, file)
 
 
-def action_optimize(ctx):
+def action_yabee(ctx):
+    for file in ctx.files:
+        if file.endswith(".blend"):
+            logger.info("%s: Exporting through YABEE: %s", ctx.name, file)
+            full_path = f"{ctx.cwd}/{file}"
+            run_blender(ctx.cwd, full_path, "blender/export_with_yabee.py", file[:-6] + ".egg")
+
+
+def action_optimize(ctx, map_textures="true"):
+    map_textures = map_textures.lower() not in ("", "0", "false")
+
     textures = set()
     ctx.cache_eggs()
     for tree in ctx.eggs.values():
         for tex in tree.findall("Texture"):
             textures.add(eggparse.sanitize_string(tex.get_child(0).value))
 
-    texture_mapper = build_asset_mapper(textures, ctx.model_name)
+    texture_mapper = build_asset_mapper(textures, ctx.model_name) if map_textures else {}
     for fnold, fnnew in texture_mapper.items():
         fnold = __patch_filename(fnold)
         shutil.move(fnold, fnnew)
 
     for file, eggtree in ctx.eggs.items():
         logger.info("%s: Optimizing model: %s", ctx.name, file)
         # The first thing we should do is patch the texture paths
         for tex in eggtree.findall("Texture"):
             tex_node = tex.get_child(0)
-            tex_node.value = texture_mapper[eggparse.sanitize_string(tex_node.value)]
+            old_value = eggparse.sanitize_string(tex_node.value)
+            tex_node.value = texture_mapper.get(old_value, old_value)
 
         # We also need to remove the default cube and the cameras if they're present in the model
         nodeset = set()
         for node in eggtree.children:
             if isinstance(node, eggparse.EggBranch) and node.node_type == "Group":
                 if node.node_name == "Camera" or node.node_name.startswith("Cube."):
                     nodeset.add(node)
@@ -267,15 +282,15 @@
         f"*.png : force-rgba dual linear clamp_u clamp_v margin 5\n"
     )
     with open("textures.txa", "w") as txa_file:
         txa_file.write(txa_text)
 
     all_eggs = [file for file in ctx.files if file.endswith(".egg")]
 
-    logger.info("%s: Palettizing %s...", ctx.name, ', '.join(all_eggs))
+    logger.info("%s: Palettizing %s...", ctx.name, ", ".join(all_eggs))
     util.run_panda(
         ctx.putil_ctx,
         "egg-palettize",
         "-opt",
         "-redo",
         "-nodb",
         "-inplace",
@@ -334,35 +349,62 @@
         for group in tree.findall("Group"):
             if fnmatch.fnmatch(group.node_name, pattern):
                 removals.add(group)
 
         tree.remove_nodes(removals)
 
 
-def action_egg2bam(ctx):
+def action_egg2bam(ctx, all_textures=""):
+    all_textures = all_textures.lower() not in ("", "0", "false")
+
     files = []
     # if followed by palettize we wont have eggs here
     ctx.cache_eggs()
+
+    copied_files = set()
     for file, eggtree in ctx.eggs.items():
         logger.info("%s: Copying %s into the dist directory", ctx.name, file)
         files.append(file)
-
         operations.set_texture_prefix(eggtree, f"{ctx.output_phase}/maps")
         for tex in eggtree.findall("Texture"):
             filename = eggparse.sanitize_string(tex.get_child(0).value).split("/")[-1]
-            shutil.copy(filename, f"{ctx.output_texture}/{filename}")
+            copied_files.add(filename)
+
+    if all_textures:
+        copied_files.clear()
+        for filename in ctx.files:
+            if image_regex.match(filename):
+                copied_files.add(filename)
+
+    copied_files = {cf: ctx.path_overrides.get(cf) for cf in copied_files}
+    delete_paths = set()
+    delete_parents = set()
+    for filename, target_path in copied_files.items():
+        if target_path is None:
+            copy_path = pathlib.Path(ctx.output_texture, filename)
+        else:
+            copy_path = pathlib.Path(ctx.output_texture, target_path, filename)
+        copy_path.parent.mkdir(parents=True, exist_ok=True)
+        shutil.copy(filename, copy_path)
+        if filename in ctx.post_remove:
+            delete_paths.add(copy_path)
+            delete_parents.add(copy_path.parent)
 
     ctx.uncache_eggs()
     for file in ctx.files:
         if file.endswith(".egg"):
-            shutil.copy(file, f"{ctx.output_model}/{file}")
+            shutil.copy(file, pathlib.Path(ctx.output_model, file))
 
     os.chdir(ctx.output_model)
     os.chdir(ctx.putil_ctx.resources_path)
     ctx.putil_ctx.working_path = ctx.putil_ctx.resources_path
     for file in files:
         if file.endswith(".egg"):
             logger.info("%s: Converting %s to bam", ctx.name, file)
             egg2bam(ctx.putil_ctx, ctx.output_model_rel + "/" + file)
             os.unlink(f"{ctx.output_model}/{file}")
     os.chdir(ctx.cwd)
     ctx.putil_ctx.working_path = ctx.cwd
+    for dp in delete_paths:
+        os.unlink(dp)
+    for folder in delete_parents:
+        ctx.reverse_rmdir(folder)
```

### Comparing `panda_utils-1.4.0/panda_utils/assetpipeline/textures.py` & `panda_utils-1.4.1/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/blender/export_glb.py` & `panda_utils-1.4.1/panda_utils/blender/export_glb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 import bpy
 
 argv = sys.argv
-argv = argv[argv.index("--") + 1:]  # get all arguments after "--"
+argv = argv[argv.index("--") + 1 :]  # get all arguments after "--"
 
 output_file = argv[0]
 
 
 def update_texture_paths():
     for mat in bpy.data.materials:
         if mat.use_nodes:
```

### Comparing `panda_utils-1.4.0/panda_utils/blender/import_model.py` & `panda_utils-1.4.1/panda_utils/blender/import_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import bpy
 import sys
 
 argv = sys.argv
-argv = argv[argv.index("--") + 1:]  # get all arguments after "--"
+argv = argv[argv.index("--") + 1 :]  # get all arguments after "--"
 
 output_file, *input_files = argv
 
 
 def import_model():
-    bpy.ops.object.select_all(action='SELECT')
+    bpy.ops.object.select_all(action="SELECT")
     bpy.ops.object.delete(use_global=False)
     for file in input_files:
         if file.endswith("fbx"):
             bpy.ops.import_scene.fbx(filepath=file)
         elif file.endswith("obj"):
             bpy.ops.import_scene.obj(filepath=file)
```

### Comparing `panda_utils-1.4.0/panda_utils/eggtree/eggparse.py` & `panda_utils-1.4.1/panda_utils/eggtree/eggparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     def __init__(self, node_type, node_name, node_value):
         self.node_type = node_type
         self.node_name = (node_name or "").strip()
         self.node_value = node_value
 
     def equals(self, other):
         return (
-            isinstance(other, EggLeaf) and other.node_name == self.node_name and other.node_value == self.node_value
+            isinstance(other, EggLeaf)
+            and other.node_name == self.node_name
+            and other.node_value == self.node_value
             and other.node_type == self.node_type
         )
 
     def __repr__(self):
         if self.node_name:
             return f"<{self.node_type}> {self.node_name.strip()} {{ {self.node_value.strip()} }}"
         return f"<{self.node_type}> {{ {self.node_value.strip()} }}"
@@ -134,15 +136,15 @@
         return self.children[index]
 
     def add_child(self, child):
         self.children += child
 
 
 def sanitize_string(val):
-    if val and val[0] in '"\'':
+    if val and val[0] in "\"'":
         return val[1:-1]
     return val
 
 
 single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
 preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\" ]+ )?\{([^\n]*)")
```

### Comparing `panda_utils-1.4.0/panda_utils/eggtree/operations.py` & `panda_utils-1.4.1/panda_utils/eggtree/operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from panda_utils.eggtree import eggparse
 
 
 def set_texture_prefix(tree: eggparse.EggTree, new_prefix: str) -> None:
     textures = tree.findall("Texture")
     for texture in textures:
         texture_name = texture.get_child(0)
-        filename = eggparse.sanitize_string(texture_name.value).split("/")[-1]
+        og_filename = eggparse.sanitize_string(texture_name.value)
+        if og_filename.startswith(new_prefix) and "/.." not in og_filename:
+            continue
+        filename = og_filename.split("/")[-1]
         texture_name.value = f"{new_prefix}/{filename}"
 
 
 def add_comment(tree: eggparse.EggTree, comment: str) -> None:
     comment_str = eggparse.EggString(f'"{comment}"')
     comment_tree = eggparse.EggTree(comment_str)
     comment = eggparse.EggBranch("Comment", None, comment_tree)
```

### Comparing `panda_utils-1.4.0/panda_utils/tools/animconvert.py` & `panda_utils-1.4.1/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/tools/convert.py` & `panda_utils-1.4.1/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/tools/downscale.py` & `panda_utils-1.4.1/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/tools/palettize.py` & `panda_utils-1.4.1/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/tools/toontown.py` & `panda_utils-1.4.1/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils/util.py` & `panda_utils-1.4.1/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.0/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.4.1/panda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.4.0
+Version: 1.4.1
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.0/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.4.1/panda_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 panda_utils/assetpipeline/__main__.py
 panda_utils/assetpipeline/imports.py
 panda_utils/assetpipeline/misc.py
 panda_utils/assetpipeline/models.py
 panda_utils/assetpipeline/textures.py
 panda_utils/blender/__init__.py
 panda_utils/blender/export_glb.py
+panda_utils/blender/export_with_yabee.py
 panda_utils/blender/import_model.py
 panda_utils/blender/patch_paths.py
 panda_utils/eggtree/__init__.py
 panda_utils/eggtree/eggparse.py
 panda_utils/eggtree/operations.py
 panda_utils/tools/__init__.py
 panda_utils/tools/animconvert.py
```

### Comparing `panda_utils-1.4.0/pyproject.toml` & `panda_utils-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

