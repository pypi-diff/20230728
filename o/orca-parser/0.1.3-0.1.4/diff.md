# Comparing `tmp/orca_parser-0.1.3-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6589 bytes, number of entries: 8
+Zip file size: 6963 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-19 09:53 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    12102 b- defN 23-Jul-28 18:35 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/RECORD
-8 files, 16234 bytes uncompressed, 5453 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 18:37 orca_parser-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-28 18:37 orca_parser-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-28 18:37 orca_parser-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-28 18:37 orca_parser-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-28 18:37 orca_parser-0.1.4.dist-info/RECORD
+8 files, 18204 bytes uncompressed, 5827 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.3.dist-info/LICENSE
+Filename: orca_parser-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.3.dist-info/METADATA
+Filename: orca_parser-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.3.dist-info/WHEEL
+Filename: orca_parser-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.3.dist-info/top_level.txt
+Filename: orca_parser-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.3.dist-info/RECORD
+Filename: orca_parser-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jul  6 10:37:13 2023
 
 @author: Alex
 """
 import numpy as np
-import ase
+import ase, pandas
 from ase.io import read
 
 def readin(fname):
     # ORCA sometimes makes output that is hard to parse, we will try to read it the quick way first
     try:
         f = open(fname)
         content = f.read()
@@ -187,15 +187,67 @@
         hours = hours + (days*24)
         minutes = minutes + (hours*60)
         seconds = seconds + (minutes*60)
         seconds = seconds + (miliseconds/1000)
         return seconds
     
     def parse_input(self):
-        return self.raw.split("|  1>")[1].split("\n")[0]
+        self.Z = int(round(float(self.raw.split("Sum of atomic charges:")[1].split("\n")[0])))
+        self.Multiplicity = int(round(float(self.raw.split("* xyz")[1].split("\n")[0].split()[1])))
+        inp = self.raw.split("|  1>")[1].split("\n")[0]
+        inp = inp.upper()
+        print(inp)
+        inp = inp.replace("!", "")
+        inp = inp.split()
+        inp_dict = {"Job": None, 
+                    "Freq": False,
+                    "Solvation": "Gas",
+                    "Dispersion": None,
+                    "Charge": self.Z,
+                    "defgrid": None,
+                    "def2/J": None,
+                    "Multiplicity": self.Multiplicity}
+        i = 0
+        while i < len(inp):
+            if inp[i] in ["SP", "OPT"]:
+                inp_dict["Job"] = inp[i]
+                del inp[i]
+                continue
+            elif "FREQ" in inp[i]:
+                inp_dict["Freq"] = True
+                del inp[i]
+                continue
+            elif inp[i] in ["B3LYP", "PBE"] or "WB9" in inp[i]:
+                inp_dict["Functional"] = inp[i]
+                del inp[i]
+                continue
+            elif "CPCM" in inp[i] or "SMD" in inp[i]:
+                inp_dict["Solvation"] = inp[i]
+                del inp[i]
+                continue
+            elif "DEF2-" in inp[i] or "SVP" in inp[i] or "VP" in inp[i]:
+                inp_dict["BasisSet"] = inp[i]
+                del inp[i]
+                continue
+            elif "D3" in inp[i] or "D3BJ" in inp[i] or "D4" in inp[i]:
+                inp_dict["Dispersion"] = inp[i]
+                del inp[i]
+                continue
+            elif "DEFGRID" in inp[i]:
+                inp_dict["defgrid"] = inp[i]
+                del inp[i]
+                continue
+            elif "DEF2/J" in inp[i]:
+                inp_dict["def2/J"] = True
+                del inp[i]
+                continue
+            
+            
+            i+= 1
+        return inp_dict
     
     def convergence(self):
         self.conv = dict()
         self.tol = dict()
         if "Geometry convergence" not in self.raw:
             return 0
         for segment in self.raw.split("Geometry convergence")[1:]:
```

## Comparing `orca_parser-0.1.3.dist-info/LICENSE` & `orca_parser-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

