# Comparing `tmp/descriptastorus-2.6.0.tar.gz` & `tmp/descriptastorus-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descriptastorus-2.6.0.tar", last modified: Wed Oct 19 12:46:08 2022, max compression
+gzip compressed data, was "descriptastorus-2.6.1.tar", last modified: Fri Jul 28 15:28:05 2023, max compression
```

## Comparing `descriptastorus-2.6.0.tar` & `descriptastorus-2.6.1.tar`

### file list

```diff
@@ -1,41 +1,59 @@
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.865163 descriptastorus-2.6.0/
--rw-r--r--   0 bkelley    (501) staff       (20)     1597 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/LICENSE
--rw-r--r--   0 bkelley    (501) staff       (20)      261 2022-10-19 12:46:08.865029 descriptastorus-2.6.0/PKG-INFO
--rw-r--r--   0 bkelley    (501) staff       (20)     9196 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/README.md
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.854327 descriptastorus-2.6.0/descriptastorus/
--rw-r--r--   0 bkelley    (501) staff       (20)     8222 2022-10-13 10:16:35.000000 descriptastorus-2.6.0/descriptastorus/DescriptaStore.py
--rw-r--r--   0 bkelley    (501) staff       (20)    13124 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/MolFileIndex.py
--rw-r--r--   0 bkelley    (501) staff       (20)     1808 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus/__init__.py
--rw-r--r--   0 bkelley    (501) staff       (20)    12299 2022-10-13 12:15:20.000000 descriptastorus-2.6.0/descriptastorus/append_store.py
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.855439 descriptastorus-2.6.0/descriptastorus/cli/
--rw-r--r--   0 bkelley    (501) staff       (20)     1654 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/cli/__init__.py
--rw-r--r--   0 bkelley    (501) staff       (20)     4269 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/cli/storus.py
--rw-r--r--   0 bkelley    (501) staff       (20)     3531 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/cli/validate.py
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.864529 descriptastorus-2.6.0/descriptastorus/descriptors/
--rw-r--r--   0 bkelley    (501) staff       (20)    13404 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/descriptors/DescriptorGenerator-theirs.py
--rw-r--r--   0 bkelley    (501) staff       (20)    12617 2022-10-13 08:22:43.000000 descriptastorus-2.6.0/descriptastorus/descriptors/DescriptorGenerator.py
--rw-r--r--   0 bkelley    (501) staff       (20)    11099 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/descriptors/QED.py
--rw-r--r--   0 bkelley    (501) staff       (20)      118 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/descriptors/__init__.py
--rw-r--r--   0 bkelley    (501) staff       (20)    31293 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/descriptors/dists.py
--rw-r--r--   0 bkelley    (501) staff       (20)  3389239 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/descriptors/hists.py
--rw-r--r--   0 bkelley    (501) staff       (20)    18959 2022-10-13 12:19:07.000000 descriptastorus-2.6.0/descriptastorus/descriptors/rdDescriptors.py
--rw-r--r--   0 bkelley    (501) staff       (20)     4222 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/descriptors/rdNormalizedDescriptors.py
--rw-r--r--   0 bkelley    (501) staff       (20)     2817 2022-10-13 07:09:27.000000 descriptastorus-2.6.0/descriptastorus/descriptors/rdkit_fixes.py
--rw-r--r--   0 bkelley    (501) staff       (20)     1441 2022-10-13 12:15:04.000000 descriptastorus-2.6.0/descriptastorus/keyvalue.py
--rw-r--r--   0 bkelley    (501) staff       (20)    12886 2022-10-13 12:14:42.000000 descriptastorus-2.6.0/descriptastorus/make_store.py
--rw-r--r--   0 bkelley    (501) staff       (20)      107 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/mode.py
--rw-r--r--   0 bkelley    (501) staff       (20)    18447 2022-10-13 09:42:38.000000 descriptastorus-2.6.0/descriptastorus/raw.py
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.864861 descriptastorus-2.6.0/descriptastorus/stores/
--rw-r--r--   0 bkelley    (501) staff       (20)       48 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/stores/__init__.py
--rw-r--r--   0 bkelley    (501) staff       (20)     1131 2022-10-13 09:57:20.000000 descriptastorus-2.6.0/descriptastorus/stores/dbmstore.py
--rw-r--r--   0 bkelley    (501) staff       (20)     1312 2022-10-13 09:55:30.000000 descriptastorus-2.6.0/descriptastorus/stores/kyotostore.py
--rw-r--r--   0 bkelley    (501) staff       (20)      651 2022-10-13 07:06:06.000000 descriptastorus-2.6.0/descriptastorus/utils.py
-drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2022-10-19 12:46:08.855005 descriptastorus-2.6.0/descriptastorus.egg-info/
--rw-r--r--   0 bkelley    (501) staff       (20)      261 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/PKG-INFO
--rw-r--r--   0 bkelley    (501) staff       (20)     1120 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/SOURCES.txt
--rw-r--r--   0 bkelley    (501) staff       (20)        1 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/dependency_links.txt
--rw-r--r--   0 bkelley    (501) staff       (20)      111 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/entry_points.txt
--rw-r--r--   0 bkelley    (501) staff       (20)       20 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/requires.txt
--rw-r--r--   0 bkelley    (501) staff       (20)       16 2022-10-19 12:46:08.000000 descriptastorus-2.6.0/descriptastorus.egg-info/top_level.txt
--rw-r--r--   0 bkelley    (501) staff       (20)       38 2022-10-19 12:46:08.865217 descriptastorus-2.6.0/setup.cfg
--rw-r--r--   0 bkelley    (501) staff       (20)     3520 2022-10-19 12:45:16.000000 descriptastorus-2.6.0/setup.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.172504 descriptastorus-2.6.1/
+-rw-r--r--   0 bkelley    (501) staff       (20)     1602 2023-07-28 15:24:43.000000 descriptastorus-2.6.1/LICENSE
+-rw-r--r--   0 bkelley    (501) staff       (20)     9821 2023-07-28 15:28:05.172243 descriptastorus-2.6.1/PKG-INFO
+-rw-r--r--   0 bkelley    (501) staff       (20)     9196 2019-06-19 13:56:29.000000 descriptastorus-2.6.1/README.md
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.001656 descriptastorus-2.6.1/descriptastorus/
+-rw-r--r--   0 bkelley    (501) staff       (20)     8222 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/DescriptaStore.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    13124 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/MolFileIndex.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1811 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus/__init__.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    12299 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/append_store.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.055258 descriptastorus-2.6.1/descriptastorus/cli/
+-rw-r--r--   0 bkelley    (501) staff       (20)     1654 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/descriptastorus/cli/__init__.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     4269 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/cli/storus.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3531 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/descriptastorus/cli/validate.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.110485 descriptastorus-2.6.1/descriptastorus/descriptors/
+-rw-r--r--   0 bkelley    (501) staff       (20)    13404 2021-11-01 14:48:50.000000 descriptastorus-2.6.1/descriptastorus/descriptors/DescriptorGenerator-theirs.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    12894 2023-07-28 15:25:18.000000 descriptastorus-2.6.1/descriptastorus/descriptors/DescriptorGenerator.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    11099 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/descriptastorus/descriptors/QED.py
+-rw-r--r--   0 bkelley    (501) staff       (20)      118 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/descriptors/__init__.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    31293 2021-09-13 16:22:07.000000 descriptastorus-2.6.1/descriptastorus/descriptors/dists.py
+-rw-r--r--   0 bkelley    (501) staff       (20)  3389239 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/descriptors/hists.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    18959 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/descriptors/rdDescriptors.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     4427 2023-07-28 15:25:18.000000 descriptastorus-2.6.1/descriptastorus/descriptors/rdNormalizedDescriptors.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     2817 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/descriptastorus/descriptors/rdkit_fixes.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1441 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/keyvalue.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    12886 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/make_store.py
+-rw-r--r--   0 bkelley    (501) staff       (20)      107 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/descriptastorus/mode.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    18447 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/raw.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.112011 descriptastorus-2.6.1/descriptastorus/stores/
+-rw-r--r--   0 bkelley    (501) staff       (20)       48 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/descriptastorus/stores/__init__.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1131 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/stores/dbmstore.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1312 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/descriptastorus/stores/kyotostore.py
+-rw-r--r--   0 bkelley    (501) staff       (20)      651 2019-07-17 20:10:46.000000 descriptastorus-2.6.1/descriptastorus/utils.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.002898 descriptastorus-2.6.1/descriptastorus.egg-info/
+-rw-r--r--   0 bkelley    (501) staff       (20)     9821 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/PKG-INFO
+-rw-r--r--   0 bkelley    (501) staff       (20)     1573 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/SOURCES.txt
+-rw-r--r--   0 bkelley    (501) staff       (20)        1 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/dependency_links.txt
+-rw-r--r--   0 bkelley    (501) staff       (20)      111 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/entry_points.txt
+-rw-r--r--   0 bkelley    (501) staff       (20)       32 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/requires.txt
+-rw-r--r--   0 bkelley    (501) staff       (20)       16 2023-07-28 15:28:04.000000 descriptastorus-2.6.1/descriptastorus.egg-info/top_level.txt
+-rw-r--r--   0 bkelley    (501) staff       (20)      669 2023-07-28 15:23:56.000000 descriptastorus-2.6.1/pyproject.toml
+-rw-r--r--   0 bkelley    (501) staff       (20)       38 2023-07-28 15:28:05.172556 descriptastorus-2.6.1/setup.cfg
+-rw-r--r--   0 bkelley    (501) staff       (20)     3531 2023-07-28 15:27:22.000000 descriptastorus-2.6.1/setup.py
+drwxr-xr-x   0 bkelley    (501) staff       (20)        0 2023-07-28 15:28:05.171911 descriptastorus-2.6.1/tests/
+-rw-r--r--   0 bkelley    (501) staff       (20)    10290 2023-07-28 15:25:18.000000 descriptastorus-2.6.1/tests/test_CLI.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3467 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_CanonicalizeInput.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3387 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/tests/test_ChiralMorgan.py
+-rw-r--r--   0 bkelley    (501) staff       (20)    23815 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_Descriptastore.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3293 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_DescriptastoreAppend.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     7658 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/tests/test_FPDescriptors.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3829 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_NoneReturnFromDescriptorEngine.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     2335 2023-07-28 15:25:18.000000 descriptastorus-2.6.1/tests/test_RDNormalized.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     4107 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/tests/test_RawStorage.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1970 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_StoreNansMultiProcess.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1866 2023-07-28 14:59:16.000000 descriptastorus-2.6.1/tests/test_cache.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1820 2023-07-28 14:59:33.000000 descriptastorus-2.6.1/tests/test_keyvalue.py
+-rw-r--r--   0 bkelley    (501) staff       (20)      680 2020-05-18 14:58:03.000000 descriptastorus-2.6.1/tests/test_pandas.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1651 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/tests/test_rawStore.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     3175 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/tests/test_smiles_reindex.py
+-rw-r--r--   0 bkelley    (501) staff       (20)     1015 2019-06-07 17:44:29.000000 descriptastorus-2.6.1/tests/test_test1.py
```

### Comparing `descriptastorus-2.6.0/LICENSE` & `descriptastorus-2.6.1/descriptastorus/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Copyright (c) 2018, Novartis Institutes for BioMedical Research Inc.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above
-      copyright notice, this list of conditions and the following
-      disclaimer in the documentation and/or other materials provided
-      with the distribution.
-    * Neither the name of Novartis Institutes for BioMedical Research Inc.
-      nor the names of its contributors may be used to endorse or promote
-      products derived from this software without specific prior written
-      permission.
+#  Copyright (c) 2018, Novartis Institutes for BioMedical Research Inc.
+#  All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are
+# met:
+#
+#     * Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#     * Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#     * Neither the name of Novartis Institutes for BioMedical Research Inc.
+#       nor the names of its contributors may be used to endorse or promote
+#       products derived from this software without specific prior written
+#       permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+# OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+# LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+# THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `descriptastorus-2.6.0/README.md` & `descriptastorus-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/DescriptaStore.py` & `descriptastorus-2.6.1/descriptastorus/DescriptaStore.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/MolFileIndex.py` & `descriptastorus-2.6.1/descriptastorus/MolFileIndex.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/__init__.py` & `descriptastorus-2.6.1/descriptastorus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 #
 from . import raw
 from .DescriptaStore import DescriptaStore
 from .mode import Mode
 
 # try and load key stores
 from . import stores
