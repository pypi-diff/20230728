# Comparing `tmp/twinstop-0.0.5.tar.gz` & `tmp/twinstop-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.0.5.tar", last modified: Fri Jul 28 14:15:29 2023, max compression
+gzip compressed data, was "twinstop-0.1.0.tar", last modified: Fri Jul 28 19:48:38 2023, max compression
```

## Comparing `twinstop-0.0.5.tar` & `twinstop-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.667548 twinstop-0.0.5/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.0.5/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 14:15:29.667548 twinstop-0.0.5/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.0.5/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.0.5/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-28 14:15:29.667548 twinstop-0.0.5/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.0.5/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.0.5/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-28 14:15:22.000000 twinstop-0.0.5/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.0.5/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.667548 twinstop-0.0.5/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.0.5/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.0.5/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.bkp2.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   114451 2023-07-26 14:18:34.000000 twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.0.5/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:15:29.663548 twinstop-0.0.5/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-28 14:15:29.000000 twinstop-0.0.5/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.0/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 19:48:38.736694 twinstop-0.1.0/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.1.0/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.0/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-28 19:48:38.736694 twinstop-0.1.0/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.0/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.0/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-28 16:05:53.000000 twinstop-0.1.0/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.1.0/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.0/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   119028 2023-07-28 16:09:29.000000 twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.1.0/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.0.5/LICENSE` & `twinstop-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/PKG-INFO` & `twinstop-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.5
+Version: 0.1.0
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.5/setup.cfg` & `twinstop-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/block_selection.py` & `twinstop-0.1.0/src/twinstop/block_selection.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.1.0/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/data_files/scaler.pkl` & `twinstop-0.1.0/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.bkp2.py` & `twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 -q <str>   query file path: a transcriptome in fasta format
 -s <str>   subject file path: a nucleotide transcriptome in fasta format, with with makeblastdb run beforehand
 -o <str>   output folder path, where files generated by Twinstop will be saved
 
 ### Common optional arguments:
 #    Memory and CPU control
 -c <int>          nº of CPUs employed. Default: 1
--time_mem <bool>  prints time and memory usage throughout the pipeline. Defalt: True
+-time_mem <bool>  prints time and memory usage throughout the pipeline. Defalt: False
 
 #    Workflow
 -force <int>  controls the rerun of the phases of Twinstop. By default, it runs phases for which no output is detected.
-              Provide a number, representing the phase from which Twinstop will start the rerun 
+              Provide a number, representing the phase from which Twinstop will start the rerun
               For information about phases, run:  twinstop -h phases
 
 #    Output: these switches control the optional output files written for candidates
 -cds_q <bool>  fasta file with CDS sequences of query.       Default: False
 -cds_s <bool>  fasta file with CDS sequences of subject.     Default: False
 -pep_q <bool>  fasta file with protein sequences of query.   Default: True
 -pep_s <bool>  fasta file with protein sequences of subject. Default: False
@@ -52,14 +52,28 @@
 -debug <bool>     Creates files with all filtered and filtered_out candidates for filtering phases: 3, 4, 6, 7
 -benchmark <bool> Developer option; activates benchmarking. See details with: twinstop -h benchmark
 
 ### Other options:
 -print_opt: print currently active options
 -h | --help: print this help and exit"""
 
+
+description_of_phases={
+    0:'Running tblastx between the transcriptomes',
+    1:'Extracting CDS sequences and translating to get protein sequences',
+    2:'Partitioning in UGA-containing ORFs, selecting best one per candidate',
+    3:'Removing redundancy due to overlapping blast hits',
+    4:'Extending to have complete UGA-containing ORFs, then removing duplicates',
+    5:'Performing pairwise alignments between complete UGA-containing ORFs',
+    6:'Filtering out candidates that do not have UGA-UGA alignments',
+    7:'Filtering candidates based on sequence conservation and other features',
+    8:'Annotating candidates through blastp',
+    9:'Producing output files'
+}
+
 phases_help="""
 TBD
 """
 
 benchmark_help="""
 ### Benchmark usage: these are required if -benchmark is active
 # Benchmarking is performed counting how many of the selenoproteins expected on the subject are recovered
