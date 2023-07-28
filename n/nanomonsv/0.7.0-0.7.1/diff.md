# Comparing `tmp/nanomonsv-0.7.0.tar.gz` & `tmp/nanomonsv-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomonsv-0.7.0.tar", last modified: Thu Jun 29 06:36:54 2023, max compression
+gzip compressed data, was "nanomonsv-0.7.1.tar", last modified: Fri Jul 28 08:53:56 2023, max compression
```

## Comparing `nanomonsv-0.7.0.tar` & `nanomonsv-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.809836 nanomonsv-0.7.0/nanomonsv/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/cluster_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/count_sread_by_alignment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/nanomonsv/data/
--rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/filt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/gather_support_read_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/generate_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/insert_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/locate_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/locate_bp_sbnd.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/long_read_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/merge_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/my_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/post_proc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/pyssw.py
--rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/smith_waterman.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/ssw_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/swalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/vcf_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/nanomonsv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:36:54.809836 nanomonsv-0.7.0/nanomonsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 06:36:54.000000 nanomonsv-0.7.0/nanomonsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:36:54.813836 nanomonsv-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-29 06:36:40.000000 nanomonsv-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20822 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/cluster_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21130 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/count_sread_by_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   147053 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    79292 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)   152156 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    82867 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/gather_support_read_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/generate_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/insert_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/locate_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/locate_bp_sbnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/long_read_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/merge_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/my_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/post_proc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15065 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/pyssw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30170 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/smith_waterman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/ssw_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/swalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/vcf_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/nanomonsv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/nanomonsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 08:53:56.000000 nanomonsv-0.7.1/nanomonsv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:53:56.663528 nanomonsv-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-28 08:53:45.000000 nanomonsv-0.7.1/setup.py
```

### Comparing `nanomonsv-0.7.0/LICENSE` & `nanomonsv-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/PKG-INFO` & `nanomonsv-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -40,31 +40,28 @@
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
 Python (tested with >=3.6), pysam, numpy, parasail
 
