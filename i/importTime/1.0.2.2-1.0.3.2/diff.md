# Comparing `tmp/importTime-1.0.2.2-py2.py3-none-any.whl.zip` & `tmp/importTime-1.0.3.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 6812 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 00:04 importTime/__init__.py
--rw-r--r--  2.0 unx     2480 b- defN 23-Jul-28 00:04 importTime/importTime.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1602 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      574 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/RECORD
-7 files, 16134 bytes uncompressed, 5790 bytes compressed:  64.1%
+Zip file size: 6640 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2480 b- defN 23-Jul-28 00:25 importTime/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-28 00:25 importTime-1.0.3.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1580 b- defN 23-Jul-28 00:25 importTime-1.0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-28 00:25 importTime-1.0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-28 00:25 importTime-1.0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      496 b- defN 23-Jul-28 00:25 importTime-1.0.3.2.dist-info/RECORD
+6 files, 16034 bytes uncompressed, 5742 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: importTime/__init__.py
 Comment: 
 
-Filename: importTime/importTime.py
+Filename: importTime-1.0.3.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: importTime-1.0.2.2.dist-info/LICENSE.txt
+Filename: importTime-1.0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: importTime-1.0.2.2.dist-info/METADATA
+Filename: importTime-1.0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: importTime-1.0.2.2.dist-info/WHEEL
+Filename: importTime-1.0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: importTime-1.0.2.2.dist-info/top_level.txt
-Comment: 
-
-Filename: importTime-1.0.2.2.dist-info/RECORD
+Filename: importTime-1.0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## importTime/__init__.py

