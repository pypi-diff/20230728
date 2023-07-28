# Comparing `tmp/chromahacker-0.2.5.tar.gz` & `tmp/chromahacker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.2.5.tar", max compression
+gzip compressed data, was "chromahacker-0.3.0.tar", max compression
```

## Comparing `chromahacker-0.2.5.tar` & `chromahacker-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.2.5/README.md
--rw-r--r--   0        0        0     6148 2023-07-21 18:41:22.475897 chromahacker-0.2.5/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.2.5/chromahacker/__init__.py
--rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.2.5/chromahacker/color_input.py
--rw-r--r--   0        0        0      572 2023-07-21 22:32:55.660377 chromahacker-0.2.5/chromahacker/palettize.py
--rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.2.5/chromahacker/process_image.py
--rw-r--r--   0        0        0      469 2023-07-21 17:43:15.983637 chromahacker-0.2.5/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-07-21 22:33:11.518517 chromahacker-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.3.0/README.md
+-rw-r--r--   0        0        0     6148 2023-07-21 18:41:22.475897 chromahacker-0.3.0/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.3.0/chromahacker/__init__.py
+-rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.3.0/chromahacker/color_input.py
+-rw-r--r--   0        0        0      669 2023-07-28 01:39:26.539405 chromahacker-0.3.0/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.3.0/chromahacker/process_image.py
+-rw-r--r--   0        0        0      469 2023-07-21 17:43:15.983637 chromahacker-0.3.0/chromahacker/spline.py
+-rw-r--r--   0        0        0      337 2023-07-28 01:41:42.672092 chromahacker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.3.0/PKG-INFO
```

### Comparing `chromahacker-0.2.5/chromahacker/.DS_Store` & `chromahacker-0.3.0/chromahacker/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahacker-0.2.5/chromahacker/color_input.py` & `chromahacker-0.3.0/chromahacker/color_input.py`

 * *Files identical despite different names*

### Comparing `chromahacker-0.2.5/chromahacker/palettize.py` & `chromahacker-0.3.0/chromahacker/palettize.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,8 +14,13 @@
 
     fn = spline_from(*args, accurate=accurate)
 
     if accurate:
         display = np.array([[fn(j) for j in i] for i in img])
     else:
         display = np.rint(fn(img)).astype(np.uint8)
-    cv2.imwrite(os.getcwd() + '/wallpaper.' + output, display)
+
+    img_encode = cv2.imencode('.' + output, display)[1]
+
+    data_encode = np.array(img_encode)
+    byte_encode = data_encode.tobytes()
+    return byte_encode
```