@@ -101,15 +115,15 @@
     'ann': False,
     'benchmark_subject_gff': '',
     'benchmark_query': '',
     'unavailable_families':['SelK', 'SelKi', 'SelO', 'SelS', 'TR'],
     'benchmark': False,
     'debug': False,
     'timeout': 2.0,
-    'time_mem_control': True,
+    'time_mem': False,
     'model': 'd'
 }
 
 
 
 
 # packages:
@@ -169,16 +183,16 @@
     ------
     Exception
         We raise an exception to stop the program in case returncode is
         different that zero, indicating that subprocess.run has not run
         successfully.
         We also print the stdout and stderr to know more about the problem
     '''
-    if not os.path.exists(tblastx_format_6_outfile) or IsFormat6FileForced:
-        write('Running format 6 tBLASTx')
+    #if not os.path.exists(tblastx_format_6_outfile) or IsFormat6FileForced:
+    if True:
         # to avoid BLAST 'No such file or directory error', we make sure to build the subject 
         # transcriptome as a BLAST db before running tBLASTx.
         cmd_makeblastdb = 'makeblastdb -in ' + path_db_file + ' -dbtype nucl'
         cmd_makeblastdb_list = shlex.split(cmd_makeblastdb)
         # subprocess.run allows to execute external programs inside a Python code
         y = subprocess.run(cmd_makeblastdb_list, capture_output=True)
         # controls that the subject transcriptome is nucleotide dtype, else raises Exception
@@ -1588,14 +1602,15 @@
 #     selenocandidates_df = selenocandidates_df.reindex(columns=columns_index)
 #
 #     return selenocandidates_df
 
 def pretty_output(df):
     pretty_outfile = ''
     for i, row in df.iterrows():
+        pretty_outfile+='='*80+'\n'
         comparison_string = ''
         Us_string = ''
         # write(row)
         for index, x in enumerate(row['Q_align_prot_seq']):
             if x == '-' or row['Subj_align_prot_seq'][index] == '-':
                 comparison_string += ' '
                 Us_string += ' '
@@ -1681,15 +1696,15 @@
                     pretty_outfile += f"Sbjct  {row['End'] - n * idx * 3 - 1 + acumulated_gaps_subj * 3:<5d}  {subj_chunks[idx]}  {row['End'] + (-1 * (n * idx + len(subj_chunks[idx])) + gaps_subj) * 3:<5d}\n"
                 acumulated_gaps_subj = gaps_subj
 
             pretty_outfile += f'              {U_chunks[idx]}\n'
 
     return pretty_outfile
 
-def outputs(selenocandidates_df, IsQueryCDSeqReturned, path_cds_q, IsTargetCDSeqReturned, path_cds_t,
+def make_outputs(selenocandidates_df, IsQueryCDSeqReturned, path_cds_q, IsTargetCDSeqReturned, path_cds_t,
             IsQueryProtSeqReturned, path_pep_q, IsTargetProtSeqReturned, path_pep_t, IsQueryGFFileReturned,
             IsTargetGFFileReturned, path_query_gff, path_subj_gff):
     '''
     Function with the several optional script outfiles dependent on boolean 
     values.
 
     Parameters
