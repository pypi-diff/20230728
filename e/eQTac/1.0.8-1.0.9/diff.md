# Comparing `tmp/eQTac-1.0.8.tar.gz` & `tmp/eQTac-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.8.tar", last modified: Thu Apr 20 07:29:19 2023, max compression
+gzip compressed data, was "eQTac-1.0.9.tar", last modified: Fri Jul 28 03:17:31 2023, max compression
```

## Comparing `eQTac-1.0.8.tar` & `eQTac-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.718642 eQTac-1.0.8/
--rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5925 2023-04-20 07:29:19.716647 eQTac-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5428 2023-04-20 07:28:59.000000 eQTac-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.590985 eQTac-1.0.8/eQTac/
--rw-rw-rw-   0        0        0        0 2023-04-19 08:08:46.000000 eQTac-1.0.8/eQTac/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-04-20 07:27:33.000000 eQTac-1.0.8/eQTac/control_FDR.py
--rw-rw-rw-   0        0        0     4277 2023-04-20 07:27:36.000000 eQTac-1.0.8/eQTac/eQTac_correlation.py
--rw-rw-rw-   0        0        0     2195 2023-04-20 07:27:39.000000 eQTac-1.0.8/eQTac/eQTac_permutation.py
--rw-rw-rw-   0        0        0     2697 2023-04-20 07:27:42.000000 eQTac-1.0.8/eQTac/filter_bkg.py
--rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_PRE.py
--rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_mut_fa.py
--rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.8/eQTac/generate_snp_dict.py
--rw-rw-rw-   0        0        0     3727 2023-04-20 07:27:44.000000 eQTac-1.0.8/eQTac/geno2score.py
--rw-rw-rw-   0        0        0     2476 2023-04-20 07:27:32.000000 eQTac-1.0.8/eQTac/get_nullseq.py
-drwxrwxrwx   0        0        0        0 2023-04-20 07:29:19.697697 eQTac-1.0.8/eQTac.egg-info/
--rw-rw-rw-   0        0        0     5925 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 07:29:19.000000 eQTac-1.0.8/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 07:29:19.721634 eQTac-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-04-20 07:28:25.000000 eQTac-1.0.8/setup.py
+drwxr-xr-x   0 jiangfeng  (1009) BIGC      (1001)        0 2023-07-28 03:17:31.573912 eQTac-1.0.9/
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     1511 2023-04-20 07:29:45.000000 eQTac-1.0.9/LICENSE
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)       17 2023-04-20 07:29:45.000000 eQTac-1.0.9/MANIFEST.in
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     6180 2023-07-28 03:17:31.573912 eQTac-1.0.9/PKG-INFO
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     5818 2023-07-28 02:59:35.000000 eQTac-1.0.9/README.md
+drwxr-xr-x   0 jiangfeng  (1009) BIGC      (1001)        0 2023-07-28 03:17:31.572911 eQTac-1.0.9/eQTac/
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)        0 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/__init__.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     1941 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/control_FDR.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     4277 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/eQTac_correlation.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     2195 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/eQTac_permutation.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     2697 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/filter_bkg.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     4744 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/generate_PRE.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     2594 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/generate_mut_fa.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)      910 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/generate_snp_dict.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     3727 2023-04-20 07:29:45.000000 eQTac-1.0.9/eQTac/geno2score.py
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     2501 2023-07-28 03:12:30.000000 eQTac-1.0.9/eQTac/get_nullseq.py
+drwxr-xr-x   0 jiangfeng  (1009) BIGC      (1001)        0 2023-07-28 03:17:31.573912 eQTac-1.0.9/eQTac.egg-info/
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)     6180 2023-07-28 03:17:31.000000 eQTac-1.0.9/eQTac.egg-info/PKG-INFO
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)      410 2023-07-28 03:17:31.000000 eQTac-1.0.9/eQTac.egg-info/SOURCES.txt
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)        1 2023-07-28 03:17:31.000000 eQTac-1.0.9/eQTac.egg-info/dependency_links.txt
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)       86 2023-07-28 03:17:31.000000 eQTac-1.0.9/eQTac.egg-info/requires.txt
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)        6 2023-07-28 03:17:31.000000 eQTac-1.0.9/eQTac.egg-info/top_level.txt
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)       38 2023-07-28 03:17:31.573912 eQTac-1.0.9/setup.cfg
+-rw-r--r--   0 jiangfeng  (1009) BIGC      (1001)      767 2023-07-28 03:05:38.000000 eQTac-1.0.9/setup.py
```

### Comparing `eQTac-1.0.8/LICENSE` & `eQTac-1.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, JFF
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+BSD 3-Clause License
+
+Copyright (c) 2023, JFF
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `eQTac-1.0.8/PKG-INFO` & `eQTac-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,138 @@
-Metadata-Version: 2.1
-Name: eQTac
-Version: 1.0.8
-Summary: The eQTac method.
-Home-page: https://github.com/JFF1594032292/eQTac
-Author: Jiang Feng
-Author-email: 1594032292@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# eQTac
-EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
-## Schematic 
-![](./imgs/Schematic.png)
-## Dependence
-### Python packages
-```
-numpy >= 1.21.6
-pandas >= 1.2.3
-pybedtools >= 0.8.1
-pysam >= 0.15.3
-rpy2 >= 3.5.11
-scipy >= 1.7.3
-```
-### Other software (need manual installation)
-```
-plink >= v1.90b6.24 (plink should in $PATH)
-bedtools >= v2.30.0 (bedtools should in $PATH)
-R >= 3.6.1
-    r-gkmSVM >= 0.8.0
-```
-## Installation & test example
-```
-# installation
-pip install eQTac 
-
-# test examples
-git clone https://github.com/JFF1594032292/eQTac.git # just for test
-cd eQTac/Utilities_pipeline
-nohup sh example_All_pipeline.sh &
-```
-Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
-
-## Input data
-1. Data used in model training:
-    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
-    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
-    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
-2. Data used in eQTac calculation.
-    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
-    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
-    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
-    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
-## Usage pattern
-We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
-### Pipeline-level pattern
-For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
-It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
-```
-python Part-All-eQTac_pipeline.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-exp test_data/test.exp_residual \
-	-n 100 \
-	-o output_eQTac \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-```
-### Part-level pattern
-For the function level pattern, we provide four scripts:
-```
-Part-1-Train_model.py
-Part-2-Generate_PRE_fa.py
-Part-3-Predict_PRE_score.py
-Part-4-Calculate_eQTac_correlation.py
-```
-It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
-```
-python Part-1-Train_model.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-o output_eQTac_part \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-
-python Part-2-Generate_PRE_fa.py \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-o output_eQTac_part
-
-python Part-3-Predict_PRE_score.py \
-	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
-	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
-	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
-	-geno test_data/test.geno \
-	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
-	-T 1 \
-	-o output_eQTac_part
-
-python Part-4-Calculate_eQTac_correlation.py \
-	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
-	-exp test_data/test.exp_residual \
-	-n 50 \
-	-o output_eQTac_part
-```
-### Function-level pattern
-For the function level pattern, we provide a series of functions:
-```
-from eQTac.get_nullseq import get_nullseq
-from eQTac.filter_bkg import filter_bkg
-from eQTac.generate_snp_dict import generate_snp_dict
-from eQTac.generate_PRE import generate_PRE
-from eQTac.generate_mut_fa import generate_mut_fa
-from eQTac.geno2score import geno2score
-from eQTac.eQTac_correlation import eQTac_correlation
-from eQTac.eQTac_permutation import eQTac_permutation
-from eQTac.control_FDR import control_FDR
-```
-These functions can be used to construct the whole pipeline.
-### Recomend
-We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
-
-Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
-
-If you are familiar with this pipeline, you can directly use the `function-level` pattern to construct your own pipeline.
-## Notes
-1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
+Metadata-Version: 2.1
+Name: eQTac
+Version: 1.0.9
+Summary: The eQTac method.
+Home-page: https://github.com/JFF1594032292/eQTac
+Author: Jiang Feng
+Author-email: 1594032292@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# eQTac
+EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, the only additional data was ATAC-seq or ChIP-seq peak data. 
+## Schematic 
+![](./imgs/Schematic.png)
+## Dependence
+### Python packages
+```
+numpy >= 1.21.6
+pandas >= 1.2.3
+pybedtools >= 0.8.1
+pysam >= 0.15.3
+rpy2 >= 3.5.11
+scipy >= 1.7.3
+```
+### Other software (need manual installation)
+```
+plink >= v1.90b6.24 (not plink2, plink should in $PATH)
+bedtools >= v2.30.0 (bedtools should in $PATH)
+R >= 3.6.1
+    r-gkmSVM >= 0.8.0
+```
+## Installation & test example
+```
+# installation
+pip install eQTac 
+
+# test examples
+git clone https://github.com/JFF1594032292/eQTac.git # just for test
+cd eQTac/Utilities_pipeline
+nohup sh example_All_pipeline.sh &
+```
+Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
+
+## Input data
+1. Data used in model training:
+    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
+<<<<<<< HEAD
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+=======
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from generated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+>>>>>>> 4b8bfa95564736c3bf45c48056ea656cf880d680
+    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
+2. Data used in eQTac calculation.
+    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
+    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
+    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
+    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
+## Usage pattern
+We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
+### Pipeline-level pattern
+For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
+It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
+```
+python Part-All-eQTac_pipeline.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-exp test_data/test.exp_residual \
+	-n 100 \
+	-o output_eQTac \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+```
+### Part-level pattern
+For the function level pattern, we provide four scripts:
+```
+Part-1-Train_model.py
+Part-2-Generate_PRE_fa.py
+Part-3-Predict_PRE_score.py
+Part-4-Calculate_eQTac_correlation.py
+```
+It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
+```
+python Part-1-Train_model.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-o output_eQTac_part \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+
+python Part-2-Generate_PRE_fa.py \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-o output_eQTac_part
+
+python Part-3-Predict_PRE_score.py \
+	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
+	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
+	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
+	-geno test_data/test.geno \
+	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
+	-T 1 \
+	-o output_eQTac_part
+
+python Part-4-Calculate_eQTac_correlation.py \
+	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
+	-exp test_data/test.exp_residual \
+	-n 50 \
+	-o output_eQTac_part
+```
+### Function-level pattern
+For the function level pattern, we provide a series of functions:
+```
+from eQTac.get_nullseq import get_nullseq
+from eQTac.filter_bkg import filter_bkg
+from eQTac.generate_snp_dict import generate_snp_dict
+from eQTac.generate_PRE import generate_PRE
+from eQTac.generate_mut_fa import generate_mut_fa
+from eQTac.geno2score import geno2score
+from eQTac.eQTac_correlation import eQTac_correlation
+from eQTac.eQTac_permutation import eQTac_permutation
+from eQTac.control_FDR import control_FDR
+```
+These functions can be used to construct the whole pipeline.
+### Recomend
+We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
+
+Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
+
+If you are familiar with this pipeline, you can directly use the **function-level** pattern to construct your own pipeline.
+## Notes
+1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
```