-__version__ = "2.6.0"
+__version__ = "2.5.0.29"
```

### Comparing `descriptastorus-2.6.0/descriptastorus/append_store.py` & `descriptastorus-2.6.1/descriptastorus/append_store.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/cli/__init__.py` & `descriptastorus-2.6.1/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#  Copyright (c) 2018, Novartis Institutes for BioMedical Research Inc.
-#  All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions are
-# met:
-#
-#     * Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#     * Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#     * Neither the name of Novartis Institutes for BioMedical Research Inc.
-#       nor the names of its contributors may be used to endorse or promote
-#       products derived from this software without specific prior written
-#       permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-# OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-# LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-# THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2018-2023, Novartis Institutes for BioMedical Research Inc.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+    * Redistributions of source code must retain the above copyright
+      notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above
+      copyright notice, this list of conditions and the following
+      disclaimer in the documentation and/or other materials provided
+      with the distribution.
+    * Neither the name of Novartis Institutes for BioMedical Research Inc.
+      nor the names of its contributors may be used to endorse or promote
+      products derived from this software without specific prior written
+      permission.
 #
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
```

### Comparing `descriptastorus-2.6.0/descriptastorus/cli/storus.py` & `descriptastorus-2.6.1/descriptastorus/cli/storus.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/cli/validate.py` & `descriptastorus-2.6.1/descriptastorus/cli/validate.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/DescriptorGenerator-theirs.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/DescriptorGenerator-theirs.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/DescriptorGenerator.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/DescriptorGenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,46 +209,54 @@
                         
         if len(smiles) + len(self.cache) > MAX_CACHE:
             self.cache.clear()
             
         # all cached
         if len(_results) == len(smiles):
             all_results = [r[1] for r in _results]