```diff
@@ -0,0 +1,155 @@
+00000000: 696d 706f 7274 2074 696d 650d 0a69 6d70  import time..imp
+00000010: 6f72 7420 6a73 6f6e 0d0a 0d0a 7374 6172  ort json....star
+00000020: 7454 696d 6520 3d20 7469 6d65 2e74 696d  tTime = time.tim
+00000030: 6528 290d 0a73 7461 7274 496d 706f 7274  e()..startImport
+00000040: 5469 6d65 203d 2074 696d 652e 7469 6d65  Time = time.time
+00000050: 2829 0d0a 6f75 7444 6174 6120 3d20 5b5d  ()..outData = []
+00000060: 0d0a 0d0a 6465 6620 7374 6172 7449 6d70  ....def startImp
+00000070: 6f72 7428 293a 0d0a 2020 2020 2222 220d  ort():..    """.
+00000080: 0a20 2020 2043 616c 6c20 7468 6973 2066  .    Call this f
+00000090: 756e 6374 696f 6e20 6174 2074 6865 2073  unction at the s
+000000a0: 7461 7274 206f 6620 7468 6520 696d 706f  tart of the impo
+000000b0: 7274 2074 6f20 7374 6172 7420 7468 6520  rt to start the 
+000000c0: 7469 6d65 722e 0d0a 2020 2020 0d0a 2020  timer...    ..  
+000000d0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+000000e0: 2020 2020 4e6f 6e65 0d0a 2020 2020 0d0a      None..    ..
+000000f0: 2020 2020 2222 220d 0a20 2020 2067 6c6f      """..    glo
+00000100: 6261 6c20 7374 6172 7449 6d70 6f72 7454  bal startImportT
+00000110: 696d 650d 0a20 2020 2073 7461 7274 496d  ime..    startIm
+00000120: 706f 7274 5469 6d65 203d 2074 696d 652e  portTime = time.
+00000130: 7469 6d65 2829 0d0a 2020 2020 0d0a 6465  time()..    ..de
+00000140: 6620 656e 6449 6d70 6f72 7428 6465 7363  f endImport(desc
+00000150: 7269 7074 696f 6e29 3a0d 0a20 2020 2022  ription):..    "
+00000160: 2222 0d0a 2020 2020 4361 6c6c 2074 6869  ""..    Call thi
+00000170: 7320 6675 6e63 7469 6f6e 2061 7420 7468  s function at th
+00000180: 6520 656e 6420 6f66 2074 6865 2069 6d70  e end of the imp
+00000190: 6f72 7420 746f 2065 6e64 2074 6865 2074  ort to end the t
+000001a0: 696d 6572 2061 6e64 2070 7269 6e74 2074  imer and print t
+000001b0: 6865 2074 696d 652e 0d0a 2020 2020 0d0a  he time...    ..
+000001c0: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
+000001d0: 2020 2064 6573 6372 6970 7469 6f6e 2028     description (
+000001e0: 7374 7229 3a20 4465 7363 7269 7074 696f  str): Descriptio
+000001f0: 6e20 6f72 206e 616d 6520 6f66 2074 6865  n or name of the
+00000200: 2069 6d70 6f72 742e 0d0a 2020 2020 0d0a   import...    ..
+00000210: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00000220: 2020 2020 2020 4e6f 6e65 0d0a 2020 2020        None..    
+00000230: 0d0a 2020 2020 2222 220d 0a20 2020 2067  ..    """..    g
+00000240: 6c6f 6261 6c20 656e 6449 6d70 6f72 7454  lobal endImportT
+00000250: 696d 650d 0a20 2020 2067 6c6f 6261 6c20  ime..    global 
+00000260: 6f75 7444 6174 610d 0a20 2020 206f 7574  outData..    out
+00000270: 4461 7461 2e61 7070 656e 6428 7b22 6465  Data.append({"de
+00000280: 7363 7269 7074 696f 6e22 3a64 6573 6372  scription":descr
+00000290: 6970 7469 6f6e 2c20 2274 696d 6522 3a20  iption, "time": 
+000002a0: 7469 6d65 2e74 696d 6528 2920 2d20 7374  time.time() - st
+000002b0: 6172 7449 6d70 6f72 7454 696d 657d 290d  artImportTime}).
+000002c0: 0a20 2020 2070 7269 6e74 2822 5469 6d65  .    print("Time
+000002d0: 2074 6f20 496d 706f 7274 207b 307d 3a20   to Import {0}: 
+000002e0: 7b31 7d22 2e66 6f72 6d61 7428 6465 7363  {1}".format(desc
+000002f0: 7269 7074 696f 6e2c 2020 7469 6d65 2e74  ription,  time.t
+00000300: 696d 6528 2920 2d20 7374 6172 7449 6d70  ime() - startImp
+00000310: 6f72 7454 696d 6529 290d 0a0d 0a0d 0a64  ortTime))......d
+00000320: 6566 2073 7461 7274 546f 7461 6c28 293a  ef startTotal():
+00000330: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
+00000340: 616c 6c20 7468 6973 2066 756e 6374 696f  all this functio
+00000350: 6e20 6174 2074 6865 2077 6865 6e20 796f  n at the when yo
+00000360: 7520 7761 6e74 2074 6f20 7374 6172 7420  u want to start 
+00000370: 7468 6520 746f 7461 6c20 7469 6d65 722e  the total timer.
+00000380: 0d0a 2020 2020 0d0a 2020 2020 5265 7475  ..    ..    Retu
+00000390: 726e 733a 0d0a 2020 2020 2020 2020 4e6f  rns:..        No
+000003a0: 6e65 0d0a 2020 2020 0d0a 2020 2020 2222  ne..    ..    ""
+000003b0: 220d 0a20 2020 2067 6c6f 6261 6c20 7374  "..    global st
+000003c0: 6172 7454 696d 650d 0a20 2020 2073 7461  artTime..    sta
+000003d0: 7274 5469 6d65 203d 2074 696d 652e 7469  rtTime = time.ti
+000003e0: 6d65 2829 0d0a 2020 2020 0d0a 6465 6620  me()..    ..def 
+000003f0: 656e 6454 6f74 616c 2829 3a0d 0a20 2020  endTotal():..   
+00000400: 2022 2222 0d0a 2020 2020 4361 6c6c 2074   """..    Call t
+00000410: 6869 7320 6675 6e63 7469 6f6e 2061 7420  his function at 
+00000420: 7468 6520 656e 6420 6f66 2074 6865 2069  the end of the i
+00000430: 6d70 6f72 7420 746f 2065 6e64 2074 6865  mport to end the
+00000440: 2074 696d 6572 2061 6e64 2070 7269 6e74   timer and print
+00000450: 2074 6865 2074 696d 652e 0d0a 2020 2020   the time...    
+00000460: 0d0a 2020 2020 4172 6773 3a0d 0a20 2020  ..    Args:..   
+00000470: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00000480: 2028 7374 7229 3a20 4465 7363 7269 7074   (str): Descript
+00000490: 696f 6e20 6f72 206e 616d 6520 6f66 2074  ion or name of t
+000004a0: 6865 2069 6d70 6f72 742e 0d0a 2020 2020  he import...    
+000004b0: 0d0a 2020 2020 5265 7475 726e 733a 0d0a  ..    Returns:..
+000004c0: 2020 2020 2020 2020 4e6f 6e65 0d0a 2020          None..  
+000004d0: 2020 0d0a 2020 2020 2222 220d 0a20 2020    ..    """..   
+000004e0: 2067 6c6f 6261 6c20 656e 6449 6d70 6f72   global endImpor
+000004f0: 7454 696d 650d 0a20 2020 2067 6c6f 6261  tTime..    globa
+00000500: 6c20 6f75 7444 6174 610d 0a20 2020 206f  l outData..    o
+00000510: 7574 4461 7461 2e61 7070 656e 6428 7b22  utData.append({"
+00000520: 6465 7363 7269 7074 696f 6e22 3a22 746f  description":"to
+00000530: 7461 6c22 2c20 2274 696d 6522 3a20 7469  tal", "time": ti
+00000540: 6d65 2e74 696d 6528 2920 2d20 7374 6172  me.time() - star
+00000550: 7454 696d 657d 290d 0a20 2020 2070 7269  tTime})..    pri
+00000560: 6e74 2822 546f 7461 6c20 7469 6d65 2074  nt("Total time t
+00000570: 6f20 496d 706f 7274 3a20 7b30 7d22 2e66  o Import: {0}".f
+00000580: 6f72 6d61 7428 2074 696d 652e 7469 6d65  ormat( time.time
+00000590: 2829 202d 2073 7461 7274 5469 6d65 2929  () - startTime))
+000005a0: 0d0a 0d0a 6465 6620 7361 7665 4353 5628  ....def saveCSV(
+000005b0: 6669 6c65 7061 7468 293a 0d0a 2020 2020  filepath):..    
+000005c0: 2222 220d 0a20 2020 2053 6176 6520 7468  """..    Save th
+000005d0: 6520 6461 7461 2074 6f20 6120 4353 5620  e data to a CSV 
+000005e0: 6669 6c65 2e0d 0a20 2020 200d 0a20 2020  file...    ..   
+000005f0: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00000600: 6669 6c65 7061 7468 2028 7374 7229 3a20  filepath (str): 
+00000610: 5061 7468 2074 6f20 7468 6520 4353 5620  Path to the CSV 
+00000620: 6669 6c65 2e0d 0a20 2020 200d 0a20 2020  file...    ..   
+00000630: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00000640: 2020 204e 6f6e 650d 0a20 2020 2022 2222     None..    """
+00000650: 0d0a 2020 2020 676c 6f62 616c 206f 7574  ..    global out
+00000660: 4461 7461 0d0a 2020 2020 7769 7468 206f  Data..    with o
+00000670: 7065 6e28 6669 6c65 7061 7468 2c20 2777  pen(filepath, 'w
+00000680: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
+00000690: 2020 666f 7220 6974 656d 2069 6e20 6f75    for item in ou
+000006a0: 7444 6174 613a 0d0a 2020 2020 2020 2020  tData:..        
+000006b0: 2020 2020 662e 7772 6974 6528 227b 307d      f.write("{0}
+000006c0: 2c7b 317d 5c6e 222e 666f 726d 6174 2869  ,{1}\n".format(i
+000006d0: 7465 6d5b 2264 6573 6372 6970 7469 6f6e  tem["description
+000006e0: 225d 2c20 6974 656d 5b22 7469 6d65 225d  "], item["time"]
+000006f0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00000700: 0d0a 6465 6620 7361 7665 4a53 4f4e 2866  ..def saveJSON(f
+00000710: 696c 6570 6174 6829 3a0d 0a20 2020 2022  ilepath):..    "
+00000720: 2222 0d0a 2020 2020 5361 7665 2074 6865  ""..    Save the
+00000730: 2064 6174 6120 746f 2061 204a 534f 4e20   data to a JSON 
+00000740: 6669 6c65 2e0d 0a20 2020 200d 0a20 2020  file...    ..   
+00000750: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00000760: 6669 6c65 7061 7468 2028 7374 7229 3a20  filepath (str): 
+00000770: 5061 7468 2074 6f20 7468 6520 4a53 4f4e  Path to the JSON
+00000780: 2066 696c 652e 0d0a 2020 2020 0d0a 2020   file...    ..  
+00000790: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+000007a0: 2020 2020 4e6f 6e65 0d0a 2020 2020 2222      None..    ""
+000007b0: 220d 0a20 2020 2067 6c6f 6261 6c20 6f75  "..    global ou
+000007c0: 7444 6174 610d 0a20 2020 206f 7065 6e28  tData..    open(
+000007d0: 6669 6c65 7061 7468 2c20 2777 2729 2e77  filepath, 'w').w
+000007e0: 7269 7465 286a 736f 6e2e 6475 6d70 7328  rite(json.dumps(
+000007f0: 6f75 7444 6174 612c 2069 6e64 656e 743d  outData, indent=
+00000800: 3429 290d 0a20 2020 2020 2020 2020 2020  4))..           
+00000810: 200d 0a0d 0a64 6566 2064 6562 7567 496d   ....def debugIm
+00000820: 706f 7274 5469 6d65 7328 6d6f 6475 6c65  portTimes(module
+00000830: 7320 3d20 5b5d 2c20 6465 7363 7269 7074  s = [], descript
+00000840: 696f 6e20 3d20 226d 6f64 756c 6573 2229  ion = "modules")
+00000850: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00000860: 4465 6275 6720 7468 6520 696d 706f 7274  Debug the import
+00000870: 2074 696d 6573 206f 6620 7468 6520 6d6f   times of the mo
+00000880: 6475 6c65 732e 0d0a 2020 2020 0d0a 2020  dules...    ..  
+00000890: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+000008a0: 206d 6f64 756c 6573 2028 6c69 7374 5b73   modules (list[s
+000008b0: 7472 5d29 3a20 4c69 7374 206f 6620 6d6f  tr]): List of mo
+000008c0: 6475 6c65 7320 746f 2069 6d70 6f72 742e  dules to import.
+000008d0: 0d0a 2020 2020 0d0a 2020 2020 5265 7475  ..    ..    Retu
+000008e0: 726e 733a 0d0a 2020 2020 2020 2020 4e6f  rns:..        No
+000008f0: 6e65 0d0a 2020 2020 2020 2020 0d0a 2020  ne..        ..  
+00000900: 2020 2222 220d 0a20 2020 206f 7574 5465    """..    outTe
+00000910: 7874 203d 2022 696d 706f 7274 2022 0d0a  xt = "import "..
+00000920: 2020 2020 666f 7220 6d6f 6475 6c65 2069      for module i
+00000930: 6e20 6d6f 6475 6c65 733a 0d0a 2020 2020  n modules:..    
+00000940: 2020 2020 6f75 7454 6578 7420 2b3d 2022      outText += "
+00000950: 7b30 7d20 222e 666f 726d 6174 286d 6f64  {0} ".format(mod
+00000960: 756c 6529 0d0a 2020 2020 2020 2020 0d0a  ule)..        ..
+00000970: 2020 2020 7374 6172 7449 6d70 6f72 7428      startImport(
+00000980: 290d 0a20 2020 2065 7865 6328 6f75 7454  )..    exec(outT
+00000990: 6578 7429 0d0a 2020 2020 656e 6449 6d70  ext)..    endImp
+000009a0: 6f72 7428 6465 7363 7269 7074 696f 6e29  ort(description)
```

