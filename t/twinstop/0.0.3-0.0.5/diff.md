# Comparing `tmp/twinstop-0.0.3.tar.gz` & `tmp/twinstop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.0.3.tar", last modified: Wed Jul 26 10:38:39 2023, max compression
+gzip compressed data, was "twinstop-0.0.5.tar", last modified: Fri Jul 28 14:15:29 2023, max compression
```

## Comparing `twinstop-0.0.3.tar` & `twinstop-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.3/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 10:38:39.975844 twinstop-0.0.3/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.3/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.3/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-26 10:38:39.975844 twinstop-0.0.3/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.3/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.3/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 10:37:53.000000 twinstop-0.0.3/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.0.3/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.3/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   112541 2023-07-26 10:36:55.000000 twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.3/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:38:39.975844 twinstop-0.0.3/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-26 10:38:39.000000 twinstop-0.0.3/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.667548 twinstop-0.0.5/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.5/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 14:15:29.667548 twinstop-0.0.5/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.5/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.5/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-28 14:15:29.667548 twinstop-0.0.5/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.5/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.5/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-28 14:15:22.000000 twinstop-0.0.5/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.0.5/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.667548 twinstop-0.0.5/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.5/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   114451 2023-07-26 14:18:34.000000 twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.5/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/twinstop.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.0.3/LICENSE` & `twinstop-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/PKG-INFO` & `twinstop-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.3
+Version: 0.0.5
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.3/setup.cfg` & `twinstop-0.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	biopython >= 1.78, <=1.81
 	easyterm >= 1.0.0
 	easybioinfo >= 0.2.1
-	extend-orfs-pyranges >= 0.1.1
+	extend-orfs-pyranges >= 0.1.5
 	file-chunk-iterators >= 0.0.1
 	pyranges >= 0.0.120
 	pandas >= 1.3.5
 	pyfaidx >= 0.7.2
 	multiprocess >= 0.70.14
 	numpy >= 1.21.5
 	scikit-learn >= 1.3.0
```

### Comparing `twinstop-0.0.3/src/twinstop/block_selection.py` & `twinstop-0.0.5/src/twinstop/block_selection.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.0.5/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/data_files/scaler.pkl` & `twinstop-0.0.5/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py` & `twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,83 +1,113 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jun 23 11:55:40 2022
 
-@author: Sergio Sánchez Moragues
+@author: Sergio Sánchez Moragues and Marco Mariotti
 """
 
 help_msg = """Twinstop is a de novo selenoprotein identification pipeline.
 It is based on the evolutionary conservation around the UGA-coding selenocysteine between two homologous
 selenoproteins from two closely related transcriptomes.
 
-### Inputs/Outputs:
+### Compulsory Inputs/Outputs arguments:
+-q <str>   query file path: a transcriptome in fasta format
+-s <str>   subject file path: a nucleotide transcriptome in fasta format, with with makeblastdb run beforehand
+-o <str>   output folder path, where files generated by Twinstop will be saved
+
+### Common optional arguments:
+#    Memory and CPU control
+-c <int>          nº of CPUs employed. Default: 1
+-time_mem <bool>  prints time and memory usage throughout the pipeline. Defalt: True
+
+#    Workflow
+-force <int>  controls the rerun of the phases of Twinstop. By default, it runs phases for which no output is detected.
+              Provide a number, representing the phase from which Twinstop will start the rerun 
+              For information about phases, run:  twinstop -h phases
+
+#    Output: these switches control the optional output files written for candidates
+-cds_q <bool>  fasta file with CDS sequences of query.       Default: False
+-cds_s <bool>  fasta file with CDS sequences of subject.     Default: False
+-pep_q <bool>  fasta file with protein sequences of query.   Default: True
+-pep_s <bool>  fasta file with protein sequences of subject. Default: False
+-gff_q <bool>  GFF file with coordinates on query.           Default: True
+-gff_s <bool>  GFF file with coordinates on subject.         Default: False
+
+#    Optional phase 7, annotation of candidates:
+-ann <bool>    perform the annotation of candidates (Phase 7). Requires -ann_db
+-ann_db <str>  path to database (protein fasta) to annotate candidates; recommended: Uniref50.
+               Note: makeblastdb must have been run on this file beforehand to use it
+
+### Advanced:
+# Twinstop can be very memory intensive, so it splits tables into chunks which are load and processed serially.
+-n_chunks <int> nº of chunks in which to divide the input file of phases 1,2,5.
+                Dividing in chunks reduces the memory but increases time. Default: 10
+-n_lines <int>  Chunk size (number of lines) used in phases 3,4. Default: 2500000
+-par_fct <int>  In phases 3,4,5, chunks are further divided in subchunks, processed in parallel.
+                This option sets the parallelization factor: the nº of subchunks per chunk is
+                determined as par_fct * N_CPUs. Default: 1
+# When performing pairwise alignments with the Biopython, some get stuck and take forever, so:
+-timeout <float>   Sets the maximum time for the execution of a pairwise alignment (phase 5).
+                   The alignments exceeding the timeout are computed using MAFFT instead. Default: 2.0
+# Developer options
+-debug <bool>     Creates files with all filtered and filtered_out candidates for filtering phases: 3, 4, 6, 7
+-benchmark <bool> Developer option; activates benchmarking. See details with: twinstop -h benchmark
 
