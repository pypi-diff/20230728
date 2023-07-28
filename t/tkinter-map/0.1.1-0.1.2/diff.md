# Comparing `tmp/tkinter-map-0.1.1.tar.gz` & `tmp/tkinter-map-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter-map-0.1.1.tar", last modified: Sat Jul 22 10:38:14 2023, max compression
+gzip compressed data, was "tkinter-map-0.1.2.tar", last modified: Fri Jul 28 18:18:55 2023, max compression
```

## Comparing `tkinter-map-0.1.1.tar` & `tkinter-map-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.719296 tkinter-map-0.1.1/
--rw-rw-rw-   0        0        0     1077 2023-07-16 08:51:05.000000 tkinter-map-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       69 2023-07-19 20:18:55.000000 tkinter-map-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2477 2023-07-22 10:38:14.718309 tkinter-map-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2023-07-20 17:10:37.000000 tkinter-map-0.1.1/README.md
--rw-rw-rw-   0        0        0        5 2023-07-16 05:22:19.000000 tkinter-map-0.1.1/VERSION
--rw-rw-rw-   0        0        0       42 2023-07-22 10:38:14.720292 tkinter-map-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-07-15 18:16:09.000000 tkinter-map-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.592548 tkinter-map-0.1.1/tkinter_map.egg-info/
--rw-rw-rw-   0        0        0     2477 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-22 10:38:13.000000 tkinter-map-0.1.1/tkinter_map.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.635495 tkinter-map-0.1.1/tkmap/
-drwxrwxrwx   0        0        0        0 2023-07-22 10:38:14.714308 tkinter-map-0.1.1/tkmap/.json/
--rw-rw-rw-   0        0        0      378 2023-07-19 19:23:52.000000 tkinter-map-0.1.1/tkmap/.json/google-map.json
--rw-rw-rw-   0        0        0      384 2023-07-19 19:25:10.000000 tkinter-map-0.1.1/tkmap/.json/google-satellite.json
--rw-rw-rw-   0        0        0      254 2023-07-20 16:52:14.000000 tkinter-map-0.1.1/tkmap/.json/mapbox-satellite-2x.json
--rw-rw-rw-   0        0        0      208 2023-07-20 16:52:09.000000 tkinter-map-0.1.1/tkmap/.json/mapbox-satellite.json
--rw-rw-rw-   0        0        0      261 2023-07-19 19:15:15.000000 tkinter-map-0.1.1/tkmap/.json/openstreetmap.json
--rw-rw-rw-   0        0        0     1029 2023-07-20 17:45:17.000000 tkinter-map-0.1.1/tkmap/__init__.py
--rw-rw-rw-   0        0        0     6690 2023-07-22 09:44:24.000000 tkinter-map-0.1.1/tkmap/bio.py
--rw-rw-rw-   0        0        0     2293 2023-07-21 17:13:04.000000 tkinter-map-0.1.1/tkmap/model.py
--rw-rw-rw-   0        0        0    18662 2023-07-22 10:33:44.000000 tkinter-map-0.1.1/tkmap/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:18:55.144343 tkinter-map-0.1.2/
+-rw-rw-rw-   0        0        0     1077 2023-07-16 08:51:05.000000 tkinter-map-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-07-19 20:18:55.000000 tkinter-map-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2517 2023-07-28 18:18:55.142354 tkinter-map-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-07-28 18:15:56.000000 tkinter-map-0.1.2/README.md
+-rw-rw-rw-   0        0        0        5 2023-07-23 07:21:54.000000 tkinter-map-0.1.2/VERSION
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:18:55.144343 tkinter-map-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-07-28 18:10:05.000000 tkinter-map-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:18:54.902990 tkinter-map-0.1.2/tkinter_map.egg-info/
+-rw-rw-rw-   0        0        0     2517 2023-07-28 18:18:54.000000 tkinter-map-0.1.2/tkinter_map.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-07-28 18:18:54.000000 tkinter-map-0.1.2/tkinter_map.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:18:54.000000 tkinter-map-0.1.2/tkinter_map.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 18:18:54.000000 tkinter-map-0.1.2/tkinter_map.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 18:18:54.955858 tkinter-map-0.1.2/tkmap/
+drwxrwxrwx   0        0        0        0 2023-07-28 18:18:55.133373 tkinter-map-0.1.2/tkmap/.json/
+-rw-rw-rw-   0        0        0      378 2023-07-19 19:23:52.000000 tkinter-map-0.1.2/tkmap/.json/google-map.json
+-rw-rw-rw-   0        0        0      384 2023-07-19 19:25:10.000000 tkinter-map-0.1.2/tkmap/.json/google-satellite.json
+-rw-rw-rw-   0        0        0      254 2023-07-20 16:52:14.000000 tkinter-map-0.1.2/tkmap/.json/mapbox-satellite-2x.json
+-rw-rw-rw-   0        0        0      208 2023-07-20 16:52:09.000000 tkinter-map-0.1.2/tkmap/.json/mapbox-satellite.json
+-rw-rw-rw-   0        0        0      261 2023-07-19 19:15:15.000000 tkinter-map-0.1.2/tkmap/.json/openstreetmap.json
+-rw-rw-rw-   0        0        0     1029 2023-07-20 17:45:17.000000 tkinter-map-0.1.2/tkmap/__init__.py
+-rw-rw-rw-   0        0        0     6688 2023-07-27 15:29:31.000000 tkinter-map-0.1.2/tkmap/bio.py
+-rw-rw-rw-   0        0        0     2293 2023-07-21 17:13:04.000000 tkinter-map-0.1.2/tkmap/model.py
+-rw-rw-rw-   0        0        0    19722 2023-07-23 09:30:25.000000 tkinter-map-0.1.2/tkmap/widget.py
```

### Comparing `tkinter-map-0.1.1/LICENSE` & `tkinter-map-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter-map-0.1.1/README.md` & `tkinter-map-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Tkmap widget
 
 **Efficient web map canvas for tkinter.**
 