### Comparing `eQTac-1.0.8/README.md` & `eQTac-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # eQTac
-EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
+EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, the only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Schematic 
 ![](./imgs/Schematic.png)
 ## Dependence
 ### Python packages
 ```
 numpy >= 1.21.6
 pandas >= 1.2.3
 pybedtools >= 0.8.1
 pysam >= 0.15.3
 rpy2 >= 3.5.11
 scipy >= 1.7.3
 ```
 ### Other software (need manual installation)
 ```
-plink >= v1.90b6.24 (plink should in $PATH)
+plink >= v1.90b6.24 (not plink2, plink should in $PATH)
 bedtools >= v2.30.0 (bedtools should in $PATH)
 R >= 3.6.1
     r-gkmSVM >= 0.8.0
 ```
 ## Installation & test example
 ```
 # installation
@@ -30,15 +30,19 @@
 nohup sh example_All_pipeline.sh &
 ```
 Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
 
 ## Input data
 1. Data used in model training:
     1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
+<<<<<<< HEAD
     2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+=======
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from generated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+>>>>>>> 4b8bfa95564736c3bf45c48056ea656cf880d680
     3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
 2. Data used in eQTac calculation.
     1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
     2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
     3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
     4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
 ## Usage pattern
@@ -112,10 +116,10 @@
 ```
 These functions can be used to construct the whole pipeline.
 ### Recomend
 We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
 
 Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
 
-If you are familiar with this pipeline, you can directly use the `function-level` pattern to construct your own pipeline.
+If you are familiar with this pipeline, you can directly use the **function-level** pattern to construct your own pipeline.
 ## Notes
-1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
+1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
```

