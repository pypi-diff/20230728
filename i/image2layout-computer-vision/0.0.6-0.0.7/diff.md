# Comparing `tmp/image2layout_computer_vision-0.0.6.tar.gz` & `tmp/image2layout_computer_vision-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.0.6.tar", last modified: Wed Jul 26 09:05:31 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.0.7.tar", last modified: Fri Jul 28 02:29:51 2023, max compression
```

## Comparing `image2layout_computer_vision-0.0.6.tar` & `image2layout_computer_vision-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.110434 image2layout_computer_vision-0.0.6/
--rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/LICENSE
--rw-r--r--   0 felixdo    (501) staff       (20)     2331 2023-07-26 09:05:31.110218 image2layout_computer_vision-0.0.6/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)     1761 2023-07-26 09:02:55.000000 image2layout_computer_vision-0.0.6/README.md
--rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-26 09:04:05.000000 image2layout_computer_vision-0.0.6/pyproject.toml
--rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-26 09:05:31.110492 image2layout_computer_vision-0.0.6/setup.cfg
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.105716 image2layout_computer_vision-0.0.6/src/
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.106193 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/
--rw-r--r--   0 felixdo    (501) staff       (20)      364 2023-07-26 08:56:55.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/__init__.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.107503 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/
--rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     8717 2023-07-26 08:59:02.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/main.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.108847 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/
--rw-r--r--   0 felixdo    (501) staff       (20)      143 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)    13036 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/imagebox.py
--rw-r--r--   0 felixdo    (501) staff       (20)     2310 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/main.py
--rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.109890 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/
--rw-r--r--   0 felixdo    (501) staff       (20)      172 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/color_system.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/imaging.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/pixel_mask.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-26 09:05:31.107025 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/
--rw-r--r--   0 felixdo    (501) staff       (20)     2331 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)      851 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-r--r--   0 felixdo    (501) staff       (20)       42 2023-07-26 09:05:31.000000 image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-26 08:41:36.000000 image2layout_computer_vision-0.0.6/src/sandbox.py
--rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.6/src/test.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.653675 image2layout_computer_vision-0.0.7/
+-rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.7/LICENSE
+-rw-r--r--   0 felixdo    (501) staff       (20)     2690 2023-07-28 02:29:51.653519 image2layout_computer_vision-0.0.7/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)     2120 2023-07-28 02:28:07.000000 image2layout_computer_vision-0.0.7/README.md
+-rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-27 11:41:21.000000 image2layout_computer_vision-0.0.7/pyproject.toml
+-rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-28 02:29:51.653724 image2layout_computer_vision-0.0.7/setup.cfg
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.648703 image2layout_computer_vision-0.0.7/src/
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.649129 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/
+-rw-r--r--   0 felixdo    (501) staff       (20)      416 2023-07-27 04:43:37.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/__init__.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.650398 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/color_extract/
+-rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     8721 2023-07-27 10:41:52.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/color_extract/main.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.651612 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/
+-rw-r--r--   0 felixdo    (501) staff       (20)      212 2023-07-27 04:43:44.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)    14054 2023-07-27 11:33:06.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     2679 2023-07-28 02:27:47.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/main.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.653111 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/
+-rw-r--r--   0 felixdo    (501) staff       (20)      227 2023-07-27 11:28:42.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     2221 2023-07-27 11:32:07.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/annotation.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/color_system.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/imaging.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/pixel_mask.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 02:29:51.649936 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/
+-rw-r--r--   0 felixdo    (501) staff       (20)     2690 2023-07-28 02:29:51.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)      923 2023-07-28 02:29:51.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-28 02:29:51.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)       54 2023-07-28 02:29:51.000000 image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-27 10:41:57.000000 image2layout_computer_vision-0.0.7/src/sandbox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     8862 2023-07-27 11:39:27.000000 image2layout_computer_vision-0.0.7/src/sandbox_ocr.py
+-rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.7/src/test.py
```

### Comparing `image2layout_computer_vision-0.0.6/LICENSE` & `image2layout_computer_vision-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/PKG-INFO` & `image2layout_computer_vision-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.0.6
+Version: 0.0.7
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,20 +67,36 @@
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -v $(pwd):/app cv bash
 ```
 
 ## Usage
 
-> Python
+1. Run this python code to pre-download model weights
+
+```python
+from image2layout_computer_vision import model_dispatch_layout
+model_dispatch_layout._load()
+```
+
+2. Detect texts
+
 ```python
 import image2layout_computer_vision as icv
 