+[![pypi](https://img.shields.io/pypi/l/tkinter-map.svg)](https://github.com/Moustikitos/tkinter-map/blob/master/LICENSE)
+
+## Support this project
+
+[![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate)
+[![Paypal me](https://img.shields.io/badge/PayPal-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
+
 ## Install
 
 ### Version 0.1
 
 ```bash
 python -m pip install tkinter-map
 ```
@@ -29,15 +36,15 @@
 ```python
 >>> from tkmap import widget, model
 >>> canvas = widget.Tkmap()
 >>> canvas.pack(fill="both", expand=True)
 >>> canvas.open(model.OpenStreetMap(), zoom=10, location=(48.645272, 1.841411))
 ```
 
-![Tkmap widget](./docs/widget.png)
+![Tkmap widget](https://raw.githubusercontent.com/Moustikitos/tkinter-map/master/img/widget.png)
 
 ## Features
 
 - [x] Tile set:
   - [x] Google map
   - [x] Google satellite
   - [x] Open Street map
```

### Comparing `tkinter-map-0.1.1/setup.py` & `tkinter-map-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "download_url":
         "https://github.com/Moustikitos/tkinter-map/archive/master.zip",
     "description": "Efficient web map tkinter canvas",
     "long_description": LONG_DESCRIPTION,
     "long_description_content_type": "text/markdown",
     "packages": ["tkmap"],
     "install_requires": [],
-    "license": "Cpyright 2023 THOORENS Bruno",
+    "license": "Copyright 2023, THOORENS Bruno, MIT licence",
     "classifiers": [
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
```

### Comparing `tkinter-map-0.1.1/tkmap/__init__.py` & `tkinter-map-0.1.2/tkmap/__init__.py`

 * *Files identical despite different names*

### Comparing `tkinter-map-0.1.1/tkmap/bio.py` & `tkinter-map-0.1.2/tkmap/bio.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         Args:
             zoom (int): tile set zoom level.
             row (int): tile set row.
             col (int): tile set column.
 
         Returns:
-            str | bool: base64-encoded data if any tile found else `False`
+            str|bool: base64-encoded data if any tile found else `False`
         """
 
         req = self.sqlite.execute(
             "SELECT data FROM tiles WHERE zoom=? AND row=? AND col=?;",
             (zoom, row, col)
         ).fetchall()
         if len(req):
```

### Comparing `tkinter-map-0.1.1/tkmap/model.py` & `tkinter-map-0.1.2/tkmap/model.py`

 * *Files identical despite different names*

### Comparing `tkinter-map-0.1.1/tkmap/widget.py` & `tkinter-map-0.1.2/tkmap/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,41 @@
         """
         Delete the image item from canvas and image data from tcl interpreter.
         """
         logging.info(f" -> {__class__.__name__} {self._imgtk} cleared")
         Tile.tkeval(self._clear)
 
 
+def _xscroll(a, b, widget):
+    a, b = float(a), float(b)
+    if a > 0. or b < 1.0:
+        tkinter._default_root.eval(
+            f"place configure {widget} -height 2 -rely 1.0 "
+            f"-relx {a} -relwidth {max(0.01, b - a)} -anchor sw"
+        )
+    else:
+        tkinter._default_root.eval(f"place forget {widget}")
+
+
+def _yscroll(a, b, widget):
+    a, b = float(a), float(b)
+    if a > 0. or b < 1.0:
+        tkinter._default_root.eval(
+            f"place configure {widget} -width 2 -relx 1.0 "
+            f"-rely {a} -relheight {max(0.01, b - a)} -anchor ne"
+        )
+    else:
+        tkinter._default_root.eval(f"place forget {widget}")
+
+
 # inertia computation @ 100Hz & k = 0.9
 def _drift(obj: tkinter.Canvas, speed_x: float, speed_y: float) -> None:
     t = time.time()
     dt = t - obj._tps[1]
-    dx = speed_x * dt
-    dy = speed_y * dt
+    dx, dy = speed_x * dt, speed_y * dt
     obj._tps[1] = t
     if obj._tps[0] is None and (dx*dx + dy*dy) > 1:
         obj.tk.eval(
             f"{obj._w} xview scroll {int(round(dx))} units;"
             f"{obj._w} yview scroll {int(round(dy))} units"
         )
         obj._after_tasks.append(
@@ -169,32 +190,40 @@
             compute map coordinates.
         workers (List[bio.TileWorker]): List of python thread used to perform
             tile downloads or database queries.
     """
 
     @property
     def bbox(obj) -> tuple:
-        "Returns east, north, west and south boundaries view on canvas area."
+        "Returns west, north, east and south boundaries view on canvas area."
         return [
             int(float(e)) for e in obj.tk.eval(
                 f"list [{obj._w} canvasx 0] [{obj._w} canvasy 0]"
                 f" [{obj._w} canvasx [expr [winfo width {obj._w}]]]"
                 f" [{obj._w} canvasy [expr [winfo height {obj._w}]]]"
             ).split()
         ]
 
     def __init__(self, master=None, cnf={}, **kw) -> None:
         self.framerate = kw.pop("framerate", 4)
         self.cachesize = kw.pop("cachesize", 500)
 
         tkinter.Canvas.__init__(self, master, cnf, **kw)
+        # scrollincrement needs to be set to pixel size for correct drift
+        # effect
         self["xscrollincrement"] = self["yscrollincrement"] = 1
+        self["xscrollcommand"] = \
+            lambda a, b, f=tkinter.Frame(self, bg="systemHighlight")._w: \
+            _xscroll(a, b, f)
+        self["yscrollcommand"] = \
+            lambda a, b, f=tkinter.Frame(self, bg="systemHighlight")._w: \
+            _yscroll(a, b, f)
 
         self.coords = ttk.Label(
-            relief="solid", padding=(5, 1),
+            self, relief="solid", padding=(5, 1),
             font=("calibri", "8"), textvariable="coords"
         )
         self._coords_place = dict(y=-4, rely=1.0, relx=0.5, anchor="s")
 
         load_img_package(self.tk)
 
         self.JOB = queue.LifoQueue()
@@ -359,23 +388,23 @@
             worker = self.workers.pop(0)
             worker.kill()
 
     def _update_drawarea(self) -> None:
         tw, th = self.mapmodel.tilesize
         nr, nc = self.mapsize
         bd = self.borderwidth
-        e, n, w, s = self.bbox
+        w, n, e, s = self.bbox
         self.drawarea = (
-            max(0, e//tw-bd), max(0, n//th-bd),
-            min(nr, w//tw+bd), min(nc, s//th+bd)
+            max(0, w//tw-bd), max(0, n//th-bd),
+            min(nr, e//tw+bd), min(nc, s//th+bd)
         )
 
     def _update(self) -> None:
         c1, r1, c2, r2 = self.drawarea
-        e, n, w, s = self.bbox
+        w, n, e, s = self.bbox
         cmd = self.tk.eval
         r = self.radius
         _w = self._w
 
         tags_to_show = set(
             functools.reduce(
                 list.__add__,
@@ -390,15 +419,15 @@
         for tag in tags_to_show - cached_tiles:
             if tag not in self.QUEUED.queue:
                 self.QUEUED.put(tag)
                 self.JOB.put([tag, self.mapmodel])
 
         all_tiles = cmd(f"{_w} find overlapping {self['scrollregion']}")
         tile_to_show = \
-            cmd(f"{_w} find overlapping {e - r} {n - r} {w + r} {s + r}")
+            cmd(f"{_w} find overlapping {w - r} {n - r} {e + r} {s + r}")
         tile_to_hide = set(all_tiles.split()) - set(tile_to_show.split())
         standing_by_tiles = tags_to_show & cached_tiles
 
         try:
             cmd(
                 "foreach id {" + " ".join(tile_to_hide) + "} "
                 "{" + _w + " itemconfig $id -state hidden};"
```

