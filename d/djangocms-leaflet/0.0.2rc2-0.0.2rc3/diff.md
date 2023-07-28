# Comparing `tmp/djangocms_leaflet-0.0.2rc2.tar.gz` & `tmp/djangocms_leaflet-0.0.2rc3.tar.gz`

## Comparing `djangocms_leaflet-0.0.2rc2.tar` & `djangocms_leaflet-0.0.2rc3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/package-lock.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/package.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/webpack.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/assets/src/leaflet.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/__init__.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/apps.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/cms_plugins.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/models.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0001_initial.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
--rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/LICENSE.txt
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/README.md
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc2/PKG-INFO
+-rw-r--r--   0        0        0    58673 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/package-lock.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/package.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/webpack.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/assets/src/leaflet.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/__init__.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/apps.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/cms_plugins.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/models.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/migrations/0001_initial.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/migrations/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-2x-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-2x-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-black.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-black.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-blue.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-blue.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-gold.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-gold.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-green.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-green.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-grey.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-grey.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-orange.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-orange.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-red.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-red.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-violet.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-violet.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-icon-yellow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-icon-yellow.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/leaflet-color-markers/marker-shadow.png -> /home/jens/develop/djangocms/phi/static/images/leaflet-color-markers/marker-shadow.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   169468 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png
+-rw-r--r--   0        0        0   174912 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/leaflet.bundle.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/leaflet.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/templates/djangocms_leaflet/map.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/templates/djangocms_leaflet/marker.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/LICENSE.txt
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/README.md
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/pyproject.toml
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 djangocms_leaflet-0.0.2rc3/PKG-INFO
```

### Comparing `djangocms_leaflet-0.0.2rc2/package-lock.json` & `djangocms_leaflet-0.0.2rc3/package-lock.json`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/cms_plugins.py` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/models.py` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0001_initial.py` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/migrations/0002_auto_20200310_2328.py`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/djangocms_leaflet/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/2b3e1faf89f94a483539.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/416d91365b44e4b4f477.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/8f2c4d11474275fbc161.png`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/static/webpack/leaflet.bundle.js` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/static/webpack/leaflet.bundle.js`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/src/djangocms_leaflet/templates/djangocms_leaflet/map.html` & `djangocms_leaflet-0.0.2rc3/src/djangocms_leaflet/templates/djangocms_leaflet/map.html`

 * *Files 16% similar despite different names*

```diff
@@ -22,83 +22,99 @@
 00000150: 7469 6320 2764 6a61 6e67 6f63 6d73 5f6c  tic 'djangocms_l
 00000160: 6561 666c 6574 2f77 6562 7061 636b 2f6c  eaflet/webpack/l
 00000170: 6561 666c 6574 2e62 756e 646c 652e 6a73  eaflet.bundle.js
 00000180: 2720 257d 223e 3c2f 7363 7269 7074 3e0a  ' %}"></script>.
 00000190: 7b25 2065 6e64 6164 6474 6f62 6c6f 636b  {% endaddtoblock
 000001a0: 2025 7d0a 0a7b 2520 6164 6474 6f62 6c6f   %}..{% addtoblo
 000001b0: 636b 2022 6a73 2220 7374 7269 7020 257d  ck "js" strip %}
