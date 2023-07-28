# Comparing `tmp/am2r_yams-0.0.5.tar.gz` & `tmp/am2r_yams-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-0.0.5.tar", last modified: Mon Jul 24 20:33:08 2023, max compression
+gzip compressed data, was "am2r_yams-0.0.7.tar", last modified: Fri Jul 28 11:51:55 2023, max compression
```

## Comparing `am2r_yams-0.0.5.tar` & `am2r_yams-0.0.7.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.079119 am2r_yams-0.0.5/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/Patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.079119 am2r_yams-0.0.5/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/__pyinstaller/hook-am2r_yams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.087119 am2r_yams-0.0.5/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.5/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.5/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.5/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.5/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.5/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.5/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (123)   941568 2023-07-24 20:32:54.000000 am2r_yams-0.0.5/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-24 20:32:53.000000 am2r_yams-0.0.5/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-24 20:32:57.000000 am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (123)   170496 2023-07-24 20:32:57.000000 am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-07-24 20:32:56.000000 am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.087119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.5/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.087119 am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/sprites/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.095119 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorArachnus.png
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorBlue.png
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorGenesis.png
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorGuardian.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorLocked.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorQueen.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorScrew.png
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSerris.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSpider.png
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSuper.png
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTester.png
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTorizo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.075119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.099119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.099119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.103119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.103119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.103119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.107119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.107119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.111119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.111119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.111119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.111119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.115119 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.115119 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
--rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newA4Doors.png
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newA4Doors2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUIMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUIPBomb.png
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUISMissile.png
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpHideout.png
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.079119 am2r_yams-0.0.5/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:33:07.000000 am2r_yams-0.0.5/am2r_yams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 20:33:08.000000 am2r_yams-0.0.5/am2r_yams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/am2r_yams_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/am2r_yams_tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 20:32:23.000000 am2r_yams-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-24 20:33:08.119120 am2r_yams-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.959507 am2r_yams-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 11:51:55.959507 am2r_yams-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.931506 am2r_yams-0.0.7/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.931506 am2r_yams-0.0.7/am2r_yams/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/__pyinstaller/hook-am2r_yams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.935506 am2r_yams-0.0.7/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (123)   204800 2021-09-19 09:20:24.000000 am2r_yams-0.0.7/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    42496 2022-06-15 03:36:02.000000 am2r_yams-0.0.7/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (123)    27528 2020-10-19 18:40:26.000000 am2r_yams-0.0.7/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)     6656 2021-03-13 10:51:42.000000 am2r_yams-0.0.7/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (123)  2030080 2023-03-28 12:36:58.000000 am2r_yams-0.0.7/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   173432 2021-10-22 20:57:42.000000 am2r_yams-0.0.7/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   941568 2023-07-28 11:51:46.000000 am2r_yams-0.0.7/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   319029 2023-07-28 11:51:45.000000 am2r_yams-0.0.7/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-28 11:51:48.000000 am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (123)   173056 2023-07-28 11:51:48.000000 am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    21992 2023-07-28 11:51:48.000000 am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.935506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)   419720 2021-10-22 20:57:34.000000 am2r_yams-0.0.7/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.935506 am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (123)    52104 2020-10-19 18:52:12.000000 am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (123)   436600 2021-10-22 20:58:02.000000 am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/sprites/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.939506 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorArachnus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorBlue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorGenesis.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorGuardian.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorLocked.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorQueen.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorScrew.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSerris.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSpider.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSuper.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTester.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTorizo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.927506 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.943506 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.943506 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.943506 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.947507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.947507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.947507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.951507 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.955507 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.955507 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newA4Doors.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newA4Doors2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.955507 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUIMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUIPBomb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUISMissile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpHideout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.955507 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.931506 am2r_yams-0.0.7/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 11:51:55.000000 am2r_yams-0.0.7/am2r_yams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:51:55.959507 am2r_yams-0.0.7/am2r_yams_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/am2r_yams_tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 11:51:29.000000 am2r_yams-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-28 11:51:55.959507 am2r_yams-0.0.7/setup.cfg
```

### Comparing `am2r_yams-0.0.5/LICENSE` & `am2r_yams-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/PKG-INFO` & `am2r_yams-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 0.0.5
+Version: 0.0.7
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `am2r_yams-0.0.5/am2r_yams/Patcher.py` & `am2r_yams-0.0.7/am2r_yams/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,79 +3,99 @@
 import platform
 import shutil
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 from typing import Callable
+from contextlib import contextmanager
 
 # TODO: revise this to be cleaner. Following things to keep in mind here
-# 1. AFAIK the DLLs must be in path before loading the CLR. test whether that's truly the case
-# 2. the CLR should only loaded *once*. I.e importing this module multiple times shouldnt cause exceptions of trying to load it multiple times.
-# 3. Figure out how to deal with non-system dotnet installations
+# 1. AFAIK the DLLs must be in path before loading the CLR. test whether that's truly the case.
+#    Maybe we can remove from path when we're done?
+# 2. Figure out how to deal with non-system dotnet installations
 yams_path = os.fspath(Path(__file__).with_name(name="yams"))
 sys.path.append(yams_path)
-from pythonnet import load
+from pythonnet import load, unload
 
-load("coreclr")
-import clr
 
-clr.AddReference("YAMS-LIB")
-from YAMS_LIB import Patcher
-
-
-def get_lib_version() -> str:
-    return Patcher.Version
-
-
-# TODO: ADD TESTS!!!
-def patch_game(
-    input_path: Path,
-    output_path: Path,
-    patch_data: dict,
-    progress_update: Callable[[str, float], None],
-):
-    # Copy to input dir to temp dir first to do operations there
-    progress_update("Copying to temporary path...", 0)
-    tempdir = tempfile.TemporaryDirectory()
-    shutil.copytree(input_path, tempdir.name, dirs_exist_ok=True)
-
-    # Get data.win path. Both of these *need* to be strings, as otherwise patcher won't accept them.
-    output_data_win: str = os.fspath(
-        _prepare_environment_and_get_data_win_path(tempdir.name)
-    )
-    input_data_win: str = shutil.move(output_data_win, output_data_win + "_orig")
-    input_data_win_path = Path(input_data_win)
-
-    # TODO: do some check on whether input is valid? on patcher side probably.
-
-    # Temp write patch_data into json file for yams later
-    progress_update("Creating json file...", 0.3)
-    json_file: str = os.fspath(input_data_win_path.parent.joinpath("yams-data.json"))
-    with open(json_file, "w+") as f:
-        f.write(json.dumps(patch_data))
-
-    # AM2RLauncher installations usually have a profile.xml file. For less confusion, remove it if it exists
-    profile_xml_path = Path(tempdir.name).joinpath("profile.xml")
-    if profile_xml_path.exists():
-        profile_xml_path.unlink()
-
-    # TODO: this is where we'd call the patcher to do some customization options like music shuffler or samus palettes
-
-    # Patch data.win
-    progress_update("Patching data file...", 0.6)
-    Patcher.Main(input_data_win, output_data_win, json_file)
-
-    # Move temp dir to output dir and get rid of it. Also delete original data.win
-    input_data_win_path.unlink()
-    progress_update("Moving to output directory...", 0.8)
-    shutil.copytree(tempdir.name, output_path, dirs_exist_ok=True)
-    shutil.rmtree(tempdir.name)
-
-    progress_update("Exporting finished!", 1)
+# TODO: add docstrings for methods when not in alpha and has stableish API
+class Wrapper:
+    def __init__(self, lib):
+        self.csharp_patcher = lib
+
+    def get_csharp_version(self) -> str:
+        return self.csharp_patcher.Version
+
+    # TODO: ADD TESTS!!!
+    def patch_game(
+        self,
+        input_path: Path,
+        output_path: Path,
+        patch_data: dict,
+        progress_update: Callable[[str, float], None],
+    ):
+        # Copy to input dir to temp dir first to do operations there
+        progress_update("Copying to temporary path...", 0)
+        tempdir = tempfile.TemporaryDirectory()
+        shutil.copytree(input_path, tempdir.name, dirs_exist_ok=True)
+
+        # Get data.win path. Both of these *need* to be strings, as otherwise patcher won't accept them.
+        output_data_win: str = os.fspath(
+            _prepare_environment_and_get_data_win_path(tempdir.name)
+        )
+        input_data_win: str = shutil.move(output_data_win, output_data_win + "_orig")
+        input_data_win_path = Path(input_data_win)
+
+        # TODO: do some check on whether input is valid? on patcher side probably.
+
+        # Temp write patch_data into json file for yams later
+        progress_update("Creating json file...", 0.3)
+        json_file: str = os.fspath(
+            input_data_win_path.parent.joinpath("yams-data.json")
+        )
+        with open(json_file, "w+") as f:
+            f.write(json.dumps(patch_data))
+
+        # AM2RLauncher installations usually have a profile.xml file. For less confusion, remove it if it exists
+        profile_xml_path = Path(tempdir.name).joinpath("profile.xml")
+        if profile_xml_path.exists():
+            profile_xml_path.unlink()
+
+        # TODO: this is where we'd call the patcher to do some customization options like music shuffler or samus palettes
+
+        # Patch data.win
+        progress_update("Patching data file...", 0.6)
+        self.csharp_patcher.Main(input_data_win, output_data_win, json_file)
+
+        # Move temp dir to output dir and get rid of it. Also delete original data.win
+        input_data_win_path.unlink()
+        progress_update("Moving to output directory...", 0.8)
+        shutil.copytree(tempdir.name, output_path, dirs_exist_ok=True)
+        shutil.rmtree(tempdir.name)
+
+        progress_update("Exporting finished!", 1)
+
+
+@contextmanager
+def load_wrapper() -> Wrapper:
+    try:
+        # Load dotnet runtime
+        load("coreclr")
+        import clr
+
+        clr.AddReference("YAMS-LIB")
+        from YAMS_LIB import Patcher as CSharp_Patcher
+
+        yield Wrapper(CSharp_Patcher)
+    finally:
+        # Unload dotnet runtime and references
+        del CSharp_Patcher
+        unload()
+        del clr
 
 
 def _prepare_environment_and_get_data_win_path(folder: str) -> Path:
     current_platform = platform.system()
     folderPath = Path(folder)
     if current_platform == "Windows":
         return folderPath.joinpath("data.win")
```

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-0.0.7/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-0.0.7/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.7/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-0.0.7/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-0.0.7/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-0.0.7/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-0.0.7/am2r_yams/yams/UndertaleModLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-0.0.7/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/0.0.7': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), delete: ['YAMS-LIB/0.0.5']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'YAMS-LIB/0.0.7': OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Macross.Json.Extensions', '3.0.0'), ('SixLabors.ImageSharp', "*

 * *              "'3.0.1'), ('UndertaleModLib', '1.0.0')])), ('runtime', "*

 * *              "OrderedDict([('YAMS-LIB.dll', OrderedDict())]))]), delete: ['YAMS-LIB/0.0.5' […]*

```diff
@@ -58,15 +58,15 @@
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/0.0.5": {
+        "YAMS-LIB/0.0.7": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         }
     },
     "runtimeTarget": {
         "name": ".NETCoreApp,Version=v6.0",
@@ -159,15 +159,15 @@
                     "SharpZipLib": "1.3.3",
                     "System.Drawing.Common": "5.0.3"
                 },
                 "runtime": {
                     "UndertaleModLib.dll": {}
                 }
             },
-            "YAMS-LIB/0.0.5": {
+            "YAMS-LIB/0.0.7": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
                     "SixLabors.ImageSharp": "3.0.1",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
                     "YAMS-LIB.dll": {}
```

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 8% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xc32d3ed1
+	             Time stamp: 0xbbe4a954
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00029200
+	              Code Size: 0x00029c00
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0002b00a
+	        Entry Point RVA: 0x0002b9fe
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0002c000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,66 +41,66 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0002afb8 [0x0000004f]
+	     Import Table: 0x0002b9ac [0x0000004f]
 	   Resource Table: 0x0002c000 [0x0000031c]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0002e000 [0x0000000c]
-	            Debug: 0x0002aee0 [0x00000054]
+	            Debug: 0x0002b8d4 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00029038
+	   Virtual Size: 0x00029a30
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00029200
+	  Raw Data Size: 0x00029c00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x0000031c
 	Virtual Address: 0x0002c000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00029400
+	   Raw Data Ptr: 0x00029e00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x0002e000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00029800
+	   Raw Data Ptr: 0x0002a200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0000d084 [0x0001de5c]
+	         Metadata: 0x0000d440 [0x0001e494]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -109,30 +109,30 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0000207c [8208 == 0x00002010]
-	    Strings: 0x0000207c - 0x00003bf8 [7036 == 0x00001b7c]
-	       Blob: 0x0001c4d4 - 0x0001de5c [6536 == 0x00001988]
-	User string: 0x00003bf8 - 0x0001c4c4 [100556 == 0x000188cc]
-	       GUID: 0x0001c4c4 - 0x0001c4d4 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000021dc [8560 == 0x00002170]
+	    Strings: 0x000021dc - 0x00003e38 [7260 == 0x00001c5c]
+	       Blob: 0x0001c9f4 - 0x0001e494 [6816 == 0x00001aa0]
+	User string: 0x00003e38 - 0x0001c9e4 [101292 == 0x00018bac]
+	       GUID: 0x0001c9e4 - 0x0001c9f4 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at b34c)
-Table TypeRef: 107 records (6 bytes, at b356)
-Table TypeDef: 24 records (14 bytes, at b5d8)
-Table Field: 201 records (6 bytes, at b728)
-Table Method: 71 records (14 bytes, at bbde)
-Table Param: 71 records (6 bytes, at bfc0)
-Table MemberRef: 266 records (6 bytes, at c16a)
-Table Constant: 110 records (6 bytes, at c7a6)
-Table CustomAttribute: 304 records (6 bytes, at ca3a)
-Table ClassLayout: 1 records (8 bytes, at d15a)
-Table StandaloneSig: 6 records (2 bytes, at d162)
-Table TypeSpec: 43 records (2 bytes, at d16e)
-Table FieldRVA: 1 records (6 bytes, at d1c4)
-Table Assembly: 1 records (22 bytes, at d1ca)
-Table AssemblyRef: 9 records (20 bytes, at d1e0)
-Table NestedClass: 6 records (4 bytes, at d294)
-Table MethodSpec: 20 records (4 bytes, at d2ac)
+Table Module: 1 records (10 bytes, at b708)
+Table TypeRef: 110 records (6 bytes, at b712)
+Table TypeDef: 26 records (14 bytes, at b9a6)
+Table Field: 210 records (6 bytes, at bb12)
+Table Method: 75 records (14 bytes, at bffe)
+Table Param: 74 records (6 bytes, at c418)
+Table MemberRef: 276 records (6 bytes, at c5d4)
+Table Constant: 110 records (6 bytes, at cc4c)
+Table CustomAttribute: 321 records (6 bytes, at cee0)
+Table ClassLayout: 1 records (8 bytes, at d666)
+Table StandaloneSig: 7 records (2 bytes, at d66e)
+Table TypeSpec: 47 records (2 bytes, at d67c)
+Table FieldRVA: 1 records (6 bytes, at d6da)
+Table Assembly: 1 records (22 bytes, at d6e0)
+Table AssemblyRef: 9 records (20 bytes, at d6f6)
+Table NestedClass: 7 records (4 bytes, at d7aa)
+Table MethodSpec: 21 records (4 bytes, at d7c6)
```

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/YAMS-LIB.pdb` & `am2r_yams-0.0.7/am2r_yams/yams/YAMS-LIB.pdb`

 * *Files 9% similar despite different names*

