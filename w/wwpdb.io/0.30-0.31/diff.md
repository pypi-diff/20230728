# Comparing `tmp/wwpdb.io-0.30.tar.gz` & `tmp/wwpdb.io-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.io-0.30.tar", last modified: Wed Jun  7 15:01:23 2023, max compression
+gzip compressed data, was "wwpdb.io-0.31.tar", last modified: Fri Jul 28 10:42:58 2023, max compression
```

## Comparing `wwpdb.io-0.30.tar` & `wwpdb.io-0.31.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.168917 wwpdb.io-0.30/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-07 15:00:32.000000 wwpdb.io-0.30/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-06-07 15:01:23.168917 wwpdb.io-0.30/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-06-07 15:00:32.000000 wwpdb.io-0.30/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-07 15:01:23.168917 wwpdb.io-0.30/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2019 2023-06-07 15:00:32.000000 wwpdb.io-0.30/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb/io/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb/io/cvs/
--rw-r--r--   0 vsts      (1001) docker     (123)    30369 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/cvs/CvsAdmin.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8868 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/cvs/CvsUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/cvs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb/io/file/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    24712 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/DataExchange.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20256 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/DataFile.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)    19073 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/DataMaintenance.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19244 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5643 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/file/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb/io/graphics/
--rw-r--r--   0 vsts      (1001) docker     (123)    21126 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/graphics/GraphicsContext3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/graphics/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.168917 wwpdb.io-0.30/wwpdb/io/locator/
--rw-r--r--   0 vsts      (1001) docker     (123)     7798 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/ChemRefPathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46376 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/DataReference.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27907 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/PathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6396 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/ReleaseFileNames.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/ReleasePathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2669 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/locator/localFTPPathInfo.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.168917 wwpdb.io-0.30/wwpdb/io/misc/
--rw-r--r--   0 vsts      (1001) docker     (123)     3765 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/misc/FormatOut.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/misc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.168917 wwpdb.io-0.30/wwpdb/io/sftp/
--rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/sftp/ArchiveIoBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7319 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/sftp/ArchiveIoSftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-07 15:00:32.000000 wwpdb.io-0.30/wwpdb/io/sftp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-07 15:01:23.164917 wwpdb.io-0.30/wwpdb.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-06-07 15:01:23.000000 wwpdb.io-0.30/wwpdb.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      961 2023-06-07 15:01:23.000000 wwpdb.io-0.30/wwpdb.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-07 15:01:23.000000 wwpdb.io-0.30/wwpdb.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-07 15:01:08.000000 wwpdb.io-0.30/wwpdb.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-06-07 15:01:23.000000 wwpdb.io-0.30/wwpdb.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-07 15:01:23.000000 wwpdb.io-0.30/wwpdb.io.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.610606 wwpdb.io-0.31/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-28 10:42:00.000000 wwpdb.io-0.31/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-07-28 10:42:58.610606 wwpdb.io-0.31/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-28 10:42:00.000000 wwpdb.io-0.31/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-28 10:42:58.610606 wwpdb.io-0.31/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2019 2023-07-28 10:42:00.000000 wwpdb.io-0.31/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.602605 wwpdb.io-0.31/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.606605 wwpdb.io-0.31/wwpdb/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.606605 wwpdb.io-0.31/wwpdb/io/cvs/
+-rw-r--r--   0 vsts      (1001) docker     (123)    30369 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/cvs/CvsAdmin.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8868 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/cvs/CvsUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/cvs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.606605 wwpdb.io-0.31/wwpdb/io/file/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    24712 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/DataExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20256 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/DataFile.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    19073 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/DataMaintenance.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19244 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5643 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/file/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.606605 wwpdb.io-0.31/wwpdb/io/graphics/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21126 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/graphics/GraphicsContext3D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/graphics/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.610606 wwpdb.io-0.31/wwpdb/io/locator/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7798 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/ChemRefPathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46235 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/DataReference.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28453 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/PathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6396 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/ReleaseFileNames.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/ReleasePathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2669 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/locator/localFTPPathInfo.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.610606 wwpdb.io-0.31/wwpdb/io/misc/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3765 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/misc/FormatOut.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/misc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.610606 wwpdb.io-0.31/wwpdb/io/sftp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/sftp/ArchiveIoBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7319 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/sftp/ArchiveIoSftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:00.000000 wwpdb.io-0.31/wwpdb/io/sftp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:42:58.606605 wwpdb.io-0.31/wwpdb.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-07-28 10:42:58.000000 wwpdb.io-0.31/wwpdb.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      961 2023-07-28 10:42:58.000000 wwpdb.io-0.31/wwpdb.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 10:42:58.000000 wwpdb.io-0.31/wwpdb.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 10:42:41.000000 wwpdb.io-0.31/wwpdb.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-07-28 10:42:58.000000 wwpdb.io-0.31/wwpdb.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-28 10:42:58.000000 wwpdb.io-0.31/wwpdb.io.egg-info/top_level.txt
```

### Comparing `wwpdb.io-0.30/LICENSE` & `wwpdb.io-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/PKG-INFO` & `wwpdb.io-0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.30
+Version: 0.31
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.30/README.md` & `wwpdb.io-0.31/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/setup.py` & `wwpdb.io-0.31/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/cvs/CvsAdmin.py` & `wwpdb.io-0.31/wwpdb/io/cvs/CvsAdmin.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/cvs/CvsUtility.py` & `wwpdb.io-0.31/wwpdb/io/cvs/CvsUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/file/DataExchange.py` & `wwpdb.io-0.31/wwpdb/io/file/DataExchange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/file/DataFile.py` & `wwpdb.io-0.31/wwpdb/io/file/DataFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/file/DataMaintenance.py` & `wwpdb.io-0.31/wwpdb/io/file/DataMaintenance.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/file/ValidateXml.py` & `wwpdb.io-0.31/wwpdb/io/file/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/file/mmCIFUtil.py` & `wwpdb.io-0.31/wwpdb/io/file/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/graphics/GraphicsContext3D.py` & `wwpdb.io-0.31/wwpdb/io/graphics/GraphicsContext3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/ChemRefPathInfo.py` & `wwpdb.io-0.31/wwpdb/io/locator/ChemRefPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/DataReference.py` & `wwpdb.io-0.31/wwpdb/io/locator/DataReference.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,19 +212,15 @@
         return False
 
     def getVersionId(self):
         """Return version identifier (integer), current symbolic setting, or None"""
         return self.__versionId
 
     def getDepositionDataSetId(self):