## Comparing `importTime-1.0.2.2.dist-info/LICENSE.txt` & `importTime-1.0.3.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `importTime-1.0.2.2.dist-info/METADATA` & `importTime-1.0.3.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importTime
-Version: 1.0.2.2
+Version: 1.0.3.2
 Summary: Debug import time or use this inside of a profiler.
 Home-page: https://github.com/vltmedia/importTime
 Author: Justin Jaro
 Author-email: info@VLTMedia.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,30 +16,30 @@
 
 ## Usage
 
 
 ### Debug Import Times
 This will print out the time it takes to import each module, but will not import them globally to your application. Please just use this function to debug times.
 ```python
-from importTime.importTime import debugImportTimes
+from importTime import debugImportTimes
 
 debugImportTimes(["numpy", "torch", "mediapipe", "PIL"], "MainDeps")
 ```
 
 ### Prints:
 ```python
 Time to Import  MainDeps: 0.08100032806396484
 ```
 
 ### Reveal Times
 Can be added to your currently running application. This will print out the time it takes to import between ```startImport()``` and ```endImport("moduleName")```. 
 ```python
 ```python
 
-from importTime.importTime import startImport , endImport, startTotal, endTotal, saveCSV
+from importTime import startImport , endImport, startTotal, endTotal, saveCSV
 
 
 startTotal()
 
 startImport()
 import numpy as np
 endImport("numpy")
```

