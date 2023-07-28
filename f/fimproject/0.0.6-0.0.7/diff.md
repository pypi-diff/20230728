# Comparing `tmp/FIMProject-0.0.6.tar.gz` & `tmp/fimproject-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FIMProject-0.0.6.tar", last modified: Fri Jul 21 13:22:09 2023, max compression
+gzip compressed data, was "fimproject-0.0.7.tar", last modified: Fri Jul 28 10:12:00 2023, max compression
```

## Comparing `FIMProject-0.0.6.tar` & `fimproject-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:09.686531 FIMProject-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-07-01 11:37:01.000000 FIMProject-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1142 2023-07-21 13:22:09.687539 FIMProject-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-21 12:10:10.000000 FIMProject-0.0.6/README.md
--rw-rw-rw-   0        0        0       88 2023-07-01 11:37:01.000000 FIMProject-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1004 2023-07-21 13:22:09.689538 FIMProject-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:09.658355 FIMProject-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:09.670407 FIMProject-0.0.6/src/FIM/
--rw-rw-rw-   0        0        0     4784 2023-07-03 21:52:07.000000 FIMProject-0.0.6/src/FIM/Apriori.py
--rw-rw-rw-   0        0        0      286 2023-07-21 12:10:10.000000 FIMProject-0.0.6/src/FIM/__init__.py
--rw-rw-rw-   0        0        0     3227 2023-07-03 13:24:27.000000 FIMProject-0.0.6/src/FIM/association_rules.py
--rw-rw-rw-   0        0        0     4807 2023-07-03 22:05:02.000000 FIMProject-0.0.6/src/FIM/eclat.py
--rw-rw-rw-   0        0        0     5673 2023-07-05 13:07:14.000000 FIMProject-0.0.6/src/FIM/fpgrowth.py
--rw-rw-rw-   0        0        0     5328 2023-07-03 22:16:47.000000 FIMProject-0.0.6/src/FIM/hmine.py
--rw-rw-rw-   0        0        0     3290 2023-07-05 11:17:05.000000 FIMProject-0.0.6/src/FIM/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:09.684026 FIMProject-0.0.6/src/FIMProject.egg-info/
--rw-rw-rw-   0        0        0     1142 2023-07-21 13:22:09.000000 FIMProject-0.0.6/src/FIMProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-21 13:22:09.000000 FIMProject-0.0.6/src/FIMProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:22:09.000000 FIMProject-0.0.6/src/FIMProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-21 13:22:09.000000 FIMProject-0.0.6/src/FIMProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 13:22:09.000000 FIMProject-0.0.6/src/FIMProject.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:09.685027 FIMProject-0.0.6/src/FSM/
--rw-rw-rw-   0        0        0        0 2023-07-03 13:23:35.000000 FIMProject-0.0.6/src/FSM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:00.713570 fimproject-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-07-01 11:37:01.000000 fimproject-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3049 2023-07-28 10:12:00.713570 fimproject-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2397 2023-07-28 10:07:47.000000 fimproject-0.0.7/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-01 11:37:01.000000 fimproject-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1005 2023-07-28 10:12:00.715126 fimproject-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:00.688130 fimproject-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:00.699273 fimproject-0.0.7/src/FIM/
+-rw-rw-rw-   0        0        0      286 2023-07-21 12:10:10.000000 fimproject-0.0.7/src/FIM/__init__.py
+-rw-rw-rw-   0        0        0     4784 2023-07-03 21:52:07.000000 fimproject-0.0.7/src/FIM/apriori.py
+-rw-rw-rw-   0        0        0     3227 2023-07-03 13:24:27.000000 fimproject-0.0.7/src/FIM/association_rules.py
+-rw-rw-rw-   0        0        0     4807 2023-07-03 22:05:02.000000 fimproject-0.0.7/src/FIM/eclat.py
+-rw-rw-rw-   0        0        0     5673 2023-07-05 13:07:14.000000 fimproject-0.0.7/src/FIM/fpgrowth.py
+-rw-rw-rw-   0        0        0     5328 2023-07-03 22:16:47.000000 fimproject-0.0.7/src/FIM/hmine.py
+-rw-rw-rw-   0        0        0     3290 2023-07-05 11:17:05.000000 fimproject-0.0.7/src/FIM/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:00.701165 fimproject-0.0.7/src/FSM/
+-rw-rw-rw-   0        0        0        0 2023-07-03 13:23:35.000000 fimproject-0.0.7/src/FSM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 10:12:00.712566 fimproject-0.0.7/src/fimproject.egg-info/
+-rw-rw-rw-   0        0        0     3049 2023-07-28 10:12:00.000000 fimproject-0.0.7/src/fimproject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-28 10:12:00.000000 fimproject-0.0.7/src/fimproject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 10:12:00.000000 fimproject-0.0.7/src/fimproject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-28 10:12:00.000000 fimproject-0.0.7/src/fimproject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 10:12:00.000000 fimproject-0.0.7/src/fimproject.egg-info/top_level.txt
```

### Comparing `FIMProject-0.0.6/LICENSE` & `fimproject-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/setup.cfg` & `fimproject-0.0.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2046 494d 5072 6f6a 6563 740d 0a76   = FIMProject..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e36 0d0a  ersion = 0.0.6..
+00000010: 203d 2066 696d 7072 6f6a 6563 740d 0a76   = fimproject..v
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e37 0d0a  ersion = 0.0.7..
 00000030: 6175 7468 6f72 203d 2046 6174 6968 2053  author = Fatih S
 00000040: 656e 0d0a 6175 7468 6f72 5f65 6d61 696c  en..author_email