### Comparing `eQTac-1.0.8/eQTac/control_FDR.py` & `eQTac-1.0.9/eQTac/control_FDR.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/eQTac_correlation.py` & `eQTac-1.0.9/eQTac/eQTac_correlation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/eQTac_permutation.py` & `eQTac-1.0.9/eQTac/eQTac_permutation.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/filter_bkg.py` & `eQTac-1.0.9/eQTac/filter_bkg.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/generate_PRE.py` & `eQTac-1.0.9/eQTac/generate_PRE.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/generate_mut_fa.py` & `eQTac-1.0.9/eQTac/generate_mut_fa.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/generate_snp_dict.py` & `eQTac-1.0.9/eQTac/generate_snp_dict.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/geno2score.py` & `eQTac-1.0.9/eQTac/geno2score.py`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.8/eQTac/get_nullseq.py` & `eQTac-1.0.9/eQTac/get_nullseq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 # -*- coding: utf-8 -*-
 #########################################################################
 # File Name: get_nullseq.py
 # Created on : 2022-12-17 16:06:59
 # Author: JFF
-# Last Modified: 2022-12-17 16:07:01
+# Last Modified: 2023-07-28 10:24:14
 # Description:
 # Usage:
 # Input:
 # Output:
 #########################################################################
 import os
 import sys
 import re
 import rpy2.robjects as robjects
 from shutil import copyfile
 
