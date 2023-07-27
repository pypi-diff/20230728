# Comparing `tmp/tmxpy-0.1.4.tar.gz` & `tmp/tmxpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmxpy-0.1.4.tar", last modified: Tue Jul 25 23:32:19 2023, max compression
+gzip compressed data, was "tmxpy-0.1.5.tar", last modified: Thu Jul 27 23:40:40 2023, max compression
```

## Comparing `tmxpy-0.1.4.tar` & `tmxpy-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.466991 tmxpy-0.1.4/
--rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1387 2023-07-25 23:32:19.465990 tmxpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-07-18 17:45:31.000000 tmxpy-0.1.4/README.md
--rw-rw-rw-   0        0        0      719 2023-07-25 12:46:37.000000 tmxpy-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 23:32:19.466991 tmxpy-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.443978 tmxpy-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.453979 tmxpy-0.1.4/src/tmxpy/
--rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.4/src/tmxpy/__init__.py
--rw-rw-rw-   0        0        0     7744 2023-07-25 23:19:24.000000 tmxpy-0.1.4/src/tmxpy/tmxpy.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.463989 tmxpy-0.1.4/src/tmxpy.egg-info/
--rw-rw-rw-   0        0        0     1387 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.805318 tmxpy-0.1.5/
+-rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1890 2023-07-27 23:40:40.804317 tmxpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2023-07-27 23:39:59.000000 tmxpy-0.1.5/README.md
+-rw-rw-rw-   0        0        0      719 2023-07-27 21:23:19.000000 tmxpy-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 23:40:40.805318 tmxpy-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.781296 tmxpy-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.792307 tmxpy-0.1.5/src/tmxpy/
+-rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.5/src/tmxpy/__init__.py
+-rw-rw-rw-   0        0        0    10158 2023-07-27 23:32:33.000000 tmxpy-0.1.5/src/tmxpy/tmxpy.py
+drwxrwxrwx   0        0        0        0 2023-07-27 23:40:40.802316 tmxpy-0.1.5/src/tmxpy.egg-info/
+-rw-rw-rw-   0        0        0     1890 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 23:40:40.000000 tmxpy-0.1.5/src/tmxpy.egg-info/top_level.txt
```

### Comparing `tmxpy-0.1.4/LICENSE` & `tmxpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.4/PKG-INFO` & `tmxpy-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,33 +14,52 @@
 
 # TMXpy
 
 A Python library for reading and writing TMX files.
 
 This library is fairly computer intensive, especially when rendering large maps. It is recommended to use a computer with decent specs when using this library.
 
+**Please note**: This library only supports files saved with the CSV encoding.
+
 ## Features
 
-- Rendering of TMX files to images (CSV encoding only)
+- Rendering of TMX files to images
+- Replacing specific warps with other warps
+- Changing tiles of a TMX file
+- Adding tilesets to a TMX file
 
 ## Installation
 
 ```bash
 pip install tmxpy
 ```
 
-## Usage
+## Usage and Examples
 
 ```python
 from tmxpy import TMXpy
 from pathlib import Path
 
 tmx = TMXpy(sheets=[Path("path/to/tilesheet/directory")], path=Path("path/to/tmx/file"))
 tmx.generateGIDDict()
 tmx.renderAllLayers().save("path/to/output/image.png")
+
+tmx.parseWarps()
+tmx.replace_warp(0, {
+    "map_x": 23,
+    "map_y": 17,
+    "destination": "Town",
+    "dest_x": 10,
+    "dest_y": 8,
+})
+
+tmx.setTile(23, 17, "129", layerName="Buildings")
+
 ```
 
+Further examples can be found in the [tests](https://github.com/AnotherPillow/tmxpy/tree/main/tests) directory.
+
 ## Development/Testing
 
 - Install dependencies with `pip install -r requirements.txt`
 - Tests can be added to tests/name_of_test.py and run with `py -m tests.name_of_test`
 - It can be built with `py -m build`
```

### Comparing `tmxpy-0.1.4/pyproject.toml` & `tmxpy-0.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmxpy"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="AnotherPillow", email="redacted@email.xyz" }
 ]
 description = "A Python library for reading and writing TMX files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tmxpy-0.1.4/src/tmxpy/tmxpy.py` & `tmxpy-0.1.5/src/tmxpy/tmxpy.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 class TMXpy:
     spriteSheetFolderPaths: Sequence[Path|str] = []
     inputFile: bs4.BeautifulSoup
     tileDimensions: tuple[int, int] = (0, 0)
     tmxDimensions: tuple[int, int] = (0, 0)
     tiles: dict = {}
+    maxGID: int = 0
 
     def __init__(self, sheets: Sequence[Path|str], path: str | Path = '', xml: str = ''):
         """Initializes the TMXpy class"""
         
         if path != '':
             self.path = path
             self.inputFile = bs4.BeautifulSoup(open(path), "xml")
@@ -73,25 +74,38 @@
                     "src": src,
                     "x": int((i - int(tileset["firstgid"])) % int(tileset["columns"])),
                     "y": int((i - int(tileset["firstgid"])) / int(tileset["columns"])),
                     "width": int(tileset["tilewidth"]),
                     "height": int(tileset["tileheight"])
                 }
 