-000001c0: 0a3c 7363 7269 7074 2064 6566 6572 3e0a  .<script defer>.
-000001d0: 7769 6e64 6f77 2e6f 6e6c 6f61 6420 3d20  window.onload = 
-000001e0: 6675 6e63 7469 6f6e 2829 207b 0a20 2020  function() {.   
-000001f0: 2063 6f6e 7374 206d 6170 203d 204c 2e6d   const map = L.m
-00000200: 6170 2827 6d61 702d 7b7b 2069 6e73 7461  ap('map-{{ insta
-00000210: 6e63 652e 6964 207d 7d27 292e 7365 7456  nce.id }}').setV
-00000220: 6965 7728 5b7b 7b20 696e 7374 616e 6365  iew([{{ instance
-00000230: 2e6c 6174 6974 7564 6520 7d7d 2c20 7b7b  .latitude }}, {{
-00000240: 2069 6e73 7461 6e63 652e 6c6f 6e67 6974   instance.longit
-00000250: 7564 6520 7d7d 5d2c 207b 7b20 696e 7374  ude }}], {{ inst
-00000260: 616e 6365 2e7a 6f6f 6d5f 6c65 7665 6c20  ance.zoom_level 
-00000270: 7d7d 293b 0a0a 2020 2020 4c2e 7469 6c65  }});..    L.tile
-00000280: 4c61 7965 7228 2768 7474 7073 3a2f 2f7b  Layer('https://{
-00000290: 737d 2e74 696c 652e 6f70 656e 7374 7265  s}.tile.openstre
-000002a0: 6574 6d61 702e 6f72 672f 7b7a 7d2f 7b78  etmap.org/{z}/{x
-000002b0: 7d2f 7b79 7d2e 706e 6727 2c20 7b0a 2020  }/{y}.png', {.  
-000002c0: 2020 2020 2020 6174 7472 6962 7574 696f        attributio
-000002d0: 6e3a 2027 2663 6f70 793b 203c 6120 6872  n: '&copy; <a hr
-000002e0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-000002f0: 6f70 656e 7374 7265 6574 6d61 702e 6f72  openstreetmap.or
-00000300: 672f 636f 7079 7269 6768 7422 3e4f 7065  g/copyright">Ope
-00000310: 6e53 7472 6565 744d 6170 3c2f 613e 2063  nStreetMap</a> c
-00000320: 6f6e 7472 6962 7574 6f72 7327 0a20 2020  ontributors'.   
-00000330: 207d 292e 6164 6454 6f28 6d61 7029 3b0a   }).addTo(map);.
-00000340: 0a20 2020 207b 2320 6874 7470 733a 2f2f  .    {# https://
-00000350: 7374 6163 6b6f 7665 7266 6c6f 772e 636f  stackoverflow.co
-00000360: 6d2f 7175 6573 7469 6f6e 732f 3634 3930  m/questions/6490
-00000370: 3231 3731 2f61 6e67 756c 6172 2d31 302d  2171/angular-10-
-00000380: 6c65 6166 6c65 742d 7765 6270 6163 6b2d  leaflet-webpack-
-00000390: 6272 6561 6b69 6e67 2d75 726c 2d74 6f2d  breaking-url-to-
-000003a0: 6d61 726b 6572 2d69 636f 6e2d 706e 6720  marker-icon-png 
-000003b0: 237d 0a20 2020 206c 6574 2044 6566 6175  #}.    let Defau
-000003c0: 6c74 4963 6f6e 203d 204c 2e69 636f 6e28  ltIcon = L.icon(
-000003d0: 7b0a 2020 2020 2020 2020 6963 6f6e 5572  {.        iconUr
-000003e0: 6c3a 2027 7b25 2020 7374 6174 6963 2022  l: '{%  static "
-000003f0: 646a 616e 676f 636d 735f 6c65 6166 6c65  djangocms_leafle
-00000400: 742f 696d 6167 6573 2f6c 6561 666c 6574  t/images/leaflet
-00000410: 2d63 6f6c 6f72 2d6d 6172 6b65 7273 2f6d  -color-markers/m
-00000420: 6172 6b65 722d 6963 6f6e 2d32 782d 626c  arker-icon-2x-bl
-00000430: 7565 2e70 6e67 2220 257d 272c 0a20 2020  ue.png" %}',.   
-00000440: 2020 2020 2073 6861 646f 7755 726c 3a20       shadowUrl: 
-00000450: 277b 2520 2073 7461 7469 6320 2264 6a61  '{%  static "dja
-00000460: 6e67 6f63 6d73 5f6c 6561 666c 6574 2f69  ngocms_leaflet/i
-00000470: 6d61 6765 732f 6c65 6166 6c65 742d 636f  mages/leaflet-co
-00000480: 6c6f 722d 6d61 726b 6572 732f 6d61 726b  lor-markers/mark
-00000490: 6572 2d73 6861 646f 772e 706e 6722 2025  er-shadow.png" %
-000004a0: 7d27 2c0a 2020 2020 2020 2020 6963 6f6e  }',.        icon
-000004b0: 5369 7a65 3a20 5b32 342c 2033 365d 2c0a  Size: [24, 36],.
-000004c0: 2020 2020 2020 2020 6963 6f6e 416e 6368          iconAnch
-000004d0: 6f72 3a20 5b31 322c 2033 365d 0a20 2020  or: [12, 36].   
-000004e0: 207d 293b 0a20 2020 204c 2e4d 6172 6b65   });.    L.Marke
-000004f0: 722e 7072 6f74 6f74 7970 652e 6f70 7469  r.prototype.opti
-00000500: 6f6e 732e 6963 6f6e 203d 2044 6566 6175  ons.icon = Defau
-00000510: 6c74 4963 6f6e 3b0a 0a20 2020 207b 2520  ltIcon;..    {% 
-00000520: 6966 2069 6e73 7461 6e63 652e 7365 745f  if instance.set_
-00000530: 6d61 726b 6572 2025 7d0a 2020 2020 2020  marker %}.      
-00000540: 2020 4c2e 6d61 726b 6572 285b 7b7b 2069    L.marker([{{ i
-00000550: 6e73 7461 6e63 652e 6c61 7469 7475 6465  nstance.latitude
-00000560: 207d 7d2c 207b 7b20 696e 7374 616e 6365   }}, {{ instance
-00000570: 2e6c 6f6e 6769 7475 6465 207d 7d5d 292e  .longitude }}]).
-00000580: 6164 6454 6f28 6d61 7029 0a20 2020 2020  addTo(map).     
-00000590: 2020 2020 2020 202e 6269 6e64 506f 7075         .bindPopu
-000005a0: 7028 277b 7b20 696e 7374 616e 6365 2e6e  p('{{ instance.n
-000005b0: 616d 6520 7d7d 2729 0a20 2020 2020 2020  ame }}').       
-000005c0: 2020 2020 202e 6f70 656e 506f 7075 7028       .openPopup(
-000005d0: 293b 0a20 2020 207b 2520 656e 6469 6620  );.    {% endif 
-000005e0: 257d 0a7d 0a3c 2f73 6372 6970 743e 0a7b  %}.}.</script>.{
-000005f0: 2520 656e 6461 6464 746f 626c 6f63 6b20  % endaddtoblock 
-00000600: 257d 0a0a 7b25 2066 6f72 2070 6c75 6769  %}..{% for plugi
-00000610: 6e20 696e 2069 6e73 7461 6e63 652e 6368  n in instance.ch
-00000620: 696c 645f 706c 7567 696e 5f69 6e73 7461  ild_plugin_insta
-00000630: 6e63 6573 2025 7d0a 7b25 2072 656e 6465  nces %}.{% rende
-00000640: 725f 706c 7567 696e 2070 6c75 6769 6e20  r_plugin plugin 
-00000650: 257d 0a7b 2520 656e 6466 6f72 2025 7d0a  %}.{% endfor %}.
-00000660: 7b25 2065 6e64 6c6f 6361 6c69 7a65 2025  {% endlocalize %
-00000670: 7d                                       }
+000001c0: 0a3c 7363 7269 7074 3e0a 7b23 2052 6570  .<script>.{# Rep
+000001d0: 6c61 6365 6d65 6e74 2066 6f72 206a 7175  lacement for jqu
+000001e0: 6572 79e2 8099 7320 2428 6675 6e63 7469  ery...s $(functi
+000001f0: 6f6e 2829 207b 7d29 2023 7d0a 7b23 2068  on() {}) #}.{# h
+00000200: 7474 7073 3a2f 2f73 7461 636b 6f76 6572  ttps://stackover
+00000210: 666c 6f77 2e63 6f6d 2f71 7565 7374 696f  flow.com/questio
+00000220: 6e73 2f37 3939 3938 312f 646f 6375 6d65  ns/799981/docume
+00000230: 6e74 2d72 6561 6479 2d65 7175 6976 616c  nt-ready-equival
+00000240: 656e 742d 7769 7468 6f75 742d 6a71 7565  ent-without-jque
+00000250: 7279 2023 7d0a 6675 6e63 7469 6f6e 2072  ry #}.function r
+00000260: 6561 6479 2866 6e29 207b 0a20 2069 6620  eady(fn) {.  if 
+00000270: 2864 6f63 756d 656e 742e 7265 6164 7953  (document.readyS
+00000280: 7461 7465 2021 3d3d 2027 6c6f 6164 696e  tate !== 'loadin
+00000290: 6727 2920 7b0a 2020 2020 666e 2829 3b0a  g') {.    fn();.
+000002a0: 2020 2020 7265 7475 726e 3b0a 2020 7d0a      return;.  }.
+000002b0: 2020 646f 6375 6d65 6e74 2e61 6464 4576    document.addEv
+000002c0: 656e 744c 6973 7465 6e65 7228 2744 4f4d  entListener('DOM
+000002d0: 436f 6e74 656e 744c 6f61 6465 6427 2c20  ContentLoaded', 
+000002e0: 666e 293b 0a7d 0a72 6561 6479 2866 756e  fn);.}.ready(fun
+000002f0: 6374 696f 6e28 2920 7b0a 2020 2020 6d61  ction() {.    ma
+00000300: 7020 3d20 4c2e 6d61 7028 276d 6170 2d7b  p = L.map('map-{
+00000310: 7b20 696e 7374 616e 6365 2e69 6420 7d7d  { instance.id }}
+00000320: 2729 2e73 6574 5669 6577 285b 7b7b 2069  ').setView([{{ i
+00000330: 6e73 7461 6e63 652e 6c61 7469 7475 6465  nstance.latitude
+00000340: 207d 7d2c 207b 7b20 696e 7374 616e 6365   }}, {{ instance
+00000350: 2e6c 6f6e 6769 7475 6465 207d 7d5d 2c20  .longitude }}], 
+00000360: 7b7b 2069 6e73 7461 6e63 652e 7a6f 6f6d  {{ instance.zoom
+00000370: 5f6c 6576 656c 207d 7d29 3b0a 0a20 2020  _level }});..   
+00000380: 204c 2e74 696c 654c 6179 6572 2827 6874   L.tileLayer('ht
+00000390: 7470 733a 2f2f 7b73 7d2e 7469 6c65 2e6f  tps://{s}.tile.o
+000003a0: 7065 6e73 7472 6565 746d 6170 2e6f 7267  penstreetmap.org
+000003b0: 2f7b 7a7d 2f7b 787d 2f7b 797d 2e70 6e67  /{z}/{x}/{y}.png
+000003c0: 272c 207b 0a20 2020 2020 2020 2061 7474  ', {.        att
+000003d0: 7269 6275 7469 6f6e 3a20 2726 636f 7079  ribution: '&copy
+000003e0: 3b20 3c61 2068 7265 663d 2268 7474 7073  ; <a href="https
+000003f0: 3a2f 2f77 7777 2e6f 7065 6e73 7472 6565  ://www.openstree
+00000400: 746d 6170 2e6f 7267 2f63 6f70 7972 6967  tmap.org/copyrig
+00000410: 6874 223e 4f70 656e 5374 7265 6574 4d61  ht">OpenStreetMa
+00000420: 703c 2f61 3e20 636f 6e74 7269 6275 746f  p</a> contributo
+00000430: 7273 270a 2020 2020 7d29 2e61 6464 546f  rs'.    }).addTo
+00000440: 286d 6170 293b 0a0a 2020 2020 7b23 2068  (map);..    {# h
+00000450: 7474 7073 3a2f 2f73 7461 636b 6f76 6572  ttps://stackover
+00000460: 666c 6f77 2e63 6f6d 2f71 7565 7374 696f  flow.com/questio
+00000470: 6e73 2f36 3439 3032 3137 312f 616e 6775  ns/64902171/angu
+00000480: 6c61 722d 3130 2d6c 6561 666c 6574 2d77  lar-10-leaflet-w
+00000490: 6562 7061 636b 2d62 7265 616b 696e 672d  ebpack-breaking-
+000004a0: 7572 6c2d 746f 2d6d 6172 6b65 722d 6963  url-to-marker-ic
+000004b0: 6f6e 2d70 6e67 2023 7d0a 2020 2020 6c65  on-png #}.    le
+000004c0: 7420 4465 6661 756c 7449 636f 6e20 3d20  t DefaultIcon = 
+000004d0: 4c2e 6963 6f6e 287b 0a20 2020 2020 2020  L.icon({.       
+000004e0: 2069 636f 6e55 726c 3a20 277b 2520 2073   iconUrl: '{%  s
+000004f0: 7461 7469 6320 2264 6a61 6e67 6f63 6d73  tatic "djangocms
+00000500: 5f6c 6561 666c 6574 2f69 6d61 6765 732f  _leaflet/images/
+00000510: 6c65 6166 6c65 742d 636f 6c6f 722d 6d61  leaflet-color-ma
+00000520: 726b 6572 732f 6d61 726b 6572 2d69 636f  rkers/marker-ico
+00000530: 6e2d 3278 2d62 6c75 652e 706e 6722 2025  n-2x-blue.png" %
+00000540: 7d27 2c0a 2020 2020 2020 2020 7368 6164  }',.        shad
+00000550: 6f77 5572 6c3a 2027 7b25 2020 7374 6174  owUrl: '{%  stat
+00000560: 6963 2022 646a 616e 676f 636d 735f 6c65  ic "djangocms_le
+00000570: 6166 6c65 742f 696d 6167 6573 2f6c 6561  aflet/images/lea
+00000580: 666c 6574 2d63 6f6c 6f72 2d6d 6172 6b65  flet-color-marke
+00000590: 7273 2f6d 6172 6b65 722d 7368 6164 6f77  rs/marker-shadow
+000005a0: 2e70 6e67 2220 257d 272c 0a20 2020 2020  .png" %}',.     
+000005b0: 2020 2069 636f 6e53 697a 653a 205b 3234     iconSize: [24
+000005c0: 2c20 3336 5d2c 0a20 2020 2020 2020 2069  , 36],.        i
+000005d0: 636f 6e41 6e63 686f 723a 205b 3132 2c20  conAnchor: [12, 
+000005e0: 3336 5d0a 2020 2020 7d29 3b0a 2020 2020  36].    });.    
+000005f0: 4c2e 4d61 726b 6572 2e70 726f 746f 7479  L.Marker.prototy
+00000600: 7065 2e6f 7074 696f 6e73 2e69 636f 6e20  pe.options.icon 
+00000610: 3d20 4465 6661 756c 7449 636f 6e3b 0a0a  = DefaultIcon;..
+00000620: 2020 2020 7b25 2069 6620 696e 7374 616e      {% if instan
+00000630: 6365 2e73 6574 5f6d 6172 6b65 7220 257d  ce.set_marker %}
+00000640: 0a20 2020 2020 2020 204c 2e6d 6172 6b65  .        L.marke
+00000650: 7228 5b7b 7b20 696e 7374 616e 6365 2e6c  r([{{ instance.l
+00000660: 6174 6974 7564 6520 7d7d 2c20 7b7b 2069  atitude }}, {{ i
+00000670: 6e73 7461 6e63 652e 6c6f 6e67 6974 7564  nstance.longitud
+00000680: 6520 7d7d 5d29 2e61 6464 546f 286d 6170  e }}]).addTo(map
+00000690: 290a 2020 2020 2020 2020 2020 2020 2e62  ).            .b
+000006a0: 696e 6450 6f70 7570 2827 7b7b 2069 6e73  indPopup('{{ ins
+000006b0: 7461 6e63 652e 6e61 6d65 207d 7d27 290a  tance.name }}').
+000006c0: 2020 2020 2020 2020 2020 2020 2e6f 7065              .ope
+000006d0: 6e50 6f70 7570 2829 3b0a 2020 2020 7b25  nPopup();.    {%
+000006e0: 2065 6e64 6966 2025 7d0a 7d29 0a3c 2f73   endif %}.}).</s
+000006f0: 6372 6970 743e 0a7b 2520 656e 6461 6464  cript>.{% endadd
+00000700: 746f 626c 6f63 6b20 257d 0a0a 7b25 2066  toblock %}..{% f
+00000710: 6f72 2070 6c75 6769 6e20 696e 2069 6e73  or plugin in ins
+00000720: 7461 6e63 652e 6368 696c 645f 706c 7567  tance.child_plug
+00000730: 696e 5f69 6e73 7461 6e63 6573 2025 7d0a  in_instances %}.
+00000740: 7b25 2072 656e 6465 725f 706c 7567 696e  {% render_plugin
+00000750: 2070 6c75 6769 6e20 257d 0a7b 2520 656e   plugin %}.{% en
+00000760: 6466 6f72 2025 7d0a 7b25 2065 6e64 6c6f  dfor %}.{% endlo
+00000770: 6361 6c69 7a65 2025 7d                   calize %}
```

### Comparing `djangocms_leaflet-0.0.2rc2/LICENSE.txt` & `djangocms_leaflet-0.0.2rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_leaflet-0.0.2rc2/README.md` & `djangocms_leaflet-0.0.2rc3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install djangocms-leaflet
 ```
+## Usage
+
+Add a map plugin to a placeholder and fill in the form. Add markers as sub plugins if needed.
+In the template `src/djangocms_leaflet/templates/djangocms_leaflet/map.html` the tile server
+of the OpenStreetMap website is defined. Make sure you comply with their usage policy or
+use another tile server by replacing the tile server’s URL.
 
 ## License
 
 `djangocms-leaflet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Integrated library
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangocms_leaflet-0.0.2rc2/PKG-INFO` & `djangocms_leaflet-0.0.2rc3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-leaflet
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: django CMS plug-ins for the JavaScript map library Leaflet
 Project-URL: Documentation, https://github.com/MacLake/djangocms-leaflet#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-leaflet/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-leaflet
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -36,14 +36,20 @@
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install djangocms-leaflet
 ```
+## Usage
+
+Add a map plugin to a placeholder and fill in the form. Add markers as sub plugins if needed.
+In the template `src/djangocms_leaflet/templates/djangocms_leaflet/map.html` the tile server
+of the OpenStreetMap website is defined. Make sure you comply with their usage policy or
+use another tile server by replacing the tile server’s URL.
 
 ## License
 
 `djangocms-leaflet` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Integrated library
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