-
-def get_nullseq(pos_bed_path, out_folder):
+def get_nullseq(pos_bed_path, out_folder, xfold):
     """
     Generates null sequences (negative set) with matching repeat and GC content as the input bed file for positive set regions.\n
     A wrapper of genNullSeqs from gkmSVM R package.
-    
+
     ## Parameters
     pos_bed_path
         positive training set bed file. e.g. ATAC peak bed file.
     out_folder
         output directory
-    
+
     ## Returns
     pos_fa
         positive sequence .fa file
     pos_bed_newpath
         positive sequence .bed file. (copy to output directory)
     negraw_fa
         raw negative sequence .fa file.
     negraw_bed
         raw negative sequence .bed file.
-    
+
+
     ## Notes
     The output ``negraw_fa`` and ``negraw_bed`` file not remove the duplicate sequences, and raw negative sequences may also contain potential positive sequences.(e.g. peaks with P<0.05 but q>0.05)\n
     The ``negraw_fa`` and ``negraw_bed`` showed filtered by ``filter_bkg`` function.
-    
+
     """
     pos_bed = os.path.basename(pos_bed_path)
     prefix = re.sub("\.bed$", "", pos_bed)
-    #make dir
+    # make dir
     if not os.path.exists(out_folder):
         os.mkdir(out_folder)
     # copy pos_bed to output folder & add a "pos" suffix
     pos_bed_newpath = out_folder + "/" + prefix + ".pos.bed"
     copyfile(pos_bed_path, pos_bed_newpath)
     # gkmSVM genNullSeqs
     pos_fa = out_folder + "/" + prefix + ".pos.fa"
     negraw_bed = out_folder + "/" + prefix + ".negraw.bed"
     negraw_fa = out_folder + "/" + prefix + ".negraw.fa"
