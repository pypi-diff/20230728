# Comparing `tmp/rouskinhf-0.2.4.tar.gz` & `tmp/rouskinhf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.2.4.tar", last modified: Thu Jul 27 04:47:59 2023, max compression
+gzip compressed data, was "rouskinhf-0.2.5.tar", last modified: Fri Jul 28 05:17:19 2023, max compression
```

## Comparing `rouskinhf-0.2.4.tar` & `rouskinhf-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:47:59.228090 rouskinhf-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-27 04:47:59.224089 rouskinhf-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:47:59.224089 rouskinhf-0.2.4/rouskinhf/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/datafolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/import_dataset_fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/info_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/list_datapoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/rnastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/rouskinhf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:47:59.224089 rouskinhf-0.2.4/rouskinhf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-27 04:47:59.000000 rouskinhf-0.2.4/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 04:47:59.000000 rouskinhf-0.2.4/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 04:47:59.000000 rouskinhf-0.2.4/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-27 04:47:59.000000 rouskinhf-0.2.4/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 04:47:59.000000 rouskinhf-0.2.4/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 04:47:59.228090 rouskinhf-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 04:46:52.000000 rouskinhf-0.2.4/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.472392 rouskinhf-0.2.5/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.2.5/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)     7107 2023-07-28 05:17:19.472221 rouskinhf-0.2.5/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     6656 2023-07-27 16:53:00.000000 rouskinhf-0.2.5/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-28 05:16:41.000000 rouskinhf-0.2.5/pyproject.toml
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.471206 rouskinhf-0.2.5/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)      134 2023-07-28 00:54:40.000000 rouskinhf-0.2.5/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    17391 2023-07-27 22:00:29.000000 rouskinhf-0.2.5/rouskinhf/datafolder.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    10786 2023-07-27 22:09:13.000000 rouskinhf-0.2.5/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.2.5/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2838 2023-07-27 04:57:54.000000 rouskinhf-0.2.5/rouskinhf/import_dataset_fun.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     4609 2023-07-26 22:55:50.000000 rouskinhf-0.2.5/rouskinhf/info_file.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    12498 2023-07-27 22:24:56.000000 rouskinhf-0.2.5/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3652 2023-07-25 20:41:22.000000 rouskinhf-0.2.5/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2503 2023-07-25 00:20:58.000000 rouskinhf-0.2.5/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6262 2023-07-25 18:54:46.000000 rouskinhf-0.2.5/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3681 2023-07-28 00:53:48.000000 rouskinhf-0.2.5/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.471948 rouskinhf-0.2.5/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     7107 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      458 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-28 05:17:19.472438 rouskinhf-0.2.5/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.2.5/setup.py
```

### Comparing `rouskinhf-0.2.4/LICENSE` & `rouskinhf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/PKG-INFO` & `rouskinhf-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
 [![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
 ![PyPI](https://img.shields.io/pypi/v/rouskinhf)
+![GitHub tag (with filter)](https://img.shields.io/github/v/tag/rouskinlab/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
```

### Comparing `rouskinhf-0.2.4/README.md` & `rouskinhf-0.2.5/rouskinhf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,24 @@
+Metadata-Version: 2.1
+Name: rouskinhf
+Version: 0.2.5
+Summary: A library to manipulate data for our DMS prediction models.
+Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
 [![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
 ![PyPI](https://img.shields.io/pypi/v/rouskinhf)
+![GitHub tag (with filter)](https://img.shields.io/github/v/tag/rouskinlab/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
```

### Comparing `rouskinhf-0.2.4/pyproject.toml` & `rouskinhf-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.2.4/rouskinhf/datafolder.py` & `rouskinhf-0.2.5/rouskinhf/datafolder.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .info_file import infoFileWriter
 import os
 import numpy as np
 from huggingface_hub import HfApi
 from huggingface_hub import snapshot_download
 
 
-GENERATE_NPY = False
+GENERATE_NPY = True
 PREDICT_STRUCTURE = False
 PREDICT_DMS = False
 ROUSKINLAB = 'rouskinlab/'
 
 class DataFolderTemplate(PathDatafolder):
 
     def __init__(self, name, path_out) -> None:
```

### Comparing `rouskinhf-0.2.4/rouskinhf/datapoint.py` & `rouskinhf-0.2.5/rouskinhf/datapoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,17 +57,19 @@
 
         if not sequence_has_regular_characters(sequence):
             raise Exception(f"Sequence {sequence} contains characters other than ACGTUacgtu.")
 
         self.reference = reference
         self.sequence = sequence
         self.structure = structure
-        self.paired_bases = self._format_paired_bases(paired_bases) if paired_bases is not None else self._format_paired_bases(self.structure_to_paired_bases(structure)) if structure is not None else None
-        self.dms = self._format_dms(dms) if dms is not None else None
-        self.opt_dict = {'paired_bases': self.paired_bases, 'dms': self.dms}
+        if paired_bases is not None or structure is not None:
+            self.paired_bases = self._format_paired_bases(paired_bases) if paired_bases is not None else self._format_paired_bases(self.structure_to_paired_bases(structure))
+        if dms is not None:
+            self.dms = self._format_dms(dms) 
+        self.opt_dict = {attr: eval(f'self.{attr}') for attr in ['paired_bases', 'dms'] if hasattr(self, attr)}
 
     def _format_paired_bases(self, paired_bases):
         """Returns a set of tuples.
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
         >>> datapoint._format_paired_bases([[1, 4], [0, 5]])
         ((0, 5), (1, 4))
         """
@@ -95,15 +97,17 @@
 
     def _format_dms(self, dms):
         """returns a tuple
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
         >>> datapoint._format_dms([1.0, 2.0, 3.0])
         (1.0, 2.0, 3.0)
         """
-        return tuple(dms) if dms is not None else None
+        if type(dms) == np.ndarray:
+            dms = dms.tolist()
+        return tuple(dms) 
         
 
     def to_dict(self):
         return self.reference, {'sequence': self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}
 
     def to_flat_dict(self):
         return {'reference': self.reference, 'sequence': self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}
@@ -112,15 +116,20 @@
     def from_flat_dict(cls, d):
         return cls(sequence=d['sequence'], reference=d['reference'], **{k:v for k,v in d.items() if k not in ['sequence', 'reference']})
 
     def __str__(self):
         return '"'+self.reference+'"' + ':' + str({"sequence": self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}).replace("'",'"').replace('(','[').replace(')',']').replace('None','null')
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}('{self.reference}', sequence='{self.sequence}', paired_bases={self.paired_bases}, dms={self.dms})"
+        out = f"{self.__class__.__name__}('{self.reference}', sequence='{self.sequence}'"
+        if hasattr(self, 'paired_bases'):
+            out += f", paired_bases={self.paired_bases}"
+        if hasattr(self, 'dms'):
+            out += f", dms={self.dms}"
+        return out + ')'
 
     def structure_to_paired_bases(self, structure):
         """Returns a list of tuples (i,j) where i and j are paired bases."""
         paired_bases = set()
         stack = []
         for i, char in enumerate(structure):
             if char == '(':
@@ -130,15 +139,15 @@
         return paired_bases
 
     def embed_sequence(self):
         """Returns a list of integers corresponding to the sequence.
 
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
         >>> datapoint.embed_sequence()
-        array([0, 0, 1, 1, 2, 2])
+        array([1, 1, 2, 2, 3, 3])
         """
         return np.array([seq2int[base] for base in self.sequence])
 
     def embed_structure(self):
         """Returns a list of integers corresponding to the structure.
 
         >>> from numpy import array
@@ -192,15 +201,15 @@
 
     def from_json_line(string):
         """Create a datapoint from a json line. The json line should have the following format:
         "reference": {"sequence": "sequence", "paired_bases": [[1, 2], [3,4]], "dms": [1.0, 2.0, 3.0]}
 
         Example:
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU"}')
-        Datapoint('reference', sequence='ACAAGU', paired_bases=None, dms=None)
+        Datapoint('reference', sequence='ACAAGU')
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
         Datapoint('reference', sequence='ACAAGU', paired_bases=((1, 2), (3, 4)), dms=(1.0, 2.0, 3.0))
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "something else than ACGTUacgtu", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
         """
 
         # process the string into a dictionary
         string= string.strip()[:-1] if string.strip()[-1] == ',' else string.strip()
```

### Comparing `rouskinhf-0.2.4/rouskinhf/env.py` & `rouskinhf-0.2.5/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/rouskinhf/import_dataset_fun.py` & `rouskinhf-0.2.5/rouskinhf/import_dataset_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     dict: {str: ndarray}
         Dictionary with the following keys: 'references', 'sequences', and 'structure' or 'DMS' depending on the data type.
 
     Example
     -------
 
     >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
+    Force download from HuggingFace Hub
     Over a total of 2 datapoints, there are:
         - 2 valid datapoints
         - 0 invalid datapoints (ex: sequence with non-regular characters)
         - 0 datapoints with the same reference
         - 0 duplicate sequences with the same structure / dms
         - 0 duplicate sequences with different structure / dms
     Using data from HuggingFace Hub
```

### Comparing `rouskinhf-0.2.4/rouskinhf/info_file.py` & `rouskinhf-0.2.5/rouskinhf/info_file.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/rouskinhf/list_datapoints.py` & `rouskinhf-0.2.5/rouskinhf/list_datapoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
             np.array: dms matrix of floats arrays.
 
         Examples:
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
             >>> datapoints.to_dms_npy('temp/dms.npy')
             array([[1.0, 2.0, 3.0]], dtype=object)
         """
-
-        arr = np.array([datapoint.dms for datapoint in self.datapoints], dtype=object)
-        np.save(path, arr)
+        
+        arr = np.array([np.array(datapoint.dms, dtype=np.float32) for datapoint in self.datapoints], dtype=object)
+        np.save(path, arr, allow_pickle=True)
         return arr
 
 
     def to_sequence_npy(self, path):
         """Writes the sequence npy file from the list of datapoints.
 
         Args:
@@ -93,15 +93,15 @@
         Returns:
             np.array: int-encoded sequence matrix
 
         Examples:
             >>> from numpy import array
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0]),\
                                                Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
-            >>> assert not (datapoints.to_sequence_npy('temp/sequence.npy') - array([[0, 0, 1 ,1, 2, 2],[0, 0, 1, 1, 2 ,2]], dtype=object)).any(), "The sequence matrix is not correct."
+            >>> assert not (datapoints.to_sequence_npy('temp/sequence.npy') - array([[1, 1, 2, 2, 3, 3],[1, 1, 2, 2, 3, 3]], dtype=object)).any(), "The sequence matrix is not correct."
         """
 
         arr = np.array([datapoint.embed_sequence() for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
         return arr
```

### Comparing `rouskinhf-0.2.4/rouskinhf/parsers.py` & `rouskinhf-0.2.5/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/rouskinhf/path.py` & `rouskinhf-0.2.5/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/rouskinhf/rnastructure.py` & `rouskinhf-0.2.5/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.4/rouskinhf/util.py` & `rouskinhf-0.2.5/rouskinhf/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,18 @@
         'X': 0,
         'A': 1,
         'C': 2,
         'G': 3,
         'U': 4,
     }
 
+int2seq = {v: k for k, v in seq2int.items()}
+
 dot2int = {'.': 1, '(': 2, ')': 3, 'X': 0}
-int2dot = ['X', '.', '(', ')']
+int2dot = {v: k for k, v in dot2int.items()}
 
 
 def fastaToDict(fasta_file):
     """
     Reads a fasta file and returns a dictionary {sequence: reference}.
 
     Args:
```

### Comparing `rouskinhf-0.2.4/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: rouskinhf
-Version: 0.2.4
-Summary: A library to manipulate data for our DMS prediction models.
-Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
 [![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
 ![PyPI](https://img.shields.io/pypi/v/rouskinhf)
+![GitHub tag (with filter)](https://img.shields.io/github/v/tag/rouskinlab/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
```

