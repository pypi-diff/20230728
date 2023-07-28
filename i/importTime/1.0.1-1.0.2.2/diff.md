# Comparing `tmp/importTime-1.0.1-py2.py3-none-any.whl.zip` & `tmp/importTime-1.0.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6340 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 23:28 importTime/__init__.py
--rw-r--r--  2.0 unx     1445 b- defN 23-Jul-27 23:28 importTime/importTime.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      866 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/RECORD
-7 files, 14352 bytes uncompressed, 5338 bytes compressed:  62.8%
+Zip file size: 6812 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 00:04 importTime/__init__.py
+-rw-r--r--  2.0 unx     2480 b- defN 23-Jul-28 00:04 importTime/importTime.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1602 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      574 b- defN 23-Jul-28 00:04 importTime-1.0.2.2.dist-info/RECORD
+7 files, 16134 bytes uncompressed, 5790 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: importTime/__init__.py
 Comment: 
 
 Filename: importTime/importTime.py
 Comment: 
 
-Filename: importTime-1.0.1.dist-info/LICENSE.txt
+Filename: importTime-1.0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: importTime-1.0.1.dist-info/METADATA
+Filename: importTime-1.0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: importTime-1.0.1.dist-info/WHEEL
+Filename: importTime-1.0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: importTime-1.0.1.dist-info/top_level.txt
+Filename: importTime-1.0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: importTime-1.0.1.dist-info/RECORD
+Filename: importTime-1.0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## importTime/importTime.py

```diff
@@ -1,13 +1,12 @@
 import time
 import json
 
 startTime = time.time()
 startImportTime = time.time()
-endTime = time.time()
 outData = []
 
 def startImport():
     """
     Call this function at the start of the import to start the timer.
     
     Returns:
@@ -29,14 +28,42 @@
     
     """
     global endImportTime
     global outData
     outData.append({"description":description, "time": time.time() - startImportTime})
     print("Time to Import {0}: {1}".format(description,  time.time() - startImportTime))
 
+
+def startTotal():
+    """
+    Call this function at the when you want to start the total timer.
+    
+    Returns:
+        None
+    
+    """
+    global startTime
+    startTime = time.time()
+    
+def endTotal():
+    """
+    Call this function at the end of the import to end the timer and print the time.
+    
+    Args:
+        description (str): Description or name of the import.
+    
+    Returns:
+        None
+    
+    """
+    global endImportTime
+    global outData
+    outData.append({"description":"total", "time": time.time() - startTime})
+    print("Total time to Import: {0}".format( time.time() - startTime))
+
 def saveCSV(filepath):
     """
     Save the data to a CSV file.
     
     Args:
         filepath (str): Path to the CSV file.
     
@@ -58,7 +85,25 @@
     Returns:
         None
     """
     global outData
     open(filepath, 'w').write(json.dumps(outData, indent=4))
             
 
+def debugImportTimes(modules = [], description = "modules"):
+    """
+    Debug the import times of the modules.
+    
+    Args:
+        modules (list[str]): List of modules to import.
+    
+    Returns:
+        None
+        
+    """
+    outText = "import "
+    for module in modules:
+        outText += "{0} ".format(module)
+        
+    startImport()
+    exec(outText)
+    endImport(description)
```

## Comparing `importTime-1.0.1.dist-info/LICENSE.txt` & `importTime-1.0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `importTime-1.0.1.dist-info/RECORD` & `importTime-1.0.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 importTime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-importTime/importTime.py,sha256=qOChsvs7lVIRBwAkzInMJme5CFV4g0wnXokLK31TPEw,1445
-importTime-1.0.1.dist-info/LICENSE.txt,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-importTime-1.0.1.dist-info/METADATA,sha256=AQaymZ_6vBxX393Qpz2zdOFJfoUpUogn1NQn3Q8POro,866
-importTime-1.0.1.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
-importTime-1.0.1.dist-info/top_level.txt,sha256=JH9k6SWVkd-fOX-HVOobga6KlggF4tyK-jb9ceOpe1M,11
-importTime-1.0.1.dist-info/RECORD,,
+importTime/importTime.py,sha256=Cr04uimC15a2lrrAOKmCmoUYhbJ5QeNYWM22gTpVAL0,2480
+importTime-1.0.2.2.dist-info/LICENSE.txt,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+importTime-1.0.2.2.dist-info/METADATA,sha256=jxt5sGqXe1AwnES7yOFMo5Z8vSEzGqlWzFzAU8FZP1o,1602
+importTime-1.0.2.2.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
+importTime-1.0.2.2.dist-info/top_level.txt,sha256=JH9k6SWVkd-fOX-HVOobga6KlggF4tyK-jb9ceOpe1M,11
+importTime-1.0.2.2.dist-info/RECORD,,
```

