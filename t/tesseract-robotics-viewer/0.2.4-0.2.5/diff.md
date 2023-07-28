# Comparing `tmp/tesseract_robotics_viewer-0.2.4-py3-none-any.whl.zip` & `tmp/tesseract_robotics_viewer-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 51011 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       31 b- defN 23-May-04 20:12 tesseract_robotics_viewer/__init__.py
--rw-rw-rw-  2.0 fat    20857 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/tesseract_env_to_gltf.py
--rw-rw-rw-  2.0 fat    26418 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/tesseract_viewer.py
--rw-rw-rw-  2.0 fat    35051 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/tesseract_viewer_aio.py
--rw-rw-rw-  2.0 fat     2896 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/util.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-04 20:12 tesseract_robotics_viewer/resources/__init__.py
--rw-rw-rw-  2.0 fat   169227 b- defN 23-May-04 20:12 tesseract_robotics_viewer/resources/geometries.json
--rw-rw-rw-  2.0 fat    24768 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/resources/static/app.js
--rw-rw-rw-  2.0 fat      570 b- defN 23-Jul-04 04:24 tesseract_robotics_viewer/resources/static/index.html
--rw-rw-rw-  2.0 fat      382 b- defN 23-Jul-21 19:31 tesseract_robotics_viewer-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 19:31 tesseract_robotics_viewer-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Jul-21 19:31 tesseract_robotics_viewer-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1296 b- defN 23-Jul-21 19:31 tesseract_robotics_viewer-0.2.4.dist-info/RECORD
-13 files, 281614 bytes uncompressed, 48773 bytes compressed:  82.7%
+Zip file size: 51048 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       31 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/__init__.py
+-rw-rw-r--  2.0 unx    20857 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/tesseract_env_to_gltf.py
+-rw-rw-r--  2.0 unx    26418 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/tesseract_viewer.py
+-rw-rw-r--  2.0 unx    35051 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/tesseract_viewer_aio.py
+-rw-rw-r--  2.0 unx     2896 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/util.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/resources/__init__.py
+-rw-rw-r--  2.0 unx   169227 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/resources/geometries.json
+-rw-rw-r--  2.0 unx    24848 b- defN 23-Jul-28 01:14 tesseract_robotics_viewer/resources/static/app.js
+-rw-rw-r--  2.0 unx      570 b- defN 23-Jul-28 01:02 tesseract_robotics_viewer/resources/static/index.html
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jul-28 01:16 tesseract_robotics_viewer-0.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-28 01:16 tesseract_robotics_viewer-0.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-28 01:16 tesseract_robotics_viewer-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1296 b- defN 23-Jul-28 01:16 tesseract_robotics_viewer-0.2.5.dist-info/RECORD
+13 files, 281739 bytes uncompressed, 48810 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: tesseract_robotics_viewer/resources/static/app.js
 Comment: 
 
 Filename: tesseract_robotics_viewer/resources/static/index.html
 Comment: 
 
-Filename: tesseract_robotics_viewer-0.2.4.dist-info/METADATA
+Filename: tesseract_robotics_viewer-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: tesseract_robotics_viewer-0.2.4.dist-info/WHEEL
+Filename: tesseract_robotics_viewer-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: tesseract_robotics_viewer-0.2.4.dist-info/top_level.txt
+Filename: tesseract_robotics_viewer-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tesseract_robotics_viewer-0.2.4.dist-info/RECORD
+Filename: tesseract_robotics_viewer-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tesseract_robotics_viewer/resources/static/app.js

### js-beautify {}

```diff
@@ -83,16 +83,18 @@
         this._light = light;
 
         document.body.appendChild(renderer.domElement);
 
         const controls = new OrbitControls(camera, renderer.domElement);
 
         // Only add VR button if it is supported
-        if (await navigator.xr.isSessionSupported('immersive-vr')) {
-            document.body.appendChild(VRButton.createButton(renderer));
+        if ('xr' in navigator) {
+            if (await navigator.xr.isSessionSupported('immersive-vr')) {
+                document.body.appendChild(VRButton.createButton(renderer));
+            }
         }
 
         renderer.setAnimationLoop(this.render.bind(this));
 
         const gridHelper = new THREE.GridHelper(10, 10);
         this._scene.add(gridHelper);
```

## Comparing `tesseract_robotics_viewer-0.2.4.dist-info/RECORD` & `tesseract_robotics_viewer-0.2.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 tesseract_robotics_viewer/__init__.py,sha256=ZCWz1d0Ma8gq3EMd7zUtwuNiXuJOVXqY4vP8rc3TFvw,31
 tesseract_robotics_viewer/tesseract_env_to_gltf.py,sha256=6VZJANFD8g45o3G-baKYZGpbEll05p_larzAEvzrrAw,20857
 tesseract_robotics_viewer/tesseract_viewer.py,sha256=NRY9Gz_8aiy8ajplaEDU45oIMU-qNgarjzphwRB2nNk,26418
 tesseract_robotics_viewer/tesseract_viewer_aio.py,sha256=seV6w-MCt6jEiUfYNG3MRX7oo6JyvwarsmrExR1nu30,35051
 tesseract_robotics_viewer/util.py,sha256=R_jXHOONrnWhd9s0TFkvYIZvm9u29VI2eD72vHHfa8M,2896
 tesseract_robotics_viewer/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tesseract_robotics_viewer/resources/geometries.json,sha256=mA_R99zldqzsVwTehXrj6CM7_5-iG5Mr-5HgwwYm9mw,169227
-tesseract_robotics_viewer/resources/static/app.js,sha256=bnrF52tBe3LBi-8e721eQxtBOuDsUXoEIPbakv9Ieaw,24768
+tesseract_robotics_viewer/resources/static/app.js,sha256=Eweq9momtihcc0DK2PqvXePVC_6oygJgDJS7pBwjvFQ,24848
 tesseract_robotics_viewer/resources/static/index.html,sha256=w5tRucppnVa-AT_-AI5E8qJnKkrWce068tsC1Ep3S-8,570
-tesseract_robotics_viewer-0.2.4.dist-info/METADATA,sha256=zlSIgq8kdDd7OnIgESz9GVer1NHmdNxJCDAZeNmHj4w,382
-tesseract_robotics_viewer-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tesseract_robotics_viewer-0.2.4.dist-info/top_level.txt,sha256=ahiYXVyvmhLAkQF6dKuRxxRGBgeAA8RK02YvUcE0rB8,26
-tesseract_robotics_viewer-0.2.4.dist-info/RECORD,,
+tesseract_robotics_viewer-0.2.5.dist-info/METADATA,sha256=DYfRyJscUlDzId7AJqMhn5nlB2NcdfKWApE01Q3Zu_U,427
+tesseract_robotics_viewer-0.2.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+tesseract_robotics_viewer-0.2.5.dist-info/top_level.txt,sha256=ahiYXVyvmhLAkQF6dKuRxxRGBgeAA8RK02YvUcE0rB8,26
+tesseract_robotics_viewer-0.2.5.dist-info/RECORD,,
```

