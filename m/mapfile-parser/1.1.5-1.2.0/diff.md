# Comparing `tmp/mapfile_parser-1.1.5.tar.gz` & `tmp/mapfile_parser-1.2.0.tar.gz`

## Comparing `mapfile_parser-1.1.5.tar` & `mapfile_parser-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.gitattributes
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/mypy.ini
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/requirements.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.github/workflows/upload_pypi.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/__main__.py
--rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/mapfile.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/progress_stats.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/utils.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/__init__.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/first_diff.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/pj64_syms.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/progress.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/sym_info.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/symbol_sizes_csv.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/src/mapfile_parser/frontends/upload_frogress.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/LICENSE
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.gitattributes
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/mypy.ini
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/requirements.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.github/workflows/upload_pypi.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/__main__.py
+-rw-r--r--   0        0        0    16186 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/mapfile.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/progress_stats.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/utils.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/__init__.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/first_diff.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/pj64_syms.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/progress.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/sym_info.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/symbol_sizes_csv.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/src/mapfile_parser/frontends/upload_frogress.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 mapfile_parser-1.2.0/PKG-INFO
```

### Comparing `mapfile_parser-1.1.5/.github/workflows/mypy.yml` & `mapfile_parser-1.2.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/.github/workflows/upload_pypi.yml` & `mapfile_parser-1.2.0/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/__main__.py` & `mapfile_parser-1.2.0/src/mapfile_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/mapfile.py` & `mapfile_parser-1.2.0/src/mapfile_parser/mapfile.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/progress_stats.py` & `mapfile_parser-1.2.0/src/mapfile_parser/progress_stats.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/utils.py` & `mapfile_parser-1.2.0/src/mapfile_parser/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 
 def readFileAsBytearray(filepath: Path) -> bytearray:
     if not filepath.exists():
         return bytearray(0)
     with filepath.open(mode="rb") as f:
         return bytearray(f.read())
 
-def hexbytes(bs):
-    return ":".join("{:02X}".format(c) for c in bs)
+def hexbytes(bs: bytes, addColons: bool=True) -> str:
+    glue = ""
+    if addColons:
+        glue = ""
+    return glue.join("{:02X}".format(c) for c in bs)
 
 def getGitCommitTimestamp() -> int:
     return int(subprocess.check_output(['git', 'show', '-s', '--format=%ct']).decode('ascii').rstrip())
 
 def getGitCommitHash() -> str:
     return subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode('ascii').strip()
```

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/first_diff.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/first_diff.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 # SPDX-FileCopyrightText: © 2022 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
+from typing import Callable
 
 from .. import mapfile
 from .. import utils
 
 
-def doFirstDiff(mapPath: Path, expectedMapPath: Path, romPath: Path, expectedRomPath: Path, diffCount: int=5, mismatchSize: bool=False) -> int:
+def doFirstDiff(mapPath: Path, expectedMapPath: Path, romPath: Path, expectedRomPath: Path, diffCount: int=5, mismatchSize: bool=False, addColons: bool=True, bytesConverterCallback:Callable[[bytes, mapfile.MapFile],str|None]|None=None) -> int:
     if not mapPath.exists():
         print(f"{mapPath} must exist")
         return 1
     if not expectedMapPath.exists():
         print(f"{expectedMapPath} must exist")
         return 1
     if not romPath.exists():
@@ -57,15 +58,22 @@
         ):
             if diffs == 0:
                 vromInfo = builtMapFile.findSymbolByVramOrVrom(i)
                 extraMessage = ""
                 if vromInfo is not None:
                     extraMessage = f", {vromInfo.getAsStrPlusOffset()}"
                 print(f"First difference at ROM addr 0x{i:X}{extraMessage}")
-                print(f"Bytes: {utils.hexbytes(builtRom[i : i + 4])} vs {utils.hexbytes(expectedRom[i : i + 4])}")
+                builtBytes = builtRom[i : i + 4]
+                expectedBytes = expectedRom[i : i + 4]
+                print(f"Bytes: {utils.hexbytes(builtBytes, addColons=addColons)} vs {utils.hexbytes(expectedBytes, addColons=addColons)}")
+                if bytesConverterCallback is not None:
+                    builtConverted = bytesConverterCallback(builtBytes, builtMapFile)
+                    expectedConverted = bytesConverterCallback(expectedBytes, expectedMapFile)
+                    if builtConverted is not None and expectedConverted is not None:
+                        print(f"{builtConverted} vs {expectedConverted}")
             diffs += 1
 
         if (
             len(map_search_diff) < diffCount
             and builtRom[i] >> 2 != expectedRom[i] >> 2
         ):
             vromInfo = builtMapFile.findSymbolByVramOrVrom(i)
@@ -74,15 +82,22 @@
                 if vromMessage not in map_search_diff:
                     map_search_diff.add(vromMessage)
 
                     extraMessage = ""
                     if vromInfo is not None:
                         extraMessage = f", {vromInfo.getAsStrPlusOffset()}"
                     print(f"Instruction difference at ROM addr 0x{i:X}{extraMessage}")
-                    print(f"Bytes: {utils.hexbytes(builtRom[i : i + 4])} vs {utils.hexbytes(expectedRom[i : i + 4])}")
+                    builtBytes = builtRom[i : i + 4]
+                    expectedBytes = expectedRom[i : i + 4]
+                    print(f"Bytes: {utils.hexbytes(builtBytes, addColons=addColons)} vs {utils.hexbytes(expectedBytes, addColons=addColons)}")
+                    if bytesConverterCallback is not None:
+                        builtConverted = bytesConverterCallback(builtBytes, builtMapFile)
+                        expectedConverted = bytesConverterCallback(expectedBytes, expectedMapFile)
+                        if builtConverted is not None and expectedConverted is not None:
+                            print(f"{builtConverted} vs {expectedConverted}")
 
         if len(map_search_diff) >= diffCount and diffs > shift_cap:
             break
 
     if diffs == 0:
         print("No differences but ROMs differ?")
         return 1
```

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/pj64_syms.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/pj64_syms.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/progress.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/progress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/sym_info.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/sym_info.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/symbol_sizes_csv.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/symbol_sizes_csv.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/src/mapfile_parser/frontends/upload_frogress.py` & `mapfile_parser-1.2.0/src/mapfile_parser/frontends/upload_frogress.py`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/.gitignore` & `mapfile_parser-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/LICENSE` & `mapfile_parser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/README.md` & `mapfile_parser-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mapfile_parser-1.1.5/pyproject.toml` & `mapfile_parser-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: © 2022 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "mapfile_parser"
-version = "1.1.5"
+version = "1.2.0"
 description = "Map file parser library focusing decompilation projects"
 readme = "README.md"
 requires-python = ">=3.7"
 dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/Decompollaborate/mapfile_parser"
```

### Comparing `mapfile_parser-1.1.5/PKG-INFO` & `mapfile_parser-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapfile_parser
-Version: 1.1.5
+Version: 1.2.0
 Summary: Map file parser library focusing decompilation projects
 Project-URL: Homepage, https://github.com/Decompollaborate/mapfile_parser
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/mapfile_parser/issues
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```