@@ -1722,15 +1737,14 @@
         Path to save the gff file from the target if opt['dff_t'] == True
 
     Returns
     -------
     None
     '''
 
-    write('Producing output')
 
     output_cds_q = ''
     output_cds_t = ''
     output_pep_q = ''
     output_pep_t = ''
 
     for i, row in selenocandidates_df.iterrows():
@@ -1756,23 +1770,27 @@
                 output_pep_q += f">{row['Run_info']},{row['Q_ID']}[{row['Q_align_s']}:{row['Q_align_e']}],{row['ID']}\n"
             output_pep_q += f"{row['Q_align_prot_seq'].replace('-', '')}\n"
         if IsTargetProtSeqReturned:
             output_pep_t += f">{row['Run_info']},{row['Chromosome']}[{row['Start']}:{row['End']}],{row['ID']}\n"
             output_pep_t += f"{row['Subj_align_prot_seq'].replace('-', '')}\n"
 
     if IsQueryCDSeqReturned:
+        write(f'Output: fasta of query CDSs  --> {path_cds_q}')
         with open(path_cds_q, 'w') as fw:
             fw.write(output_cds_q)
     if IsTargetCDSeqReturned:
+        write(f'Output: fasta of subject CDSs --> {path_cds_t}')        
         with open(path_cds_t, 'w') as fw:
             fw.write(output_cds_t)
     if IsQueryProtSeqReturned:
+        write(f'Output: fasta of query proteins --> {path_pep_q}')        
         with open(path_pep_q, 'w') as fw:
             fw.write(output_pep_q)
     if IsTargetProtSeqReturned:
+        write(f'Output: fasta of subject proteins --> {path_pep_t}')
         with open(path_pep_t, 'w') as fw:
             fw.write(output_pep_t)
 
     # if IsCandidatesDotplotReturned:
     #     dot_plot(selenocandidates_df, path_dotplot)
 
     selenocandidates_df.rename(columns={'ID': 'Gene_ID'}, inplace=True)
@@ -1787,22 +1805,24 @@
             columns={'Q_ID': 'Chromosome', 'Q_align_s': 'Start',
                      'Q_align_e': 'End', 'Q_Strand': 'Strand'})
         query_df_reduced = query_df.loc[
             :, ['Chromosome', 'Source', 'Feature', 'Start', 'End',
                 'Strand', 'Score', 'Gene_ID', 'Annot_Title']]
 
         py_query = pr.PyRanges(query_df_reduced)
+        write(f'Output: query GFF --> {path_query_gff}')
         py_query.to_gff3(path=path_query_gff)
 
     if IsTargetGFFileReturned:
         candidates_reduced = selenocandidates_df.loc[
             :, ['Chromosome', 'Source', 'Feature', 'Start', 'End',
                 'Strand', 'Score', 'Gene_ID', 'Annot_Title']]
 
         py_subj = pr.PyRanges(candidates_reduced)
+        write(f'Output: subject GFF --> {path_subj_gff}')
         py_subj.to_gff3(path=path_subj_gff)
 
 def get_proc_status(keys=None):
     '''
     This function creates a dictionary with the information of the proc file which can be accessed
     by keys, if no keys it returns the dictionary.
 
@@ -2015,15 +2035,14 @@
     #     print(row['Query_CDS'])
     return candidates_df
 
 def main():
 
     initial_time = datetime.now()
     # .strftime method allows to put a datetime object in clock format '%H:%M:%S'
-    current_time = initial_time.strftime('%H:%M:%S')
 
     # easyterm method to create a dictionary with command line input parameters and a help message
     opt = command_line_options(def_opt, help_msg,
                                advanced_help_msg={'phases':phases_help}
     )
     # os.path.abspath(relative/absolute path) gets the absolute path of a file
     q_file = os.path.abspath(opt['q'])
@@ -2044,18 +2063,18 @@
     ############# Main paths ####################
     path_tblastx_outfile = 'tblastx.tsv'
     path_postchunking_outfile = 'tblastx_df_postchunking.tsv'
     path_fragmentation_outfile = 'all_orfs.tsv'
     path_overlapping_outfile = 'nov_orfs.tsv'
     path_extend_outfile = 'ext_orfs.tsv'
     path_pairwise_outfile = 'aln_orfs.tsv'