```diff
@@ -1,1353 +1,1375 @@
 00000000: 4253 4a42 0100 0100 0000 0000 0c00 0000  BSJB............
 00000010: 5044 4220 7631 2e30 0000 0000 0000 0600  PDB v1.0........
 00000020: 7c00 0000 6400 0000 2350 6462 0000 0000  |...d...#Pdb....
-00000030: e000 0000 540c 0000 237e 0000 340d 0000  ....T...#~..4...
-00000040: a805 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
-00000050: dc12 0000 0400 0000 2355 5300 e012 0000  ........#US.....
-00000060: 5000 0000 2347 5549 4400 0000 3013 0000  P...#GUID...0...
-00000070: 5441 0000 2342 6c6f 6200 0000 a2c5 929b  TA..#Blob.......
-00000080: 9c08 8e46 8485 8b98 c37c dc31 ed21 c9c1  ...F.....|.1.!..
+00000030: e000 0000 dc0c 0000 237e 0000 bc0d 0000  ........#~......
+00000040: c405 0000 2353 7472 696e 6773 0000 0000  ....#Strings....
+00000050: 8013 0000 0400 0000 2355 5300 8413 0000  ........#US.....
+00000060: 5000 0000 2347 5549 4400 0000 d413 0000  P...#GUID.......
+00000070: 1442 0000 2342 6c6f 6200 0000 ecc2 cd88  .B..#Blob.......
+00000080: e33e 604b bfe2 6e97 e80c 6b68 586b b6d1  .>`K..n...khXk..
 00000090: 0000 0000 579d 0228 090a 0000 0100 0000  ....W..(........
-000000a0: 6b00 0000 1800 0000 c900 0000 4700 0000  k...........G...
-000000b0: 4700 0000 0a01 0000 6e00 0000 3001 0000  G.......n...0...
-000000c0: 0100 0000 0600 0000 2b00 0000 0100 0000  ........+.......
-000000d0: 0100 0000 0900 0000 0600 0000 1400 0000  ................
+000000a0: 6e00 0000 1a00 0000 d200 0000 4b00 0000  n...........K...
+000000b0: 4a00 0000 1401 0000 6e00 0000 4101 0000  J.......n...A...
+000000c0: 0100 0000 0700 0000 2f00 0000 0100 0000  ......../.......
+000000d0: 0100 0000 0900 0000 0700 0000 1500 0000  ................
 000000e0: 0000 0000 0200 0001 0000 0000 0000 bf00  ................
-000000f0: 0000 0000 0000 8400 0500 0000 4700 0000  ............G...
-00000100: 7300 0000 8e00 0000 0400 0000 0500 0000  s...............
-00000110: 0800 0000 2b00 0100 3500 0200 6400 0100  ....+...5...d...
+000000f0: 0000 0000 0000 8400 0500 0000 4b00 0000  ............K...
+00000100: 7800 0000 9400 0000 0400 0000 0500 0000  x...............
+00000110: 0900 0000 2b00 0100 3500 0200 6400 0100  ....+...5...d...
 00000120: 6e00 0200 bd00 0100 ce00 0200 1e01 0100  n...............
 00000130: 2f01 0200 6901 0100 7a01 0200 0000 0000  /...i...z.......
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0100 7f27 0100 2b29 0000 0000 0100 1b3e  ...'..+).......>
-00000160: 0200 223e 0000 0000 0000 0000 0200 c53e  ..">...........>
-00000170: 0000 0000 0000 0000 0200 d23e 0200 da3e  ...........>...>
-00000180: 0200 e73e 0000 0000 0000 0000 0100 ef3e  ...>...........>
-00000190: 0100 f73e 0100 ff3e 0100 073f 0100 0f3f  ...>...>...?...?
-000001a0: 0100 173f 0100 1f3f 0100 273f 0100 2f3f  ...?...?..'?../?
-000001b0: 0100 373f 0100 3f3f 0100 473f 0100 4f3f  ..7?..??..G?..O?
-000001c0: 0100 573f 0100 603f 0100 683f 0100 713f  ..W?..`?..h?..q?
-000001d0: 0100 793f 0100 813f 0100 893f 0100 913f  ..y?...?...?...?
-000001e0: 0100 993f 0100 a13f 0100 a93f 0100 b13f  ...?...?...?...?
-000001f0: 0100 b93f 0100 c13f 0100 c93f 0100 d13f  ...?...?...?...?
-00000200: 0100 d93f 0100 e13f 0100 e93f 0100 f13f  ...?...?...?...?
-00000210: 0000 0000 0100 f93f 0100 0040 0100 2040  .......?...@.. @
-00000220: 0100 3640 0100 4c40 0100 5840 0100 6440  ..6@..L@..X@..d@
-00000230: 0100 7040 0100 1a41 0100 2241 0000 0000  ..p@...A.."A....
-00000240: 0100 2a41 0000 0000 0100 3241 0100 3a41  ..*A......2A..:A
-00000250: 0100 4241 0100 4a41 0600 0300 0100 0100  ..BA..JA........
-00000260: 0000 0000 6900 0000 0700 0300 0200 0100  ....i...........
-00000270: 0000 0000 8ca1 0000 0700 0300 3600 0500  ............6...
-00000280: 2800 0000 2b00 0000 0700 0300 3700 0500  (...+.......7...
-00000290: fa00 0000 4400 0000 0700 0300 3800 0500  ....D.......8...
-000002a0: 3e01 0000 0502 0000 0700 0300 3b00 0500  >...........;...
-000002b0: 0402 0000 4000 0000 0700 0300 3c00 0500  ....@.......<...
-000002c0: 0303 0000 4000 0000 0700 0300 3d00 0500  ....@.......=...
-000002d0: a63f 0000 4f00 0000 0700 0300 3e00 0500  .?..O.......>...
-000002e0: 3a41 0000 2500 0000 0700 0300 3f00 0500  :A..%.......?...
-000002f0: c542 0000 2500 0000 0700 0300 4000 0500  .B..%.......@...
-00000300: 3644 0000 2800 0000 0700 0300 4100 0500  6D..(.......A...
-00000310: 8c44 0000 4500 0000 0700 0300 4200 0500  .D..E.......B...
-00000320: 6945 0000 4500 0000 0700 0300 4300 0500  iE..E.......C...
-00000330: 8746 0000 2b00 0000 0700 0300 4400 0500  .F..+.......D...
-00000340: fd4b 0000 c801 0000 0700 0300 4500 0500  .K..........E...
-00000350: 094c 0000 aa01 0000 0700 0300 4a00 0500  .L..........J...
-00000360: fb4e 0000 2b00 0000 0700 0300 4b00 0500  .N..+.......K...
-00000370: 714f 0000 2b00 0000 0700 0300 4c00 0500  qO..+.......L...
-00000380: 0b51 0000 d50d 0000 0700 0300 5b00 0500  .Q..........[...
-00000390: 0167 0000 2b00 0000 0700 0300 5c00 0500  .g..+.......\...
-000003a0: a567 0000 2100 0000 0700 0300 5d00 0500  .g..!.......]...
-000003b0: 7868 0000 1c00 0000 0700 0300 5e00 0500  xh..........^...
-000003c0: 6e69 0000 1c00 0000 0700 0300 5f00 0500  ni.........._...
-000003d0: 0c6a 0000 2b00 0000 0700 0300 6000 0500  .j..+.......`...
-000003e0: a36a 0000 1c00 0000 0700 0300 6100 0500  .j..........a...
-000003f0: 346b 0000 1c00 0000 0700 0300 6200 0500  4k..........b...
-00000400: 2b6c 0000 2b00 0000 0700 0300 6300 0500  +l..+.......c...
-00000410: 166d 0000 2b00 0000 0700 0300 6400 0500  .m..+.......d...
-00000420: e06d 0000 2b00 0000 0700 0300 6500 0500  .m..+.......e...
-00000430: ec6f 0000 1b00 0000 0700 0300 6600 0500  .o..........f...
-00000440: d173 0000 2b00 0000 0700 0300 6700 0500  .s..+.......g...
-00000450: ee74 0000 cc06 0000 0700 0300 6800 0500  .t..........h...
-00000460: 3277 0000 3800 0000 0700 0300 6900 0500  2w..8.......i...
-00000470: 767e 0000 5304 0000 0700 0300 6b00 0500  v~..S.......k...
-00000480: 927e 0000 3704 0000 0700 0300 6c00 0500  .~..7.......l...
-00000490: ac7e 0000 c703 0000 0700 0300 6d00 0500  .~..........m...
-000004a0: c87e 0000 8b03 0000 0700 0300 6e00 0500  .~..........n...
-000004b0: d17e 0000 8203 0000 0700 0300 6f00 0500  .~..........o...
-000004c0: 437f 0000 8900 0000 0700 0300 7000 0500  C...........p...
-000004d0: f782 0000 8b03 0000 0700 0300 7200 0500  ............r...
-000004e0: 1383 0000 6f03 0000 0700 0300 7600 0500  ....o.......v...
-000004f0: 7b85 0000 2c00 0000 0700 0300 7700 0500  {...,.......w...
-00000500: a28b 0000 1600 0000 0700 0300 7800 0500  ............x...
-00000510: 1e8c 0000 2100 0000 0700 0300 7900 0500  ....!.......y...
-00000520: f98c 0000 2500 0000 0700 0300 7a00 0500  ....%.......z...
-00000530: 2c8d 0000 6000 0000 0700 0300 7b00 0500  ,...`.......{...
-00000540: 628e 0000 4900 0000 0700 0300 7c00 0500  b...I.......|...
-00000550: 0a8f 0000 3700 0000 0700 0300 7d00 0500  ....7.......}...
-00000560: a08f 0000 2100 0000 0700 0300 7e00 0500  ....!.......~...
-00000570: 2090 0000 3700 0000 0700 0300 7f00 0500   ...7...........
-00000580: b690 0000 4c00 0000 0700 0300 8000 0500  ....L...........
-00000590: 3691 0000 2b00 0000 0700 0300 8100 0500  6...+...........
-000005a0: 1592 0000 1001 0000 0700 0300 8200 0500  ................
-000005b0: 3192 0000 da00 0000 0700 0300 8300 0500  1...............
-000005c0: 7792 0000 8200 0000 0700 0300 8400 0500  w...............
-000005d0: a095 0000 5d00 0000 0700 0300 8500 0500  ....]...........
-000005e0: ba95 0000 4300 0000 0700 0300 8700 0500  ....C...........
-000005f0: 48a1 0000 4300 0000 0900 0300 8800 0500  H...C...........
-00000600: 0000 0000 0b00 0000 0a00 0500 8800 0500  ................
-00000610: 0000 0000 3300 0000 0d00 0500 8800 0500  ....3...........
-00000620: 0000 0000 1d00 0000 1000 0500 8800 0500  ................
-00000630: 0000 0000 1200 0000 1100 0500 8800 0500  ................
-00000640: 0000 0000 1d00 0000 1200 0500 8800 0500  ................
-00000650: 0000 0000 1200 0000 1500 0300 8800 0500  ................
-00000660: 0000 0000 0e00 0000 1600 0300 8800 0500  ................
-00000670: 0000 0000 0e00 0000 1700 0300 8800 0500  ................
-00000680: 0000 0000 0e00 0000 1800 0300 8800 0500  ................
-00000690: 0000 0000 0e00 0000 1900 0300 8800 0500  ................
-000006a0: 0000 0000 1d00 0000 1a00 0300 8800 0500  ................
-000006b0: 0000 0000 1a00 0000 1b00 0300 8800 0500  ................
-000006c0: 0000 0000 1a00 0000 1c00 0300 8800 0500  ................
-000006d0: 0000 0000 1a00 0000 1d00 0300 8800 0500  ................
-000006e0: 0000 0000 1d00 0000 1e00 0300 8800 0500  ................
-000006f0: 0000 0000 1d00 0000 1f00 0300 8800 0500  ................
-00000700: 0000 0000 1d00 0000 2000 0300 8800 0500  ........ .......
-00000710: 0000 0000 1d00 0000 2100 0300 8800 0500  ........!.......
-00000720: 0000 0000 4300 0000 2200 0300 8800 0500  ....C...".......
-00000730: 0000 0000 5a00 0000 2300 0300 8800 0500  ....Z...#.......
-00000740: 0000 0000 5a00 0000 2400 0300 8800 0500  ....Z...$.......
-00000750: 0000 0000 4300 0000 2500 0300 8800 0500  ....C...%.......
-00000760: 0000 0000 1600 0000 2600 0300 8800 0500  ........&.......
-00000770: 0000 0000 1b00 0000 2700 0300 8800 0500  ........'.......
-00000780: 0000 0000 1100 0000 2800 0300 8800 0500  ........(.......
-00000790: 0000 0000 1100 0000 2900 0300 8800 0500  ........).......
-000007a0: 0000 0000 1100 0000 2a00 0300 8800 0500  ........*.......
-000007b0: 0000 0000 1100 0000 2b00 0300 8800 0500  ........+.......
-000007c0: 0000 0000 1100 0000 2c00 0300 8800 0500  ........,.......
-000007d0: 0000 0000 1100 0000 2d00 0300 8800 0500  ........-.......
-000007e0: 0000 0000 1100 0000 2e00 0300 8800 0500  ................
-000007f0: 0000 0000 1100 0000 2f00 0300 8800 0500  ......../.......
-00000800: 0000 0000 1100 0000 3000 0300 8800 0500  ........0.......
-00000810: 0000 0000 1600 0000 3100 0300 8800 0500  ........1.......
-00000820: 0000 0000 1b00 0000 3200 0300 8800 0500  ........2.......
-00000830: 0000 0000 1b00 0000 3300 0300 8800 0500  ........3.......
-00000840: 0000 0000 1b00 0000 3400 0300 8800 0500  ........4.......
-00000850: 0000 0000 1b00 0000 3500 0300 8800 0500  ........5.......
-00000860: 0000 0000 1b00 0000 3700 0300 8800 0500  ........7.......
-00000870: 0000 0000 0e00 0000 3800 0300 8800 0500  ........8.......
-00000880: 0000 0000 8700 0000 3900 0300 8900 0500  ........9.......
-00000890: 0000 0000 2900 0000 3a00 0300 8a00 0500  ....)...:.......
-000008a0: 0000 0000 2900 0000 3b00 0300 8b00 0500  ....)...;.......
-000008b0: 0000 0000 0e00 0000 3c00 0300 8b00 0500  ........<.......
-000008c0: 0000 0000 8500 0000 3d00 0300 8b00 0500  ........=.......
-000008d0: 0000 0000 7700 0000 3e00 0300 8b00 0500  ....w...>.......
-000008e0: 0000 0000 7f02 0000 3e00 0300 8b00 0500  ........>.......
-000008f0: 0b00 0000 0b00 0000 3e00 0300 8c00 0500  ........>.......
-00000900: 2e00 0000 4302 0000 3e00 0300 8d00 0500  ....C...>.......
-00000910: 3200 0000 3f02 0000 3f00 0300 8f00 0500  2...?...?.......
-00000920: 0000 0000 1d00 0000 4000 0300 8f00 0500  ........@.......
-00000930: 0000 0000 1d00 0000 4200 0300 8f00 0500  ........B.......
-00000940: 0000 0000 2400 0000 4400 0300 8f00 0500  ....$...D.......
-00000950: 0000 0000 3900 0000 4500 0300 8f00 0500  ....9...E.......
-00000960: 0000 0000 3100 0000 4600 0300 8f00 0500  ....1...F.......
-00000970: 0000 0000 3900 0000 4700 0300 8f00 0500  ....9...G.......
-00000980: 0000 0000 3100 0000 0000 0000 9305 0000  ....1...........
-00000990: 0000 0100 0000 0100 c103 0000 0200 6402  ..............d.
-000009a0: 0000 0300 4102 0000 0400 0f03 0000 0500  ....A...........
-000009b0: 8304 0000 0600 7303 0000 0700 cc01 0000  ......s.........
-000009c0: 0800 9801 0000 0900 4f01 0000 0a00 3d05  ........O.....=.
-000009d0: 0000 0b00 e402 0000 0c00 2303 0000 0d00  ..........#.....
-000009e0: ef04 0000 0e00 1505 0000 0f00 4c03 0000  ............L...
-000009f0: 1000 3803 0000 1100 4800 0000 1200 5800  ..8.....H.....X.
-00000a00: 0000 1300 3500 0000 1400 fc01 0000 1500  ....5...........
-00000a10: 7704 0000 1600 f703 0000 1700 6403 0000  w...........d...
-00000a20: 1800 5f01 0000 1900 2100 0000 1a00 8702  .._.....!.......
-00000a30: 0000 1b00 6b01 0000 1c00 ea00 0000 1d00  ....k...........
-00000a40: d900 0000 1e00 3501 0000 1f00 7801 0000  ......5.....x...
-00000a50: 2000 c504 0000 2100 aa04 0000 2200 9604   .....!....."...
-00000a60: 0000 2300 db04 0000 2400 8503 0000 2500  ..#.....$.....%.
-00000a70: 2c05 0000 2600 4405 0000 2700 5605 0000  ,...&.D...'.V...
-00000a80: 2800 fc04 0000 2900 0502 0000 2a00 bc01  (.....).....*...
-00000a90: 0000 2b00 ac01 0000 2c00 5c02 0000 2d00  ..+.....,.\...-.
-00000aa0: b600 0000 2e00 af03 0000 2f00 a503 0000  ........../.....
-00000ab0: 3000 7505 0000 3100 8405 0000 3200 6805  0.u...1.....2.h.
-00000ac0: 0000 3300 0304 0000 3400 ac03 0000 3600  ..3.....4.....6.
-00000ad0: be03 0000 3700 1100 0000 3800 f001 0000  ....7.....8.....
-00000ae0: 3900 e301 0000 3a00 be03 0000 3b00 be03  9.....:.....;...
-00000af0: 0000 3d00 de01 0000 3e00 1202 0000 3f00  ..=.....>.....?.
-00000b00: 1202 0000 4000 1202 0000 4200 af00 0000  ....@.....B.....
-00000b10: 4400 af00 0000 4500 1202 0000 4700 7c02  D.....E.....G.|.
-00000b20: 0000 4800 7003 0000 4900 5502 0000 4a00  ..H.p...I.U...J.
-00000b30: 3103 0000 4b00 8f04 0000 4c00 f702 0000  1...K.....L.....
-00000b40: 4d00 3c02 0000 4e00 3c02 0000 4f00 c802  M.<...N.<...O...
-00000b50: 0000 5000 6404 0000 5100 1e04 0000 5200  ..P.d...Q.....R.
-00000b60: 4e04 0000 5300 3804 0000 5400 1004 0000  N...S.8...T.....
-00000b70: 5500 cc03 0000 5600 e303 0000 5700 2501  U.....V.....W.%.
-00000b80: 0000 5800 bb02 0000 5900 1801 0000 5a00  ..X.....Y.....Z.
-00000b90: 9902 0000 5b00 f600 0000 5c00 a802 0000  ....[.....\.....
-00000ba0: 5d00 0501 0000 6000 de01 0000 6400 7003  ].....`.....d.p.
-00000bb0: 0000 6600 de01 0000 6700 de01 0000 6800  ..f.....g.....h.
-00000bc0: de01 0000 6900 de01 0000 6a00 de01 0000  ....i.....j.....
-00000bd0: 6b00 de01 0000 6c00 de01 0000 6d00 de01  k.....l.....m...
-00000be0: 0000 6e00 df02 0000 6f00 de01 0000 7100  ..n.....o.....q.
-00000bf0: 9c05 0000 7400 9105 0000 7600 be00 0000  ....t.....v.....
-00000c00: 7700 7e02 0000 7a00 c100 0000 7b00 df02  w.~...z.....{...
-00000c10: 0000 7c00 d803 0000 7d00 0c05 0000 7e00  ..|.....}.....~.
-00000c20: de01 0000 8200 3102 0000 8300 9703 0000  ......1.........
-00000c30: 8600 ee03 0000 8700 4401 0000 8800 8a01  ........D.......
-00000c40: 0000 8900 c700 0000 8a00 9105 0000 8b00  ................
-00000c50: de01 0000 8c00 7003 0000 8d00 1202 0000  ......p.........
-00000c60: 8e00 7c02 0000 8f00 d803 0000 9000 d803  ..|.............
-00000c70: 0000 9100 d803 0000 9200 d803 0000 9300  ................
-00000c80: d803 0000 9400 1202 0000 9500 df02 0000  ................
-00000c90: 9600 7003 0000 9700 de01 0000 9a00 1b02  ..p.............
-00000ca0: 0000 9d00 2802 0000 9e00 d802 0000 9f00  ....(...........
-00000cb0: ac03 0000 0000 0c05 0000 0000 0c05 0000  ................
-00000cc0: 0000 0c05 0000 0200 9e03 0000 0300 7302  ..............s.
-00000cd0: 0000 0400 0100 0000 0500 9002 6900 033e  ............i..>
-00000ce0: 9800 093e 7f00 0f3e 0103 153e 0000 0000  ...>...>...>....
-00000cf0: 0100 f728 0200 0000 0100 9a3e 0400 0000  ...(.......>....
-00000d00: 2700 0400 9d01 2700 0500 c303 0301 0300  '.....'.........
-00000d10: 9b01 2301 0300 9b01 4301 0300 9b01 8301  ..#.....C.......
-00000d20: 0300 9b01 a301 0300 9b01 c301 0300 9b01  ................
-00000d30: 0000 0000 0043 5324 3c3e 385f 5f6c 6f63  .....CS$<>8__loc
-00000d40: 616c 7330 0043 5324 3c3e 385f 5f6c 6f63  als0.CS$<>8__loc
-00000d50: 616c 7331 006f 7074 696f 6e73 4469 7370  als1.optionsDisp
-00000d60: 6c61 7955 7365 7232 0077 6174 6572 5475  layUser2.waterTu
-00000d70: 7262 696e 6544 6f6f 7243 4300 7468 6f74  rbineDoorCC.thot
-00000d80: 684c 6566 7444 6f6f 7243 4300 7468 6f74  hLeftDoorCC.thot
-00000d90: 6852 6967 6874 446f 6f72 4343 0054 686f  hRightDoorCC.Tho
-00000da0: 7468 4272 6964 6765 4c65 6674 446f 6f72  thBridgeLeftDoor
-00000db0: 4944 0041 3257 6174 6572 5475 7262 696e  ID.A2WaterTurbin
-00000dc0: 654c 6566 7444 6f6f 7249 4400 5468 6f74  eLeftDoorID.Thot
-00000dd0: 6842 7269 6467 6552 6967 6874 446f 6f72  hBridgeRightDoor
-00000de0: 4944 0064 6f6f 7249 4400 7376 366c 6f61  ID.doorID.sv6loa
-00000df0: 6400 6964 0066 6f75 6e64 0063 6f6c 6c69  d.id.found.colli
-00000e00: 7369 6f6e 436f 6465 546f 4265 0073 686f  sionCodeToBe.sho
-00000e10: 6f74 4d69 7373 696c 6543 6f64 6500 6e65  otMissileCode.ne
-00000e20: 7747 616d 6543 6f64 6500 6465 7074 6873  wGameCode.depths
-00000e30: 5069 7065 436f 6465 0077 6174 6572 6661  PipeCode.waterfa
-00000e40: 6c6c 7350 6970 6543 6f64 6500 6e65 7374  llsPipeCode.nest
-00000e50: 5069 7065 436f 6465 0068 6964 656f 7574  PipeCode.hideout
-00000e60: 5069 7065 436f 6465 0063 6853 7465 7046  PipeCode.chStepF
-00000e70: 6972 6543 6f64 6500 6372 6561 7465 436f  ireCode.createCo
-00000e80: 6465 0075 6e6c 6f63 6b53 7475 6666 436f  de.unlockStuffCo
-00000e90: 6465 0064 7261 7747 7569 436f 6465 006c  de.drawGuiCode.l
-00000ea0: 6162 426c 6f63 6b43 6f64 6500 6368 5374  abBlockCode.chSt
-00000eb0: 6570 436f 6e74 726f 6c43 6f64 6500 636f  epControlCode.co
-00000ec0: 6c6c 6973 696f 6e43 6f64 6500 6761 6d65  llisionCode.game
-00000ed0: 5365 6c4d 656e 7553 7465 7043 6f64 6500  SelMenuStepCode.
-00000ee0: 6c6f 6164 476c 6f62 616c 7343 6f64 6500  loadGlobalsCode.
-00000ef0: 7361 7665 476c 6f62 616c 7343 6f64 6500  saveGlobalsCode.
-00000f00: 6368 6172 6163 7465 7256 6172 7343 6f64  characterVarsCod
-00000f10: 6500 636f 6465 0061 3450 6167 6532 496d  e.code.a4Page2Im
-00000f20: 6167 6500 6134 5061 6765 496d 6167 6500  age.a4PageImage.
-00000f30: 7465 6d70 5469 6c65 0073 7461 7274 4e65  tempTile.startNe
-00000f40: 7747 616d 6500 636f 6465 4e61 6d65 0069  wGame.codeName.i
-00000f50: 6e74 6572 6e61 6c4e 616d 6500 726f 6f6d  nternalName.room
-00000f60: 4e61 6d65 0070 6963 6b75 704e 616d 6500  Name.pickupName.
-00000f70: 6e61 6d65 0077 6973 646f 6d53 6570 746f  name.wisdomSepto
-00000f80: 6767 4372 6561 7465 0063 7265 6174 6500  ggCreate.create.
-00000f90: 7376 3653 6176 6500 6f57 6973 646f 6d53  sv6Save.oWisdomS
-00000fa0: 6570 746f 6767 0066 696c 6550 6174 6800  eptogg.filePath.
-00000fb0: 6900 646f 6f72 4c6f 636b 006c 6162 426c  i.doorLock.labBl
-00000fc0: 6f63 6b00 7061 6765 4974 656d 0064 6570  ock.pageItem.dep
-00000fd0: 7468 7350 6970 6552 6f6f 6d00 7761 7465  thsPipeRoom.wate
-00000fe0: 7266 616c 6c73 5069 7065 526f 6f6d 006e  rfallsPipeRoom.n
-00000ff0: 6573 7450 6970 6552 6f6f 6d00 6869 6465  estPipeRoom.hide
-00001000: 6f75 7450 6970 6552 6f6f 6d00 676d 526f  outPipeRoom.gmRo
-00001010: 6f6d 0072 6f6f 6d00 646f 6f72 5361 6d75  om.room.doorSamu
-00001020: 7343 6f6c 6c69 7369 6f6e 0063 6f6c 6c69  sCollision.colli
-00001030: 7369 6f6e 0070 6167 6544 696d 656e 7369  sion.pageDimensi
-00001040: 6f6e 0077 6973 646f 6d53 6570 746f 6767  on.wisdomSeptogg
-00001050: 4163 7469 6f6e 0076 6172 446f 6f72 4163  Action.varDoorAc
-00001060: 7469 6f6e 0061 6374 696f 6e00 6135 4163  tion.action.a5Ac
-00001070: 7469 7661 7465 436f 6e64 6974 696f 6e00  tivateCondition.
-00001080: 656d 7042 6174 7465 7279 4365 6c6c 436f  empBatteryCellCo
-00001090: 6e64 6974 696f 6e00 7363 7244 4e41 5370  ndition.scrDNASp
-000010a0: 6177 6e00 676f 0077 6973 646f 6d53 6570  awn.go.wisdomSep
-000010b0: 746f 6767 5374 6570 0073 7562 7363 7265  toggStep.subscre
-000010c0: 656e 4d65 6e75 5374 6570 0070 6963 6b75  enMenuStep.picku
-000010d0: 7000 7375 6244 6972 0061 3544 6f6f 7200  p.subDir.a5Door.
-000010e0: 6673 0073 7636 6c6f 6164 4465 7461 696c  fs.sv6loadDetail
-000010f0: 7300 6d73 0073 6565 644f 626a 6563 7400  s.ms.seedObject.
-00001100: 736f 6c69 644f 626a 6563 7400 6761 6d65  solidObject.game
-00001110: 4f62 6a65 6374 0070 6970 654f 626a 6563  Object.pipeObjec
-00001120: 7400 676d 4f62 6a65 6374 0065 6e65 6d79  t.gmObject.enemy
-00001130: 4f62 6a65 6374 0065 7461 6e6b 536e 6970  Object.etankSnip
-00001140: 7065 7400 7069 7065 4247 5469 6c65 7365  pet.pipeBGTilese
-00001150: 7400 6465 7074 6873 456e 7472 616e 6365  t.depthsEntrance
-00001160: 5069 7065 5469 6c65 7365 7400 7761 7465  PipeTileset.wate
-00001170: 7266 616c 6c73 5069 7065 5469 6c65 7365  rfallsPipeTilese
-00001180: 7400 6465 7074 6873 4578 6974 5069 7065  t.depthsExitPipe
-00001190: 5469 6c65 7365 7400 6869 6465 6f75 7450  Tileset.hideoutP
-000011a0: 6970 6554 696c 6573 6574 0064 6f6f 7254  ipeTileset.doorT
-000011b0: 696c 6573 6574 0077 6973 646f 6d53 6570  ileset.wisdomSep
-000011c0: 746f 6767 4576 656e 7400 7042 6f6d 6243  toggEvent.pBombC
-000011d0: 6861 7261 6374 6572 4576 656e 7400 7375  haracterEvent.su
-000011e0: 7065 724d 6973 7369 6c65 4368 6172 6163  perMissileCharac
-000011f0: 7465 7245 7665 6e74 006d 6973 7369 6c65  terEvent.missile
-00001200: 4368 6172 6163 7465 7245 7665 6e74 0065  CharacterEvent.e
-00001210: 5461 6e6b 4368 6172 6163 7465 7245 7665  TankCharacterEve
-00001220: 6e74 0076 6172 446f 6f72 4576 656e 7400  nt.varDoorEvent.
-00001230: 6974 656d 7353 7761 7053 6372 6970 7400  itemsSwapScript.
-00001240: 636f 6465 5465 7874 006e 6577 446f 6f72  codeText.newDoor
-00001250: 5265 706c 6163 656d 656e 7454 6578 7400  ReplacementText.
-00001260: 7375 6273 6372 6565 6e4d 6973 6344 6177  subscreenMiscDaw
-00001270: 0073 7344 7261 7700 7375 6263 7265 656e  .ssDraw.subcreen
-00001280: 426f 6f74 7344 7261 7700 7375 6273 6372  BootsDraw.subscr
-00001290: 6565 6e53 7569 7444 7261 7700 6472 6177  eenSuitDraw.draw
-000012a0: 456e 6449 6e64 6578 0064 6f6f 7245 7665  EndIndex.doorEve
-000012b0: 6e74 496e 6465 7800 6472 6177 5374 6172  ntIndex.drawStar
-000012c0: 7449 6e64 6578 0061 7373 656d 626c 7900  tIndex.assembly.
-000012d0: 7175 616e 7469 7479 0000 0000 0000 0000  quantity........
-000012e0: 0fd0 2988 b811 1342 878b 770e 8597 ac16  ..)....B..w.....
-000012f0: f862 513f c607 d311 9053 00c0 4fa3 02a1  .bQ?.....S..O...
-00001300: bc74 2e93 a9db 7844 8d46 0f32 a7ba b3d3  .t....xD.F.2....
-00001310: 05ec feb5 d08c 834a 96da 4662 84bb 4bd8  .......J..Fb..K.
-00001320: 0847 4d7e 6e09 5c4c aeda cb10 ba6a 740d  .GM~n.\L.....jt.
-00001330: 0004 686f 6d65 0672 756e 6e65 7204 776f  ..home.runner.wo
-00001340: 726b 0459 414d 5308 5941 4d53 2d4c 4942  rk.YAMS.YAMS-LIB
-00001350: 0a50 726f 6772 616d 2e63 7309 2f00 0106  .Program.cs./...
-00001360: 0d12 1217 2020 fcd7 b607 0947 2a7f 005f  ....  .....G*.._
-00001370: d4dc 8bfa 96be 9c69 7aa0 808c d517 10d9  .......iz.......
-00001380: d077 717a 270f 0d53 6565 644f 626a 6563  .wqz'..SeedObjec
-00001390: 742e 6373 092f 0001 060d 1212 1756 2056  t.cs./.......V V
-000013a0: 65af b720 c3e8 22d1 155a 7563 de4b a863  e.. .."..Zuc.K.c
-000013b0: e3cc 373b 3f57 25d2 3772 9abe a3a6 0a03  ..7;?W%.7r......
-000013c0: 6f62 6a07 5265 6c65 6173 6506 6e65 7436  obj.Release.net6
-000013d0: 2e30 1a59 414d 532d 4c49 422e 476c 6f62  .0.YAMS-LIB.Glob
-000013e0: 616c 5573 696e 6773 2e67 2e63 7310 2f00  alUsings.g.cs./.
-000013f0: 0106 0d12 1217 808f 8093 809b 80a2 205d  .............. ]
-00001400: d6d5 28fd d6c4 4688 4302 02cd 32e6 b714  ..(...F.C...2...
-00001410: 4a8a ec9d fc9f 674a 11e9 0331 1930 c42e  J.....gJ...1.0..
-00001420: 2e4e 4554 436f 7265 4170 702c 5665 7273  .NETCoreApp,Vers
-00001430: 696f 6e3d 7636 2e30 2e41 7373 656d 626c  ion=v6.0.Assembl
-00001440: 7941 7474 7269 6275 7465 732e 6373 102f  yAttributes.cs./
-00001450: 0001 060d 1212 1780 8f80 9380 9b80 ef20  ............... 
-00001460: 7897 e595 3cb5 cd51 3150 9b35 0421 8634  x...<..Q1P.5.!.4
-00001470: c24b 9ce7 a68b 984f fb5a 1668 6eb5 af5c  .K.....O.Z.hn..\
-00001480: 1859 414d 532d 4c49 422e 4173 7365 6d62  .YAMS-LIB.Assemb
-00001490: 6c79 496e 666f 2e63 7310 2f00 0106 0d12  lyInfo.cs./.....
-000014a0: 1217 808f 8093 809b 8150 20cc 01c3 8551  .........P ....Q
-000014b0: b3bd 617f 9461 cb0e 2e52 f6be 28c1 0771  ..a..a...R..(..q
-000014c0: e665 5b7d cc0f f0b6 ef7b 0701 0282 2476  .e[}.....{....$v
-000014d0: 6572 7369 6f6e 0032 0063 6f6d 7069 6c65  ersion.2.compile
-000014e0: 722d 7665 7273 696f 6e00 342e 362e 302d  r-version.4.6.0-
-000014f0: 332e 3233 3235 392e 382b 6333 6363 3164  3.23259.8+c3cc1d
-00001500: 3063 6565 6162 3161 3635 6461 3032 3137  0ceeab1a65da0217
-00001510: 6534 3033 3835 3161 3165 3861 3330 3038  e403851a1e8a3008
-00001520: 3661 006c 616e 6775 6167 6500 4323 0073  6a.language.C#.s
-00001530: 6f75 7263 652d 6669 6c65 2d63 6f75 6e74  ource-file-count
-00001540: 0035 006f 7574 7075 742d 6b69 6e64 0044  .5.output-kind.D
-00001550: 796e 616d 6963 616c 6c79 4c69 6e6b 6564  ynamicallyLinked
-00001560: 4c69 6272 6172 7900 6f70 7469 6d69 7a61  Library.optimiza
-00001570: 7469 6f6e 0072 656c 6561 7365 0070 6c61  tion.release.pla
-00001580: 7466 6f72 6d00 416e 7943 7075 0072 756e  tform.AnyCpu.run
-00001590: 7469 6d65 2d76 6572 7369 6f6e 0037 2e30  time-version.7.0
-000015a0: 2e39 2b38 6539 6131 3762 3232 3136 6635  .9+8e9a17b2216f5
-000015b0: 3161 3537 3838 6638 6231 6334 3637 6134  1a5788f8b1c467a4
-000015c0: 6366 3362 3736 3965 3764 3700 6c61 6e67  cf3b769e7d7.lang
-000015d0: 7561 6765 2d76 6572 7369 6f6e 0070 7265  uage-version.pre
-000015e0: 7669 6577 006e 756c 6c61 626c 6500 456e  view.nullable.En
-000015f0: 6162 6c65 0064 6566 696e 6500 5452 4143  able.define.TRAC
-00001600: 452c 5245 4c45 4153 452c 4e45 542c 4e45  E,RELEASE,NET,NE
-00001610: 5436 5f30 2c4e 4554 434f 5245 4150 502c  T6_0,NETCOREAPP,
-00001620: 4e45 5435 5f30 5f4f 525f 4752 4541 5445  NET5_0_OR_GREATE
-00001630: 522c 4e45 5436 5f30 5f4f 525f 4752 4541  R,NET6_0_OR_GREA
-00001640: 5445 522c 4e45 5443 4f52 4541 5050 315f  TER,NETCOREAPP1_
-00001650: 305f 4f52 5f47 5245 4154 4552 2c4e 4554  0_OR_GREATER,NET
-00001660: 434f 5245 4150 5031 5f31 5f4f 525f 4752  COREAPP1_1_OR_GR
-00001670: 4541 5445 522c 4e45 5443 4f52 4541 5050  EATER,NETCOREAPP
-00001680: 325f 305f 4f52 5f47 5245 4154 4552 2c4e  2_0_OR_GREATER,N
-00001690: 4554 434f 5245 4150 5032 5f31 5f4f 525f  ETCOREAPP2_1_OR_
-000016a0: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
-000016b0: 5050 325f 325f 4f52 5f47 5245 4154 4552  PP2_2_OR_GREATER
-000016c0: 2c4e 4554 434f 5245 4150 5033 5f30 5f4f  ,NETCOREAPP3_0_O
-000016d0: 525f 4752 4541 5445 522c 4e45 5443 4f52  R_GREATER,NETCOR
-000016e0: 4541 5050 335f 315f 4f52 5f47 5245 4154  EAPP3_1_OR_GREAT
-000016f0: 4552 00a3 ba49 4353 6861 7270 436f 6465  ER...ICSharpCode
-00001700: 2e53 6861 7270 5a69 704c 6962 2e64 6c6c  .SharpZipLib.dll
-00001710: 0000 016c 9904 9800 8003 0087 d282 16a4  ...l............
-00001720: 95d1 4abd 3f1f c402 13b4 ed4d 6163 726f  ..J.?......Macro
-00001730: 7373 2e4a 736f 6e2e 4578 7465 6e73 696f  ss.Json.Extensio
-00001740: 6e73 2e64 6c6c 0000 0155 c478 ba00 0001  ns.dll...U.x....
-00001750: 00b2 09ba d9ca d5dc 4e93 a42a 22b1 17ec  ........N..*"...
-00001760: 344d 6963 726f 736f 6674 2e43 5368 6172  4Microsoft.CShar
-00001770: 702e 646c 6c00 0001 0749 52d7 0080 0000  p.dll....IR.....
-00001780: 17e1 8671 93a1 9e42 a11d 4bf1 cb94 691c  ...q...B..K...i.
-00001790: 4d69 6372 6f73 6f66 742e 5669 7375 616c  Microsoft.Visual
-000017a0: 4261 7369 632e 436f 7265 2e64 6c6c 0000  Basic.Core.dll..
-000017b0: 01fd f562 8500 2001 0008 ae07 b107 183f  ...b.. ........?
-000017c0: 4282 f29e 3548 56b3 9f4d 6963 726f 736f  B...5HV..Microso
-000017d0: 6674 2e56 6973 7561 6c42 6173 6963 2e64  ft.VisualBasic.d
-000017e0: 6c6c 0000 019a 0054 d700 8000 00a8 a4e9  ll.....T........
-000017f0: c9a3 ffc3 4aae 82d9 bfb4 281d 754d 6963  ....J.....(.uMic
-00001800: 726f 736f 6674 2e57 696e 3332 2e50 7269  rosoft.Win32.Pri
-00001810: 6d69 7469 7665 732e 646c 6c00 0001 66d5  mitives.dll...f.
-00001820: 2dfc 0080 0000 e73e d1c6 4da4 f344 8f16  -......>..M..D..
-00001830: 2586 5dd6 7d54 4d69 6372 6f73 6f66 742e  %.].}TMicrosoft.
-00001840: 5769 6e33 322e 5265 6769 7374 7279 2e64  Win32.Registry.d
-00001850: 6c6c 0000 0161 b328 9f00 a000 007a 4531  ll...a.(.....zE1
-00001860: 5af2 af1d 489d 9445 67ef 8b8b 1e6d 7363  Z...H..Eg....msc
-00001870: 6f72 6c69 622e 646c 6c00 0001 cdd0 f4f6  orlib.dll.......
-00001880: 0020 0100 fcaf 6eca 8e72 524a bf2b 9464  . ....n..rRJ.+.d
-00001890: ddc5 4cef 6e65 7473 7461 6e64 6172 642e  ..L.netstandard.
-000018a0: 646c 6c00 0001 2f8c b0fe 00c0 0100 faf8  dll.../.........
-000018b0: f92e a718 f040 8eb8 58ce cd30 4898 5072  .....@..X..0H.Pr
-000018c0: 6f70 6572 7479 4368 616e 6765 642e 646c  opertyChanged.dl
-000018d0: 6c00 0001 8b5a 978a 0080 0000 3174 ff35  l....Z......1t.5
-000018e0: d3a6 344c 90ea 21b0 de57 7fe0 5369 784c  ..4L..!..W..SixL
-000018f0: 6162 6f72 732e 496d 6167 6553 6861 7270  abors.ImageSharp
-00001900: 2e64 6c6c 0000 016c 8a3e dd00 601f 007f  .dll...l.>..`...
-00001910: 776a e7b5 74d7 4aaa 9d41 db13 6c03 4353  wj..t.J..A..l.CS
-00001920: 7973 7465 6d2e 4170 7043 6f6e 7465 7874  ystem.AppContext
-00001930: 2e64 6c6c 0000 0170 94a2 e200 8000 0025  .dll...p.......%
-00001940: 2e6c 6fa8 98f6 4d8c 7a65 cb60 d06b d753  .lo...M.ze.`.k.S
-00001950: 7973 7465 6d2e 4275 6666 6572 732e 646c  ystem.Buffers.dl
-00001960: 6c00 0001 4862 a3da 0080 0000 b7aa 5ee8  l...Hb........^.
-00001970: 37bf c340 a7a9 80fb 3588 0655 5379 7374  7..@....5..USyst
-00001980: 656d 2e43 6f6c 6c65 6374 696f 6e73 2e43  em.Collections.C
-00001990: 6f6e 6375 7272 656e 742e 646c 6c00 0001  oncurrent.dll...
-000019a0: 801f 71e1 00a0 0000 9df2 9458 7ad0 f54d  ..q........Xz..M
-000019b0: 89ee e2ea 7478 52a8 5379 7374 656d 2e43  ....txR.System.C
-000019c0: 6f6c 6c65 6374 696f 6e73 2e64 6c6c 0000  ollections.dll..
-000019d0: 0189 c9a8 ca00 0001 0048 1fec 5634 526b  .........H..V4Rk
-000019e0: 4082 f7a3 b914 aaec c953 7973 7465 6d2e  @........System.
-000019f0: 436f 6c6c 6563 7469 6f6e 732e 496d 6d75  Collections.Immu
-00001a00: 7461 626c 652e 646c 6c00 0001 7a6e d5f0  table.dll...zn..
-00001a10: 0040 0100 3840 68b9 d79c 9746 8218 e630  .@..8@h....F...0
-00001a20: 2acc ca10 5379 7374 656d 2e43 6f6c 6c65  *...System.Colle
-00001a30: 6374 696f 6e73 2e4e 6f6e 4765 6e65 7269  ctions.NonGeneri
-00001a40: 632e 646c 6c00 0001 d8e6 4cac 00a0 0000  c.dll.....L.....
-00001a50: d21c c278 ed7e a648 858e 03c2 f6be df33  ...x.~.H.......3
-00001a60: 5379 7374 656d 2e43 6f6c 6c65 6374 696f  System.Collectio
-00001a70: 6e73 2e53 7065 6369 616c 697a 6564 2e64  ns.Specialized.d
-00001a80: 6c6c 0000 019c fa3c d300 a000 0023 9f8f  ll.....<.....#..
-00001a90: 8a45 230e 44b8 cc5f c180 b6bf c653 7973  .E#.D.._.....Sys
-00001aa0: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
-00001ab0: 656c 2e41 6e6e 6f74 6174 696f 6e73 2e64  el.Annotations.d
-00001ac0: 6c6c 0000 01be 614b ec00 c000 0055 a438  ll....aK.....U.8
-00001ad0: af72 c4c4 4e90 86bc 1224 07f2 eb53 7973  .r..N....$...Sys
-00001ae0: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
-00001af0: 656c 2e44 6174 6141 6e6e 6f74 6174 696f  el.DataAnnotatio
-00001b00: 6e73 2e64 6c6c 0000 0184 683a fe00 8000  ns.dll....h:....
-00001b10: 0005 d0f9 02c1 73b8 4b89 44c0 7c3c 00f1  ......s.K.D.|<..
-00001b20: ab53 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
-00001b30: 744d 6f64 656c 2e64 6c6c 0000 014e 2422  tModel.dll...N$"
-00001b40: 8700 8000 00e9 ad6e e8bd 5995 4ea9 e15c  .......n..Y.N..\
-00001b50: 5c7c a0bd 0353 7973 7465 6d2e 436f 6d70  \|...System.Comp
-00001b60: 6f6e 656e 744d 6f64 656c 2e45 7665 6e74  onentModel.Event
-00001b70: 4261 7365 6441 7379 6e63 2e64 6c6c 0000  BasedAsync.dll..
-00001b80: 01e2 a443 9700 8000 00fd e5d9 3533 23ce  ...C........53#.
-00001b90: 4081 038b a246 c95b d253 7973 7465 6d2e  @....F.[.System.
-00001ba0: 436f 6d70 6f6e 656e 744d 6f64 656c 2e50  ComponentModel.P
-00001bb0: 7269 6d69 7469 7665 732e 646c 6c00 0001  rimitives.dll...
-00001bc0: 4296 8faf 00a0 0000 f190 fdcb 2f09 1540  B.........../..@
-00001bd0: b5ed 6b66 648c ea66 5379 7374 656d 2e43  ..kfd..fSystem.C
-00001be0: 6f6d 706f 6e65 6e74 4d6f 6465 6c2e 5479  omponentModel.Ty
-00001bf0: 7065 436f 6e76 6572 7465 722e 646c 6c00  peConverter.dll.
-00001c00: 0001 78b1 0aa1 00c0 0100 f5c9 711b 41c1  ..x.........q.A.
-00001c10: 2b4f a387 838a 4ca9 04c5 5379 7374 656d  +O....L...System
-00001c20: 2e43 6f6e 6669 6775 7261 7469 6f6e 2e64  .Configuration.d
-00001c30: 6c6c 0000 0142 606d 9700 8000 0047 fc59  ll...B`m.....G.Y
-00001c40: 3fb8 f598 4bb7 c800 e5d4 fe5d 2853 7973  ?...K......](Sys
-00001c50: 7465 6d2e 436f 6e73 6f6c 652e 646c 6c00  tem.Console.dll.
-00001c60: 0001 c631 eba4 00a0 0000 01fb ca4e 49e4  ...1.........NI.
-00001c70: fd47 8ba7 a6a6 0d03 5401 5379 7374 656d  .G......T.System
-00001c80: 2e43 6f72 652e 646c 6c00 0001 0f44 62a6  .Core.dll....Db.
-00001c90: 00a0 0000 1145 5732 5df8 7844 88f9 180f  .....EW2].xD....
-00001ca0: b7c6 af61 5379 7374 656d 2e44 6174 612e  ...aSystem.Data.
-00001cb0: 436f 6d6d 6f6e 2e64 6c6c 0000 0171 db86  Common.dll...q..
-00001cc0: f800 8002 0070 101f 3c3b 13f1 42a8 564f  .....p..<;..B.VO
-00001cd0: 2861 4a19 ac53 7973 7465 6d2e 4461 7461  (aJ..System.Data
-00001ce0: 2e44 6174 6153 6574 4578 7465 6e73 696f  .DataSetExtensio
-00001cf0: 6e73 2e64 6c6c 0000 01d9 8f9f bf00 8000  ns.dll..........
-00001d00: 00a0 76e7 b0b2 20f3 4c91 083a bbe6 ac79  ..v... .L..:...y
-00001d10: ef53 7973 7465 6d2e 4461 7461 2e64 6c6c  .System.Data.dll
-00001d20: 0000 010c 4483 9e00 a000 002d 7ff2 3276  ....D......-..2v
-00001d30: 1ae6 44ae 9eb3 76fe e7e2 dc53 7973 7465  ..D...v....Syste
-00001d40: 6d2e 4469 6167 6e6f 7374 6963 732e 436f  m.Diagnostics.Co
-00001d50: 6e74 7261 6374 732e 646c 6c00 0001 b13e  ntracts.dll....>
-00001d60: 63fc 0080 0000 276b 11c6 c4f0 2544 b417  c.....'k....%D..
-00001d70: 4af0 15a4 eb81 5379 7374 656d 2e44 6961  J.....System.Dia
-00001d80: 676e 6f73 7469 6373 2e44 6562 7567 2e64  gnostics.Debug.d
-00001d90: 6c6c 0000 01ed 49cb f400 8000 004b 9eb6  ll....I......K..
-00001da0: 499b 2776 4cae b41c 2924 2a3e e553 7973  I.'vL...)$*>.Sys
-00001db0: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
-00001dc0: 4469 6167 6e6f 7374 6963 536f 7572 6365  DiagnosticSource
-00001dd0: 2e64 6c6c 0000 018c f22c f800 c000 0031  .dll.....,.....1
-00001de0: 3552 2d2c 67e3 4487 e849 98de 1554 b053  5R-,g.D..I...T.S
-00001df0: 7973 7465 6d2e 4469 6167 6e6f 7374 6963  ystem.Diagnostic
-00001e00: 732e 4669 6c65 5665 7273 696f 6e49 6e66  s.FileVersionInf
-00001e10: 6f2e 646c 6c00 0001 5fe3 fcf2 0080 0000  o.dll..._.......
-00001e20: 4d91 ef25 cb82 d040 b004 9607 0811 7076  M..%...@......pv
-00001e30: 5379 7374 656d 2e44 6961 676e 6f73 7469  System.Diagnosti
-00001e40: 6373 2e50 726f 6365 7373 2e64 6c6c 0000  cs.Process.dll..
-00001e50: 0128 cad2 b200 c000 007d 9733 70f0 bac2  .(.......}.3p...
-00001e60: 45a1 fa60 16b0 497e 2353 7973 7465 6d2e  E..`..I~#System.
-00001e70: 4469 6167 6e6f 7374 6963 732e 5374 6163  Diagnostics.Stac
-00001e80: 6b54 7261 6365 2e64 6c6c 0000 0135 fff9  kTrace.dll...5..
-00001e90: b200 a000 00ad 5f8a 71cb 64c7 459c 731d  ......_.q.d.E.s.
-00001ea0: 01da b22d 7953 7973 7465 6d2e 4469 6167  ...-ySystem.Diag
-00001eb0: 6e6f 7374 6963 732e 5465 7874 5772 6974  nostics.TextWrit
-00001ec0: 6572 5472 6163 654c 6973 7465 6e65 722e  erTraceListener.
-00001ed0: 646c 6c00 0001 5a50 95c4 0080 0000 88d5  dll...ZP........
-00001ee0: 8bd4 95e2 d24b 94d5 f302 b798 1df6 5379  .....K........Sy
-00001ef0: 7374 656d 2e44 6961 676e 6f73 7469 6373  stem.Diagnostics
-00001f00: 2e54 6f6f 6c73 2e64 6c6c 0000 01a0 613c  .Tools.dll....a<
-00001f10: fe00 8000 00cc 118d eff1 3cf0 42a5 309f  ..........<.B.0.
-00001f20: 6b00 7903 fb53 7973 7465 6d2e 4469 6167  k.y..System.Diag
-00001f30: 6e6f 7374 6963 732e 5472 6163 6553 6f75  nostics.TraceSou
-00001f40: 7263 652e 646c 6c00 0001 66d5 d884 00a0  rce.dll...f.....
-00001f50: 0000 5722 142a d78a e144 b398 42db 6ad1  ..W".*...D..B.j.
-00001f60: b885 5379 7374 656d 2e44 6961 676e 6f73  ..System.Diagnos
-00001f70: 7469 6373 2e54 7261 6369 6e67 2e64 6c6c  tics.Tracing.dll
-00001f80: 0000 016e 9980 de00 a000 00e8 77f8 d4fb  ...n........w...
-00001f90: 6360 43aa 5057 a2c1 5c08 9553 7973 7465  c`C.PW..\..Syste
-00001fa0: 6d2e 646c 6c00 0001 1b34 e8f0 0000 0100  m.dll....4......
-00001fb0: 042d f79f 0ace ff43 9292 a2bb 74fc e9ac  .-.....C....t...
-00001fc0: 5379 7374 656d 2e44 7261 7769 6e67 2e43  System.Drawing.C
-00001fd0: 6f6d 6d6f 6e2e 646c 6c00 0001 218d 42d5  ommon.dll...!.B.
-00001fe0: 0020 0200 0843 fec0 6a78 bb46 9f62 dc8a  . ...C..jx.F.b..
-00001ff0: c5b5 5abc 5379 7374 656d 2e44 7261 7769  ..Z.System.Drawi
-00002000: 6e67 2e64 6c6c 0000 012a c527 8600 8000  ng.dll...*.'....
-00002010: 0053 29d0 50ec d5fd 41b7 5dc0 3bb4 fec2  .S).P...A.].;...
-00002020: aa53 7973 7465 6d2e 4472 6177 696e 672e  .System.Drawing.
-00002030: 5072 696d 6974 6976 6573 2e64 6c6c 0000  Primitives.dll..
-00002040: 0130 b401 ca00 c000 008e 8f7f 0f67 cfeb  .0...........g..
-00002050: 438c aca0 408d d5b7 8853 7973 7465 6d2e  C...@....System.
-00002060: 4479 6e61 6d69 632e 5275 6e74 696d 652e  Dynamic.Runtime.
-00002070: 646c 6c00 0001 7af8 ba93 0080 0000 00d2  dll...z.........
-00002080: 3986 f2b3 5047 98a0 8d09 122b 601d 5379  9...PG.....+`.Sy
-00002090: 7374 656d 2e46 6f72 6d61 7473 2e41 736e  stem.Formats.Asn
-000020a0: 312e 646c 6c00 0001 d5eb 2df8 00a0 0000  1.dll.....-.....
-000020b0: 6809 fe95 7ccf be4c aa8e 7879 c0e9 dd04  h...|..L..xy....
-000020c0: 5379 7374 656d 2e47 6c6f 6261 6c69 7a61  System.Globaliza
-000020d0: 7469 6f6e 2e43 616c 656e 6461 7273 2e64  tion.Calendars.d
-000020e0: 6c6c 0000 0119 2fbb 9a00 8000 008e 0099  ll..../.........
-000020f0: e074 bd7f 4caa 3458 690f b25a 7b53 7973  .t..L.4Xi..Z{Sys
-00002100: 7465 6d2e 476c 6f62 616c 697a 6174 696f  tem.Globalizatio
-00002110: 6e2e 646c 6c00 0001 d1af f6a4 0080 0000  n.dll...........
-00002120: 4f43 3c41 90af 6f45 9f16 2060 991e 4966  OC<A..oE.. `..If
-00002130: 5379 7374 656d 2e47 6c6f 6261 6c69 7a61  System.Globaliza
-00002140: 7469 6f6e 2e45 7874 656e 7369 6f6e 732e  tion.Extensions.
-00002150: 646c 6c00 0001 f33d 8be4 0080 0000 198b  dll....=........
-00002160: dc84 e703 df49 959b ece8 5b61 08d3 5379  .....I....[a..Sy
-00002170: 7374 656d 2e49 4f2e 436f 6d70 7265 7373  stem.IO.Compress
-00002180: 696f 6e2e 4272 6f74 6c69 2e64 6c6c 0000  ion.Brotli.dll..
-00002190: 01bc 6117 e100 8000 003c 5edd 0f96 2796  ..a......<^...'.
-000021a0: 41bc 60e7 167c 93ec ff53 7973 7465 6d2e  A.`..|...System.
-000021b0: 494f 2e43 6f6d 7072 6573 7369 6f6e 2e64  IO.Compression.d
-000021c0: 6c6c 0000 01ea 16ee b900 a000 00b4 df97  ll..............
-000021d0: ee7e bd80 459a 36f1 fbf4 4867 3853 7973  .~..E.6...Hg8Sys
-000021e0: 7465 6d2e 494f 2e43 6f6d 7072 6573 7369  tem.IO.Compressi
-000021f0: 6f6e 2e46 696c 6553 7973 7465 6d2e 646c  on.FileSystem.dl
-00002200: 6c00 0001 6b99 aed3 0080 0000 523d 5710  l...k.......R=W.
-00002210: 75f0 1a48 ada5 d1b7 890b 0c6c 5379 7374  u..H.......lSyst
-00002220: 656d 2e49 4f2e 436f 6d70 7265 7373 696f  em.IO.Compressio
-00002230: 6e2e 5a69 7046 696c 652e 646c 6c00 0001  n.ZipFile.dll...
-00002240: 5853 7cc3 0080 0000 580d 2f60 b7c2 004e  XS|.....X./`...N
-00002250: a5bf 0576 acb1 67d9 5379 7374 656d 2e49  ...v..g.System.I
-00002260: 4f2e 646c 6c00 0001 1ced 88ed 0080 0000  O.dll...........
-00002270: 2b3c c477 14f7 844c bba2 c24f 55c2 8603  +<.w...L...OU...
-00002280: 5379 7374 656d 2e49 4f2e 4669 6c65 5379  System.IO.FileSy
-00002290: 7374 656d 2e41 6363 6573 7343 6f6e 7472  stem.AccessContr
-000022a0: 6f6c 2e64 6c6c 0000 01a5 3b8d 9000 a000  ol.dll....;.....
-000022b0: 007a eb3c 18a8 34fc 4c9a 38c0 0ddf dedc  .z.<..4.L.8.....
-000022c0: 8853 7973 7465 6d2e 494f 2e46 696c 6553  .System.IO.FileS
-000022d0: 7973 7465 6d2e 646c 6c00 0001 f9c7 0dbf  ystem.dll.......
-000022e0: 0080 0000 eca4 c059 9fbc 744e a4af 37c2  .......Y..tN..7.
-000022f0: dca4 b1f9 5379 7374 656d 2e49 4f2e 4669  ....System.IO.Fi
-00002300: 6c65 5379 7374 656d 2e44 7269 7665 496e  leSystem.DriveIn
-00002310: 666f 2e64 6c6c 0000 0175 7d28 cf00 8000  fo.dll...u}(....
-00002320: 006e a90f b3e5 511d 47b0 7485 905f 7688  .n....Q.G.t.._v.
-00002330: 0553 7973 7465 6d2e 494f 2e46 696c 6553  .System.IO.FileS
-00002340: 7973 7465 6d2e 5072 696d 6974 6976 6573  ystem.Primitives
-00002350: 2e64 6c6c 0000 01b3 710c 9800 8000 0050  .dll....q......P
-00002360: 7c76 ce46 08de 4499 13d6 6755 6ff3 ed53  |v.F..D...gUo..S
-00002370: 7973 7465 6d2e 494f 2e46 696c 6553 7973  ystem.IO.FileSys
-00002380: 7465 6d2e 5761 7463 6865 722e 646c 6c00  tem.Watcher.dll.
-00002390: 0001 eeb6 f7b2 00a0 0000 d4b5 5f3a 5fd9  ............_:_.
-000023a0: 3b41 8dc2 cac6 4bde 7572 5379 7374 656d  ;A....K.urSystem
-000023b0: 2e49 4f2e 4973 6f6c 6174 6564 5374 6f72  .IO.IsolatedStor
-000023c0: 6167 652e 646c 6c00 0001 a38e dec4 00a0  age.dll.........
-000023d0: 0000 3710 05cc 327d f64d b4ce 8a5c 6c81  ..7...2}.M...\l.
-000023e0: 614e 5379 7374 656d 2e49 4f2e 4d65 6d6f  aNSystem.IO.Memo
-000023f0: 7279 4d61 7070 6564 4669 6c65 732e 646c  ryMappedFiles.dl
-00002400: 6c00 0001 47f5 1ff4 0080 0000 9151 f98c  l...G........Q..
-00002410: 5e36 494b 90f8 515d 8b59 68cf 5379 7374  ^6IK..Q].Yh.Syst
-00002420: 656d 2e49 4f2e 5069 7065 732e 4163 6365  em.IO.Pipes.Acce
-00002430: 7373 436f 6e74 726f 6c2e 646c 6c00 0001  ssControl.dll...
-00002440: 7f6c 5bfc 0080 0000 3bd5 5395 4e3d 4b4d  .l[.....;.S.N=KM
-00002450: 9687 50e1 5508 b91f 5379 7374 656d 2e49  ..P.U...System.I
-00002460: 4f2e 5069 7065 732e 646c 6c00 0001 26a5  O.Pipes.dll...&.
-00002470: fdc3 00a0 0000 d904 bc24 8b94 9a47 9743  .........$...G.C
-00002480: a06e d131 4978 5379 7374 656d 2e49 4f2e  .n.1IxSystem.IO.
-00002490: 556e 6d61 6e61 6765 644d 656d 6f72 7953  UnmanagedMemoryS
-000024a0: 7472 6561 6d2e 646c 6c00 0001 d746 0fa0  tream.dll....F..
-000024b0: 0080 0000 d3a0 8040 199b 5441 b8d9 284f  .......@..TA..(O
-000024c0: 57b3 9292 5379 7374 656d 2e4c 696e 712e  W...System.Linq.
-000024d0: 646c 6c00 0001 d06e d586 00c0 0000 697d  dll....n......i}
-000024e0: 34b4 dfec 2b40 bd36 4017 1269 d6a6 5379  4...+@.6@..i..Sy
-000024f0: 7374 656d 2e4c 696e 712e 4578 7072 6573  stem.Linq.Expres
-00002500: 7369 6f6e 732e 646c 6c00 0001 85c6 9691  sions.dll.......
-00002510: 0040 0100 1ac9 5fc9 1258 fc47 aa66 0d42  .@...._..X.G.f.B
-00002520: 9ed0 c519 5379 7374 656d 2e4c 696e 712e  ....System.Linq.
-00002530: 5061 7261 6c6c 656c 2e64 6c6c 0000 019a  Parallel.dll....
-00002540: e108 c500 c000 00f0 26d0 c04a 43cf 4286  ........&..JC.B.
-00002550: 80d5 7630 02e0 4e53 7973 7465 6d2e 4c69  ..v0..NSystem.Li
-00002560: 6e71 2e51 7565 7279 6162 6c65 2e64 6c6c  nq.Queryable.dll
-00002570: 0000 012f 3dc9 8700 c000 00b4 2fac f0a4  .../=......./...
-00002580: 719c 4596 cef1 c318 bcdc e853 7973 7465  q.E........Syste
-00002590: 6d2e 4d65 6d6f 7279 2e64 6c6c 0000 01d1  m.Memory.dll....
-000025a0: f194 9700 e000 0039 ecd5 1a26 3372 43a1  .......9...&3rC.
-000025b0: 3b0a 2cd8 c030 3853 7973 7465 6d2e 4e65  ;.,..08System.Ne
-000025c0: 742e 646c 6c00 0001 d616 97d6 0080 0000  t.dll...........
-000025d0: 5be1 7e6f d1ef d447 bb98 0601 2b17 a015  [.~o...G....+...
-000025e0: 5379 7374 656d 2e4e 6574 2e48 7474 702e  System.Net.Http.
-000025f0: 646c 6c00 0001 9234 82c2 0020 0100 4285  dll....4... ..B.
-00002600: 9141 8cd2 c44a 9267 5fb6 c70d fe03 5379  .A...J.g_.....Sy
-00002610: 7374 656d 2e4e 6574 2e48 7474 702e 4a73  stem.Net.Http.Js
-00002620: 6f6e 2e64 6c6c 0000 01d6 70c7 eb00 8000  on.dll....p.....
-00002630: 00c5 125f 9f70 f8f9 4491 411f 3d51 8729  ..._.p..D.A.=Q.)
-00002640: 2053 7973 7465 6d2e 4e65 742e 4874 7470   System.Net.Http
-00002650: 4c69 7374 656e 6572 2e64 6c6c 0000 0131  Listener.dll...1
-00002660: 7ce3 f600 a000 00e5 f981 6441 2a43 4eb3  |.........dA*CN.
-00002670: e76c 51b6 41a4 2353 7973 7465 6d2e 4e65  .lQ.A.#System.Ne
-00002680: 742e 4d61 696c 2e64 6c6c 0000 012f 7bf6  t.Mail.dll.../{.
-00002690: d600 c000 00ec ef60 8c04 4e6a 499b d4ff  .......`..NjI...
-000026a0: 1379 5c16 2553 7973 7465 6d2e 4e65 742e  .y\.%System.Net.
-000026b0: 4e61 6d65 5265 736f 6c75 7469 6f6e 2e64  NameResolution.d
-000026c0: 6c6c 0000 017a 3c48 e300 8000 0089 4311  ll...z<H......C.
-000026d0: e3dc 4efa 4681 2104 d992 6096 b953 7973  ..N.F.!...`..Sys
-000026e0: 7465 6d2e 4e65 742e 4e65 7477 6f72 6b49  tem.Net.NetworkI
-000026f0: 6e66 6f72 6d61 7469 6f6e 2e64 6c6c 0000  nformation.dll..
-00002700: 01b1 ee6a 8600 c000 0006 798a 0663 7c93  ...j......y..c|.
-00002710: 4780 d5ac 2183 564d 9e53 7973 7465 6d2e  G...!.VM.System.
-00002720: 4e65 742e 5069 6e67 2e64 6c6c 0000 0126  Net.Ping.dll...&
-00002730: c08c eb00 8000 00e1 52c0 3460 a08b 46ac  ........R.4`..F.
-00002740: 6865 8747 2a97 0b53 7973 7465 6d2e 4e65  he.G*..System.Ne
-00002750: 742e 5072 696d 6974 6976 6573 2e64 6c6c  t.Primitives.dll
-00002760: 0000 0112 d83d 8800 c000 0084 7bc3 b094  .....=......{...
-00002770: 397b 4da0 2fc9 34b4 6560 b853 7973 7465  9{M./.4.e`.Syste
-00002780: 6d2e 4e65 742e 5265 7175 6573 7473 2e64  m.Net.Requests.d
-00002790: 6c6c 0000 01a2 8b03 cf00 e000 0081 1a5b  ll.............[
-000027a0: 1c42 02c0 40b0 a164 f25d 024e 4153 7973  .B..@..d.].NASys
-000027b0: 7465 6d2e 4e65 742e 5365 6375 7269 7479  tem.Net.Security
-000027c0: 2e64 6c6c 0000 0125 1d0d 9100 0001 0016  .dll...%........
-000027d0: 0258 8074 d086 4eb7 e3fc b0e2 cd22 3553  .X.t..N......"5S
-000027e0: 7973 7465 6d2e 4e65 742e 5365 7276 6963  ystem.Net.Servic
-000027f0: 6550 6f69 6e74 2e64 6c6c 0000 01ea 7bb7  ePoint.dll....{.
-00002800: c800 8000 000a cce3 6eaa fc06 4292 947c  ........n...B..|
-00002810: 79ae d821 0a53 7973 7465 6d2e 4e65 742e  y..!.System.Net.
-00002820: 536f 636b 6574 732e 646c 6c00 0001 b667  Sockets.dll....g
-00002830: 82e2 0000 0100 52ba 356f 9cb6 b547 958a  ......R.5o...G..
-00002840: 3902 0297 251a 5379 7374 656d 2e4e 6574  9...%.System.Net
-00002850: 2e57 6562 436c 6965 6e74 2e64 6c6c 0000  .WebClient.dll..
-00002860: 01de 75d8 b100 a000 0061 c26e 6835 0ccd  ..u......a.nh5..
-00002870: 4f85 dc2f 9b1f 8e52 0053 7973 7465 6d2e  O../...R.System.
-00002880: 4e65 742e 5765 6248 6561 6465 7243 6f6c  Net.WebHeaderCol
-00002890: 6c65 6374 696f 6e2e 646c 6c00 0001 5298  lection.dll...R.
-000028a0: a3af 0080 0000 9b0f bdce c94d dc4a 819b  ...........M.J..
-000028b0: 4efd 3172 d63f 5379 7374 656d 2e4e 6574  N.1r.?System.Net
-000028c0: 2e57 6562 5072 6f78 792e 646c 6c00 0001  .WebProxy.dll...
-000028d0: 4c21 05ed 0080 0000 b4ff cb6a 98e5 2546  L!.........j..%F
-000028e0: bcfe 7ace a33e 78db 5379 7374 656d 2e4e  ..z..>x.System.N
-000028f0: 6574 2e57 6562 536f 636b 6574 732e 436c  et.WebSockets.Cl
-00002900: 6965 6e74 2e64 6c6c 0000 018e 6030 ea00  ient.dll....`0..
-00002910: 8000 00d1 cbc2 a741 9dde 489b 9ef3 e424  .......A..H....$
-00002920: 25e4 2a53 7973 7465 6d2e 4e65 742e 5765  %.*System.Net.We
-00002930: 6253 6f63 6b65 7473 2e64 6c6c 0000 01f2  bSockets.dll....
-00002940: 6bd8 a000 a000 0018 fa75 49d6 02fa 4cb6  k........uI...L.
-00002950: a320 9f5a bdce 1053 7973 7465 6d2e 4e75  . .Z...System.Nu
-00002960: 6d65 7269 6373 2e64 6c6c 0000 0184 9828  merics.dll.....(
-00002970: ab00 8000 005e c453 95d3 d45e 44bb 10b8  .....^.S...^D...
-00002980: 106a aec7 6153 7973 7465 6d2e 4e75 6d65  .j..aSystem.Nume
-00002990: 7269 6373 2e56 6563 746f 7273 2e64 6c6c  rics.Vectors.dll
-000029a0: 0000 0128 605a dc00 c000 007e 186e 89d2  ...(`Z.....~.n..
-000029b0: cdb6 418a a3b7 3df7 dc27 d753 7973 7465  ..A...=..'.Syste
-000029c0: 6d2e 4f62 6a65 6374 4d6f 6465 6c2e 646c  m.ObjectModel.dl
-000029d0: 6c00 0001 9f0e 5aac 00c0 0000 67a6 7345  l.....Z.....g.sE
-000029e0: dcc6 104c 8668 0bb2 638b 7324 5379 7374  ...L.h..c.s$Syst
-000029f0: 656d 2e52 6566 6c65 6374 696f 6e2e 4469  em.Reflection.Di
-00002a00: 7370 6174 6368 5072 6f78 792e 646c 6c00  spatchProxy.dll.
-00002a10: 0001 309b 53d8 0080 0000 3a9b 950e d84e  ..0.S.....:....N
-00002a20: 184c 83d5 f836 66cd e4b5 5379 7374 656d  .L...6f...System
-00002a30: 2e52 6566 6c65 6374 696f 6e2e 646c 6c00  .Reflection.dll.
-00002a40: 0001 7aef 99f4 0080 0000 d4a3 74c6 ac2d  ..z.........t..-
-00002a50: da40 a910 978d 3860 89b2 5379 7374 656d  .@....8`..System
-00002a60: 2e52 6566 6c65 6374 696f 6e2e 456d 6974  .Reflection.Emit
-00002a70: 2e64 6c6c 0000 01bd ed33 c000 e000 003e  .dll.....3.....>
-00002a80: e0e1 3102 dfa7 4c9c 39a7 d340 04f3 7553  ..1...L.9..@..uS
-00002a90: 7973 7465 6d2e 5265 666c 6563 7469 6f6e  ystem.Reflection
-00002aa0: 2e45 6d69 742e 494c 4765 6e65 7261 7469  .Emit.ILGenerati
-00002ab0: 6f6e 2e64 6c6c 0000 01ea 8ba1 b100 a000  on.dll..........
-00002ac0: 0061 47ef bfb1 5a7b 4495 6eab 804d a813  .aG...Z{D.n..M..
-00002ad0: 3d53 7973 7465 6d2e 5265 666c 6563 7469  =System.Reflecti
-00002ae0: 6f6e 2e45 6d69 742e 4c69 6768 7477 6569  on.Emit.Lightwei
-00002af0: 6768 742e 646c 6c00 0001 3990 09cb 0080  ght.dll...9.....
-00002b00: 0000 6599 3a9e d785 854c a454 6ac0 387f  ..e.:....L.Tj.8.
-00002b10: d650 5379 7374 656d 2e52 6566 6c65 6374  .PSystem.Reflect
-00002b20: 696f 6e2e 4578 7465 6e73 696f 6e73 2e64  ion.Extensions.d
-00002b30: 6c6c 0000 01e7 0a6e 9a00 8000 00b0 bb2a  ll.....n.......*
-00002b40: d038 0c35 4c94 2514 b83e f83a d553 7973  .8.5L.%..>.:.Sys
-00002b50: 7465 6d2e 5265 666c 6563 7469 6f6e 2e4d  tem.Reflection.M
-00002b60: 6574 6164 6174 612e 646c 6c00 0001 a1e5  etadata.dll.....
-00002b70: 61c2 0020 0200 1e2f 7240 4688 fa4a a99a  a.. .../r@F..J..
-00002b80: 89ad 2bf2 7020 5379 7374 656d 2e52 6566  ..+.p System.Ref
-00002b90: 6c65 6374 696f 6e2e 5072 696d 6974 6976  lection.Primitiv
-00002ba0: 6573 2e64 6c6c 0000 0191 2932 ee00 a000  es.dll....)2....
-00002bb0: 007c 4929 f4b5 222d 4596 77b6 5a5b 4d24  .|I).."-E.w.Z[M$
-00002bc0: f353 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
-00002bd0: 6f6e 2e54 7970 6545 7874 656e 7369 6f6e  on.TypeExtension
-00002be0: 732e 646c 6c00 0001 3a94 eae3 0080 0000  s.dll...:.......
-00002bf0: 89a1 ba5e 6a57 7c45 92e9 ef81 f8e6 d8da  ...^jW|E........
-00002c00: 5379 7374 656d 2e52 6573 6f75 7263 6573  System.Resources
-00002c10: 2e52 6561 6465 722e 646c 6c00 0001 febc  .Reader.dll.....
-00002c20: a5b5 0080 0000 c3e8 8ab1 6ba5 8849 a02b  ..........k..I.+
-00002c30: 6f9c 54f3 bae2 5379 7374 656d 2e52 6573  o.T...System.Res
-00002c40: 6f75 7263 6573 2e52 6573 6f75 7263 654d  ources.ResourceM
-00002c50: 616e 6167 6572 2e64 6c6c 0000 01bc 85f7  anager.dll......
-00002c60: ce00 8000 0017 6017 82e9 ade6 4988 c3d0  ......`.....I...
-00002c70: 60bb 8c8c 5d53 7973 7465 6d2e 5265 736f  `...]System.Reso
-00002c80: 7572 6365 732e 5772 6974 6572 2e64 6c6c  urces.Writer.dll
-00002c90: 0000 0183 6b9b 8d00 8000 00f9 827c bb7f  ....k........|..
-00002ca0: 0463 4b99 b7f5 a734 22ca 0853 7973 7465  .cK....4"..Syste
-00002cb0: 6d2e 5275 6e74 696d 652e 436f 6d70 696c  m.Runtime.Compil
-00002cc0: 6572 5365 7276 6963 6573 2e55 6e73 6166  erServices.Unsaf
-00002cd0: 652e 646c 6c00 0001 6c72 7bc8 0080 0000  e.dll...lr{.....
-00002ce0: 8cd2 862d 3c11 ef44 8746 70b8 60b6 a3c6  ...-<..D.Fp.`...
-00002cf0: 5379 7374 656d 2e52 756e 7469 6d65 2e43  System.Runtime.C
-00002d00: 6f6d 7069 6c65 7253 6572 7669 6365 732e  ompilerServices.
-00002d10: 5669 7375 616c 432e 646c 6c00 0001 e4e9  VisualC.dll.....
-00002d20: 92c1 0080 0000 bbf3 2cba 4956 e44c 85e2  ........,.IV.L..
-00002d30: eab1 f356 d66c 5379 7374 656d 2e52 756e  ...V.lSystem.Run
-00002d40: 7469 6d65 2e64 6c6c 0000 014f a117 ce00  time.dll...O....
-00002d50: 8007 00a3 ef9c 58c3 b940 4d90 cede 3294  ......X..@M...2.
-00002d60: d4f3 0453 7973 7465 6d2e 5275 6e74 696d  ...System.Runtim
-00002d70: 652e 4578 7465 6e73 696f 6e73 2e64 6c6c  e.Extensions.dll
-00002d80: 0000 01fb 93c6 cd00 8000 0079 3b4b 0168  ...........y;K.h
-00002d90: 882e 4592 2115 ec92 b811 7253 7973 7465  ..E.!.....rSyste
-00002da0: 6d2e 5275 6e74 696d 652e 4861 6e64 6c65  m.Runtime.Handle
-00002db0: 732e 646c 6c00 0001 ebda e6f5 0080 0000  s.dll...........
-00002dc0: 9cc4 740a 05b5 1a4d 808c 076b abad a534  ..t....M...k...4
-00002dd0: 5379 7374 656d 2e52 756e 7469 6d65 2e49  System.Runtime.I
-00002de0: 6e74 6572 6f70 5365 7276 6963 6573 2e64  nteropServices.d
-00002df0: 6c6c 0000 01af cc8a 9c00 4001 0080 3b45  ll........@...;E
-00002e00: 973f ea70 4db5 d1a6 3ac2 986c 8b53 7973  .?.pM...:..l.Sys
-00002e10: 7465 6d2e 5275 6e74 696d 652e 496e 7465  tem.Runtime.Inte
-00002e20: 726f 7053 6572 7669 6365 732e 5275 6e74  ropServices.Runt
-00002e30: 696d 6549 6e66 6f72 6d61 7469 6f6e 2e64  imeInformation.d
-00002e40: 6c6c 0000 0119 3232 d500 8000 0007 f899  ll....22........
-00002e50: ecaf 3300 41b1 033e e1e8 7154 d753 7973  ..3.A..>..qT.Sys
-00002e60: 7465 6d2e 5275 6e74 696d 652e 496e 7472  tem.Runtime.Intr
-00002e70: 696e 7369 6373 2e64 6c6c 0000 0132 532d  insics.dll...2S-
-00002e80: 8100 c002 008f 41a5 9a68 4bba 4fb9 819d  ......A..hK.O...
-00002e90: 1b29 7f51 1f53 7973 7465 6d2e 5275 6e74  .).Q.System.Runt
-00002ea0: 696d 652e 4c6f 6164 6572 2e64 6c6c 0000  ime.Loader.dll..
-00002eb0: 01bd 89ce 9900 8000 00cb e5cd 3ba8 4a1f  ............;.J.
-00002ec0: 4892 5b14 edbf bd26 bd53 7973 7465 6d2e  H.[....&.System.
-00002ed0: 5275 6e74 696d 652e 4e75 6d65 7269 6373  Runtime.Numerics
-00002ee0: 2e64 6c6c 0000 0124 2e2e fc00 a000 00c6  .dll...$........
-00002ef0: 9bca 61ba aead 4fa2 bcf1 8b03 35d5 a853  ..a...O.....5..S
-00002f00: 7973 7465 6d2e 5275 6e74 696d 652e 5365  ystem.Runtime.Se
-00002f10: 7269 616c 697a 6174 696f 6e2e 646c 6c00  rialization.dll.
-00002f20: 0001 5732 cda0 0080 0000 96e2 9c85 b24f  ..W2...........O
-00002f30: 0c41 aa16 4e58 5d80 311b 5379 7374 656d  .A..NX].1.System
-00002f40: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
-00002f50: 7a61 7469 6f6e 2e46 6f72 6d61 7474 6572  zation.Formatter
-00002f60: 732e 646c 6c00 0001 8cf0 ff9b 00a0 0000  s.dll...........
-00002f70: e825 4dad c610 d949 9dbb 619b 1a21 4f2e  .%M....I..a..!O.
-00002f80: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
-00002f90: 6572 6961 6c69 7a61 7469 6f6e 2e4a 736f  erialization.Jso
-00002fa0: 6e2e 646c 6c00 0001 8772 c189 0080 0000  n.dll....r......
-00002fb0: dfbb 2c4f b09b 474a 80eb af14 4c47 2a68  ..,O..GJ....LG*h
-00002fc0: 5379 7374 656d 2e52 756e 7469 6d65 2e53  System.Runtime.S
-00002fd0: 6572 6961 6c69 7a61 7469 6f6e 2e50 7269  erialization.Pri
-00002fe0: 6d69 7469 7665 732e 646c 6c00 0001 ca14  mitives.dll.....
-00002ff0: 3ec6 0080 0000 6ed2 d5f7 b8da f446 9b4b  >.....n......F.K
-00003000: be28 0c09 e6e8 5379 7374 656d 2e52 756e  .(....System.Run
-00003010: 7469 6d65 2e53 6572 6961 6c69 7a61 7469  time.Serializati
-00003020: 6f6e 2e58 6d6c 2e64 6c6c 0000 0152 bc99  on.Xml.dll...R..
-00003030: d400 c000 00c4 715b 4877 e90c 41bc 7941  ......q[Hw..A.yA
-00003040: 423c b424 5253 7973 7465 6d2e 5365 6375  B<.$RSystem.Secu
-00003050: 7269 7479 2e41 6363 6573 7343 6f6e 7472  rity.AccessContr
-00003060: 6f6c 2e64 6c6c 0000 01de 06e9 b000 e000  ol.dll..........
-00003070: 00fb c501 60dd 56b5 4b8e 958c 0bbf e0d6  ....`.V.K.......
-00003080: 4753 7973 7465 6d2e 5365 6375 7269 7479  GSystem.Security
-00003090: 2e43 6c61 696d 732e 646c 6c00 0001 3fae  .Claims.dll...?.
-000030a0: 48a4 00c0 0000 edad 319d 89bd 704d 90a5  H.......1...pM..
-000030b0: 3185 0c1e 2b37 5379 7374 656d 2e53 6563  1...+7System.Sec
-000030c0: 7572 6974 792e 4372 7970 746f 6772 6170  urity.Cryptograp
-000030d0: 6879 2e41 6c67 6f72 6974 686d 732e 646c  hy.Algorithms.dl
-000030e0: 6c00 0001 c701 8c95 0000 0100 e8b0 26da  l.............&.
-000030f0: db55 544d 84db 4f31 51f8 23db 5379 7374  .UTM..O1Q.#.Syst
-00003100: 656d 2e53 6563 7572 6974 792e 4372 7970  em.Security.Cryp
-00003110: 746f 6772 6170 6879 2e43 6e67 2e64 6c6c  tography.Cng.dll
-00003120: 0000 01a7 2137 a900 c000 00d2 d896 fb91  ....!7..........
-00003130: 538c 4ab8 cd2f c889 004e f053 7973 7465  S.J../...N.Syste
-00003140: 6d2e 5365 6375 7269 7479 2e43 7279 7074  m.Security.Crypt
-00003150: 6f67 7261 7068 792e 4373 702e 646c 6c00  ography.Csp.dll.
-00003160: 0001 52ed 5ec5 00a0 0000 ab21 6ba9 89a5  ..R.^......!k...
-00003170: be41 88ad bbeb 1330 938f 5379 7374 656d  .A.....0..System
-00003180: 2e53 6563 7572 6974 792e 4372 7970 746f  .Security.Crypto
-00003190: 6772 6170 6879 2e45 6e63 6f64 696e 672e  graphy.Encoding.
-000031a0: 646c 6c00 0001 82cb 6986 00a0 0000 de52  dll.....i......R
-000031b0: 53ff 2cb4 1d43 a6fe 0857 4f4a a648 5379  S.,..C...WOJ.HSy
-000031c0: 7374 656d 2e53 6563 7572 6974 792e 4372  stem.Security.Cr
-000031d0: 7970 746f 6772 6170 6879 2e4f 7065 6e53  yptography.OpenS
-000031e0: 736c 2e64 6c6c 0000 01d9 3597 c800 8000  sl.dll....5.....
-000031f0: 002f 85b5 187e 8878 44b2 9b7a 5607 e643  ./...~.xD..zV..C
-00003200: c653 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
-00003210: 2e43 7279 7074 6f67 7261 7068 792e 5072  .Cryptography.Pr
-00003220: 696d 6974 6976 6573 2e64 6c6c 0000 01f8  imitives.dll....
-00003230: 48bd b500 a000 0008 e488 d541 95c4 42a9  H..........A..B.
-00003240: c1d9 b932 5124 3153 7973 7465 6d2e 5365  ...2Q$1System.Se
-00003250: 6375 7269 7479 2e43 7279 7074 6f67 7261  curity.Cryptogra
-00003260: 7068 792e 5835 3039 4365 7274 6966 6963  phy.X509Certific
-00003270: 6174 6573 2e64 6c6c 0000 011e 8a31 f300  ates.dll.....1..
-00003280: e000 0038 99aa b575 db67 4e91 674a 6366  ...8...u.gN.gJcf
-00003290: 4066 c153 7973 7465 6d2e 5365 6375 7269  @f.System.Securi
-000032a0: 7479 2e64 6c6c 0000 01d7 281a af00 8000  ty.dll....(.....
-000032b0: 00fb e9da 24ff 618c 46bd 1b68 2e35 d8f5  ....$.a.F..h.5..
-000032c0: 0453 7973 7465 6d2e 5365 6375 7269 7479  .System.Security
-000032d0: 2e50 7269 6e63 6970 616c 2e64 6c6c 0000  .Principal.dll..
-000032e0: 0197 afa4 d700 8000 0027 8a16 bac0 9544  .........'.....D
-000032f0: 4aa4 52ae 3e07 2e8d 6253 7973 7465 6d2e  J.R.>...bSystem.
-00003300: 5365 6375 7269 7479 2e50 7269 6e63 6970  Security.Princip
-00003310: 616c 2e57 696e 646f 7773 2e64 6c6c 0000  al.Windows.dll..
-00003320: 0137 b68c a200 a000 0007 4c72 b4ef d98a  .7........Lr....
-00003330: 4a8d 474f 44c7 e710 ea53 7973 7465 6d2e  J.GOD....System.
-00003340: 5365 6375 7269 7479 2e53 6563 7572 6553  Security.SecureS
-00003350: 7472 696e 672e 646c 6c00 0001 8ba7 83bf  tring.dll.......
-00003360: 0080 0000 cb5c 39de 14de 2e48 ac1c 4ab6  .....\9....H..J.
-00003370: b5b4 9011 5379 7374 656d 2e53 6572 7669  ....System.Servi
-00003380: 6365 4d6f 6465 6c2e 5765 622e 646c 6c00  ceModel.Web.dll.
-00003390: 0001 3dd3 54b3 0080 0000 a43a 99fe eb55  ..=.T......:...U
-000033a0: 9248 bbc3 a67b b1ba 123d 5379 7374 656d  .H...{...=System
-000033b0: 2e53 6572 7669 6365 5072 6f63 6573 732e  .ServiceProcess.
-000033c0: 646c 6c00 0001 899a cec1 0080 0000 5539  dll...........U9
-000033d0: 1e62 bd38 4d42 896d f311 a44b efb1 5379  .b.8MB.m...K..Sy
-000033e0: 7374 656d 2e54 6578 742e 456e 636f 6469  stem.Text.Encodi
-000033f0: 6e67 2e43 6f64 6550 6167 6573 2e64 6c6c  ng.CodePages.dll
-00003400: 0000 013c 2e5d f600 8000 00e1 b1ec fb2f  ...<.]........./
-00003410: d5b5 44a0 24ad c731 b431 0053 7973 7465  ..D.$..1.1.Syste
-00003420: 6d2e 5465 7874 2e45 6e63 6f64 696e 672e  m.Text.Encoding.
-00003430: 646c 6c00 0001 80b4 14a3 0080 0000 9ce3  dll.............
-00003440: b249 0b7e 8e43 9049 d265 90a2 e97d 5379  .I.~.C.I.e...}Sy
-00003450: 7374 656d 2e54 6578 742e 456e 636f 6469  stem.Text.Encodi
-00003460: 6e67 2e45 7874 656e 7369 6f6e 732e 646c  ng.Extensions.dl
-00003470: 6c00 0001 3f1b b5b0 00a0 0000 354c 6745  l...?.......5LgE
-00003480: cf2e 034a ad89 10f2 c783 bf90 5379 7374  ...J........Syst
-00003490: 656d 2e54 6578 742e 456e 636f 6469 6e67  em.Text.Encoding
-000034a0: 732e 5765 622e 646c 6c00 0001 b007 b8df  s.Web.dll.......
-000034b0: 00a0 0000 b7cd 6a87 6293 da46 8545 efbb  ......j.b..F.E..
-000034c0: 2261 49c1 5379 7374 656d 2e54 6578 742e  "aI.System.Text.
-000034d0: 4a73 6f6e 2e64 6c6c 0000 012f 3d98 cb00  Json.dll.../=...
-000034e0: 2001 00b1 04e5 583b b9ad 419e 3eda 6af1   .....X;..A.>.j.
-000034f0: 8497 7d53 7973 7465 6d2e 5465 7874 2e52  ..}System.Text.R
-00003500: 6567 756c 6172 4578 7072 6573 7369 6f6e  egularExpression
-00003510: 732e 646c 6c00 0001 7742 4fab 00c0 0000  s.dll...wBO.....
-00003520: c770 ed57 161f 3e47 af43 d65f 9424 cc8a  .p.W..>G.C._.$..
-00003530: 5379 7374 656d 2e54 6872 6561 6469 6e67  System.Threading
-00003540: 2e43 6861 6e6e 656c 732e 646c 6c00 0001  .Channels.dll...
-00003550: 34bd fda0 0080 0000 3eb0 35d8 8199 f847  4.......>.5....G
-00003560: a870 6faa 4125 5e13 5379 7374 656d 2e54  .po.A%^.System.T
-00003570: 6872 6561 6469 6e67 2e64 6c6c 0000 01d3  hreading.dll....
-00003580: c2ec 9700 c000 0079 d76d 0a6c 4cde 42b1  .......y.m.lL.B.
-00003590: e029 f8d3 f114 1f53 7973 7465 6d2e 5468  .).....System.Th
-000035a0: 7265 6164 696e 672e 4f76 6572 6c61 7070  reading.Overlapp
-000035b0: 6564 2e64 6c6c 0000 0178 ccd2 a700 8000  ed.dll...x......
-000035c0: 0007 8bfa 9af2 34bb 42a1 453c abbf a67e  ......4.B.E<...~
-000035d0: b753 7973 7465 6d2e 5468 7265 6164 696e  .System.Threadin
-000035e0: 672e 5461 736b 732e 4461 7461 666c 6f77  g.Tasks.Dataflow
-000035f0: 2e64 6c6c 0000 016a 9fb3 f100 c000 0057  .dll...j.......W
-00003600: 1ee8 dc8f c8e2 4a9a 65f4 a83c 8ea0 fb53  ......J.e..<...S
-00003610: 7973 7465 6d2e 5468 7265 6164 696e 672e  ystem.Threading.
-00003620: 5461 736b 732e 646c 6c00 0001 0ec2 eab6  Tasks.dll.......
-00003630: 0080 0000 6555 7af7 eadb 8e4a b632 8c91  ....eUz....J.2..
-00003640: 7360 3ac0 5379 7374 656d 2e54 6872 6561  s`:.System.Threa
-00003650: 6469 6e67 2e54 6173 6b73 2e45 7874 656e  ding.Tasks.Exten
-00003660: 7369 6f6e 732e 646c 6c00 0001 0d9a feea  sions.dll.......
-00003670: 0080 0000 f3e4 81af 9578 2242 bb05 7b41  .........x"B..{A
-00003680: 707b b388 5379 7374 656d 2e54 6872 6561  p{..System.Threa
-00003690: 6469 6e67 2e54 6173 6b73 2e50 6172 616c  ding.Tasks.Paral
-000036a0: 6c65 6c2e 646c 6c00 0001 a67f 5b80 0080  lel.dll.....[...
-000036b0: 0000 5c62 7c74 ec73 8e4e b839 6f02 5da1  ..\b|t.s.N.9o.].
-000036c0: a896 5379 7374 656d 2e54 6872 6561 6469  ..System.Threadi
-000036d0: 6e67 2e54 6872 6561 642e 646c 6c00 0001  ng.Thread.dll...
-000036e0: bb81 fb87 00a0 0000 e0b9 fc04 8874 0b40  .............t.@
-000036f0: 9ba3 b7d0 1384 5979 5379 7374 656d 2e54  ......YySystem.T
-00003700: 6872 6561 6469 6e67 2e54 6872 6561 6450  hreading.ThreadP
-00003710: 6f6f 6c2e 646c 6c00 0001 13dd 58a8 0080  ool.dll.....X...
-00003720: 0000 9b33 fec3 3559 9e4a a6d4 0131 935f  ...3..5Y.J...1._
-00003730: 9a55 5379 7374 656d 2e54 6872 6561 6469  .USystem.Threadi
-00003740: 6e67 2e54 696d 6572 2e64 6c6c 0000 012c  ng.Timer.dll...,
-00003750: 6170 9600 8000 008f a3c6 bd14 b84c 4ea9  ap...........LN.
-00003760: 0b55 2fa7 ee6f 7c53 7973 7465 6d2e 5472  .U/..o|System.Tr
-00003770: 616e 7361 6374 696f 6e73 2e64 6c6c 0000  ansactions.dll..
-00003780: 01b6 6269 8000 8000 0032 370a 9851 5f81  ..bi.....27..Q_.
-00003790: 4882 e391 2b9c ba95 e953 7973 7465 6d2e  H...+....System.
-000037a0: 5472 616e 7361 6374 696f 6e73 2e4c 6f63  Transactions.Loc
-000037b0: 616c 2e64 6c6c 0000 01d1 1503 9700 a000  al.dll..........
-000037c0: 0065 2922 d1f3 3d59 4dbc 04a1 7e7c 7099  .e)"..=YM...~|p.
-000037d0: ee53 7973 7465 6d2e 5661 6c75 6554 7570  .System.ValueTup
-000037e0: 6c65 2e64 6c6c 0000 0157 aaac b900 8000  le.dll...W......
-000037f0: 009d 5a87 c7ad 3ff1 47a7 9196 b0b9 8f8d  ..Z...?.G.......
-00003800: 8f53 7973 7465 6d2e 5765 622e 646c 6c00  .System.Web.dll.
-00003810: 0001 4e23 e2cb 0080 0000 e6e7 1a23 27f3  ..N#.........#'.
-00003820: 4c49 94ec a1a6 803d 461c 5379 7374 656d  LI.....=F.System
-00003830: 2e57 6562 2e48 7474 7055 7469 6c69 7479  .Web.HttpUtility
-00003840: 2e64 6c6c 0000 0131 94f5 db00 8000 007a  .dll...1.......z
-00003850: ac04 a898 e8be 4792 f630 01a8 f4ec c453  ......G..0.....S
-00003860: 7973 7465 6d2e 5769 6e64 6f77 732e 646c  ystem.Windows.dl
-00003870: 6c00 0001 6f48 e4a1 0080 0000 f3d1 e27f  l...oH..........
-00003880: 7302 b54a a4db e65a e300 054e 5379 7374  s..J...Z...NSyst
-00003890: 656d 2e58 6d6c 2e64 6c6c 0000 01d6 1f9e  em.Xml.dll......
-000038a0: c900 a000 008f 30e0 f426 0edf 42a4 a2ad  ......0..&..B...
-000038b0: eeb4 311a c753 7973 7465 6d2e 586d 6c2e  ..1..System.Xml.
-000038c0: 4c69 6e71 2e64 6c6c 0000 01a6 3c94 9f00  Linq.dll....<...
-000038d0: 8000 0057 8590 7147 a8f6 46b3 0f20 8504  ...W..qG..F.. ..
-000038e0: 17ca 0e53 7973 7465 6d2e 586d 6c2e 5265  ...System.Xml.Re
-000038f0: 6164 6572 5772 6974 6572 2e64 6c6c 0000  aderWriter.dll..
-00003900: 0118 5d09 c400 0002 00cc 4d0c 99ac a283  ..].......M.....
-00003910: 4da7 237e 2215 a46b 5553 7973 7465 6d2e  M.#~"..kUSystem.
-00003920: 586d 6c2e 5365 7269 616c 697a 6174 696f  Xml.Serializatio
-00003930: 6e2e 646c 6c00 0001 ba95 f98d 0080 0000  n.dll...........
-00003940: e090 daba 8a7c 774e bbd6 4159 9902 3cf0  .....|wN..AY..<.
-00003950: 5379 7374 656d 2e58 6d6c 2e58 446f 6375  System.Xml.XDocu
-00003960: 6d65 6e74 2e64 6c6c 0000 01e7 a6eb a600  ment.dll........
-00003970: c000 004f c15e 4b58 f36a 4182 97ea 9b66  ...O.^KX.jA....f
-00003980: 8fac 4053 7973 7465 6d2e 586d 6c2e 586d  ..@System.Xml.Xm
-00003990: 6c44 6f63 756d 656e 742e 646c 6c00 0001  lDocument.dll...
-000039a0: 598a 6bbf 0080 0000 a48e 3b4b 693f 6544  Y.k.......;Ki?eD
-000039b0: 9260 55b3 fc15 0f6b 5379 7374 656d 2e58  .`U....kSystem.X
-000039c0: 6d6c 2e58 6d6c 5365 7269 616c 697a 6572  ml.XmlSerializer
-000039d0: 2e64 6c6c 0000 0154 3213 e500 0001 00d7  .dll...T2.......
-000039e0: 2bb6 9ceb 003d 488b 5a6d baac 634c 1d53  +....=H.Zm..cL.S
-000039f0: 7973 7465 6d2e 586d 6c2e 5850 6174 682e  ystem.Xml.XPath.
-00003a00: 646c 6c00 0001 7d58 6acd 0080 0000 b5ae  dll...}Xj.......
-00003a10: a120 b4fc aa4d b1b1 b538 b71e 8822 5379  . ...M...8..."Sy
-00003a20: 7374 656d 2e58 6d6c 2e58 5061 7468 2e58  stem.Xml.XPath.X
-00003a30: 446f 6375 6d65 6e74 2e64 6c6c 0000 0183  Document.dll....
-00003a40: 736c c600 8000 0058 b7df 8d54 8252 4a8a  sl.....X...T.RJ.
-00003a50: 97c7 8e66 9354 a555 6e64 6572 7461 6c65  ...f.T.Undertale
-00003a60: 4d6f 644c 6962 2e64 6c6c 0000 019b f66e  ModLib.dll.....n
-00003a70: ff00 2003 0090 9cab 0b12 8da2 418c 4e3a  .. .........A.N:
-00003a80: 2c98 30b2 3357 696e 646f 7773 4261 7365  ,.0.3WindowsBase
-00003a90: 2e64 6c6c 0000 0114 1787 b000 8000 003c  .dll...........<
-00003aa0: 440f c83d 91f4 4796 13af 540a 1d28 c015  D..=..G...T..(..
-00003ab0: 0100 0046 0f09 1000 1502 0003 000a 002c  ...F...........,
-00003ac0: 0600 3d04 5514 5369 784c 6162 6f72 732e  ..=.U.SixLabors.
-00003ad0: 496d 6167 6553 6861 7270 2153 6978 4c61  ImageSharp!SixLa
-00003ae0: 626f 7273 2e49 6d61 6765 5368 6172 702e  bors.ImageSharp.
-00003af0: 5069 7865 6c46 6f72 6d61 7473 1f53 6978  PixelFormats.Six
-00003b00: 4c61 626f 7273 2e49 6d61 6765 5368 6172  Labors.ImageShar
-00003b10: 702e 5072 6f63 6573 7369 6e67 0653 7973  p.Processing.Sys
-00003b20: 7465 6d1a 5379 7374 656d 2e43 6f6c 6c65  tem.System.Colle
-00003b30: 6374 696f 6e73 2e47 656e 6572 6963 0953  ctions.Generic.S
-00003b40: 7973 7465 6d2e 494f 0b53 7973 7465 6d2e  ystem.IO.System.
-00003b50: 4c69 6e71 0f53 7973 7465 6d2e 4e65 742e  Linq.System.Net.
-00003b60: 4874 7470 1053 7973 7465 6d2e 5468 7265  Http.System.Thre
-00003b70: 6164 696e 6716 5379 7374 656d 2e54 6872  ading.System.Thr
-00003b80: 6561 6469 6e67 2e54 6173 6b73 1453 7973  eading.Tasks.Sys
-00003b90: 7465 6d2e 476c 6f62 616c 697a 6174 696f  tem.Globalizatio
-00003ba0: 6e11 5379 7374 656d 2e52 6566 6c65 6374  n.System.Reflect
-00003bb0: 696f 6e10 5379 7374 656d 2e54 6578 742e  ion.System.Text.
-00003bc0: 4a73 6f6e 0f55 6e64 6572 7461 6c65 4d6f  Json.UndertaleMo
-00003bd0: 644c 6962 1a55 6e64 6572 7461 6c65 4d6f  dLib.UndertaleMo
-00003be0: 644c 6962 2e44 6563 6f6d 7069 6c65 7216  dLib.Decompiler.
-00003bf0: 556e 6465 7274 616c 654d 6f64 4c69 622e  UndertaleModLib.
-00003c00: 4d6f 6465 6c73 2053 6978 4c61 626f 7273  Models SixLabors
-00003c10: 2e49 6d61 6765 5368 6172 702e 466f 726d  .ImageSharp.Form
-00003c20: 6174 732e 506e 6733 01a7 9501 a7aa 01a7  ats.Png3........
-00003c30: cc01 a7ec 01a7 f301 a80e 01a8 1801 a824  ...............$
-00003c40: 01a8 3401 a845 01a8 5c01 a871 01a8 8301  ..4..E..\..q....
-00003c50: a894 01a8 a401 a8bf 01a8 d694 d602 0000  ................
-00003c60: 0006 003a 2009 0a00 5404 000d 0021 1600  ...: ...T....!..
-00003c70: 0b00 3104 0e0d 001e 047b 1000 0102 7902  ..1......{....y.
-00003c80: 0000 0b00 0001 0041 0200 1200 4b80 8a00  .......A....K...
-00003c90: 0b00 1104 0007 000d 0026 0700 1600 1e07  .........&......
-00003ca0: 0045 023d 1500 3302 000b 0049 0200 2000  .E.=..3....I.. .
-00003cb0: 2b02 0016 0063 5400 1f00 1b02 0e07 002c  +....cT........,
-00003cc0: 047b 1200 6202 001d 0001 0279 0200 000b  .{..b......y....
-00003cd0: 0000 0100 0007 004a 0808 2700 4c02 0027  .......J..'.L..'
-00003ce0: 0080 8602 0019 003d 0200 2200 4802 0022  .......=..".H.."
-00003cf0: 0064 0200 1400 1b02 0e07 0029 047b 0e00  .d.........).{..
-00003d00: 3902 001d 0001 0279 0200 000b 0000 0100  9......y........
-00003d10: 4c04 0027 004e 0200 2700 808b 0200 1900  L..'.N..'.......
-00003d20: 3f02 0022 004a 0200 2200 6802 0014 001b  ?..".J..".h.....
-00003d30: 020e 0700 2a04 7b0e 003a 0200 1d00 0102  ....*.{..:......
-00003d40: 7902 0000 0b00 0001 0072 0679 3b00 7802  y........r.y;.x.
-00003d50: 003b 0078 0200 3b00 7e02 003b 006b 0200  .;.x..;.~..;.k..
-00003d60: 3b00 80a6 0200 5600 80a6 0200 5600 80a6  ;.....V.....V...
-00003d70: 0200 5600 80a6 0200 5600 80a6 0200 5600  ..V.....V.....V.
-00003d80: 80a6 0200 5600 80a6 0200 5600 80ae 0400  ....V.....V.....
-00003d90: 5600 80bc 0200 5600 80b4 0200 5600 80b2  V.....V.....V...
-00003da0: 0200 5600 809d 0600 4b00 809f 0200 4b00  ..V.....K.....K.
-00003db0: 8099 0200 4b00 7506 0046 0078 0200 4600  ....K.u..F.x..F.
-00003dc0: 7602 0046 0076 0200 4600 7702 0046 0080  v..F.v..F.w..F..
-00003dd0: a206 004b 0080 a002 004b 0080 a202 004b  ...K.....K.....K
-00003de0: 0080 a202 004b 0080 9f02 004b 0080 9c02  .....K.....K....
-00003df0: 004b 0080 9e02 004b 0080 9d02 004b 0080  .K.....K.....K..
-00003e00: a402 004b 0080 9e02 004b 0080 a002 004b  ...K.....K.....K
-00003e10: 0080 a002 004b 0080 9e02 004b 0080 9e02  .....K.....K....
-00003e20: 004b 0080 9f02 004b 0080 9d02 004b 0080  .K.....K.....K..
-00003e30: a402 004b 0080 9d02 004b 0080 9d02 004b  ...K.....K.....K
-00003e40: 0080 9d02 004b 0032 0600 2000 8099 0200  .....K.2.. .....
-00003e50: 4b00 8099 0200 4b00 8099 0200 4b00 8099  K.....K.....K...
-00003e60: 0200 4b00 8099 0200 4b00 8099 0200 4b00  ..K.....K.....K.
-00003e70: 8099 0200 4b00 8099 0200 4b00 8099 0200  ....K.....K.....
-00003e80: 4b0b 0604 0081 450b 061a 0081 370e 061a  K.....E.....7...
-00003e90: 0082 0f18 0620 0084 2b0b 0634 0081 450b  ..... ..+..4..E.
-00003ea0: 061a 0081 4500 391a 0020 0080 a602 004b  ....E.9.. .....K
-00003eb0: 0080 a602 004b 0080 a602 004b 0080 a602  .....K.....K....
-00003ec0: 004b 0039 0400 2000 80a6 0200 4b00 80a6  .K.9.. .....K...
-00003ed0: 0200 4b00 80a6 0200 4b00 80a6 0200 4b00  ..K.....K.....K.
-00003ee0: 80a6 0200 4b00 80a6 0200 4b00 80a6 0200  ....K.....K.....
-00003ef0: 4b00 80a6 0200 4b00 80a6 0200 4b00 80a7  K.....K.....K...
-00003f00: 0200 4b00 80a7 0200 4b00 80a7 0200 4b00  ..K.....K.....K.
-00003f10: 80a7 0200 4b00 80a7 0200 4b00 80a7 0200  ....K.....K.....
-00003f20: 4b00 80a7 0200 4b0a 0604 0081 1637 0618  K.....K......7..
-00003f30: 008a 9612 0672 0082 e712 0628 0082 e712  .....r.....(....
-00003f40: 0628 0082 e70f 0628 0082 450a 0624 0081  .(.....(..E..$..
-00003f50: 4705 0480 8400 4500 790c 0021 0056 0200  G.....E.y..!.V..
-00003f60: 0c00 2502 0011 0037 0200 0c00 4002 0007  ..%....7....@...
-00003f70: 0031 0200 0800 3902 0007 0024 0200 0800  .1....9....$....
-00003f80: 3402 000e 0030 0200 0700 7502 0022 0075  4....0....u..".u
-00003f90: 0200 0d00 2302 0012 0035 0200 0c00 3c02  ....#....5....<.
-00003fa0: 0007 002f 0200 0900 3502 0007 0024 0200  .../....5....$..
-00003fb0: 0800 3402 000e 002e 0200 0700 2702 0011  ..4.........'...
-00003fc0: 004d 0400 1800 3406 001c 0035 0200 1d00  .M....4....5....
-00003fd0: 4f06 0018 0057 0200 1301 80d2 0200 2700  O....W........'.
-00003fe0: 4808 0018 005f 0200 0d00 5902 0021 0056  H...._....Y..!.V
-00003ff0: 0600 2100 8090 0600 2702 80a6 0600 2700  ..!.....'.....'.
-00004000: 809e 0a00 2700 3c06 0018 0080 8a02 0013  ....'.<.........
-00004010: 0080 8202 0013 0080 8402 0013 007f 0200  ................
-00004020: 1300 5e02 2a2a 0000 0200 0800 6907 0048  ..^.**......i..H
-00004030: 0477 2400 4802 0024 0000 0600 027b 1c08  .w$.H..$.....{..
-00004040: 0180 9a0e 5d27 0068 0600 2700 5906 0021  ....]'.h..'.Y..!
-00004050: 0080 8502 0027 0074 0600 2100 7402 0021  .....'.t..!.t..!
-00004060: 0074 0200 2100 7402 0021 004c 0632 1b00  .t..!.t..!.L.2..
-00004070: 0002 000c 0061 0700 3d02 771e 0000 0600  .....a..=.w.....
-00004080: 027f 2408 002d 0855 1200 6802 0827 0180  ..$..-.U..h..'..
-00004090: da06 7921 0069 0400 2100 7706 0027 007e  ..y!.i..!.w..'.~
-000040a0: 0200 2700 7502 0027 0363 0632 6600 0002  ..'.u..'.c.2f...
-000040b0: 000c 0061 0700 3408 771e 0000 0600 0279  ...a..4.w......y
-000040c0: 2408 0080 900a 5521 0380 e406 0027 0072  $.....U!.....'.r
-000040d0: 0e00 2700 2d02 0007 0057 0200 1c02 6e02  ..'.-....W....n.
-000040e0: 000d 0024 0600 1200 4502 0021 003a 0200  ...$....E..!.:..
-000040f0: 0700 2a02 0009 0033 0200 0700 2002 000c  ..*....3.... ...
-00004100: 0028 0200 0e00 2402 0007 0680 8808 0007  .(....$.........
-00004110: 0080 8e10 322b 0000 0200 0c00 6107 0054  ....2+......a..T
-00004120: 0277 2100 0006 0002 7f24 0800 290a 5507  .w!......$..).U.
-00004130: 005b 022e 1700 0002 000a 0065 0700 2e04  .[.........e....
-00004140: 770f 0031 0208 2f00 0006 0002 7b18 0804  w..1../.....{...
-00004150: 8090 0a59 3304 8086 0a00 3300 250c 0007  ...Y3.....3.%...
-00004160: 001b 022e 1b00 0002 000a 0065 0700 2e04  ...........e....
-00004170: 770f 002d 0208 2f00 0006 0002 7b18 0804  w..-../.....{...
-00004180: 8088 0a59 3304 7e0a 0033 0061 1400 2700  ...Y3.~..3.a..'.
-00004190: 4f06 0021 0055 0632 1b00 0002 000c 0061  O..!.U.2.......a
-000041a0: 0700 7c02 7724 0000 0600 027f 2408 0071  ..|.w$......$..q
-000041b0: 0c55 2200 7402 0022 0021 0200 1200 2202  .U".t..".!....".
-000041c0: 0012 0906 0200 7a09 0614 007d 0078 1800  ......z....}.x..
-000041d0: 2200 2402 0012 002f 0200 1609 0602 0065  ".$..../.......e
-000041e0: 0043 1600 2c00 1002 0009 0036 0200 1800  .C..,......6....
-000041f0: 2c02 0009 0017 0200 0900 1602 0009 003f  ,..............?
-00004200: 0400 2c00 1002 0009 002c 0200 0900 1702  ..,......,......
-00004210: 0009 0016 0200 0900 3f04 002c 0010 0200  ........?..,....
-00004220: 0900 2c02 0009 0017 0200 0900 1602 0009  ..,.............
-00004230: 003f 0400 2c00 1002 0009 002c 0200 0900  .?..,......,....
-00004240: 1702 0009 0015 0200 080a 0404 0065 001d  .............e..
-00004250: 1600 0d0a 0404 0065 001d 1600 0d0a 0404  .......e........
-00004260: 0062 001d 1600 0d0a 0404 0061 001d 1600  .b.........a....
-00004270: 0c00 3506 0018 000b 020a 0700 0005 0023  ..5............#
-00004280: 047f 0700 3502 0028 001a 0200 0900 2104  ....5..(......!.
-00004290: 0007 004d 0200 4900 4402 001e 0018 0200  ...M..I.D.......
-000042a0: 1200 2302 000d 0033 0200 0700 1702 0009  ..#....3........
-000042b0: 002d 0200 0700 1b02 000e 001c 0200 0700  .-..............
-000042c0: 2404 0007 0055 0200 4900 1b02 0012 0026  $....U..I......&
-000042d0: 0200 0d00 2f02 0007 001a 0200 0900 2902  ..../.........).
-000042e0: 0007 001a 0200 0c00 1b02 000e 001f 0200  ................
-000042f0: 0700 1b02 0012 0003 4b30 0600 0800 6d0c  ........K0....m.
-00004300: 0e12 3e5d 1300 501e 0027 0050 0200 2700  ..>]..P..'.P..'.
-00004310: 2606 0007 0048 0200 1c5d 1202 000d 001d  &....H...]......
-00004320: 80bc 0012 0071 0200 3801 817a 0600 1301  .....q..8..z....
-00004330: 817a 0400 1300 80aa 082a 3300 0002 0008  .z.......*3.....
-00004340: 0069 0700 3c02 7724 0000 0600 027f 1c08  .i..<.w$........
-00004350: 0080 ef08 0c3b 0000 0200 0b00 6307 0063  .....;......c..c
-00004360: 0277 2400 0006 0002 7f22 0800 3c08 5718  .w$......"..<.W.
-00004370: 0043 0200 1300 4802 0013 0080 9302 0027  .C....H........'
-00004380: 0080 9302 0027 0168 0200 2700 5404 0018  .....'.h..'.T...
-00004390: 0072 0200 1300 7002 0013 0080 8902 0013  .r....p.........
-000043a0: 0080 af02 0013 0080 8d02 0013 006e 0200  .............n..
-000043b0: 2700 2106 0010 0036 0608 1800 4b02 0018  '.!....6....K...
-000043c0: 004b 0200 1800 4902 0018 004a 0200 1800  .K....I....J....
-000043d0: 3d02 0018 0037 0200 1800 3f02 0018 005c  =....7....?....\
-000043e0: 0200 3100 5502 0031 0056 0200 3200 5502  ..1.U..1.V..2.U.
-000043f0: 0031 0055 0200 3100 5602 0032 0056 0200  .1.U..1.V..2.V..
-00004400: 3200 5602 0032 0056 0200 2e00 5204 002b  2.V..2.V....R..+
-00004410: 0049 0200 2b00 5202 002b 0072 0400 2200  .I..+.R..+.r..".
-00004420: 6602 000d 0021 0200 1200 5902 002c 0069  f....!....Y..,.i
-00004430: 0200 1200 3306 0018 0060 0200 3100 5802  ....3....`..1.X.
-00004440: 0030 005a 0200 3200 5902 0031 005a 0200  .0.Z..2.Y..1.Z..
-00004450: 3200 5902 0031 005a 0200 3200 5a02 0032  2.Y..1.Z..2.Z..2
-00004460: 004f 0600 2b00 4602 002b 004f 0200 2b00  .O..+.F..+.O..+.
-00004470: 4604 0012 006f 0400 2200 6402 000d 001e  F....o..".d.....
-00004480: 0200 1200 5302 002c 005d 0600 3200 3508  ....S..,.]..2.5.
-00004490: 0018 005d 0200 2e00 5602 002e 0057 0200  ...]....V....W..
-000044a0: 2f00 5702 002e 0056 0200 2e00 5702 002f  /.W....V....W../
-000044b0: 0057 0200 2f00 5802 002f 0057 0800 3800  .W../.X../.W..8.
-000044c0: 5602 0038 005e 0200 3200 5004 0028 0047  V..8.^..2.P..(.G
-000044d0: 0200 2800 5002 0028 0049 0400 1200 7104  ..(.P..(.I....q.
-000044e0: 0022 0066 0200 0d00 2002 0012 0056 0200  .".f.... ....V..
-000044f0: 2900 3906 0018 0062 0200 3100 5a02 0030  ).9....b..1.Z..0
-00004500: 005c 0200 3200 5b02 0031 005c 0200 3200  .\..2.[..1.\..2.
-00004510: 5b02 0031 005c 0200 3200 5c02 0032 005f  [..1.\..2.\..2._
-00004520: 0800 3800 5f02 0038 005f 0200 3800 5f02  ..8._..8._..8._.
-00004530: 0038 006f 0200 4500 5504 002b 004c 0200  .8.o..E.U..+.L..
-00004540: 2b00 5502 002b 0075 0400 2200 6802 000d  +.U..+.u..".h...
-00004550: 0024 0200 1200 5f02 002c 004a 0400 1200  .$...._..,.J....
-00004560: 8089 0600 2700 8089 0200 2700 8087 0200  ....'.....'.....
-00004570: 2700 8089 0200 2701 816c 1e79 2701 816c  '.....'..l.y'..l
-00004580: 0400 2701 816c 0400 2701 816c 0400 2700  ..'..l..'..l..'.
-00004590: 80ba 0800 2100 3006 0016 002e 0200 0700  ....!.0.........
-000045a0: 1002 0009 0010 0200 0900 1402 000c 0014  ................
-000045b0: 0200 0c00 3302 0025 0041 0200 1d00 2702  ....3..%.A....'.
-000045c0: 0007 0056 0200 1c00 6f02 000d 001e 0200  ...V....o.......
-000045d0: 1200 2502 0009 0023 0200 0d0b 0602 0080  ..%....#........
-000045e0: 8a0b 0618 0080 8c00 7c1c 0027 0280 9806  ........|..'....
-000045f0: 004d 003f 0a00 1800 6302 0013 0070 0600  .M.?....c....p..
-00004600: 1300 5c06 0027 005c 0200 2701 8094 0600  ..\..'.\..'.....
-00004610: 2701 812c 0e00 0d00 6d0c 0013 0080 8102  '..,....m.......
-00004620: 0013 0055 0200 1300 6a02 0013 004f 0200  ...U....j....O..
-00004630: 1300 6102 0013 0068 0200 1300 4606 0018  ..a....h....F...
-00004640: 0281 5602 0013 0041 0600 1800 6902 0013  ..V....A....i...
-00004650: 087b 0800 1308 7b12 0013 087b 1600 1308  .{....{....{....
-00004660: 7b12 0013 087b 1600 1308 7b12 0013 0047  {....{....{....G
-00004670: 1600 1800 8096 0200 1300 80b5 0200 1309  ................
-00004680: 1206 0013 005a 1400 1301 80e8 0e00 0d00  .....Z..........
-00004690: 3c08 000d 006b 0600 0d00 8080 0600 2600  <....k........&.
-000046a0: 8084 0200 2c01 8104 0600 0d01 80ce 0800  ....,...........
-000046b0: 0d00 5904 0018 087b 0200 1300 7912 0013  ..Y....{....y...
-000046c0: 0063 0400 1808 7b02 0013 0080 8312 0013  .c....{.........
-000046d0: 0059 0400 1808 7b02 0013 0079 1200 1300  .Y....{....y....
-000046e0: 5a04 0018 087b 0200 1300 7612 0013 0281  Z....{....v.....
-000046f0: 4c06 000d 1e1a 0a00 1301 8100 3e00 1300  L...........>...
-00004700: 7b08 0027 004f 0600 1800 4f02 0013 004e  {..'.O....O....N
-00004710: 0200 1800 4802 0013 036b 0428 4b00 0002  ....H....k.(K...
-00004720: 0008 0069 0700 5008 7924 0000 0600 0279  ...i..P.y$.....y
-00004730: 1a08 003e 0a5f 1c00 0c02 3e12 0000 0200  ...>._....>.....
-00004740: 1200 5507 0060 0446 3200 0002 001b 0043  ..U..`.F2......C
-00004750: 0900 4d02 7718 0002 7f42 0b00 000b 0000  ..M.w....B......
-00004760: 0100 027d 670b 0000 0b00 0001 004c 1049  ...}g........L.I
-00004770: 1300 5302 0013 004d 0600 1300 5402 0013  ..S....M....T...
-00004780: 0180 8402 3e36 0000 0200 1200 5509 0041  ....>6......U..A
-00004790: 0477 1300 027d 300b 0000 0b00 0001 004b  .w...}0........K
-000047a0: 0a49 1300 5202 0013 0076 0200 2700 5006  .I..R....v..'.P.
-000047b0: 0018 004a 0200 1300 5002 0013 0181 3a02  ...J....P.....:.
-000047c0: 2836 0000 0200 0800 6909 003d 0479 1300  (6......i..=.y..
-000047d0: 027d 1a0b 0000 0b00 0001 004f 0a5f 1800  .}.........O._..
-000047e0: 4902 0013 004f 0200 1300 8088 0228 2b00  I....O.......(+.
-000047f0: 0002 0008 0069 0700 5002 7924 0000 0600  .....i..P.y$....
-00004800: 027f 1a08 004d 085f 1300 5302 0013 0280  .....M._..S.....
-00004810: 9602 2836 0000 0200 0800 6909 0046 0679  ..(6......i..F.y
-00004820: 1300 027b 1a0b 0000 0b00 0001 0050 0c5f  ...{.........P._
-00004830: 1300 5602 0013 0180 d602 2836 0000 0200  ..V.......(6....
-00004840: 0800 6909 0049 0479 1300 027d 1a0b 0000  ..i..I.y...}....
-00004850: 0b00 0001 004e 0c5f 1300 5502 0013 056b  .....N._..U....k
-00004860: 0228 809c 0000 0200 0800 6907 0056 0c79  .(........i..V.y
-00004870: 2400 0006 0002 751a 0800 4b14 5f13 0051  $.....u...K._..Q
-00004880: 0200 1304 6b04 2880 8a00 0002 0008 0069  ....k.(........i
-00004890: 0700 520a 7924 0000 0600 0277 1a08 004a  ..R.y$.....w...J
-000048a0: 105f 1800 4802 0013 0050 0200 1300 4806  ._..H....P....H.
-000048b0: 0013 0050 0200 1300 8089 0228 2b00 0002  ...P.......(+...
-000048c0: 0008 0069 0700 5702 7924 0000 0600 027f  ...i..W.y$......
-000048d0: 1a08 0048 085f 1300 5002 0013 0048 0600  ...H._..P....H..
-000048e0: 1300 5002 0013 0048 0600 1300 5002 0013  ..P....H....P...
-000048f0: 081a 0600 1308 1a12 0013 081a 1200 1312  ................
-00004900: 1a12 0013 0812 2800 1300 7e16 0061 0067  ......(...~..a.g
-00004910: 0600 2700 6602 0021 0060 0200 2100 3a06  ..'.f..!.`..!.:.
-00004920: 2a36 0000 0200 0800 6909 0041 0277 1200  *6......i..A.w..
-00004930: 027f 1c0b 0000 0b00 0001 0040 085d 0d00  ...........@.]..
-00004940: 4302 0018 0480 ca02 0013 1012 0e00 2100  C.............!.
-00004950: 6f22 0027 0712 0200 2127 1210 0027 0712  o".'....!'...'..
-00004960: 5000 2100 6810 0021 0812 0200 2100 2a16  P.!.h..!....!.*.
-00004970: 0007 0052 0200 1c2d 1202 000d 0021 5c00  ...R...-.....!\.
-00004980: 1200 7b02 0038 002a 0400 0700 5202 001c  ..{..8.*....R...
-00004990: 2612 0200 0d00 214e 0012 007a 0200 3800  &.....!N...z..8.
-000049a0: 3804 0018 0080 8102 0013 002e 0200 1300  8...............
-000049b0: 3802 0013 0038 0400 1800 2e02 0013 0075  8....8.........u
-000049c0: 0200 1300 7202 0013 0d1a 0200 1300 7720  ....r.........w 
-000049d0: 0061 0460 0200 1300 4710 0018 0035 0200  .a.`....G....5..
-000049e0: 1300 7c02 0013 006c 042a 2b00 0002 0008  ..|....l.*+.....
-000049f0: 0069 0700 3f02 7724 0000 0600 027f 1c08  .i..?.w$........
-00004a00: 0040 085d 2500 4402 0025 0080 8006 004b  .@.]%.D..%.....K
-00004a10: 0080 9d02 003d 0018 064a 0d00 0005 0018  .....=...J......
-00004a20: 0049 1a00 0d04 7702 0000 808e 0059 0610  .I....w......Y..
-00004a30: 4001 80ec 0200 8086 0006 0400 0500 5d04  @.............].
-00004a40: 0040 0006 0200 0500 5f04 0040 0006 0200  .@......_..@....
-00004a50: 0500 5904 0040 0006 0200 0500 0004 0023  ..Y..@.........#
-00004a60: 1a0e 1c00 4802 7313 0006 0200 0500 5d06  ....H.s.......].
-00004a70: 0040 0006 0200 0500 6504 0040 0006 0200  .@......e..@....
-00004a80: 0500 6704 0040 0006 0200 0500 6304 0040  ..g..@......c..@
-00004a90: 0006 0200 0500 5f04 0040 0006 0200 0500  ......_..@......
-00004aa0: 5d04 0040 0006 0200 0500 6504 0040 0006  ]..@......e..@..
-00004ab0: 0200 0500 6b04 0040 0006 0200 0500 6904  ....k..@......i.
-00004ac0: 0040 0006 0200 0500 6104 0040 0006 0200  .@......a..@....
-00004ad0: 0500 5d0a 0040 0006 0200 0500 5d04 0040  ..]..@......]..@
-00004ae0: 0006 0200 0500 5d04 0040 0006 0200 0500  ......]..@......
-00004af0: 5d04 0040 0006 0200 0500 5d04 0040 0006  ]..@......]..@..
-00004b00: 0200 0200 5d04 0040 0006 0200 0200 2808  ....]..@......(.
-00004b10: 0006 0002 bf51 2c0e 0000 0e00 7180 ba3d  .....Q,.....q..=
-00004b20: 1c00 6002 0813 0074 0279 1c00 6202 0813  ..`....t.y..b...
-00004b30: 006a 0279 1c00 5c02 0813 0080 8006 793d  .j.y..\.......y=
-00004b40: 007a 0200 3d08 1206 0027 0062 1200 2701  .z..=....'.b..'.
-00004b50: 8172 0800 270e 120a 0013 0051 1e00 2700  .r..'......Q..'.
-00004b60: 5102 0027 0032 0600 1800 0c02 2a12 0000  Q..'.2......*...
-00004b70: 0200 0800 6907 0052 0420 3000 0002 0008  ....i..R. 0.....
-00004b80: 0069 0700 1f04 7707 0002 7d1c 0b00 000b  .i....w...}.....
-00004b90: 0000 0100 027d 790b 0000 0b00 0001 0013  .....}y.........
-00004ba0: 105d 0900 1906 0007 0014 0246 0d00 0005  .].........F....
-00004bb0: 0016 004d 1c00 1304 7703 000c 022a 1200  ...M....w....*..
-00004bc0: 0005 0008 0069 0900 1004 2c0e 0000 0500  .....i....,.....
-00004bd0: 0e00 5d09 0020 0477 0e00 4204 001d 0055  ..].. .w..B....U
-00004be0: 0208 3800 0d04 7903 0024 0200 0c00 7304  ..8...y..$....s.
-00004bf0: 086e 0016 0200 1200 1f02 0009 1c04 0679  .n.............y
-00004c00: 7900 1704 360c 003b 0202 3900 3b02 0a39  y...6..;..9.;..9
-00004c10: 003b 0273 3900 2d02 020c 002d 0200 0c00  .;.s9.-....-....
-00004c20: 2d02 7d0c 002d 0204 0c00 2d02 000c 002d  -.}..-....-....-
-00004c30: 027b 0c00 2d02 020c 002d 0204 0c00 2d02  .{..-....-....-.
-00004c40: 7f0c 002d 020e 0c00 2d02 7d0c 002d 0204  ...-....-.}..-..
-00004c50: 0c00 2d02 000c 002d 027d 0c00 2d02 000c  ..-....-.}..-...
-00004c60: 002d 0202 0900 2d02 7d09 002d 0206 0900  .-....-.}..-....
-00004c70: 2d02 7309 002d 0200 0900 2d02 0009 005d  -.s..-....-....]
-00004c80: 025f 5200 0004 0033 066f 0f00 1102 0006  ._R....3.o......
-00004c90: 0006 0200 0200 0223 280e 0000 0b00 0001  .......#(.......
-00004ca0: 000a 6451 0400 0600 1602 0002 1906 0e00  ..dQ............
-00004cb0: 000b 0000 0100 0b6e 5d04 0043 0208 3800  .......n]..C..8.
-00004cc0: 020b 300e 0000 0e00 1880 8024 0d00 0005  ..0........$....
-00004cd0: 0025 002f 1c00 3504 7715 0043 0200 2400  .%./..5.w..C..$.
-00004ce0: 1c02 0009 006a 0208 5700 3904 7925 0180  .....j..W.9.y%..
-00004cf0: 8802 0080 8e00 3c08 0025 3f04 0200 80a3  ......<..%?.....
-00004d00: 0022 0436 0c00 1f02 0c0c 0181 0002 7f0c  .".6............
-00004d10: 0024 040c 0c01 810a 027f 0c00 2104 730c  .$..........!.s.
-00004d20: 0180 ec02 000c 0000 0400 2304 591c 0045  ..........#.Y..E
-00004d30: 004e 0c00 6202 4b0c 0055 0206 0c00 6c02  .N..b.K..U....l.
-00004d40: 040c 0069 0200 0c00 8085 0202 0c10 6b02  ...i..........k.
-00004d50: 750c 007f 2208 0900 5902 0609 004d 0275  u..."...Y....M.u
-00004d60: 0910 6702 0209 0061 227f 0900 4b02 7b09  ..g....a"...K.{.
-00004d70: 004b 0202 0900 4b02 0409 004b 0200 0900  .K....K....K....
-00004d80: 4f02 0609 0014 027d 0900 4902 6322 0000  O......}..I.c"..
-00004d90: 0400 3404 6f0a 0002 bf67 560e 0000 0e07  ..4.o....gV.....
-00004da0: 7b80 a223 7107 7b12 0071 077b 1200 7100  {..#q.{..q.{..q.
-00004db0: 5616 002c 0181 2002 0876 005b 0679 2c01  V..,.. ..v.[.y,.
-00004dc0: 812c 0208 7600 5406 792c 0181 1802 0876  .,..v.T.y,.....v
-00004dd0: 0712 0a79 809b 0046 1600 0e00 4402 000d  ...y...F....D...
-00004de0: 0049 0200 0d00 5802 000e 1312 0200 80a2  .I....X.........
-00004df0: 0026 2c00 0d00 5e02 0813 004d 0222 3600  .&,...^....M."6.
-00004e00: 0002 0008 0069 0900 4302 770d 0002 7f1c  .....i..C.w.....
-00004e10: 0b00 000b 0000 0100 0c06 1a12 0000 0200  ................
-00004e20: 1200 5507 0060 0446 3200 0002 001b 0043  ..U..`.F2......C
-00004e30: 0901 6c02 7718 0002 7f42 0b00 000b 0000  ..l.w....B......
-00004e40: 0100 027d 670b 0000 0b00 0001 0150 0c49  ...}g........P.I
-00004e50: 2700 270c 000d 0060 0208 1300 80ca 042a  '.'....`.......*
-00004e60: 4300 0002 000c 0061 0700 7702 771e 0000  C......a..w.w...
-00004e70: 0600 027f 2408 000a 065f 0400 0002 007f  ....$...._......
-00004e80: 027f 4e00 037f 2c06 0007 006f 0600 2808  ..N...,....o..(.
-00004e90: 5f0d 0051 0208 1301 3802 7927 002a 0800  _..Q....8.y'.*..
-00004ea0: 0d00 6702 0813 2912 0679 2700 6858 3646  ..g...)..y'.hX6F
-00004eb0: 0000 0200 0e00 5d09 0017 0677 0b03 1202  ......]....w....
-00004ec0: 0818 0017 0c79 0b00 5f02 0812 0002 6b20  .....y.._.....k 
-00004ed0: 0b00 000b 0000 0100 681e 0646 0000 0200  ........h..F....
-00004ee0: 0e00 5d09 002d 0477 1601 4202 0818 0002  ..]..-.w..B.....
-00004ef0: 7b20 0b00 000b 0000 0100 6710 0646 0000  { ........g..F..
-00004f00: 0200 0e00 5d09 0142 0477 1800 027d 280b  ....]..B.w...}(.
-00004f10: 0000 0b00 0001 0067 0e06 4600 0002 000e  .......g..F.....
-00004f20: 005d 0900 2e04 7716 0142 0208 1800 027b  .]....w..B.....{
-00004f30: 200b 0000 0b00 0001 006c 0e06 4600 0002   ........l..F...
-00004f40: 000e 005d 0900 1706 770b 0412 0208 1800  ...]....w.......
-00004f50: 180e 790e 005f 0208 1200 0269 200b 0000  ..y.._.....i ...
-00004f60: 0b00 0001 004c 2208 1b00 0002 000f 005b  .....L"........[
-00004f70: 0700 8087 0277 2400 0006 0002 7f2a 0801  .....w$......*..
-00004f80: 2408 4f27 0124 0400 2700 809b 0800 2100  $.O'.$..'.....!.
-00004f90: 2906 000d 0064 0208 1300 0c02 3612 0000  )....d......6...
-00004fa0: 0500 1200 5509 0010 041c 0e00 0005 0006  ....U...........
-00004fb0: 006d 0900 5a06 7731 001c 0400 0c00 8088  .m..Z.w1........
-00004fc0: 0408 6700 1602 0012 0017 0200 0900 5204  ..g...........R.
-00004fd0: 7912 0002 6b18 0e00 000b 0000 0100 027d  y...k..........}
-00004fe0: 100e 0000 0b00 0001 005d 2649 2700 5f02  .........]&I'._.
-00004ff0: 0027 0029 0600 0d00 5d02 0813 1412 0279  .'.)....]......y
-00005000: 2707 1a2c 0027 0080 af12 0027 0080 af02  '..,.'.....'....
-00005010: 0027 0180 ce0a 0021 0025 0800 0d00 5c04  .'.....!.%....\.
-00005020: 0813 0061 0879 2100 4d04 000d 0b12 0400  ...a.y!.M.......
-00005030: 2100 4f1a 000d 004f 0400 0d00 4f04 000d  !.O....O....O...
-00005040: 1912 0400 2100 5336 000d 0081 3b04 0021  ....!.S6....;..!
-00005050: 0081 3804 0021 005d 0400 2100 1614 520d  ..8..!.]..!...R.
-00005060: 0000 0200 1c00 411a 0020 0477 0700 2802  ......A.. .w..(.
-00005070: 0009 002f 0400 1500 4602 001e 0002 7544  .../....F.....uD
-00005080: 0b00 000e 0080 9014 3557 0512 0600 7800  ........5W....x.
-00005090: 691a 0027 0080 a804 0027 0080 ae04 0038  i..'.....'.....8
-000050a0: 0080 8f04 0027 005f 0a00 2700 5f02 0027  .....'._..'._..'
-000050b0: 1412 0400 2106 122c 0027 0712 1000 2704  ....!..,.'....'.
-000050c0: 1212 0027 0612 0c00 271d 120e 0027 1712  ...'....'....'..
-000050d0: 3e00 85f4 005c 3600 3b00 6f02 0021 005c  >....\6.;.o..!.\
-000050e0: 0400 3e00 6f02 0021 005c 0400 3b00 6f02  ..>.o..!.\..;.o.
-000050f0: 0021 005c 0400 3e00 6f02 0021 005b 0400  .!.\..>.o..!.[..
-00005100: 3b00 6e02 0021 005c 0400 3e00 6f02 0021  ;.n..!.\..>.o..!
-00005110: 005c 0400 3e00 6f02 0021 0038 0e0e 0d00  .\..>.o..!.8....
-00005120: 3104 7b28 0001 0279 0200 000b 0000 0100  1.{(...y........
-00005130: 0102 7905 0980 1a06 0005 0981 1a06 0005  ..y.............
-00005140: 0982 1a06 0005 0800 0400 0006 0000 0035  ...............5
-00005150: 1505 1500 0000 5f17 050b 0059 0800 0b00  ......_....Y....
-00005160: 5108 000b 004f 1000 2553 7973 7465 6d2e  Q....O..%System.
-00005170: 436f 6d70 6f6e 656e 744d 6f64 656c 2e44  ComponentModel.D
-00005180: 6174 6141 6e6e 6f74 6174 696f 6e73 1c53  ataAnnotations.S
-00005190: 7973 7465 6d2e 5275 6e74 696d 652e 5365  ystem.Runtime.Se
-000051a0: 7269 616c 697a 6174 696f 6e1e 5379 7374  rialization.Syst
-000051b0: 656d 2e54 6578 742e 4a73 6f6e 2e53 6572  em.Text.Json.Ser
-000051c0: 6961 6c69 7a61 7469 6f6e 2a01 a795 01a7  ialization*.....
-000051d0: aa01 a7cc 01a7 ec01 a7f3 01a8 0e01 a818  ................
-000051e0: 01a8 2401 a834 01a8 4501 be38 01be 5e01  ..$..4..E..8..^.
-000051f0: a883 01be 7b0c 0000 0018 80ac 050b 001c  ....{...........
-00005200: 0800 0700 0000 2481 7805 0c00 0000 2681  ......$.x.....&.
-00005210: 8205 0b00 3208 0007 0000 001f 818d 0507  ....2...........
-00005220: 0000 0018 8346 3207 0000 0018 834d 2e07  .....F2......M..
-00005230: 0000 0018 8353 2e07 0000 0018 8359 2e07  .....S.......Y..
-00005240: 0000 0018 8480 3107 0000 0018 8490 4907  ......1.......I.
-00005250: 0000 0017 8491 4907 0000 0017 8492 3307  ......I.......3.
-00005260: 0000 0018 84ac 5107 0000 0018 84ad 5107  ......Q.......Q.
-00005270: 0000 0018 84ae 5107 0000 0018 84af 5107  ......Q.......Q.
-00005280: 0000 0154 8612 3f08 0000 0181 0a86 1f34  ...T..?........4
-00005290: 0700 0002 6686 2d34 0800 0001 80a6 8635  ....f.-4.......5
-000052a0: 3407 0000 0021 86ab 3607 0000 0034 8830  4....!..6....4.0
-000052b0: 3f07 0000 002f 88d1 4907 0000 0034 88da  ?..../..I....4..
-000052c0: 4a07 0000 002d 88e3 4707 0000 002e 88e8  J....-..G.......
-000052d0: 2f07 0000 002e 88ea 5a07 0000 0033 88ec  /.......Z....3..
-000052e0: 2f07 0000 0033 88ee 5b07 0000 002c 88f0  /....3..[....,..
-000052f0: 2f07 0000 002c 88f2 5807 0000 0035 891d  /....,..X....5..
-00005300: 3507 0000 0030 896c 5b07 0000 0030 897b  5....0.l[....0.{
-00005310: 5b07 0000 002f 8983 5b07 0000 002f 898a  [..../..[..../..
-00005320: 5b07 0000 0034 8991 5b06 0000 0034 380d  [....4..[....48.
-00005330: 1f03 0000 3c3d 0d0e 0037 0200 0d00 6a02  ....<=...7....j.
-00005340: 0855 003c 0279 0900 2202 000d 0001 0279  .U.<.y.."......y
-00005350: 1504 0000 3c46 0d0e 002b 0200 0d00 2202  ....<F...+....".
-00005360: 000d 0001 0279 1504 0000 3c4d 0d0e 002a  .....y....<M...*
-00005370: 0200 0d00 2202 000d 0001 0279 0b00 0000  ...."......y....
-00005380: 2454 0d0d 0001 0279 0b05 0000 2559 0d35  $T.....y....%Y.5
-00005390: 0b04 0200 0b05 0000 246a 0d35 0904 0200  ........$j.5....
-000053a0: 80a8 0600 0021 8083 2709 0000 0200 0d00  .....!..'.......
-000053b0: 5f04 001d 0477 0700 0004 0002 7d26 0600  _....w......}&..
-000053c0: 1b0a 0409 0000 0500 0c00 6104 0000 0700  ..........a.....
-000053d0: 2204 770d 0041 0200 1d00 2f02 001d 000e  ".w..A..../.....
-000053e0: 0408 0700 2002 0013 0027 0200 1400 2104  .... ....'....!.
-000053f0: 0013 0080 8302 084f 0030 0671 1a00 6d02  .......O.0.q..m.
-00005400: 083b 0017 0479 0d00 1702 000d 004e 0200  .;...y.......N..
-00005410: 1800 2e02 0007 0022 0200 0f00 2202 000f  ......."...."...
-00005420: 005c 0200 2c00 6002 002c 0025 0200 0d00  .\..,.`..,.%....
-00005430: 2602 0012 001e 0200 1b00 6602 0023 0000  &.........f..#..
-00005440: 0400 0249 2409 0001 3c4d 0700 0000 4286  ...I$...<M....B.
-00005450: 0652 0700 0000 4289 2252 0700 0000 3180  .R....B."R....1.
-00005460: 9b2c 0700 0000 6a80 b326 0700 0000 4a80  .,....j..&....J.
-00005470: b625 0700 0000 6e80 bf27 0700 0000 4d80  .%....n..'....M.
-00005480: c226 0000                                .&..
+00000150: 0100 7f27 0100 2b29 0000 0000 0100 993e  ...'..+).......>
+00000160: 0100 a03e 0200 d03e 0000 0000 0000 0000  ...>...>........
+00000170: 0000 0000 0200 733f 0000 0000 0000 0000  ......s?........
+00000180: 0200 8a3f 0200 923f 0200 9f3f 0000 0000  ...?...?...?....
+00000190: 0000 0000 0100 a73f 0100 af3f 0100 b73f  .......?...?...?
+000001a0: 0100 bf3f 0100 c73f 0100 cf3f 0100 d73f  ...?...?...?...?
+000001b0: 0100 df3f 0100 e73f 0100 ef3f 0100 f73f  ...?...?...?...?
+000001c0: 0100 ff3f 0100 0740 0100 0f40 0100 1840  ...?...@...@...@
+000001d0: 0100 2040 0100 2940 0100 3140 0100 3940  .. @..)@..1@..9@
+000001e0: 0100 4140 0100 4940 0100 5140 0100 5940  ..A@..I@..Q@..Y@
+000001f0: 0100 6140 0100 6940 0100 7140 0100 7940  ..a@..i@..q@..y@
+00000200: 0100 8140 0100 8940 0100 9140 0100 9940  ...@...@...@...@
+00000210: 0100 a140 0100 a940 0000 0000 0100 b140  ...@...@.......@
+00000220: 0100 b840 0100 d840 0100 ee40 0100 0441  ...@...@...@...A
+00000230: 0100 1041 0100 1c41 0100 2841 0100 d241  ...A...A..(A...A
+00000240: 0100 da41 0000 0000 0100 e241 0000 0000  ...A.......A....
+00000250: 0100 ea41 0100 f241 0100 fa41 0100 0242  ...A...A...A...B
+00000260: 0000 0000 0100 0a42 0600 0300 0100 0100  .......B........
+00000270: 0000 0000 6900 0000 0700 0300 0200 0100  ....i...........
+00000280: 0000 0000 f2a3 0000 0700 0300 3600 0500  ............6...
+00000290: 2800 0000 2b00 0000 0700 0300 3700 0500  (...+.......7...
+000002a0: fa00 0000 4400 0000 0700 0300 3800 0500  ....D.......8...
+000002b0: 3e01 0000 0502 0000 0700 0300 3b00 0500  >...........;...
+000002c0: 0402 0000 4000 0000 0700 0300 3c00 0500  ....@.......<...
+000002d0: 0303 0000 4000 0000 0700 0300 3d00 0500  ....@.......=...
+000002e0: 743c 0000 2000 0000 0700 0300 3e00 0500  t<.. .......>...
+000002f0: fc3c 0000 2000 0000 0700 0300 3f00 0500  .<.. .......?...
+00000300: a53d 0000 2000 0000 0700 0300 4000 0500  .=.. .......@...
+00000310: 4141 0000 4f00 0000 0700 0300 4100 0500  AA..O.......A...
+00000320: d542 0000 2500 0000 0700 0300 4200 0500  .B..%.......B...
+00000330: 6044 0000 2500 0000 0700 0300 4300 0500  `D..%.......C...
+00000340: d145 0000 2800 0000 0700 0300 4400 0500  .E..(.......D...
+00000350: 2746 0000 4500 0000 0700 0300 4500 0500  'F..E.......E...
+00000360: 0447 0000 4500 0000 0700 0300 4600 0500  .G..E.......F...
+00000370: 9148 0000 2b00 0000 0700 0300 4700 0500  .H..+.......G...
+00000380: 074e 0000 c801 0000 0700 0300 4800 0500  .N..........H...
+00000390: 134e 0000 aa01 0000 0700 0300 4d00 0500  .N..........M...
+000003a0: 0551 0000 2b00 0000 0700 0300 4e00 0500  .Q..+.......N...
+000003b0: 7b51 0000 2b00 0000 0700 0300 4f00 0500  {Q..+.......O...
+000003c0: 1553 0000 d50d 0000 0700 0300 5e00 0500  .S..........^...
+000003d0: 0b69 0000 2b00 0000 0700 0300 5f00 0500  .i..+......._...
+000003e0: af69 0000 2100 0000 0700 0300 6000 0500  .i..!.......`...
+000003f0: 826a 0000 1c00 0000 0700 0300 6100 0500  .j..........a...
+00000400: 786b 0000 1c00 0000 0700 0300 6200 0500  xk..........b...
+00000410: 166c 0000 2b00 0000 0700 0300 6300 0500  .l..+.......c...
+00000420: ad6c 0000 1c00 0000 0700 0300 6400 0500  .l..........d...
+00000430: 3e6d 0000 1c00 0000 0700 0300 6500 0500  >m..........e...
+00000440: 356e 0000 2b00 0000 0700 0300 6600 0500  5n..+.......f...
+00000450: 206f 0000 2b00 0000 0700 0300 6700 0500   o..+.......g...
+00000460: ea6f 0000 2b00 0000 0700 0300 6800 0500  .o..+.......h...
+00000470: f671 0000 1b00 0000 0700 0300 6900 0500  .q..........i...
+00000480: db75 0000 2b00 0000 0700 0300 6a00 0500  .u..+.......j...
+00000490: f876 0000 cc06 0000 0700 0300 6b00 0500  .v..........k...
+000004a0: 3c79 0000 3800 0000 0700 0300 6c00 0500  <y..8.......l...
+000004b0: 8080 0000 5304 0000 0700 0300 6e00 0500  ....S.......n...
+000004c0: 9c80 0000 3704 0000 0700 0300 6f00 0500  ....7.......o...
+000004d0: b680 0000 c703 0000 0700 0300 7000 0500  ............p...
+000004e0: d280 0000 8b03 0000 0700 0300 7100 0500  ............q...
+000004f0: db80 0000 8203 0000 0700 0300 7200 0500  ............r...
+00000500: 4d81 0000 8900 0000 0700 0300 7300 0500  M...........s...
+00000510: 0185 0000 8b03 0000 0700 0300 7500 0500  ............u...
+00000520: 1d85 0000 6f03 0000 0700 0300 7900 0500  ....o.......y...
+00000530: 8587 0000 2c00 0000 0700 0300 7a00 0500  ....,.......z...
+00000540: ac8d 0000 1600 0000 0700 0300 7b00 0500  ............{...
+00000550: 288e 0000 2100 0000 0700 0300 7c00 0500  (...!.......|...
+00000560: 038f 0000 2500 0000 0700 0300 7d00 0500  ....%.......}...
+00000570: 368f 0000 6000 0000 0700 0300 7e00 0500  6...`.......~...
+00000580: 6c90 0000 4900 0000 0700 0300 7f00 0500  l...I...........
+00000590: 1491 0000 3700 0000 0700 0300 8000 0500  ....7...........
+000005a0: aa91 0000 2100 0000 0700 0300 8100 0500  ....!...........
+000005b0: 2a92 0000 3700 0000 0700 0300 8200 0500  *...7...........
+000005c0: c092 0000 4c00 0000 0700 0300 8300 0500  ....L...........
+000005d0: 4093 0000 2b00 0000 0700 0300 8400 0500  @...+...........
+000005e0: 1f94 0000 1001 0000 0700 0300 8500 0500  ................
+000005f0: 3b94 0000 da00 0000 0700 0300 8600 0500  ;...............
+00000600: 8194 0000 8200 0000 0700 0300 8700 0500  ................
+00000610: ca97 0000 5d00 0000 0700 0300 8800 0500  ....]...........
+00000620: e497 0000 4300 0000 0700 0300 8a00 0500  ....C...........
+00000630: aea3 0000 4300 0000 0900 0300 8b00 0500  ....C...........
+00000640: 0000 0000 0b00 0000 0a00 0300 8b00 0500  ................
+00000650: 0000 0000 8000 0000 0b00 0500 8e00 0500  ................
+00000660: 0000 0000 3300 0000 0f00 0500 8e00 0500  ....3...........
+00000670: 0000 0000 3300 0000 1200 0500 8e00 0500  ....3...........
+00000680: 0000 0000 1200 0000 1300 0500 8e00 0500  ................
+00000690: 0000 0000 1d00 0000 1400 0500 8e00 0500  ................
+000006a0: 0000 0000 1200 0000 1700 0300 8e00 0500  ................
+000006b0: 0000 0000 0e00 0000 1800 0300 8e00 0500  ................
+000006c0: 0000 0000 0e00 0000 1900 0300 8e00 0500  ................
+000006d0: 0000 0000 0e00 0000 1a00 0300 8e00 0500  ................
+000006e0: 0000 0000 0e00 0000 1b00 0300 8e00 0500  ................
+000006f0: 0000 0000 1d00 0000 1c00 0300 8e00 0500  ................
+00000700: 0000 0000 1a00 0000 1d00 0300 8e00 0500  ................
+00000710: 0000 0000 1a00 0000 1e00 0300 8e00 0500  ................
+00000720: 0000 0000 1a00 0000 1f00 0300 8e00 0500  ................
+00000730: 0000 0000 1d00 0000 2000 0300 8e00 0500  ........ .......
+00000740: 0000 0000 1d00 0000 2100 0300 8e00 0500  ........!.......
+00000750: 0000 0000 1d00 0000 2200 0300 8e00 0500  ........".......
+00000760: 0000 0000 1d00 0000 2300 0300 8e00 0500  ........#.......
+00000770: 0000 0000 4300 0000 2400 0300 8e00 0500  ....C...$.......
+00000780: 0000 0000 5a00 0000 2500 0300 8e00 0500  ....Z...%.......
+00000790: 0000 0000 5a00 0000 2600 0300 8e00 0500  ....Z...&.......
+000007a0: 0000 0000 4300 0000 2700 0300 8e00 0500  ....C...'.......
+000007b0: 0000 0000 1600 0000 2800 0300 8e00 0500  ........(.......
+000007c0: 0000 0000 1b00 0000 2900 0300 8e00 0500  ........).......
+000007d0: 0000 0000 1100 0000 2a00 0300 8e00 0500  ........*.......
+000007e0: 0000 0000 1100 0000 2b00 0300 8e00 0500  ........+.......
+000007f0: 0000 0000 1100 0000 2c00 0300 8e00 0500  ........,.......
+00000800: 0000 0000 1100 0000 2d00 0300 8e00 0500  ........-.......
+00000810: 0000 0000 1100 0000 2e00 0300 8e00 0500  ................
+00000820: 0000 0000 1100 0000 2f00 0300 8e00 0500  ......../.......
+00000830: 0000 0000 1100 0000 3000 0300 8e00 0500  ........0.......
+00000840: 0000 0000 1100 0000 3100 0300 8e00 0500  ........1.......
+00000850: 0000 0000 1100 0000 3200 0300 8e00 0500  ........2.......
+00000860: 0000 0000 1600 0000 3300 0300 8e00 0500  ........3.......
+00000870: 0000 0000 1b00 0000 3400 0300 8e00 0500  ........4.......
+00000880: 0000 0000 1b00 0000 3500 0300 8e00 0500  ........5.......
+00000890: 0000 0000 1b00 0000 3600 0300 8e00 0500  ........6.......
+000008a0: 0000 0000 1b00 0000 3700 0300 8e00 0500  ........7.......
+000008b0: 0000 0000 1b00 0000 3900 0300 8e00 0500  ........9.......
+000008c0: 0000 0000 0e00 0000 3a00 0300 8e00 0500  ........:.......
+000008d0: 0000 0000 8700 0000 3b00 0300 8f00 0500  ........;.......
+000008e0: 0000 0000 2900 0000 3c00 0300 9000 0500  ....)...<.......
+000008f0: 0000 0000 2900 0000 3d00 0300 9100 0500  ....)...=.......
+00000900: 0000 0000 0e00 0000 3e00 0300 9100 0500  ........>.......
+00000910: 0000 0000 8500 0000 3f00 0300 9100 0500  ........?.......
+00000920: 0000 0000 7700 0000 4000 0300 9100 0500  ....w...@.......
+00000930: 0000 0000 7f02 0000 4000 0300 9100 0500  ........@.......
+00000940: 0b00 0000 0b00 0000 4000 0300 9200 0500  ........@.......
+00000950: 2e00 0000 4302 0000 4000 0300 9300 0500  ....C...@.......
+00000960: 3200 0000 3f02 0000 4100 0300 9500 0500  2...?...A.......
+00000970: 0000 0000 1d00 0000 4200 0300 9500 0500  ........B.......
+00000980: 0000 0000 1d00 0000 4400 0300 9500 0500  ........D.......
+00000990: 0000 0000 2400 0000 4600 0300 9500 0500  ....$...F.......
+000009a0: 0000 0000 3900 0000 4700 0300 9500 0500  ....9...G.......
+000009b0: 0000 0000 3100 0000 4800 0300 9500 0500  ....1...H.......
+000009c0: 0000 0000 3900 0000 4900 0300 9500 0500  ....9...I.......
+000009d0: 0000 0000 3100 0000 4b00 0300 9500 0500  ....1...K.......
+000009e0: 0000 0000 4000 0000 0000 0000 a205 0000  ....@...........
+000009f0: 0000 0100 0000 0100 d003 0000 0200 7302  ..............s.
+00000a00: 0000 0300 4d02 0000 0400 1e03 0000 0500  ....M...........
+00000a10: 9204 0000 0600 8203 0000 0700 cc01 0000  ................
+00000a20: 0800 9801 0000 0900 4f01 0000 0a00 4c05  ........O.....L.
+00000a30: 0000 0b00 f302 0000 0c00 3203 0000 0d00  ..........2.....
+00000a40: fe04 0000 0e00 2405 0000 0f00 5b03 0000  ......$.....[...
+00000a50: 1000 4703 0000 1100 4800 0000 1200 5800  ..G.....H.....X.
+00000a60: 0000 1300 3500 0000 1400 0802 0000 1500  ....5...........
+00000a70: 8604 0000 1600 0604 0000 1700 7303 0000  ............s...
+00000a80: 1800 5f01 0000 1900 2100 0000 1a00 9602  .._.....!.......
+00000a90: 0000 1b00 6b01 0000 1c00 ea00 0000 1d00  ....k...........
+00000aa0: d900 0000 1e00 3501 0000 1f00 7801 0000  ......5.....x...
+00000ab0: 2000 d404 0000 2100 b904 0000 2200 a504   .....!....."...
+00000ac0: 0000 2300 ea04 0000 2400 9403 0000 2500  ..#.....$.....%.
+00000ad0: 3b05 0000 2600 5305 0000 2700 6505 0000  ;...&.S...'.e...
+00000ae0: 2800 0b05 0000 2900 1102 0000 2a00 bc01  (.....).....*...
+00000af0: 0000 2b00 ac01 0000 2c00 6802 0000 2d00  ..+.....,.h...-.
+00000b00: b600 0000 2e00 be03 0000 2f00 b403 0000  ........../.....
+00000b10: 3000 8405 0000 3100 9305 0000 3200 7705  0.....1.....2.w.
+00000b20: 0000 3300 1204 0000 3400 bb03 0000 3600  ..3.....4.....6.
+00000b30: cd03 0000 3700 1100 0000 3800 fc01 0000  ....7.....8.....
+00000b40: 3900 ef01 0000 3a00 cd03 0000 3b00 cd03  9.....:.....;...
+00000b50: 0000 3d00 ab05 0000 3e00 ab05 0000 4000  ..=.....>.....@.
+00000b60: 7002 0000 4200 de01 0000 4300 1e02 0000  p...B.....C.....
+00000b70: 4400 1e02 0000 4500 1e02 0000 4700 af00  D.....E.....G...
+00000b80: 0000 4900 af00 0000 4a00 1e02 0000 4c00  ..I.....J.....L.
+00000b90: 8b02 0000 4d00 7f03 0000 4e00 6102 0000  ....M.....N.a...
+00000ba0: 4f00 4003 0000 5000 9e04 0000 5100 0603  O.@...P.....Q...
+00000bb0: 0000 5200 4802 0000 5300 4802 0000 5400  ..R.H...S.H...T.
+00000bc0: d702 0000 5500 7304 0000 5600 2d04 0000  ....U.s...V.-...
+00000bd0: 5700 5d04 0000 5800 4704 0000 5900 1f04  W.]...X.G...Y...
+00000be0: 0000 5a00 db03 0000 5b00 f203 0000 5c00  ..Z.....[.....\.
+00000bf0: 2501 0000 5d00 ca02 0000 5e00 1801 0000  %...].....^.....
+00000c00: 5f00 a802 0000 6000 f600 0000 6100 b702  _.....`.....a...
+00000c10: 0000 6200 0501 0000 6500 de01 0000 6900  ..b.....e.....i.
+00000c20: 7f03 0000 6b00 de01 0000 6c00 de01 0000  ....k.....l.....
+00000c30: 6d00 de01 0000 6e00 de01 0000 6f00 de01  m.....n.....o...
+00000c40: 0000 7000 de01 0000 7100 de01 0000 7200  ..p.....q.....r.
+00000c50: de01 0000 7300 ee02 0000 7400 de01 0000  ....s.....t.....
+00000c60: 7600 b805 0000 7900 a005 0000 7b00 be00  v.....y.....{...
+00000c70: 0000 7c00 8d02 0000 7f00 c100 0000 8000  ..|.............
+00000c80: ee02 0000 8100 e703 0000 8200 1b05 0000  ................
+00000c90: 8300 de01 0000 8700 3d02 0000 8800 a603  ........=.......
+00000ca0: 0000 8b00 fd03 0000 8c00 4401 0000 8d00  ..........D.....
+00000cb0: 8a01 0000 8e00 c700 0000 8f00 a005 0000  ................
+00000cc0: 9000 de01 0000 9100 7f03 0000 9200 1e02  ................
+00000cd0: 0000 9300 8b02 0000 9400 e703 0000 9500  ................
+00000ce0: e703 0000 9600 e703 0000 9700 e703 0000  ................
+00000cf0: 9800 e703 0000 9900 1e02 0000 9a00 ee02  ................
+00000d00: 0000 9b00 7f03 0000 9c00 de01 0000 9f00  ................
+00000d10: 2702 0000 a200 3402 0000 a300 e702 0000  '.....4.........
+00000d20: a400 bb03 0000 0000 0100 0000 0100 e301  ................
+00000d30: 0000 0200 cd03 0000 0000 1b05 0000 0000  ................
+00000d40: 1b05 0000 0000 1b05 0000 0200 ad03 0000  ................
+00000d50: 0300 8202 0000 0400 0100 0000 0500 9f02  ................
+00000d60: 6900 813e 9800 873e 7f00 8d3e 1003 933e  i..>...>...>...>
+00000d70: 0000 0000 0100 f728 0200 0000 0100 483f  .......(......H?
+00000d80: 0400 0000 2700 0400 9d01 2700 0500 c303  ....'.....'.....
+00000d90: 0301 0300 9b01 2301 0300 9b01 4301 0300  ......#.....C...
+00000da0: 9b01 6301 0300 9b01 a301 0300 9b01 c301  ..c.............
+00000db0: 0300 9b01 e301 0300 9b01 0000 0043 5324  .............CS$
+00000dc0: 3c3e 385f 5f6c 6f63 616c 7330 0043 5324  <>8__locals0.CS$
+00000dd0: 3c3e 385f 5f6c 6f63 616c 7331 006f 7074  <>8__locals1.opt
+00000de0: 696f 6e73 4469 7370 6c61 7955 7365 7232  ionsDisplayUser2
+00000df0: 0077 6174 6572 5475 7262 696e 6544 6f6f  .waterTurbineDoo
+00000e00: 7243 4300 7468 6f74 684c 6566 7444 6f6f  rCC.thothLeftDoo
+00000e10: 7243 4300 7468 6f74 6852 6967 6874 446f  rCC.thothRightDo
+00000e20: 6f72 4343 0054 686f 7468 4272 6964 6765  orCC.ThothBridge
+00000e30: 4c65 6674 446f 6f72 4944 0041 3257 6174  LeftDoorID.A2Wat
+00000e40: 6572 5475 7262 696e 654c 6566 7444 6f6f  erTurbineLeftDoo
+00000e50: 7249 4400 5468 6f74 6842 7269 6467 6552  rID.ThothBridgeR
+00000e60: 6967 6874 446f 6f72 4944 0064 6f6f 7249  ightDoorID.doorI
+00000e70: 4400 7376 366c 6f61 6400 6964 0066 6f75  D.sv6load.id.fou
+00000e80: 6e64 0063 6f6c 6c69 7369 6f6e 436f 6465  nd.collisionCode
+00000e90: 546f 4265 0073 686f 6f74 4d69 7373 696c  ToBe.shootMissil
+00000ea0: 6543 6f64 6500 6e65 7747 616d 6543 6f64  eCode.newGameCod
+00000eb0: 6500 6465 7074 6873 5069 7065 436f 6465  e.depthsPipeCode
+00000ec0: 0077 6174 6572 6661 6c6c 7350 6970 6543  .waterfallsPipeC
+00000ed0: 6f64 6500 6e65 7374 5069 7065 436f 6465  ode.nestPipeCode
+00000ee0: 0068 6964 656f 7574 5069 7065 436f 6465  .hideoutPipeCode
+00000ef0: 0063 6853 7465 7046 6972 6543 6f64 6500  .chStepFireCode.
+00000f00: 6372 6561 7465 436f 6465 0075 6e6c 6f63  createCode.unloc
+00000f10: 6b53 7475 6666 436f 6465 0064 7261 7747  kStuffCode.drawG
+00000f20: 7569 436f 6465 006c 6162 426c 6f63 6b43  uiCode.labBlockC
+00000f30: 6f64 6500 6368 5374 6570 436f 6e74 726f  ode.chStepContro
+00000f40: 6c43 6f64 6500 636f 6c6c 6973 696f 6e43  lCode.collisionC
+00000f50: 6f64 6500 6761 6d65 5365 6c4d 656e 7553  ode.gameSelMenuS
+00000f60: 7465 7043 6f64 6500 6c6f 6164 476c 6f62  tepCode.loadGlob
+00000f70: 616c 7343 6f64 6500 7361 7665 476c 6f62  alsCode.saveGlob
+00000f80: 616c 7343 6f64 6500 6368 6172 6163 7465  alsCode.characte
+00000f90: 7256 6172 7343 6f64 6500 636f 6465 0074  rVarsCode.code.t
+00000fa0: 6578 7475 7265 5061 6765 0061 3450 6167  exturePage.a4Pag
+00000fb0: 6532 496d 6167 6500 6134 5061 6765 496d  e2Image.a4PageIm
+00000fc0: 6167 6500 7465 6d70 5469 6c65 0073 7461  age.tempTile.sta
+00000fd0: 7274 4e65 7747 616d 6500 636f 6465 4e61  rtNewGame.codeNa
+00000fe0: 6d65 0069 6e74 6572 6e61 6c4e 616d 6500  me.internalName.
+00000ff0: 726f 6f6d 4e61 6d65 0070 6963 6b75 704e  roomName.pickupN
+00001000: 616d 6500 6e61 6d65 0077 6973 646f 6d53  ame.name.wisdomS
+00001010: 6570 746f 6767 4372 6561 7465 0063 7265  eptoggCreate.cre
+00001020: 6174 6500 7376 3653 6176 6500 6267 006f  ate.sv6Save.bg.o
+00001030: 5769 7364 6f6d 5365 7074 6f67 6700 6669  WisdomSeptogg.fi
+00001040: 6c65 5061 7468 0069 0064 6f6f 724c 6f63  lePath.i.doorLoc
+00001050: 6b00 6c61 6242 6c6f 636b 0070 6167 6549  k.labBlock.pageI
+00001060: 7465 6d00 6465 7074 6873 5069 7065 526f  tem.depthsPipeRo
+00001070: 6f6d 0077 6174 6572 6661 6c6c 7350 6970  om.waterfallsPip
+00001080: 6552 6f6f 6d00 6e65 7374 5069 7065 526f  eRoom.nestPipeRo
+00001090: 6f6d 0068 6964 656f 7574 5069 7065 526f  om.hideoutPipeRo
+000010a0: 6f6d 0067 6d52 6f6f 6d00 726f 6f6d 0064  om.gmRoom.room.d
+000010b0: 6f6f 7253 616d 7573 436f 6c6c 6973 696f  oorSamusCollisio
+000010c0: 6e00 636f 6c6c 6973 696f 6e00 7061 6765  n.collision.page
+000010d0: 4469 6d65 6e73 696f 6e00 7769 7364 6f6d  Dimension.wisdom
+000010e0: 5365 7074 6f67 6741 6374 696f 6e00 7661  SeptoggAction.va
+000010f0: 7244 6f6f 7241 6374 696f 6e00 6163 7469  rDoorAction.acti
+00001100: 6f6e 0061 3541 6374 6976 6174 6543 6f6e  on.a5ActivateCon
+00001110: 6469 7469 6f6e 0065 6d70 4261 7474 6572  dition.empBatter
+00001120: 7943 656c 6c43 6f6e 6469 7469 6f6e 0073  yCellCondition.s
+00001130: 6372 444e 4153 7061 776e 0067 6f00 7769  crDNASpawn.go.wi
+00001140: 7364 6f6d 5365 7074 6f67 6753 7465 7000  sdomSeptoggStep.
+00001150: 7375 6273 6372 6565 6e4d 656e 7553 7465  subscreenMenuSte
+00001160: 7000 7069 636b 7570 0073 7562 4469 7200  p.pickup.subDir.
+00001170: 6135 446f 6f72 0066 7300 7376 366c 6f61  a5Door.fs.sv6loa
+00001180: 6444 6574 6169 6c73 006d 7300 7365 6564  dDetails.ms.seed
+00001190: 4f62 6a65 6374 0073 6f6c 6964 4f62 6a65  Object.solidObje
+000011a0: 6374 0067 616d 654f 626a 6563 7400 7069  ct.gameObject.pi
+000011b0: 7065 4f62 6a65 6374 0067 6d4f 626a 6563  peObject.gmObjec
+000011c0: 7400 656e 656d 794f 626a 6563 7400 6574  t.enemyObject.et
+000011d0: 616e 6b53 6e69 7070 6574 0070 6970 6542  ankSnippet.pipeB
+000011e0: 4754 696c 6573 6574 0064 6570 7468 7345  GTileset.depthsE
+000011f0: 6e74 7261 6e63 6550 6970 6554 696c 6573  ntrancePipeTiles
+00001200: 6574 0077 6174 6572 6661 6c6c 7350 6970  et.waterfallsPip
+00001210: 6554 696c 6573 6574 0064 6570 7468 7345  eTileset.depthsE
+00001220: 7869 7450 6970 6554 696c 6573 6574 0068  xitPipeTileset.h
+00001230: 6964 656f 7574 5069 7065 5469 6c65 7365  ideoutPipeTilese
+00001240: 7400 646f 6f72 5469 6c65 7365 7400 7769  t.doorTileset.wi
+00001250: 7364 6f6d 5365 7074 6f67 6745 7665 6e74  sdomSeptoggEvent
+00001260: 0070 426f 6d62 4368 6172 6163 7465 7245  .pBombCharacterE
+00001270: 7665 6e74 0073 7570 6572 4d69 7373 696c  vent.superMissil
+00001280: 6543 6861 7261 6374 6572 4576 656e 7400  eCharacterEvent.
+00001290: 6d69 7373 696c 6543 6861 7261 6374 6572  missileCharacter
+000012a0: 4576 656e 7400 6554 616e 6b43 6861 7261  Event.eTankChara
+000012b0: 6374 6572 4576 656e 7400 7661 7244 6f6f  cterEvent.varDoo
+000012c0: 7245 7665 6e74 0069 7465 6d73 5377 6170  rEvent.itemsSwap
+000012d0: 5363 7269 7074 0063 6f64 6554 6578 7400  Script.codeText.
+000012e0: 6e65 7744 6f6f 7252 6570 6c61 6365 6d65  newDoorReplaceme
+000012f0: 6e74 5465 7874 0073 7562 7363 7265 656e  ntText.subscreen
+00001300: 4d69 7363 4461 7700 7373 4472 6177 0073  MiscDaw.ssDraw.s
+00001310: 7562 6372 6565 6e42 6f6f 7473 4472 6177  ubcreenBootsDraw
+00001320: 0073 7562 7363 7265 656e 5375 6974 4472  .subscreenSuitDr
+00001330: 6177 0064 7261 7745 6e64 496e 6465 7800  aw.drawEndIndex.
+00001340: 646f 6f72 4576 656e 7449 6e64 6578 0064  doorEventIndex.d
+00001350: 7261 7753 7461 7274 496e 6465 7800 6173  rawStartIndex.as
+00001360: 7365 6d62 6c79 0074 6578 7475 7265 456e  sembly.textureEn
+00001370: 7472 7900 7175 616e 7469 7479 0000 0000  try.quantity....
+00001380: 0000 0000 0fd0 2988 b811 1342 878b 770e  ......)....B..w.
+00001390: 8597 ac16 f862 513f c607 d311 9053 00c0  .....bQ?.....S..
+000013a0: 4fa3 02a1 bc74 2e93 a9db 7844 8d46 0f32  O....t....xD.F.2
+000013b0: a7ba b3d3 05ec feb5 d08c 834a 96da 4662  ...........J..Fb
+000013c0: 84bb 4bd8 0847 4d7e 6e09 5c4c aeda cb10  ..K..GM~n.\L....
+000013d0: ba6a 740d 0004 686f 6d65 0672 756e 6e65  .jt...home.runne
+000013e0: 7204 776f 726b 0459 414d 5308 5941 4d53  r.work.YAMS.YAMS
+000013f0: 2d4c 4942 0a50 726f 6772 616d 2e63 7309  -LIB.Program.cs.
+00001400: 2f00 0106 0d12 1217 2020 bea2 0787 9530  /.......  .....0
+00001410: b05f a00d a072 7967 b006 0b11 2132 ff92  ._...ryg....!2..
+00001420: 2c2a c7e3 0360 e991 5b76 0d53 6565 644f  ,*...`..[v.SeedO
+00001430: 626a 6563 742e 6373 092f 0001 060d 1212  bject.cs./......
+00001440: 1756 205b d519 ac1a e6af b0e4 c85d f573  .V [.........].s
+00001450: 95bc 909e e39b 57fc 8ad8 262d c891 a2ae  ......W...&-....
+00001460: 3dae 3903 6f62 6a07 5265 6c65 6173 6506  =.9.obj.Release.
+00001470: 6e65 7436 2e30 1a59 414d 532d 4c49 422e  net6.0.YAMS-LIB.
+00001480: 476c 6f62 616c 5573 696e 6773 2e67 2e63  GlobalUsings.g.c
+00001490: 7310 2f00 0106 0d12 1217 808f 8093 809b  s./.............
+000014a0: 80a2 205d d6d5 28fd d6c4 4688 4302 02cd  .. ]..(...F.C...
+000014b0: 32e6 b714 4a8a ec9d fc9f 674a 11e9 0331  2...J.....gJ...1
+000014c0: 1930 c42e 2e4e 4554 436f 7265 4170 702c  .0...NETCoreApp,
+000014d0: 5665 7273 696f 6e3d 7636 2e30 2e41 7373  Version=v6.0.Ass
+000014e0: 656d 626c 7941 7474 7269 6275 7465 732e  emblyAttributes.
+000014f0: 6373 102f 0001 060d 1212 1780 8f80 9380  cs./............
+00001500: 9b80 ef20 7897 e595 3cb5 cd51 3150 9b35  ... x...<..Q1P.5
+00001510: 0421 8634 c24b 9ce7 a68b 984f fb5a 1668  .!.4.K.....O.Z.h
+00001520: 6eb5 af5c 1859 414d 532d 4c49 422e 4173  n..\.YAMS-LIB.As
+00001530: 7365 6d62 6c79 496e 666f 2e63 7310 2f00  semblyInfo.cs./.
+00001540: 0106 0d12 1217 808f 8093 809b 8150 20b5  .............P .
+00001550: 256f a358 2c99 4f38 42d2 427e 9434 783e  %o.X,.O8B.B~.4x>
+00001560: a700 faf7 e0d8 8640 7d7f 7faa c614 0101  .......@}.......
+00001570: 0282 2476 6572 7369 6f6e 0032 0063 6f6d  ..$version.2.com
+00001580: 7069 6c65 722d 7665 7273 696f 6e00 342e  piler-version.4.
+00001590: 362e 302d 332e 3233 3235 392e 382b 6333  6.0-3.23259.8+c3
+000015a0: 6363 3164 3063 6565 6162 3161 3635 6461  cc1d0ceeab1a65da
+000015b0: 3032 3137 6534 3033 3835 3161 3165 3861  0217e403851a1e8a
+000015c0: 3330 3038 3661 006c 616e 6775 6167 6500  30086a.language.
+000015d0: 4323 0073 6f75 7263 652d 6669 6c65 2d63  C#.source-file-c
+000015e0: 6f75 6e74 0035 006f 7574 7075 742d 6b69  ount.5.output-ki
+000015f0: 6e64 0044 796e 616d 6963 616c 6c79 4c69  nd.DynamicallyLi
+00001600: 6e6b 6564 4c69 6272 6172 7900 6f70 7469  nkedLibrary.opti
+00001610: 6d69 7a61 7469 6f6e 0072 656c 6561 7365  mization.release
+00001620: 0070 6c61 7466 6f72 6d00 416e 7943 7075  .platform.AnyCpu
+00001630: 0072 756e 7469 6d65 2d76 6572 7369 6f6e  .runtime-version
+00001640: 0037 2e30 2e39 2b38 6539 6131 3762 3232  .7.0.9+8e9a17b22
+00001650: 3136 6635 3161 3537 3838 6638 6231 6334  16f51a5788f8b1c4
+00001660: 3637 6134 6366 3362 3736 3965 3764 3700  67a4cf3b769e7d7.
+00001670: 6c61 6e67 7561 6765 2d76 6572 7369 6f6e  language-version
+00001680: 0070 7265 7669 6577 006e 756c 6c61 626c  .preview.nullabl
+00001690: 6500 456e 6162 6c65 0064 6566 696e 6500  e.Enable.define.
+000016a0: 5452 4143 452c 5245 4c45 4153 452c 4e45  TRACE,RELEASE,NE
+000016b0: 542c 4e45 5436 5f30 2c4e 4554 434f 5245  T,NET6_0,NETCORE
+000016c0: 4150 502c 4e45 5435 5f30 5f4f 525f 4752  APP,NET5_0_OR_GR
+000016d0: 4541 5445 522c 4e45 5436 5f30 5f4f 525f  EATER,NET6_0_OR_
+000016e0: 4752 4541 5445 522c 4e45 5443 4f52 4541  GREATER,NETCOREA
+000016f0: 5050 315f 305f 4f52 5f47 5245 4154 4552  PP1_0_OR_GREATER
+00001700: 2c4e 4554 434f 5245 4150 5031 5f31 5f4f  ,NETCOREAPP1_1_O
+00001710: 525f 4752 4541 5445 522c 4e45 5443 4f52  R_GREATER,NETCOR
+00001720: 4541 5050 325f 305f 4f52 5f47 5245 4154  EAPP2_0_OR_GREAT
+00001730: 4552 2c4e 4554 434f 5245 4150 5032 5f31  ER,NETCOREAPP2_1
+00001740: 5f4f 525f 4752 4541 5445 522c 4e45 5443  _OR_GREATER,NETC
+00001750: 4f52 4541 5050 325f 325f 4f52 5f47 5245  OREAPP2_2_OR_GRE
+00001760: 4154 4552 2c4e 4554 434f 5245 4150 5033  ATER,NETCOREAPP3
+00001770: 5f30 5f4f 525f 4752 4541 5445 522c 4e45  _0_OR_GREATER,NE
+00001780: 5443 4f52 4541 5050 335f 315f 4f52 5f47  TCOREAPP3_1_OR_G
+00001790: 5245 4154 4552 00a3 ba49 4353 6861 7270  REATER...ICSharp
+000017a0: 436f 6465 2e53 6861 7270 5a69 704c 6962  Code.SharpZipLib
+000017b0: 2e64 6c6c 0000 016c 9904 9800 8003 0087  .dll...l........
+000017c0: d282 16a4 95d1 4abd 3f1f c402 13b4 ed4d  ......J.?......M
+000017d0: 6163 726f 7373 2e4a 736f 6e2e 4578 7465  across.Json.Exte
+000017e0: 6e73 696f 6e73 2e64 6c6c 0000 0155 c478  nsions.dll...U.x
+000017f0: ba00 0001 00b2 09ba d9ca d5dc 4e93 a42a  ............N..*
+00001800: 22b1 17ec 344d 6963 726f 736f 6674 2e43  "...4Microsoft.C
+00001810: 5368 6172 702e 646c 6c00 0001 0749 52d7  Sharp.dll....IR.
+00001820: 0080 0000 17e1 8671 93a1 9e42 a11d 4bf1  .......q...B..K.
+00001830: cb94 691c 4d69 6372 6f73 6f66 742e 5669  ..i.Microsoft.Vi
+00001840: 7375 616c 4261 7369 632e 436f 7265 2e64  sualBasic.Core.d
+00001850: 6c6c 0000 01fd f562 8500 2001 0008 ae07  ll.....b.. .....
+00001860: b107 183f 4282 f29e 3548 56b3 9f4d 6963  ...?B...5HV..Mic
+00001870: 726f 736f 6674 2e56 6973 7561 6c42 6173  rosoft.VisualBas
+00001880: 6963 2e64 6c6c 0000 019a 0054 d700 8000  ic.dll.....T....
+00001890: 00a8 a4e9 c9a3 ffc3 4aae 82d9 bfb4 281d  ........J.....(.
+000018a0: 754d 6963 726f 736f 6674 2e57 696e 3332  uMicrosoft.Win32
+000018b0: 2e50 7269 6d69 7469 7665 732e 646c 6c00  .Primitives.dll.
+000018c0: 0001 66d5 2dfc 0080 0000 e73e d1c6 4da4  ..f.-......>..M.
+000018d0: f344 8f16 2586 5dd6 7d54 4d69 6372 6f73  .D..%.].}TMicros
+000018e0: 6f66 742e 5769 6e33 322e 5265 6769 7374  oft.Win32.Regist
+000018f0: 7279 2e64 6c6c 0000 0161 b328 9f00 a000  ry.dll...a.(....
+00001900: 007a 4531 5af2 af1d 489d 9445 67ef 8b8b  .zE1Z...H..Eg...
+00001910: 1e6d 7363 6f72 6c69 622e 646c 6c00 0001  .mscorlib.dll...
+00001920: cdd0 f4f6 0020 0100 fcaf 6eca 8e72 524a  ..... ....n..rRJ
+00001930: bf2b 9464 ddc5 4cef 6e65 7473 7461 6e64  .+.d..L.netstand
+00001940: 6172 642e 646c 6c00 0001 2f8c b0fe 00c0  ard.dll.../.....
+00001950: 0100 faf8 f92e a718 f040 8eb8 58ce cd30  .........@..X..0
+00001960: 4898 5072 6f70 6572 7479 4368 616e 6765  H.PropertyChange
+00001970: 642e 646c 6c00 0001 8b5a 978a 0080 0000  d.dll....Z......
+00001980: 3174 ff35 d3a6 344c 90ea 21b0 de57 7fe0  1t.5..4L..!..W..
+00001990: 5369 784c 6162 6f72 732e 496d 6167 6553  SixLabors.ImageS
+000019a0: 6861 7270 2e64 6c6c 0000 016c 8a3e dd00  harp.dll...l.>..
+000019b0: 601f 007f 776a e7b5 74d7 4aaa 9d41 db13  `...wj..t.J..A..
+000019c0: 6c03 4353 7973 7465 6d2e 4170 7043 6f6e  l.CSystem.AppCon
+000019d0: 7465 7874 2e64 6c6c 0000 0170 94a2 e200  text.dll...p....
+000019e0: 8000 0025 2e6c 6fa8 98f6 4d8c 7a65 cb60  ...%.lo...M.ze.`
+000019f0: d06b d753 7973 7465 6d2e 4275 6666 6572  .k.System.Buffer
+00001a00: 732e 646c 6c00 0001 4862 a3da 0080 0000  s.dll...Hb......
+00001a10: b7aa 5ee8 37bf c340 a7a9 80fb 3588 0655  ..^.7..@....5..U
+00001a20: 5379 7374 656d 2e43 6f6c 6c65 6374 696f  System.Collectio
+00001a30: 6e73 2e43 6f6e 6375 7272 656e 742e 646c  ns.Concurrent.dl
+00001a40: 6c00 0001 801f 71e1 00a0 0000 9df2 9458  l.....q........X
+00001a50: 7ad0 f54d 89ee e2ea 7478 52a8 5379 7374  z..M....txR.Syst
+00001a60: 656d 2e43 6f6c 6c65 6374 696f 6e73 2e64  em.Collections.d
+00001a70: 6c6c 0000 0189 c9a8 ca00 0001 0048 1fec  ll...........H..
+00001a80: 5634 526b 4082 f7a3 b914 aaec c953 7973  V4Rk@........Sys
+00001a90: 7465 6d2e 436f 6c6c 6563 7469 6f6e 732e  tem.Collections.
+00001aa0: 496d 6d75 7461 626c 652e 646c 6c00 0001  Immutable.dll...
+00001ab0: 7a6e d5f0 0040 0100 3840 68b9 d79c 9746  zn...@..8@h....F
+00001ac0: 8218 e630 2acc ca10 5379 7374 656d 2e43  ...0*...System.C
+00001ad0: 6f6c 6c65 6374 696f 6e73 2e4e 6f6e 4765  ollections.NonGe
+00001ae0: 6e65 7269 632e 646c 6c00 0001 d8e6 4cac  neric.dll.....L.
+00001af0: 00a0 0000 d21c c278 ed7e a648 858e 03c2  .......x.~.H....
+00001b00: f6be df33 5379 7374 656d 2e43 6f6c 6c65  ...3System.Colle
+00001b10: 6374 696f 6e73 2e53 7065 6369 616c 697a  ctions.Specializ
+00001b20: 6564 2e64 6c6c 0000 019c fa3c d300 a000  ed.dll.....<....
+00001b30: 0023 9f8f 8a45 230e 44b8 cc5f c180 b6bf  .#...E#.D.._....
+00001b40: c653 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
+00001b50: 744d 6f64 656c 2e41 6e6e 6f74 6174 696f  tModel.Annotatio
+00001b60: 6e73 2e64 6c6c 0000 01be 614b ec00 c000  ns.dll....aK....
+00001b70: 0055 a438 af72 c4c4 4e90 86bc 1224 07f2  .U.8.r..N....$..
+00001b80: eb53 7973 7465 6d2e 436f 6d70 6f6e 656e  .System.Componen
+00001b90: 744d 6f64 656c 2e44 6174 6141 6e6e 6f74  tModel.DataAnnot
+00001ba0: 6174 696f 6e73 2e64 6c6c 0000 0184 683a  ations.dll....h:
+00001bb0: fe00 8000 0005 d0f9 02c1 73b8 4b89 44c0  ..........s.K.D.
+00001bc0: 7c3c 00f1 ab53 7973 7465 6d2e 436f 6d70  |<...System.Comp
+00001bd0: 6f6e 656e 744d 6f64 656c 2e64 6c6c 0000  onentModel.dll..
+00001be0: 014e 2422 8700 8000 00e9 ad6e e8bd 5995  .N$".......n..Y.
+00001bf0: 4ea9 e15c 5c7c a0bd 0353 7973 7465 6d2e  N..\\|...System.
+00001c00: 436f 6d70 6f6e 656e 744d 6f64 656c 2e45  ComponentModel.E
+00001c10: 7665 6e74 4261 7365 6441 7379 6e63 2e64  ventBasedAsync.d
+00001c20: 6c6c 0000 01e2 a443 9700 8000 00fd e5d9  ll.....C........
+00001c30: 3533 23ce 4081 038b a246 c95b d253 7973  53#.@....F.[.Sys
+00001c40: 7465 6d2e 436f 6d70 6f6e 656e 744d 6f64  tem.ComponentMod
+00001c50: 656c 2e50 7269 6d69 7469 7665 732e 646c  el.Primitives.dl
+00001c60: 6c00 0001 4296 8faf 00a0 0000 f190 fdcb  l...B...........
+00001c70: 2f09 1540 b5ed 6b66 648c ea66 5379 7374  /..@..kfd..fSyst
+00001c80: 656d 2e43 6f6d 706f 6e65 6e74 4d6f 6465  em.ComponentMode
+00001c90: 6c2e 5479 7065 436f 6e76 6572 7465 722e  l.TypeConverter.
+00001ca0: 646c 6c00 0001 78b1 0aa1 00c0 0100 f5c9  dll...x.........
+00001cb0: 711b 41c1 2b4f a387 838a 4ca9 04c5 5379  q.A.+O....L...Sy
+00001cc0: 7374 656d 2e43 6f6e 6669 6775 7261 7469  stem.Configurati
+00001cd0: 6f6e 2e64 6c6c 0000 0142 606d 9700 8000  on.dll...B`m....
+00001ce0: 0047 fc59 3fb8 f598 4bb7 c800 e5d4 fe5d  .G.Y?...K......]
+00001cf0: 2853 7973 7465 6d2e 436f 6e73 6f6c 652e  (System.Console.
+00001d00: 646c 6c00 0001 c631 eba4 00a0 0000 01fb  dll....1........
+00001d10: ca4e 49e4 fd47 8ba7 a6a6 0d03 5401 5379  .NI..G......T.Sy
+00001d20: 7374 656d 2e43 6f72 652e 646c 6c00 0001  stem.Core.dll...
+00001d30: 0f44 62a6 00a0 0000 1145 5732 5df8 7844  .Db......EW2].xD
+00001d40: 88f9 180f b7c6 af61 5379 7374 656d 2e44  .......aSystem.D
+00001d50: 6174 612e 436f 6d6d 6f6e 2e64 6c6c 0000  ata.Common.dll..
+00001d60: 0171 db86 f800 8002 0070 101f 3c3b 13f1  .q.......p..<;..
+00001d70: 42a8 564f 2861 4a19 ac53 7973 7465 6d2e  B.VO(aJ..System.
+00001d80: 4461 7461 2e44 6174 6153 6574 4578 7465  Data.DataSetExte
+00001d90: 6e73 696f 6e73 2e64 6c6c 0000 01d9 8f9f  nsions.dll......
+00001da0: bf00 8000 00a0 76e7 b0b2 20f3 4c91 083a  ......v... .L..:
+00001db0: bbe6 ac79 ef53 7973 7465 6d2e 4461 7461  ...y.System.Data
+00001dc0: 2e64 6c6c 0000 010c 4483 9e00 a000 002d  .dll....D......-
+00001dd0: 7ff2 3276 1ae6 44ae 9eb3 76fe e7e2 dc53  ..2v..D...v....S
+00001de0: 7973 7465 6d2e 4469 6167 6e6f 7374 6963  ystem.Diagnostic
+00001df0: 732e 436f 6e74 7261 6374 732e 646c 6c00  s.Contracts.dll.
+00001e00: 0001 b13e 63fc 0080 0000 276b 11c6 c4f0  ...>c.....'k....
+00001e10: 2544 b417 4af0 15a4 eb81 5379 7374 656d  %D..J.....System
+00001e20: 2e44 6961 676e 6f73 7469 6373 2e44 6562  .Diagnostics.Deb
+00001e30: 7567 2e64 6c6c 0000 01ed 49cb f400 8000  ug.dll....I.....
+00001e40: 004b 9eb6 499b 2776 4cae b41c 2924 2a3e  .K..I.'vL...)$*>
+00001e50: e553 7973 7465 6d2e 4469 6167 6e6f 7374  .System.Diagnost
+00001e60: 6963 732e 4469 6167 6e6f 7374 6963 536f  ics.DiagnosticSo
+00001e70: 7572 6365 2e64 6c6c 0000 018c f22c f800  urce.dll.....,..
+00001e80: c000 0031 3552 2d2c 67e3 4487 e849 98de  ...15R-,g.D..I..
+00001e90: 1554 b053 7973 7465 6d2e 4469 6167 6e6f  .T.System.Diagno
+00001ea0: 7374 6963 732e 4669 6c65 5665 7273 696f  stics.FileVersio
+00001eb0: 6e49 6e66 6f2e 646c 6c00 0001 5fe3 fcf2  nInfo.dll..._...
+00001ec0: 0080 0000 4d91 ef25 cb82 d040 b004 9607  ....M..%...@....
+00001ed0: 0811 7076 5379 7374 656d 2e44 6961 676e  ..pvSystem.Diagn
+00001ee0: 6f73 7469 6373 2e50 726f 6365 7373 2e64  ostics.Process.d
+00001ef0: 6c6c 0000 0128 cad2 b200 c000 007d 9733  ll...(.......}.3
+00001f00: 70f0 bac2 45a1 fa60 16b0 497e 2353 7973  p...E..`..I~#Sys
+00001f10: 7465 6d2e 4469 6167 6e6f 7374 6963 732e  tem.Diagnostics.
+00001f20: 5374 6163 6b54 7261 6365 2e64 6c6c 0000  StackTrace.dll..
+00001f30: 0135 fff9 b200 a000 00ad 5f8a 71cb 64c7  .5........_.q.d.
+00001f40: 459c 731d 01da b22d 7953 7973 7465 6d2e  E.s....-ySystem.
+00001f50: 4469 6167 6e6f 7374 6963 732e 5465 7874  Diagnostics.Text
+00001f60: 5772 6974 6572 5472 6163 654c 6973 7465  WriterTraceListe
+00001f70: 6e65 722e 646c 6c00 0001 5a50 95c4 0080  ner.dll...ZP....
+00001f80: 0000 88d5 8bd4 95e2 d24b 94d5 f302 b798  .........K......
+00001f90: 1df6 5379 7374 656d 2e44 6961 676e 6f73  ..System.Diagnos
+00001fa0: 7469 6373 2e54 6f6f 6c73 2e64 6c6c 0000  tics.Tools.dll..
+00001fb0: 01a0 613c fe00 8000 00cc 118d eff1 3cf0  ..a<..........<.
+00001fc0: 42a5 309f 6b00 7903 fb53 7973 7465 6d2e  B.0.k.y..System.
+00001fd0: 4469 6167 6e6f 7374 6963 732e 5472 6163  Diagnostics.Trac
+00001fe0: 6553 6f75 7263 652e 646c 6c00 0001 66d5  eSource.dll...f.
+00001ff0: d884 00a0 0000 5722 142a d78a e144 b398  ......W".*...D..
+00002000: 42db 6ad1 b885 5379 7374 656d 2e44 6961  B.j...System.Dia
+00002010: 676e 6f73 7469 6373 2e54 7261 6369 6e67  gnostics.Tracing
+00002020: 2e64 6c6c 0000 016e 9980 de00 a000 00e8  .dll...n........
+00002030: 77f8 d4fb 6360 43aa 5057 a2c1 5c08 9553  w...c`C.PW..\..S
+00002040: 7973 7465 6d2e 646c 6c00 0001 1b34 e8f0  ystem.dll....4..
+00002050: 0000 0100 042d f79f 0ace ff43 9292 a2bb  .....-.....C....
+00002060: 74fc e9ac 5379 7374 656d 2e44 7261 7769  t...System.Drawi
+00002070: 6e67 2e43 6f6d 6d6f 6e2e 646c 6c00 0001  ng.Common.dll...
+00002080: 218d 42d5 0020 0200 0843 fec0 6a78 bb46  !.B.. ...C..jx.F
+00002090: 9f62 dc8a c5b5 5abc 5379 7374 656d 2e44  .b....Z.System.D
+000020a0: 7261 7769 6e67 2e64 6c6c 0000 012a c527  rawing.dll...*.'
+000020b0: 8600 8000 0053 29d0 50ec d5fd 41b7 5dc0  .....S).P...A.].
+000020c0: 3bb4 fec2 aa53 7973 7465 6d2e 4472 6177  ;....System.Draw
+000020d0: 696e 672e 5072 696d 6974 6976 6573 2e64  ing.Primitives.d
+000020e0: 6c6c 0000 0130 b401 ca00 c000 008e 8f7f  ll...0..........
+000020f0: 0f67 cfeb 438c aca0 408d d5b7 8853 7973  .g..C...@....Sys
+00002100: 7465 6d2e 4479 6e61 6d69 632e 5275 6e74  tem.Dynamic.Runt
+00002110: 696d 652e 646c 6c00 0001 7af8 ba93 0080  ime.dll...z.....
+00002120: 0000 00d2 3986 f2b3 5047 98a0 8d09 122b  ....9...PG.....+
+00002130: 601d 5379 7374 656d 2e46 6f72 6d61 7473  `.System.Formats
+00002140: 2e41 736e 312e 646c 6c00 0001 d5eb 2df8  .Asn1.dll.....-.
+00002150: 00a0 0000 6809 fe95 7ccf be4c aa8e 7879  ....h...|..L..xy
+00002160: c0e9 dd04 5379 7374 656d 2e47 6c6f 6261  ....System.Globa
+00002170: 6c69 7a61 7469 6f6e 2e43 616c 656e 6461  lization.Calenda
+00002180: 7273 2e64 6c6c 0000 0119 2fbb 9a00 8000  rs.dll..../.....
+00002190: 008e 0099 e074 bd7f 4caa 3458 690f b25a  .....t..L.4Xi..Z
+000021a0: 7b53 7973 7465 6d2e 476c 6f62 616c 697a  {System.Globaliz
+000021b0: 6174 696f 6e2e 646c 6c00 0001 d1af f6a4  ation.dll.......
+000021c0: 0080 0000 4f43 3c41 90af 6f45 9f16 2060  ....OC<A..oE.. `
+000021d0: 991e 4966 5379 7374 656d 2e47 6c6f 6261  ..IfSystem.Globa
+000021e0: 6c69 7a61 7469 6f6e 2e45 7874 656e 7369  lization.Extensi
+000021f0: 6f6e 732e 646c 6c00 0001 f33d 8be4 0080  ons.dll....=....
+00002200: 0000 198b dc84 e703 df49 959b ece8 5b61  .........I....[a
+00002210: 08d3 5379 7374 656d 2e49 4f2e 436f 6d70  ..System.IO.Comp
+00002220: 7265 7373 696f 6e2e 4272 6f74 6c69 2e64  ression.Brotli.d
+00002230: 6c6c 0000 01bc 6117 e100 8000 003c 5edd  ll....a......<^.
+00002240: 0f96 2796 41bc 60e7 167c 93ec ff53 7973  ..'.A.`..|...Sys
+00002250: 7465 6d2e 494f 2e43 6f6d 7072 6573 7369  tem.IO.Compressi
+00002260: 6f6e 2e64 6c6c 0000 01ea 16ee b900 a000  on.dll..........
+00002270: 00b4 df97 ee7e bd80 459a 36f1 fbf4 4867  .....~..E.6...Hg
+00002280: 3853 7973 7465 6d2e 494f 2e43 6f6d 7072  8System.IO.Compr
+00002290: 6573 7369 6f6e 2e46 696c 6553 7973 7465  ession.FileSyste
+000022a0: 6d2e 646c 6c00 0001 6b99 aed3 0080 0000  m.dll...k.......
+000022b0: 523d 5710 75f0 1a48 ada5 d1b7 890b 0c6c  R=W.u..H.......l
+000022c0: 5379 7374 656d 2e49 4f2e 436f 6d70 7265  System.IO.Compre
+000022d0: 7373 696f 6e2e 5a69 7046 696c 652e 646c  ssion.ZipFile.dl
+000022e0: 6c00 0001 5853 7cc3 0080 0000 580d 2f60  l...XS|.....X./`
+000022f0: b7c2 004e a5bf 0576 acb1 67d9 5379 7374  ...N...v..g.Syst
+00002300: 656d 2e49 4f2e 646c 6c00 0001 1ced 88ed  em.IO.dll.......
+00002310: 0080 0000 2b3c c477 14f7 844c bba2 c24f  ....+<.w...L...O
+00002320: 55c2 8603 5379 7374 656d 2e49 4f2e 4669  U...System.IO.Fi
+00002330: 6c65 5379 7374 656d 2e41 6363 6573 7343  leSystem.AccessC
+00002340: 6f6e 7472 6f6c 2e64 6c6c 0000 01a5 3b8d  ontrol.dll....;.
+00002350: 9000 a000 007a eb3c 18a8 34fc 4c9a 38c0  .....z.<..4.L.8.
+00002360: 0ddf dedc 8853 7973 7465 6d2e 494f 2e46  .....System.IO.F
+00002370: 696c 6553 7973 7465 6d2e 646c 6c00 0001  ileSystem.dll...
+00002380: f9c7 0dbf 0080 0000 eca4 c059 9fbc 744e  ...........Y..tN
+00002390: a4af 37c2 dca4 b1f9 5379 7374 656d 2e49  ..7.....System.I
+000023a0: 4f2e 4669 6c65 5379 7374 656d 2e44 7269  O.FileSystem.Dri
+000023b0: 7665 496e 666f 2e64 6c6c 0000 0175 7d28  veInfo.dll...u}(
+000023c0: cf00 8000 006e a90f b3e5 511d 47b0 7485  .....n....Q.G.t.
+000023d0: 905f 7688 0553 7973 7465 6d2e 494f 2e46  ._v..System.IO.F
+000023e0: 696c 6553 7973 7465 6d2e 5072 696d 6974  ileSystem.Primit
+000023f0: 6976 6573 2e64 6c6c 0000 01b3 710c 9800  ives.dll....q...
+00002400: 8000 0050 7c76 ce46 08de 4499 13d6 6755  ...P|v.F..D...gU
+00002410: 6ff3 ed53 7973 7465 6d2e 494f 2e46 696c  o..System.IO.Fil
+00002420: 6553 7973 7465 6d2e 5761 7463 6865 722e  eSystem.Watcher.
+00002430: 646c 6c00 0001 eeb6 f7b2 00a0 0000 d4b5  dll.............
+00002440: 5f3a 5fd9 3b41 8dc2 cac6 4bde 7572 5379  _:_.;A....K.urSy
+00002450: 7374 656d 2e49 4f2e 4973 6f6c 6174 6564  stem.IO.Isolated
+00002460: 5374 6f72 6167 652e 646c 6c00 0001 a38e  Storage.dll.....
+00002470: dec4 00a0 0000 3710 05cc 327d f64d b4ce  ......7...2}.M..
+00002480: 8a5c 6c81 614e 5379 7374 656d 2e49 4f2e  .\l.aNSystem.IO.
+00002490: 4d65 6d6f 7279 4d61 7070 6564 4669 6c65  MemoryMappedFile
+000024a0: 732e 646c 6c00 0001 47f5 1ff4 0080 0000  s.dll...G.......
+000024b0: 9151 f98c 5e36 494b 90f8 515d 8b59 68cf  .Q..^6IK..Q].Yh.
+000024c0: 5379 7374 656d 2e49 4f2e 5069 7065 732e  System.IO.Pipes.
+000024d0: 4163 6365 7373 436f 6e74 726f 6c2e 646c  AccessControl.dl
+000024e0: 6c00 0001 7f6c 5bfc 0080 0000 3bd5 5395  l....l[.....;.S.
+000024f0: 4e3d 4b4d 9687 50e1 5508 b91f 5379 7374  N=KM..P.U...Syst
+00002500: 656d 2e49 4f2e 5069 7065 732e 646c 6c00  em.IO.Pipes.dll.
+00002510: 0001 26a5 fdc3 00a0 0000 d904 bc24 8b94  ..&..........$..
+00002520: 9a47 9743 a06e d131 4978 5379 7374 656d  .G.C.n.1IxSystem
+00002530: 2e49 4f2e 556e 6d61 6e61 6765 644d 656d  .IO.UnmanagedMem
+00002540: 6f72 7953 7472 6561 6d2e 646c 6c00 0001  oryStream.dll...
+00002550: d746 0fa0 0080 0000 d3a0 8040 199b 5441  .F.........@..TA
+00002560: b8d9 284f 57b3 9292 5379 7374 656d 2e4c  ..(OW...System.L
+00002570: 696e 712e 646c 6c00 0001 d06e d586 00c0  inq.dll....n....
+00002580: 0000 697d 34b4 dfec 2b40 bd36 4017 1269  ..i}4...+@.6@..i
+00002590: d6a6 5379 7374 656d 2e4c 696e 712e 4578  ..System.Linq.Ex
+000025a0: 7072 6573 7369 6f6e 732e 646c 6c00 0001  pressions.dll...
+000025b0: 85c6 9691 0040 0100 1ac9 5fc9 1258 fc47  .....@...._..X.G
+000025c0: aa66 0d42 9ed0 c519 5379 7374 656d 2e4c  .f.B....System.L
+000025d0: 696e 712e 5061 7261 6c6c 656c 2e64 6c6c  inq.Parallel.dll
+000025e0: 0000 019a e108 c500 c000 00f0 26d0 c04a  ............&..J
+000025f0: 43cf 4286 80d5 7630 02e0 4e53 7973 7465  C.B...v0..NSyste
+00002600: 6d2e 4c69 6e71 2e51 7565 7279 6162 6c65  m.Linq.Queryable
+00002610: 2e64 6c6c 0000 012f 3dc9 8700 c000 00b4  .dll.../=.......
+00002620: 2fac f0a4 719c 4596 cef1 c318 bcdc e853  /...q.E........S
+00002630: 7973 7465 6d2e 4d65 6d6f 7279 2e64 6c6c  ystem.Memory.dll
+00002640: 0000 01d1 f194 9700 e000 0039 ecd5 1a26  ...........9...&
+00002650: 3372 43a1 3b0a 2cd8 c030 3853 7973 7465  3rC.;.,..08Syste
+00002660: 6d2e 4e65 742e 646c 6c00 0001 d616 97d6  m.Net.dll.......
+00002670: 0080 0000 5be1 7e6f d1ef d447 bb98 0601  ....[.~o...G....
+00002680: 2b17 a015 5379 7374 656d 2e4e 6574 2e48  +...System.Net.H
+00002690: 7474 702e 646c 6c00 0001 9234 82c2 0020  ttp.dll....4... 
+000026a0: 0100 4285 9141 8cd2 c44a 9267 5fb6 c70d  ..B..A...J.g_...
+000026b0: fe03 5379 7374 656d 2e4e 6574 2e48 7474  ..System.Net.Htt
+000026c0: 702e 4a73 6f6e 2e64 6c6c 0000 01d6 70c7  p.Json.dll....p.
+000026d0: eb00 8000 00c5 125f 9f70 f8f9 4491 411f  ......._.p..D.A.
+000026e0: 3d51 8729 2053 7973 7465 6d2e 4e65 742e  =Q.) System.Net.
+000026f0: 4874 7470 4c69 7374 656e 6572 2e64 6c6c  HttpListener.dll
+00002700: 0000 0131 7ce3 f600 a000 00e5 f981 6441  ...1|.........dA
+00002710: 2a43 4eb3 e76c 51b6 41a4 2353 7973 7465  *CN..lQ.A.#Syste
+00002720: 6d2e 4e65 742e 4d61 696c 2e64 6c6c 0000  m.Net.Mail.dll..
+00002730: 012f 7bf6 d600 c000 00ec ef60 8c04 4e6a  ./{........`..Nj
+00002740: 499b d4ff 1379 5c16 2553 7973 7465 6d2e  I....y\.%System.
+00002750: 4e65 742e 4e61 6d65 5265 736f 6c75 7469  Net.NameResoluti
+00002760: 6f6e 2e64 6c6c 0000 017a 3c48 e300 8000  on.dll...z<H....
+00002770: 0089 4311 e3dc 4efa 4681 2104 d992 6096  ..C...N.F.!...`.
+00002780: b953 7973 7465 6d2e 4e65 742e 4e65 7477  .System.Net.Netw
+00002790: 6f72 6b49 6e66 6f72 6d61 7469 6f6e 2e64  orkInformation.d
+000027a0: 6c6c 0000 01b1 ee6a 8600 c000 0006 798a  ll.....j......y.
+000027b0: 0663 7c93 4780 d5ac 2183 564d 9e53 7973  .c|.G...!.VM.Sys
+000027c0: 7465 6d2e 4e65 742e 5069 6e67 2e64 6c6c  tem.Net.Ping.dll
+000027d0: 0000 0126 c08c eb00 8000 00e1 52c0 3460  ...&........R.4`
+000027e0: a08b 46ac 6865 8747 2a97 0b53 7973 7465  ..F.he.G*..Syste
+000027f0: 6d2e 4e65 742e 5072 696d 6974 6976 6573  m.Net.Primitives
+00002800: 2e64 6c6c 0000 0112 d83d 8800 c000 0084  .dll.....=......
+00002810: 7bc3 b094 397b 4da0 2fc9 34b4 6560 b853  {...9{M./.4.e`.S
+00002820: 7973 7465 6d2e 4e65 742e 5265 7175 6573  ystem.Net.Reques
+00002830: 7473 2e64 6c6c 0000 01a2 8b03 cf00 e000  ts.dll..........
+00002840: 0081 1a5b 1c42 02c0 40b0 a164 f25d 024e  ...[.B..@..d.].N
+00002850: 4153 7973 7465 6d2e 4e65 742e 5365 6375  ASystem.Net.Secu
+00002860: 7269 7479 2e64 6c6c 0000 0125 1d0d 9100  rity.dll...%....
+00002870: 0001 0016 0258 8074 d086 4eb7 e3fc b0e2  .....X.t..N.....
+00002880: cd22 3553 7973 7465 6d2e 4e65 742e 5365  ."5System.Net.Se
+00002890: 7276 6963 6550 6f69 6e74 2e64 6c6c 0000  rvicePoint.dll..
+000028a0: 01ea 7bb7 c800 8000 000a cce3 6eaa fc06  ..{.........n...
+000028b0: 4292 947c 79ae d821 0a53 7973 7465 6d2e  B..|y..!.System.
+000028c0: 4e65 742e 536f 636b 6574 732e 646c 6c00  Net.Sockets.dll.
+000028d0: 0001 b667 82e2 0000 0100 52ba 356f 9cb6  ...g......R.5o..
+000028e0: b547 958a 3902 0297 251a 5379 7374 656d  .G..9...%.System
+000028f0: 2e4e 6574 2e57 6562 436c 6965 6e74 2e64  .Net.WebClient.d
+00002900: 6c6c 0000 01de 75d8 b100 a000 0061 c26e  ll....u......a.n
+00002910: 6835 0ccd 4f85 dc2f 9b1f 8e52 0053 7973  h5..O../...R.Sys
+00002920: 7465 6d2e 4e65 742e 5765 6248 6561 6465  tem.Net.WebHeade
+00002930: 7243 6f6c 6c65 6374 696f 6e2e 646c 6c00  rCollection.dll.
+00002940: 0001 5298 a3af 0080 0000 9b0f bdce c94d  ..R............M
+00002950: dc4a 819b 4efd 3172 d63f 5379 7374 656d  .J..N.1r.?System
+00002960: 2e4e 6574 2e57 6562 5072 6f78 792e 646c  .Net.WebProxy.dl
+00002970: 6c00 0001 4c21 05ed 0080 0000 b4ff cb6a  l...L!.........j
+00002980: 98e5 2546 bcfe 7ace a33e 78db 5379 7374  ..%F..z..>x.Syst
+00002990: 656d 2e4e 6574 2e57 6562 536f 636b 6574  em.Net.WebSocket
+000029a0: 732e 436c 6965 6e74 2e64 6c6c 0000 018e  s.Client.dll....
+000029b0: 6030 ea00 8000 00d1 cbc2 a741 9dde 489b  `0.........A..H.
+000029c0: 9ef3 e424 25e4 2a53 7973 7465 6d2e 4e65  ...$%.*System.Ne
+000029d0: 742e 5765 6253 6f63 6b65 7473 2e64 6c6c  t.WebSockets.dll
+000029e0: 0000 01f2 6bd8 a000 a000 0018 fa75 49d6  ....k........uI.
+000029f0: 02fa 4cb6 a320 9f5a bdce 1053 7973 7465  ..L.. .Z...Syste
+00002a00: 6d2e 4e75 6d65 7269 6373 2e64 6c6c 0000  m.Numerics.dll..
+00002a10: 0184 9828 ab00 8000 005e c453 95d3 d45e  ...(.....^.S...^
+00002a20: 44bb 10b8 106a aec7 6153 7973 7465 6d2e  D....j..aSystem.
+00002a30: 4e75 6d65 7269 6373 2e56 6563 746f 7273  Numerics.Vectors
+00002a40: 2e64 6c6c 0000 0128 605a dc00 c000 007e  .dll...(`Z.....~
+00002a50: 186e 89d2 cdb6 418a a3b7 3df7 dc27 d753  .n....A...=..'.S
+00002a60: 7973 7465 6d2e 4f62 6a65 6374 4d6f 6465  ystem.ObjectMode
+00002a70: 6c2e 646c 6c00 0001 9f0e 5aac 00c0 0000  l.dll.....Z.....
+00002a80: 67a6 7345 dcc6 104c 8668 0bb2 638b 7324  g.sE...L.h..c.s$
+00002a90: 5379 7374 656d 2e52 6566 6c65 6374 696f  System.Reflectio
+00002aa0: 6e2e 4469 7370 6174 6368 5072 6f78 792e  n.DispatchProxy.
+00002ab0: 646c 6c00 0001 309b 53d8 0080 0000 3a9b  dll...0.S.....:.
+00002ac0: 950e d84e 184c 83d5 f836 66cd e4b5 5379  ...N.L...6f...Sy
+00002ad0: 7374 656d 2e52 6566 6c65 6374 696f 6e2e  stem.Reflection.
+00002ae0: 646c 6c00 0001 7aef 99f4 0080 0000 d4a3  dll...z.........
+00002af0: 74c6 ac2d da40 a910 978d 3860 89b2 5379  t..-.@....8`..Sy
+00002b00: 7374 656d 2e52 6566 6c65 6374 696f 6e2e  stem.Reflection.
+00002b10: 456d 6974 2e64 6c6c 0000 01bd ed33 c000  Emit.dll.....3..
+00002b20: e000 003e e0e1 3102 dfa7 4c9c 39a7 d340  ...>..1...L.9..@
+00002b30: 04f3 7553 7973 7465 6d2e 5265 666c 6563  ..uSystem.Reflec
+00002b40: 7469 6f6e 2e45 6d69 742e 494c 4765 6e65  tion.Emit.ILGene
+00002b50: 7261 7469 6f6e 2e64 6c6c 0000 01ea 8ba1  ration.dll......
+00002b60: b100 a000 0061 47ef bfb1 5a7b 4495 6eab  .....aG...Z{D.n.
+00002b70: 804d a813 3d53 7973 7465 6d2e 5265 666c  .M..=System.Refl
+00002b80: 6563 7469 6f6e 2e45 6d69 742e 4c69 6768  ection.Emit.Ligh
+00002b90: 7477 6569 6768 742e 646c 6c00 0001 3990  tweight.dll...9.
+00002ba0: 09cb 0080 0000 6599 3a9e d785 854c a454  ......e.:....L.T
+00002bb0: 6ac0 387f d650 5379 7374 656d 2e52 6566  j.8..PSystem.Ref
+00002bc0: 6c65 6374 696f 6e2e 4578 7465 6e73 696f  lection.Extensio
+00002bd0: 6e73 2e64 6c6c 0000 01e7 0a6e 9a00 8000  ns.dll.....n....
+00002be0: 00b0 bb2a d038 0c35 4c94 2514 b83e f83a  ...*.8.5L.%..>.:
+00002bf0: d553 7973 7465 6d2e 5265 666c 6563 7469  .System.Reflecti
+00002c00: 6f6e 2e4d 6574 6164 6174 612e 646c 6c00  on.Metadata.dll.
+00002c10: 0001 a1e5 61c2 0020 0200 1e2f 7240 4688  ....a.. .../r@F.
+00002c20: fa4a a99a 89ad 2bf2 7020 5379 7374 656d  .J....+.p System
+00002c30: 2e52 6566 6c65 6374 696f 6e2e 5072 696d  .Reflection.Prim
+00002c40: 6974 6976 6573 2e64 6c6c 0000 0191 2932  itives.dll....)2
+00002c50: ee00 a000 007c 4929 f4b5 222d 4596 77b6  .....|I).."-E.w.
+00002c60: 5a5b 4d24 f353 7973 7465 6d2e 5265 666c  Z[M$.System.Refl
+00002c70: 6563 7469 6f6e 2e54 7970 6545 7874 656e  ection.TypeExten
+00002c80: 7369 6f6e 732e 646c 6c00 0001 3a94 eae3  sions.dll...:...
+00002c90: 0080 0000 89a1 ba5e 6a57 7c45 92e9 ef81  .......^jW|E....
+00002ca0: f8e6 d8da 5379 7374 656d 2e52 6573 6f75  ....System.Resou
+00002cb0: 7263 6573 2e52 6561 6465 722e 646c 6c00  rces.Reader.dll.
+00002cc0: 0001 febc a5b5 0080 0000 c3e8 8ab1 6ba5  ..............k.
+00002cd0: 8849 a02b 6f9c 54f3 bae2 5379 7374 656d  .I.+o.T...System
+00002ce0: 2e52 6573 6f75 7263 6573 2e52 6573 6f75  .Resources.Resou
+00002cf0: 7263 654d 616e 6167 6572 2e64 6c6c 0000  rceManager.dll..
+00002d00: 01bc 85f7 ce00 8000 0017 6017 82e9 ade6  ..........`.....
+00002d10: 4988 c3d0 60bb 8c8c 5d53 7973 7465 6d2e  I...`...]System.
+00002d20: 5265 736f 7572 6365 732e 5772 6974 6572  Resources.Writer
+00002d30: 2e64 6c6c 0000 0183 6b9b 8d00 8000 00f9  .dll....k.......
+00002d40: 827c bb7f 0463 4b99 b7f5 a734 22ca 0853  .|...cK....4"..S
+00002d50: 7973 7465 6d2e 5275 6e74 696d 652e 436f  ystem.Runtime.Co
+00002d60: 6d70 696c 6572 5365 7276 6963 6573 2e55  mpilerServices.U
+00002d70: 6e73 6166 652e 646c 6c00 0001 6c72 7bc8  nsafe.dll...lr{.
+00002d80: 0080 0000 8cd2 862d 3c11 ef44 8746 70b8  .......-<..D.Fp.
+00002d90: 60b6 a3c6 5379 7374 656d 2e52 756e 7469  `...System.Runti
+00002da0: 6d65 2e43 6f6d 7069 6c65 7253 6572 7669  me.CompilerServi
+00002db0: 6365 732e 5669 7375 616c 432e 646c 6c00  ces.VisualC.dll.
+00002dc0: 0001 e4e9 92c1 0080 0000 bbf3 2cba 4956  ............,.IV
+00002dd0: e44c 85e2 eab1 f356 d66c 5379 7374 656d  .L.....V.lSystem
+00002de0: 2e52 756e 7469 6d65 2e64 6c6c 0000 014f  .Runtime.dll...O
+00002df0: a117 ce00 8007 00a3 ef9c 58c3 b940 4d90  ..........X..@M.
+00002e00: cede 3294 d4f3 0453 7973 7465 6d2e 5275  ..2....System.Ru
+00002e10: 6e74 696d 652e 4578 7465 6e73 696f 6e73  ntime.Extensions
+00002e20: 2e64 6c6c 0000 01fb 93c6 cd00 8000 0079  .dll...........y
+00002e30: 3b4b 0168 882e 4592 2115 ec92 b811 7253  ;K.h..E.!.....rS
+00002e40: 7973 7465 6d2e 5275 6e74 696d 652e 4861  ystem.Runtime.Ha
+00002e50: 6e64 6c65 732e 646c 6c00 0001 ebda e6f5  ndles.dll.......
+00002e60: 0080 0000 9cc4 740a 05b5 1a4d 808c 076b  ......t....M...k
+00002e70: abad a534 5379 7374 656d 2e52 756e 7469  ...4System.Runti
+00002e80: 6d65 2e49 6e74 6572 6f70 5365 7276 6963  me.InteropServic
+00002e90: 6573 2e64 6c6c 0000 01af cc8a 9c00 4001  es.dll........@.
+00002ea0: 0080 3b45 973f ea70 4db5 d1a6 3ac2 986c  ..;E.?.pM...:..l
+00002eb0: 8b53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00002ec0: 496e 7465 726f 7053 6572 7669 6365 732e  InteropServices.
+00002ed0: 5275 6e74 696d 6549 6e66 6f72 6d61 7469  RuntimeInformati
+00002ee0: 6f6e 2e64 6c6c 0000 0119 3232 d500 8000  on.dll....22....
+00002ef0: 0007 f899 ecaf 3300 41b1 033e e1e8 7154  ......3.A..>..qT
+00002f00: d753 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+00002f10: 496e 7472 696e 7369 6373 2e64 6c6c 0000  Intrinsics.dll..
+00002f20: 0132 532d 8100 c002 008f 41a5 9a68 4bba  .2S-......A..hK.
+00002f30: 4fb9 819d 1b29 7f51 1f53 7973 7465 6d2e  O....).Q.System.
+00002f40: 5275 6e74 696d 652e 4c6f 6164 6572 2e64  Runtime.Loader.d
+00002f50: 6c6c 0000 01bd 89ce 9900 8000 00cb e5cd  ll..............
+00002f60: 3ba8 4a1f 4892 5b14 edbf bd26 bd53 7973  ;.J.H.[....&.Sys
+00002f70: 7465 6d2e 5275 6e74 696d 652e 4e75 6d65  tem.Runtime.Nume
+00002f80: 7269 6373 2e64 6c6c 0000 0124 2e2e fc00  rics.dll...$....
+00002f90: a000 00c6 9bca 61ba aead 4fa2 bcf1 8b03  ......a...O.....
+00002fa0: 35d5 a853 7973 7465 6d2e 5275 6e74 696d  5..System.Runtim
+00002fb0: 652e 5365 7269 616c 697a 6174 696f 6e2e  e.Serialization.
+00002fc0: 646c 6c00 0001 5732 cda0 0080 0000 96e2  dll...W2........
+00002fd0: 9c85 b24f 0c41 aa16 4e58 5d80 311b 5379  ...O.A..NX].1.Sy
+00002fe0: 7374 656d 2e52 756e 7469 6d65 2e53 6572  stem.Runtime.Ser
+00002ff0: 6961 6c69 7a61 7469 6f6e 2e46 6f72 6d61  ialization.Forma
+00003000: 7474 6572 732e 646c 6c00 0001 8cf0 ff9b  tters.dll.......
+00003010: 00a0 0000 e825 4dad c610 d949 9dbb 619b  .....%M....I..a.
+00003020: 1a21 4f2e 5379 7374 656d 2e52 756e 7469  .!O.System.Runti
+00003030: 6d65 2e53 6572 6961 6c69 7a61 7469 6f6e  me.Serialization
+00003040: 2e4a 736f 6e2e 646c 6c00 0001 8772 c189  .Json.dll....r..
+00003050: 0080 0000 dfbb 2c4f b09b 474a 80eb af14  ......,O..GJ....
+00003060: 4c47 2a68 5379 7374 656d 2e52 756e 7469  LG*hSystem.Runti
+00003070: 6d65 2e53 6572 6961 6c69 7a61 7469 6f6e  me.Serialization
+00003080: 2e50 7269 6d69 7469 7665 732e 646c 6c00  .Primitives.dll.
+00003090: 0001 ca14 3ec6 0080 0000 6ed2 d5f7 b8da  ....>.....n.....
+000030a0: f446 9b4b be28 0c09 e6e8 5379 7374 656d  .F.K.(....System
+000030b0: 2e52 756e 7469 6d65 2e53 6572 6961 6c69  .Runtime.Seriali
+000030c0: 7a61 7469 6f6e 2e58 6d6c 2e64 6c6c 0000  zation.Xml.dll..
+000030d0: 0152 bc99 d400 c000 00c4 715b 4877 e90c  .R........q[Hw..
+000030e0: 41bc 7941 423c b424 5253 7973 7465 6d2e  A.yAB<.$RSystem.
+000030f0: 5365 6375 7269 7479 2e41 6363 6573 7343  Security.AccessC
+00003100: 6f6e 7472 6f6c 2e64 6c6c 0000 01de 06e9  ontrol.dll......
+00003110: b000 e000 00fb c501 60dd 56b5 4b8e 958c  ........`.V.K...
+00003120: 0bbf e0d6 4753 7973 7465 6d2e 5365 6375  ....GSystem.Secu
+00003130: 7269 7479 2e43 6c61 696d 732e 646c 6c00  rity.Claims.dll.
+00003140: 0001 3fae 48a4 00c0 0000 edad 319d 89bd  ..?.H.......1...
+00003150: 704d 90a5 3185 0c1e 2b37 5379 7374 656d  pM..1...+7System
+00003160: 2e53 6563 7572 6974 792e 4372 7970 746f  .Security.Crypto
+00003170: 6772 6170 6879 2e41 6c67 6f72 6974 686d  graphy.Algorithm
+00003180: 732e 646c 6c00 0001 c701 8c95 0000 0100  s.dll...........
+00003190: e8b0 26da db55 544d 84db 4f31 51f8 23db  ..&..UTM..O1Q.#.
+000031a0: 5379 7374 656d 2e53 6563 7572 6974 792e  System.Security.
+000031b0: 4372 7970 746f 6772 6170 6879 2e43 6e67  Cryptography.Cng
+000031c0: 2e64 6c6c 0000 01a7 2137 a900 c000 00d2  .dll....!7......
+000031d0: d896 fb91 538c 4ab8 cd2f c889 004e f053  ....S.J../...N.S
+000031e0: 7973 7465 6d2e 5365 6375 7269 7479 2e43  ystem.Security.C
+000031f0: 7279 7074 6f67 7261 7068 792e 4373 702e  ryptography.Csp.
+00003200: 646c 6c00 0001 52ed 5ec5 00a0 0000 ab21  dll...R.^......!
+00003210: 6ba9 89a5 be41 88ad bbeb 1330 938f 5379  k....A.....0..Sy
+00003220: 7374 656d 2e53 6563 7572 6974 792e 4372  stem.Security.Cr
+00003230: 7970 746f 6772 6170 6879 2e45 6e63 6f64  yptography.Encod
+00003240: 696e 672e 646c 6c00 0001 82cb 6986 00a0  ing.dll.....i...
+00003250: 0000 de52 53ff 2cb4 1d43 a6fe 0857 4f4a  ...RS.,..C...WOJ
+00003260: a648 5379 7374 656d 2e53 6563 7572 6974  .HSystem.Securit
+00003270: 792e 4372 7970 746f 6772 6170 6879 2e4f  y.Cryptography.O
+00003280: 7065 6e53 736c 2e64 6c6c 0000 01d9 3597  penSsl.dll....5.
+00003290: c800 8000 002f 85b5 187e 8878 44b2 9b7a  ...../...~.xD..z
+000032a0: 5607 e643 c653 7973 7465 6d2e 5365 6375  V..C.System.Secu
+000032b0: 7269 7479 2e43 7279 7074 6f67 7261 7068  rity.Cryptograph
+000032c0: 792e 5072 696d 6974 6976 6573 2e64 6c6c  y.Primitives.dll
+000032d0: 0000 01f8 48bd b500 a000 0008 e488 d541  ....H..........A
+000032e0: 95c4 42a9 c1d9 b932 5124 3153 7973 7465  ..B....2Q$1Syste
+000032f0: 6d2e 5365 6375 7269 7479 2e43 7279 7074  m.Security.Crypt
+00003300: 6f67 7261 7068 792e 5835 3039 4365 7274  ography.X509Cert
+00003310: 6966 6963 6174 6573 2e64 6c6c 0000 011e  ificates.dll....
+00003320: 8a31 f300 e000 0038 99aa b575 db67 4e91  .1.....8...u.gN.
+00003330: 674a 6366 4066 c153 7973 7465 6d2e 5365  gJcf@f.System.Se
+00003340: 6375 7269 7479 2e64 6c6c 0000 01d7 281a  curity.dll....(.
+00003350: af00 8000 00fb e9da 24ff 618c 46bd 1b68  ........$.a.F..h
+00003360: 2e35 d8f5 0453 7973 7465 6d2e 5365 6375  .5...System.Secu
+00003370: 7269 7479 2e50 7269 6e63 6970 616c 2e64  rity.Principal.d
+00003380: 6c6c 0000 0197 afa4 d700 8000 0027 8a16  ll...........'..
+00003390: bac0 9544 4aa4 52ae 3e07 2e8d 6253 7973  ...DJ.R.>...bSys
+000033a0: 7465 6d2e 5365 6375 7269 7479 2e50 7269  tem.Security.Pri
+000033b0: 6e63 6970 616c 2e57 696e 646f 7773 2e64  ncipal.Windows.d
+000033c0: 6c6c 0000 0137 b68c a200 a000 0007 4c72  ll...7........Lr
+000033d0: b4ef d98a 4a8d 474f 44c7 e710 ea53 7973  ....J.GOD....Sys
+000033e0: 7465 6d2e 5365 6375 7269 7479 2e53 6563  tem.Security.Sec
+000033f0: 7572 6553 7472 696e 672e 646c 6c00 0001  ureString.dll...
+00003400: 8ba7 83bf 0080 0000 cb5c 39de 14de 2e48  .........\9....H
+00003410: ac1c 4ab6 b5b4 9011 5379 7374 656d 2e53  ..J.....System.S
+00003420: 6572 7669 6365 4d6f 6465 6c2e 5765 622e  erviceModel.Web.
+00003430: 646c 6c00 0001 3dd3 54b3 0080 0000 a43a  dll...=.T......:
+00003440: 99fe eb55 9248 bbc3 a67b b1ba 123d 5379  ...U.H...{...=Sy
+00003450: 7374 656d 2e53 6572 7669 6365 5072 6f63  stem.ServiceProc
+00003460: 6573 732e 646c 6c00 0001 899a cec1 0080  ess.dll.........
+00003470: 0000 5539 1e62 bd38 4d42 896d f311 a44b  ..U9.b.8MB.m...K
+00003480: efb1 5379 7374 656d 2e54 6578 742e 456e  ..System.Text.En
+00003490: 636f 6469 6e67 2e43 6f64 6550 6167 6573  coding.CodePages
+000034a0: 2e64 6c6c 0000 013c 2e5d f600 8000 00e1  .dll...<.]......
+000034b0: b1ec fb2f d5b5 44a0 24ad c731 b431 0053  .../..D.$..1.1.S
+000034c0: 7973 7465 6d2e 5465 7874 2e45 6e63 6f64  ystem.Text.Encod
+000034d0: 696e 672e 646c 6c00 0001 80b4 14a3 0080  ing.dll.........
+000034e0: 0000 9ce3 b249 0b7e 8e43 9049 d265 90a2  .....I.~.C.I.e..
+000034f0: e97d 5379 7374 656d 2e54 6578 742e 456e  .}System.Text.En
+00003500: 636f 6469 6e67 2e45 7874 656e 7369 6f6e  coding.Extension
+00003510: 732e 646c 6c00 0001 3f1b b5b0 00a0 0000  s.dll...?.......
+00003520: 354c 6745 cf2e 034a ad89 10f2 c783 bf90  5LgE...J........
+00003530: 5379 7374 656d 2e54 6578 742e 456e 636f  System.Text.Enco
+00003540: 6469 6e67 732e 5765 622e 646c 6c00 0001  dings.Web.dll...
+00003550: b007 b8df 00a0 0000 b7cd 6a87 6293 da46  ..........j.b..F
+00003560: 8545 efbb 2261 49c1 5379 7374 656d 2e54  .E.."aI.System.T
+00003570: 6578 742e 4a73 6f6e 2e64 6c6c 0000 012f  ext.Json.dll.../
+00003580: 3d98 cb00 2001 00b1 04e5 583b b9ad 419e  =... .....X;..A.
+00003590: 3eda 6af1 8497 7d53 7973 7465 6d2e 5465  >.j...}System.Te
+000035a0: 7874 2e52 6567 756c 6172 4578 7072 6573  xt.RegularExpres
+000035b0: 7369 6f6e 732e 646c 6c00 0001 7742 4fab  sions.dll...wBO.
+000035c0: 00c0 0000 c770 ed57 161f 3e47 af43 d65f  .....p.W..>G.C._
+000035d0: 9424 cc8a 5379 7374 656d 2e54 6872 6561  .$..System.Threa
+000035e0: 6469 6e67 2e43 6861 6e6e 656c 732e 646c  ding.Channels.dl
+000035f0: 6c00 0001 34bd fda0 0080 0000 3eb0 35d8  l...4.......>.5.
+00003600: 8199 f847 a870 6faa 4125 5e13 5379 7374  ...G.po.A%^.Syst
+00003610: 656d 2e54 6872 6561 6469 6e67 2e64 6c6c  em.Threading.dll
+00003620: 0000 01d3 c2ec 9700 c000 0079 d76d 0a6c  ...........y.m.l
+00003630: 4cde 42b1 e029 f8d3 f114 1f53 7973 7465  L.B..).....Syste
+00003640: 6d2e 5468 7265 6164 696e 672e 4f76 6572  m.Threading.Over
+00003650: 6c61 7070 6564 2e64 6c6c 0000 0178 ccd2  lapped.dll...x..
+00003660: a700 8000 0007 8bfa 9af2 34bb 42a1 453c  ..........4.B.E<
+00003670: abbf a67e b753 7973 7465 6d2e 5468 7265  ...~.System.Thre
+00003680: 6164 696e 672e 5461 736b 732e 4461 7461  ading.Tasks.Data
+00003690: 666c 6f77 2e64 6c6c 0000 016a 9fb3 f100  flow.dll...j....
+000036a0: c000 0057 1ee8 dc8f c8e2 4a9a 65f4 a83c  ...W......J.e..<
+000036b0: 8ea0 fb53 7973 7465 6d2e 5468 7265 6164  ...System.Thread
+000036c0: 696e 672e 5461 736b 732e 646c 6c00 0001  ing.Tasks.dll...
+000036d0: 0ec2 eab6 0080 0000 6555 7af7 eadb 8e4a  ........eUz....J
+000036e0: b632 8c91 7360 3ac0 5379 7374 656d 2e54  .2..s`:.System.T
+000036f0: 6872 6561 6469 6e67 2e54 6173 6b73 2e45  hreading.Tasks.E
+00003700: 7874 656e 7369 6f6e 732e 646c 6c00 0001  xtensions.dll...
+00003710: 0d9a feea 0080 0000 f3e4 81af 9578 2242  .............x"B
+00003720: bb05 7b41 707b b388 5379 7374 656d 2e54  ..{Ap{..System.T
+00003730: 6872 6561 6469 6e67 2e54 6173 6b73 2e50  hreading.Tasks.P
+00003740: 6172 616c 6c65 6c2e 646c 6c00 0001 a67f  arallel.dll.....
+00003750: 5b80 0080 0000 5c62 7c74 ec73 8e4e b839  [.....\b|t.s.N.9
+00003760: 6f02 5da1 a896 5379 7374 656d 2e54 6872  o.]...System.Thr
+00003770: 6561 6469 6e67 2e54 6872 6561 642e 646c  eading.Thread.dl
+00003780: 6c00 0001 bb81 fb87 00a0 0000 e0b9 fc04  l...............
+00003790: 8874 0b40 9ba3 b7d0 1384 5979 5379 7374  .t.@......YySyst
+000037a0: 656d 2e54 6872 6561 6469 6e67 2e54 6872  em.Threading.Thr
+000037b0: 6561 6450 6f6f 6c2e 646c 6c00 0001 13dd  eadPool.dll.....
+000037c0: 58a8 0080 0000 9b33 fec3 3559 9e4a a6d4  X......3..5Y.J..
+000037d0: 0131 935f 9a55 5379 7374 656d 2e54 6872  .1._.USystem.Thr
+000037e0: 6561 6469 6e67 2e54 696d 6572 2e64 6c6c  eading.Timer.dll
+000037f0: 0000 012c 6170 9600 8000 008f a3c6 bd14  ...,ap..........
+00003800: b84c 4ea9 0b55 2fa7 ee6f 7c53 7973 7465  .LN..U/..o|Syste
+00003810: 6d2e 5472 616e 7361 6374 696f 6e73 2e64  m.Transactions.d
+00003820: 6c6c 0000 01b6 6269 8000 8000 0032 370a  ll....bi.....27.
+00003830: 9851 5f81 4882 e391 2b9c ba95 e953 7973  .Q_.H...+....Sys
+00003840: 7465 6d2e 5472 616e 7361 6374 696f 6e73  tem.Transactions
+00003850: 2e4c 6f63 616c 2e64 6c6c 0000 01d1 1503  .Local.dll......
+00003860: 9700 a000 0065 2922 d1f3 3d59 4dbc 04a1  .....e)"..=YM...
+00003870: 7e7c 7099 ee53 7973 7465 6d2e 5661 6c75  ~|p..System.Valu
+00003880: 6554 7570 6c65 2e64 6c6c 0000 0157 aaac  eTuple.dll...W..
+00003890: b900 8000 009d 5a87 c7ad 3ff1 47a7 9196  ......Z...?.G...
+000038a0: b0b9 8f8d 8f53 7973 7465 6d2e 5765 622e  .....System.Web.
+000038b0: 646c 6c00 0001 4e23 e2cb 0080 0000 e6e7  dll...N#........
+000038c0: 1a23 27f3 4c49 94ec a1a6 803d 461c 5379  .#'.LI.....=F.Sy
+000038d0: 7374 656d 2e57 6562 2e48 7474 7055 7469  stem.Web.HttpUti
+000038e0: 6c69 7479 2e64 6c6c 0000 0131 94f5 db00  lity.dll...1....
+000038f0: 8000 007a ac04 a898 e8be 4792 f630 01a8  ...z......G..0..
+00003900: f4ec c453 7973 7465 6d2e 5769 6e64 6f77  ...System.Window
+00003910: 732e 646c 6c00 0001 6f48 e4a1 0080 0000  s.dll...oH......
+00003920: f3d1 e27f 7302 b54a a4db e65a e300 054e  ....s..J...Z...N
+00003930: 5379 7374 656d 2e58 6d6c 2e64 6c6c 0000  System.Xml.dll..
+00003940: 01d6 1f9e c900 a000 008f 30e0 f426 0edf  ..........0..&..
+00003950: 42a4 a2ad eeb4 311a c753 7973 7465 6d2e  B.....1..System.
+00003960: 586d 6c2e 4c69 6e71 2e64 6c6c 0000 01a6  Xml.Linq.dll....
+00003970: 3c94 9f00 8000 0057 8590 7147 a8f6 46b3  <......W..qG..F.
+00003980: 0f20 8504 17ca 0e53 7973 7465 6d2e 586d  . .....System.Xm
+00003990: 6c2e 5265 6164 6572 5772 6974 6572 2e64  l.ReaderWriter.d
+000039a0: 6c6c 0000 0118 5d09 c400 0002 00cc 4d0c  ll....].......M.
+000039b0: 99ac a283 4da7 237e 2215 a46b 5553 7973  ....M.#~"..kUSys
+000039c0: 7465 6d2e 586d 6c2e 5365 7269 616c 697a  tem.Xml.Serializ
+000039d0: 6174 696f 6e2e 646c 6c00 0001 ba95 f98d  ation.dll.......
+000039e0: 0080 0000 e090 daba 8a7c 774e bbd6 4159  .........|wN..AY
+000039f0: 9902 3cf0 5379 7374 656d 2e58 6d6c 2e58  ..<.System.Xml.X
+00003a00: 446f 6375 6d65 6e74 2e64 6c6c 0000 01e7  Document.dll....
+00003a10: a6eb a600 c000 004f c15e 4b58 f36a 4182  .......O.^KX.jA.
+00003a20: 97ea 9b66 8fac 4053 7973 7465 6d2e 586d  ...f..@System.Xm
+00003a30: 6c2e 586d 6c44 6f63 756d 656e 742e 646c  l.XmlDocument.dl
+00003a40: 6c00 0001 598a 6bbf 0080 0000 a48e 3b4b  l...Y.k.......;K
+00003a50: 693f 6544 9260 55b3 fc15 0f6b 5379 7374  i?eD.`U....kSyst
+00003a60: 656d 2e58 6d6c 2e58 6d6c 5365 7269 616c  em.Xml.XmlSerial
+00003a70: 697a 6572 2e64 6c6c 0000 0154 3213 e500  izer.dll...T2...
+00003a80: 0001 00d7 2bb6 9ceb 003d 488b 5a6d baac  ....+....=H.Zm..
+00003a90: 634c 1d53 7973 7465 6d2e 586d 6c2e 5850  cL.System.Xml.XP
+00003aa0: 6174 682e 646c 6c00 0001 7d58 6acd 0080  ath.dll...}Xj...
+00003ab0: 0000 b5ae a120 b4fc aa4d b1b1 b538 b71e  ..... ...M...8..
+00003ac0: 8822 5379 7374 656d 2e58 6d6c 2e58 5061  ."System.Xml.XPa
+00003ad0: 7468 2e58 446f 6375 6d65 6e74 2e64 6c6c  th.XDocument.dll
+00003ae0: 0000 0183 736c c600 8000 0058 b7df 8d54  ....sl.....X...T
+00003af0: 8252 4a8a 97c7 8e66 9354 a555 6e64 6572  .RJ....f.T.Under
+00003b00: 7461 6c65 4d6f 644c 6962 2e64 6c6c 0000  taleModLib.dll..
+00003b10: 019b f66e ff00 2003 0090 9cab 0b12 8da2  ...n.. .........
+00003b20: 418c 4e3a 2c98 30b2 3357 696e 646f 7773  A.N:,.0.3Windows
+00003b30: 4261 7365 2e64 6c6c 0000 0114 1787 b000  Base.dll........
+00003b40: 8000 003c 440f c83d 91f4 4796 13af 540a  ...<D..=..G...T.
+00003b50: 1d28 c015 0100 0046 0f09 1000 1502 0003  .(.....F........
+00003b60: 000a 002c 0600 3d04 5514 5369 784c 6162  ...,..=.U.SixLab
+00003b70: 6f72 732e 496d 6167 6553 6861 7270 2153  ors.ImageSharp!S
+00003b80: 6978 4c61 626f 7273 2e49 6d61 6765 5368  ixLabors.ImageSh
+00003b90: 6172 702e 5069 7865 6c46 6f72 6d61 7473  arp.PixelFormats
+00003ba0: 1f53 6978 4c61 626f 7273 2e49 6d61 6765  .SixLabors.Image
+00003bb0: 5368 6172 702e 5072 6f63 6573 7369 6e67  Sharp.Processing
+00003bc0: 0653 7973 7465 6d1a 5379 7374 656d 2e43  .System.System.C
+00003bd0: 6f6c 6c65 6374 696f 6e73 2e47 656e 6572  ollections.Gener
+00003be0: 6963 0953 7973 7465 6d2e 494f 0b53 7973  ic.System.IO.Sys
+00003bf0: 7465 6d2e 4c69 6e71 0f53 7973 7465 6d2e  tem.Linq.System.
+00003c00: 4e65 742e 4874 7470 1053 7973 7465 6d2e  Net.Http.System.
+00003c10: 5468 7265 6164 696e 6716 5379 7374 656d  Threading.System
+00003c20: 2e54 6872 6561 6469 6e67 2e54 6173 6b73  .Threading.Tasks
+00003c30: 1453 7973 7465 6d2e 476c 6f62 616c 697a  .System.Globaliz
+00003c40: 6174 696f 6e11 5379 7374 656d 2e52 6566  ation.System.Ref
+00003c50: 6c65 6374 696f 6e10 5379 7374 656d 2e54  lection.System.T
+00003c60: 6578 742e 4a73 6f6e 0f55 6e64 6572 7461  ext.Json.Underta
+00003c70: 6c65 4d6f 644c 6962 1a55 6e64 6572 7461  leModLib.Underta
+00003c80: 6c65 4d6f 644c 6962 2e44 6563 6f6d 7069  leModLib.Decompi
+00003c90: 6c65 7216 556e 6465 7274 616c 654d 6f64  ler.UndertaleMod
+00003ca0: 4c69 622e 4d6f 6465 6c73 2053 6978 4c61  Lib.Models SixLa
+00003cb0: 626f 7273 2e49 6d61 6765 5368 6172 702e  bors.ImageSharp.
+00003cc0: 466f 726d 6174 732e 506e 6733 01a7 9501  Formats.Png3....
+00003cd0: a7aa 01a7 cc01 a7ec 01a7 f301 a80e 01a8  ................
+00003ce0: 1801 a824 01a8 3401 a845 01a8 5c01 a871  ...$..4..E..\..q
+00003cf0: 01a8 8301 a894 01a8 a401 a8bf 01a8 d695  ................
+00003d00: 5402 0000 0006 003a 2009 0a00 5404 000d  T......: ...T...
+00003d10: 0021 1600 0b00 3104 0e0d 001e 047b 1000  .!....1......{..
+00003d20: 0102 7902 0000 0b00 0001 0041 0200 1200  ..y........A....
+00003d30: 4b80 8a00 0b00 1104 0007 000d 0026 0700  K............&..
+00003d40: 1600 1e07 0045 023d 1500 3302 000b 0049  .....E.=..3....I
+00003d50: 0200 2000 2b02 0016 0063 5400 1f00 1b02  .. .+....cT.....
+00003d60: 0e07 002c 047b 1200 6202 001d 0001 0279  ...,.{..b......y
+00003d70: 0200 000b 0000 0100 0007 004a 0808 2700  ...........J..'.
+00003d80: 4c02 0027 0080 8602 0019 003d 0200 2200  L..'.......=..".
+00003d90: 4802 0022 0064 0200 1400 1b02 0e07 0029  H..".d.........)
+00003da0: 047b 0e00 3902 001d 0001 0279 0200 000b  .{..9......y....
+00003db0: 0000 0100 4c04 0027 004e 0200 2700 808b  ....L..'.N..'...
+00003dc0: 0200 1900 3f02 0022 004a 0200 2200 6802  ....?..".J..".h.
+00003dd0: 0014 001b 020e 0700 2a04 7b0e 003a 0200  ........*.{..:..
+00003de0: 1d00 0102 7902 0000 0b00 0001 0072 0679  ....y........r.y
+00003df0: 3b00 7802 003b 0078 0200 3b00 7e02 003b  ;.x..;.x..;.~..;
+00003e00: 006b 0200 3b00 80a6 0200 5600 80a6 0200  .k..;.....V.....
+00003e10: 5600 80a6 0200 5600 80a6 0200 5600 80a6  V.....V.....V...
+00003e20: 0200 5600 80a6 0200 5600 80a6 0200 5600  ..V.....V.....V.
+00003e30: 80ae 0400 5600 80bc 0200 5600 80b4 0200  ....V.....V.....
+00003e40: 5600 80b2 0200 5600 809d 0600 4b00 809f  V.....V.....K...
+00003e50: 0200 4b00 8099 0200 4b00 7506 0046 0078  ..K.....K.u..F.x
+00003e60: 0200 4600 7602 0046 0076 0200 4600 7702  ..F.v..F.v..F.w.
+00003e70: 0046 0080 a206 004b 0080 a002 004b 0080  .F.....K.....K..
+00003e80: a202 004b 0080 a202 004b 0080 9f02 004b  ...K.....K.....K
+00003e90: 0080 9c02 004b 0080 9e02 004b 0080 9d02  .....K.....K....
+00003ea0: 004b 0080 a402 004b 0080 9e02 004b 0080  .K.....K.....K..
+00003eb0: a002 004b 0080 a002 004b 0080 9e02 004b  ...K.....K.....K
+00003ec0: 0080 9e02 004b 0080 9f02 004b 0080 9d02  .....K.....K....
+00003ed0: 004b 0080 a402 004b 0080 9d02 004b 0080  .K.....K.....K..
+00003ee0: 9d02 004b 0080 9d02 004b 0032 0600 2000  ...K.....K.2.. .
+00003ef0: 8099 0200 4b00 8099 0200 4b00 8099 0200  ....K.....K.....
+00003f00: 4b00 8099 0200 4b00 8099 0200 4b00 8099  K.....K.....K...
+00003f10: 0200 4b00 8099 0200 4b00 8099 0200 4b00  ..K.....K.....K.
+00003f20: 8099 0200 4b0b 0604 0081 450b 061a 0081  ....K.....E.....
+00003f30: 370e 061a 0082 0f18 0620 0084 2b0b 0634  7........ ..+..4
+00003f40: 0081 450b 061a 0081 4500 391a 0020 0080  ..E.....E.9.. ..
+00003f50: a602 004b 0080 a602 004b 0080 a602 004b  ...K.....K.....K
+00003f60: 0080 a602 004b 0039 0400 2000 80a6 0200  .....K.9.. .....
+00003f70: 4b00 80a6 0200 4b00 80a6 0200 4b00 80a6  K.....K.....K...
+00003f80: 0200 4b00 80a6 0200 4b00 80a6 0200 4b00  ..K.....K.....K.
+00003f90: 80a6 0200 4b00 80a6 0200 4b00 80a6 0200  ....K.....K.....
+00003fa0: 4b00 80a7 0200 4b00 80a7 0200 4b00 80a7  K.....K.....K...
+00003fb0: 0200 4b00 80a7 0200 4b00 80a7 0200 4b00  ..K.....K.....K.
+00003fc0: 80a7 0200 4b00 80a7 0200 4b0a 0604 0081  ....K.....K.....
+00003fd0: 1637 0618 008a 9612 0672 0082 e712 0628  .7.......r.....(
+00003fe0: 0082 e712 0628 0082 e70f 0628 0082 450a  .....(.....(..E.
+00003ff0: 0624 0081 4700 2f2e 000d 002b 0442 2200  .$..G./....+.B".
+00004000: 0002 0010 0059 0900 5f04 7717 0002 7d2c  .....Y.._.w...},
+00004010: 0b00 000b 0000 0100 300e 450d 0060 0442  ........0.E..`.B
+00004020: 4200 0002 0010 0059 0900 6004 7717 0002  B......Y..`.w...
+00004030: 7d2c 0b00 000b 0000 0100 2d0e 4510 0181  },........-.E...
+00004040: 1804 2e60 0000 0200 0600 6d09 0053 0677  ...`......m..S.w
+00004050: 1700 027b 180b 0000 0e05 0412 5945 0079  ...{........YE.y
+00004060: 0c00 2100 5602 000c 0025 0200 1100 3702  ..!.V....%....7.
+00004070: 000c 0040 0200 0700 3102 0008 0039 0200  ...@....1....9..
+00004080: 0700 2402 0008 0034 0200 0e00 3002 0007  ..$....4....0...
+00004090: 0075 0200 2200 7502 000d 0023 0200 1200  .u..".u....#....
+000040a0: 3502 000c 003c 0200 0700 2f02 0009 0035  5....<..../....5
+000040b0: 0200 0700 2402 0008 0034 0200 0e00 2e02  ....$....4......
+000040c0: 0007 0027 0200 1100 4d04 0018 0034 0600  ...'....M....4..
+000040d0: 1c00 3502 001d 004f 0600 1800 5702 0013  ..5....O....W...
+000040e0: 0180 d202 0027 0048 0800 1800 5f02 000d  .....'.H...._...
+000040f0: 0059 0200 2100 5606 0021 0080 9006 0027  .Y..!.V..!.....'
+00004100: 0280 a606 0027 0080 9e0a 0027 003c 0600  .....'.....'.<..
+00004110: 1800 808a 0200 1300 8082 0200 1300 8084  ................
+00004120: 0200 1300 7f02 0013 005e 022a 2a00 0002  .........^.**...
+00004130: 0008 0069 0700 4804 7724 0048 0200 2400  ...i..H.w$.H..$.
+00004140: 0006 0002 7b1c 0801 809a 0e5d 2700 6806  ....{......]'.h.
+00004150: 0027 0059 0600 2100 8085 0200 2700 7406  .'.Y..!.....'.t.
+00004160: 0021 0074 0200 2100 7402 0021 0074 0200  .!.t..!.t..!.t..
+00004170: 2100 4c06 321b 0000 0200 0c00 6107 003d  !.L.2.......a..=
+00004180: 0277 1e00 0006 0002 7f24 0800 2d08 5512  .w.......$..-.U.
+00004190: 0068 0208 2701 80da 0679 2100 6904 0021  .h..'....y!.i..!
+000041a0: 0077 0600 2700 7e02 0027 0075 0200 2703  .w..'.~..'.u..'.
+000041b0: 6306 3266 0000 0200 0c00 6107 0034 0877  c.2f......a..4.w
+000041c0: 1e00 0006 0002 7924 0800 8090 0a55 2103  ......y$.....U!.
+000041d0: 80e4 0600 2700 720e 0027 002d 0200 0700  ....'.r..'.-....
+000041e0: 5702 001c 026e 0200 0d00 2406 0012 0045  W....n....$....E
+000041f0: 0200 2100 3a02 0007 002a 0200 0900 3302  ..!.:....*....3.
+00004200: 0007 0020 0200 0c00 2802 000e 0024 0200  ... ....(....$..
+00004210: 0706 8088 0800 0700 808e 1032 2b00 0002  ...........2+...
+00004220: 000c 0061 0700 5402 7721 0000 0600 027f  ...a..T.w!......
+00004230: 2408 0029 0a55 0700 5b02 2e17 0000 0200  $..).U..[.......
+00004240: 0a00 6507 002e 0477 0f00 3102 082f 0000  ..e....w..1../..
+00004250: 0600 027b 1808 0480 900a 5933 0480 860a  ...{......Y3....
+00004260: 0033 0025 0c00 0700 1b02 2e1b 0000 0200  .3.%............
+00004270: 0a00 6507 002e 0477 0f00 2d02 082f 0000  ..e....w..-../..
+00004280: 0600 027b 1808 0480 880a 5933 047e 0a00  ...{......Y3.~..
+00004290: 3300 80a4 1000 2100 5e04 0027 005e 0200  3.....!.^..'.^..
+000042a0: 2700 6106 0027 004f 0600 2100 5506 321b  '.a..'.O..!.U.2.
+000042b0: 0000 0200 0c00 6107 007c 0277 2400 0006  ......a..|.w$...
+000042c0: 0002 7f24 0800 710c 5522 0074 0200 2200  ...$..q.U".t..".
+000042d0: 2102 0012 0022 0200 1209 0602 007a 0906  !....".......z..
+000042e0: 1400 7d00 7818 0022 0024 0200 1200 2f02  ..}.x..".$..../.
+000042f0: 0016 0906 0200 6500 4316 002c 0010 0200  ......e.C..,....
+00004300: 0900 3602 0018 002c 0200 0900 1702 0009  ..6....,........
+00004310: 0016 0200 0900 3f04 002c 0010 0200 0900  ......?..,......
+00004320: 2c02 0009 0017 0200 0900 1602 0009 003f  ,..............?
+00004330: 0400 2c00 1002 0009 002c 0200 0900 1702  ..,......,......
+00004340: 0009 0016 0200 0900 3f04 002c 0010 0200  ........?..,....
+00004350: 0900 2c02 0009 0017 0200 0900 1502 0008  ..,.............
+00004360: 0a04 0400 6500 1d16 000d 0a04 0400 6500  ....e.........e.
+00004370: 1d16 000d 0a04 0400 6200 1d16 000d 0a04  ........b.......
+00004380: 0400 6100 1d16 000c 0035 0600 1800 0b02  ..a......5......
+00004390: 0a07 0000 0500 2304 7f07 0035 0200 2800  ......#....5..(.
+000043a0: 1a02 0009 0021 0400 0700 4d02 0049 0044  .....!....M..I.D
+000043b0: 0200 1e00 1802 0012 0023 0200 0d00 3302  .........#....3.
+000043c0: 0007 0017 0200 0900 2d02 0007 001b 0200  ........-.......
+000043d0: 0e00 1c02 0007 0024 0400 0700 5502 0049  .......$....U..I
+000043e0: 001b 0200 1200 2602 000d 002f 0200 0700  ......&..../....
+000043f0: 1a02 0009 0029 0200 0700 1a02 000c 001b  .....)..........
+00004400: 0200 0e00 1f02 0007 001b 0200 1200 034b  ...............K
+00004410: 3006 0008 006d 0c0e 123e 5d13 0050 1e00  0....m...>]..P..
+00004420: 2700 5002 0027 0026 0600 0700 4802 001c  '.P..'.&....H...
+00004430: 5d12 0200 0d00 1d80 bc00 1200 7102 0038  ]...........q..8
+00004440: 0181 7a06 0013 0181 7a04 0013 0080 aa08  ..z.....z.......
+00004450: 2a33 0000 0200 0800 6907 003c 0277 2400  *3......i..<.w$.
+00004460: 0006 0002 7f1c 0800 80ef 080c 3b00 0002  ............;...
+00004470: 000b 0063 0700 6302 7724 0000 0600 027f  ...c..c.w$......
+00004480: 2208 003c 0857 1800 4302 0013 0048 0200  "..<.W..C....H..
+00004490: 1300 8093 0200 2700 8093 0200 2701 6802  ......'.....'.h.
+000044a0: 0027 0054 0400 1800 7202 0013 0070 0200  .'.T....r....p..
+000044b0: 1300 8089 0200 1300 80af 0200 1300 808d  ................
+000044c0: 0200 1300 6e02 0027 0021 0600 1000 3606  ....n..'.!....6.
+000044d0: 0818 004b 0200 1800 4b02 0018 0049 0200  ...K....K....I..
+000044e0: 1800 4a02 0018 003d 0200 1800 3702 0018  ..J....=....7...
+000044f0: 003f 0200 1800 5c02 0031 0055 0200 3100  .?....\..1.U..1.
+00004500: 5602 0032 0055 0200 3100 5502 0031 0056  V..2.U..1.U..1.V
+00004510: 0200 3200 5602 0032 0056 0200 3200 5602  ..2.V..2.V..2.V.
+00004520: 002e 0052 0400 2b00 4902 002b 0052 0200  ...R..+.I..+.R..
+00004530: 2b00 7204 0022 0066 0200 0d00 2102 0012  +.r..".f....!...
+00004540: 0059 0200 2c00 6902 0012 0033 0600 1800  .Y..,.i....3....
+00004550: 6002 0031 0058 0200 3000 5a02 0032 0059  `..1.X..0.Z..2.Y
+00004560: 0200 3100 5a02 0032 0059 0200 3100 5a02  ..1.Z..2.Y..1.Z.
+00004570: 0032 005a 0200 3200 4f06 002b 0046 0200  .2.Z..2.O..+.F..
+00004580: 2b00 4f02 002b 0046 0400 1200 6f04 0022  +.O..+.F....o.."
+00004590: 0064 0200 0d00 1e02 0012 0053 0200 2c00  .d.........S..,.
+000045a0: 5d06 0032 0035 0800 1800 5d02 002e 0056  ]..2.5....]....V
+000045b0: 0200 2e00 5702 002f 0057 0200 2e00 5602  ....W../.W....V.
+000045c0: 002e 0057 0200 2f00 5702 002f 0058 0200  ...W../.W../.X..
+000045d0: 2f00 5708 0038 0056 0200 3800 5e02 0032  /.W..8.V..8.^..2
+000045e0: 0050 0400 2800 4702 0028 0050 0200 2800  .P..(.G..(.P..(.
+000045f0: 4904 0012 0071 0400 2200 6602 000d 0020  I....q..".f.... 
+00004600: 0200 1200 5602 0029 0039 0600 1800 6202  ....V..).9....b.
+00004610: 0031 005a 0200 3000 5c02 0032 005b 0200  .1.Z..0.\..2.[..
+00004620: 3100 5c02 0032 005b 0200 3100 5c02 0032  1.\..2.[..1.\..2
+00004630: 005c 0200 3200 5f08 0038 005f 0200 3800  .\..2._..8._..8.
+00004640: 5f02 0038 005f 0200 3800 6f02 0045 0055  _..8._..8.o..E.U
+00004650: 0400 2b00 4c02 002b 0055 0200 2b00 7504  ..+.L..+.U..+.u.
+00004660: 0022 0068 0200 0d00 2402 0012 005f 0200  .".h....$...._..
+00004670: 2c00 4a04 0012 0080 8906 0027 0080 8902  ,.J........'....
+00004680: 0027 0080 8702 0027 0080 8902 0027 0181  .'.....'.....'..
+00004690: 6c1e 7927 0181 6c04 0027 0181 6c04 0027  l.y'..l..'..l..'
+000046a0: 0181 6c04 0027 0080 ba08 0021 0030 0600  ..l..'.....!.0..
+000046b0: 1600 2e02 0007 0010 0200 0900 1002 0009  ................
+000046c0: 0014 0200 0c00 1402 000c 0033 0200 2500  ...........3..%.
+000046d0: 4102 001d 0027 0200 0700 5602 001c 006f  A....'....V....o
+000046e0: 0200 0d00 1e02 0012 0025 0200 0900 2302  .........%....#.
+000046f0: 000d 0b06 0200 808a 0b06 1800 808c 007c  ...............|
+00004700: 1c00 2702 8098 0600 4d00 3f0a 0018 0063  ..'.....M.?....c
+00004710: 0200 1300 7006 0013 005c 0600 2700 5c02  ....p....\..'.\.
+00004720: 0027 0180 9406 0027 0181 2c0e 000d 006d  .'.....'..,....m
+00004730: 0c00 1300 8081 0200 1300 5502 0013 006a  ..........U....j
+00004740: 0200 1300 4f02 0013 0061 0200 1300 6802  ....O....a....h.
+00004750: 0013 0046 0600 1802 8156 0200 1300 4106  ...F.....V....A.
+00004760: 0018 0069 0200 1308 7b08 0013 087b 1200  ...i....{....{..
+00004770: 1308 7b16 0013 087b 1200 1308 7b16 0013  ..{....{....{...
+00004780: 087b 1200 1300 4716 0018 0080 9602 0013  .{....G.........
+00004790: 0080 b502 0013 0912 0600 1300 5a14 0013  ............Z...
+000047a0: 0181 1a0e 000d 003c 0800 0d00 6b06 000d  .......<....k...
+000047b0: 0080 8006 0026 0080 8402 002c 0181 0406  .....&.....,....
+000047c0: 000d 0180 ce08 000d 0059 0400 1808 7b02  .........Y....{.
+000047d0: 0013 0079 1200 1300 6304 0018 087b 0200  ...y....c....{..
+000047e0: 1300 8083 1200 1300 5904 0018 087b 0200  ........Y....{..
+000047f0: 1300 7912 0013 005a 0400 1808 7b02 0013  ..y....Z....{...
+00004800: 0076 1200 1302 814c 0600 0d1e 1a0a 0013  .v.....L........
+00004810: 0181 003e 0013 007b 0800 2700 4f06 0018  ...>...{..'.O...
+00004820: 004f 0200 1300 4e02 0018 0048 0200 1303  .O....N....H....
+00004830: 6b04 284b 0000 0200 0800 6907 0050 0879  k.(K......i..P.y
+00004840: 2400 0006 0002 791a 0800 3e0a 5f1c 000c  $.....y...>._...
+00004850: 023e 1200 0002 0012 0055 0700 6004 4632  .>.......U..`.F2
+00004860: 0000 0200 1b00 4309 004d 0277 1800 027f  ......C..M.w....
+00004870: 420b 0000 0b00 0001 0002 7d67 0b00 000b  B.........}g....
+00004880: 0000 0100 4c10 4913 0053 0200 1300 4d06  ....L.I..S....M.
+00004890: 0013 0054 0200 1301 8084 023e 3600 0002  ...T.......>6...
+000048a0: 0012 0055 0900 4104 7713 0002 7d30 0b00  ...U..A.w...}0..
+000048b0: 000b 0000 0100 4b0a 4913 0052 0200 1300  ......K.I..R....
+000048c0: 7602 0027 0050 0600 1800 4a02 0013 0050  v..'.P....J....P
+000048d0: 0200 1301 813a 0228 3600 0002 0008 0069  .....:.(6......i
+000048e0: 0900 3d04 7913 0002 7d1a 0b00 000b 0000  ..=.y...}.......
+000048f0: 0100 4f0a 5f18 0049 0200 1300 4f02 0013  ..O._..I....O...
+00004900: 0080 8802 282b 0000 0200 0800 6907 0050  ....(+......i..P
+00004910: 0279 2400 0006 0002 7f1a 0800 4d08 5f13  .y$.........M._.
+00004920: 0053 0200 1302 8096 0228 3600 0002 0008  .S.......(6.....
+00004930: 0069 0900 4606 7913 0002 7b1a 0b00 000b  .i..F.y...{.....
+00004940: 0000 0100 500c 5f13 0056 0200 1301 80d6  ....P._..V......
+00004950: 0228 3600 0002 0008 0069 0900 4904 7913  .(6......i..I.y.
+00004960: 0002 7d1a 0b00 000b 0000 0100 4e0c 5f13  ..}.........N._.
+00004970: 0055 0200 1305 6b02 2880 9c00 0002 0008  .U....k.(.......
+00004980: 0069 0700 560c 7924 0000 0600 0275 1a08  .i..V.y$.....u..
+00004990: 004b 145f 1300 5102 0013 046b 0428 808a  .K._..Q....k.(..
+000049a0: 0000 0200 0800 6907 0052 0a79 2400 0006  ......i..R.y$...
+000049b0: 0002 771a 0800 4a10 5f18 0048 0200 1300  ..w...J._..H....
+000049c0: 5002 0013 0048 0600 1300 5002 0013 0080  P....H....P.....
+000049d0: 8902 282b 0000 0200 0800 6907 0057 0279  ..(+......i..W.y
+000049e0: 2400 0006 0002 7f1a 0800 4808 5f13 0050  $.........H._..P
+000049f0: 0200 1300 4806 0013 0050 0200 1300 4806  ....H....P....H.
+00004a00: 0013 0050 0200 1308 1a06 0013 081a 1200  ...P............
+00004a10: 1308 1a12 0013 121a 1200 1308 1228 0013  .............(..
+00004a20: 007e 1600 6100 6706 0027 0066 0200 2100  .~..a.g..'.f..!.
+00004a30: 6002 0021 003a 062a 3600 0002 0008 0069  `..!.:.*6......i
+00004a40: 0900 4102 7712 0002 7f1c 0b00 000b 0000  ..A.w...........
+00004a50: 0100 4008 5d0d 0043 0200 1804 80ca 0200  ..@.]..C........
+00004a60: 1310 120e 0021 006f 2200 2707 1202 0021  .....!.o".'....!
+00004a70: 2712 1000 2707 1250 0021 0068 1000 2108  '...'..P.!.h..!.
+00004a80: 1202 0021 002a 1600 0700 5202 001c 2d12  ...!.*....R...-.
+00004a90: 0200 0d00 215c 0012 007b 0200 3800 2a04  ....!\...{..8.*.
+00004aa0: 0007 0052 0200 1c26 1202 000d 0021 4e00  ...R...&.....!N.
+00004ab0: 1200 7a02 0038 0038 0400 1800 8081 0200  ..z..8.8........
+00004ac0: 1300 2e02 0013 0038 0200 1300 3804 0018  .......8....8...
+00004ad0: 002e 0200 1300 7502 0013 0072 0200 130d  ......u....r....
+00004ae0: 1a02 0013 0077 2000 6104 6002 0013 0047  .....w .a.`....G
+00004af0: 1000 1800 3502 0013 007c 0200 1300 6c04  ....5....|....l.
+00004b00: 2a2b 0000 0200 0800 6907 003f 0277 2400  *+......i..?.w$.
+00004b10: 0006 0002 7f1c 0800 4008 5d25 0044 0200  ........@.]%.D..
+00004b20: 2500 8080 0600 4b00 809d 0200 3d00 1806  %.....K.....=...
+00004b30: 4a0d 0000 0500 1800 491a 000d 0477 0200  J.......I....w..
+00004b40: 0080 8e00 5906 1040 0180 ec02 0080 8600  ....Y..@........
+00004b50: 0604 0005 005d 0400 4000 0602 0005 005f  .....]..@......_
+00004b60: 0400 4000 0602 0005 0059 0400 4000 0602  ..@......Y..@...
+00004b70: 0005 0000 0400 231a 0e1c 0048 0273 1300  ......#....H.s..
+00004b80: 0602 0005 005d 0600 4000 0602 0005 0065  .....]..@......e
+00004b90: 0400 4000 0602 0005 0067 0400 4000 0602  ..@......g..@...
+00004ba0: 0005 0063 0400 4000 0602 0005 005f 0400  ...c..@......_..
+00004bb0: 4000 0602 0005 005d 0400 4000 0602 0005  @......]..@.....
+00004bc0: 0065 0400 4000 0602 0005 006b 0400 4000  .e..@......k..@.
+00004bd0: 0602 0005 0069 0400 4000 0602 0005 0061  .....i..@......a
+00004be0: 0400 4000 0602 0005 005d 0a00 4000 0602  ..@......]..@...
+00004bf0: 0005 005d 0400 4000 0602 0005 005d 0400  ...]..@......]..
+00004c00: 4000 0602 0005 005d 0400 4000 0602 0005  @......]..@.....
+00004c10: 005d 0400 4000 0602 0002 005d 0400 4000  .]..@......]..@.
+00004c20: 0602 0002 0028 0800 0600 02bf 512c 0e00  .....(......Q,..
+00004c30: 000e 0071 80ba 3d1c 0060 0208 1300 7402  ...q..=..`....t.
+00004c40: 791c 0062 0208 1300 6a02 791c 005c 0208  y..b....j.y..\..
+00004c50: 1300 8080 0679 3d00 7a02 003d 0812 0600  .....y=.z..=....
+00004c60: 2700 6212 0027 0181 7208 0027 0e12 0a00  '.b..'..r..'....
+00004c70: 1300 511e 0027 0051 0200 2700 3206 0018  ..Q..'.Q..'.2...
+00004c80: 000c 022a 1200 0002 0008 0069 0700 5204  ...*.......i..R.
+00004c90: 2030 0000 0200 0800 6907 001f 0477 0700   0......i....w..
+00004ca0: 027d 1c0b 0000 0b00 0001 0002 7d79 0b00  .}..........}y..
+00004cb0: 000b 0000 0100 1310 5d09 0019 0600 0700  ........].......
+00004cc0: 1402 460d 0000 0500 1600 4d1c 0013 0477  ..F.......M....w
+00004cd0: 0300 0c02 2a12 0000 0500 0800 6909 0010  ....*.......i...
+00004ce0: 042c 0e00 0005 000e 005d 0900 2004 770e  .,.......].. .w.
+00004cf0: 0042 0400 1d00 5502 0838 000d 0479 0300  .B....U..8...y..
+00004d00: 2402 000c 0073 0408 6e00 1602 0012 001f  $....s..n.......
+00004d10: 0200 091c 0406 7979 0017 0436 0c00 3b02  ......yy...6..;.
+00004d20: 0239 003b 020a 3900 3b02 7339 002d 0202  .9.;..9.;.s9.-..
+00004d30: 0c00 2d02 000c 002d 027d 0c00 2d02 040c  ..-....-.}..-...
+00004d40: 002d 0200 0c00 2d02 7b0c 002d 0202 0c00  .-....-.{..-....
+00004d50: 2d02 040c 002d 027f 0c00 2d02 0e0c 002d  -....-....-....-
+00004d60: 027d 0c00 2d02 040c 002d 0200 0c00 2d02  .}..-....-....-.
+00004d70: 7d0c 002d 0200 0c00 2d02 0209 002d 027d  }..-....-....-.}
+00004d80: 0900 2d02 0609 002d 0273 0900 2d02 0009  ..-....-.s..-...
+00004d90: 002d 0200 0900 5d02 5f52 0000 0400 3306  .-....]._R....3.
+00004da0: 6f0f 0011 0200 0600 0602 0002 0002 2328  o.............#(
+00004db0: 0e00 000b 0000 0100 0a64 5104 0006 0016  .........dQ.....
+00004dc0: 0200 0219 060e 0000 0b00 0001 000b 6e5d  ..............n]
+00004dd0: 0400 4302 0838 0002 0b30 0e00 000e 0018  ..C..8...0......
+00004de0: 8080 240d 0000 0500 2500 2f1c 0035 0477  ..$.....%./..5.w
+00004df0: 1500 4302 0024 001c 0200 0900 6a02 0857  ..C..$......j..W
+00004e00: 0039 0479 2501 8088 0200 808e 003c 0800  .9.y%........<..
+00004e10: 253f 0402 0080 a300 2204 360c 001f 020c  %?......".6.....
+00004e20: 0c01 8100 027f 0c00 2404 0c0c 0181 0a02  ........$.......
+00004e30: 7f0c 0021 0473 0c01 80ec 0200 0c00 0004  ...!.s..........
+00004e40: 0023 0459 1c00 4500 4e0c 0062 024b 0c00  .#.Y..E.N..b.K..
+00004e50: 5502 060c 006c 0204 0c00 6902 000c 0080  U....l....i.....
+00004e60: 8502 020c 106b 0275 0c00 7f22 0809 0059  .....k.u..."...Y
+00004e70: 0206 0900 4d02 7509 1067 0202 0900 6122  ....M.u..g....a"
+00004e80: 7f09 004b 027b 0900 4b02 0209 004b 0204  ...K.{..K....K..
+00004e90: 0900 4b02 0009 004f 0206 0900 1402 7d09  ..K....O......}.
+00004ea0: 0049 0263 2200 0004 0034 046f 0a00 02bf  .I.c"....4.o....
+00004eb0: 6756 0e00 000e 077b 80a2 2371 077b 1200  gV.....{..#q.{..
+00004ec0: 7107 7b12 0071 0056 1600 2c01 8120 0208  q.{..q.V..,.. ..
+00004ed0: 7600 5b06 792c 0181 2c02 0876 0054 0679  v.[.y,..,..v.T.y
+00004ee0: 2c01 8118 0208 7607 120a 7980 9b00 4616  ,.....v...y...F.
+00004ef0: 000e 0044 0200 0d00 4902 000d 0058 0200  ...D....I....X..
+00004f00: 0e13 1202 0080 a200 262c 000d 005e 0208  ........&,...^..
+00004f10: 1300 4d02 2236 0000 0200 0800 6909 0043  ..M."6......i..C
+00004f20: 0277 0d00 027f 1c0b 0000 0b00 0001 000c  .w..............
+00004f30: 061a 1200 0002 0012 0055 0700 6004 4632  .........U..`.F2
+00004f40: 0000 0200 1b00 4309 016c 0277 1800 027f  ......C..l.w....
+00004f50: 420b 0000 0b00 0001 0002 7d67 0b00 000b  B.........}g....
+00004f60: 0000 0101 500c 4927 0027 0c00 0d00 6002  ....P.I'.'....`.
+00004f70: 0813 0080 ca04 2a43 0000 0200 0c00 6107  ......*C......a.
+00004f80: 0077 0277 1e00 0006 0002 7f24 0800 0a06  .w.w.......$....
+00004f90: 5f04 0000 0200 7f02 7f4e 0003 7f2c 0600  _........N...,..
+00004fa0: 0700 6f06 0028 085f 0d00 5102 0813 0138  ..o..(._..Q....8
+00004fb0: 0279 2700 2a08 000d 0067 0208 1329 1206  .y'.*....g...)..
+00004fc0: 7927 0068 5836 4600 0002 000e 005d 0900  y'.hX6F......]..
+00004fd0: 1706 770b 0312 0208 1800 170c 790b 005f  ..w.........y.._
+00004fe0: 0208 1200 026b 200b 0000 0b00 0001 0068  .....k ........h
+00004ff0: 1e06 4600 0002 000e 005d 0900 2d04 7716  ..F......]..-.w.
+00005000: 0142 0208 1800 027b 200b 0000 0b00 0001  .B.....{ .......
+00005010: 0067 1006 4600 0002 000e 005d 0901 4204  .g..F......]..B.
+00005020: 7718 0002 7d28 0b00 000b 0000 0100 670e  w...}(........g.
+00005030: 0646 0000 0200 0e00 5d09 002e 0477 1601  .F......]....w..
+00005040: 4202 0818 0002 7b20 0b00 000b 0000 0100  B.....{ ........
+00005050: 6c0e 0646 0000 0200 0e00 5d09 0017 0677  l..F......]....w
+00005060: 0b04 1202 0818 0018 0e79 0e00 5f02 0812  .........y.._...
+00005070: 0002 6920 0b00 000b 0000 0100 4c22 081b  ..i ........L"..
+00005080: 0000 0200 0f00 5b07 0080 8702 7724 0000  ......[.....w$..
+00005090: 0600 027f 2a08 0124 084f 2701 2404 0027  ....*..$.O'.$..'
+000050a0: 0080 9f08 0021 0029 0600 0d00 6402 0813  .....!.)....d...
+000050b0: 000c 0236 1200 0005 0012 0055 0900 1004  ...6.......U....
+000050c0: 1c0e 0000 0500 0600 6d09 005a 0677 3100  ........m..Z.w1.
+000050d0: 1c04 000c 0080 8804 0867 0016 0200 1200  .........g......
+000050e0: 1702 0009 0052 0479 1200 026b 180e 0000  .....R.y...k....
+000050f0: 0b00 0001 0002 7d10 0e00 000b 0000 0100  ......}.........
+00005100: 5d26 4927 005f 0200 2700 2b06 000d 005d  ]&I'._..'.+....]
+00005110: 0208 1314 1202 7927 071a 2c00 2700 80af  ......y'..,.'...
+00005120: 1200 2700 80af 0200 2700 2608 000d 005a  ..'.....'.&....Z
+00005130: 0208 1301 80ce 0279 2100 2508 000d 005c  .......y!.%....\
+00005140: 0408 1300 6108 7921 004d 0400 0d0b 1204  ....a.y!.M......
+00005150: 0021 004f 1a00 0d00 4f04 000d 004f 0400  .!.O....O....O..
+00005160: 0d19 1204 0021 0053 3600 0d00 813b 0400  .....!.S6....;..
+00005170: 2100 8138 0400 2100 5d04 0021 0016 1452  !..8..!.]..!...R
+00005180: 0d00 0002 001c 0041 1a00 2004 7707 0028  .......A.. .w..(
+00005190: 0200 0900 2f04 0015 0046 0200 1e00 0275  ..../....F.....u
+000051a0: 440b 0000 0e00 8090 1435 5706 1206 0080  D........5W.....
+000051b0: b400 691a 0027 0080 a804 0027 0080 ae04  ..i..'.....'....
+000051c0: 0038 0080 8f04 0027 005f 0a00 2700 5f02  .8.....'._..'._.
+000051d0: 0027 1412 0400 2106 122c 0027 0712 1000  .'....!..,.'....
+000051e0: 2704 1212 0027 0612 0c00 271d 120e 0027  '....'....'....'
+000051f0: 1712 3e00 85f4 005c 3600 3b00 6f02 0021  ..>....\6.;.o..!
+00005200: 005c 0400 3e00 6f02 0021 005c 0400 3b00  .\..>.o..!.\..;.
+00005210: 6f02 0021 005c 0400 3e00 6f02 0021 005b  o..!.\..>.o..!.[
+00005220: 0400 3b00 6e02 0021 005c 0400 3e00 6f02  ..;.n..!.\..>.o.
+00005230: 0021 005c 0400 3e00 6f02 0021 0038 0a0e  .!.\..>.o..!.8..
+00005240: 0d00 3104 7b28 0001 0279 0200 000b 0000  ..1.{(...y......
+00005250: 0100 0102 7905 0980 1a06 0005 0981 1a06  ....y...........
+00005260: 0005 0982 1a06 0005 0800 0400 0006 0000  ................
+00005270: 0035 1505 2f03 0000 0014 004a 8221 0d20  .5../......J.!. 
+00005280: 0080 8702 0012 0022 0400 0600 2902 000c  ......."....)...
+00005290: 003b 0200 1b00 0102 7902 0000 0900 0001  .;......y.......
+000052a0: 0001 0000 1500 0000 5f18 050b 0059 0800  ........_....Y..
+000052b0: 0b00 5108 000b 004f 1000 2553 7973 7465  ..Q....O..%Syste
+000052c0: 6d2e 436f 6d70 6f6e 656e 744d 6f64 656c  m.ComponentModel
+000052d0: 2e44 6174 6141 6e6e 6f74 6174 696f 6e73  .DataAnnotations
+000052e0: 1c53 7973 7465 6d2e 5275 6e74 696d 652e  .System.Runtime.
+000052f0: 5365 7269 616c 697a 6174 696f 6e1e 5379  Serialization.Sy
+00005300: 7374 656d 2e54 6578 742e 4a73 6f6e 2e53  stem.Text.Json.S
+00005310: 6572 6961 6c69 7a61 7469 6f6e 2a01 a795  erialization*...
+00005320: 01a7 aa01 a7cc 01a7 ec01 a7f3 01a8 0e01  ................
+00005330: a818 01a8 2401 a834 01a8 4501 bee6 01bf  ....$..4..E.....
+00005340: 0c01 a883 01bf 2916 0000 001d 80c5 050b  ......).........
+00005350: 0024 0800 0b00 2808 000b 0026 0800 0700  .$....(....&....
+00005360: 0000 2481 9905 0c00 0000 2681 a305 0b00  ..$.......&.....
+00005370: 3208 0007 0000 001f 81ae 0507 0000 0018  2...............
+00005380: 833c 3207 0000 0018 8343 2e07 0000 0018  .<2......C......
+00005390: 8349 2e07 0000 0018 834f 2e07 0000 0018  .I.......O......
+000053a0: 8476 3107 0000 0018 8486 4907 0000 0017  .v1.......I.....
+000053b0: 8487 4907 0000 0017 8488 3307 0000 0018  ..I.......3.....
+000053c0: 84a2 5107 0000 0018 84a3 5107 0000 0018  ..Q.......Q.....
+000053d0: 84a4 5107 0000 0018 84a5 5107 0000 0154  ..Q.......Q....T
+000053e0: 8608 3f08 0000 0181 0a86 1534 0700 0002  ..?........4....
+000053f0: 6686 2334 0800 0001 80a6 862b 3407 0000  f.#4.......+4...
+00005400: 0021 86a1 3607 0000 0034 8826 3f07 0000  .!..6....4.&?...
+00005410: 002f 88c7 4907 0000 0034 88d0 4a07 0000  ./..I....4..J...
+00005420: 002d 88d9 4707 0000 002e 88de 2f07 0000  .-..G......./...
+00005430: 002e 88e0 5a07 0000 0033 88e2 2f07 0000  ....Z....3../...
+00005440: 0033 88e4 5b07 0000 002c 88e6 2f07 0000  .3..[....,../...
+00005450: 002c 88e8 5807 0000 0035 8913 3507 0000  .,..X....5..5...
+00005460: 0030 8962 5b07 0000 0030 8971 5b07 0000  .0.b[....0.q[...
+00005470: 002f 8979 5b07 0000 002f 8980 5b07 0000  ./.y[..../..[...
+00005480: 0034 8987 5b06 0000 0034 380d 1f04 0000  .4..[....48.....
+00005490: 3c3d 0d0e 0037 0200 0d00 6a02 0855 003c  <=...7....j..U.<
+000054a0: 0279 0900 2202 000d 0001 0279 1505 0000  .y.."......y....
+000054b0: 3c46 0d0e 002b 0200 0d00 2202 000d 0001  <F...+....".....
+000054c0: 0279 1505 0000 3c4d 0d0e 002a 0200 0d00  .y....<M...*....
+000054d0: 2202 000d 0001 0279 0b00 0000 2454 0d0d  "......y....$T..
+000054e0: 0001 0279 0b06 0000 2559 0d35 0b04 0200  ...y....%Y.5....
+000054f0: 0b06 0000 246a 0d35 0904 0200 80a8 0700  ....$j.5........
+00005500: 0021 8083 2709 0000 0200 0d00 5f04 001d  .!..'......._...
+00005510: 0477 0700 0004 0002 7d26 0600 1b0a 0409  .w......}&......
+00005520: 0000 0500 0c00 6104 0000 0700 2204 770d  ......a.....".w.
+00005530: 0041 0200 1d00 2f02 001d 000e 0408 0700  .A..../.........
+00005540: 2002 0013 0027 0200 1400 2104 0013 0080   ....'....!.....
+00005550: 8302 084f 0030 0671 1a00 6d02 083b 0017  ...O.0.q..m..;..
+00005560: 0479 0d00 1702 000d 004e 0200 1800 2e02  .y.......N......
+00005570: 0007 0022 0200 0f00 2202 000f 005c 0200  ..."...."....\..
+00005580: 2c00 6002 002c 0025 0200 0d00 2602 0012  ,.`..,.%....&...
+00005590: 001e 0200 1b00 6602 0023 0000 0400 0249  ......f..#.....I
+000055a0: 2409 0001 3c4d 0700 0000 4285 fc52 0700  $...<M....B..R..
+000055b0: 0000 4289 1852 0700 0000 3180 9b2c 0700  ..B..R....1..,..
+000055c0: 0000 6a80 b326 0700 0000 4a80 b625 0700  ..j..&....J..%..
+000055d0: 0000 6e80 bf27 0700 0000 4d80 c226 0700  ..n..'....M..&..
+000055e0: 0000 6c82 2226 0000                      ..l."&..
```

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.7/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-0.0.7/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorAnim_9.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorAnim_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorArachnus.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorArachnus.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorBlue.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorBlue.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorBomb.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPA3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorGenesis.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorGenesis.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorGuardian.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorGuardian.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorIceBeam.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorIceBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorLocked.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorLocked.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorMissile.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorPBomb.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorQueen.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorQueen.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorScrew.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorScrew.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSerris.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSerris.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSpider.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSpider.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorSuper.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorSuper.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTester.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTester.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTorizo.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTorizo.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/bg_MapBottom2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/bg_MapBottom2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newA4Doors.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newA4Doors.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/newA4Doors2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/newA4Doors2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUIMissile.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUIMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUIPBomb.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUIPBomb.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/sGUISMissile.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/sGUISMissile.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpHideout.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpHideout.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png` & `am2r_yams-0.0.7/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png`

 * *Files identical despite different names*

### Comparing `am2r_yams-0.0.5/am2r_yams.egg-info/PKG-INFO` & `am2r_yams-0.0.7/am2r_yams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: am2r-yams
-Version: 0.0.5
+Version: 0.0.7
 Summary: An open source randomizer patcher for AM2R.
 Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `am2r_yams-0.0.5/am2r_yams.egg-info/SOURCES.txt` & `am2r_yams-0.0.7/am2r_yams.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-am2r_yams/Patcher.py
 am2r_yams/__init__.py
+am2r_yams/wrapper.py
 am2r_yams.egg-info/PKG-INFO
 am2r_yams.egg-info/SOURCES.txt
 am2r_yams.egg-info/dependency_links.txt
 am2r_yams.egg-info/entry_points.txt
 am2r_yams.egg-info/not-zip-safe
 am2r_yams.egg-info/requires.txt
 am2r_yams.egg-info/top_level.txt
```

### Comparing `am2r_yams-0.0.5/setup.cfg` & `am2r_yams-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = am2r_yams
-version = 0.0.5
+version = 0.0.7
 description = An open source randomizer patcher for AM2R.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Miepee/YAMS
 author = Miepee
 license_files = 
 	LICENSE
```