-> [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
 nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
-> ##### For use of SSW Library
-> Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
 `bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
@@ -126,34 +123,35 @@
 The Oxford Nanopore Sequencing data used in the bioRxiv paper is available through the public sequence repository service (BioProject ID: PRJDB10898):
 - COLO829: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248304[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248305[accn])
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
-Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
+Also, please kindly cite the [NAR paper](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946) when you use these data.
 
 See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
 
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
-nanomonsv parse [-h] [--debug]
+nanomonsv parse [-h] [--reference_fasta reference.fa] [--debug]
                 [--split_alignment_check_margin SPLIT_ALIGNMENT_CHECK_MARGIN]
                 [--minimum_breakpoint_ambiguity MINIMUM_BREAKPOINT_AMBIGUITY]
-                bam_file output_prefix
+                alignment_file output_prefix
 ```
-- **bam_file**: Path to input indexed BAM file
+- **alignment_file**: Path to input indexed BAM or CRAM file
 - **output_prefix**: Output file prefix
 
 See the help (`nanomonsv parse -h`) for other options.
+From v0.7.0, nanomonsv can accept CRAM format files. For CRAM files, we recommend to add the PATH to the reference genome file by `--reference_fasta`.
 
 After successful completion, you will find supporting reads stratified by deletions, insertions, and rearrangements: 
 ({output_prefix}.deletion.sorted.bed.gz, {output_prefix}.insertion.sorted.bed.gz, {output_prefix}.rearrangement.sorted.bedpe.gz, and {output_prefix}.bp_info.sorted.bed.gz and their indexes (.tbi files). 
 
 
 ### get
 
@@ -165,15 +163,16 @@
               [--min_tumor_variant_read_num MIN_TUMOR_VARIANT_READ_NUM]
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
-              [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
+              [--var_read_min_mapq VAR_READ_MIN_MAPQ]
+              [--qv10] [--qv15] [--qv20] [--qv25] [--use_racon]
               [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
               [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
@@ -185,14 +184,20 @@
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
 You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
 
+From v0.7.0, we prepared preset parameter options:
+- **--qv10**: Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5
+- **--qv15**: Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.
+- **--qv20**: Parameter preset for sequencing data with a base quality of around 20. Recommended for ONT data with Q20+ chemistry.
+- **--qv25**: Parameter preset for sequencing data with a base quality above 25. Recommended for PacBio Hifi data.
+  
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint,
```

### Comparing `nanomonsv-0.7.0/README.md` & `nanomonsv-0.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,28 @@
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
 Python (tested with >=3.6), pysam, numpy, parasail
 
-> [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
 nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
-> ##### For use of SSW Library
-> Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
 `bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
@@ -106,34 +103,35 @@
 The Oxford Nanopore Sequencing data used in the bioRxiv paper is available through the public sequence repository service (BioProject ID: PRJDB10898):
 - COLO829: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248304[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248305[accn])
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
-Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
+Also, please kindly cite the [NAR paper](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946) when you use these data.
 
 See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
 
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
-nanomonsv parse [-h] [--debug]
+nanomonsv parse [-h] [--reference_fasta reference.fa] [--debug]
                 [--split_alignment_check_margin SPLIT_ALIGNMENT_CHECK_MARGIN]
                 [--minimum_breakpoint_ambiguity MINIMUM_BREAKPOINT_AMBIGUITY]
-                bam_file output_prefix
+                alignment_file output_prefix
 ```
-- **bam_file**: Path to input indexed BAM file
+- **alignment_file**: Path to input indexed BAM or CRAM file
 - **output_prefix**: Output file prefix
 
 See the help (`nanomonsv parse -h`) for other options.
+From v0.7.0, nanomonsv can accept CRAM format files. For CRAM files, we recommend to add the PATH to the reference genome file by `--reference_fasta`.
 
 After successful completion, you will find supporting reads stratified by deletions, insertions, and rearrangements: 
 ({output_prefix}.deletion.sorted.bed.gz, {output_prefix}.insertion.sorted.bed.gz, {output_prefix}.rearrangement.sorted.bedpe.gz, and {output_prefix}.bp_info.sorted.bed.gz and their indexes (.tbi files). 
 
 
 ### get
 
@@ -145,15 +143,16 @@
               [--min_tumor_variant_read_num MIN_TUMOR_VARIANT_READ_NUM]
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
-              [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
+              [--var_read_min_mapq VAR_READ_MIN_MAPQ]
+              [--qv10] [--qv15] [--qv20] [--qv25] [--use_racon]
               [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
               [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
@@ -165,14 +164,20 @@
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
 You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
 
+From v0.7.0, we prepared preset parameter options:
+- **--qv10**: Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5
+- **--qv15**: Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.
+- **--qv20**: Parameter preset for sequencing data with a base quality of around 20. Recommended for ONT data with Q20+ chemistry.
+- **--qv25**: Parameter preset for sequencing data with a base quality above 25. Recommended for PacBio Hifi data.
+  
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint,
```

### Comparing `nanomonsv-0.7.0/nanomonsv/arg_parser.py` & `nanomonsv-0.7.1/nanomonsv/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,16 +111,19 @@
 
     get.add_argument("--var_read_min_mapq", default = 0, type = int,
                      help = "Threshould for mapping quality in validate step (default: 0)")
 
     get.add_argument("--validation_score_ratio_thres", default = 1.2, type = float,
                      help = "Threshould for threshould for SV segment validation by alignment")
 
-    get.add_argument("--use_ssw_lib", default = False, action = 'store_true',
-                     help = "Use SSW Library. This is for backward comaptibility, and may be removed in the future (default: False)")
+    get.add_argument("--sw_jump_params", nargs = 4, default = [1, 3, 3, 2], type = int,
+                     help = "Parameters (match score, mismatch penalty, gap penalty, insertion penalty) for one-time smith-waterman algorithm (default: [1, 3, 3, 2]")
+
+    # get.add_argument("--use_ssw_lib", default = False, action = 'store_true',
+    #                  help = "Use SSW Library. This is for backward comaptibility, and may be removed in the future (default: False)")
 
     get.add_argument("--qv10", default = False, action = 'store_true',
                      help = "Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5")
 
     get.add_argument("--qv15", default = False, action = 'store_true',
                      help = "Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.")
```

### Comparing `nanomonsv-0.7.0/nanomonsv/cluster.py` & `nanomonsv-0.7.1/nanomonsv/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,27 +344,29 @@
             cl = self.sv_cluster_list[i]
             if current_chr != cl.chr1 or current_pos > cl.end1 + self.cluster_margin_size:
                 remove_cluster.append(cl)
 
                 if self.svtype == "rearrangement":
 
                     if self.filter_rearrangement_cluster(cl): continue
-                    print_line_readids = ';'.join(cl.readids)
+                    # print_line_readids = ';'.join(cl.readids)
+                    print_line_readids = repr(cl.readids)
                     print_line_info1 = ';'.join(cl.info1)
                     print_line_info2 = ';'.join(cl.info2)
         
                     print(f'{cl.chr1}\t{cl.start1}\t{cl.end1}\t{cl.chr2}\t{cl.start2}\t{cl.end2}\t' +
                         f'{print_line_readids}\t0\t{cl.dir1}\t{cl.dir2}\t{print_line_info1}\t{print_line_info2}',
                         file = self.hout)
 
                 elif self.svtype in ["insertion", "deletion"]:
 
                     matched_control_margin_choice = 100 if self.svtype == "insertion" else 10
                     if self.filter_indel_cluster(cl, matched_control_margin = matched_control_margin_choice): continue
-                    print_line_readids = ';'.join(cl.readids)
+                    # print_line_readids = ';'.join(cl.readids)
+                    print_line_readids = repr(cl.readids)
                     print_line_size = ';'.join([str(x) for x in cl.size])
                     print_line_info1 = ';'.join(cl.info1)
 
                     print(f'{cl.chr1}\t{cl.start1}\t{cl.end1}\t{cl.chr2}\t{cl.start2}\t{cl.end2}\t' +
                         f'{print_line_readids}\t0\t{cl.dir1}\t{cl.dir2}\t{print_line_size}\t{print_line_info1}',
                         file = self.hout)
```

### Comparing `nanomonsv-0.7.0/nanomonsv/cluster_sbnd.py` & `nanomonsv-0.7.1/nanomonsv/cluster_sbnd.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,16 @@
         remove_cluster = []
         for i in range(len(self.sbnd_cluster_list)):
             cl = self.sbnd_cluster_list[i]
             if current_chr != cl.chr or current_pos > cl.end + self.cluster_margin_size:
                 remove_cluster.append(cl)
 
                 if self.filter_single_breakend_cluster(cl): continue
-                print_line_readids = ';'.join(cl.readids)
+                # print_line_readids = ';'.join(cl.readids)
+                print_line_readids = repr(cl.readids)
                 print_line_info = ';'.join(cl.info)
         
                 print(f'{cl.chr}\t{cl.start}\t{cl.end}\t{print_line_readids}\t0\t{cl.dir}\t{print_line_info}',
                     file = self.hout)
                         
         for cl in remove_cluster:
             self.sbnd_cluster_list.remove(cl)
```

### Comparing `nanomonsv-0.7.0/nanomonsv/count_sread_by_alignment.py` & `nanomonsv-0.7.1/nanomonsv/count_sread_by_alignment.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz` & `nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg19.bed.gz.tbi` & `nanomonsv-0.7.1/nanomonsv/data/LINE1.hg19.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz` & `nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/data/LINE1.hg38.bed.gz.tbi` & `nanomonsv-0.7.1/nanomonsv/data/LINE1.hg38.bed.gz.tbi`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/filt.py` & `nanomonsv-0.7.1/nanomonsv/filt.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/gather_support_read_seq.py` & `nanomonsv-0.7.1/nanomonsv/gather_support_read_seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     # readid2alignment = {}
     cid = 0
     with open(input_file, 'r') as hin:
         for line in hin:
             F = line.rstrip('\n').split('\t')
             key = f"{F[0]},{F[1]},{F[2]},{F[8]},{F[3]},{F[4]},{F[5]},{F[9]},{mode},{cid}"
                 # ','.join([F[0], F[1], F[2], F[8], F[3], F[4], F[5], F[9], mode])
-            readids = F[6].split(';')
+            # readids = F[6].split(';')
+            readids = eval(F[6])
 
             if mode == "r":
                 info1 = F[10].split(';')
                 info2 = F[11].split(';')
                 for i in range(len(readids)):
                     tinfo1 = info1[i].split(',') 
                     tinfo2 = info2[i].split(',')
@@ -70,15 +71,17 @@
 
     cid = 0
     with open(input_file, 'r') as hin:
         for line in hin:
             tchr, tstart, tend, treadids, _, tstrand, tinfos = line.rstrip('\n').split('\t')
             tkey = f"{tchr},{tstart},{tend},{tstrand},b,{cid}" # ','.join([tchr, tstart, tend, tstrand])
            
-            readids = treadids.split(';')
+            # readids = treadids.split(';')
+            readids = eval(treadids)
+
             infos = tinfos.split(';') 
             for i in range(len(readids)):
                 ttinfo = infos[i].split(',')
                 qpos, qlen, qstrand = int(ttinfo[1]), int(ttinfo[3]), ttinfo[4]             
                 if readids[i] not in readid2alignment_sbnd: readid2alignment_sbnd[readids[i]] = []
                 if tstrand == qstrand: 
                     readid2alignment_sbnd[readids[i]].append((tkey, max(1, qpos - alignment_margin), qlen, qstrand, '*'))
```

### Comparing `nanomonsv-0.7.0/nanomonsv/generate_consensus.py` & `nanomonsv-0.7.1/nanomonsv/generate_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/insert_classify.py` & `nanomonsv-0.7.1/nanomonsv/insert_classify.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/locate_bp.py` & `nanomonsv-0.7.1/nanomonsv/locate_bp.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from . import smith_waterman
 from .my_seq import reverse_complement
 from .logger import get_logger
 
 logger = get_logger(__name__)
 
 
-def get_refined_bp(contig, fasta_file_ins, chr1, start1, end1, dir1, chr2, start2, end2, dir2, mode, h_log, rd_margin = 20, i_margin = 500):
+def get_refined_bp(contig, fasta_file_ins, chr1, start1, end1, dir1, chr2, start2, end2, dir2, mode, h_log, 
+                   sw_jump_params, rd_margin = 20, i_margin = 500):
 
     start1 = max(1, start1)
     start2 = max(1, start2)
 
     if mode != "i":
 
         ref_len1 = fasta_file_ins.get_reference_length(chr1)
@@ -28,15 +29,18 @@
 
         region1_seq = fasta_file_ins.fetch(chr1, bstart1 - 1, bend1)
         region2_seq = fasta_file_ins.fetch(chr2, bstart2 - 1, bend2)
 
         if dir1 == '-': region1_seq = reverse_complement(region1_seq)
         if dir2 == '+': region2_seq = reverse_complement(region2_seq)
 
-        sret = smith_waterman.sw_jump(contig, region1_seq, region2_seq)
+        sret = smith_waterman.sw_jump(contig, region1_seq, region2_seq,
+                                      match_score = sw_jump_params[0], mismatch_penalty = sw_jump_params[1],
+                                      gap_cost = sw_jump_params[2], jump_cost = sw_jump_params[3])
+
         if sret is None: return(None)
         score, contig_align, region1_align, region2_align, contig_seq, region_seq = sret
 
         bp_pos1 = bstart1 + region1_align[1] - 1 if dir1 == '+' else bend1 - region1_align[1] + 1 
         bp_pos2 = bstart2 + region2_align[0] - 1 if dir2 == '-' else bend2 - region2_align[0] + 1
 
         if contig_align[2] - contig_align[1] == 1:
@@ -55,15 +59,18 @@
     
     else:
     
         contig_start = contig[:min(i_margin, len(contig))]
         contig_end = contig[-min(i_margin, len(contig)):]
 
         region_seq = fasta_file_ins.fetch(chr1, max(0, start1 - 100), end2 + 100)
-        sret = smith_waterman.sw_jump(region_seq, contig_start, contig_end)
+        sret = smith_waterman.sw_jump(region_seq, contig_start, contig_end,
+                                      match_score = sw_jump_params[0], mismatch_penalty = sw_jump_params[1], 
+                                      gap_cost = sw_jump_params[2], jump_cost = sw_jump_params[3])
+
         if sret is None: return(None)
         score, region_align, contig_start_align, contig_end_align, region_seq, contig_seq = sret
 
         bp_pos1 = max(0, start1 - 100) + region_align[1]
         bp_pos2 = max(0, start1 - 100) + region_align[2]
 
         inseq_start = contig_start_align[1]
@@ -74,27 +81,27 @@
         print(region_seq, file = h_log)
         print(contig_seq, file = h_log)
 
         return(bp_pos1, bp_pos2, inseq)
 
         
  
-def locate_bp(consensus_file, output_file, reference_fasta, debug):
+def locate_bp(consensus_file, output_file, reference_fasta, sw_jump_params, debug):
 
     fasta_file_ins = pysam.FastaFile(reference_fasta)
 
     with open(consensus_file, 'r') as hin, open(output_file, 'w') as hout, \
         open(output_file + ".locate_bp.log", 'w') as hout_log:
         for line in hin:
             F = line.rstrip('\n').split('\t')
             temp_key, tconsensus = F[0], F[1]
             print(temp_key + '\n' + tconsensus, file = hout_log)
             chr1, start1, end1, dir1, chr2, start2, end2, dir2, mode, cid = temp_key.split(',')
             start1, end1, start2, end2 = int(start1), int(end1), int(start2), int(end2)       
-            bret = get_refined_bp(tconsensus, fasta_file_ins, chr1, start1, end1, dir1, chr2, start2, end2, dir2, mode, hout_log)
+            bret = get_refined_bp(tconsensus, fasta_file_ins, chr1, start1, end1, dir1, chr2, start2, end2, dir2, mode, hout_log, sw_jump_params)
             if bret is not None:  
                 bp_pos1, bp_pos2, inseq = bret 
                 print(bp_pos1, bp_pos2, inseq, file = hout_log)
                 print('', file = hout_log)
                 print(f"{chr1}\t{bp_pos1}\t{dir1}\t{chr2}\t{bp_pos2}\t{dir2}\t{inseq}\t{mode}_{cid}", file = hout)
                 # print('\t'.join([chr1, str(bp_pos1), dir1, chr2, str(bp_pos2), dir2, inseq]), file = hout)
```

### Comparing `nanomonsv-0.7.0/nanomonsv/locate_bp_sbnd.py` & `nanomonsv-0.7.1/nanomonsv/locate_bp_sbnd.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/long_read_validate.py` & `nanomonsv-0.7.1/nanomonsv/long_read_validate.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/merge_control.py` & `nanomonsv-0.7.1/nanomonsv/merge_control.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/my_seq.py` & `nanomonsv-0.7.1/nanomonsv/my_seq.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/parse.py` & `nanomonsv-0.7.1/nanomonsv/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,28 +207,30 @@
             # if abs(qpos2[1] - qpos1[2]) <= split_alignment_check_margin:
             if qpos2[1] - qpos1[2] <= split_alignment_check_margin1 and qpos1[2] - qpos2[1] <= split_alignment_check_margin2:
                 bp_flag = True
                 tchr1, tstart1, tend1, tmapQ1, tnumM1, tnumI1, tnumD1, tis_supp1, tis_2nd1 = query2target[qpos1]
                 tchr2, tstart2, tend2, tmapQ2, tnumM2, tnumI2, tnumD2, tis_supp2, tis_2nd2 = query2target[qpos2]
                 
                 if qpos2[1] - qpos1[2] > 0:
-                    outward_ambiguity, inward_ambiguity = minimum_ambiguity, max(qpos2[1] - qpos1[2], minimum_ambiguity)
+                    outward_ambiguity, inward_ambiguity = max(qpos2[1] - qpos1[2], minimum_ambiguity), minimum_ambiguity
                 else:
-                    outward_ambiguity, inward_ambiguity = max(qpos1[2] - qpos2[1], minimum_ambiguity), minimum_ambiguity
+                    outward_ambiguity, inward_ambiguity = minimum_ambiguity, max(qpos1[2] - qpos2[1], minimum_ambiguity)
+                
                 
                 bchr1, bchr2 = tchr1, tchr2
                 if qpos1[4] == '+': 
                     bstart1, bend1, bstrand1 = max(int(tend1) - inward_ambiguity, 0), int(tend1) + outward_ambiguity, '+'
                 else:
                     bstart1, bend1, bstrand1 = max(int(tstart1) - outward_ambiguity, 0), int(tstart1) + inward_ambiguity, '-'
                 
                 if qpos2[4] == '+': 
                     bstart2, bend2, bstrand2 = max(int(tstart2) - outward_ambiguity, 0), int(tstart2) + inward_ambiguity, '-'
                 else:
                     bstart2, bend2, bstrand2 = max(int(tend2) - inward_ambiguity, 0), int(tend2) + outward_ambiguity, '+'
+
                 
                 bread_name = qpos1[0]
                 
                 binfo1 = ','.join([str(qpos1[1]), '*', str(qpos1[2]), str(qpos1[3]), qpos1[4], tmapQ1, tnumM1, tnumI1, tnumD1, tis_supp1, tis_2nd1])
                 binfo2 = ','.join([str(qpos2[1]), '*', str(qpos2[2]), str(qpos2[3]), qpos2[4], tmapQ2, tnumM2, tnumI2, tnumD2, tis_supp2, tis_2nd2])
                 
                 if bchr1 > bchr2 or (bchr1 == bchr2 and bstart1 > bstart2):
```

### Comparing `nanomonsv-0.7.0/nanomonsv/post_proc.py` & `nanomonsv-0.7.1/nanomonsv/post_proc.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/pyssw.py` & `nanomonsv-0.7.1/nanomonsv/pyssw.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/run.py` & `nanomonsv-0.7.1/nanomonsv/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     generate_consensus_sbnd(args.tumor_prefix + ".support_read_seq.sbnd.%d.txt" % (index),
         args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
         use_racon = args.use_racon, debug = args.debug, max_memory_minimap2 = args.max_memory_minimap2)
 
     logger.info("Locating single-base resolution break points for candidate SVs (%d)" % (index))
     locate_bp(args.tumor_prefix + ".consensus_seq.%d.txt" % (index),
         args.tumor_prefix + ".refined_bp.%d.txt" % (index),
-        args.reference_fasta, args.debug)
+        args.reference_fasta, args.sw_jump_params, args.debug)
     locate_bp_sbnd(args.tumor_prefix + ".consensus_seq.sbnd.%d.txt" % (index),
         args.tumor_prefix + ".refined_bp.sbnd.%d.txt" % (index),
         args.reference_fasta, args.debug)
 
     logger.info("Counting the number of supporting read for the tumor by realignment of SV candidate segments (%d)" % (index))
     count_sread_by_alignment(
         args.tumor_prefix + ".refined_bp.%d.txt" % (index), 
@@ -212,20 +212,24 @@
     # parameter preset 
     if sum([int(x == True) for x in [args.qv10, args.qv15, args.qv20, args.qv25]]) > 1:
         logger.error("Parameter preset (qv10, qv15, qv20, qv25) should be set only once")
         sys.exit(1)
 
     if args.qv10:
         args.validation_score_ratio_thres = 1.2
+        args.sw_jump_params = [1, 2, 2, 2]
     elif args.qv15:
         args.validation_score_ratio_thres = 1.4
+        args.sw_jump_params = [1, 3, 3, 2]
     elif args.qv20: 
         args.validation_score_ratio_thres = 1.6
+        args.sw_jump_params = [1, 4, 4, 2]
     elif args.qv25:
         args.validation_score_ratio_thres = 1.8
+        args.sw_jump_params = [1, 6, 6, 2]
 
     # check existences
     is_exists_bam(args.tumor_bam)
     is_exists(args.reference_fasta)
     if args.control_bam is not None: is_exists_bam(args.control_bam)
    
     # check parsed files existences
```

### Comparing `nanomonsv-0.7.0/nanomonsv/smith_waterman.py` & `nanomonsv-0.7.1/nanomonsv/smith_waterman.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 #! /usr/bin/env python3
 
 import numpy as np
 
-def sw_jump(contig, region1_seq, region2_seq, match_score = 1, mismatch_penalty = 2, gap_cost = 2, jump_cost = 2):
+def sw_jump(contig, region1_seq, region2_seq, match_score = 1, mismatch_penalty = 2, gap_cost = 2, jump_cost = 2, minimum_score = 10):
 
     H1 = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int32)
     H1_path = np.zeros((len(contig) + 1, len(region1_seq) + 1), np.int32)
     H2 = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
     H2_path = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
     H2_origin_i = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
     H2_origin_j = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
-    # jump_ind = np.zeros((len(contig) + 1), np.int)
+    H2_origin_score = np.zeros((len(contig) + 1, len(region2_seq) + 1), np.int32)
 
     
     for i in range(1, H1.shape[0]):
         for j in range(1, H1.shape[1]):
             match = H1[i - 1, j - 1] + (match_score if contig[i - 1] == region1_seq[j - 1] else - mismatch_penalty)
             delete = H1[i - 1, j] - gap_cost
             insert = H1[i, j - 1] - gap_cost
-            tscores = (0, match, delete, insert)
+            tscores = (float("-inf"), match, delete, insert)
             H1[i, j] = max(tscores)
             H1_path[i,j] = tscores.index(max(tscores))
 
     H1_max = np.amax(H1, axis = 1)
     H1_argmax = np.argmax(H1, axis = 1)
 
     for i in range(1, H2.shape[0]):
         for j in range(1, H2.shape[1]):
             match = H2[i - 1, j - 1] + (match_score if contig[i - 1] == region2_seq[j - 1] else - mismatch_penalty)
             delete = H2[i - 1, j] - gap_cost
             insert = H2[i, j - 1] - gap_cost
 
-            jump = np.max(H1_max[:i]) + (match_score if contig[i - 1] == region2_seq[j - 1] else - mismatch_penalty)
-            jump_diff = i - np.argmax(H1_max[:i])
-            jump = jump - jump_cost * np.log(jump_diff)
+            jump = float("-inf")
+            org_i = np.argmax(H1_max[:i])
+            if H1_max[org_i] >= minimum_score:
+
+                jump = H1_max[org_i] + (match_score if contig[i - 1] == region2_seq[j - 1] else - mismatch_penalty)
+                jump_diff = i - org_i
+                jump = jump - jump_cost * np.log(jump_diff)
  
-            tscores = (0, match, delete, insert, jump)
+            tscores = (float("-inf"), match, delete, insert, jump)
             H2[i, j] = max(tscores)
             H2_path[i, j] = tscores.index(max(tscores))
 
             if H2_path[i, j] == 4:
                 H2_origin_i[i, j] = np.argmax(H1_max[:i])
                 H2_origin_j[i, j]  = H1_argmax[H2_origin_i[i, j]]
+                H2_origin_score[i, j] = H1_max[org_i]
 
-
-    i_cur, j2_cur = np.unravel_index(H2.argmax(), H2.shape)
+    # i_cur, j2_cur = np.unravel_index(H2.argmax(), H2.shape)
     # a_string, b_string = a[i_end - 1], b[j_end - 1]
+    if np.max(H2[H2.shape[0] - 1, :]) >= np.max(H2[:, H2.shape[1] - 1]):
+        j2_cur = np.unravel_index(H2[H2.shape[0] - 1, :].argmax(), (1, H2.shape[1]))[1]
+        i_cur = H2.shape[0] - 1
+    else:
+        j2_cur = H2.shape[1] - 1 
+        i_cur = np.unravel_index(H2[:, H2.shape[1] - 1].argmax(), (H2.shape[0], 1))[0]
+
+
     contig_match, region1_seq_match, region2_seq_match = '', '', ''
     i_end, i2_end, j2_end = i_cur, i_cur, j2_cur # one-based position
 
     match_count, deletion_count, insertion_count, jump_count = 0, 0, 0, 0
+    H1_score = 0
     scores = []
 
     while i_cur > 0 and j2_cur > 0:
         scores.append(H2[i_cur, j2_cur])
         if H2_path[i_cur, j2_cur] == 1:
             contig_match, region2_seq_match = contig[i_cur - 1] + contig_match, region2_seq[j2_cur - 1] + region2_seq_match
             i_cur, j2_cur = i_cur - 1, j2_cur - 1
@@ -66,27 +79,28 @@
             contig_match, region2_seq_match = '-' + contig_match, region2_seq[j2_cur - 1] + region2_seq_match
             i_cur, j2_cur = i_cur, j2_cur - 1
             insertion_count = insertion_count + 1
         elif H2_path[i_cur, j2_cur] ==  4:
             contig_match, region2_seq_match = contig[i_cur - 1] + contig_match, region2_seq[j2_cur - 1] + region2_seq_match
             i1_end = H2_origin_i[i_cur, j2_cur]
             j1_end = H2_origin_j[i_cur, j2_cur]
+            H1_score = H2_origin_score[i_cur, j2_cur]
             i2_start = i_cur
             j2_start = j2_cur # one-based alignment start of second fragment
             """
             i2_start, i1_end = i_cur, i_cur - 1
             j2_start = j2_cur # one-based alignment start of second fragment
             i_cur = i_cur - 1
             """
             jump_count = jump_count + 1
             break
         elif H2_path[i_cur, j2_cur] == 0:
             break
 
-    if jump_count == 0:
+    if H1_score < minimum_score or H2.max() - H1_score < minimum_score or jump_count == 0:
         return(None)
 
     contig_match = ' ' + contig_match
     # j1_end = H1_argmax[i_cur]
     j1_cur = j1_end
     i_cur = i1_end
```

### Comparing `nanomonsv-0.7.0/nanomonsv/ssw_lib.py` & `nanomonsv-0.7.1/nanomonsv/ssw_lib.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/swalign.py` & `nanomonsv-0.7.1/nanomonsv/swalign.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/utils.py` & `nanomonsv-0.7.1/nanomonsv/utils.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv/vcf_convert.py` & `nanomonsv-0.7.1/nanomonsv/vcf_convert.py`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/nanomonsv.egg-info/PKG-INFO` & `nanomonsv-0.7.1/nanomonsv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomonsv
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python tools for detecting structural variation from nanopore sequence data
 Home-page: https://github.com/friend1ws/nanomonsv
 Author: Yuichi Shiraishi
 Author-email: friend1ws@gamil.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -40,31 +40,28 @@
 ### Binary programs
 
 [htslib](http://www.htslib.org/), [mafft](https://mafft.cbrc.jp/alignment/software/), [racon](https://github.com/isovic/racon)(optional from ver. 0.3.0. However, we recommend to use this option. Add --use_racon option when you perfrom get command.)
 
 ### Python
 Python (tested with >=3.6), pysam, numpy, parasail
 
-> [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) (This became optional since version 0.2.0. We have changed the main engine of Smith-Waterman algorithm to parasail.)
 
 
 ### For advanced use (`insert_classify` command)
 [bwa](https://github.com/lh3/bwa), [minimap2](https://github.com/lh3/minimap2), [bedtools](https://bedtools.readthedocs.io/en/latest/), [RepeatMasker](http://www.repeatmasker.org/)
 
 ## Preparation
 
 ### For basic use (`parse`, `get` command)
 
 #### Install software and add them to the PATH
 
 nanomonsv uses, `tabix`, `bgzip` (which are part of HTSlib projects) and `mafft` inside the program,
 assuming those are installed, and the paths are already added to the running environment.
 
-> ##### For use of SSW Library
-> Since version 0.2.0, nanomonsv can be executed without SSW Library. When users want to use SSW Library, create the libssw.so and add the path to the LD_LIBRARY_PATH environment variable. Please refer the **How to use the Python wrapper ssw_lib.py** section in the [SSW Library](https://github.com/mengyao/Complete-Striped-Smith-Waterman-Library) repository page.
 
 ###### For use of racon
 Since version 0.3.0, we support racon for the step where generating consensus sequence and get single-base resolution breakpoints. racon may become the default instead of mafft in the future.
 
 
 ### For advanced use (`insert_classify` command)
 `bwa`, `minimap2`, `bedtools` and `RepeatMasker` are required to be installed and these paths are added to the running environment.
@@ -126,34 +123,35 @@
 The Oxford Nanopore Sequencing data used in the bioRxiv paper is available through the public sequence repository service (BioProject ID: PRJDB10898):
 - COLO829: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248304[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248305[accn])
 - H2009: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248308[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248309[accn])
 - HCC1954: [tumor](https://www.ncbi.nlm.nih.gov/sra/DRX248306[accn]), [control](https://www.ncbi.nlm.nih.gov/sra/DRX248307[accn])
 
 The results of nanomonsv for the above data are available [here](https://github.com/friend1ws/nanomonsv/tree/master/misc/example).
 When you perform nanomonsv to the above data and have experienced errors, please report to us.
-Also, please kindly cite the [bioRxiv paper](https://www.biorxiv.org/content/10.1101/2020.07.22.214262v1) when you use these data.
+Also, please kindly cite the [NAR paper](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkad526/7201946) when you use these data.
 
 See tutorial [wiki page](https://github.com/friend1ws/nanomonsv/wiki/Tutorial) for an example workflow on analyzing COLO829 sample.
 
 ## Commands
 
 ### parse
 
 This step parses all the supporting reads of putative somatic SVs.
 
 ```
-nanomonsv parse [-h] [--debug]
+nanomonsv parse [-h] [--reference_fasta reference.fa] [--debug]
                 [--split_alignment_check_margin SPLIT_ALIGNMENT_CHECK_MARGIN]
                 [--minimum_breakpoint_ambiguity MINIMUM_BREAKPOINT_AMBIGUITY]
-                bam_file output_prefix
+                alignment_file output_prefix
 ```
-- **bam_file**: Path to input indexed BAM file
+- **alignment_file**: Path to input indexed BAM or CRAM file
 - **output_prefix**: Output file prefix
 
 See the help (`nanomonsv parse -h`) for other options.
+From v0.7.0, nanomonsv can accept CRAM format files. For CRAM files, we recommend to add the PATH to the reference genome file by `--reference_fasta`.
 
 After successful completion, you will find supporting reads stratified by deletions, insertions, and rearrangements: 
 ({output_prefix}.deletion.sorted.bed.gz, {output_prefix}.insertion.sorted.bed.gz, {output_prefix}.rearrangement.sorted.bedpe.gz, and {output_prefix}.bp_info.sorted.bed.gz and their indexes (.tbi files). 
 
 
 ### get
 
@@ -165,15 +163,16 @@
               [--min_tumor_variant_read_num MIN_TUMOR_VARIANT_READ_NUM]
               [--min_tumor_VAF MIN_TUMOR_VAF]
               [--max_control_variant_read_num MAX_CONTROL_VARIANT_READ_NUM]
               [--max_control_VAF MAX_CONTROL_VAF]
               [--cluster_margin_size CLUSTER_MARGIN_SIZE]
               [--median_mapQ_thres MEDIAN_MAPQ_THRES]
               [--max_overhang_size_thres MAX_OVERHANG_SIZE_THRES]
-              [--var_read_min_mapq VAR_READ_MIN_MAPQ] [--use_ssw_lib] [--use_racon]
+              [--var_read_min_mapq VAR_READ_MIN_MAPQ]
+              [--qv10] [--qv15] [--qv20] [--qv25] [--use_racon]
               [--single_bnd] [--threads THREADS] [--processes PROCESSES] 
               [--sort_option SORT_OPTION] [--max_memory_minimap2] [--debug]
               tumor_prefix tumor_bam reference.fa
  ```
  - **tumor_prefix**: Prefix to the tumor data set in the parse step
  - **tumor_bam**: Path to input indexed BAM file
  - **reference.fa**: Path to reference genome used for the alignment
@@ -185,14 +184,20 @@
 - **control_bam**: Path to the matched control BAM file
 
 When you use the control panel (recommended!), use the following argument.
 - **control_panel_prefix**: Prefix of non-matched control panel data processed in merge_control step.
 
 You can also use **--process** to use multi-processing mode. Currently, we do not recommend using **--thread** option.
 
+From v0.7.0, we prepared preset parameter options:
+- **--qv10**: Parameter preset for sequencing data with a base quality of around 10. Recommended for ONT data called by Guppy before version 5
+- **--qv15**: Parameter preset for sequencing data with a base quality of around 15. Recommended for ONT data called by Guppy version 5, 6.
+- **--qv20**: Parameter preset for sequencing data with a base quality of around 20. Recommended for ONT data with Q20+ chemistry.
+- **--qv25**: Parameter preset for sequencing data with a base quality above 25. Recommended for PacBio Hifi data.
+  
 After successful execution, you will be able to find the result file names as {tumor_prefix}.nanomonsv.result.txt.
 See the help (`nanomonsv get -h`) for other options. 
 
 When you want to change the engine of Smith-Waterman algorithm to SSW Library, specify `--use_ssw_lib` option,
 though we do not generally recommend this.
 
 Also, we basically recommend using `--use_racon` option. This will slightly improve the identification of single-base resolution breakpoint,
```

### Comparing `nanomonsv-0.7.0/nanomonsv.egg-info/SOURCES.txt` & `nanomonsv-0.7.1/nanomonsv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomonsv-0.7.0/setup.py` & `nanomonsv-0.7.1/setup.py`

 * *Files identical despite different names*