+# ImageBoxes object
 imageboxes = icv.detect_text('path/to/image.png')
-boxes = icv.detect_text_boxes('path/to/image.png')
+
+# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
+boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
+```
+
+3. Extract colors
+```python
+import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
 ```
 
 
 
 ## Build
```

### Comparing `image2layout_computer_vision-0.0.6/README.md` & `image2layout_computer_vision-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,20 +53,36 @@
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -v $(pwd):/app cv bash
 ```
 
 ## Usage
 
-> Python
+1. Run this python code to pre-download model weights
+
+```python
+from image2layout_computer_vision import model_dispatch_layout
+model_dispatch_layout._load()
+```
+
+2. Detect texts
+
 ```python
 import image2layout_computer_vision as icv
 
+# ImageBoxes object
 imageboxes = icv.detect_text('path/to/image.png')
-boxes = icv.detect_text_boxes('path/to/image.png')
+
+# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
+boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
+```
+
+3. Extract colors
+```python
+import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
 ```
 
 
 
 ## Build
```

### Comparing `image2layout_computer_vision-0.0.6/pyproject.toml` & `image2layout_computer_vision-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/color_extract/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,17 @@
             n_clusters_max=n_clusters_max,
             n_clusters_min=n_clusters_min,
             with_foreground=with_foreground,
             force_run_all=False,
             **kwargs,
         )
         self.extract_map = self.extracted_data['extract_map']
-        self.color_bg = self.extracted_data['color_bg']
-        self.color_fg = self.extracted_data['color_fg']
-        self.colors = np.array([self.color_bg, self.color_fg])
+        self.color_bg = tuple(self.extracted_data['color_bg'])
+        self.color_fg = tuple(self.extracted_data['color_fg'])
+        self.colors = [self.color_bg, self.color_fg]
     
     def __repr__(self) -> str:
         return f'ColorExtractor[{self.shape}]({self.color_bg} | {self.color_fg})'
     
     def draw_anno(self,):
         img_anno_np = np.zeros([*self.shape, 4], np.uint8)
         img_anno_np[self.extract_map == 0] = [*self.color_bg, 255]
