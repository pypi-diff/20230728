# Comparing `tmp/igv-reports-1.7.0.tar.gz` & `tmp/igv-reports-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igv-reports-1.7.0.tar", last modified: Mon Feb  6 06:22:31 2023, max compression
+gzip compressed data, was "igv-reports-1.8.0.tar", last modified: Fri Jul 28 16:33:44 2023, max compression
```

## Comparing `igv-reports-1.7.0.tar` & `igv-reports-1.8.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-02-06 06:22:31.069208 igv-reports-1.7.0/
--rw-r--r--   0 jrobinso   (502) staff       (20)     1140 2020-06-15 02:32:44.000000 igv-reports-1.7.0/LICENSE.md
--rw-r--r--   0 jrobinso   (502) staff       (20)    16007 2023-02-06 06:22:31.068851 igv-reports-1.7.0/PKG-INFO
--rw-r--r--   0 jrobinso   (502) staff       (20)    13211 2023-02-06 06:19:35.000000 igv-reports-1.7.0/README.md
-drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-02-06 06:22:31.054556 igv-reports-1.7.0/igv_reports/
--rw-r--r--   0 jrobinso   (502) staff       (20)      163 2020-06-15 02:32:45.000000 igv-reports-1.7.0/igv_reports/__init__.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1904 2022-09-20 22:13:09.000000 igv-reports-1.7.0/igv_reports/bam.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     5038 2023-02-02 05:26:56.000000 igv-reports-1.7.0/igv_reports/bedtable.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      680 2022-07-25 04:55:29.000000 igv-reports-1.7.0/igv_reports/chralias.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1561 2022-07-25 04:55:29.000000 igv-reports-1.7.0/igv_reports/datauri.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1176 2022-09-20 22:06:55.000000 igv-reports-1.7.0/igv_reports/fasta.py
--rw-r--r--   0 jrobinso   (502) staff       (20)    12094 2023-02-02 06:32:29.000000 igv-reports-1.7.0/igv_reports/feature.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      618 2022-07-25 04:55:29.000000 igv-reports-1.7.0/igv_reports/featureTree.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     3020 2023-02-02 06:24:45.000000 igv-reports-1.7.0/igv_reports/generictable.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      681 2022-07-25 17:10:04.000000 igv-reports-1.7.0/igv_reports/genome.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1240 2022-07-25 17:10:04.000000 igv-reports-1.7.0/igv_reports/ideogram.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1399 2020-06-15 02:32:45.000000 igv-reports-1.7.0/igv_reports/regions.py
--rw-r--r--   0 jrobinso   (502) staff       (20)    14912 2023-02-02 05:26:56.000000 igv-reports-1.7.0/igv_reports/report.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      621 2022-07-25 04:55:29.000000 igv-reports-1.7.0/igv_reports/stream.py
-drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-02-06 06:22:31.059831 igv-reports-1.7.0/igv_reports/templates/
--rw-r--r--   0 jrobinso   (502) staff       (20)    10816 2023-02-03 16:36:52.000000 igv-reports-1.7.0/igv_reports/templates/junction_template.html
--rw-r--r--   0 jrobinso   (502) staff       (20)     8312 2023-02-03 16:33:19.000000 igv-reports-1.7.0/igv_reports/templates/variant_template-2.html
--rw-r--r--   0 jrobinso   (502) staff       (20)     1285 2023-02-02 04:15:34.000000 igv-reports-1.7.0/igv_reports/tracks.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      544 2023-02-02 01:01:05.000000 igv-reports-1.7.0/igv_reports/utils.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     7462 2022-07-27 18:06:50.000000 igv-reports-1.7.0/igv_reports/varianttable.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     3392 2022-07-27 18:34:19.000000 igv-reports-1.7.0/igv_reports/vcf.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     4475 2023-02-02 07:02:10.000000 igv-reports-1.7.0/igv_reports/wig.py
-drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-02-06 06:22:31.058260 igv-reports-1.7.0/igv_reports.egg-info/
--rw-r--r--   0 jrobinso   (502) staff       (20)    16007 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/PKG-INFO
--rw-r--r--   0 jrobinso   (502) staff       (20)      960 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/SOURCES.txt
--rw-r--r--   0 jrobinso   (502) staff       (20)        1 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/dependency_links.txt
--rw-r--r--   0 jrobinso   (502) staff       (20)      101 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/entry_points.txt
--rw-r--r--   0 jrobinso   (502) staff       (20)       28 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/requires.txt
--rw-r--r--   0 jrobinso   (502) staff       (20)       12 2023-02-06 06:22:30.000000 igv-reports-1.7.0/igv_reports.egg-info/top_level.txt
--rw-r--r--   0 jrobinso   (502) staff       (20)       38 2023-02-06 06:22:31.069313 igv-reports-1.7.0/setup.cfg
--rw-r--r--   0 jrobinso   (502) staff       (20)     1528 2023-02-06 06:12:17.000000 igv-reports-1.7.0/setup.py
-drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-02-06 06:22:31.068034 igv-reports-1.7.0/test/
--rw-r--r--   0 jrobinso   (502) staff       (20)     4291 2022-09-20 22:13:09.000000 igv-reports-1.7.0/test/test_bam.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      636 2022-07-25 04:55:29.000000 igv-reports-1.7.0/test/test_datauri.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     1215 2022-07-20 20:54:26.000000 igv-reports-1.7.0/test/test_fasta.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     5731 2022-07-25 04:55:29.000000 igv-reports-1.7.0/test/test_feature.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      999 2022-07-25 04:55:29.000000 igv-reports-1.7.0/test/test_ideogram.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      491 2020-06-15 02:32:46.000000 igv-reports-1.7.0/test/test_regions.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     3148 2022-07-27 18:09:03.000000 igv-reports-1.7.0/test/test_table.py
--rw-r--r--   0 jrobinso   (502) staff       (20)      481 2020-06-15 02:32:46.000000 igv-reports-1.7.0/test/test_track.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     4324 2022-07-27 18:37:15.000000 igv-reports-1.7.0/test/test_vcf.py
--rw-r--r--   0 jrobinso   (502) staff       (20)     2804 2023-02-06 06:08:35.000000 igv-reports-1.7.0/test/test_wig.py
+drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-07-28 16:33:44.560617 igv-reports-1.8.0/
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1140 2020-06-15 02:32:44.000000 igv-reports-1.8.0/LICENSE.md
+-rw-r--r--   0 jrobinso   (502) staff       (20)    16008 2023-07-28 16:33:44.560251 igv-reports-1.8.0/PKG-INFO
+-rw-r--r--   0 jrobinso   (502) staff       (20)    13188 2023-07-28 16:22:23.000000 igv-reports-1.8.0/README.md
+drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-07-28 16:33:44.525209 igv-reports-1.8.0/igv_reports/
+-rw-r--r--   0 jrobinso   (502) staff       (20)      163 2020-06-15 02:32:45.000000 igv-reports-1.8.0/igv_reports/__init__.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     2033 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/bam.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     5038 2023-02-02 05:26:56.000000 igv-reports-1.8.0/igv_reports/bedtable.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      680 2022-07-25 04:55:29.000000 igv-reports-1.8.0/igv_reports/chralias.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1561 2022-07-25 04:55:29.000000 igv-reports-1.8.0/igv_reports/datauri.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1255 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/fasta.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)    13605 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/feature.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      618 2022-07-25 04:55:29.000000 igv-reports-1.8.0/igv_reports/featureTree.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     4679 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/generictable.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      681 2022-07-25 17:10:04.000000 igv-reports-1.8.0/igv_reports/genome.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1240 2022-07-25 17:10:04.000000 igv-reports-1.8.0/igv_reports/ideogram.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1399 2020-06-15 02:32:45.000000 igv-reports-1.8.0/igv_reports/regions.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)    20288 2023-07-28 15:37:34.000000 igv-reports-1.8.0/igv_reports/report.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      939 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/stream.py
+drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-07-28 16:33:44.531629 igv-reports-1.8.0/igv_reports/templates/
+-rw-r--r--   0 jrobinso   (502) staff       (20)     6518 2023-07-28 16:27:41.000000 igv-reports-1.8.0/igv_reports/templates/fusion_template.html
+-rw-r--r--   0 jrobinso   (502) staff       (20)    10816 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/templates/junction_template.html
+-rw-r--r--   0 jrobinso   (502) staff       (20)     9369 2023-07-21 17:34:42.000000 igv-reports-1.8.0/igv_reports/templates/variant_template-noembed.html
+-rw-r--r--   0 jrobinso   (502) staff       (20)     8681 2023-07-21 17:34:42.000000 igv-reports-1.8.0/igv_reports/templates/variant_template.html
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1284 2023-07-21 17:23:26.000000 igv-reports-1.8.0/igv_reports/tracks.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1215 2023-07-28 15:21:44.000000 igv-reports-1.8.0/igv_reports/utils.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     7462 2022-07-27 18:06:50.000000 igv-reports-1.8.0/igv_reports/varianttable.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     3392 2022-07-27 18:34:19.000000 igv-reports-1.8.0/igv_reports/vcf.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     4475 2023-02-02 07:02:10.000000 igv-reports-1.8.0/igv_reports/wig.py
+drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-07-28 16:33:44.528938 igv-reports-1.8.0/igv_reports.egg-info/
+-rw-r--r--   0 jrobinso   (502) staff       (20)    16008 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/PKG-INFO
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1092 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 jrobinso   (502) staff       (20)        1 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 jrobinso   (502) staff       (20)      101 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/entry_points.txt
+-rw-r--r--   0 jrobinso   (502) staff       (20)       28 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/requires.txt
+-rw-r--r--   0 jrobinso   (502) staff       (20)       12 2023-07-28 16:33:44.000000 igv-reports-1.8.0/igv_reports.egg-info/top_level.txt
+-rw-r--r--   0 jrobinso   (502) staff       (20)       38 2023-07-28 16:33:44.560716 igv-reports-1.8.0/setup.cfg
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1528 2023-07-28 04:19:21.000000 igv-reports-1.8.0/setup.py
+drwxr-xr-x   0 jrobinso   (502) staff       (20)        0 2023-07-28 16:33:44.559420 igv-reports-1.8.0/test/
+-rw-r--r--   0 jrobinso   (502) staff       (20)     4291 2023-07-20 19:52:52.000000 igv-reports-1.8.0/test/test_bam.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      636 2022-07-25 04:55:29.000000 igv-reports-1.8.0/test/test_datauri.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     1215 2022-07-20 20:54:26.000000 igv-reports-1.8.0/test/test_fasta.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     5731 2022-07-25 04:55:29.000000 igv-reports-1.8.0/test/test_feature.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      999 2022-07-25 04:55:29.000000 igv-reports-1.8.0/test/test_ideogram.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      491 2020-06-15 02:32:46.000000 igv-reports-1.8.0/test/test_regions.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      607 2023-07-21 17:23:26.000000 igv-reports-1.8.0/test/test_stream.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     3415 2023-07-21 17:23:26.000000 igv-reports-1.8.0/test/test_table.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      481 2020-06-15 02:32:46.000000 igv-reports-1.8.0/test/test_track.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)      714 2023-07-21 17:23:26.000000 igv-reports-1.8.0/test/test_utils.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     4324 2022-07-27 18:37:15.000000 igv-reports-1.8.0/test/test_vcf.py
+-rw-r--r--   0 jrobinso   (502) staff       (20)     2804 2023-02-06 06:08:35.000000 igv-reports-1.8.0/test/test_wig.py
```

### Comparing `igv-reports-1.7.0/LICENSE.md` & `igv-reports-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/PKG-INFO` & `igv-reports-1.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 Metadata-Version: 2.1
 Name: igv-reports
