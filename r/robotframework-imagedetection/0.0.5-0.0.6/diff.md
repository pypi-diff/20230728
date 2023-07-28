# Comparing `tmp/robotframework-imagedetection-0.0.5.tar.gz` & `tmp/robotframework-imagedetection-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-imagedetection-0.0.5.tar", last modified: Thu Jul 27 06:33:26 2023, max compression
+gzip compressed data, was "robotframework-imagedetection-0.0.6.tar", last modified: Fri Jul 28 11:38:24 2023, max compression
```

## Comparing `robotframework-imagedetection-0.0.5.tar` & `robotframework-imagedetection-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 06:33:26.771209 robotframework-imagedetection-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-27 06:33:26.706792 robotframework-imagedetection-0.0.5/Imagedetection/
--rw-rw-rw-   0        0        0     6207 2023-07-27 06:31:23.000000 robotframework-imagedetection-0.0.5/Imagedetection/Base_detection.py
--rw-rw-rw-   0        0        0      369 2023-07-27 06:29:27.000000 robotframework-imagedetection-0.0.5/Imagedetection/Imagedetection.py
--rw-rw-rw-   0        0        0       44 2023-07-27 06:29:27.000000 robotframework-imagedetection-0.0.5/Imagedetection/__init__.py
--rw-rw-rw-   0        0        0    11558 2023-07-27 06:29:27.000000 robotframework-imagedetection-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1294 2023-07-27 06:33:26.769196 robotframework-imagedetection-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-07-27 06:29:27.000000 robotframework-imagedetection-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 06:33:26.765633 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/
--rw-rw-rw-   0        0        0     1294 2023-07-27 06:33:26.000000 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-27 06:33:26.000000 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 06:33:26.000000 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      782 2023-07-27 06:33:26.000000 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 06:33:26.000000 robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 06:33:26.772198 robotframework-imagedetection-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1893 2023-07-27 06:29:27.000000 robotframework-imagedetection-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:38:24.677118 robotframework-imagedetection-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-28 11:38:24.651872 robotframework-imagedetection-0.0.6/Imagedetection/
+-rw-rw-rw-   0        0        0     5415 2023-07-28 11:37:17.000000 robotframework-imagedetection-0.0.6/Imagedetection/Base_detection.py
+-rw-rw-rw-   0        0        0     4622 2023-07-28 11:37:17.000000 robotframework-imagedetection-0.0.6/Imagedetection/Imagedetection.py
+-rw-rw-rw-   0        0        0       44 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.6/Imagedetection/__init__.py
+-rw-rw-rw-   0        0        0    11558 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     9229 2023-07-28 11:38:24.676112 robotframework-imagedetection-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7981 2023-07-28 11:37:17.000000 robotframework-imagedetection-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 11:38:24.669434 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/
+-rw-rw-rw-   0        0        0     9229 2023-07-28 11:38:24.000000 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-28 11:38:24.000000 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:38:24.000000 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      797 2023-07-28 11:38:24.000000 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-28 11:38:24.000000 robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:38:24.678109 robotframework-imagedetection-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1893 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.6/setup.py
```

### Comparing `robotframework-imagedetection-0.0.5/Imagedetection/Base_detection.py` & `robotframework-imagedetection-0.0.6/Imagedetection/Base_detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import cv2
 import numpy as np
 import tensorflow as tf
-from robot.api import logger
 from keras.models import load_model
 from keras.preprocessing import image
 from keras.preprocessing.image import ImageDataGenerator
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 class Base_Detect:
 
     def __init__(self):
         self.epoch = 20
 
     def train_model(self,training_path, validation_path):
@@ -65,38 +64,31 @@
                 folder_path = os.path.join(path,folder)
                 if os.path.isdir(folder_path):
                     subfolders.append(folder)
             return subfolders
         except FileNotFoundError as e:
             print(e)
 
-    def capture_and_predict(self,model_name):
+    def capture_and_predict(self,model_name,save_path):
         # Take a photos from a camera
 
         camera = cv2.VideoCapture(0)
         if not camera.isOpened():
             print("Error: camera not accessible.")
             return None
         
         _, frame = camera.read()
 
         # Provide the desired save path for the captured photo
-        save_path = "captured_photo2.jpg"
         cv2.imwrite(save_path, frame)
         camera.release()
 
         self._predict(model_name,save_path)
             
-        curdir = os.getcwd()
-        current_directory_with_double_backslashes = curdir.replace("\\", "\\\\")
-
-        Log_photo = fr"<img src={current_directory_with_double_backslashes}\\{save_path} width='150' height='100'>"
-        logger.info(Log_photo,html=True,also_console=False)
-
-
+        
     def _predict(self,model_name, photo_path):
         model = load_model(model_name)
         # Load the testing image
         
         img = image.load_img(photo_path, target_size=(200, 200))
         X = image.img_to_array(img)
         X = np.expand_dims(X, axis=0)
@@ -104,23 +96,15 @@
         prediction_probs = model.predict(X)[0]
         
         class_labels = self._get_subfolders("Data/training/")
         
         predicted_class = class_labels[np.argmax(prediction_probs)]
         print("Predicted class:", predicted_class)
         #print("Predicted probs:", prediction_probs)
-
-
-    def predict_from_path(self,model_name, photo_path):
-        # You need to train a model first to use this function. 
         
-        self._predict(model_name,photo_path)
-
-        Log_photo = f'<img src="{photo_path}" width="150" height="100">'
-        logger.info(Log_photo,html=True,also_console=False)
 
     def predict_from_google_model(self,_model,_image):
         from PIL import Image, ImageOps  
         
         # Disable scientific notation for clarity
         np.set_printoptions(suppress=True)
 
@@ -153,13 +137,10 @@
 
         # Predicts the model
         prediction = model.predict(data)
         index = np.argmax(prediction)
         class_name = class_names[index]
         confidence_score = prediction[0][index]
 
-        Log_photo = f'<img src="{_image}" width="150" height="100">'
-        logger.info(Log_photo,html=True,also_console=False)
-
         # Print prediction and confidence score
         print("Class:", class_name[2:], end="")
         print("Confidence Score:", confidence_score)
```

### Comparing `robotframework-imagedetection-0.0.5/LICENSE` & `robotframework-imagedetection-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-imagedetection-0.0.5/robotframework_imagedetection.egg-info/requires.txt` & `robotframework-imagedetection-0.0.6/robotframework_imagedetection.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 tensorflow-intel==2.13.0
 tensorflow-io-gcs-filesystem==0.31.0
 termcolor==2.3.0
 typing_extensions==4.5.0
 urllib3==1.26.16
 Werkzeug==2.3.6
 wrapt==1.15.0
+robotframework
```

### Comparing `robotframework-imagedetection-0.0.5/setup.py` & `robotframework-imagedetection-0.0.6/setup.py`

 * *Files identical despite different names*

