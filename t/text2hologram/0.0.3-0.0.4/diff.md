# Comparing `tmp/text2hologram-0.0.3.tar.gz` & `tmp/text2hologram-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2hologram-0.0.3.tar", last modified: Wed Jul 26 19:15:31 2023, max compression
+gzip compressed data, was "text2hologram-0.0.4.tar", last modified: Fri Jul 28 21:13:19 2023, max compression
```

## Comparing `text2hologram-0.0.3.tar` & `text2hologram-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.715929 text2hologram-0.0.3/
--rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      698 2023-07-26 19:15:31.714245 text2hologram-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.3/README.md
--rw-rw-rw-   0        0        0      826 2023-07-26 19:15:20.000000 text2hologram-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 19:15:31.715929 text2hologram-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.686898 text2hologram-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.703726 text2hologram-0.0.3/src/text2hologram/
--rw-rw-rw-   0        0        0     1525 2023-07-26 18:50:40.000000 text2hologram-0.0.3/src/text2hologram/__main__.py
--rw-rw-rw-   0        0        0      964 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/config.json
--rw-rw-rw-   0        0        0      338 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/device_setup.py
--rw-rw-rw-   0        0        0      910 2023-07-26 18:51:12.000000 text2hologram-0.0.3/src/text2hologram/image_generation.py
--rw-rw-rw-   0        0        0      703 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/model.py
--rw-rw-rw-   0        0        0     7070 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/post_processing.py
--rw-rw-rw-   0        0        0      663 2023-07-26 18:55:16.000000 text2hologram-0.0.3/src/text2hologram/settings.py
--rw-rw-rw-   0        0        0      340 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.713245 text2hologram-0.0.3/src/text2hologram.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.222856 text2hologram-0.0.4/
+-rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      698 2023-07-28 21:13:19.221855 text2hologram-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.4/README.md
+-rw-rw-rw-   0        0        0      826 2023-07-28 21:12:55.000000 text2hologram-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 21:13:19.222856 text2hologram-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.195856 text2hologram-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.211856 text2hologram-0.0.4/src/text2hologram/
+-rw-rw-rw-   0        0        0     2473 2023-07-28 21:11:19.000000 text2hologram-0.0.4/src/text2hologram/__main__.py
+-rw-rw-rw-   0        0        0      964 2023-07-28 18:01:04.000000 text2hologram-0.0.4/src/text2hologram/config.json
+-rw-rw-rw-   0        0        0      487 2023-07-28 17:36:58.000000 text2hologram-0.0.4/src/text2hologram/device_setup.py
+-rw-rw-rw-   0        0        0      920 2023-07-28 21:11:30.000000 text2hologram-0.0.4/src/text2hologram/image_generation.py
+-rw-rw-rw-   0        0        0     2191 2023-07-28 17:51:12.000000 text2hologram-0.0.4/src/text2hologram/model.py
+-rw-rw-rw-   0        0        0     7070 2023-07-26 18:37:12.000000 text2hologram-0.0.4/src/text2hologram/post_processing.py
+-rw-rw-rw-   0        0        0      454 2023-07-28 17:26:17.000000 text2hologram-0.0.4/src/text2hologram/read_all.py
+-rw-rw-rw-   0        0        0      711 2023-07-28 17:42:08.000000 text2hologram-0.0.4/src/text2hologram/settings.py
+-rw-rw-rw-   0        0        0      340 2023-07-26 18:37:12.000000 text2hologram-0.0.4/src/text2hologram/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.219858 text2hologram-0.0.4/src/text2hologram.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/top_level.txt
```

### Comparing `text2hologram-0.0.3/PKG-INFO` & `text2hologram-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text2hologram-0.0.3/pyproject.toml` & `text2hologram-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2hologram"
-version = "0.0.3"
+version = "0.0.4"
 description = "Generate holograms from text"
 readme = "README.md"
 authors = [{ name = "Pengze Li", email = "linsonng@163.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `text2hologram-0.0.3/src/text2hologram/__main__.py` & `text2hologram-0.0.4/src/text2hologram/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,59 @@
 from text2hologram.device_setup import setup_device
 from text2hologram.model import load_model
 from text2hologram.image_generation import generate_images
 from text2hologram.post_processing import process_depth_map, cgh
 import argparse
 import numpy as np
 
+# This function loads the default settings from the `config.json` file,
+# defines and parses the command line arguments, and updates the settings
+# based on the command line arguments.
 def parse_arguments():
-    # Load default settings from config.json
+    # Load default settings from `config.json`
     settings = load_settings()
+    
     # Define command line arguments
     parser = argparse.ArgumentParser(description='Process some integers.')
+    parser.add_argument('--device', default=settings['general']['device'], help='Device')
     parser.add_argument('--iterations', type=int, default=settings['general']['iterations'], help='Number of iterations')
     parser.add_argument('--inference_steps', type=int, default=settings['diffusion']['inference_steps'], help='Number of Stable Diffusion inference steps')
     parser.add_argument('--outputdir', default=settings['general']['output directory'], help='Output directory')
+    
     # Parse command line arguments
     args = parser.parse_args()
+    
+    # Update settings based on the parsed command line arguments
     settings = update_settings(settings, args)
+    
     return settings
 
+# The main function. It parses the command line arguments,
+# sets up the device, loads the model and necessary transforms, generates images,
+# processes the depth map, performs CGH, and waits for the user to press Enter to exit.
 def main():
+    # Parse command line arguments and load updated settings
     settings = parse_arguments()
+    
+    # Set up the device
     device = setup_device(settings)
+    
+    # Load the model and necessary transforms
     midas, pipe, transform = load_model(device)
+    
+    # Get user input for the sentence to base the image creation on
     prompt = input("Enter a sentence, which the image is going to be created based on : ")
-    image_name, images = generate_images(pipe, prompt, settings)
+    
+    # Generate images
+    image_name, images = generate_images(pipe, prompt, settings, device)
+    
+    # Process the depth map
     process_depth_map(midas, transform, np.array(images[0]), device, settings)
+    
+    # Perform CGH
     cgh(settings, image_name)
+    
+    # Wait for the user to press Enter to exit
     input("Press Enter to exit...")
 
 if __name__ == "__main__":
     main()
```

### Comparing `text2hologram-0.0.3/src/text2hologram/config.json` & `text2hologram-0.0.4/src/text2hologram/config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'diffusion'": "{'inference_steps': 30}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "beam": {
         "wavelength": 5.15e-07
     },
     "diffusion": {
-        "inference_steps": 64
+        "inference_steps": 30
     },
     "general": {
         "device": "cuda",
         "hologram number": 1,
         "iterations": 60,
         "learning rate": 0.04,
         "output directory": "CGH_output/",
```

### Comparing `text2hologram-0.0.3/src/text2hologram/image_generation.py` & `text2hologram-0.0.4/src/text2hologram/image_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import torch
 import random
 from text2hologram.utils import create_dirs
 from PIL import Image
 
-def generate_images(pipe, prompt, settings):
+def generate_images(pipe, prompt, settings, device):
     seed = random.randint(0, 2147483647)
     negative_prompt = "nude, naked"
     print("Creating images.")
     images = pipe(
         prompt,
         height = settings['slm']['resolution'][0],
         width = settings['slm']['resolution'][1],
         num_inference_steps = settings['diffusion']['inference_steps'],
         guidance_scale = 9,
         num_images_per_prompt = 1,
         negative_prompt = negative_prompt,
-        generator = torch.Generator("cuda").manual_seed(seed)
+        generator = torch.Generator(device).manual_seed(seed)
         ).images
     create_dirs([settings['general']['output directory']])
     image_name = settings['general']['output directory'] + "/"+ prompt[0:20] + ".jpg"
     images[0].save(image_name)
     print("Image saved as "+ image_name)
     return image_name, images
+
```

### Comparing `text2hologram-0.0.3/src/text2hologram/post_processing.py` & `text2hologram-0.0.4/src/text2hologram/post_processing.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.3/src/text2hologram/settings.py` & `text2hologram-0.0.4/src/text2hologram/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,9 @@
         settings = json.load(f)
     return settings
 
 def update_settings(settings, args):
     settings['general']['iterations'] = args.iterations
     settings['diffusion']['inference_steps'] = args.inference_steps
     settings['general']['output directory'] = args.outputdir
+    settings['general']['device'] = args.device
     return settings
```

### Comparing `text2hologram-0.0.3/src/text2hologram.egg-info/PKG-INFO` & `text2hologram-0.0.4/src/text2hologram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text2hologram-0.0.3/src/text2hologram.egg-info/SOURCES.txt` & `text2hologram-0.0.4/src/text2hologram.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 src/text2hologram/__main__.py
 src/text2hologram/config.json
 src/text2hologram/device_setup.py
 src/text2hologram/image_generation.py
 src/text2hologram/model.py
 src/text2hologram/post_processing.py
+src/text2hologram/read_all.py
 src/text2hologram/settings.py
 src/text2hologram/utils.py
 src/text2hologram.egg-info/PKG-INFO
 src/text2hologram.egg-info/SOURCES.txt
 src/text2hologram.egg-info/dependency_links.txt
 src/text2hologram.egg-info/entry_points.txt
 src/text2hologram.egg-info/requires.txt
```