-            return allmols, all_results
+            if keep_mols:
+                return allmols, all_results
+            else:
+                return all_results
         
         # none cached
         elif len(_results) == 0:
             results = self.processMols(mols, goodsmiles, internalParsing=True)
             if MAX_CACHE:
                 if len(indices) == len(smiles):
                     for smile, res, m in zip(smiles, results, allmols):
                         self.cache[smile] = res, m
-
-                    return mols, results
+                    if keep_mols:
+                        return mols, results
+                    return results
 
             # default values are None
             all_results = [None] * len(smiles)
             for idx,result,m in zip(indices, results, allmols):
                 self.cache[smiles[idx]] = result,m
                 all_results[idx] = result
-            return allmols, all_results
+            if keep_mols:
+                return allmols, all_results
+            return all_results
         # some cached
         else:
             results = self.processMols(mols, goodsmiles, internalParsing=True)
             all_results = [None] * len(smiles)
             # grab cached
             for i,res in _results:
                 all_results[i] = res
 
             # grab processed
             for idx,result,m in zip(indices, results, allmols):
                 if MAX_CACHE:
                     self.cache[smiles[idx]] = result,m
                 all_results[idx] = result
-            return allmols, all_results
+            if keep_mols:
+                return allmols, all_results
+            return all_results
 
     def processCtab(self, ctab):
         raise NotImplementedError
     
     def processSDF(self, sdf):
         raise NotImplementedError