-    d = dict(pos_bed_newpath=pos_bed_newpath, pos_fa=pos_fa, negraw_bed=negraw_bed, negraw_fa=negraw_fa)
+
+    d = dict(pos_bed_newpath=pos_bed_newpath, pos_fa=pos_fa, negraw_bed=negraw_bed, negraw_fa=negraw_fa, xfold=xfold)
     robjects.r(
-        "library(gkmSVM);genNullSeqs('%(pos_bed_newpath)s',nMaxTrials=20,xfold=2.5,GC_match_tol=0.05,repeat_match_tol=0.05,length_match_tol=0.05,batchsize=500000,genomeVersion='hg19', outputPosFastaFN='%(pos_fa)s', outputBedFN='%(negraw_bed)s', outputNegFastaFN='%(negraw_fa)s')"
+        "library(gkmSVM);genNullSeqs('%(pos_bed_newpath)s',nMaxTrials=20,xfold='%(xfold)f',GC_match_tol=0.05,repeat_match_tol=0.05,length_match_tol=0.05,batchsize=500000,genomeVersion='hg19', outputPosFastaFN='%(pos_fa)s', outputBedFN='%(negraw_bed)s', outputNegFastaFN='%(negraw_fa)s')"
         % d)
     return pos_fa, pos_bed_newpath, negraw_fa, negraw_bed
 
 
 if __name__ == '__main__':