-Version: 1.7.0
+Version: 1.8.0
 Summary: Creates self-contained html pages for visual variant review with IGV (igv.js).
 Home-page: https://github.com/igvteam/igv-reports
 Author: Jim Robinson
 License: MIT
 Description: # igv-reports
         
         A Python application to generate self-contained HTML reports that consist of a table of genomic sites or regions and associated IGV views for each site.
         The generated HTML page contains all data neccessary for IGV as uuencoded blobs. It can be opened within a web browser as a static page, with no depenency on the original input files.
         
-        ### _NEW - alignments marked "duplicate" are now filtered by default.  See the --exclude-flags option._
-        
         ## Installation
         
         #### Prerequisites
         
         igv-reports __requires Python 3.6__ or greater.  
         
-        As with all Python projects, use of a __virtual environment__ is recommended.
-        Instructions for creating a virtual environment using ```conda``` follow.
-        
-        __1.__ Install Anaconda from https://docs.anaconda.com/anaconda/
-        
-        __2.__ Create a virtual environment
-        
-        ```bash
-        conda create -n igvreports python=3.7.1
-        conda activate igvreports
-        ```
         
         #### Installing igv-reports
         
         ```bash
         pip install igv-reports
         ```
         
@@ -67,29 +54,30 @@
             * __--sequence__ INT.   Column of sequence (chromosome) name.
             
         * Optional for generic tab delimited __sites__ file
             * __--zero-based__  Specify that the position in the __sites__ file is 0-based (e.g. UCSC files) rather than 1-based.  Default is ```false```.
         
         * Optional
             * __--genome__ **_New_** An igv.js genome identifier (e.g. hg38).  If supplied fasta, ideogram, and the default annotation track for the specified genome will be used.
+            * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.  Useful when __fasta__ is used to specify the reference.
             * __--tracks__ LIST.  Space-delimited list of track files, see below for supported formats.  If both *tracks* and *track-config* are specified *tracks* will appear first by default.
             * __--track-config__  FILE.  File containing array of json configuration objects for igv.js tracks.  See the [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Tracks-2.0) for more details.  This option allows customization of track parameters.  When using this option, the track ```url``` and ```indexURL``` properties should be set to the paths of the respective files.