-        """Return the data set identier -  (uppoer case)"""
-        return self.__depositionDataSetId
-
-    def getDepositonDataSetId(self):
-        """Return the data set identier -  (uppoer case)"""
+        """Return the data set identier -  (upper case)"""
         return self.__depositionDataSetId
 
     def getPartitionNumber(self):
         """Return the file partition number (integer)  or symbolic setting."""
         return self.__filePartNumber
 
     def getContentTypeAcronym(self):
```

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/PathInfo.py` & `wwpdb.io-0.31/wwpdb/io/locator/PathInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # 23-Aug-2014   jdw   add method getEmDepositVolumeParamsFilePath()
 # 14-Sep-2014   jdw   add isValidFileName(fileName, requireVersion=True) and splitFileName(fileName)
 # 24-Sep-2014   jdw   add getFileExtension(formatType)
 # 13-Dec-2016   jdw   add getStructureFactorsPdbxFilePath()
 # 23-Oct-2017   jdw   config for logging - add parseFileName wrapper method
 # 24-Mar-2018   ep    add mileStone argument to getFilePathContentTypeTemplate()
 # 06-Jun-2023   dh    add getNMRCombinedFilePath
+# 15-Jun-2023   dh    add getMolecularRestraintsFilePath
 ##
 """
 Common methods for finding path information for resource and data files in the wwPDB data processing
 and annotation system.
 
 """
 __docformat__ = "restructuredtext en"
@@ -357,14 +358,26 @@
             versionId=versionId,
             partNumber="1",
             contentTypeBase="nmr-chemical-shifts",
             formatType=formatType,
             mileStone=mileStone,
         )
 
+    def getMolecularRestraintsFilePath(self, dataSetId, formatType="nmr-star", wfInstanceId=None, fileSource="archive", versionId="latest", mileStone=None):
+        return self.__getStandardPath(
+            dataSetId=dataSetId,
+            wfInstanceId=wfInstanceId,
+            fileSource=fileSource,
+            versionId=versionId,
+            partNumber="1",
+            contentTypeBase="nmr-restraints",
+            formatType=formatType,
+            mileStone=mileStone,
+        )
+
     def getNMRCombinedFilePath(self, dataSetId, formatType="nmr-star", wfInstanceId=None, fileSource="archive", versionId="latest", mileStone=None):
         return self.__getStandardPath(
             dataSetId=dataSetId,
             wfInstanceId=wfInstanceId,
             fileSource=fileSource,
             versionId=versionId,
             partNumber="1",
```

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/ReleaseFileNames.py` & `wwpdb.io-0.31/wwpdb/io/locator/ReleaseFileNames.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/ReleasePathInfo.py` & `wwpdb.io-0.31/wwpdb/io/locator/ReleasePathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/locator/localFTPPathInfo.py` & `wwpdb.io-0.31/wwpdb/io/locator/localFTPPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/misc/FormatOut.py` & `wwpdb.io-0.31/wwpdb/io/misc/FormatOut.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/sftp/ArchiveIoBase.py` & `wwpdb.io-0.31/wwpdb/io/sftp/ArchiveIoBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb/io/sftp/ArchiveIoSftp.py` & `wwpdb.io-0.31/wwpdb/io/sftp/ArchiveIoSftp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.30/wwpdb.io.egg-info/PKG-INFO` & `wwpdb.io-0.31/wwpdb.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.30
+Version: 0.31
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.30/wwpdb.io.egg-info/SOURCES.txt` & `wwpdb.io-0.31/wwpdb.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

