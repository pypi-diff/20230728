# Comparing `tmp/mapfile_parser-1.1.4.tar.gz` & `tmp/mapfile_parser-1.1.5.tar.gz`

## Comparing `mapfile_parser-1.1.4.tar` & `mapfile_parser-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    14977 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/LICENSE
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/PKG-INFO
```

### Comparing `mapfile_parser-1.1.4/.github/workflows/mypy.yml` & `mapfile_parser-1.1.5/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/.github/workflows/upload_pypi.yml` & `mapfile_parser-1.1.5/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/__main__.py` & `mapfile_parser-1.1.5/src/mapfile_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/mapfile.py` & `mapfile_parser-1.1.5/src/mapfile_parser/mapfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 from . import utils
 
 
 regex_fileDataEntry = re.compile(r"^\s+(?P<section>\.[^\s]+)\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s+(?P<name>[^\s]+)$")
 regex_functionEntry = re.compile(r"^\s+(?P<vram>0x[^\s]+)\s+(?P<name>[^\s]+)$")
 regex_label = re.compile(r"^(?P<name>\.?L[0-9A-F]{8})$")
 regex_fill = re.compile(r"^\s+(?P<fill>\*[^\s\*]+\*)\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s*$")
+regex_loadAddress = re.compile(r"\s+(?P<vram>0x[^\s]+)\s+(?P<size>0x[^\s]+)\s+(?P<loadaddress>load address)\s+(?P<vrom>0x[^\s]+)$")
+
+@dataclasses.dataclass
+class LoadAddressData:
+    vram: int
+    size: int
+    vrom: int
 
 @dataclasses.dataclass
 class Symbol:
     name: str
     vram: int
     size: int = -1 # in bytes
     vrom: int|None = None
@@ -30,14 +37,19 @@
         return f"0x{self.vram:08X}"
 
     def getVromStr(self) -> str:
         if self.vrom is None:
             return "None"
         return f"0x{self.vrom:06X}"
 
+    def getSizeStr(self) -> str:
+        if self.size < 0:
+            return "None"
+        return f"0x{self.size:X}"
+
 
     @staticmethod
     def printCsvHeader():
         print("Symbol name,VRAM,Size in bytes")
 
     def printAsCsv(self):
         print(f"{self.name},{self.vram:08X},{self.size}")
@@ -137,30 +149,35 @@
 @dataclasses.dataclass
 class FoundSymbolInfo:
     file: File
     symbol: Symbol
     offset: int = 0
 
     def getAsStr(self) -> str:
-        return f"'{self.symbol.name}' (VRAM: {self.symbol.getVramStr()}, VROM: {self.symbol.getVromStr()}, {self.file.filepath})"
+        return f"'{self.symbol.name}' (VRAM: {self.symbol.getVramStr()}, VROM: {self.symbol.getVromStr()}, SIZE: {self.symbol.getSizeStr()}, {self.file.filepath})"
 
     def getAsStrPlusOffset(self, symName: str|None=None) -> str:
         if self.offset != 0:
-            message = f"{symName or self.symbol.name} is at 0x{self.offset:X} bytes inside"
+            if symName is not None:
+                message = symName
+            else:
+                message = f"0x{self.symbol.vram + self.offset:X}"
+            message += f" is at 0x{self.offset:X} bytes inside"
         else:
             message = "Symbol"
         return f"{message} {self.getAsStr()}"
 
 class MapFile:
     def __init__(self):
         self.filesList: list[File] = list()
         self.debugging: bool = False
 
     def readMapFile(self, mapPath: Path):
         tempFilesList: list[File] = list()
+        loadAddressData: LoadAddressData|None = None
 
         with mapPath.open("r") as f:
             mapData = f.read()
 
             # Skip the stuff we don't care about
             startIndex = 0
             auxVar = 0