+        self.maxGID = len(self.tiles)
+
+    def findPathOfTileSheet(self, sheet: str, ext: str = '') -> str:
+        """Finds the folder containing the given sheet"""
+        for path in self.spriteSheetFolderPaths:
+            fullpath = self.addExtIfNeeded(os.path.join(path, sheet), ext)
+            if os.path.exists(fullpath):
+                return str(fullpath)
+        else:
+            raise Exception(f"TMXpy: Could not find tileset {sheet} in any of the given paths {self.spriteSheetFolderPaths}")
+        
+    def addExtIfNeeded(self, path: str, ext: str) -> str:
+        """Adds an extension to a path if it doesn't have it"""
+        if not path.endswith(ext):
+            path += ext
+        return path
+        
+
     def renderTile(self, gid: str) -> Image.Image:
         """Renders a tile from the TMX file"""
         tile = self.tiles[gid]
         
         #path = os.path.join(self.spriteSheetFolderPaths[0], tile["src"]) + ".png"
-        for path in self.spriteSheetFolderPaths:
-            if os.path.exists(os.path.join(path, tile["src"] + ".png")):
-                path = os.path.join(path, tile["src"]) + ".png"
-                break
-        else:
-            raise Exception(f"TMXpy: Could not find tileset {tile['src']} in any of the given paths {self.spriteSheetFolderPaths}")
+        path = self.findPathOfTileSheet(tile["src"], ".png")
         tilesheet = Image.open(path)
         
         tile = tilesheet.crop((tile["x"] * tile["width"], tile["y"] * tile["height"], tile["x"] * tile["width"] + tile["width"], tile["y"] * tile["height"] + tile["height"]))
         return tile
 
     def renderLayer(self, layerID: int) -> Image.Image:
         """Renders a layer in the TMX file"""
@@ -181,16 +195,67 @@
         columns = rows[y].split(",")
         
         columns[x] = tile
         rows[y] = ",".join(columns)
         output = "\n".join(rows)
         
         layer.contents[0].replace_with(output) # type: ignore <-- like wtf pylint why what is this
+
+    def addTilesheet(self, filename: str, setname: str, tileproperties: dict[str, list]) -> None:
+        #loop through the sheet dirs, check if filename exists in any of them
+        imgpath = self.findPathOfTileSheet(filename, ".png")
+        img = Image.open(imgpath)
+        
+        width_tiles = img.width // 16
+        height_tiles = img.height // 16
+
+        elm = self.inputFile.new_tag("tileset", 
+            attrs={
+                "name": setname,
+                "tilewidth": "16",
+                "tileheight": "16",
+                "tilecount": str(width_tiles * height_tiles),
+                "columns": str(width_tiles),
+                "firstgid": str(self.maxGID + 1)
+            })
         
+        imgelm = self.inputFile.new_tag("image",
+            attrs={
+                "source": filename,
+                "width": str(img.width),
+                "height": str(img.height)
+            }
+        )
+
+        elm.append(imgelm)
+        
+        for tile in tileproperties: #iter through dict
+            tileelm = self.inputFile.new_tag("tile", id=tile)
+            propselm = self.inputFile.new_tag("properties")
+
+            for prop in tileproperties[tile]: #iter through list in dict (key for list is tile id)
+                #dict would be like {tile_id: [{name: "name", value: "value", type: "type"}, ...]}
+                propelm = self.inputFile.new_tag("property",
+                    attrs={
+                        "name": prop['name'],
+                        "value": tileproperties[tile][prop]['value'],
+                        "type": tileproperties[tile][prop]['type']
+                    }
+                )
+                propselm.append(propelm)
+
+            tileelm.append(propselm)
+            elm.append(tileelm)
+
+        map = self.inputFile.map
+        if map is None:
+            raise Exception("TMXpy: No map element found")
         
+        map.append(elm)
+
 
     def save(self, path: str or Path):
 
         if 'warps' in self.__dict__:
             self.inputFile.find("property", {"name": "Warp"})['value'] = " ".join([f"{w['map_x']} {w['map_y']} {w['destination']} {w['dest_x']} {w['dest_y']}" for w in self.warps]) # type: ignore
 
         with open(path, "w") as f:
```

### Comparing `tmxpy-0.1.4/src/tmxpy.egg-info/PKG-INFO` & `tmxpy-0.1.5/src/tmxpy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -14,33 +14,52 @@
 
 # TMXpy
 
 A Python library for reading and writing TMX files.
 
 This library is fairly computer intensive, especially when rendering large maps. It is recommended to use a computer with decent specs when using this library.
 
+**Please note**: This library only supports files saved with the CSV encoding.
+
 ## Features
 
-- Rendering of TMX files to images (CSV encoding only)
+- Rendering of TMX files to images
+- Replacing specific warps with other warps
+- Changing tiles of a TMX file
+- Adding tilesets to a TMX file
 
 ## Installation
 
 ```bash
 pip install tmxpy
 ```
 
-## Usage
+## Usage and Examples
 
 ```python
 from tmxpy import TMXpy
 from pathlib import Path
 
 tmx = TMXpy(sheets=[Path("path/to/tilesheet/directory")], path=Path("path/to/tmx/file"))
 tmx.generateGIDDict()
 tmx.renderAllLayers().save("path/to/output/image.png")
+
+tmx.parseWarps()
+tmx.replace_warp(0, {
+    "map_x": 23,
+    "map_y": 17,
+    "destination": "Town",
+    "dest_x": 10,
+    "dest_y": 8,
+})
+
+tmx.setTile(23, 17, "129", layerName="Buildings")
+
 ```
 
+Further examples can be found in the [tests](https://github.com/AnotherPillow/tmxpy/tree/main/tests) directory.
+
 ## Development/Testing
 
 - Install dependencies with `pip install -r requirements.txt`
 - Tests can be added to tests/name_of_test.py and run with `py -m tests.name_of_test`
 - It can be built with `py -m build`
```