```

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/QED.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/QED.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/dists.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/dists.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/hists.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/hists.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/rdDescriptors.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/rdDescriptors.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/rdNormalizedDescriptors.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/rdNormalizedDescriptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,23 @@
 cdfs = {}
 
 for name, (dist, params, minV,maxV,avg,std) in dists.dists.items():
     arg = params[:-2]
     loc = params[-2]
     scale = params[-1]
 
+    if dist in ['gilbrat', 'gibrat']:
+        # fix change in scikit learn
+        if hasattr(dist, 'gilbrat'):
+            dist = 'gilbrat'
+        else:
+            dist = 'gibrat'
+            
     dist = getattr(st, dist)
+        
     
     # make the cdf with the parameters
     def cdf(v, dist=dist, arg=arg,loc=loc,scale=scale,minV=minV,maxV=maxV):
         v = dist.cdf(np.clip(v, minV, maxV), loc=loc, scale=scale, *arg)
         return np.clip(v, 0., 1.)
     
     cdfs[name] = cdf
```

### Comparing `descriptastorus-2.6.0/descriptastorus/descriptors/rdkit_fixes.py` & `descriptastorus-2.6.1/descriptastorus/descriptors/rdkit_fixes.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/keyvalue.py` & `descriptastorus-2.6.1/descriptastorus/keyvalue.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/make_store.py` & `descriptastorus-2.6.1/descriptastorus/make_store.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/raw.py` & `descriptastorus-2.6.1/descriptastorus/raw.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/stores/dbmstore.py` & `descriptastorus-2.6.1/descriptastorus/stores/dbmstore.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/stores/kyotostore.py` & `descriptastorus-2.6.1/descriptastorus/stores/kyotostore.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/descriptastorus/utils.py` & `descriptastorus-2.6.1/descriptastorus/utils.py`

 * *Files identical despite different names*

