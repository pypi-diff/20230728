# Comparing `tmp/jamofetch-3.4.1.tar.gz` & `tmp/jamofetch-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.4.1.tar", max compression
+gzip compressed data, was "jamofetch-3.5.0.tar", max compression
```

## Comparing `jamofetch-3.4.1.tar` & `jamofetch-3.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4728 2023-07-21 01:16:33.706667 jamofetch-3.4.1/README.md
--rw-r--r--   0        0        0      522 2023-07-21 01:14:48.920470 jamofetch-3.4.1/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-07 23:08:25.647260 jamofetch-3.4.1/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10838 2023-07-18 02:30:40.133609 jamofetch-3.4.1/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 jamofetch-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4675 2023-07-22 04:56:00.098688 jamofetch-3.5.0/README.md
+-rw-r--r--   0        0        0      522 2023-07-27 23:07:05.500848 jamofetch-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-07 23:08:25.647260 jamofetch-3.5.0/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10932 2023-07-27 23:05:24.072873 jamofetch-3.5.0/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.5.0/PKG-INFO
```

### Comparing `jamofetch-3.4.1/README.md` & `jamofetch-3.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -58,27 +58,26 @@
     real_path = lib_seq.get_real_path_wait()
     print(f"sequence ready at {real_path}")
 ```
 ## Command Line Tool
 Installing jamofetch with pip exposes a command line interface.
 ```
 (venv) [dnscott@ln004 jamofetch]$ jamofetch  -h
-usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [-v] [--logging LOGGING]
+usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [--logging LOGGING]
 
 options:
   -h, --help            show this help message and exit
   -l LIBRARY, --library LIBRARY
                         library name(s) for which to retrieve sequence
   -d DIRECTORY, --directory DIRECTORY
                         directory where to link sequence, defaults to current directory. Directory will be created if it doesn't exit.
   -i INTERVAL, --interval INTERVAL
                         wait interval in seconds to check if sequence has been fetched, ignored if wait flag not set
   -m MAX, --max MAX     maximum time to wait for sequence in seconds, ignored if wait flag not set. Specify -1 to wait indefinetely.
   -w, --wait            wait for jamo to link sequence, output real path of linked sequence
-  -v, --version         print jamofetch version
   --logging LOGGING     logging level (specify DEBUG for verbose logging)
 (venv) [dnscott@ln004 jamofetch]$ jamofetch -d data -l NPUNN -l NOOHG -l HOGH -w --max -1
 fetching sequence:
 NPUNN /global/dna/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz BACKUP_COMPLETE 6391936239a7711d789a9380
 NOOHG /global/dna/dm_archive/sdm/pacbio/00/26/91/pbio-2691.26653.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz RESTORED 6347dbb35bc59487d7e768d6
 HOGH /global/dna/dm_archive/sdm/illumina/00/63/97/6397.2.44053.GGCTAC.fastq.gz RESTORE_IN_PROGRESS 51d52a82067c014cd6ef4f6f
```

### Comparing `jamofetch-3.4.1/pyproject.toml` & `jamofetch-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.4.1"
+version = "3.5.0"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.4.1/src/jamofetch/jamofetch.py` & `jamofetch-3.5.0/src/jamofetch/jamofetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,19 +168,20 @@
         and return a LibSeq object containing the path to the sequence.
         """
         pathlib.Path(self._link_dir).mkdir(parents=True, exist_ok=True, mode=0o775)
         os.chdir(self._link_dir)
         clean_lib_name = _clean_library_name(lib_name)
 
         cmd = self.get_cmd(clean_lib_name)
+        print(cmd, file=out_file)
         output = subprocess.check_output(cmd, shell=True)
         for line in output.splitlines():
             print(line.decode("utf-8"), file=out_file)
-
         seq_path = _find_fastq_path(clean_lib_name, self._link_dir)
+        print(f"{clean_lib_name} {seq_path}", file=out_file)
         return JamoLibSeq(clean_lib_name, seq_path, self._wait_interval_secs, self._wait_max_secs)
 
 
 def _fetch_seq(fetcher: JamoFetcher, libs):
     lib_seq_dict = {}
     for lib in libs:
         try:
```

### Comparing `jamofetch-3.4.1/PKG-INFO` & `jamofetch-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.4.1
+Version: 3.5.0
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -73,27 +73,26 @@
     real_path = lib_seq.get_real_path_wait()
     print(f"sequence ready at {real_path}")
 ```
 ## Command Line Tool
 Installing jamofetch with pip exposes a command line interface.
 ```
 (venv) [dnscott@ln004 jamofetch]$ jamofetch  -h
-usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [-v] [--logging LOGGING]
+usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [--logging LOGGING]
 
 options:
   -h, --help            show this help message and exit
   -l LIBRARY, --library LIBRARY
                         library name(s) for which to retrieve sequence
   -d DIRECTORY, --directory DIRECTORY
                         directory where to link sequence, defaults to current directory. Directory will be created if it doesn't exit.
   -i INTERVAL, --interval INTERVAL
                         wait interval in seconds to check if sequence has been fetched, ignored if wait flag not set
   -m MAX, --max MAX     maximum time to wait for sequence in seconds, ignored if wait flag not set. Specify -1 to wait indefinetely.
   -w, --wait            wait for jamo to link sequence, output real path of linked sequence
-  -v, --version         print jamofetch version
   --logging LOGGING     logging level (specify DEBUG for verbose logging)
 (venv) [dnscott@ln004 jamofetch]$ jamofetch -d data -l NPUNN -l NOOHG -l HOGH -w --max -1
 fetching sequence:
 NPUNN /global/dna/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz BACKUP_COMPLETE 6391936239a7711d789a9380
 NOOHG /global/dna/dm_archive/sdm/pacbio/00/26/91/pbio-2691.26653.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz RESTORED 6347dbb35bc59487d7e768d6
 HOGH /global/dna/dm_archive/sdm/illumina/00/63/97/6397.2.44053.GGCTAC.fastq.gz RESTORE_IN_PROGRESS 51d52a82067c014cd6ef4f6f
```