-    get_nullseq("../Utilities_pipeline/test_data/test.positive.bed", ".")
+    get_nullseq("../Utilities_pipeline/test_data/test.positive.bed", ".", xfold=2.5)
```

### Comparing `eQTac-1.0.8/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.9/eQTac.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,138 @@
-Metadata-Version: 2.1
-Name: eQTac
-Version: 1.0.8
-Summary: The eQTac method.
-Home-page: https://github.com/JFF1594032292/eQTac
-Author: Jiang Feng
-Author-email: 1594032292@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# eQTac
-EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
-## Schematic 
-![](./imgs/Schematic.png)
-## Dependence
-### Python packages
-```
-numpy >= 1.21.6
-pandas >= 1.2.3
-pybedtools >= 0.8.1
-pysam >= 0.15.3
-rpy2 >= 3.5.11
-scipy >= 1.7.3
-```
-### Other software (need manual installation)
-```
-plink >= v1.90b6.24 (plink should in $PATH)
-bedtools >= v2.30.0 (bedtools should in $PATH)
-R >= 3.6.1
-    r-gkmSVM >= 0.8.0
-```
-## Installation & test example
-```
-# installation
-pip install eQTac 
-
-# test examples
-git clone https://github.com/JFF1594032292/eQTac.git # just for test
-cd eQTac/Utilities_pipeline
-nohup sh example_All_pipeline.sh &
-```
-Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
-
-## Input data
-1. Data used in model training:
-    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
-    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
-    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
-2. Data used in eQTac calculation.
-    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
-    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
-    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
-    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
-## Usage pattern
-We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
-### Pipeline-level pattern
-For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
-It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
-```
-python Part-All-eQTac_pipeline.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-exp test_data/test.exp_residual \
-	-n 100 \
-	-o output_eQTac \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-```
-### Part-level pattern
-For the function level pattern, we provide four scripts:
-```
-Part-1-Train_model.py
-Part-2-Generate_PRE_fa.py
-Part-3-Predict_PRE_score.py
-Part-4-Calculate_eQTac_correlation.py
-```
-It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
-```
-python Part-1-Train_model.py \
-	-p test_data/test.positive.bed \
-	-ex test_data/test.exclude.bed \
-	-o output_eQTac_part \
-	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
-
-python Part-2-Generate_PRE_fa.py \
-	-pre test_data/test.pre.bed \
-	--geno test_data/test.geno \
-	--snp test_data/test.geno.snplist \
-	-fa test_data/test.hg19.chr17.fa \
-	-o output_eQTac_part
-
-python Part-3-Predict_PRE_score.py \
-	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
-	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
-	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
-	-geno test_data/test.geno \
-	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
-	-T 1 \
-	-o output_eQTac_part
-
-python Part-4-Calculate_eQTac_correlation.py \
-	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
-	-exp test_data/test.exp_residual \
-	-n 50 \
-	-o output_eQTac_part
-```
-### Function-level pattern
-For the function level pattern, we provide a series of functions:
-```
-from eQTac.get_nullseq import get_nullseq
-from eQTac.filter_bkg import filter_bkg
-from eQTac.generate_snp_dict import generate_snp_dict
-from eQTac.generate_PRE import generate_PRE
-from eQTac.generate_mut_fa import generate_mut_fa
-from eQTac.geno2score import geno2score
-from eQTac.eQTac_correlation import eQTac_correlation
-from eQTac.eQTac_permutation import eQTac_permutation
-from eQTac.control_FDR import control_FDR
-```
-These functions can be used to construct the whole pipeline.
-### Recomend
-We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
-
-Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
-
-If you are familiar with this pipeline, you can directly use the `function-level` pattern to construct your own pipeline.
-## Notes
-1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
+Metadata-Version: 2.1
+Name: eQTac
+Version: 1.0.9
+Summary: The eQTac method.
+Home-page: https://github.com/JFF1594032292/eQTac
+Author: Jiang Feng
+Author-email: 1594032292@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# eQTac
+EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, the only additional data was ATAC-seq or ChIP-seq peak data. 
+## Schematic 
+![](./imgs/Schematic.png)
+## Dependence
+### Python packages
+```
+numpy >= 1.21.6
+pandas >= 1.2.3
+pybedtools >= 0.8.1
+pysam >= 0.15.3
+rpy2 >= 3.5.11
+scipy >= 1.7.3
+```
+### Other software (need manual installation)
+```
+plink >= v1.90b6.24 (not plink2, plink should in $PATH)
+bedtools >= v2.30.0 (bedtools should in $PATH)
+R >= 3.6.1
+    r-gkmSVM >= 0.8.0
+```
+## Installation & test example
+```
+# installation
+pip install eQTac 
+
+# test examples
+git clone https://github.com/JFF1594032292/eQTac.git # just for test
+cd eQTac/Utilities_pipeline
+nohup sh example_All_pipeline.sh &
+```
+Then it will generate an `output_eQTac` folder, which contained results file `test.geno.vcf.gz.PRE_score.eQTac_result.FDR.txt`. (example takes 3~5min)
+
+## Input data
+1. Data used in model training:
+    1. **Positive sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, we recomended to trim peaks to the core region (e.g. summits $\pm$ 100bp). See `test_data/test.positive.bed`.
+<<<<<<< HEAD
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from genrated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+=======
+    2. **Excluded sets in bed format.** It's usually the peak data from ATAC-seq or ChIP-seq, but with more relaxed thresholds (e.g. p=0.2). These region will be removed from generated negative regions, in order to remove potential positive sequences from negative sets. See `test_data/test`.exclude.bed.
+>>>>>>> 4b8bfa95564736c3bf45c48056ea656cf880d680
+    3. Fasta file with .fai index. Usually the human genome sequnce file in fasta format. See `test_data/test.hg19.chr17.fa`.
+2. Data used in eQTac calculation.
+    1. **PRE.bed**. The candidate regions used to assess chromatin accessibility scores across different individuals and then calculate correlation with target genes. See `test_data/test.pre.bed`.
+    2. **Genotype data in plink format**. Individual genotype in eQTL datasets. See `test_data/test.geno.bed, test_data/test.geno.bim, test_data/test.geno.fam`.
+    3. **Expression file**. The expresion values are normalized expression values (see GTEx) and already corrected for covariates. See `test_data/test.exp_residual`.
+    4. Snplist file. SNP list file used in eQTac analysis. Note: only single nucleotide mutations. See `test_data/test.geno.snplist`.
+## Usage pattern
+We provided three level patterns: (1) pipeline level. (2) part level. (3) function level.
+### Pipeline-level pattern
+For the function level pattern, we provide a script: Part-All-eQTac_pipeline.py.
+It can be used as `Utilities_pipeline/example_All_pipeline.sh`:
+```
+python Part-All-eQTac_pipeline.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-exp test_data/test.exp_residual \
+	-n 100 \
+	-o output_eQTac \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+```
+### Part-level pattern
+For the function level pattern, we provide four scripts:
+```
+Part-1-Train_model.py
+Part-2-Generate_PRE_fa.py
+Part-3-Predict_PRE_score.py
+Part-4-Calculate_eQTac_correlation.py
+```
+It can be used as `Utilities_pipeline/example_Part_pipeline.sh`:
+```
+python Part-1-Train_model.py \
+	-p test_data/test.positive.bed \
+	-ex test_data/test.exclude.bed \
+	-o output_eQTac_part \
+	-t 3 -l 10 -k 6 -c 10 -g 2 -e 0.01
+
+python Part-2-Generate_PRE_fa.py \
+	-pre test_data/test.pre.bed \
+	--geno test_data/test.geno \
+	--snp test_data/test.geno.snplist \
+	-fa test_data/test.hg19.chr17.fa \
+	-o output_eQTac_part
+
+python Part-3-Predict_PRE_score.py \
+	-m output_eQTac_part/test.positive.pos.svmmodel.3_10_6_0.01.model.txt \
+	-l output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info \
+	-mfa output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist.ld_info.snplist.bed.mutate.fa \
+	-geno test_data/test.geno \
+	-snp output_eQTac_part/test.geno.snplist.bed--test.pre.bed.pre_snplist \
+	-T 1 \
+	-o output_eQTac_part
+
+python Part-4-Calculate_eQTac_correlation.py \
+	-pre output_eQTac_part/test.geno.vcf.gz.PRE_score \
+	-exp test_data/test.exp_residual \
+	-n 50 \
+	-o output_eQTac_part
+```
+### Function-level pattern
+For the function level pattern, we provide a series of functions:
+```
+from eQTac.get_nullseq import get_nullseq
+from eQTac.filter_bkg import filter_bkg
+from eQTac.generate_snp_dict import generate_snp_dict
+from eQTac.generate_PRE import generate_PRE
+from eQTac.generate_mut_fa import generate_mut_fa
+from eQTac.geno2score import geno2score
+from eQTac.eQTac_correlation import eQTac_correlation
+from eQTac.eQTac_permutation import eQTac_permutation
+from eQTac.control_FDR import control_FDR
+```
+These functions can be used to construct the whole pipeline.
+### Recomend
+We recomend to use the **pipeline-level** pattern at first to make sure that all input formats are valid. 
+
+Then use the **part-level** pattern to debug parameters. (e.g. training a best performance model). The first step is the most time-consuming step, we recomended to use the part-level pattern to save the SVM model `xxx.svmmodel.3_10_6_0.01.model.txt`.
+
+If you are familiar with this pipeline, you can directly use the **function-level** pattern to construct your own pipeline.
+## Notes
+1. The test result is very volatile, because of the small size of test dataset (only ~6MB length of sequences). The results will be stable with tens of thousands or more peaks used as positive set.
```

### Comparing `eQTac-1.0.8/setup.py` & `eQTac-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.8",
+    version="1.0.9",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
@@ -21,8 +21,8 @@
     install_requires=[
         'numpy >= 1.21.6',
         'pandas >= 1.2.3',
         'pybedtools >= 0.8.1',
         'pysam >= 0.15.3',
         'rpy2 >= 3.5.11',
         'scipy >= 1.7.3'],
-)
+)
```

