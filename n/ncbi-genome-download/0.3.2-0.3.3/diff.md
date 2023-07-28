# Comparing `tmp/ncbi-genome-download-0.3.2.tar.gz` & `tmp/ncbi-genome-download-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi-genome-download-0.3.2.tar", last modified: Mon Jul 24 06:26:48 2023, max compression
+gzip compressed data, was "ncbi-genome-download-0.3.3.tar", last modified: Fri Jul 28 12:49:19 2023, max compression
```

## Comparing `ncbi-genome-download-0.3.2.tar` & `ncbi-genome-download-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/README-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.592561 ncbi-genome-download-0.3.2/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6113 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/contrib/gimme_taxa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/ncbi_genome_download/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/ncbi_genome_download/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 06:26:48.000000 ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:26:48.596561 ncbi-genome-download-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/assembly_status.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/new_format_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/noascii_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/partial_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/type_material.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/viral_summary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-24 06:26:34.000000 ncbi-genome-download-0.3.2/tests/weird_organism_name_summary.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:49:19.480194 ncbi-genome-download-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-28 12:49:19.480194 ncbi-genome-download-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/README-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:49:19.472194 ncbi-genome-download-0.3.3/contrib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6113 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/contrib/gimme_taxa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:49:19.472194 ncbi-genome-download-0.3.3/ncbi_genome_download/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/ncbi_genome_download/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:49:19.476194 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 12:49:19.000000 ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 12:49:19.480194 ncbi-genome-download-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:49:19.480194 ncbi-genome-download-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/assembly_status.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/new_format_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/noascii_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/partial_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/type_material.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/viral_summary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 12:49:09.000000 ncbi-genome-download-0.3.3/tests/weird_organism_name_summary.txt
```

### Comparing `ncbi-genome-download-0.3.2/LICENSE` & `ncbi-genome-download-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/PKG-INFO` & `ncbi-genome-download-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi-genome-download
-Version: 0.3.2
+Version: 0.3.3
 Summary: Download genome files from the NCBI FTP server.
 Home-page: https://github.com/kblin/ncbi-genome-download/
 Author: Kai Blin
 Author-email: kblin@biosustain.dtu.dk
 License: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # NCBI Genome Downloading Scripts
 
 [![PyPI release](https://img.shields.io/pypi/v/ncbi-genome-download.svg)](https://pypi.python.org/pypi/ncbi-genome-download/)
+[![DOI](https://zenodo.org/badge/57950916.svg)](https://zenodo.org/badge/latestdoi/57950916)
 
 Some script to download bacterial and fungal genomes from NCBI after they
 restructured their FTP a while ago.
 
 Idea shamelessly stolen from [Mick Watson's Kraken downloader
 scripts](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/)
 that can also be found in [Mick's GitHub
@@ -321,11 +322,16 @@
 
 ```bash
 python gimme_taxa.py
 python gimme_taxa.py -h
 python gimme_taxa.py --help
 ```
 
+## Citing `ncbi-genome-download`
+
+You can cite `ncbi-genome-download` via the Zenodo deposit under
+[DOI: 10.5281/zenodo.8192433](https://doi.org/10.5281/zenodo.8192433).
+
 ## License
 
 All code is available under the Apache License version 2, see the
 [`LICENSE`](LICENSE) file for details.
```

### Comparing `ncbi-genome-download-0.3.2/README-CN.md` & `ncbi-genome-download-0.3.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/README.md` & `ncbi-genome-download-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # NCBI Genome Downloading Scripts
 
 [![PyPI release](https://img.shields.io/pypi/v/ncbi-genome-download.svg)](https://pypi.python.org/pypi/ncbi-genome-download/)
+[![DOI](https://zenodo.org/badge/57950916.svg)](https://zenodo.org/badge/latestdoi/57950916)
 
 Some script to download bacterial and fungal genomes from NCBI after they
 restructured their FTP a while ago.
 
 Idea shamelessly stolen from [Mick Watson's Kraken downloader
 scripts](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/)
 that can also be found in [Mick's GitHub
@@ -302,11 +303,16 @@
 
 ```bash
 python gimme_taxa.py
 python gimme_taxa.py -h
 python gimme_taxa.py --help
 ```
 
+## Citing `ncbi-genome-download`
+
+You can cite `ncbi-genome-download` via the Zenodo deposit under
+[DOI: 10.5281/zenodo.8192433](https://doi.org/10.5281/zenodo.8192433).
+
 ## License
 
 All code is available under the Apache License version 2, see the
 [`LICENSE`](LICENSE) file for details.
```

### Comparing `ncbi-genome-download-0.3.2/contrib/gimme_taxa.py` & `ncbi-genome-download-0.3.3/contrib/gimme_taxa.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/__main__.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/__main__.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/config.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/config.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/core.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/core.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/jobs.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/jobs.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/metadata.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/metadata.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download/summary.py` & `ncbi-genome-download-0.3.3/ncbi_genome_download/summary.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/PKG-INFO` & `ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi-genome-download
-Version: 0.3.2
+Version: 0.3.3
 Summary: Download genome files from the NCBI FTP server.
 Home-page: https://github.com/kblin/ncbi-genome-download/
 Author: Kai Blin
 Author-email: kblin@biosustain.dtu.dk
 License: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # NCBI Genome Downloading Scripts
 
 [![PyPI release](https://img.shields.io/pypi/v/ncbi-genome-download.svg)](https://pypi.python.org/pypi/ncbi-genome-download/)
+[![DOI](https://zenodo.org/badge/57950916.svg)](https://zenodo.org/badge/latestdoi/57950916)
 
 Some script to download bacterial and fungal genomes from NCBI after they
 restructured their FTP a while ago.
 
 Idea shamelessly stolen from [Mick Watson's Kraken downloader
 scripts](http://www.opiniomics.org/building-a-kraken-database-with-new-ftp-structure-and-no-gi-numbers/)
 that can also be found in [Mick's GitHub
@@ -321,11 +322,16 @@
 
 ```bash
 python gimme_taxa.py
 python gimme_taxa.py -h
 python gimme_taxa.py --help
 ```
 
+## Citing `ncbi-genome-download`
+
+You can cite `ncbi-genome-download` via the Zenodo deposit under
+[DOI: 10.5281/zenodo.8192433](https://doi.org/10.5281/zenodo.8192433).
+
 ## License
 
 All code is available under the Apache License version 2, see the
 [`LICENSE`](LICENSE) file for details.
```

### Comparing `ncbi-genome-download-0.3.2/ncbi_genome_download.egg-info/SOURCES.txt` & `ncbi-genome-download-0.3.3/ncbi_genome_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/setup.py` & `ncbi-genome-download-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/assembly_status.txt` & `ncbi-genome-download-0.3.3/tests/assembly_status.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/new_format_summary.txt` & `ncbi-genome-download-0.3.3/tests/new_format_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/noascii_summary.txt` & `ncbi-genome-download-0.3.3/tests/noascii_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/partial_summary.txt` & `ncbi-genome-download-0.3.3/tests/partial_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/type_material.txt` & `ncbi-genome-download-0.3.3/tests/type_material.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/viral_summary.txt` & `ncbi-genome-download-0.3.3/tests/viral_summary.txt`

 * *Files identical despite different names*

### Comparing `ncbi-genome-download-0.3.2/tests/weird_organism_name_summary.txt` & `ncbi-genome-download-0.3.3/tests/weird_organism_name_summary.txt`

 * *Files identical despite different names*