-            * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.
+            * __--roi__ LIST.  Space-delimited list of region-of-interest (ROI) files.  See [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Regions-of-Interest).
             * __--template__ FILE. HTML template file.
             * __--output__ FILE. Output file name; default="igvjs_viewer.html".
             * __--info-columns__ LIST. Space delimited list of info field names to include in the variant table.  If __sites__ is a VCF file these are the info ID values.  If __sites__ is a tab delimited format these are column names.
             * __--info-columns-prefixes__ LIST. For VCF based reports only.  Space delimited list of prefixes of VCF info field IDs to include in the variant table.  Any info field with ID starting with one of the listed values will be included.
             * __--samples__ LIST.  Space delimited list of sample (i.e. genotypes) names.  Used in conjunction with __--sample-columns__.
             * __--sample-columns__ LIST. Space delimited list of VCF sample FORMAT field names to include in the variant table.  If __--samples__ is specified columns will be restricted to those samples, otherwise all samples will be included.
             * __--flanking__ INT. Genomic region to include either side of variant; default=1000.
             * __--standalone__ Embed all JavaScript referenced via ```<script>``` tags in the page.
             * __--sort__ Applies to alignment tracks only.  If specified alignments are initally sorted by the specified option. Supported values include  ```BASE, STRAND, INSERT_SIZE, MATE_CHR, and NONE```. Default value is ```BASE``` for single nucleotide variants, ```NONE``` (no sorting) otherwise.  See the igv.js documentation for more information.
             * __--exclude-flags__  INT. Value is passed to samtools as "-F" flag.  Used to filter alignments.  Default value is 1536 which filters alignments marked "duplicate" or "vendor failed". To include all alignments use ```--exclude-flags 0```.  See [samtools documentation](http://www.htslib.org/doc/samtools-view.html) for more details.
             * __--idlink__ URL tempate for information link for VCF ID values.  The token $$ will be substituted with the ID value.  Example: ```--idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$'```
-             
+            * __--no-encode__ Don't embed data.  Fasta and track URLs are embedded unchanged.  The resulting report is depedendent on the original data files, which must be specified as URLs.  Local files are not supported with this option.
         
         **Track file formats:**
         
         Currently supported track file formats are BAM, CRAM, VCF, BED, GFF3, GTF, WIG, and BEDGRAPH.  FASTA. BAM, CRAM, and VCF  
         files must be indexed.  Tabix is supported and it is recommended that all large files be indexed.   
         
         ## Examples
@@ -112,15 +100,15 @@
         
         
         #### Create a variant report from a VCF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_vcf.html))
         
         ```bash
         
         create_report test/data/variants/variants.vcf.gz \
-        http://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
         --ideogram test/data/hg38/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
         --samples reads_1_fastq \
         --sample-columns DP GQ \
         --tracks test/data/variants/variants.vcf.gz test/data/variants/recalibrated.bam test/data/hg38/refGene.txt.gz \
         --output examples/example_vcf.html
@@ -129,89 +117,94 @@
         
         
         
         #### Create a variant report with tracks defined in an [igv.js track config json file](https://github.com/igvteam/igv-reports/tree/master/test/data/variants/trackConfigs.json): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_config.html))
         
         ``` bash
         create_report test/data/variants/variants.vcf.gz \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
         --ideogram test/data/hg38/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
         --track-config test/data/variants/trackConfigs.json \
         --output examples/example_config.html
         ```
         
         
         #### Create a variant report from a TCGA MAF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_maf.html))
         
         ```bash
         
         create_report test/data/variants/tcga_test.maf \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
+        --genome hg19 \
         --flanking 1000 \
         --info-columns Chromosome Start_position End_position Variant_Classification Variant_Type Reference_Allele Tumor_Seq_Allele1 Tumor_Seq_Allele2 dbSNP_RS \
-        --tracks  https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/tcga_test.maf \
         --output examples/example_maf.html
         
         ```
         
         #### Create a variant report from a generic tab-delimited file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_tab.html))
         
         ```bash
         
         create_report test/data/variants/test.maflite.tsv \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
+        --genome hg19 \
         --sequence 1 --begin 2 --end 3 \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns chr start end ref_allele alt_allele \
-        --tracks https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
         --output examples/example_tab.html
         
         ```
-        #### NEW (version 1.5.0) - Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
+        ####  Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
         
         ```bash
         
         create_report test/data/variants/SKBR3_Sniffles_tra.bedpe \
         --genome hg19 \
         --flanking 1000 \
-        --tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam \
         --output examples/example_bedpe.html
         ```
         
         #### Create a variant report with custom ID link urls: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_idlink.html))
         
         ```bash
         
         create_report test/data/variants/1kg_phase3_sites.vcf.gz \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
+        --genome hg19 \
         --flanking 1000 \
-        --tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam \
         --idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$' \
         --output examples/example_idlink.html
         
         ```
         
         #### Create a junction report from a splice-junction bed file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_junctions.html))
         
         ```bash
         create_report test/data/junctions/Introns.38.bed \
-        https://s3.dualstack.us-east-1.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --genome hg38 \
         --type junction \
-        --ideogram test/data/hg38/cytoBandIdeo.txt \
         --track-config test/data/junctions/tracks.json \
         --info-columns TCGA GTEx variant_name \
         --title "Sample A" \
         --output examples/example_junctions.html
         ```
         
+        #### Create a fusion report from a Trinity fusion json file: 
+        
+        ```bash
+        create_report test/data/fusion/igv.fusion_inspector_web.json \
+        --fasta test/data/fusion/igv.genome.fa  \
+        --template igv_reports/templates/fusion_template.html  \  
+        --track-config test/data/fusion/tracks.json  \
+        --output examples/example_fusion.html
+        ```
+        
         #### Create a report containing wig and bedgraph files
         
         ```bash
         create_report test/data/wig/regions.bed \
         --genome hg19 \
         --exclude-flags 512 \
         --tracks test/data/wig/ucsc.bedgraph test/data/wig/mixed_step.wig test/data/wig/variable_step.wig \
@@ -219,31 +212,41 @@
         
         ```
         
         #### Use of ```info-columns-prefixes``` option.  Variant track only, no alignments. ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_ann.html))
         
         
         ```bash
-        create_report test/data/infofields/consensus.filtered.ann.vcf \
+        python igv_reports/report.py test/data/annotated_vcf/consensus.filtered.ann.vcf \
         --genome hg19 \
         --flanking 1000 \
         --info-columns cosmic_gene \
         --info-columns-prefixes clinvar \
-        --tracks test/data/infofields/consensus.filtered.ann.vcf \
-        --output https://igv.org/igv-reports/examples/1.5.1/example_ann.html 
+        --tracks test/data/annotated_vcf/consensus.filtered.ann.vcf \
+        --output examples/example_ann.html 
         ```
         
         #### Use ```--exclude-flags``` option to include duplicate alignments in report.  Default value is 1536 which filters duplicates and vendor-failed reads.
         
         ```bash
         create_report test/data/dups/dups.bed \
         --genome hg19 \
         --exclude-flags 512 \
         --tracks test/data/dups/dups.bam \
         --output examples/example_dups.html
+        ```
+        
+        ### Use ```-no-embed``` option to use external URL references for tracks in the report.  
+        
+        ```bash
+        create_report test/data/variants/variants.vcf.gz \
+        --genome hg38 \
+        --no-embed \
+        --tracks https://igv-genepattern-org.s3.amazonaws.com/test/reports/variants.vcf.gz https://igv-genepattern-org.s3.amazonaws.com/test/reports/recalibrated.bam \
+        --output examples/example_noembed.html
         
         ```
         
         #### Converting genomic files to data URIs for use in igv.js 
         
         The script ```create_datauri``` (```python igv_reports/datauri.py```) converts the contents of a file to a data uri for use in igv.js.   The datauri will be printed to stdout.  *NOTE* It is not neccessary to run this script explicitly to create a report, it is documented here
         for use with stand-alone igv.js.
```

### Comparing `igv-reports-1.7.0/README.md` & `igv-reports-1.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 # igv-reports
 
 A Python application to generate self-contained HTML reports that consist of a table of genomic sites or regions and associated IGV views for each site.
 The generated HTML page contains all data neccessary for IGV as uuencoded blobs. It can be opened within a web browser as a static page, with no depenency on the original input files.
 
-### _NEW - alignments marked "duplicate" are now filtered by default.  See the --exclude-flags option._
-
 ## Installation
 
 #### Prerequisites
 
 igv-reports __requires Python 3.6__ or greater.  
 
-As with all Python projects, use of a __virtual environment__ is recommended.
-Instructions for creating a virtual environment using ```conda``` follow.
-
-__1.__ Install Anaconda from https://docs.anaconda.com/anaconda/
-
-__2.__ Create a virtual environment
-
-```bash
-conda create -n igvreports python=3.7.1
-conda activate igvreports
-```
 
 #### Installing igv-reports
 
 ```bash
 pip install igv-reports
 ```
 
@@ -60,29 +47,30 @@
     * __--sequence__ INT.   Column of sequence (chromosome) name.
     
 * Optional for generic tab delimited __sites__ file
     * __--zero-based__  Specify that the position in the __sites__ file is 0-based (e.g. UCSC files) rather than 1-based.  Default is ```false```.
 
 * Optional
     * __--genome__ **_New_** An igv.js genome identifier (e.g. hg38).  If supplied fasta, ideogram, and the default annotation track for the specified genome will be used.
+    * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.  Useful when __fasta__ is used to specify the reference.
     * __--tracks__ LIST.  Space-delimited list of track files, see below for supported formats.  If both *tracks* and *track-config* are specified *tracks* will appear first by default.
     * __--track-config__  FILE.  File containing array of json configuration objects for igv.js tracks.  See the [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Tracks-2.0) for more details.  This option allows customization of track parameters.  When using this option, the track ```url``` and ```indexURL``` properties should be set to the paths of the respective files.
-    * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.
+    * __--roi__ LIST.  Space-delimited list of region-of-interest (ROI) files.  See [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Regions-of-Interest).
     * __--template__ FILE. HTML template file.
     * __--output__ FILE. Output file name; default="igvjs_viewer.html".
     * __--info-columns__ LIST. Space delimited list of info field names to include in the variant table.  If __sites__ is a VCF file these are the info ID values.  If __sites__ is a tab delimited format these are column names.
     * __--info-columns-prefixes__ LIST. For VCF based reports only.  Space delimited list of prefixes of VCF info field IDs to include in the variant table.  Any info field with ID starting with one of the listed values will be included.
     * __--samples__ LIST.  Space delimited list of sample (i.e. genotypes) names.  Used in conjunction with __--sample-columns__.
     * __--sample-columns__ LIST. Space delimited list of VCF sample FORMAT field names to include in the variant table.  If __--samples__ is specified columns will be restricted to those samples, otherwise all samples will be included.
     * __--flanking__ INT. Genomic region to include either side of variant; default=1000.
     * __--standalone__ Embed all JavaScript referenced via ```<script>``` tags in the page.
     * __--sort__ Applies to alignment tracks only.  If specified alignments are initally sorted by the specified option. Supported values include  ```BASE, STRAND, INSERT_SIZE, MATE_CHR, and NONE```. Default value is ```BASE``` for single nucleotide variants, ```NONE``` (no sorting) otherwise.  See the igv.js documentation for more information.
     * __--exclude-flags__  INT. Value is passed to samtools as "-F" flag.  Used to filter alignments.  Default value is 1536 which filters alignments marked "duplicate" or "vendor failed". To include all alignments use ```--exclude-flags 0```.  See [samtools documentation](http://www.htslib.org/doc/samtools-view.html) for more details.
     * __--idlink__ URL tempate for information link for VCF ID values.  The token $$ will be substituted with the ID value.  Example: ```--idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$'```
-     
+    * __--no-encode__ Don't embed data.  Fasta and track URLs are embedded unchanged.  The resulting report is depedendent on the original data files, which must be specified as URLs.  Local files are not supported with this option.
 
 **Track file formats:**
 
 Currently supported track file formats are BAM, CRAM, VCF, BED, GFF3, GTF, WIG, and BEDGRAPH.  FASTA. BAM, CRAM, and VCF  
 files must be indexed.  Tabix is supported and it is recommended that all large files be indexed.   
 
 ## Examples
@@ -105,15 +93,15 @@
 
 
 #### Create a variant report from a VCF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_vcf.html))
 
 ```bash
 
 create_report test/data/variants/variants.vcf.gz \
-http://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+--fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
 --ideogram test/data/hg38/cytoBandIdeo.txt \
 --flanking 1000 \
 --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
 --samples reads_1_fastq \
 --sample-columns DP GQ \
 --tracks test/data/variants/variants.vcf.gz test/data/variants/recalibrated.bam test/data/hg38/refGene.txt.gz \
 --output examples/example_vcf.html
@@ -122,89 +110,94 @@
 
 
 
 #### Create a variant report with tracks defined in an [igv.js track config json file](https://github.com/igvteam/igv-reports/tree/master/test/data/variants/trackConfigs.json): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_config.html))
 
 ``` bash
 create_report test/data/variants/variants.vcf.gz \
-https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+--fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
 --ideogram test/data/hg38/cytoBandIdeo.txt \
 --flanking 1000 \
 --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
 --track-config test/data/variants/trackConfigs.json \
 --output examples/example_config.html
 ```
 
 
 #### Create a variant report from a TCGA MAF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_maf.html))
 
 ```bash
 
 create_report test/data/variants/tcga_test.maf \
-https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
---ideogram test/data/hg19/cytoBandIdeo.txt \
+--genome hg19 \
 --flanking 1000 \
 --info-columns Chromosome Start_position End_position Variant_Classification Variant_Type Reference_Allele Tumor_Seq_Allele1 Tumor_Seq_Allele2 dbSNP_RS \
---tracks  https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+--tracks test/data/variants/tcga_test.maf \
 --output examples/example_maf.html
 
 ```
 
 #### Create a variant report from a generic tab-delimited file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_tab.html))
 
 ```bash
 
 create_report test/data/variants/test.maflite.tsv \
-https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
+--genome hg19 \
 --sequence 1 --begin 2 --end 3 \
---ideogram test/data/hg19/cytoBandIdeo.txt \
 --flanking 1000 \
 --info-columns chr start end ref_allele alt_allele \
---tracks https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
 --output examples/example_tab.html
 
 ```
-#### NEW (version 1.5.0) - Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
+####  Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
 
 ```bash
 
 create_report test/data/variants/SKBR3_Sniffles_tra.bedpe \
 --genome hg19 \
 --flanking 1000 \
---tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+--tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam \
 --output examples/example_bedpe.html
 ```
 
 #### Create a variant report with custom ID link urls: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_idlink.html))
 
 ```bash
 
 create_report test/data/variants/1kg_phase3_sites.vcf.gz \
-https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
---ideogram test/data/hg19/cytoBandIdeo.txt \
+--genome hg19 \
 --flanking 1000 \
---tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+--tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam \
 --idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$' \
 --output examples/example_idlink.html
 
 ```
 
 #### Create a junction report from a splice-junction bed file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_junctions.html))
 
 ```bash
 create_report test/data/junctions/Introns.38.bed \
-https://s3.dualstack.us-east-1.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+--genome hg38 \
 --type junction \
---ideogram test/data/hg38/cytoBandIdeo.txt \
 --track-config test/data/junctions/tracks.json \
 --info-columns TCGA GTEx variant_name \
 --title "Sample A" \
 --output examples/example_junctions.html
 ```
 
+#### Create a fusion report from a Trinity fusion json file: 
+
+```bash
+create_report test/data/fusion/igv.fusion_inspector_web.json \
+--fasta test/data/fusion/igv.genome.fa  \
+--template igv_reports/templates/fusion_template.html  \  
+--track-config test/data/fusion/tracks.json  \
+--output examples/example_fusion.html
+```
+
 #### Create a report containing wig and bedgraph files
 
 ```bash
 create_report test/data/wig/regions.bed \
 --genome hg19 \
 --exclude-flags 512 \
 --tracks test/data/wig/ucsc.bedgraph test/data/wig/mixed_step.wig test/data/wig/variable_step.wig \
@@ -212,31 +205,41 @@
 
 ```
 
 #### Use of ```info-columns-prefixes``` option.  Variant track only, no alignments. ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_ann.html))
 
 
 ```bash
-create_report test/data/infofields/consensus.filtered.ann.vcf \
+python igv_reports/report.py test/data/annotated_vcf/consensus.filtered.ann.vcf \
 --genome hg19 \
 --flanking 1000 \
 --info-columns cosmic_gene \
 --info-columns-prefixes clinvar \
---tracks test/data/infofields/consensus.filtered.ann.vcf \
---output https://igv.org/igv-reports/examples/1.5.1/example_ann.html 
+--tracks test/data/annotated_vcf/consensus.filtered.ann.vcf \
+--output examples/example_ann.html 
 ```
 
 #### Use ```--exclude-flags``` option to include duplicate alignments in report.  Default value is 1536 which filters duplicates and vendor-failed reads.
 
 ```bash
 create_report test/data/dups/dups.bed \
 --genome hg19 \
 --exclude-flags 512 \
 --tracks test/data/dups/dups.bam \
 --output examples/example_dups.html
+```
+
+### Use ```-no-embed``` option to use external URL references for tracks in the report.  
+
+```bash
+create_report test/data/variants/variants.vcf.gz \
+--genome hg38 \
+--no-embed \
+--tracks https://igv-genepattern-org.s3.amazonaws.com/test/reports/variants.vcf.gz https://igv-genepattern-org.s3.amazonaws.com/test/reports/recalibrated.bam \
+--output examples/example_noembed.html
 
 ```
 
 #### Converting genomic files to data URIs for use in igv.js 
 
 The script ```create_datauri``` (```python igv_reports/datauri.py```) converts the contents of a file to a data uri for use in igv.js.   The datauri will be printed to stdout.  *NOTE* It is not neccessary to run this script explicitly to create a report, it is documented here
 for use with stand-alone igv.js.
```

### Comparing `igv-reports-1.7.0/igv_reports/bam.py` & `igv-reports-1.8.0/igv_reports/bam.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,18 @@
                 samargs.append("-F")
                 samargs.append(str(self.args.exclude_flags))
         else:
             samargs.append("-F")
             samargs.append("1536")
 
         if region:
-            range_string = self.get_chrname(region['chr']) + ":" + str(region['start']) + "-" + str(region['end'])
+            if region['start'] is not None:
+                range_string = self.get_chrname(region['chr']) + ":" + str(region['start']) + "-" + str(region['end'])
+            else:
+                range_string = self.get_chrname(region['chr'])
             samargs.append(range_string)
         if region2:
             range_string = self.get_chrname(region2['chr']) + ":" + str(region2['start']) + "-" + str(region2['end'])
             samargs.append(range_string)
 
         return pysam.view(*samargs)
```

### Comparing `igv-reports-1.7.0/igv_reports/bedtable.py` & `igv-reports-1.8.0/igv_reports/bedtable.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/chralias.py` & `igv-reports-1.8.0/igv_reports/chralias.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/datauri.py` & `igv-reports-1.8.0/igv_reports/datauri.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/fasta.py` & `igv-reports-1.8.0/igv_reports/fasta.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,32 +23,31 @@
 
         fasta.close()
 
         return slice_seq
 
 class FastaReader:
 
-    def __init__(self, path):
-
-        self.fasta = pysam.FastaFile(path)
+    def __init__(self, file):
+        self.fasta = pysam.FastaFile(file)
 
     def slice(self, region = None):
 
         if None == region:
             with open(self.fasta,"r") as f:
                 return(f.read())
 
         else :
 
             if isinstance(region,str):
                 region = regions.parse_region(region)
 
             chr = region["chr"]
-            start = region["start"] - 1
-            end = region["end"]
+            start = region["start"] - 1 if region["start"] is not None else None
+            end = region["end"] if region["end"] is not None else None
 
             try:
                 seq = self.fasta.fetch(chr, start, end)
 
 
             except KeyError:
                 chr = "chr" + chr
```

### Comparing `igv-reports-1.7.0/igv_reports/feature.py` & `igv-reports-1.8.0/igv_reports/feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -234,14 +234,18 @@
             return parse_bedpe(f, reader)
         elif format == 'refgene':
             return parse_refgene(f, reader)
         elif format == 'bedgraph':
             return parse_bedgraph(f, reader)
         elif format == 'tab':
             return parse_tab(f, reader)
+        elif format == 'maf':
+            return parse_maf(f, reader)
+        elif format == 'mut':
+            return parse_mut(f, reader)
         else:
             raise Exception("Unknown file format: " + path)
     finally:
         if f:
             f.close()
 
 
@@ -251,14 +255,16 @@
         if line.startswith("track") and reader is not None:
             reader.trackline = line
         elif not (line.startswith('#') or line.startswith('track') or line.startswith('browser')):
             tokens = line.rstrip('\n').rstrip('\r').split('\t')
             if len(tokens) >= 3:
                 chr = tokens[0]
                 start = int(tokens[1])
+                if start < 0:
+                    continue
                 end = int(tokens[2])
                 name = tokens[3] if len(tokens) > 3 else ''
                 features.append(Feature(chr, start, end, line, name))
     return features
 
 def parse_bedgraph(f, reader=None):
     features = []
@@ -336,14 +342,51 @@
             reader.trackline = line
         elif not (line.startswith('#') or line.startswith('track') or line.startswith('browser')):
             tokens = line.rstrip('\n').rstrip('\r').split('\t')
             if len(tokens) > 2:
                 rows.append(tokens)
     return rows
 
+def parse_mut(f, reader=None):
+    firstline = True
+    features = []
+    for line in f:
+        if not line.startswith('#'):
+            if firstline:
+                reader.trackline = line
+                firstline = False
+            else:
+                tokens = line.rstrip('\n').rstrip('\r').split('\t')
+                if len(tokens) >= 3:
+                    chr = tokens[0]
+                    start = int(tokens[1]) - 1
+                    end = int(tokens[2])
+                    name = ''
+                    features.append(Feature(chr, start, end, line, name))
+
+    return features
+
+def parse_maf(f, reader=None):
+    firstline = True
+    features = []
+    for line in f:
+        if not line.startswith('#'):
+            if firstline:
+                reader.trackline = line
+                firstline = False
+            else:
+                tokens = line.rstrip('\n').rstrip('\r').split('\t')
+                if len(tokens) >= 6:
+                    chr = tokens[4]
+                    start = int(tokens[5]) - 1
+                    end = int(tokens[6])
+                    name =  ''
+                    features.append(Feature(chr, start, end, line, name))
+    return features
+
 
 def infer_format(filename):
     '''
     Infer the genomic file format from the filename.  First known formats are checked.  Next presenece of
     the magic string "refgene" in the filename is checked for UCSC refgene files.  This is a legacy
     IGV convention.  The order is important, a recognized extension wins.
     NOTE: Formats are for output data uris.  CRAM format is converted to BAM before output.
@@ -368,14 +411,18 @@
         return "gff"
     elif filename.endswith(".gtf"):
         return "gtf"
     elif filename.endswith(".wig"):
         return "wig"
     elif filename.endswith(".bedgraph"):
         return "bedgraph"
+    elif filename.endswith(".maf"):
+        return "maf"
+    elif filename.endswith(".mut"):
+        return "mut"
     elif filename.find("refgene"):
         return "refgene"
     else:
         idx = filename.rfind(".")
         if idx > 0:
             return filename[idx + 1:]
         else:
```

### Comparing `igv-reports-1.7.0/igv_reports/featureTree.py` & `igv-reports-1.8.0/igv_reports/featureTree.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/genome.py` & `igv-reports-1.8.0/igv_reports/genome.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/ideogram.py` & `igv-reports-1.8.0/igv_reports/ideogram.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/regions.py` & `igv-reports-1.8.0/igv_reports/regions.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/report.py` & `igv-reports-1.8.0/igv_reports/report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 import sys
 import json
 import math
 import argparse
 from urllib.request import urlopen
-from igv_reports import datauri, tracks, utils
+from igv_reports import datauri, tracks, utils, feature
 from igv_reports.varianttable import VariantTable
 from igv_reports.bedtable import BedTable
 from igv_reports.bedtable import BedpeTable
 from igv_reports.bedtable import JunctionBedTable
 from igv_reports.generictable import GenericTable
 from igv_reports.regions import parse_region
-from igv_reports.feature import MockReader
 from igv_reports.fasta import FastaReader
 from igv_reports.ideogram import IdeogramReader
 from igv_reports.genome import get_genome
+from igv_reports.tracks import get_track_type
+from igv_reports.stream import resource_exists
+from igv_reports.utils import resolve_relative_path
 
 '''
 Create an html report.  This is the main function for the application.
 '''
+
+
 def create_report(args):
 
-    trackconfigs = []
-    trackreaders = []
-    session_dict = {}
+    # Read the variant data -- this populates the variant table and defines the corresponding regions
 
-    # Read the variant data
     variants_file = args.sites
 
     if variants_file.endswith(".bcf") or variants_file.endswith(".vcf") or variants_file.endswith(".vcf.gz"):
         table = VariantTable(variants_file, args.info_columns, args.info_columns_prefixes, args.samples,
                              args.sample_columns, args.idlink)
 
     elif variants_file.endswith(".bed") or variants_file.endswith(".bed.gz"):
@@ -39,72 +40,159 @@
             table = BedTable(variants_file)
 
     elif variants_file.endswith(".bedpe") or variants_file.endswith(".bedpe.gz"):
         table = BedpeTable(variants_file)
 
     elif variants_file.endswith(".maf") or variants_file.endswith(".maf.gz") or (
             args.sequence is not None and args.begin is not None and args.end is not None):
-        # A hack -- since these file formats are not supported by igv.js mock up a bed style track from a table of generic features
-        table = GenericTable(variants_file, args.info_columns, args.sequence, args.begin, args.end, args.zero_based)
-        flist = []
-        for tuple in table.features:
-            flist.append(tuple[0])
-        trackconfigs.append({
-            "config": {"name": "variants", "type": "annotation", "format": "bed"},
-            "reader": MockReader(flist)
-        })
+        table = GenericTable.from_tabfile(variants_file, args.info_columns, args.sequence, args.begin, args.end, args.zero_based)
+
+    elif variants_file.endswith(".json"):
+        table = GenericTable.from_fusionjson(variants_file)
 
     # Track json array.  Tracks can come from (1) tracks CL argument, (2) genome CL argument, and (3) track_config Cl argument
     trackjson = []
 
     # Check for optional genome argument.  If supplied an igv.js genome json definition is used in lieu of a fasta file
     if args.genome is not None:
         genome = get_genome(args.genome)
         if args.fasta is None:
             args.fasta = genome["fastaURL"]
         if args.ideogram is None and "cytobandURL" in genome:
             args.ideogram = genome["cytobandURL"]
         if "tracks" in genome:
             for config in genome["tracks"]:
+                if "format" not in config and "url in c":
+                    config["format"] = feature.infer_format(config["url"])
+                if "type" not in config:
+                    config["type"] = get_track_type(config["format"])
+
+                # Add potential index references
+
                 trackjson.append(config)
 
+    # --tracks argument
     if args.tracks is not None:
         for track in args.tracks:
-           trackjson.append(tracks.get_track_json_dict(track))
+            config = tracks.get_track_json_dict(track)
+            # If this is a no-embed report add index URLs
+            if args.no_embed == True:
+                add_index(config)
+            trackjson.append(config)
+
+    # --roi argument
+    if args.roi is not None:
+        for track in args.roi:
+            config = tracks.get_track_json_dict(track)
+            config["type"] = "roi"
+            # If this is a no-embed report add index URLs
+            if args.no_embed == True:
+                add_index(config)
+            trackjson.append(config)
 
+    # --track_config argument
     if args.track_config is not None:
         for trackobj in args.track_config:
             with open(trackobj) as f:
                 j = json.load(f)
-                for c in j:
-                    trackjson.append(c)
+                for config in j:
+                    if "url" in config:
+                        config["url"] = resolve_relative_path(trackobj, config["url"])
+                    if "format" not in config and "url" in config:
+                        config["format"] = feature.infer_format(config["url"])
+                    if "type" not in config:
+                        config["type"] = get_track_type(config["format"])
+                    trackjson.append(config)
+
+    if args.no_embed == True:
+        igv_config = json.dumps(create_noembed_session(args, trackjson))
+        locus_dict = json.dumps(create_locus_dict(table))
 
-    # Create file readers for tracks.  This is done outside the locus loop so initialization happens once
+    # Create the session dictionary json, containing a session object for each variant
+    else:
+        session_dict = json.dumps(create_session_dict(args, table, trackjson))
+
+    # Generate the HTML
+    template_file = args.template
+    if None == template_file:
+        if 'junction' == args.type:
+            template_file = os.path.dirname(sys.modules['igv_reports'].__file__) + '/templates/junction_template.html'
+        elif 'fusion' == args.type:
+            template_file = os.path.dirname(sys.modules['igv_reports'].__file__) + '/templates/fusion_template.html'
+        elif args.no_embed == True:
+            template_file = os.path.dirname(
+                sys.modules['igv_reports'].__file__) + '/templates/variant_template-noembed.html'
+        else:
+            template_file = os.path.dirname(sys.modules['igv_reports'].__file__) + '/templates/variant_template.html'
+
+    output_file = args.output
+
+    standalone = args.standalone
+    with open(template_file, "r") as f:
+        data = f.readlines()
+
+        with open(output_file, "w") as o:
+
+            for i, line in enumerate(data):
+
+                if args.title is not None and line.startswith("<!--title-->"):
+                    o.write("<h1>" + args.title + "</h1>")
+
+                if standalone:
+                    if line.strip().startswith("<script") and ".js\"" in line:
+                        inline_script(line, o, "js")
+                        continue
+                    elif line.strip().startswith("<link") and line.strip().endswith("css\">"):
+                        inline_script(line, o, "css")
+                        continue
+                j = line.find('"@TABLE_JSON@"')
+                if j >= 0:
+                    line = line.replace('"@TABLE_JSON@"', table.to_JSON())
+
+                j = line.find('"@SESSION_DICTIONARY@"')
+                if j >= 0:
+                    line = line.replace('"@SESSION_DICTIONARY@"', session_dict)
+
+                j = line.find('"@LOCUS_DICTIONARY@"')
+                if j >= 0:
+                    line = line.replace('"@LOCUS_DICTIONARY@"', locus_dict)
+
+                j = line.find('"@IGV_CONFIG@"')
+                if j >= 0:
+                    line = line.replace('"@IGV_CONFIG@"', igv_config)
+
+                sort_option = args.sort.upper() if args.sort is not None else "BASE"
+                j = line.find('"@SORT@"')
+                if j >= 0:
+                    line = line.replace('"@SORT@"', '"' + sort_option + '"')
+
+                o.write(line)
 
-    for config in trackjson:
-        reader = utils.getreader(config, None, args)
-        trackconfigs.append({
-            "config": config,
-            "reader": reader
-        })
 
+# Create a dictionary of igv.js session objects, one for each variant
+def create_session_dict(args, table, trackjson):
 
+    session_dict = {}
+
+    # Create file readers for tracks.  This is done outside the locus loop so initialization happens once
+    readers = []
+    for config in trackjson:
+        readers.append(utils.getreader(config, None, args))
 
     # Other readers
     fasta_reader = FastaReader(args.fasta)
     if (args.ideogram):
         ideogram_reader = IdeogramReader(args.ideogram)
     else:
         ideogram_reader = None
 
     # loop through regions defined from variant, annotation, or bedpe files,  creating an igv.js session for each one
     flanking = 0
     if args.flanking is not None:
         flanking = float(args.flanking)
-
     i = 0
     for tuple in table.features:
         i += 1
         print(f"Working on variant {i}/{len(table.features)}")
 
         feature = tuple[0]
         unique_id = tuple[1]
@@ -124,34 +212,31 @@
             if hasattr(feature, "viewport"):
                 region = parse_region(feature.viewport)
                 chr = region["chr"]
                 start = region["start"]
                 end = region["end"]
             else:
                 chr = feature.chr
-                start = int(math.floor(feature.start - flanking / 2))
-                start = max(start, 1)  # bound start to 1
-                end = int(math.ceil(feature.end + flanking / 2))
-                region = {
-                    "chr": chr,
-                    "start": start,
-                    "end": end
-                }
+
+                if feature.start is not None:
+                    start = int(math.floor(feature.start - flanking / 2))
+                    start = max(start, 1)  # bound start to 1
+                else:
+                    start = None
+                end = int(math.ceil(feature.end + flanking / 2)) if feature.end is not None else None
+
+                region = {"chr": chr, "start": start, "end": end}
 
                 # If feature has a second locus (bedpe file) create the region here.
                 if hasattr(feature, 'chr2') and feature.chr2 is not None:
                     chr2 = feature.chr2
                     start2 = int(math.floor(feature.start2 - flanking / 2))
                     start2 = max(start2, 1)  # bound start to 1
                     end2 = int(math.ceil(feature.end2 + flanking / 2))
-                    region2 = {
-                        "chr": chr2,
-                        "start": start2,
-                        "end": end2
-                    }
+                    region2 = {"chr": chr2, "start": start2, "end": end2}
 
             # Fasta
             data = fasta_reader.slice(region)
             fa = '>' + chr + ':' + str(start) + '-' + str(end) + '\n' + data
 
             if region2 is not None:
                 data2 = fasta_reader.slice(region2)
@@ -174,110 +259,134 @@
             if (hasattr(feature, "viewport")):
                 initial_locus = feature.viewport
             else:
                 initial_locus = locus_string(feature.chr, feature.start, feature.end)
                 if region2 is not None:
                     initial_locus += f' {locus_string(feature.chr2, feature.start2, feature.end2)}'
 
-            session_json = {
-                "locus": initial_locus,
-                "reference": fastaJson,
-                "tracks": []
-            }
 
-            track_objects = []
-            # Loop through user supplied track configs
-            # "cram" input format is converted to "bam" for output track configs
-            for tc in trackconfigs:
-                trackobj = tc["config"];
-
-                # Set some defaults if not specified
-                if "url" in trackobj:
-                    default_trackobj = tracks.get_track_json_dict(trackobj["url"]);
-                    if "type" not in trackobj:
-                        trackobj["type"] = default_trackobj["type"]
-                    if "format" not in trackobj:
-                        trackobj["format"] = default_trackobj["format"]
-                    if trackobj["format"] == "cram":
-                        trackobj["format"] = "bam"
-                    if "name" not in trackobj:
-                        trackobj["name"] = default_trackobj["url"]
+            # Loop through track configs
+            tracks = []
+            roi = []
+            track_order = 1
+            idx = 0
+            for config in trackjson:
+
+                reader = readers[idx]
+                idx += 1
+
+                # "cram" input format is converted to "bam" for output track configs
+                if config["format"] == "cram":
+                    config["format"] = "bam"
+
+                if config["format"] == "bcf":
+                    config["format"] == "vcf"
 
                 # Indexes are not used with data URIs
-                if "indexURL" in trackobj:
-                    del trackobj["indexURL"]
+                if "indexURL" in config:
+                    del config["indexURL"]
 
-                reader = tc["reader"]
                 data = reader.slice(region, region2)
-                trackobj["url"] = datauri.get_data_uri(data)
-                track_objects.append(trackobj)
 
-            track_order = 1
-            for trackobj in track_objects:
-                if (trackobj["type"] == "alignment"):
-                    trackobj["height"] = 500
-                    is_snv = feature.end - feature.start == 1
-                    if (trackobj["type"]) == "alignment" and (args.sort is not None or is_snv) and (
+                # replace url with data URI
+                config["url"] = datauri.get_data_uri(data)
+
+                if (config["type"] == "alignment"):
+                    if "height" not in config:
+                        config["height"] = 500
+                        
+                    is_snv = feature.end is not None and feature.end - feature.start == 1
+                    
+                    if (config["type"]) == "alignment" and (args.sort is not None or is_snv) and (
                             args.sort != 'NONE'):
                         sort_option = 'BASE' if args.sort is None else args.sort.upper()
-                        trackobj["sort"] = {
+                        config["sort"] = {
                             "option": sort_option,
                             "chr": chr,
                             "position": str(feature.start + 1),
                             "direction": "ASC"
                         }
-                if "order" not in trackobj:
-                    trackobj["order"] = track_order
-                session_json["tracks"].append(trackobj)
+                if "order" not in config:
+                    config["order"] = track_order
                 track_order += 1
 
-            # Build the session data URI
+                if "roi" == config["type"]:
+                    roi.append(config)
+                else:
+                    tracks.append(config)
 
+            session_json = {
+                "locus": initial_locus,
+                "reference": fastaJson,
+                "tracks": tracks
+            }
+            if len(roi) > 0:
+                session_json["roi"] = roi
+
+            # Build the session data URI
             session_string = json.dumps(session_json)
             session_uri = datauri.get_data_uri(session_string)
             session_dict[session_id] = session_uri
 
-    session_dict = json.dumps(session_dict)
+    return session_dict
 
-    template_file = args.template
-    if None == template_file:
-        if 'junction' == args.type:
-            template_file = os.path.dirname(sys.modules['igv_reports'].__file__) + '/templates/junction_template.html'
+
+# Create an igv session config object.  This is used for no-embed reports
+def create_noembed_session(args, trackjson):
+    reference = {
+        "fastaURL": args.fasta,
+    }
+    if resource_exists(args.fasta + ".fai"):
+        reference["indexURL"] = args.fasta + ".fai"
+
+    if args.ideogram is not None:
+        reference["cytobandURL"] = args.ideogram
+
+    tracks = []
+    roi = []
+    for tj in trackjson:
+        if "roi" == tj["type"]:
+            roi.append(tj)
         else:
-            template_file = os.path.dirname(sys.modules['igv_reports'].__file__) + '/templates/variant_template-2.html'
+            tracks.append(tj)
+    session = {
+        "reference": reference,
+        "tracks": tracks
+    }
+    if len(roi) > 0:
+        session["roi"] = roi
 
-    output_file = args.output
+    return session
 
-    standalone = args.standalone
-    with open(template_file, "r") as f:
-        data = f.readlines()
 
-        with open(output_file, "w") as o:
+def create_locus_dict(table):
+    locus_dict = {}
 
-            for i, line in enumerate(data):
+    # loop through regions defined from variant, annotation, or bedpe files,  creating  locus for each one
 
-                if args.title is not None and line.startswith("<!--title-->"):
-                    o.write("<h1>" + args.title + "</h1>")
+    for tuple in table.features:
 
-                if standalone:
-                    if line.strip().startswith("<script") and ".js\"" in line:
-                        inline_script(line, o, "js")
-                        continue
-                    elif line.strip().startswith("<link") and line.strip().endswith("css\">"):
-                        inline_script(line, o, "css")
-                        continue
-                j = line.find('"@TABLE_JSON@"')
-                if j >= 0:
-                    line = line.replace('"@TABLE_JSON@"', table.to_JSON())
+        feature = tuple[0]
+        unique_id = tuple[1]
 
-                j = line.find('"@SESSION_DICTIONARY@"')
-                if j >= 0:
-                    line = line.replace('"@SESSION_DICTIONARY@"', session_dict)
+        if hasattr(feature, "session_id"):
+            session_id = feature.session_id
+        else:
+            session_id = str(unique_id)
 
-                o.write(line)
+        if (hasattr(feature, "viewport")):
+            locus = feature.viewport
+        else:
+            locus = locus_string(feature.chr, feature.start + 1, feature.end)
+            if hasattr(feature, 'chr2') and feature.chr2 is not None:
+                locus += f' {locus_string(feature.chr2, feature.start2, feature.end2)}'
+
+        locus_dict[session_id] = locus
+
+    return locus_dict
 
 
 def inline_script(line, o, source_type):
     # <script type="text/javascript" src="https://igv.org/web/test/dist/igv.min.js"></script>
     if source_type == "js":
         s = line.find('src="')
         offset = 5
@@ -300,29 +409,73 @@
         else:
             o.write('</style>\n')
     else:
         raise ValueError("No file path in {l} for inline script.".format(l=line))
 
 
 def locus_string(chr, start, end):
+    if start is None:
+        return chr
+
     if (end - start) == 1:
         return f'{chr}:{start + 1}'
     else:
         return f'{chr}:{start + 1}-{end}'
 
 
+# Potentially add an index URL to a track config.  The "format" field must be set before calling this function
+def add_index(config):
+    if "url" not in config or "indexURL" in config:
+        return
+
+    indexURL = None
+    url = config["url"]
+
+    # Check tabix first
+    if url.endswith(".gz"):
+        if resource_exists(url + ".tbi"):
+            indexURL = url + ".tbi"
+        elif resource_exists(url + ".csi"):
+            indexURL = url + ".csi"
+
+    # Check potential bam/cram files
+    if "format" in config:
+        format = config["format"]
+        if format == "bam" or format == "cram":
+            if resource_exists(url + ".bai"):
+                indexURL = url + ".bai"
+            elif resource_exists(format + ".csi"):
+                indexURL = url + ".csi"
+            else:
+                k = url.rfind(".")
+                tmp = url[:k] + ".bai"
+                if resource_exists(tmp):
+                    indexURL = tmp
+        elif format == "cram" and indexURL == None:
+            if (resource_exists(url + ".crai")):
+                indexURL = url + ".crai"
+
+    if indexURL is not None:
+        config["indexURL"] = indexURL
+
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("sites", help="vcf file defining variants, required")
-    parser.add_argument("fasta", nargs="?", default=None, help="reference fasta file, required if --genome is not specified")
-    parser.add_argument("--genome",  help="igv.js genome id (e.g. hg38)")
-    parser.add_argument("--type", help="Report type.  Possible values are mutation and junctions.  Default is mutation")
+    parser.add_argument("fasta_", nargs="?", default=None,
+                        help="reference fasta file.  Deprecated positional argument,  use --fasta")
+    parser.add_argument("--fasta", nargs="?", default=None,
+                        help="reference fasta file, required if --genome is not specified")
+    parser.add_argument("--genome", help="igv.js genome id (e.g. hg38)")
+
+    parser.add_argument("--type", help="Report type.  Possible values are mutation, junction, and fusion.  Default is mutation")
     parser.add_argument("--ideogram", help="ideogram file in UCSC cytoIdeo format")
     parser.add_argument("--tracks", nargs="+", help="list of track files")
     parser.add_argument("--track-config", nargs="+", help="track json file")
+    parser.add_argument("--roi", nargs="+", help="list of region-of-interest files")
     parser.add_argument("--sort",
                         help="initial sort option for alignment tracks.   Supported values include  BASE, STRAND, INSERT_SIZE, and MATE_CHR. Default value is BASE for single nucleotide variants, no sorting otherwise.  See the igv.js documentation for more information. ")
     parser.add_argument("--template", help="html template file", default=None)
     parser.add_argument("--output", help="output file name", default="igvjs_viewer.html")
     parser.add_argument("--info-columns", nargs="+", help="list of VCF info field names to include in variant table")
     parser.add_argument("--info-columns-prefixes", nargs="+",
                         help="list of prefixes of VCF info field names to include in variant table")
@@ -337,14 +490,20 @@
                         default=None)
     parser.add_argument("--begin", help="Column of start position.  For tab-delimited sites file.", default=None)
     parser.add_argument("--end", help="column of end position. For tab-delimited sites file.", default=None)
     parser.add_argument("--zero_based",
                         help="Specify that the position in the data file is 0-based (e.g. UCSC files) rather than 1-based.",
                         default=None)
     parser.add_argument("--idlink", type=str, help="url link template for the VCF ID column")
-    parser.add_argument("--exclude-flags", type=int, help="Passed to samtools to filter alignments.  For BAM and CRAM files.", default=1536)
+    parser.add_argument("--exclude-flags", type=int,
+                        help="Passed to samtools to filter alignments.  For BAM and CRAM files.", default=1536)
+    parser.add_argument("--no-embed", help="Do not embed fasta or track data.  This is not common", action="store_true")
     args = parser.parse_args()
+
+    # For backward compatibility with 'fasta' positional argument
+    if args.fasta_ is not None and args.fasta is None:
+        args.fasta = args.fasta_
     create_report(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `igv-reports-1.7.0/igv_reports/templates/junction_template.html` & `igv-reports-1.8.0/igv_reports/templates/junction_template.html`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     <meta http-equiv="Expires" content="0"/>
     <meta charset="utf-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
     <meta name="description" content="">
     <meta name="author" content="">
 
-    <title>IGV Variant Inspector </title>
+    <title>IGV Junction Inspector </title>
 
     <!-- igv -->
-    <script src="https://cdn.jsdelivr.net/npm/igv@2.13.11/dist/igv.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/igv@2.15.9/dist/igv.min.js"></script>
 
     <style type="text/css">
         body {
             font-size: 80%;
             font-family: 'Lucida Grande', Verdana, Arial, Sans-Serif;
         }
     </style>
```

### Comparing `igv-reports-1.7.0/igv_reports/templates/variant_template-2.html` & `igv-reports-1.8.0/igv_reports/templates/variant_template.html`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
     <meta name="description" content="">
     <meta name="author" content="">
 
     <title>IGV Variant Inspector </title>
 
     <!-- igv -->
-    <script src="https://cdn.jsdelivr.net/npm/igv@2.13.11/dist/igv.min.js"></script>
-
+    <script src="https://cdn.jsdelivr.net/npm/igv@2.15.9/dist/igv.min.js"></script>
 
     <style type="text/css">
         body {
             font-size: 80%;
             font-family: 'Lucida Grande', Verdana, Arial, Sans-Serif;
         }
 
@@ -137,89 +136,99 @@
     </style>
 
 </head>
 
 <body>
 
 
+<!--title-->
+
 <div id="tableContainer" class="wrap-collabsible">
     <input id="collapsible" class="toggle" type="checkbox" checked>
     <label for="collapsible" class="lbl-toggle">Variants</label>
     <div class="collapsible-content">
         <div id="tableSelectorDiv"></div>
     </div>
 </div>
 
 <div id="igvContainer">
     <div id="igvDiv"></div>
 </div>
 
 <!--
-Uncomment for local debugging.  "igv.js" is a soft link to the local igv.js repository
+Remove igv.js script tag in header and uncomment for local debugging.  "igv.js" is the root directory of a  local
+igv.js repository.  Adjust path as neccessary
+
+
 <script type="module">
       import igv from "./igv.js/js/index.js";
 -->
 
 <script type="text/javascript">
 
-    var tableJson = "@TABLE_JSON@"
-    var igvBrowser;
-    var sessionDictionary = "@SESSION_DICTIONARY@"
+    const tableJson = "@TABLE_JSON@"
+    const sessionDictionary = "@SESSION_DICTIONARY@"
+    let igvBrowser;
 
     document.addEventListener("DOMContentLoaded", function () {
         initIGV();
     });
 
 
-    function initIGV() {
 
-        var igvDiv;
+    /**
+     * Create the igv instance initialized with the first session in the session dictionary.  This will correspond
+     * to the first variant in the variant table. *
+     */
+    function initIGV() {
 
-        igvDiv = document.getElementById("igvDiv");
-        var options =
+        const igvDiv = document.getElementById("igvDiv");
+        const options =
             {
                 sessionURL: sessionDictionary["0"],
-                showChromosomeWidget: false,
+                showChromosomeWidget: false,  // The session for each variant contains data and sequence for that variant only
                 showCenterGuide: true,
                 search: false     // disable webservice search
             };
 
         igv.createBrowser(igvDiv, options)
             .then(function (b) {
                 igvBrowser = b;
                 initTable();
             })
     }
 
     function initTable() {
 
+        // table
         const table = document.createElement("table");
         table.id = "variant_table"
         table.style.width = "100%";
-
         document.getElementById("tableSelectorDiv").appendChild(table);
 
+        // header
         const thead = document.createElement('thead');
         table.appendChild(thead);
         const headerRow = thead.insertRow(0);
-
         const headers = tableJson.headers;
         for (let j = 1; j < headers.length; j++) {
             var cell = document.createElement("th");
             headerRow.appendChild(cell);
             cell.innerHTML = headers[j];
         }
 
+
+        // body
         const tbody = document.createElement('tbody');
         table.appendChild(tbody);
         const tableRows = tableJson.rows;
         for (let i = 0; i < tableRows.length; i++) {
 
-            const json = tableRows[i];
-            const unique_id = json[0]
+            const rowData = tableRows[i];
+            const unique_id = rowData[0]
             const row = document.createElement("tr");
             row.id = "row_" + unique_id;
             tbody.appendChild(row);
 
             // First row selected by default
             if (i === 0) row.classList.add("selected")
 
@@ -235,20 +244,18 @@
                 const session = sessionDictionary[uniqueId]
                 igvBrowser.loadSession({
                     url: session
                 })
             }
 
             for (let j = 1; j < headers.length; j++) {
-
-                var value = json[j];
                 cell = document.createElement("td");
-                cell.rowID = i;
+                //cell.rowID = i;
                 row.appendChild(cell);
-                cell.innerHTML = value;
+                cell.innerHTML = rowData[j];
             }
         }
 
         // Add sorting.  Adapted from https://stackoverflow.com/questions/14267781/sorting-html-table-with-javascript/49041392
         Array.prototype.slice.call(document.querySelectorAll('th')).forEach(function (th) {
             th.addEventListener('click', function () {
                 //var table = th.parentNode
```

### Comparing `igv-reports-1.7.0/igv_reports/tracks.py` & `igv-reports-1.8.0/igv_reports/tracks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from igv_reports import feature
 
-def get_track_json_dict(filename):
+def get_track_json_dict(url):
 
-    name = get_name(filename)
-    format = feature.infer_format(filename)
-    # Note: CRAM files are output in BAM format
-    if format == 'cram':
-        format = 'bam'
-    # Note: BCF files are output in VCF format
-    if format == 'bcf':
-        format = 'vcf'
+    name = get_name(url)
+    format = feature.infer_format(url)
     type = get_track_type(format)
-    return {
+
+    trackobj = {
         "name": name,
-        "url": filename,
+        "url": url,
         "type": type,
         "format": format
     }
 
+    if type == "alignment":
+        trackobj["height"] = 500
+    elif type == "mut":
+        trackobj["height"] = 50
+        trackobj["color"] = "rgb(0,0,150)"
+
+    return trackobj
+
 def get_name(filename):
 
     idx = filename.rfind("/")
     if idx < 0:
         idx = filename.rfind("\\")
     period = filename.rfind(".")
     if idx < 0:
@@ -47,10 +50,11 @@
         "gff": "annotation",
         "gtf": "annotation",
         "bed": "annotation",
         "refgene": "annotation",
         "bcf": "variant",
         "vcf": "variant",
         "wig": "wig",
-        "bedgraph": "wig"
+        "bedgraph": "wig",
+        "maf": "mut"
     }
     return dict[format]
```

### Comparing `igv-reports-1.7.0/igv_reports/varianttable.py` & `igv-reports-1.8.0/igv_reports/varianttable.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/vcf.py` & `igv-reports-1.8.0/igv_reports/vcf.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports/wig.py` & `igv-reports-1.8.0/igv_reports/wig.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/igv_reports.egg-info/PKG-INFO` & `igv-reports-1.8.0/igv_reports.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 Metadata-Version: 2.1
 Name: igv-reports
-Version: 1.7.0
+Version: 1.8.0
 Summary: Creates self-contained html pages for visual variant review with IGV (igv.js).
 Home-page: https://github.com/igvteam/igv-reports
 Author: Jim Robinson
 License: MIT
 Description: # igv-reports
         
         A Python application to generate self-contained HTML reports that consist of a table of genomic sites or regions and associated IGV views for each site.
         The generated HTML page contains all data neccessary for IGV as uuencoded blobs. It can be opened within a web browser as a static page, with no depenency on the original input files.
         
-        ### _NEW - alignments marked "duplicate" are now filtered by default.  See the --exclude-flags option._
-        
         ## Installation
         
         #### Prerequisites
         
         igv-reports __requires Python 3.6__ or greater.  
         
-        As with all Python projects, use of a __virtual environment__ is recommended.
-        Instructions for creating a virtual environment using ```conda``` follow.
-        
-        __1.__ Install Anaconda from https://docs.anaconda.com/anaconda/
-        
-        __2.__ Create a virtual environment
-        
-        ```bash
-        conda create -n igvreports python=3.7.1
-        conda activate igvreports
-        ```
         
         #### Installing igv-reports
         
         ```bash
         pip install igv-reports
         ```
         
@@ -67,29 +54,30 @@
             * __--sequence__ INT.   Column of sequence (chromosome) name.
             
         * Optional for generic tab delimited __sites__ file
             * __--zero-based__  Specify that the position in the __sites__ file is 0-based (e.g. UCSC files) rather than 1-based.  Default is ```false```.
         
         * Optional
             * __--genome__ **_New_** An igv.js genome identifier (e.g. hg38).  If supplied fasta, ideogram, and the default annotation track for the specified genome will be used.
+            * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.  Useful when __fasta__ is used to specify the reference.
             * __--tracks__ LIST.  Space-delimited list of track files, see below for supported formats.  If both *tracks* and *track-config* are specified *tracks* will appear first by default.
             * __--track-config__  FILE.  File containing array of json configuration objects for igv.js tracks.  See the [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Tracks-2.0) for more details.  This option allows customization of track parameters.  When using this option, the track ```url``` and ```indexURL``` properties should be set to the paths of the respective files.
-            * __--ideogram__ FILE. Ideogram file in UCSC cytoIdeo format.
+            * __--roi__ LIST.  Space-delimited list of region-of-interest (ROI) files.  See [igv.js wiki](https://github.com/igvteam/igv.js/wiki/Regions-of-Interest).
             * __--template__ FILE. HTML template file.
             * __--output__ FILE. Output file name; default="igvjs_viewer.html".
             * __--info-columns__ LIST. Space delimited list of info field names to include in the variant table.  If __sites__ is a VCF file these are the info ID values.  If __sites__ is a tab delimited format these are column names.
             * __--info-columns-prefixes__ LIST. For VCF based reports only.  Space delimited list of prefixes of VCF info field IDs to include in the variant table.  Any info field with ID starting with one of the listed values will be included.
             * __--samples__ LIST.  Space delimited list of sample (i.e. genotypes) names.  Used in conjunction with __--sample-columns__.
             * __--sample-columns__ LIST. Space delimited list of VCF sample FORMAT field names to include in the variant table.  If __--samples__ is specified columns will be restricted to those samples, otherwise all samples will be included.
             * __--flanking__ INT. Genomic region to include either side of variant; default=1000.
             * __--standalone__ Embed all JavaScript referenced via ```<script>``` tags in the page.
             * __--sort__ Applies to alignment tracks only.  If specified alignments are initally sorted by the specified option. Supported values include  ```BASE, STRAND, INSERT_SIZE, MATE_CHR, and NONE```. Default value is ```BASE``` for single nucleotide variants, ```NONE``` (no sorting) otherwise.  See the igv.js documentation for more information.
             * __--exclude-flags__  INT. Value is passed to samtools as "-F" flag.  Used to filter alignments.  Default value is 1536 which filters alignments marked "duplicate" or "vendor failed". To include all alignments use ```--exclude-flags 0```.  See [samtools documentation](http://www.htslib.org/doc/samtools-view.html) for more details.
             * __--idlink__ URL tempate for information link for VCF ID values.  The token $$ will be substituted with the ID value.  Example: ```--idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$'```
-             
+            * __--no-encode__ Don't embed data.  Fasta and track URLs are embedded unchanged.  The resulting report is depedendent on the original data files, which must be specified as URLs.  Local files are not supported with this option.
         
         **Track file formats:**
         
         Currently supported track file formats are BAM, CRAM, VCF, BED, GFF3, GTF, WIG, and BEDGRAPH.  FASTA. BAM, CRAM, and VCF  
         files must be indexed.  Tabix is supported and it is recommended that all large files be indexed.   
         
         ## Examples
@@ -112,15 +100,15 @@
         
         
         #### Create a variant report from a VCF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_vcf.html))
         
         ```bash
         
         create_report test/data/variants/variants.vcf.gz \
-        http://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
         --ideogram test/data/hg38/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
         --samples reads_1_fastq \
         --sample-columns DP GQ \
         --tracks test/data/variants/variants.vcf.gz test/data/variants/recalibrated.bam test/data/hg38/refGene.txt.gz \
         --output examples/example_vcf.html
@@ -129,89 +117,94 @@
         
         
         
         #### Create a variant report with tracks defined in an [igv.js track config json file](https://github.com/igvteam/igv-reports/tree/master/test/data/variants/trackConfigs.json): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_config.html))
         
         ``` bash
         create_report test/data/variants/variants.vcf.gz \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --fasta https://igv-genepattern-org.s3.amazonaws.com/genomes/seq/hg38/hg38.fa \
         --ideogram test/data/hg38/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns GENE TISSUE TUMOR COSMIC_ID GENE SOMATIC \
         --track-config test/data/variants/trackConfigs.json \
         --output examples/example_config.html
         ```
         
         
         #### Create a variant report from a TCGA MAF file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_maf.html))
         
         ```bash
         
         create_report test/data/variants/tcga_test.maf \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
+        --genome hg19 \
         --flanking 1000 \
         --info-columns Chromosome Start_position End_position Variant_Classification Variant_Type Reference_Allele Tumor_Seq_Allele1 Tumor_Seq_Allele2 dbSNP_RS \
-        --tracks  https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/tcga_test.maf \
         --output examples/example_maf.html
         
         ```
         
         #### Create a variant report from a generic tab-delimited file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_tab.html))
         
         ```bash
         
         create_report test/data/variants/test.maflite.tsv \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
+        --genome hg19 \
         --sequence 1 --begin 2 --end 3 \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
         --flanking 1000 \
         --info-columns chr start end ref_allele alt_allele \
-        --tracks https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
         --output examples/example_tab.html
         
         ```
-        #### NEW (version 1.5.0) - Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
+        ####  Create a structural variant report from a bedpe file with two locations (BEDPE format): ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_bedpe.html))
         
         ```bash
         
         create_report test/data/variants/SKBR3_Sniffles_tra.bedpe \
         --genome hg19 \
         --flanking 1000 \
-        --tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/SKBR3_Sniffles_variants_tra.vcf test/data/variants/SKBR3.ill.bam \
         --output examples/example_bedpe.html
         ```
         
         #### Create a variant report with custom ID link urls: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_idlink.html))
         
         ```bash
         
         create_report test/data/variants/1kg_phase3_sites.vcf.gz \
-        https://s3.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg19/hg19.fasta \
-        --ideogram test/data/hg19/cytoBandIdeo.txt \
+        --genome hg19 \
         --flanking 1000 \
-        --tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam https://hgdownload.soe.ucsc.edu/goldenPath/hg19/database/refGene.txt.gz \
+        --tracks test/data/variants/1kg_phase3_sites.vcf.gz test/data/variants/NA12878_lowcoverage.bam \
         --idlink 'https://www.ncbi.nlm.nih.gov/snp/?term=$$' \
         --output examples/example_idlink.html
         
         ```
         
         #### Create a junction report from a splice-junction bed file: ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_junctions.html))
         
         ```bash
         create_report test/data/junctions/Introns.38.bed \
-        https://s3.dualstack.us-east-1.amazonaws.com/igv.broadinstitute.org/genomes/seq/hg38/hg38.fa \
+        --genome hg38 \
         --type junction \
-        --ideogram test/data/hg38/cytoBandIdeo.txt \
         --track-config test/data/junctions/tracks.json \
         --info-columns TCGA GTEx variant_name \
         --title "Sample A" \
         --output examples/example_junctions.html
         ```
         
+        #### Create a fusion report from a Trinity fusion json file: 
+        
+        ```bash
+        create_report test/data/fusion/igv.fusion_inspector_web.json \
+        --fasta test/data/fusion/igv.genome.fa  \
+        --template igv_reports/templates/fusion_template.html  \  
+        --track-config test/data/fusion/tracks.json  \
+        --output examples/example_fusion.html
+        ```
+        
         #### Create a report containing wig and bedgraph files
         
         ```bash
         create_report test/data/wig/regions.bed \
         --genome hg19 \
         --exclude-flags 512 \
         --tracks test/data/wig/ucsc.bedgraph test/data/wig/mixed_step.wig test/data/wig/variable_step.wig \
@@ -219,31 +212,41 @@
         
         ```
         
         #### Use of ```info-columns-prefixes``` option.  Variant track only, no alignments. ([Example output](https://igv.org/igv-reports/examples/1.5.1/example_ann.html))
         
         
         ```bash
-        create_report test/data/infofields/consensus.filtered.ann.vcf \
+        python igv_reports/report.py test/data/annotated_vcf/consensus.filtered.ann.vcf \
         --genome hg19 \
         --flanking 1000 \
         --info-columns cosmic_gene \
         --info-columns-prefixes clinvar \
-        --tracks test/data/infofields/consensus.filtered.ann.vcf \
-        --output https://igv.org/igv-reports/examples/1.5.1/example_ann.html 
+        --tracks test/data/annotated_vcf/consensus.filtered.ann.vcf \
+        --output examples/example_ann.html 
         ```
         
         #### Use ```--exclude-flags``` option to include duplicate alignments in report.  Default value is 1536 which filters duplicates and vendor-failed reads.
         
         ```bash
         create_report test/data/dups/dups.bed \
         --genome hg19 \
         --exclude-flags 512 \
         --tracks test/data/dups/dups.bam \
         --output examples/example_dups.html
+        ```
+        
+        ### Use ```-no-embed``` option to use external URL references for tracks in the report.  
+        
+        ```bash
+        create_report test/data/variants/variants.vcf.gz \
+        --genome hg38 \
+        --no-embed \
+        --tracks https://igv-genepattern-org.s3.amazonaws.com/test/reports/variants.vcf.gz https://igv-genepattern-org.s3.amazonaws.com/test/reports/recalibrated.bam \
+        --output examples/example_noembed.html
         
         ```
         
         #### Converting genomic files to data URIs for use in igv.js 
         
         The script ```create_datauri``` (```python igv_reports/datauri.py```) converts the contents of a file to a data uri for use in igv.js.   The datauri will be printed to stdout.  *NOTE* It is not neccessary to run this script explicitly to create a report, it is documented here
         for use with stand-alone igv.js.
```

### Comparing `igv-reports-1.7.0/igv_reports.egg-info/SOURCES.txt` & `igv-reports-1.8.0/igv_reports.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,23 @@
 igv_reports/wig.py
 igv_reports.egg-info/PKG-INFO
 igv_reports.egg-info/SOURCES.txt
 igv_reports.egg-info/dependency_links.txt
 igv_reports.egg-info/entry_points.txt
 igv_reports.egg-info/requires.txt
 igv_reports.egg-info/top_level.txt
+igv_reports/templates/fusion_template.html
 igv_reports/templates/junction_template.html
-igv_reports/templates/variant_template-2.html
+igv_reports/templates/variant_template-noembed.html
+igv_reports/templates/variant_template.html
 test/test_bam.py
 test/test_datauri.py
 test/test_fasta.py
 test/test_feature.py
 test/test_ideogram.py
 test/test_regions.py
+test/test_stream.py
 test/test_table.py
 test/test_track.py
+test/test_utils.py
 test/test_vcf.py
 test/test_wig.py
```

### Comparing `igv-reports-1.7.0/setup.py` & `igv-reports-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='igv-reports',
                  packages=['igv_reports'],
-                 version='1.7.0',
+                 version='1.8.0',
                  description='Creates self-contained html pages for visual variant review with IGV (igv.js).',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  license='MIT',
                  author='Jim Robinson',
                  url='https://github.com/igvteam/igv-reports',
                  keywords=['igv', 'bioinformatics', 'genomics', 'visualization', 'variant' ],
```

### Comparing `igv-reports-1.7.0/test/test_bam.py` & `igv-reports-1.8.0/test/test_bam.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_datauri.py` & `igv-reports-1.8.0/test/test_datauri.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_fasta.py` & `igv-reports-1.8.0/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_feature.py` & `igv-reports-1.8.0/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_ideogram.py` & `igv-reports-1.8.0/test/test_ideogram.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_table.py` & `igv-reports-1.8.0/test/test_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,30 +34,30 @@
         self.assertTrue(len(table.features), 2106)
         self.assertTrue(json)
 
 
     def test_maftable(self):
 
         maf_file = str((pathlib.Path(__file__).parent / "data/maf/tcga_test.maf").resolve())
-        table = generictable.GenericTable(maf_file)
+        table = generictable.GenericTable.from_tabfile(maf_file)
 
         json = table.to_JSON()
         self.assertEqual(len(table.features), 17)
         self.assertTrue(json)
 
     def test_maflite(self):
 
         maf_file = str((pathlib.Path(__file__).parent / "data/maf/test.maflite.tsv").resolve())
 
         info_columns = ["chr", "start", "end", "ref_allele", "alt_allele", "tumor_barcode"]
         sequence = 1
         start = 2
         end = 3
 
-        table = generictable.GenericTable(maf_file, info_columns, sequence, start, end)
+        table = generictable.GenericTable.from_tabfile(maf_file, info_columns, sequence, start, end)
 
         json = table.to_JSON()
         self.assertEqual(29, len(table.features))
         self.assertTrue(json)
 
 
     def test_annovar(self):
@@ -66,9 +66,12 @@
 
         #ANN=A|synonymous_variant|LOW|EGFR|1956|transcript|NM_001346897.1|Coding|19/26|c.2226G>A|p.(%3D)|2483/184056|2226/3276|742/1092||,A|synonymous_variant|LOW|EGFR|1956|transcript|NM_001346898.1|Coding|20/27|c.2361G>A|p.(%3D)|2618/184056|2361/3411|787/1137||,A|synonymous_variant|LOW|EGFR|1956|transcript|NM_001346899.1|Coding|19/27|c.2226G>A|p.(%3D)|2483/189060|2226/3498|742/1166||,A|synonymous_variant|LOW|EGFR|1956|transcript|NM_001346900.1|Coding|20/28|c.2202G>A|p.(%3D)|2415/98264|2202/3474|734/1158||,A|synonymous_variant|LOW|EGFR|1956|transcript|NM_001346941.1|Coding|14/22|c.1560G>A|p.(%3D)|1817/189060|1560/2832|520/944||,A|synonymous_variant|LOW|EGFR|1956|transcript|NM_005228.4|Coding|20/28|c.2361G>A|p.(%3D)|2618/189060|2361/3633|787/1211||;PROB_ABSENT=6086.16;PROB_ALT=0;PROB_ARTIFACT=3093.24;PROB_VERY_RARE=2789.3;SVLEN=.	DP:AF:OBS:SB	221:0.990543:116V-101V+2S-2N+:.
 
         table = varianttable.VariantTable(vcf_file, info_columns=["ANN"])
         json = table.to_JSON()
         self.assertTrue(json is not None)
 
+    def test_fusions(self):
 
-
+        fusions_file = str((pathlib.Path(__file__).parent / "data/fusion/fusions.json").resolve())
+        table = generictable.GenericTable.from_fusionjson(fusions_file)
+        self.assertTrue(table is not None)
```

### Comparing `igv-reports-1.7.0/test/test_vcf.py` & `igv-reports-1.8.0/test/test_vcf.py`

 * *Files identical despite different names*

### Comparing `igv-reports-1.7.0/test/test_wig.py` & `igv-reports-1.8.0/test/test_wig.py`

 * *Files identical despite different names*