-    path_candidates_outfile = 'candidates.tsv'
+    path_candidates_outfile = 'uga_orfs.tsv'
     path_selenocandidates_outfile = 'selenocandidates.tsv'
     path_selenocandidates_annotated_outfile = 'selenocandidates_annotated.tsv'
-    path_pretty_outfile = 'candidates_pretty.txt'
+    path_pretty_outfile = 'selenocandidates.pretty.txt'
     ############# Temporal paths ################
     # temporal paths are removed (os.remove(path)) before finishing their phase
     path_blastp_outfile = 'candidates_blastp.tsv'
     path_fasta_query_prot_seq = 'fasta_seq.fa'
     ############# Optional Output paths ##################
     # optional paths depend on boolean parameters
     path_cds_q = 'candidates_query.cds.fa'
@@ -2063,28 +2082,29 @@
     path_pep_q = 'candidates_query.pep.fa'
     path_pep_t = 'candidates_target.pep.fa'
     path_gff_q = 'candidates_query.gff'
     path_gff_t = 'candidates_target.gff'
     # fragments_dot_plot = opt['o'] + 'fragments_dotplot.png'
     # overlapping_dot_plot = opt['o'] + 'overlapping_dotplot.png'
 
-    write(f'TwinStop {__version__}')
-    write(f'{current_time}\n')
+    write(f' TwinStop v{__version__} | Date: {datetime.now().strftime("%Y-%m-%d %H:%M:%S")} '.center(70, '*'))
     # most used opt options are saved in variables
     n_cpu = opt['c']
     n_chunks = opt['n_chunks']
     n_lines = opt['n_lines']
     n = opt['par_fct']
     n_section =  opt['force']
     time_memory_control = opt['time_mem']
     # benchmark variable is defined as global to use it all across the script without the need of being imported
     global benchmark, debugging
     benchmark = opt['benchmark']
     debugging = opt['debug']
 
+    colors={'phase':'green', 'count':'magenta'}
+
     if benchmark:
         # read table of the Selenoprofiles4 selenocysteines prediction for subject (control selenoproteins)
         sp4_subj_gff = pd.read_csv(opt['benchmark_subject_gff'], sep="\t", header=None, index_col=False)
         sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
                                 'score', 'strand', 'frame', 'attribute', 'subj_id']
         sp4_prediction_subj = pd.DataFrame()
         sp4_prediction_subj['Transcript'] = sp4_subj_gff.Chromosome
@@ -2114,148 +2134,208 @@
         # keeps the rest of selenos
         available_selenos = selenos_annot[~selenos_annot.Sel_family.isin(unavailable_Sel_families)]
         if available_selenos.shape[0] != selenos_annot.shape[0]:
             unavailable_sel = selenos_annot[selenos_annot.Sel_family.isin(unavailable_Sel_families)]
             write(f'Unavailable Selenoprotein families predicted by Selenoprofiles 4:\n\n{unavailable_sel}')
         del selenos_annot
 
-    write('\n### PHASE 0: TBLASTX')
+    write('\n### PHASE 0: TBLASTX', how=colors['phase'])
  
     # first phase of the script is to run a tblastx between the query and subject transcriptomes to get the best
     # alignments among the transcripts.
-    run_tblastx(q_file, subj_file, n_cpu, n_section==0,
-                path_tblastx_outfile)    
-    write(f'\ntBLASTx outfile contains: {buf_count_newlines_gen(path_tblastx_outfile)} alignments')
+    if not os.path.exists(path_tblastx_outfile) or n_section==0:
+        write(description_of_phases[0])
+        run_tblastx(q_file, subj_file, n_cpu, True, #n_section==0,
+                    path_tblastx_outfile+'.tmp')
+        os.rename(path_tblastx_outfile+'.tmp', path_tblastx_outfile)
+        
+        write(f'tblastx file created --> {path_tblastx_outfile}')
+    else:
+        write(f'File found: {path_tblastx_outfile}')
+    write(f'Nº of tBLASTx hits: {buf_count_newlines_gen(path_tblastx_outfile)}', how=colors['count'])
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 1: EXTRACT SEQS')          
+    write('\n### PHASE 1: EXTRACT SEQS', how=colors['phase'])
 
     def mp_join_dfs(x):
         return join_dfs(x, subj_file, q_file)