-00000050: 203d 2066 6174 6968 2e73 6e32 3030 3040   = fatih.sn2000@
-00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
-00000070: 6970 7469 6f6e 203d 2046 7265 7175 656e  iption = Frequen
-00000080: 7420 4974 656d 7365 7420 4d69 6e69 6e67  t Itemset Mining
-00000090: 2061 6e64 2046 7265 7175 656e 7420 5365   and Frequent Se
-000000a0: 7175 656e 6365 204d 696e 696e 6720 416c  quence Mining Al
-000000b0: 676f 7269 7468 6d73 2070 6163 6b61 6765  gorithms package
-000000c0: 2066 6f72 2041 524d 0d0a 6c6f 6e67 5f64   for ARM..long_d
-000000d0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000e0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000110: 7874 2f6d 6172 6b64 6f77 6e0d 0a6b 6579  xt/markdown..key
-00000120: 776f 7264 7320 3d20 4649 4d2c 2046 7265  words = FIM, Fre
-00000130: 7175 656e 7420 4974 656d 7365 7420 4d69  quent Itemset Mi
-00000140: 6e69 6e67 2c20 4672 6571 7565 6e74 2053  ning, Frequent S
-00000150: 6571 7565 6e63 6520 4d69 6e69 6e67 2c20  equence Mining, 
-00000160: 4173 736f 6369 6174 696f 6e20 5275 6c65  Association Rule
-00000170: 204d 696e 696e 672c 2041 524d 0d0a 7572   Mining, ARM..ur
-00000180: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000190: 7562 2e63 6f6d 2f66 6174 6968 7365 6e32  ub.com/fatihsen2
-000001a0: 302f 4672 6571 7565 6e74 2d4d 696e 696e  0/Frequent-Minin
-000001b0: 672d 416c 676f 7269 7468 6d73 0d0a 7265  g-Algorithms..re
-000001c0: 6164 6d65 203d 2052 4541 444d 452e 6d64  adme = README.md
-000001d0: 0d0a 7265 7175 6972 6573 2d70 7974 686f  ..requires-pytho
-000001e0: 6e20 3d20 223e 3d33 2e37 220d 0a63 6c61  n = ">=3.7"..cla
-000001f0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-00000230: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000240: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000250: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000260: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000270: 0a70 726f 6a65 6374 2e75 726c 7320 3d20  .project.urls = 
-00000280: 0d0a 0948 6f6d 6570 6167 6520 3d20 6874  ...Homepage = ht
-00000290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002a0: 2f66 6174 6968 7365 6e32 302f 4672 6571  /fatihsen20/Freq
-000002b0: 7565 6e74 2d4d 696e 696e 672d 416c 676f  uent-Mining-Algo
-000002c0: 7269 7468 6d73 0d0a 0953 6f75 7263 6520  rithms...Source 
-000002d0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-000002e0: 2e63 6f6d 2f66 6174 6968 7365 6e32 302f  .com/fatihsen20/
-000002f0: 4672 6571 7565 6e74 2d4d 696e 696e 672d  Frequent-Mining-
-00000300: 416c 676f 7269 7468 6d73 0d0a 0d0a 5b6f  Algorithms....[o
-00000310: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000320: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
-00000330: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000340: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000350: 6573 203d 203e 3d33 2e37 0d0a 0d0a 5b6f  es = >=3.7....[o
-00000360: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000370: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-00000380: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
-00000390: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-000003a0: 6e75 6d70 7920 3d20 6e75 6d70 790d 0a70  numpy = numpy..p
-000003b0: 616e 6461 7320 3d20 7061 6e64 6173 0d0a  andas = pandas..
-000003c0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003d0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000003e0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000050: 203d 2066 6174 6968 7365 6e2e 6461 7461   = fatihsen.data
+00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
+00000070: 7269 7074 696f 6e20 3d20 4672 6571 7565  ription = Freque
+00000080: 6e74 2049 7465 6d73 6574 204d 696e 696e  nt Itemset Minin
+00000090: 6720 616e 6420 4672 6571 7565 6e74 2053  g and Frequent S
+000000a0: 6571 7565 6e63 6520 4d69 6e69 6e67 2041  equence Mining A
+000000b0: 6c67 6f72 6974 686d 7320 7061 636b 6167  lgorithms packag
+000000c0: 6520 666f 7220 4152 4d0d 0a6c 6f6e 675f  e for ARM..long_
+000000d0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000e0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000100: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000110: 6578 742f 6d61 726b 646f 776e 0d0a 6b65  ext/markdown..ke
+00000120: 7977 6f72 6473 203d 2046 494d 2c20 4672  ywords = FIM, Fr
+00000130: 6571 7565 6e74 2049 7465 6d73 6574 204d  equent Itemset M
+00000140: 696e 696e 672c 2046 7265 7175 656e 7420  ining, Frequent 
+00000150: 5365 7175 656e 6365 204d 696e 696e 672c  Sequence Mining,
+00000160: 2041 7373 6f63 6961 7469 6f6e 2052 756c   Association Rul
+00000170: 6520 4d69 6e69 6e67 2c20 4152 4d0d 0a75  e Mining, ARM..u
+00000180: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000190: 6875 622e 636f 6d2f 6661 7469 6873 656e  hub.com/fatihsen
+000001a0: 3230 2f46 7265 7175 656e 742d 4d69 6e69  20/Frequent-Mini
+000001b0: 6e67 2d41 6c67 6f72 6974 686d 730d 0a72  ng-Algorithms..r
+000001c0: 6561 646d 6520 3d20 5245 4144 4d45 2e6d  eadme = README.m
+000001d0: 640d 0a72 6571 7569 7265 732d 7079 7468  d..requires-pyth
+000001e0: 6f6e 203d 2022 3e3d 332e 3722 0d0a 636c  on = ">=3.7"..cl
+000001f0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000220: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000230: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000240: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000250: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000260: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000270: 0d0a 7072 6f6a 6563 742e 7572 6c73 203d  ..project.urls =
+00000280: 200d 0a09 486f 6d65 7061 6765 203d 2068   ...Homepage = h
+00000290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002a0: 6d2f 6661 7469 6873 656e 3230 2f46 7265  m/fatihsen20/Fre
+000002b0: 7175 656e 742d 4d69 6e69 6e67 2d41 6c67  quent-Mining-Alg
+000002c0: 6f72 6974 686d 730d 0a09 536f 7572 6365  orithms...Source
+000002d0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000002e0: 622e 636f 6d2f 6661 7469 6873 656e 3230  b.com/fatihsen20
+000002f0: 2f46 7265 7175 656e 742d 4d69 6e69 6e67  /Frequent-Mining
+00000300: 2d41 6c67 6f72 6974 686d 730d 0a0d 0a5b  -Algorithms....[
+00000310: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000320: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000330: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000340: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000350: 7265 7320 3d20 3e3d 332e 370d 0a0d 0a5b  res = >=3.7....[
+00000360: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000370: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000380: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
+00000390: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
+000003a0: 0a6e 756d 7079 203d 206e 756d 7079 0d0a  .numpy = numpy..
+000003b0: 7061 6e64 6173 203d 2070 616e 6461 730d  pandas = pandas.
+000003c0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000003d0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000003e0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `FIMProject-0.0.6/src/FIM/Apriori.py` & `fimproject-0.0.7/src/FIM/apriori.py`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/src/FIM/association_rules.py` & `fimproject-0.0.7/src/FIM/association_rules.py`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/src/FIM/eclat.py` & `fimproject-0.0.7/src/FIM/eclat.py`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/src/FIM/fpgrowth.py` & `fimproject-0.0.7/src/FIM/fpgrowth.py`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/src/FIM/hmine.py` & `fimproject-0.0.7/src/FIM/hmine.py`

 * *Files identical despite different names*

### Comparing `FIMProject-0.0.6/src/FIM/utils.py` & `fimproject-0.0.7/src/FIM/utils.py`

 * *Files identical despite different names*