```

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # %%
 import os
 import json
 import colorsys
 import numpy as np
 import pandas as pd
 from PIL import Image, ImageDraw, ImageFont
-from ..utils import get_image
+from ..utils import get_image, draw_anno_box
+from typing import Union, Dict, Tuple, List, Any
 
 # %%
 class BoxMerge:
     
     @classmethod
     def same_column_match(cls,
                 boxa, boxb,
@@ -87,28 +88,28 @@
                 break
             
             start_index = min(remaining_indices)
             
             head_index = start_index
             linked_indices = [head_index]
             
-            for next_index in range(head_index, count):
+            for next_index in range(head_index+1, count):
                 if next_index in matched_indices:
                     continue
                 if fn(sorted_boxes[head_index], sorted_boxes[next_index], **kwargs):
                     linked_indices.append(next_index)
                     head_index = next_index
             
             linked_groups.append(linked_indices)
             matched_indices.update(linked_indices)
             remaining_indices.difference_update(linked_indices)
         
         data_group = []
         for i, indices in enumerate(linked_groups):
-            original_indices = sorted_indices_reverse[indices]
+            original_indices = sorted_indices[indices]
             group_box = cls.merge_boxes(sorted_boxes[indices])
             data_group.append({
                 'indices': original_indices,
                 'box': group_box,
             })
         
         df_group = pd.DataFrame(data_group)
@@ -194,33 +195,36 @@
             self.size = self.image.size
         else:
             assert size is not None
             self.size = size
         self.level = int(level)
         self.children_levels = -1
         self.box = None
-        self.boxes = []    # all child-most boxes
+        self.boxes = []        # all child-most boxes
+        self.boxes_top = []    # top-level (1 level in) boxes
         self.box_outer = None
         
         if self.is_single_instance:
             self.children_levels = 0
             self.box = np.array(boxes, int)
             self.box_outer = np.array(self.box, int)
             self.boxes.append(boxes)
+            self.boxes_top.append(boxes)
             super().__init__([])
         else:
             imageboxes = []
             for i, box in enumerate(boxes):
                 child_imageboxes = ImageBoxes(
                     boxes=box,
                     size=self.size,
                     level=self.level + 1,
                 )
                 imageboxes.append(child_imageboxes)
                 self.boxes.extend(child_imageboxes.boxes)
+                self.boxes_top.append(child_imageboxes.box_outer.tolist())
                 
                 if self.box_outer is None:
                     self.box_outer = np.array(child_imageboxes.box_outer, int)
                 else:
                     # print(self.box_outer, child_imageboxes.box_outer)
                     self.box_outer[:2] = np.min([self.box_outer[:2], child_imageboxes.box_outer[:2]], axis=0)
                     self.box_outer[2:] = np.max([self.box_outer[2:], child_imageboxes.box_outer[2:]], axis=0)
@@ -268,112 +272,149 @@
                 'text': child.text,
                 'box': child.box,
             }
             for child in self
         ]
         return pd.DataFrame(data)
     
-    def draw_anno(self, width=2, mode='box', draw_image=True, draw_level_0=False, img_base=None):
+    def draw_anno(self,
+                width=2,
+                mode='box',
+                draw_image=True,
+                draw_level_0=False,
+                img_base=None,
+                draw_size=True,
+                color=None,
+                ):
         assert mode in ['box', 'mask', 'all']
         
-        img_anno = Image.new('RGBA', self.size) if img_base is None else img_base
+        overlay_anno_bottom = draw_anno_box(
+            self.size,
+            boxes=self.boxes,
+            color='#00FF00',
+            color_text='#000000',
+        )
         
-        if mode in ['mask', 'all']:
-            self.boxes
-            img_anno
-            
-            img_mask_inner = Image.new('L', self.size, 255)
-            img_mask_full = Image.new('RGBA', self.size, (*self.mask_color, int(self.mask_opacity*255)))
-            
-            draw = ImageDraw.Draw(img_mask_inner)
-            for box in self.boxes:
-                draw.rectangle(
-                    tuple(box),
-                    fill=0,
-                    width=0,
-                )
-            
-            img_anno.paste(img_mask_full, (0, 0), img_mask_inner)
+        overlay_anno_top = draw_anno_box(
+            self.size,
+            boxes=self.boxes_top,
+            color='#FF00FF',
+            color_text='#000000',
+        )
+        overlay_anno = Image.alpha_composite(
+            overlay_anno_bottom,
+            overlay_anno_top,
+        )
+        img_anno = Image.alpha_composite(
+            self.image.convert('RGBA'),
+            overlay_anno,
+        ).convert('RGB')
         
-        if mode in ['box', 'all']:
-            color = self.box_colors[self.level % len(self.box_colors)]
-            
-            if width is None:
-                width = max(int(min(self.size) // 400), 1)
-            
-            if not self.is_single_instance:
-                for child in self:
-                    child_img = child.draw_anno(
-                        width=width,
-                        draw_image=False,
-                        mode='box',
-                    )
-                    img_anno.paste(child_img, (0, 0), child_img)
-            
-            if self.level > 0 or draw_level_0:
-                draw = ImageDraw.Draw(img_anno)
-                draw.rectangle(
-                    tuple(self.box),
-                    outline=color,
-                    width=width,
-                )
+        return img_anno
+    
+    def to_grouped_imageboxes(self, **kwargs):
+        '''group boxes with `grouped_boxes` from self and return an ImageBoxes with grouped boxes
+        '''
         
-        if draw_image and self.image is not None:
-            return Image.alpha_composite(
-                self.image.convert('RGBA'),
-                img_anno,
-            )
+        boxes_nested_final = self.group_boxes(self.boxes, **kwargs)
         
-        return img_anno
+        imageboxes_nested = ImageBoxes(
+            boxes=boxes_nested_final,
+            image=self.image.copy(),
+        )
+        return imageboxes_nested
     
-    def to_grouped_imageboxes(self,
-                line_dist_max=1.0,
-                line_dist_min=-0.1,
-                line_iou_min=0.4,
-                row_hdist_max=0.4,
-                row_vdist_max=1.8,
-                row_height_ratio_min=0.8,
-                ):
+    @classmethod
+    def group_boxes(cls,
+                boxes:Union[np.ndarray, list],
+                line_dist_max:float=1.0,
+                line_dist_min:float=-0.1,
+                line_iou_min:float=0.4,
+                row_hdist_max:float=0.4,
+                row_vdist_max:float=1.8,
+                row_height_ratio_min:float=0.8,
+                ) -> list:
         '''processes self.boxes and returns a new ImageBoxes object with grouped boxes
         Parameters:
+            boxes
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
             line_dist_min:          min (negative) distance between boxes to be in the same sentence (as a ratio of line height)
             line_iou_min:           min vertical iou between boxes to be on the same line
             row_hdist_max:          max horizontal offset between rows to aligned as a column (as a ratio of line height)
             row_vdist_max:          max vertical distance between rows to be in the same column (as a ratio of line height)
             row_height_ratio_min:   min ratio between heights of rows to be in the same column
+        Returns:
+            boxes_nested_final (list): nested boxes
         '''
         
         # TODO: implement to keep texts, currently discard all given texts
         # TODO: implement nested boxes
         
-        _boxes = np.array(self.boxes)
-        df_group = BoxMerge.group_texts_by_match_fn(
+        _boxes = np.array(boxes)
+        assert _boxes.ndim == 2
+        assert _boxes.shape[-1] == 4
+        
+        df_group_0 = BoxMerge.group_texts_by_match_fn(
             _boxes,
             fn=BoxMerge.same_line_match,
             sort_index=0,
             dist_max=line_dist_max,
             dist_min=line_dist_min,
             iou_min=line_iou_min,
         )
-        _boxes = np.array(list(df_group['box']))
-        df_group = BoxMerge.group_texts_by_match_fn(
-            _boxes,
+        df_group_1 = BoxMerge.group_texts_by_match_fn(
+            np.array(list(df_group_0['box'])),
             fn=BoxMerge.same_column_match,
             sort_index=1,
             hdist_max=row_hdist_max,
             vdist_max=row_vdist_max,
             height_ratio_min=row_height_ratio_min,
         )
-        _boxes = np.array(list(df_group['box']))
-        df_group = BoxMerge.group_texts_by_match_fn(
-            _boxes,
+        df_group_2 = BoxMerge.group_texts_by_match_fn(
+            np.array(list(df_group_1['box'])),
             fn=BoxMerge.box_containing_match,
         )
-        self.df_group = df_group
+        _boxes_out = np.array(df_group_2['box'].to_list(), int)
         
-        return ImageBoxes(
-            image=self.image.copy(),
-            boxes=np.array(df_group['box'].to_list(), int).tolist(),
-        )
+        indices_original = cls.get_original_nested_indices([
+            df_group_0,
+            df_group_1,
+            df_group_2,
+        ])
+        indices_original
+        
+        boxes_nested_final = [
+            [
+                _boxes[i].tolist()
+                for i in _indices
+            ]
+            for _indices in indices_original
+        ]
+        return boxes_nested_final
     
+    @classmethod
+    def get_original_nested_indices(cls, df_groups: list) -> list:
+        indices_nested = [
+            [
+                v.tolist()
+                for v in _df['indices']
+            ]
+            for _df in df_groups
+        ]
+        
+        indices_original = None
+        for i, _indices in enumerate(indices_nested):
+            if i == 0:
+                indices_original = [list(v) for v in _indices]
+            else:
+                indices_original = [
+                    [
+                        v
+                        for prev_index in prev_indices
+                        for v in indices_original[prev_index]
+                    ]
+                    for prev_indices in _indices
+                ]
+        
+        return indices_original
+
 # %%
```

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # %%
 import time
 import json
 import os
 import numpy as np
 import pandas as pd