+
+    run_phase1=False
     # if the output file already exists, we can force any phase rerun with 'n_section' variable
     if not os.path.exists(path_postchunking_outfile) or n_section < 2:
+        write(description_of_phases[1])
         # chunking function allows to open files as iterators, so only a chunk is charged into memory at a time
         chunking(path_tblastx_outfile, n_chunks, 0, mp_join_dfs, 
-                 n_cpu, None, path_postchunking_outfile, n)
-    # we read the last phase outfile 'Chromosome' column (Subject transcripts ID)
-    trans_candidates = pd.read_csv(path_postchunking_outfile, usecols=['Chromosome'],
-                                   sep="\t", header=0, index_col=False)['Chromosome']
-    write(f'\nNº of unique subject transcripts: {len(trans_candidates.unique())}')
-    if benchmark:
-        # and we check how many expected selenoprotein transcripts have successfully passed the filter
-        write(f'TP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
-    del trans_candidates
+                 n_cpu, None, path_postchunking_outfile+'.tmp', n)
+        os.rename(path_postchunking_outfile+'.tmp', path_postchunking_outfile)
+        write(f'Table including sequences created --> {path_postchunking_outfile}')
+        run_phase1=True
+
+    else:
+        write(f'File found: {path_postchunking_outfile}')
+
+    if run_phase1 or benchmark:
+        # we read the last phase outfile 'Chromosome' column (Subject transcripts ID)
+        trans_candidates = pd.read_csv(path_postchunking_outfile, usecols=['Chromosome'],
+                                       sep="\t", header=0, index_col=False)['Chromosome']
+        write(f'Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
+
+        if benchmark:
+            # and we check how many expected selenoprotein transcripts have successfully passed the filter
+            write(f'TP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
+
+        del trans_candidates
+
     # using time_memory_control==True we can know the time and memory (current and peak) in each phase
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 2: FRAGMENTATION')
+    write('\n### PHASE 2: FRAGMENTATION', how=colors['phase'])
 
     if not os.path.exists(path_fragmentation_outfile) or n_section < 3:
+        write(description_of_phases[2])
         chunking(path_postchunking_outfile, n_chunks, 0, fragmentation,
-                 n_cpu, None, path_fragmentation_outfile, n)
+                 n_cpu, None, path_fragmentation_outfile+'.tmp', n)
+        os.rename(path_fragmentation_outfile+'.tmp', path_fragmentation_outfile)
+        write(f'Table with best ORFs selected (for query and subject) per candidate --> {path_fragmentation_outfile}')
+    else:
+        write(f'File found: {path_fragmentation_outfile}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 3: OVERLAPPING FILTER')
+    write('\n### PHASE 3: OVERLAPPING FILTER', how=colors['phase'])
 
+    run_phase3=False
     if not os.path.exists(path_overlapping_outfile) or n_section < 4:
+        write(description_of_phases[3])
         chunking(path_fragmentation_outfile, 0, n_lines, 
                  lambda x: overlapping_filter(x, n_cpu), n_cpu, None,
-                 path_overlapping_outfile, n, overlapping=True, chunk_by_key=True)
-        write(f'\nOverlapping outfile cointains: {buf_count_newlines_gen(path_overlapping_outfile)} alignments')
-    trans_candidates = pd.read_csv(path_overlapping_outfile, usecols=['Chromosome'],
+                 path_overlapping_outfile+'.tmp', n, overlapping=True, chunk_by_key=True)
+        os.rename(path_overlapping_outfile+'.tmp', path_overlapping_outfile)
+        write(f'Table with non-overlapping hits created --> {path_overlapping_outfile}')
+        
+        write(f'After removing overlapping hits, we have: {buf_count_newlines_gen(path_overlapping_outfile)} alignments', how=colors['count'])
+        run_phase3=True
+    else:
+        write(f'File found: {path_overlapping_outfile}')
+
+    if run_phase3 or benchmark:
+        trans_candidates = pd.read_csv(path_overlapping_outfile, usecols=['Chromosome'],
                                    sep="\t", header=0, index_col=False)['Chromosome']
-    write(f'\nNº of unique subject transcripts: {len(trans_candidates.unique())}')
-    if benchmark:
-        write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
-    del trans_candidates
+        write(f'After removing overlapping hits, Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
+
+        if benchmark:
+            write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
+        del trans_candidates
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 4: EXTEND ORFS')
+    write('\n### PHASE 4: EXTEND ORFS', how=colors['phase'])
 
     def mp_ext_orfs(x):
         return run_extend(x, q_file, subj_file)
 
+    run_phase4=False
     if not os.path.exists(path_extend_outfile) or n_section < 5:
+        write(description_of_phases[4])
+
         chunking(path_overlapping_outfile, 0, n_lines, mp_ext_orfs, n_cpu,
-                 None, path_extend_outfile, n, ext_orfs=True, chunk_by_key=True)
-        write(f'\nExtend ORFs outfile cointains: {buf_count_newlines_gen(path_extend_outfile)} alignments')
-    trans_candidates = pd.read_csv(path_extend_outfile, sep="\t", header=0,
+                 None, path_extend_outfile+'.tmp', n, ext_orfs=True, chunk_by_key=True)
+        os.rename(path_extend_outfile+'.tmp', path_extend_outfile)
+        run_phase4=True
+        write(f'Table with non-identical extended ORFs --> {path_extend_outfile}')
+        write(f'Nº of hits with non-identical extended ORFs: {buf_count_newlines_gen(path_extend_outfile)}', how=colors['count'])
+    else:
+        write(f'File found: {path_extend_outfile}')
+
+    if run_phase4 or benchmark:
+        trans_candidates = pd.read_csv(path_extend_outfile, sep="\t", header=0,
                                    index_col=False, usecols=['Chromosome'])['Chromosome']
-    write(f'\nNº of unique subject transcripts: {len(trans_candidates.unique())}')
-    if benchmark:
-        write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
-    del trans_candidates
+        write(f'Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
+        if benchmark:
+            write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
+        del trans_candidates        
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 5: PAIRWISE ALIGNMENT\n')
+    write('\n### PHASE 5: PAIRWISE ALIGNMENT', how=colors['phase'])
 
     if not os.path.exists(path_pairwise_outfile) or n_section < 6:
+        write(description_of_phases[5])
+        
         chunking(path_extend_outfile, n_chunks, 0, pairwise_alignment, n_cpu,
-                 opt['timeout'], path_pairwise_outfile, n, pairwise=True)
+                 opt['timeout'], path_pairwise_outfile+'.tmp', n, pairwise=True)
+        os.rename(path_pairwise_outfile+'.tmp', path_pairwise_outfile)
+        write(f'Table including aligned sequences --> {path_pairwise_outfile}')
+    else:
+        write(f'File found: {path_pairwise_outfile}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 6: UGA ALIGNMENT FILTER')
+    write('\n### PHASE 6: UGA ALIGNMENT FILTER', how=colors['phase'])
 
+    run_phase6=False
     # from this point we stop using chunking(). Now, dataframes are read at once.
     if not os.path.exists(path_candidates_outfile) or n_section < 7:
+        write(description_of_phases[6])
         # as we are not using chunking(), pre-phase file must be read to pass it as arg to the next phase function
         aln_orfs = pd.read_csv(path_pairwise_outfile, sep='\t', header=0, index_col=False)
         # calling function
         candidates_df = UGA_alignments(aln_orfs)
         # saving dataframe as a csv file
         candidates_df = candidates_df \
             .sort_values(by='Score', ascending=False, ignore_index=True) \
             .drop_duplicates('Chromosome', ignore_index=True)
-        candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
-
+        candidates_df.to_csv(path_or_buf=path_candidates_outfile+'.tmp', sep='\t', index=False)
+        os.rename(path_candidates_outfile+'.tmp', path_candidates_outfile)
+        
+        write(f'Table created with candidates --> {path_candidates_outfile}')
+        
+        run_phase6=True
         ##########  MODIFY TO: do chunking if not benchmarking; if benchmark, keep code above
         ###
         
         # else:
         #     chunking(path_pairwise_outfile, n_chunks, 0, UGA_alignments,
         #              n_cpu, None, path_candidates_outfile, n)
         #     candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
     else:
-        write(f'Reading {path_candidates_outfile}')
+        write(f'File found: {path_candidates_outfile}')
         candidates_df = pd.read_csv(path_candidates_outfile, sep='\t', header=0, index_col=False)
         # candidates_df = candidates_df \
         #     .sort_values(by='Score', ascending=False, ignore_index=True) \
         #     .drop_duplicates('Chromosome', ignore_index=True)
         # candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
         # here there is a control to prevent empty dfs to be passed to the next phase causing an error
         if len(candidates_df) == 0:
             write(f'Empty file {candidates_df}')
-    
-    write(f'\nCandidates outfile cointains: {buf_count_newlines_gen(path_candidates_outfile)} candidates')
-    write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
-    if benchmark:
-        write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
+
+    if run_phase6 or benchmark:
+        write(f'After the first filter, Nº of candidates: {buf_count_newlines_gen(path_candidates_outfile)}', how=colors['count'])
+        write(f'Nº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
+        if benchmark:
+            write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 7: EVO-CONSERVATION')
+    write('\n### PHASE 7: FINAL FILTER', how=colors['phase'])
 
     # if not os.path.exists(path_selenocandidates_outfile) or n_section < 8:
     #     candidates_df = evo_conservation(candidates_df, opt['selective_pressure'],
     #                                      opt['max_prot_changes'], opt['dNdS_filter'],
     #                                      opt['cons_up'], opt['cons_down'], q_file, subj_file)
     #     candidates_df.to_csv(path_or_buf=path_selenocandidates_outfile, sep='\t', index=False)
     # else:
@@ -2269,14 +2349,15 @@
     # print(sp4_subj_gff)
     # sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
     #                         'score', 'strand', 'frame', 'attribute', 'subj_id']
     # sp4_subj_gff['sec_start'] -= 1
     # sp4_subj_gff = sp4_subj_gff[sp4_subj_gff['feature'] == 'Selenocysteine'].reset_index(drop=True)
     # print(sp4_subj_gff)
     if not os.path.exists(path_selenocandidates_outfile) or n_section < 8:
+        write(description_of_phases[7])
         if benchmark:
             candidates_df = preprocessing_candidates(candidates_df, q_file, subj_file, sp4_subj_gff=sp4_subj_gff)
             tp = candidates_df[candidates_df.true_positive == True].shape[0]
             fp = candidates_df[candidates_df.true_positive == False].shape[0]
             fn = available_selenos.shape[0] - tp
             precision = round(tp / (tp + fp), 4)
             recall = round(tp / (tp + fn), 4)
@@ -2288,60 +2369,73 @@
         if opt['model'] == 'd':
             lr_filepath = twinstop_libpath + 'logistic_regression_model.def.pkl'
         elif opt['model'] == 'p':
             lr_filepath = twinstop_libpath + 'logistic_regression_model.pre.pkl'
         elif opt['model'] == 's':
             lr_filepath = twinstop_libpath + 'logistic_regression_model.sen.pkl'
 
-        lr_preds, y = regression_filter(candidates_df, lr_filepath)
+        lr_preds, y = regression_filter(candidates_df, lr_filepath, n_cpu)
         candidates_df = candidates_df[lr_preds]
+        candidates_df.sort_values(by='Density_Score', inplace=True,
+                                  ignore_index=True, ascending=False)        
         candidates_df.to_csv(path_or_buf=path_selenocandidates_outfile, sep='\t', index=False)
+        write(f'Table with final set of candidates --> {path_selenocandidates_outfile}')
 
         if benchmark:
             (_, fp_ml, fn_ml, tp_ml) = confusion_matrix(y, lr_preds).ravel()
             precision_ml = round(tp_ml / (tp_ml + fp_ml), 4)
             recall_ml = round(tp_ml / (tp_ml + fn_ml), 4)
             write(f'\nPrecision_lr: {precision_ml}')
             write(f'\nSensitivity_lr: {recall_ml}\n')
             write(f'\nPrecision Twinstop: {precision_ml}')
             write(f'\nSensitivity Twinstop: {recall * recall_ml}\n')
     else:
         candidates_df = pd.read_csv(path_selenocandidates_outfile, sep='\t', header=0, index_col=False)
-
-    write(f'\nSelenocandidates outfile cointains: {buf_count_newlines_gen(path_selenocandidates_outfile)} candidates')
+        write(f'File found: {path_selenocandidates_outfile}')
+        
+    write(f'After final filter, Nº of candidates: {buf_count_newlines_gen(path_selenocandidates_outfile)}', how=colors['count'])
     # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
     # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 8: BLASTP FOR ANNOTATION')
+    if opt['ann']:
+        write('\n### PHASE 8: BLASTP FOR ANNOTATION', how=colors['phase'])
+    else:
+        write('\n### Skipping PHASE 8 because not requested...')
 
     if not 'Annot_Title' in candidates_df and opt['ann']:
+        write(description_of_phases[8])
         candidates_df = run_blastp(candidates_df, opt['ann_db'], n_cpu,
                                    path_blastp_outfile, path_fasta_query_prot_seq)
         candidates_df.sort_values(by='Density_Score', inplace=True,
                                   ignore_index=True, ascending=False)
         candidates_df.to_csv(sep='\t', path_or_buf=path_selenocandidates_annotated_outfile, index=False)
         # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
         # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 9: OUTPUTS')
+    write('\n### PHASE 9: OUTPUTS', how=colors['phase'])
 
+    write(description_of_phases[9])
     candidates_pretty = pretty_output(candidates_df)
+    write(f'Output file with user-readable alignments created --> {path_pretty_outfile}')
     with open(path_pretty_outfile, 'w') as fw:
         fw.write(candidates_pretty)
 
-    outputs(candidates_df, opt['cds_q'], path_cds_q, opt['cds_s'], path_cds_t,
+    make_outputs(candidates_df, opt['cds_q'], path_cds_q, opt['cds_s'], path_cds_t,
             opt['pep_q'], path_pep_q, opt['pep_s'], path_pep_t, opt['gff_q'],
             opt['gff_s'], path_gff_q, path_gff_t)
 
     if time_memory_control:
         time_mem_usage(initial_time)
 
+    write('')
+    write(f' Twinstop completed | at {datetime.now().strftime("%Y-%m-%d %H:%M:%S")} '.center(70, '*'))
+
 if __name__ == '__main__':
     main()
```

### Comparing `twinstop-0.0.5/src/twinstop/test_alignment_methods.py` & `twinstop-0.1.0/src/twinstop/test_alignment_methods.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.0.5/src/twinstop.egg-info/PKG-INFO` & `twinstop-0.1.0/src/twinstop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.0.5
+Version: 0.1.0
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `twinstop-0.0.5/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.1.0/src/twinstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