-# Compulsory args:
--q : <str> query file path: a transcriptome in fasta format
--s : <str> subject file path: a nucleotide transcriptome in fasta format, with with makeblastdb run beforehand
--o : <str> output folder path, where files generated by Twinstop will be saved
-
-# Optional args:
--c : <int> nº of CPUs used to run BLAST. The default is '1' CPUs.
--force : <int> controls the rerun of the phases of Twinstop. The number represents the phase from which Twinstop
-               will start the rerun (only in the case that the output file from previous phases have already been created).
-               The default is to run only phases for which no output is detected.
-               For a list of phases, run:  twinstop -h phases
-
--n : <int> allows to divide chunks in n * c. Warning! Many chunks in a large dataset could saturate cache memory.
-
--annot_candidates : <bool> controls the annotation of candidates (Phase 7). If 'False', blastp will not run.
-                    The default is 'True'.
--annotation_db : <str> path to the database file used to annotate candidates. Only if '-annot_candidates: True'.
-                 By default, Twinstop uses Uniref50 database in fasta format.
--cds_q : <bool> controls the creation of a fasta file with the nucleotide sequences of the query candidates. The default is 'False'.
--cds_t : <bool> controls the creation of a fasta file with the nucleotide sequences of the subject candidates. The default is 'False'.
--pep_q : <bool> controls the creation of a fasta file with the protein sequences of the query candidates. The default is 'True'.
--pep_t : <bool> controls the creation of a fasta file with the protein sequences of the subject candidates. The default is 'False'.
--gff_q : <bool> controls the creation of a gff file with the alignment data of the query candidates. The default is 'True'.
--gff_t : <bool> controls the creation of a gff file with the alignment data of the subject candidates. The default is 'False'.
--benchmark : <bool> controls the creation of filtered and filtered_out candidates in each filtering phase (3, 4, 6, 7)
--timeout : <float> sets the maximum time to wait for a result in pairwise alignment (phase 5)
--time_mem_control : <bool> controls the usage of time and memory throughout the script (all phases)
-
-# Chunking parameters:
--n_chunks : <int> nº of chunks in which to divide the input file of phases 0-6. Dividing in chunks reduces the memory
-            but increases time. The default is '10' chunks.
--n_lines_over : <int> maximum of lines per chunk during overlapping (Phase 3). The default is '2500000' lines.
-
-### Options:
+### Other options:
 -print_opt: print currently active options
 -h | --help: print this help and exit"""
 
 phases_help="""
 TBD
 """
 
+benchmark_help="""
+### Benchmark usage: these are required if -benchmark is active
+# Benchmarking is performed counting how many of the selenoproteins expected on the subject are recovered
+# Note: it is generous, in the sense that only selenoprotein families that are expected in both subject 
+#  and query and counted, since they are the only ones that twinstop can, at best, predict.
+# Analogously, some selenoprotein families are always excluded since they have a terminal Sec, which
+#  cannot be predicted by the conservation approach of twinstop.
+
+-benchmark_subject_gff <str>  path to GFF-like file describing selenoproteins expected in the subject
+                              NOTE: coordinates are pyranges-like: 0-based, Start included and End excluded
+                              Format: Columns= ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
+                                                  'score', 'strand', 'frame', 'attribute', 'subj_id']
+                              Each line must contain only the Selenocysteine residues of the expected selenoproteins
+                              The attribute is selenoprofiles-like: Sec1:TR.70.selenocysteine  (here, TR is the sel_family)
+
+-benchmark_query <str>  path to tabular file describing selenoproteins expected in query. 
+                        Format: no header; fields: ['Chromosome', 'sel_family', 'id', 'subj_id']
+
+-unavailable_families <list>  list of selenoprotein families that are always excluded from benchmarking. 
+                              These have C-terminal Sec residues. Default: SelK SelKi SelO SelS TR
+"""
+
 def_opt = {
     'q': '',
     's': '',
     'o': 'twinstop_out/',
     'c': 1,
-    'n': 1,
+    'par_fct': 1,
     'n_chunks': 10,
     'n_lines': 2500000,
     'cds_q': False,
-    'cds_t': False,
+    'cds_s': False,
     'pep_q': False,
-    'pep_t': False,
+    'pep_s': False,
     'gff_q': False,
-    'gff_t': False,
-    'annotation_db': '',
+    'gff_s': False,
+    'ann_db': '',
     'force': 1000,
-    'annot_candidates': False,
-    'sp4_prediction_subj': '',
-    'sp4_prediction_query': '',
-    'sp4_subj_gff': '',
+    'ann': False,
+    'benchmark_subject_gff': '',
+    'benchmark_query': '',
+    'unavailable_families':['SelK', 'SelKi', 'SelO', 'SelS', 'TR'],
     'benchmark': False,
-    'debugging': False,
+    'debug': False,
     'timeout': 2.0,
     'time_mem_control': True,
     'model': 'd'
 }
 
 
 
@@ -432,14 +462,17 @@
     # splits DataFrame in query and subject DataFrames.
     query_df, subj_df = query_subject_dfs(chunk)
 
     query_df = extend_orfs(p=query_df, fasta_path=path_query_file, default_full=True,
                            as_df=True, stops=['TAG', 'TAA'])
     subj_df = extend_orfs(p=subj_df, fasta_path=path_subj_file, default_full=True,
                           as_df=True, stops=['TAG', 'TAA'])
+
+
+    
     # query_df.to_csv(sep='\t', path_or_buf='chunk_query_df')
     # subj_df.to_csv(sep='\t', path_or_buf='chunk_subj_df')
     # we need to get the protein sequences for the extended sequences.
     query_df, subj_df = get_cds_prot_seq(subj_df, query_df, path_subj_file, 
                                          path_query_file, CDS_sequences=True)
     # renames the PyRanges-format query columns to merge both query/subj DataFrames.
     query_df = query_df.rename(columns={'Chromosome': 'Q_ID', 'Start': 'Q_align_s',
@@ -1332,15 +1365,15 @@
     This function runs blastp. Useful to annotate the candidates
 
     Parameters
     ----------
     selenocandidates_df : <pd.DataFrame>
         DataFrame with the selenoprotein candidates.
     db_file : <str>, easyterm object
-        opt['annotation_db']
+        opt['ann_db']
     n_cpu : <int>, easyterm object
         opt['c']
     blastp_outfile : <str>
         Path for the blastp outfile.
     fasta_query_prot_seq : <str>
         Path for the fasta file with all query protein sequences.
 
@@ -1664,29 +1697,29 @@
     selenocandidates_df : <pd.DataFrame>
         Dataframe with all the selenoprotein candidates
     IsQueryCDSeqReturned : <bool>, easyterm object
         opt['cds_q']
     path_cds_q : <str>
         Path to save the cds sequence from the query if opt['cds_q'] == True
     IsTargetCDSeqReturned : <bool>, easyterm object
-        opt['cds_t']
+        opt['cds_s']
     path_cds_t : <str>
         Path to save the cds sequence from the target if opt['cds_t'] == True
     IsQueryProtSeqReturned : <bool>, easyterm object
         opt['pep_q']
     path_pep_q : <str>
         Path to save the protein sequence from the query if opt['pep_q'] == True
     IsTargetProtSeqReturned : <bool>, easyterm object
-        opt['pep_t']
+        opt['pep_s']
     path_pep_t : <str>
         Path to save the protein sequence from the target if opt['pep_t'] == True
     IsQueryGFFileReturned : <bool>, easyterm object
-        opt['dff_q']
+        opt['gff_q']
     IsTargetGFFileReturned : <bool>, easyterm object
-        opt['dff_t']
+        opt['gff_s']
     path_query_gff : <str>
         Path to save the gff file from the query if opt['dff_q'] == True
     path_subj_gff : <str>
         Path to save the gff file from the target if opt['dff_t'] == True
 
     Returns
     -------
@@ -1879,15 +1912,15 @@
         candidates_df['Run_info'] = (abbreviations[os.path.basename(q_file).split('.')[0]] + '_vs_' +
                                      abbreviations[os.path.basename(subj_file).split('.')[0]])
     except:
         candidates_df['Run_info'] = (os.path.basename(q_file).split('.')[0] +
                                      '_vs_' + os.path.basename(subj_file).split('.')[0])
     candidates_df[['sec_start', 'sec_end']] = \
         candidates_df.apply(find_sec_pos, axis=1, result_type='expand')
-    if not sp4_subj_gff == None:
+    if not sp4_subj_gff is None:
         true_positives = candidates_df[['ID', 'Chromosome', 'sec_start', 'sec_end']] \
             .merge(sp4_subj_gff[['Chromosome', 'sec_start', 'sec_end']],
                    on=['Chromosome', 'sec_start', 'sec_end'], how='inner')
     # true_positives = true_positives[true_positives.sec_start_ts.eq(true_positives.sec_start_sp4)]
     # print(candidates_df.dtypes)
     # print(candidates_df['sec_start_ts'] == candidates_df['sec_start_sp4'])
     # print(true_positive)
@@ -2036,35 +2069,35 @@
 
     write(f'TwinStop {__version__}')
     write(f'{current_time}\n')
     # most used opt options are saved in variables
     n_cpu = opt['c']
     n_chunks = opt['n_chunks']
     n_lines = opt['n_lines']
-    n = opt['n']
+    n = opt['par_fct']
     n_section =  opt['force']
-    time_memory_control = opt['time_mem_control']
+    time_memory_control = opt['time_mem']
     # benchmark variable is defined as global to use it all across the script without the need of being imported
     global benchmark, debugging
     benchmark = opt['benchmark']
-    debugging = opt['debugging']
+    debugging = opt['debug']
 
     if benchmark:
         # read table of the Selenoprofiles4 selenocysteines prediction for subject (control selenoproteins)
-        sp4_subj_gff = pd.read_csv(opt['sp4_subj_gff'], sep="\t", header=None, index_col=False)
+        sp4_subj_gff = pd.read_csv(opt['benchmark_subject_gff'], sep="\t", header=None, index_col=False)
         sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
                                 'score', 'strand', 'frame', 'attribute', 'subj_id']
         sp4_prediction_subj = pd.DataFrame()
         sp4_prediction_subj['Transcript'] = sp4_subj_gff.Chromosome
         sp4_prediction_subj[['Sel_family', 'n']] = sp4_subj_gff.apply(
             lambda x: x['attribute'].split(':')[1].split('.')[:2], axis=1, result_type='expand')
         sp4_prediction_subj['Subj_ID'] = sp4_subj_gff.subj_id
         # sp4_prediction_subj = pd.read_table(opt['sp4_prediction_subj'], sep='\t', header=None,
         #                                     names=["Transcript", "Sel_family", "n", "Subj_ID"], index_col=False)
-        sp4_prediction_query = pd.read_table(opt['sp4_prediction_query'], sep='\t', header=None,
+        sp4_prediction_query = pd.read_table(opt['benchmark_query'], sep='\t', header=None,
                                              names=["Transcript", "Sel_family", "n", "Query_ID"], index_col=False)
         # I want to get rid of the selenoprotein families which are unreachable for this script (terminal selenocysteines)
         # selenos_annot_query = pd.DataFrame(sp4_prediction_query.Name.str.split(n=3, pat=".").to_list(),
         #                                    columns=['Sel_family', 'Nº', 'Stop_codon', 'rest'])
         # selenos_annot_query.drop(labels='rest', axis=1, inplace=True)
         # selenos_annot_query['Transcript'] = sp4_prediction_query.Transcript
         # we compare subject transcripts with subject SP4 prediction subtracting the selenofamilies not present in the
@@ -2073,15 +2106,15 @@
         if selenos_annot.shape[0] != sp4_prediction_subj.shape[0]:
             unpresent_sel = sp4_prediction_subj[~sp4_prediction_subj.Sel_family.isin(sp4_prediction_query.Sel_family)]
             write(f'Selenoprotein families not present in query Selenoprofiles 4 prediction:\n\n{unpresent_sel}\n')
         # deletes a Python variable (empthy memory)
         del sp4_prediction_subj, sp4_prediction_query
 
         # I want to get rid of the selenoprotein families which are unreachable for this script (terminal selenocysteines)
-        unavailable_Sel_families = ['SelK', 'SelKi', 'SelO', 'SelS', 'TR']
+        unavailable_Sel_families = opt['unavailable_families']
         # keeps the rest of selenos
         available_selenos = selenos_annot[~selenos_annot.Sel_family.isin(unavailable_Sel_families)]
         if available_selenos.shape[0] != selenos_annot.shape[0]:
             unavailable_sel = selenos_annot[selenos_annot.Sel_family.isin(unavailable_Sel_families)]
             write(f'Unavailable Selenoprotein families predicted by Selenoprofiles 4:\n\n{unavailable_sel}')
         del selenos_annot
 
@@ -2186,14 +2219,18 @@
         # calling function
         candidates_df = UGA_alignments(aln_orfs)
         # saving dataframe as a csv file
         candidates_df = candidates_df \
             .sort_values(by='Score', ascending=False, ignore_index=True) \
             .drop_duplicates('Chromosome', ignore_index=True)
         candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
+
+        ##########  MODIFY TO: do chunking if not benchmarking; if benchmark, keep code above
+        ###
+        
         # else:
         #     chunking(path_pairwise_outfile, n_chunks, 0, UGA_alignments,
         #              n_cpu, None, path_candidates_outfile, n)
         #     candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
     else:
         write(f'Reading {path_candidates_outfile}')
         candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
@@ -2276,16 +2313,16 @@
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
     write('\n### PHASE 8: BLASTP FOR ANNOTATION')
 
-    if not 'Annot_Title' in candidates_df and opt['annot_candidates']:
-        candidates_df = run_blastp(candidates_df, opt['annotation_db'], n_cpu,
+    if not 'Annot_Title' in candidates_df and opt['ann']:
+        candidates_df = run_blastp(candidates_df, opt['ann_db'], n_cpu,
                                    path_blastp_outfile, path_fasta_query_prot_seq)
         candidates_df.sort_values(by='Density_Score', inplace=True,
                                   ignore_index=True, ascending=False)
         candidates_df.to_csv(sep='\t', path_or_buf=path_selenocandidates_annotated_outfile, index=False)
         # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
         # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
@@ -2295,16 +2332,16 @@
 
     write('\n### PHASE 9: OUTPUTS')
 
     candidates_pretty = pretty_output(candidates_df)
     with open(path_pretty_outfile, 'w') as fw:
         fw.write(candidates_pretty)
 
-    outputs(candidates_df, opt['cds_q'], path_cds_q, opt['cds_t'], path_cds_t,
-            opt['pep_q'], path_pep_q, opt['pep_t'], path_pep_t, opt['gff_q'],
-            opt['gff_t'], path_gff_q, path_gff_t)
+    outputs(candidates_df, opt['cds_q'], path_cds_q, opt['cds_s'], path_cds_t,
+            opt['pep_q'], path_pep_q, opt['pep_s'], path_pep_t, opt['gff_q'],
+            opt['gff_s'], path_gff_q, path_gff_t)
 
     if time_memory_control:
         time_mem_usage(initial_time)
 
 if __name__ == '__main__':
     main()
```

### Comparing `twinstop-0.0.3/src/twinstop/test_alignment_methods.py` & `twinstop-0.0.5/src/twinstop/test_alignment_methods.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.3/src/twinstop.egg-info/PKG-INFO` & `twinstop-0.0.5/src/twinstop.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.3
+Version: 0.0.5
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.3/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.0.5/src/twinstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