+from PIL import Image
+from typing import Union, Any, List, Dict, Tuple
 from .model_layoutmlv2 import ModelDispatch_LayoutMLv2
 from ..utils import get_image, ImageConvert
 from .imagebox import ImageBoxes, BoxMerge
 
 # %%
 model_dispatch_layout = ModelDispatch_LayoutMLv2(
     device='cpu',
 )
 
 # %%
-def detect_text(image, **kwargs) -> ImageBoxes:
+def detect_text(image: Union[Image.Image, np.ndarray], **kwargs) -> ImageBoxes:
     '''predict boxes for text in the image
     Parameters:
-        image: (PIL.Image.Image, bytes, np.ndarray) RGB image
+        image: (PIL.Image.Image, np.ndarray) RGB image
         **kwargs:
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
             line_dist_min:          min (negative) distance between boxes to be in the same sentence (as a ratio of line height)
             line_iou_min:           min vertical iou between boxes to be on the same line
             row_hdist_max:          max horizontal offset between rows to aligned as a column (as a ratio of line height)
             row_vdist_max:          max vertical distance between rows to be in the same column (as a ratio of line height)
             row_height_ratio_min:   min ratio between heights of rows to be in the same column
@@ -31,30 +33,34 @@
     _image = get_image(image).convert('RGB')
     
     true_predictions, true_boxes = model_dispatch_layout(_image)
     true_boxes_np = np.array(true_boxes, int)
     true_boxes_check = np.all(true_boxes_np[:, 2:] > true_boxes_np[:, :2], axis=-1)
     true_boxes_np = true_boxes_np[true_boxes_check]
     
-    imageboxes_individual = ImageBoxes(
+    imageboxes_raw = ImageBoxes(
         image=_image,
         boxes=true_boxes_np.tolist(),
     )
-    imageboxes = imageboxes_individual.to_grouped_imageboxes(**kwargs)
+    imageboxes = imageboxes_raw.to_grouped_imageboxes(**kwargs)
     return imageboxes
 
-def detect_text_boxes(image, **kwargs) -> np.ndarray:
+def detect_text_boxes(image: Union[Image.Image, np.ndarray], **kwargs) -> Tuple[np.ndarray, np.ndarray]:
     '''predict boxes for text in the image
     Parameters: (same as detect_text)
     Returns:
-        boxes: (np.ndarray) [N, 4] text boxes detected
+        boxes_merged: (np.ndarray) [M, 4] text boxes detected, merged boxes
+        boxes_raw:    (np.ndarray) [N, 4] text boxes detected, all individual boxes (N >= M)
     '''
     imageboxes = detect_text(image, **kwargs)
     boxes = np.array(list(imageboxes.df['box'])).astype(int)
-    return boxes
     
+    boxes_merged = np.array(imageboxes.boxes_top, int)
+    boxes_raw = np.array(imageboxes.boxes, int)
+    return boxes_merged, boxes_raw
+
 # %%
 if __name__ == '__main__':
     imageboxes = detect_text('data/inputs/SCR-20230710-ixfw.jpeg')
     imageboxes.draw_anno(width=3)
     imageboxes.df
     boxes = np.array(list(imageboxes.df['box'])).astype(int)
```

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.0.6
+Version: 0.0.7
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,20 +67,36 @@
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -v $(pwd):/app cv bash
 ```
 
 ## Usage
 
-> Python
+1. Run this python code to pre-download model weights
+
+```python
+from image2layout_computer_vision import model_dispatch_layout
+model_dispatch_layout._load()
+```
+
+2. Detect texts
+
 ```python
 import image2layout_computer_vision as icv
 
+# ImageBoxes object
 imageboxes = icv.detect_text('path/to/image.png')
-boxes = icv.detect_text_boxes('path/to/image.png')
+
+# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
+boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
+```
+
+3. Extract colors
+```python
+import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
 ```
 
 
 
 ## Build
```

### Comparing `image2layout_computer_vision-0.0.6/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.0.7/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 src/sandbox.py
+src/sandbox_ocr.py
 src/test.py
 src/image2layout_computer_vision/__init__.py
 src/image2layout_computer_vision.egg-info/PKG-INFO
 src/image2layout_computer_vision.egg-info/SOURCES.txt
 src/image2layout_computer_vision.egg-info/dependency_links.txt
 src/image2layout_computer_vision.egg-info/top_level.txt
 src/image2layout_computer_vision/color_extract/__init__.py
 src/image2layout_computer_vision/color_extract/main.py
 src/image2layout_computer_vision/ocr/__init__.py
 src/image2layout_computer_vision/ocr/imagebox.py
 src/image2layout_computer_vision/ocr/main.py
 src/image2layout_computer_vision/ocr/model_layoutmlv2.py
 src/image2layout_computer_vision/utils/__init__.py
+src/image2layout_computer_vision/utils/annotation.py
 src/image2layout_computer_vision/utils/color_system.py
 src/image2layout_computer_vision/utils/imaging.py
 src/image2layout_computer_vision/utils/pixel_mask.py
```

### Comparing `image2layout_computer_vision-0.0.6/src/sandbox.py` & `image2layout_computer_vision-0.0.7/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.6/src/test.py` & `image2layout_computer_vision-0.0.7/src/test.py`

 * *Files identical despite different names*