@@ -190,69 +207,87 @@
                         labelMatch = regex_label.search(funcName)
                         if labelMatch is None:
                             tempFilesList[-1].symbols.append(Symbol(funcName, funcVram))
                         # print(hex(funcVram), funcName)
 
                 else:
                     inFile = False
-            else:
+
+            if not inFile:
                 fillMatch = regex_fill.search(line)
                 entryMatch = regex_fileDataEntry.search(line)
+                loadAddressMatch = regex_loadAddress.search(line)
 
                 if fillMatch is not None:
                     # Add *fill* size to last file
                     size = int(fillMatch["size"], 16)
                     tempFilesList[-1].size += size
                 elif entryMatch is not None:
                     # Find file
                     filepath = Path(entryMatch["name"])
                     size = int(entryMatch["size"], 16)
                     vram = int(entryMatch["vram"], 16)
                     segmentType = entryMatch["section"]
 
                     if size > 0:
                         inFile = True
-                        tempFilesList.append(File(filepath, vram, size, segmentType))
+                        tempFile = File(filepath, vram, size, segmentType)
+                        if loadAddressData is not None and loadAddressData.vram == vram:
+                            tempFile.vrom = loadAddressData.vrom
+                        tempFilesList.append(tempFile)
+
+                elif loadAddressMatch is not None:
+                    vram = int(loadAddressMatch["vram"], 0)
+                    size = int(loadAddressMatch["size"], 0)
+                    vrom = int(loadAddressMatch["vrom"], 0)
+
+                    loadAddressData = LoadAddressData(vram, size, vrom)
 
         vromOffset = 0
         for file in tempFilesList:
             acummulatedSize = 0
             symbolsCount = len(file.symbols)
 
+            if file.vrom is not None:
+                vromOffset = file.vrom
+
             isNoloadSegment = file.isNoloadSegment
             if not isNoloadSegment:
                 file.vrom = vromOffset
 
             if symbolsCount > 0:
+                symVrom = vromOffset
+
                 # Calculate size of each symbol
                 for index in range(symbolsCount-1):
                     func = file.symbols[index]
                     nextFunc = file.symbols[index+1]
 
                     size = (nextFunc.vram - func.vram)
                     acummulatedSize += size
 
                     file.symbols[index] = Symbol(func.name, func.vram, size)
 
                     if not isNoloadSegment:
                         # Only set vrom of non bss variables
-                        file.symbols[index].vrom = vromOffset
-                        vromOffset += size
+                        file.symbols[index].vrom = symVrom
+                        symVrom += size
 
                 # Calculate size of last symbol of the file
                 func = file.symbols[symbolsCount-1]
                 size = file.size - acummulatedSize
                 file.symbols[symbolsCount-1] = Symbol(func.name, func.vram, size)
                 if not isNoloadSegment:
-                    file.symbols[symbolsCount-1].vrom = vromOffset
-                    vromOffset += size
-            else:
-                if not isNoloadSegment:
-                    # Only increment vrom offset for non bss segments
-                    vromOffset += file.size
+                    file.symbols[symbolsCount-1].vrom = symVrom
+                    symVrom += size
+
+            if not isNoloadSegment:
+                # Only increment vrom offset for non bss segments
+                vromOffset += file.size
+
             self.filesList.append(file)
         return
 
     def filterBySegmentType(self, segmentType: str) -> MapFile:
         newMapFile = MapFile()
 
         newMapFile.debugging = self.debugging
```

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/progress_stats.py` & `mapfile_parser-1.1.5/src/mapfile_parser/progress_stats.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/utils.py` & `mapfile_parser-1.1.5/src/mapfile_parser/utils.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/first_diff.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/progress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/sym_info.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-1.1.5/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/.gitignore` & `mapfile_parser-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/LICENSE` & `mapfile_parser-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/README.md` & `mapfile_parser-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.4/PKG-INFO` & `mapfile_parser-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.1.4
+Version: 1.1.5
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```

