# Comparing `tmp/miniFasta-3.0.2.tar.gz` & `tmp/miniFasta-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniFasta-3.0.2.tar", last modified: Tue Nov  8 10:05:01 2022, max compression
+gzip compressed data, was "miniFasta-3.0.3.tar", last modified: Fri Jul 28 20:28:38 2023, max compression
```

## Comparing `miniFasta-3.0.2.tar` & `miniFasta-3.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:05:01.141028 miniFasta-3.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (121)    35149 2022-11-08 10:04:48.000000 miniFasta-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7882 2022-11-08 10:05:01.141028 miniFasta-3.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     7088 2022-11-08 10:04:48.000000 miniFasta-3.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      501 2022-11-08 10:04:48.000000 miniFasta-3.0.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      974 2022-11-08 10:05:01.141028 miniFasta-3.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       69 2022-11-08 10:04:48.000000 miniFasta-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:05:01.141028 miniFasta-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:05:01.141028 miniFasta-3.0.2/src/miniFasta/
--rwxr-xr-x   0 runner    (1001) docker     (121)      252 2022-11-08 10:04:48.000000 miniFasta-3.0.2/src/miniFasta/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7297 2022-11-08 10:04:48.000000 miniFasta-3.0.2/src/miniFasta/_miniFasta.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3672 2022-11-08 10:04:48.000000 miniFasta-3.0.2/src/miniFasta/_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      911 2022-11-08 10:04:48.000000 miniFasta-3.0.2/src/miniFasta/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:05:01.141028 miniFasta-3.0.2/src/miniFasta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7882 2022-11-08 10:05:01.000000 miniFasta-3.0.2/src/miniFasta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-08 10:05:01.000000 miniFasta-3.0.2/src/miniFasta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 10:05:01.000000 miniFasta-3.0.2/src/miniFasta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 10:05:00.000000 miniFasta-3.0.2/src/miniFasta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-08 10:05:01.000000 miniFasta-3.0.2/src/miniFasta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-08 10:05:01.000000 miniFasta-3.0.2/src/miniFasta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:38.972159 miniFasta-3.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-07-28 20:28:26.000000 miniFasta-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-28 20:28:38.972159 miniFasta-3.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7088 2023-07-28 20:28:26.000000 miniFasta-3.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-28 20:28:26.000000 miniFasta-3.0.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-28 20:28:38.972159 miniFasta-3.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-07-28 20:28:26.000000 miniFasta-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:38.968159 miniFasta-3.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:38.972159 miniFasta-3.0.3/src/miniFasta/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-07-28 20:28:26.000000 miniFasta-3.0.3/src/miniFasta/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7297 2023-07-28 20:28:26.000000 miniFasta-3.0.3/src/miniFasta/_miniFasta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3751 2023-07-28 20:28:26.000000 miniFasta-3.0.3/src/miniFasta/_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      911 2023-07-28 20:28:26.000000 miniFasta-3.0.3/src/miniFasta/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:38.972159 miniFasta-3.0.3/src/miniFasta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 20:28:38.000000 miniFasta-3.0.3/src/miniFasta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:38.972159 miniFasta-3.0.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3578 2023-07-28 20:28:26.000000 miniFasta-3.0.3/tests/test_fasta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3306 2023-07-28 20:28:26.000000 miniFasta-3.0.3/tests/test_fasta_read.py
```

### Comparing `miniFasta-3.0.2/LICENSE` & `miniFasta-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miniFasta-3.0.2/PKG-INFO` & `miniFasta-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniFasta
-Version: 3.0.2
+Version: 3.0.3
 Summary: A simple FASTA read and write toolbox for small to medium size projects without dependencies.
 Home-page: https://github.com/not-a-feature/miniFASTA
 Author: Jules Kreuer / not_a_feature
 License: gpl-3.0
 Keywords: FASTA,reader,bio,bioinformatics
 Platform: unix
 Platform: linux
```

### Comparing `miniFasta-3.0.2/README.md` & `miniFasta-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `miniFasta-3.0.2/setup.cfg` & `miniFasta-3.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = miniFasta
-version = 3.0.2
+version = 3.0.3
 description = A simple FASTA read and write toolbox for small to medium size projects without dependencies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = FASTA, reader, bio, bioinformatics
 home-page = https://github.com/not-a-feature/miniFASTA
 author = Jules Kreuer / not_a_feature
 license = gpl-3.0
```

### Comparing `miniFasta-3.0.2/src/miniFasta/_miniFasta.py` & `miniFasta-3.0.3/src/miniFasta/_miniFasta.py`

 * *Files identical despite different names*

### Comparing `miniFasta-3.0.2/src/miniFasta/_reader.py` & `miniFasta-3.0.3/src/miniFasta/_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ._miniFasta import fasta_object
 
 from zipfile import ZipFile
 import gzip
 import tarfile
 
 from os import path
-from typing import Iterator, Union
+from typing import Iterator, Union, List
 
 
 def __maybeByteToStr(maybeByte) -> str:
     if isinstance(maybeByte, bytes):
         return maybeByte.decode("utf-8").rstrip()
     return str(maybeByte).rstrip()
 
@@ -73,46 +73,47 @@
             handlers = [gzip.open(file_path, "r")]  # type:ignore
     else:
         handlers = [open(file_path, "r")]  # type:ignore
 
     for h in handlers:
         with h:
             head = ""
-            body = ""
+            body: List[str] = []
             newObject = True
 
             for maybe_byte_line in h:
                 # Convert byte string to string
                 line = __maybeByteToStr(maybe_byte_line)
 
                 # Go through each line
 
                 # First Header
+                ">."
                 if newObject and line.startswith(">"):
                     head = line.strip()
-                    body = ""
+                    body = []
                     newObject = False
 
                 # N-th Header
                 elif line.startswith(">"):
                     # Yield only sequence or complete fasta_object
                     if seq:
-                        yield body
+                        yield "".join(body)
                     else:
-                        yield fasta_object(head, body)
+                        yield fasta_object(head, "".join(body))
                     head = line.strip()
-                    body = ""
+                    body = []
 
                 # Sequence
                 else:
                     addBody = line.strip()
                     if upper:
                         addBody = addBody.upper()
 
-                    body += addBody
+                    body.append(addBody)
 
             # Yield last element
             # Yield only sequence or complete fasta_object
             if seq:
-                yield body
+                yield "".join(body)
             else:
-                yield fasta_object(head, body)
+                yield fasta_object(head, "".join(body))
```

### Comparing `miniFasta-3.0.2/src/miniFasta/_writer.py` & `miniFasta-3.0.3/src/miniFasta/_writer.py`

 * *Files identical despite different names*

### Comparing `miniFasta-3.0.2/src/miniFasta.egg-info/PKG-INFO` & `miniFasta-3.0.3/src/miniFasta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniFasta
-Version: 3.0.2
+Version: 3.0.3
 Summary: A simple FASTA read and write toolbox for small to medium size projects without dependencies.
 Home-page: https://github.com/not-a-feature/miniFASTA
 Author: Jules Kreuer / not_a_feature
 License: gpl-3.0
 Keywords: FASTA,reader,bio,bioinformatics
 Platform: unix
 Platform: linux
```