### Comparing `descriptastorus-2.6.0/setup.py` & `descriptastorus-2.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,30 +64,30 @@
                 lines.append(line)
     with open(path, 'w') as w:
         w.write("".join(lines))
 
 
 else:
     logging.error("Could not run git to get version information... using hard coded version which is likely incorrect")
-    VERSION = "2.6.0"  # hardcode version
+    VERSION = "2.5.1"  # hardcode version
 
 setup(
-    name="descriptastorus",
+    name='descriptastorus',
     version=VERSION,
-    license='BSD',
-    description="Descriptor storage and molecular file indexing",
-    author="Brian Kelley",
-    author_email="bkelley@relaytx.com",
-    url="https://github.com/bp-kelley/descriptastorus",
-    install_requires=["pandas_flavor", "rdkit"],
-    test_suite="nose.collector",
-    tests_require=["nose", "pandas_flavor"],
+    description='Descriptor creation, storage and molecular file indexing',
+    author='Brian Kelley',
+    author_email='bkelley@relaytx.com',
+    url='https://github/bp-kelley/descriptastorus',
+    install_requires=['pandas_flavor', 'rdkit', 'scipy', 'numpy'],
+    test_suite='nose.collector',
+    tests_require=['nose', 'pandas_flavor'],
     include_package_data=True,
     entry_points={
-        "console_scripts": [
-            "storus = descriptastorus.cli.storus:main",
-            "storus-validate = descriptastorus.cli.validate:main",
+        'console_scripts': [
+            'storus = descriptastorus.cli.storus:main',
+            'storus-validate = descriptastorus.cli.validate:main',
         ]
     },
-    packages=find_packages(),
-)
+    
+    packages = find_packages())
+
```

