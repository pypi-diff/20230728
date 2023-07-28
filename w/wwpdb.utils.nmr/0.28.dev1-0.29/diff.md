# Comparing `tmp/wwpdb.utils.nmr-0.28.dev1.tar.gz` & `tmp/wwpdb.utils.nmr-0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.nmr-0.28.dev1.tar", last modified: Thu Jul  6 12:26:17 2023, max compression
+gzip compressed data, was "wwpdb.utils.nmr-0.29.tar", last modified: Fri Jul 28 10:26:54 2023, max compression
```

## Comparing `wwpdb.utils.nmr-0.28.dev1.tar` & `wwpdb.utils.nmr-0.29.tar`

### file list

```diff
@@ -1,115 +1,120 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.303945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)   103812 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/
--rw-r--r--   0 vsts      (1001) docker     (123)   517809 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/
--rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
--rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2763977 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py
--rw-r--r--   0 vsts      (1001) docker     (123)   130980 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
--rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.307945 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/
--rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   234229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    79373 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8451 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   212951 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   167192 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    71357 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   119610 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py
--rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.327947 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/
--rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-06 12:22:04.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-06 12:26:17.299945 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      709 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-06 12:23:12.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-06 12:26:17.000000 wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.071541 wwpdb.utils.nmr-0.29/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      248 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-07-28 10:26:54.071541 wwpdb.utils.nmr-0.29/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       36 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-28 10:26:54.071541 wwpdb.utils.nmr-0.29/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2814 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.035541 wwpdb.utils.nmr-0.29/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.039541 wwpdb.utils.nmr-0.29/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.043541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)   103825 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/AlignUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    72301 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/BMRBChemShiftStat.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12129 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/ChemCompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26972 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/CifToNmrStar.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.043541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/
+-rw-r--r--   0 vsts      (1001) docker     (123)   518384 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4051 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.043541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/
+-rw-r--r--   0 vsts      (1001) docker     (123)    27217 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     9863 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    10176 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)   103535 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrDpReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2774431 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23027 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrStarToCif.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   133550 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrVrptUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.047541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10676 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25729 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    10656 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)    25737 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3458 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3495 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8742 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   170036 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/others.csv
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3573 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8327 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3591 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv
+-rw-r--r--   0 vsts      (1001) docker     (123)     8409 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.047541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13142 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66593 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/CifReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10198 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.063541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    79462 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   234229 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   493179 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20363 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    42777 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   178190 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    79705 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8655 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11409 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    41669 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   135928 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9563 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84136 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   212951 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   295091 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9003 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   151068 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   417159 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   469882 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13554 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32899 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   167192 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   454966 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18196 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50972 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   219341 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   236108 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9611 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15500 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43150 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    92902 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10402 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27535 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   159229 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    71689 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8276 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10640 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7446 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    83785 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8792 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3593 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/LexerErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4792 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/ParserErrorListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   406211 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/ParserListenerUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33530 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   119610 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   215435 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10471 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11350 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10246 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    84828 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9089 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   165077 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   679237 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   684343 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRParserListener.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21181 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.071541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/nmr-star_schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11128 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/nmr-star_schema/category_order.pkl
+-rw-r--r--   0 vsts      (1001) docker     (123)     1814 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/nmr-star_schema/data_types.pkl
+-rw-r--r--   0 vsts      (1001) docker     (123)  5228287 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/nmr-star_schema/schema.pkl
+-rw-r--r--   0 vsts      (1001) docker     (123)   246423 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/nmr-star_schema/schema_order.pkl
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.071541 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/rci/
+-rw-r--r--   0 vsts      (1001) docker     (123)   361662 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/rci/RCI.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-28 10:23:01.000000 wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/rci/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 10:26:54.039541 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      704 2023-07-28 10:26:53.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3964 2023-07-28 10:26:54.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 10:26:53.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 10:24:15.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      330 2023-07-28 10:26:53.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-28 10:26:53.000000 wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/LICENSE` & `wwpdb.utils.nmr-0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/PKG-INFO` & `wwpdb.utils.nmr-0.29/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.28.dev1
+Version: 0.29
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/setup.py` & `wwpdb.utils.nmr-0.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                       "pynmrstar; python_version >= '3'",
                       "munkres==1.0.12; python_version == '2.7'",
                       "munkres; python_version >= '3'",
                       'mmcif', 'numpy', "scikit-learn",
                       "rmsd", "packaging", "chardet",
                       "typing_extensions",  # typing_extensions was missing from rmsd 1.5 package
                       "antlr4-python2-runtime; python_version == '2.7'",
-                      "antlr4-python3-runtime ~= 4.12.0; python_version >= '3'"],
+                      "antlr4-python3-runtime ~= 4.13.0; python_version >= '3'"],
     packages=find_packages(exclude=['wwpdb.utils.tests-nmr', 'wwpdb.utils.tests-nmr-tox', 'mock-data']),
     # Enables Manifest to be used
     include_package_data=True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         '': ['*.md', '*.rst', "*.txt", "*.cfg"],
     },
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/AlignUtil.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/AlignUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1054,15 +1054,15 @@
             length = len(myAlign)
 
             if length == 0:
                 continue
 
             _matched, unmapped, conflict, offset_1, offset_2 = getScoreOfSeqAlign(myAlign)
 
-            if length == unmapped + conflict or _matched <= conflict:
+            if length == unmapped + conflict or _matched <= conflict - conflictTh:
                 continue
 
             if not_decided_s2_comp_id:  # AMBER/GROMACS topology
                 idx2 = 0
                 for i in range(length):
                     myPr = myAlign[i]
                     myPr0 = str(myPr[0])
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/BMRBChemShiftStat.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/BMRBChemShiftStat.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/ChemCompUtil.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/ChemCompUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/CifToNmrStar.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/CifToNmrStar.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/NEFTranslator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,15 +1327,15 @@
                 sorted_seq = sorted(set((row[2], int(row[0]) + offset_seq_ids[row[2]], row[1].upper()) for row in seq_data),
                                     key=itemgetter(0, 1))
 
                 chk_dict = {(row[2], int(row[0])): row[1].upper() for row in seq_data}
 
                 for row in seq_data:
                     chk_key = (row[2], int(row[0]))
-                    if chk_dict[chk_key] != row[1]:
+                    if chk_dict[chk_key] != row[1].upper():
                         raise KeyError(f"{lp_category[1:]} loop contains different {comp_id} ({row[1]} and {chk_dict[chk_key]}) "
                                        f"with the same {chain_id} {row[2]}, {seq_id} {row[0]}.")
 
                 if len(sorted_seq[0][2]) > 1:
                     if len(chain_ids) > 1:
                         for c in chain_ids:
                             cmp_dict[c] = [x[2] for x in sorted_seq if x[0] == c]
@@ -1548,15 +1548,15 @@
                 sorted_seq = sorted(set((row[2], int(row[0]) + offset_seq_ids[row[2]], row[1].upper()) for row in seq_data),
                                     key=itemgetter(0, 1))
 
                 chk_dict = {(row[2], int(row[0])): row[1].upper() for row in seq_data}
 
                 for row in seq_data:
                     chk_key = (row[2], int(row[0]))
-                    if chk_dict[chk_key] != row[1]:
+                    if chk_dict[chk_key] != row[1].upper():
 
                         if seq_id != alt_seq_id and alt_seq_id in loop.tags:
 
                             seq_tags = [seq_id, alt_seq_id]
                             _seq_data = get_lp_tag(loop, seq_tags)
 
                             offset = None
@@ -4567,15 +4567,15 @@
 
             if atom_id[0] in ('1', '2', '3'):
                 atom_list, ambiguity_code, details = self.get_valid_star_atom(comp_id, atom_id, details, leave_unmatched, methyl_only)
                 if details is None:
                     return (atom_list, ambiguity_code, details)
                 atom_id = atom_id[1:] + atom_id[0]
 
-            if atom_id[0] in ('H', 'Q', 'M'):
+            if atom_id[0] in ('H', 'Q', 'M') and (self.__remediation_mode or atom_id[0] == 'H'):  # DAOTHER-8663
 
                 if atom_id.endswith('1') and not self.validate_comp_atom(comp_id, atom_id):
                     _atom_id = atom_id[:-1] + '3'
                     if self.validate_comp_atom(comp_id, _atom_id):
                         atom_list, ambiguity_code, details = self.get_valid_star_atom(comp_id, _atom_id, details, leave_unmatched, methyl_only)
                         return (atom_list, ambiguity_code, details)
 
@@ -4635,35 +4635,37 @@
             if '#' in atom_id:
                 atom_id = atom_id.replace('#', '%')
 
             if atom_id == 'HN' or atom_id.endswith('%') or atom_id.endswith('*'):
                 atom_list, ambiguity_code, details = self.get_star_atom(comp_id, atom_id, details, leave_unmatched, methyl_only)
                 return (atom_list, ambiguity_code, details)
 
-            if atom_id.startswith('QQ'):
-                atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[2:] + '%', details, leave_unmatched, methyl_only)
-                return (atom_list, ambiguity_code, details)
+            if atom_id[0] in ('Q', 'M') and self.__remediation_mode:  # DAOTHER-8663
 
-            if atom_id.startswith('QR') or atom_id.startswith('QX'):
-                qr_atoms = sorted(set(atom_id[:-1] + '%' for atom_id in self.__csStat.getAromaticAtoms(comp_id)
-                                      if atom_id[0] in protonBeginCode and self.__csStat.getMaxAmbigCodeWoSetId(comp_id, atom_id) == 3))
-                if len(qr_atoms) == 0:
+                if atom_id.startswith('QQ'):
+                    atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[2:] + '%', details, leave_unmatched, methyl_only)
                     return (atom_list, ambiguity_code, details)
-                atom_list = []
-                for qr_atom in qr_atoms:
-                    _atom_list, ambiguity_code, details = self.get_star_atom(comp_id, qr_atom, details, leave_unmatched, methyl_only)
-                    atom_list.extend(_atom_list)
-                return (atom_list, ambiguity_code, details)
 
-            if atom_id.startswith('Q') or atom_id.startswith('M'):
-                if atom_id[-1].isalnum():
-                    atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[1:] + '%', details, leave_unmatched, methyl_only)
+                if atom_id.startswith('QR') or atom_id.startswith('QX'):
+                    qr_atoms = sorted(set(atom_id[:-1] + '%' for atom_id in self.__csStat.getAromaticAtoms(comp_id)
+                                          if atom_id[0] in protonBeginCode and self.__csStat.getMaxAmbigCodeWoSetId(comp_id, atom_id) == 3))
+                    if len(qr_atoms) == 0:
+                        return (atom_list, ambiguity_code, details)
+                    atom_list = []
+                    for qr_atom in qr_atoms:
+                        _atom_list, ambiguity_code, details = self.get_star_atom(comp_id, qr_atom, details, leave_unmatched, methyl_only)
+                        atom_list.extend(_atom_list)
+                    return (atom_list, ambiguity_code, details)
+
+                if atom_id.startswith('Q') or atom_id.startswith('M'):
+                    if atom_id[-1].isalnum():
+                        atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[1:] + '%', details, leave_unmatched, methyl_only)
+                        return (atom_list, ambiguity_code, details)
+                    atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[1:-1] + '*', details, leave_unmatched, methyl_only)
                     return (atom_list, ambiguity_code, details)
-                atom_list, ambiguity_code, details = self.get_star_atom(comp_id, 'H' + atom_id[1:-1] + '*', details, leave_unmatched, methyl_only)
-                return (atom_list, ambiguity_code, details)
 
             if len(atom_id) > 2 and ((atom_id + '2' in self.__csStat.getAllAtoms(comp_id)) or (atom_id + '22' in self.__csStat.getAllAtoms(comp_id))):
                 atom_list, ambiguity_code, details = self.get_star_atom(comp_id, atom_id + '%', details, leave_unmatched, methyl_only)
                 return (atom_list, ambiguity_code, details)
 
             atom_list, ambiguity_code, details = self.get_star_atom(comp_id, atom_id, details, leave_unmatched, methyl_only)
 
@@ -4926,28 +4928,28 @@
 
                     if atom_id not in atoms:
 
                         _atom_id = None
 
                         if atom_id == 'HN' and self.__csStat.peptideLike(comp_id):
                             _atom_id = 'H'
-                        elif atom_id.startswith('QQ'):
+                        elif atom_id.startswith('QQ') and self.__remediation_mode:  # DAOTHER-8663
                             _atom_id = 'H' + atom_id[2:] + '%'
-                        elif atom_id.startswith('QR') or atom_id.startswith('QX'):
+                        elif (atom_id.startswith('QR') or atom_id.startswith('QX')) and self.__remediation_mode:  # DAOTHER-8663
                             qr_atoms = sorted(set(atom_id[:-1] + '%' for atom_id in self.__csStat.getAromaticAtoms(comp_id)
                                                   if atom_id[0] in protonBeginCode and self.__csStat.getMaxAmbigCodeWoSetId(comp_id, atom_id) == 3))
                             if len(qr_atoms) > 0:
                                 for qr_atom in qr_atoms:
                                     _a = copy.copy(a)
                                     _a['atom_id'] = qr_atom
                                     star_atom_list.append(_a)
                                 star_atom_list.remove(a)
                                 atom_list, details, atom_id_map = self.get_nef_atom(comp_id, star_atom_list, details, leave_unmatched)
                                 return (atom_list, details, atom_id_map)
-                        elif atom_id.startswith('Q') or atom_id.startswith('M'):
+                        elif (atom_id.startswith('Q') or atom_id.startswith('M')) and self.__remediation_mode:  # DAOTHER-8663
                             if atom_id[-1].isalnum():
                                 _atom_id = 'H' + atom_id[1:] + '%'
                             else:
                                 _atom_id = 'H' + atom_id[1:-1] + '*'
                         elif atom_id + '2' in self.__csStat.getAllAtoms(comp_id):
                             _atom_id = atom_id + '%'
 
@@ -6905,15 +6907,15 @@
                                     nef_chain = _star_chain
                                 else:
                                     cid = self.authChainId.index(_star_chain)
                                     nef_chain = indexToLetter(cid)
                             tag_map[chain_tag] = nef_chain
                             tag_map[seq_tag] = _star_seq
 
-                        if star_chain in self.star2CifChainMapping:
+                        if self.star2CifChainMapping is not None and star_chain in self.star2CifChainMapping:
                             tag_map[chain_tag] = self.star2CifChainMapping[star_chain]
 
                         if chain_tag == chain_tag_1:
                             seq_key_1 = seq_key
                         else:
                             seq_key_2 = seq_key
 
@@ -8226,15 +8228,15 @@
                                     nef_chain = _star_chain
                                 else:
                                     cid = self.authChainId.index(_star_chain)
                                     nef_chain = indexToLetter(cid)
                             tag_map[chain_tag] = nef_chain
                             tag_map[seq_tag] = _star_seq
 
-                        if star_chain in self.star2CifChainMapping:
+                        if self.star2CifChainMapping is not None and star_chain in self.star2CifChainMapping:
                             tag_map[chain_tag] = self.star2CifChainMapping[star_chain]
 
                         s.append(seq_key)
 
                     buf = [None] * len(nef_tags)
 
                     for tag in star_tags:
@@ -8624,27 +8626,27 @@
 
             _star_seq = in_row[star_tags.index(seq_tag)]
             if isinstance(_star_seq, str) and _star_seq not in emptyValue:
                 _star_seq = int(_star_seq)
 
             try:
                 tag_map[chain_tag], tag_map[seq_tag] = self.authSeqMap[(_star_chain, _star_seq)]
-            except KeyError:
+            except (KeyError, TypeError):
                 try:
                     nef_chain = self.selfSeqMap[(_star_chain, 1)][0]
-                except KeyError:
+                except (KeyError, TypeError):
                     if _star_chain in emptyValue or _star_chain not in self.authChainId:
                         nef_chain = _star_chain
                     else:
                         cid = self.authChainId.index(_star_chain)
                         nef_chain = indexToLetter(cid)
                 tag_map[chain_tag] = nef_chain
                 tag_map[seq_tag] = _star_seq
 
-            if star_chain in self.star2CifChainMapping:
+            if self.star2CifChainMapping is not None and star_chain in self.star2CifChainMapping:
                 tag_map[chain_tag] = self.star2CifChainMapping[star_chain]
 
         out = [None] * len(nef_tags)
 
         for tag in star_tags:
 
             nef_tag, _ = self.get_nef_tag(tag)
@@ -8883,15 +8885,15 @@
                                 if _star_chain in emptyValue or _star_chain not in self.authChainId:
                                     nef_chain = _star_chain
                                 else:
                                     cid = self.authChainId.index(_star_chain)
                                     nef_chain = indexToLetter(cid)
                             nef_seq = _star_seq
 
-                        if _star_chain in self.star2CifChainMapping:
+                        if self.star2CifChainMapping is not None and _star_chain in self.star2CifChainMapping:
                             nef_chain = self.star2CifChainMapping[_star_chain]
 
                         out[col] = nef_chain
                         out[col + 1] = nef_seq
 
                         comp_id = pk_assign[pk_assign_comp_id_col]
                         atom_id = pk_assign[pk_assign_atom_id_col]
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/README.md` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NEF_NMRSTAR_equivalence.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NEF_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NEFTranslator/lib/NMR-STAR_mandatory.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpReport.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrDpReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrDpUtility.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrDpUtility.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,16 @@
 # 24-Oct-2022  M. Yokochi - add support for floating chiral stereo assignments (NMR restraint remediation)
 # 15-Dec-2022  M. Yokochi - merge CS and MR as a single NMR data file in CIF format with comprehensive molecular assembly information (DAOTHER-7407, NMR restraint remediation)
 # 13-Jan-2023  M. Yokochi - add support for small angle X-ray scattering restraints (NMR restraint remediation)
 # 24-Jan-2023  M. Yokochi - add support for heteronuclear relaxation data (NOE, T1, T2, T1rho, Order parameter) (NMR restraint remediation)
 # 23-Feb-2023  M. Yokochi - combine spectral peak lists in any format into single NMR-STAR until Phase 2 release (DAOTHER-7407)
 # 24-Mar-2023  M. Yokochi - add 'nmr-nef2cif-deposit' and 'nmr-str2cif-deposit' workflow operations (DAOTHER-7407)
 # 22-Jun-2023  M. Yokochi - convert model file when pdbx_poly_seq category is missing for reuploading nmr_data after unlock (DAOTHER-8580)
+# 19-Jul-2023  M. Yokochi - fix not to merge restraint id (_Gen_dist_constraint.ID) if lower and upper bounds are different (DAOTHER-8705)
+# 20-Jul-2023  M. Yokochi - throw 'format_issue' error when polymer sequence extraction fails (DAOTHER-8644)
 ##
 """ Wrapper class for NMR data processing.
     @author: Masashi Yokochi
 """
 import sys
 import os
 import itertools
@@ -1074,14 +1076,16 @@
         self.__update_poly_seq = False
         # whether to resolve conflict
         self.__resolve_conflict = False
         # whether to detect missing mandatory tags as errors
         self.__check_mandatory_tag = False
         # whether to detect consistency of author sequence (nmr-star specific)
         self.__check_auth_seq = False
+        # whether to skip missing_mandatory_content error for validation server (DAOTHER-8658)
+        self.__validation_server = False
         # whether to translate conventional pseudo atom nomenclature in combined NMR-STAR file
         self.__transl_pseudo_name = False
         # whether to enable tolerant sequence alignment for residue variants
         self.__tolerant_seq_align = False
 
         # whether to fix format issue (enabled if NMR conventional deposition or release mode)
         self.__fix_format_issue = False
@@ -6399,14 +6403,20 @@
 
         if has_key_value(self.__inputParamDict, 'check_auth_seq'):
             if isinstance(self.__inputParamDict['check_auth_seq'], bool):
                 self.__check_auth_seq = self.__inputParamDict['check_auth_seq']
             else:
                 self.__check_auth_seq = self.__inputParamDict['check_auth_seq'] in trueValue
 
+        if has_key_value(self.__inputParamDict, 'validation_server'):
+            if isinstance(self.__inputParamDict['validation_server'], bool):
+                self.__validation_server = self.__inputParamDict['validation_server']
+            else:
+                self.__validation_server = self.__inputParamDict['validation_server'] in trueValue
+
         if has_key_value(self.__inputParamDict, 'transl_pseudo_name'):
             if isinstance(self.__inputParamDict['transl_pseudo_name'], bool):
                 self.__transl_pseudo_name = self.__inputParamDict['transl_pseudo_name']
             else:
                 self.__transl_pseudo_name = self.__inputParamDict['transl_pseudo_name'] in trueValue
         elif op in ('nmr-str-consistency-check', 'nmr-str2str-deposit', 'nmr-str2cif-deposit', 'nmr-str2nef-release'):
             self.__transl_pseudo_name = True
@@ -9102,14 +9112,15 @@
            and '_Constraint_file' in self.__lp_category_list:
             _sf = self.__star_data[file_list_id].get_saveframes_by_category('constraint_statistics')[0]
             data_file_name = get_first_sf_tag(_sf, 'Data_file_name')
             if mr_file_name_pattern.match(data_file_name) or proc_mr_file_name_pattern.match(data_file_name):
                 entry_id = get_first_sf_tag(_sf, 'Entry_ID')
                 if pdb_id_pattern.match(entry_id) or dep_id_pattern.match(entry_id):
                     self.__remediation_mode = True
+                    self.__nefT.set_remediation_mode(True)
 
         is_valid, messages, corrections = self.__nefT.resolve_sf_names_for_cif(self.__star_data[file_list_id])  # DAOTHER-7389, issue #4
         self.__sf_name_corr.append(corrections)
 
         if not is_valid:
 
             for warn in messages:
@@ -9434,15 +9445,15 @@
                 self.report.warning.appendDescription('missing_content',
                                                       {'file_name': file_name, 'description': warn})
                 self.report.setWarning()
 
                 if self.__verbose:
                     self.__lfh.write(f"+NmrDpUtility.__detectContentSubType() ++ Warning  - {warn}\n")
 
-            else:
+            elif not self.__validation_server:
 
                 err = f"The saveframe with a category {sf_category!r} is missing, "\
                     f"Deposition of distance restraints is mandatory. Please re-upload the {file_type.upper()} file."
 
                 self.report.error.appendDescription('missing_mandatory_content',
                                                     {'file_name': file_name, 'description': err})
                 self.report.setError()
@@ -9503,15 +9514,15 @@
 
             mr_loops = 0
 
             for content_subtype in self.mr_content_subtypes:
                 if content_subtype in lp_counts:
                     mr_loops += lp_counts[content_subtype]
 
-            if mr_loops == 0:
+            if mr_loops == 0 and not self.__validation_server:
 
                 if 'other_data_types' not in self.__sf_category_list:
 
                     err = "Deposition of NMR restraints used for the structure determination is mandatory. "\
                         f"Please re-upload the {file_type.upper()} file."
 
                     self.report.error.appendDescription('missing_mandatory_content',
@@ -15095,24 +15106,26 @@
                 if 'spectral_peak' in content_subtype or 'spectral_peak_alt' in content_subtype:
                     has_spectral_peak = True
 
             if not has_restraint:
 
                 if mr_file_name == '.':
 
-                    dir_path = os.path.dirname(self.__dstPath)
+                    if self.__dstPath is not None:
 
-                    rem_dir = os.path.join(dir_path, 'remediation')
+                        dir_path = os.path.dirname(self.__dstPath)
 
-                    if os.path.isdir(rem_dir):
+                        rem_dir = os.path.join(dir_path, 'remediation')
 
-                        try:
-                            os.rmdir(rem_dir)
-                        except OSError:
-                            pass
+                        if os.path.isdir(rem_dir):
+
+                            try:
+                                os.rmdir(rem_dir)
+                            except OSError:
+                                pass
 
                 else:
 
                     touch_file = os.path.join(dir_path, '.entry_without_mr')
                     if not os.path.exists(touch_file):
                         with open(touch_file, 'w') as ofh:
                             ofh.write('')
@@ -15455,15 +15468,15 @@
                             continue
 
                         if err.startswith('[Invalid data]'):
 
                             p = err.index(']') + 2
                             err = err[p:]
 
-                            self.report.error.appendDescription('invalid_data',
+                            self.report.error.appendDescription('format_issue',
                                                                 {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                  'description': err})
                             self.report.setError()
 
                             if self.__verbose:
                                 self.__lfh.write(f"+NmrDpUtility.__extractPolymerSequence() ++ ValueError  - {err}\n")
 
@@ -15725,20 +15738,22 @@
             for err in errs:
 
                 if len(err) == 0:
                     continue
 
                 if err.startswith('[Invalid data]'):
 
-                    if 'Auth' not in err or self.__check_auth_seq:
+                    _err = err.split('#')[0]
+
+                    if 'Auth' not in _err or self.__check_auth_seq:
 
                         p = err.index(']') + 2
                         err = err[p:]
 
-                        self.report.error.appendDescription('invalid_data',
+                        self.report.error.appendDescription('format_issue',
                                                             {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                              'description': err})
                         self.report.setError()
 
                         if self.__verbose:
                             self.__lfh.write(f"+NmrDpUtility.__extractPolymerSequenceInLoop() ++ ValueError  - {err}\n")
 
@@ -18254,14 +18269,17 @@
                             _atom_id = self.__nefT.get_star_atom(comp_id, atom_id, leave_unmatched=False)[0]
 
                             if len(_atom_id) == 0:
 
                                 if self.__nonblk_bad_nterm and atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                     continue
 
+                                if self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                    continue
+
                                 err = f"Invalid atom_id {atom_id!r} (comp_id {comp_id}) in a loop {lp_category}."
 
                                 self.report.error.appendDescription('invalid_atom_nomenclature',
                                                                     {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                      'description': err})
                                 self.report.setError()
 
@@ -18271,14 +18289,17 @@
                             else:
                                 _atom_ids.extend(_atom_id)
 
                         atom_ids = sorted(set(_atom_ids))
 
                     for atom_id in atom_ids:
 
+                        if self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                            continue
+
                         if atom_id == 'HN' and self.__csStat.peptideLike(comp_id):
                             self.__fixAtomNomenclature(comp_id, {'HN': 'H'})
                             continue
 
                         atom_id_ = atom_id
 
                         if (file_type == 'nef' or not self.__combined_mode or self.__transl_pseudo_name) and self.__isNmrAtomName(comp_id, atom_id):
@@ -18323,14 +18344,17 @@
                                 # @see: https://bmrb.io/ref_info/atom_nom.tbl
                                 # self.__fixAtomNomenclature(comp_id, {_atom_id_1: _atom_id_2, _atom_id_2: _atom_id_3})
                                 self.__fixAtomNomenclature(comp_id, {_atom_id_1: _atom_id_3})
 
                             elif self.__nonblk_bad_nterm and atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                 pass
 
+                            elif self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                pass
+
                             else:
 
                                 err = f"Invalid atom_id {atom_id!r} (comp_id {comp_id}) in a loop {lp_category}."
 
                                 self.report.error.appendDescription('invalid_atom_nomenclature',
                                                                     {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                      'description': err})
@@ -18351,14 +18375,18 @@
 
                             if file_type == 'nef':
                                 _atom_id = self.__nefT.get_star_atom(comp_id, atom_id, leave_unmatched=False)[0]
                                 if len(_atom_id) > 0:
                                     atom_id = _atom_id[0]
 
                             if atom_id not in ref_atom_ids:
+
+                                if self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                    continue
+
                                 unk_atom_ids.append(atom_id)
 
                         if len(unk_atom_ids) > 0:
                             cc_rel_status = self.__ccU.lastChemCompDict['_chem_comp.pdbx_release_status']
                             if cc_rel_status == 'REL':
                                 cc_name = self.__ccU.lastChemCompDict['_chem_comp.name']
                             else:
@@ -18379,14 +18407,17 @@
                         for elem in ref_elems:
                             if elem in PARAMAGNETIC_ELEMENTS or elem in FERROMAGNETIC_ELEMENTS:
                                 self.report.setDiamagnetic(False)
                                 break
 
                         for atom_id in atom_ids:
 
+                            if self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                continue
+
                             if atom_id == 'HN' and self.__csStat.peptideLike(comp_id):
                                 self.__fixAtomNomenclature(comp_id, {'HN': 'H'})
                                 continue
 
                             atom_id_ = atom_id
 
                             if (file_type == 'nef' or not self.__combined_mode or self.__transl_pseudo_name) and self.__isNmrAtomName(comp_id, atom_id):
@@ -18443,14 +18474,17 @@
                                     _auth_atom_ids.extend(auth_atom_ids)
 
                                 else:
 
                                     if self.__nonblk_bad_nterm and _auth_atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                         continue
 
+                                    if self.__remediation_mode and _auth_atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                        continue
+
                                     auth_atom_ids = self.__getAtomIdListInXplor(comp_id, _auth_atom_id)
 
                                     if len(auth_atom_ids) > 0:
                                         _auth_atom_ids.extend(auth_atom_ids)
 
                                     else:
 
@@ -18470,14 +18504,17 @@
 
                                 if not self.__nefT.validate_comp_atom(comp_id,
                                                                       translateToStdAtomName(auth_atom_id, comp_id, ref_atom_ids)):
 
                                     if self.__nonblk_bad_nterm and auth_atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                         continue
 
+                                    if self.__remediation_mode and auth_atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                        continue
+
                                     warn = f"Unmatched Auth_atom_ID {auth_atom_id!r} (Auth_comp_ID {auth_comp_id})."
 
                                     self.report.warning.appendDescription('auth_atom_nomenclature_mismatch',
                                                                           {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                            'description': warn})
                                     self.report.setWarning()
 
@@ -18500,14 +18537,17 @@
                                 if (set(auth_atom_ids) | set(atom_ids)) != set(atom_ids):
 
                                     for auth_atom_id in (set(auth_atom_ids) | set(atom_ids)) - set(atom_ids):
 
                                         if self.__nonblk_bad_nterm and auth_atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                             continue
 
+                                        if self.__remediation_mode and auth_atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                            continue
+
                                         warn = f"Unmatched Auth_atom_ID {auth_atom_id!r} (Auth_comp_ID {comp_id}, non-standard residue)."
 
                                         self.report.warning.appendDescription('auth_atom_nomenclature_mismatch',
                                                                               {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                                'description': warn})
                                         self.report.setWarning()
 
@@ -18519,14 +18559,17 @@
                             if not has_comp_id:
 
                                 for auth_atom_id in auth_atom_ids:
 
                                     if self.__nonblk_bad_nterm and auth_atom_id in ('H1', 'HT1'):  # and comp_id in first_comp_ids:
                                         continue
 
+                                    if self.__remediation_mode and auth_atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                        continue
+
                                     warn = f"Unmatched Auth_atom_ID {auth_atom_id!r} (Auth_comp_ID {comp_id}, non-standard residue)."
 
                                     self.report.warning.appendDescription('auth_atom_nomenclature_mismatch',
                                                                           {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                            'description': warn})
                                     self.report.setWarning()
 
@@ -18879,14 +18922,17 @@
 
                             if self.__verbose:
                                 self.__lfh.write(f"+NmrDpUtility.__validateAtomTypeOfCsLoop() ++ Error  - {err}\n")
 
                     for atom_id in atom_ids:
                         if not atom_id.startswith(atom_type):
 
+                            if self.__remediation_mode and atom_id[0] in ('Q', 'M'):  # DAOTHER-8663
+                                continue
+
                             err = f"Invalid atom_id {atom_id!r} (atom_type {atom_type}) in a loop {lp_category}."
 
                             self.report.error.appendDescription('invalid_atom_nomenclature',
                                                                 {'file_name': file_name, 'sf_framecode': sf_framecode, 'category': lp_category,
                                                                  'description': err})
                             self.report.setError()
 
@@ -23172,25 +23218,25 @@
                 if atom_id in self.__csStat.getRepMethylProtons(comp_id):
                     missing_ch3 = self.__csStat.getProtonsInSameGroup(comp_id, atom_id, True)
                     valid = self.__sail_flag
                     for offset in range(1, 10):
                         row_src = src_lp.data[src_idx]
                         if src_idx + offset < len(src_lp.data):
                             row = src_lp.data[src_idx + offset]
-                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == str(row_src[3])))\
-                               and row[comp_id_col] == _row[5]\
+                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == row_src[seq_id_col]))\
+                               and row[comp_id_col].upper() == comp_id\
                                and row[atom_id_col] in missing_ch3:
                                 valid = True
                                 missing_ch3.remove(row[atom_id_col])
                                 if len(missing_ch3) == 0:
                                     break
                         if src_idx - offset >= 0:
                             row = src_lp.data[src_idx - offset]
-                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == str(row_src[3])))\
-                               and row[comp_id_col] == _row[5]\
+                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == row_src[seq_id_col]))\
+                               and row[comp_id_col].upper() == comp_id\
                                and row[atom_id_col] in missing_ch3:
                                 valid = True
                                 missing_ch3.remove(row[atom_id_col])
                                 if len(missing_ch3) == 0:
                                     break
                 if atom_id in _coord_atom_site['atom_id'] and valid and len(missing_ch3) == 0:
                     _row[6] = atom_id
@@ -23292,25 +23338,25 @@
                 if atom_id in self.__csStat.getRepMethylProtons(comp_id):
                     missing_ch3 = self.__csStat.getProtonsInSameGroup(comp_id, atom_id, True)
                     valid = self.__sail_flag
                     for offset in range(1, 10):
                         row_src = src_lp.data[src_idx]
                         if src_idx + offset < len(src_lp.data):
                             row = src_lp.data[src_idx + offset]
-                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == str(row_src[3])))\
-                               and row[comp_id_col] == _row[5]\
+                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == row_src[seq_id_col]))\
+                               and row[comp_id_col].upper() == comp_id\
                                and row[6] in missing_ch3:
                                 valid = True
                                 missing_ch3.remove(row[6])
                                 if len(missing_ch3) == 0:
                                     break
                         if src_idx - offset >= 0:
                             row = src_lp.data[src_idx - offset]
-                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == str(row_src[3])))\
-                               and row[comp_id_col] == _row[5]\
+                            if (row[seq_id_col] == str(_row[3]) or (_row[3] != row_src[3] and row[seq_id_col] == row_src[seq_id_col]))\
+                               and row[comp_id_col].upper() == comp_id\
                                and row[6] in missing_ch3:
                                 valid = True
                                 missing_ch3.remove(row[6])
                                 if len(missing_ch3) == 0:
                                     break
                 if len(missing_ch3) > 0 and (_row[9] in emptyValue or float(_row[9]) >= 3.0):
                     missing_ch3 = []
@@ -23561,17 +23607,17 @@
                                 has_orig_seq = True
                                 break
                         if has_orig_seq:
                             orig_pdb_tags.append('Comp_ID')
                             orig_pdb_tags.append('Atom_ID')
                             dat = get_lp_tag(loop, orig_pdb_tags)
                             for row in dat:
-                                orig_atom_id = row[3].upper()
-                                if orig_atom_id in emptyValue:
+                                if row[3] in emptyValue:
                                     continue
+                                orig_atom_id = row[3].upper()
                                 comp_id = row[4]
                                 atom_id = row[5]
                                 if orig_atom_id == atom_id:
                                     continue
                                 ambig_code = self.__csStat.getMaxAmbigCodeWoSetId(comp_id, atom_id)
                                 if ambig_code == 0 or atom_id[0] not in protonBeginCode:
                                     continue
@@ -24093,15 +24139,121 @@
                                 else:
                                     resolved = False
 
                             except (ValueError, TypeError):
                                 resolved = False
 
                         else:
-                            resolved = False
+
+                            can_auth_asym_id = [_auth_asym_id for _auth_asym_id, _auth_seq_id, _comp_id in self.__caC['auth_to_star_seq']
+                                                if _auth_seq_id == seq_id and _comp_id == comp_id]
+
+                            if len(can_auth_asym_id) != 1:
+                                resolved = False
+
+                            else:
+                                auth_asym_id, auth_seq_id = can_auth_asym_id[0], seq_id
+
+                                seq_key = (auth_asym_id, auth_seq_id, comp_id)
+                                _seq_key = (seq_key[0], seq_key[1])
+                                if seq_key in auth_to_star_seq:
+                                    entity_assembly_id, seq_id, entity_id, _ = auth_to_star_seq[seq_key]
+                                    self.__ent_asym_id_with_exptl_data.add(entity_assembly_id)
+                                    _row[1], _row[2], _row[3], _row[4] =\
+                                        entity_assembly_id, entity_id, seq_id, seq_id
+
+                                    _row[16], _row[17], _row[18], _row[19] =\
+                                        auth_asym_id, auth_seq_id, comp_id, atom_id
+                                    if has_ins_code and seq_key in auth_to_ins_code:
+                                        _row[27] = auth_to_ins_code[seq_key]
+
+                                    if seq_key in auth_to_orig_seq:
+                                        if _row[20] not in emptyValue and seq_key not in _auth_to_orig_seq:
+                                            orig_seq_id, orig_comp_id = auth_to_orig_seq[seq_key]
+                                            _auth_to_orig_seq[seq_key] = (_row[20], orig_seq_id, orig_comp_id)
+                                        if not has_orig_seq:
+                                            orig_seq_id, orig_comp_id = auth_to_orig_seq[seq_key]
+                                            if orig_seq_id in emptyValue:
+                                                orig_seq_id = auth_seq_id
+                                            if orig_comp_id in emptyValue:
+                                                orig_comp_id = comp_id
+                                            _row[20], _row[21], _row[22], _row[23] =\
+                                                auth_asym_id, orig_seq_id, orig_comp_id, _orig_atom_id
+                                        elif any(d in emptyValue for d in orig_dat[idx]):
+                                            if seq_key in _auth_to_orig_seq:
+                                                _row[20], _row[21], _row[22] = _auth_to_orig_seq[seq_key]
+                                            if _row[23] in emptyValue:
+                                                _row[23] = atom_id
+                                            ambig_code = self.__csStat.getMaxAmbigCodeWoSetId(comp_id, atom_id)
+                                            if ambig_code > 0:
+                                                orig_seq_id, orig_comp_id = auth_to_orig_seq[seq_key]
+                                                if orig_seq_id in emptyValue:
+                                                    orig_seq_id = auth_seq_id
+                                                if orig_comp_id in emptyValue:
+                                                    orig_comp_id = comp_id
+                                                _row[20], _row[21], _row[22] =\
+                                                    auth_asym_id, orig_seq_id, orig_comp_id
+                                                if atom_id[0] not in protonBeginCode:
+                                                    _row[23] = atom_id
+                                                else:
+                                                    len_in_grp = len(self.__csStat.getProtonsInSameGroup(comp_id, atom_id))
+                                                    if len_in_grp == 2:
+                                                        _row[23] = (atom_id[0:-1] + '1')\
+                                                            if ambig_code == 2 and ch2_name_in_xplor and atom_id[-1] == '3' else atom_id
+                                                    elif len_in_grp == 3:
+                                                        _row[23] = (atom_id[-1] + atom_id[0:-1])\
+                                                            if ch3_name_in_xplor and atom_id[0] == 'H' and atom_id[-1] in ('1', '2', '3') else atom_id
+                                                    elif _row[23] in emptyValue:
+                                                        _row[23] = atom_id
+
+                                    else:
+                                        seq_key = next((k for k, v in auth_to_star_seq.items()
+                                                        if v[0] == entity_assembly_id and v[1] == seq_id and v[2] == entity_id), None)
+                                        if seq_key is not None:
+                                            _seq_key = (seq_key[0], seq_key[1])
+                                            _row[16], _row[17], _row[18], _row[19] =\
+                                                seq_key[0], seq_key[1], seq_key[2], atom_id
+                                            if has_ins_code and seq_key in auth_to_ins_code:
+                                                _row[27] = auth_to_ins_code[seq_key]
+
+                                        if has_auth_seq:
+                                            _row[20], _row[21], _row[22], _row[23] =\
+                                                row[auth_asym_id_col], row[auth_seq_id_col],\
+                                                row[auth_comp_id_col], row[auth_atom_id_col]
+
+                                    index, _row = fill_cs_row(lp, index, _row, coord_atom_site, _seq_key, comp_id, atom_id, loop, idx)
+
+                                else:
+
+                                    item = next((item for item in self.__caC['entity_assembly'] if item['auth_asym_id'] == auth_asym_id), None)
+
+                                    if item is not None and ps is not None and any(_ps for _ps in ps if _ps['chain_id'] == auth_asym_id and auth_seq_id in _ps['seq_id']):
+                                        entity_assembly_id = item['entity_assembly_id']
+                                        entity_id = item['entity_id']
+
+                                        _row[1], _row[2], _row[3], _row[4] = entity_assembly_id, entity_id, seq_id, seq_id
+
+                                        seq_key = next((k for k, v in auth_to_star_seq.items()
+                                                        if v[0] == entity_assembly_id and v[1] == seq_id and v[2] == entity_id), None)
+                                        if seq_key is not None:
+                                            _seq_key = (seq_key[0], seq_key[1])
+                                            _row[16], _row[17], _row[18], _row[19] =\
+                                                seq_key[0], seq_key[1], seq_key[2], atom_id
+                                            if has_ins_code and seq_key in auth_to_ins_code:
+                                                _row[27] = auth_to_ins_code[seq_key]
+
+                                        if has_auth_seq:
+                                            _row[20], _row[21], _row[22], _row[23] =\
+                                                row[auth_asym_id_col], row[auth_seq_id_col],\
+                                                row[auth_comp_id_col], row[auth_atom_id_col]
+
+                                        index, _row = fill_cs_row(lp, index, _row, coord_atom_site, _seq_key, comp_id, atom_id, loop, idx)
+
+                                    else:
+                                        resolved = False
 
                     if not resolved and has_auth_seq:
                         try:
                             seq_id = int(row[auth_seq_id_col])
                         except (ValueError, TypeError):
                             seq_id = None
 
@@ -28453,15 +28605,15 @@
                 if _rest_id is None:
                     pass
 
                 elif rest_id != _rest_id and len(atom1) > 0 and len(atom2) > 0:
 
                     if member_id in emptyValue or member_logic_code == 'OR':
 
-                        if (not isAmbigAtomSelection([atom1, _atom1], self.__csStat) and not isAmbigAtomSelection([atom2, _atom2], self.__csStat))\
+                        if (values == _values and not isAmbigAtomSelection([atom1, _atom1], self.__csStat) and not isAmbigAtomSelection([atom2, _atom2], self.__csStat))\
                            or (values == _values and atom1['ref_chain_id'] != atom2['ref_chain_id']
                                and ((not isAmbigAtomSelection([atom1, _atom1], self.__csStat)
                                      and atom1['ref_chain_id'] != _atom2['ref_chain_id'] and atom2['comp_id'] == _atom2['comp_id'])
                                     or (not isAmbigAtomSelection([atom2, _atom2], self.__csStat)
                                         and atom2['ref_chain_id'] != _atom1['ref_chain_id'] and atom1['comp_id'] == _atom1['comp_id']))):
                             _row[member_logic_code_col] = 'OR'
 
@@ -34094,15 +34246,15 @@
             if len(redu_count) > 0:
                 ent['number_of_redundant_constraints'] = redu_count
             if polymer_sequence is not None:
                 ent['constraints_per_residue'] = count_per_residue
                 ent['constraints_on_contact_map'] = count_on_map
             if has_inter_chain_constraint:
                 ent['constraints_on_asym_contact_map'] = count_on_asym_map
-            ent['range'] = {'max_value': max_val, 'min_value': min_val}
+            ent['range'] = {'max_value': float(f'{max_val:.2f}'), 'min_value': float(f'{min_val:.2f}')}
             if len(weights) > 0:
                 _weights = {}
                 for k, v in weights.items():
                     _weights[k] = collections.Counter(v).most_common()
                 ent['weight_of_constraints'] = _weights
             if len(potential_types) > 0:
                 _potential_types = {}
@@ -36429,15 +36581,15 @@
                 ent['number_of_combined_constraints'] = comb_count
             if len(inco_count) > 0:
                 ent['number_of_inconsistent_constraints'] = inco_count
             if len(redu_count) > 0:
                 ent['number_of_redundant_constraints'] = redu_count
             if polymer_sequence is not None:
                 ent['constraints_per_residue'] = value_per_residue
-            ent['range'] = {'max_value': max_val_, 'min_value': min_val_}
+            ent['range'] = {'max_value': float(f'{max_val_:.2f}'), 'min_value': float(f'{min_val_:.2f}')}
             if len(weights) > 0:
                 _weights = {}
                 for k, v in weights.items():
                     _weights[k] = collections.Counter(v).most_common()
                 ent['weight_of_constraints'] = _weights
             if len(potential_types) > 0:
                 _potential_types = {}
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrStarToCif.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrStarToCif.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/NmrVrptUtility.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/NmrVrptUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 ##
 # File: NmrVrptUtility.py
 # Date: 19-Apr-2023
 #
 # Updates:
+# 19-Jul-2023  M. Yokochi - add trustPdbxAuthAtomName() for OneDep validation package (DAOTHER-8705)
+# 19-Jul-2023  M. Yokochi - fix distance/dihedral angle/RDC averaging when lower/upper bounds are different in a restraint (DAOTER-8705)
 ##
 """ Wrapper class for NMR restraint validation.
     @author: Masashi Yokochi
     @note: This class is alternative implementation of wwpdb.apps.validation.src.RestraintValidation.BMRBRestraintsAnalysis
 """
 import os
 import sys
@@ -155,14 +157,17 @@
           Michael Nilges.
           J. Mol. Biol. (1995) 245, 645–660.
           DOI: 10.1006/jmbi.1994.0053
         @author: Kumaran Baskaran
         @see: wwpdb.apps.validation.src.RestraintValidation.BMRBRestraintsAnalysis.r6sum
     """
 
+    if len(r_list) == 1:
+        return r_list[0]
+
     return sum(r ** (-6.0) for r in r_list) ** (-1.0 / 6.0)
 
 
 def dist_target_values(target_value, target_value_uncertainty,
                        lower_limit, upper_limit,
                        lower_linear_limit, upper_linear_limit):
     """ Return estimated distance target value, lower_bound, upper_bound.
@@ -462,14 +467,15 @@
 
     def __init__(self, verbose=False, log=sys.stderr,
                  cR=None, caC=None, ccU=None, csStat=None):
         self.__verbose = verbose
         self.__lfh = log
 
         self.__debug = False
+        self.__trust_pdbx_auth_atom_name = False
         self.__use_cache = cR is not None and caC is not None
 
         # auxiliary input resource
         self.__inputParamDict = {}
 
         # auxiliary output resource
         self.__outputParamDict = {}
@@ -602,14 +608,21 @@
 
     def setDebugMode(self, debug):
         """ Set debug mode.
         """
 
         self.__debug = debug
 
+    def trustPdbxAuthAtomName(self, trust_pdbx_auth_atom_name):
+        """ Whether to trust _atom_site.pdbx_auth_atom_name rather than _atom_site.auth_atom_id.
+            @note: Set True for OneDep validation package.
+        """
+
+        self.__trust_pdbx_auth_atom_name = trust_pdbx_auth_atom_name
+
     def useCache(self, use_cache):
         """ Use cache file(s) of the previous run.
             Do not enable this for generation of wwPDB validation report because of no performance improvement.
         """
 
         self.__use_cache = use_cache
 
@@ -1105,18 +1118,22 @@
 
             vrpt_atom_site_cache_path = os.path.join(self.__cacheDirPath, f"{self.__cifHashCode}_vrpt_atom_site.pkl")
             self.__coordinates = load_from_pickle(vrpt_atom_site_cache_path, None)
 
             if self.__atomIdList is not None and self.__coordinates is not None:
                 return True
 
+        _auth_atom_id = 'pdbx_auth_atom_name'\
+            if self.__trust_pdbx_auth_atom_name and self.__cR.hasItem('atom_site', 'pdbx_auth_atom_name')\
+            else 'auth_atom_id'
+
         data_items = [{'name': 'auth_asym_id', 'type': 'str'},
                       {'name': 'auth_seq_id', 'type': 'int'},
                       {'name': 'auth_comp_id', 'type': 'str'},
-                      {'name': 'auth_atom_id', 'type': 'str'},
+                      {'name': _auth_atom_id, 'type': 'str', 'alt_name': 'auth_atom_id'},
                       {'name': 'label_asym_id', 'type': 'str'},
                       {'name': 'label_seq_id', 'type': 'int'},
                       {'name': 'label_comp_id', 'type': 'str'},
                       {'name': 'label_atom_id', 'type': 'str'},
                       {'name': 'label_entity_id', 'type': 'int'},
                       {'name': 'label_alt_id', 'type': 'str', 'default': '.'},
                       {'name': 'pdbx_PDB_ins_code', 'type': 'str', 'default': '?'},
@@ -1768,22 +1785,27 @@
 
             def calc_dist_rest_viol(rest_key, restraints):
 
                 error_per_model = {}
 
                 for model_id in self.__coordinates:
 
-                    dist_list = []
+                    dist_list_set = {}
 
                     for r in restraints:
                         atom_key_1 = r['atom_key_1']
                         atom_key_2 = r['atom_key_2']
                         lower_bound = r['lower_bound']
                         upper_bound = r['upper_bound']
 
+                        bound_key = (lower_bound, upper_bound)
+
+                        if bound_key not in dist_list_set:
+                            dist_list_set[bound_key] = []
+
                         atom_present = True
 
                         try:
                             pos_1 = self.__coordinates[model_id][atom_key_1]
                         except KeyError:
                             if self.__verbose:
                                 self.__lfh.write(f"Atom (auth_asym_id: {atom_key_1[0]}, auth_seq_id: {atom_key_1[1]}, "
@@ -1797,28 +1819,39 @@
                             if self.__verbose:
                                 self.__lfh.write(f"Atom (auth_asym_id: {atom_key_2[0]}, auth_seq_id: {atom_key_2[1]}, "
                                                  f"comp_id: {atom_key_2[2]}, atom_id: {atom_key_2[3]}) "
                                                  f"not found in the coordinates for distance restraint {rest_key}.\n")
                             atom_present = False
 
                         if atom_present:
+
                             d = distance(pos_1, pos_2)
                             if d == 0.0:
                                 self.__lfh.write(f"+NmrVrptUtility.__calculateDistanceRestraintViolations() ++ Error  - distance restraint {rest_key} {r} does not make sense, "
                                                  f"{os.path.basename(self.__nmrDataPath)}.\n")
-                            dist_list.append(d)
+                            dist_list_set[bound_key].append(d)
                         else:
                             self.__distRestUnmapped.append(rest_key)
 
                     error = None
 
-                    if len(dist_list) > 0:
-                        avr_d = dist_inv_6_summed(dist_list)
+                    if len(dist_list_set) > 0:
+
+                        for bound_key, dist_list in dist_list_set.items():
+
+                            if len(dist_list) == 0:
+                                continue
+
+                            lower_bound, upper_bound = bound_key
+                            avr_d = dist_inv_6_summed(dist_list)
+
+                            _error = dist_error(lower_bound, upper_bound, avr_d)
 
-                        error = dist_error(lower_bound, upper_bound, avr_d)
+                            if error is None or error > _error:
+                                error = _error
 
                     error_per_model[model_id] = error
 
                 return error_per_model
 
             def fill_smaller_error_for_each_model(error_per_model, min_error_per_model,
                                                   combination_id, member_id, min_comb_key_per_model):
@@ -1950,25 +1983,30 @@
 
             def calc_dihed_rest_viol(rest_key, restraints):
 
                 error_per_model = {}
 
                 for model_id in self.__coordinates:
 
-                    angle_list = []
+                    angle_list_set = {}
 
                     for r in restraints:
                         atom_key_1 = r['atom_key_1']
                         atom_key_2 = r['atom_key_2']
                         atom_key_3 = r['atom_key_3']
                         atom_key_4 = r['atom_key_4']
                         lower_bound = r['lower_bound']
                         upper_bound = r['upper_bound']
                         target_value = r['target_value']
 
+                        bound_key = (lower_bound, upper_bound, target_value)
+
+                        if bound_key not in angle_list_set:
+                            angle_list_set[bound_key] = []
+
                         atom_present = True
 
                         try:
                             pos_1 = self.__coordinates[model_id][atom_key_1]
                         except KeyError:
                             if self.__verbose:
                                 self.__lfh.write(f"Atom (auth_asym_id: {atom_key_1[0]}, auth_seq_id: {atom_key_1[1]}, "
@@ -2001,24 +2039,34 @@
                                 self.__lfh.write(f"Atom (auth_asym_id: {atom_key_4[0]}, auth_seq_id: {atom_key_4[1]}, "
                                                  f"comp_id: {atom_key_4[2]}, atom_id: {atom_key_4[3]}) "
                                                  f"not found in the coordinates for dihedral angle restraint {rest_key}.\n")
                             atom_present = False
 
                         if atom_present:
                             a = dihedral_angle(pos_1, pos_2, pos_3, pos_4) + 180.0
-                            angle_list.append(a)
+                            angle_list_set[bound_key].append(a)
                         else:
                             self.__dihedRestUnmapped.append(rest_key)
 
                     error = None
 
-                    if len(angle_list) > 0:
-                        avr_a = np.mean(np.array(angle_list)) - 180.0
+                    if len(angle_list_set) > 0:
+
+                        for bound_key, angle_list in angle_list_set.items():
+
+                            if len(angle_list) == 0:
+                                continue
+
+                            lower_bound, upper_bound, target_value = bound_key
+                            avr_a = np.mean(np.array(angle_list)) - 180.0
+
+                            _error = angle_error(lower_bound, upper_bound, target_value, avr_a)
 
-                        error = angle_error(lower_bound, upper_bound, target_value, avr_a)
+                            if error is None or error > _error:
+                                error = _error
 
                     error_per_model[model_id] = error
 
                 return error_per_model
 
             def fill_smaller_error_for_each_model(error_per_model, min_error_per_model,
                                                   combination_id, min_comb_key_per_model):
@@ -2114,22 +2162,27 @@
 
             def calc_rdc_rest_viol(rest_key, restraints):
 
                 error_per_model = {}
 
                 for model_id in self.__coordinates:
 
-                    rdc_list = []
+                    rdc_list_set = {}
 
                     for r in restraints:
                         atom_key_1 = r['atom_key_1']
                         atom_key_2 = r['atom_key_2']
                         lower_bound = r['lower_bound']
                         upper_bound = r['upper_bound']
 
+                        bound_key = (lower_bound, upper_bound)
+
+                        if bound_key not in rdc_list_set:
+                            rdc_list_set[bound_key] = []
+
                         atom_present = True
 
                         try:
                             pos_1 = self.__coordinates[model_id][atom_key_1]  # noqa: F841, pylint: disable='unused-variable'
                         except KeyError:
                             if self.__verbose:
                                 self.__lfh.write(f"Atom (auth_asym_id: {atom_key_1[0]}, auth_seq_id: {atom_key_1[1]}, "
@@ -2145,26 +2198,36 @@
                                                  f"comp_id: {atom_key_2[2]}, atom_id: {atom_key_2[3]}) "
                                                  f"not found in the coordinates for RDC restraint {rest_key}.\n")
                             atom_present = False
 
                         if atom_present:
                             # """ TODO: rdc() should return calculated RDC value for a given vector using the RDC alignment tensor of rest_key[0]
                             # r = rdc(rest_key[0], pos_1, pos_2)
-                            # rdc_list.append(r)
+                            # rdc_list_set[bound_key].append(r)
                             # """
                             pass
                         else:
                             self.__rdcRestUnmapped.append(rest_key)
 
                     error = None
 
-                    if len(rdc_list) > 0:
-                        avr_r = np.mean(np.array(rdc_list))
+                    if len(rdc_list_set) > 0:
+
+                        for bound_key, rdc_list in rdc_list_set.items():
+
+                            if len(rdc_list) == 0:
+                                continue
+
+                            lower_bound, upper_bound = bound_key
+                            avr_r = np.mean(np.array(rdc_list))
+
+                            _error = rdc_error(lower_bound, upper_bound, avr_r)
 
-                        error = rdc_error(lower_bound, upper_bound, avr_r)
+                            if error is None or error > _error:
+                                error = _error
 
                     error_per_model[model_id] = error
 
                 return error_per_model
 
             def fill_smaller_error_for_each_model(error_per_model, min_error_per_model,
                                                   combination_id, min_comb_key_per_model):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/aa_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/dna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/others.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/others.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_filt.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.csv`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/bmrb_cs_stat/rna_full.pkl`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/ChemCompIo.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/CifReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/CifReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/io/mmCIFUtil.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/io/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from AmberMRLexer.g4 by ANTLR 4.12.0
+# Generated from AmberMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -1270,13 +1270,13 @@
                   "R_quot", "SPACE_F", "Ambig_code_MP", "Integer_MP", "Simple_name_MP", 
                   "Equ_op_MP", "SPACE_MP", "RETURN_MP", "LINE_COMMENT_MP" ]
 
     grammarFileName = "AmberMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from AmberMRParser.g4 by ANTLR 4.12.0
+# Generated from AmberMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -845,15 +845,15 @@
     Equ_op_MP=232
     SPACE_MP=233
     RETURN_MP=234
     LINE_COMMENT_MP=235
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Amber_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from AmberPTLexer.g4 by ANTLR 4.12.0
+# Generated from AmberPTLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -644,13 +644,13 @@
                   "SPACE_AA", "FLAG_AA", "Integer", "SPACE_IA", "FLAG_IA", 
                   "Real", "SPACE_EA", "FLAG_EA" ]
 
     grammarFileName = "AmberPTLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from AmberPTParser.g4 by ANTLR 4.12.0
+# Generated from AmberPTParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -445,15 +445,15 @@
     FLAG_IA=71
     Real=72
     SPACE_EA=73
     FLAG_EA=74
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Amber_ptContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTParserListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,18 +275,19 @@
                 if compId not in monDict3 and self.__mrAtomNameMapping is not None and atomName[0] in protonBeginCode:
                     _, compId, _atomName = retrieveAtomIdentFromMRMap(self.__mrAtomNameMapping, _seqId, compId, atomName)
                     if _atomName != atomName:
                         atomName = _atomName
                         retrievedAtomNumList.append(atomNum)
                 overrun = False
                 # the second condition indicates metal ions
-                if terminus[atomNum - 2]\
+                if (terminus[atomNum - 2] and not prevCompId.endswith('5'))\
                    or (prevCompId is not None and prevCompId.endswith('3') and compId.endswith('5')
                        and not any(t for t in canceledTermNum if t - 10 < atomNum < t + 10))\
-                   or (compId == atomName and compId.title() in NAMES_ELEMENT)\
+                   or (compId == atomName and compId.split('+')[0].title() in NAMES_ELEMENT)\
+                   or (compId == atomName and compId.split('-')[0].title() in NAMES_ELEMENT)\
                    or (len(prevAtomName) > 0 and prevAtomName[0] not in NON_METAL_ELEMENTS and prevSeqId != _seqId):
 
                     if len(self.__polySeqPrmTop) > 0 and len(seqIdList) > 1 and prevAtomName.endswith('T'):
                         seqIdList.pop()
                         compIdList.pop()
                         overrun = True
 
@@ -589,29 +590,33 @@
             if len(self.__seqAlign) == 0:
                 mrFormatName = getRestraintFormatName(self.__file_type)
                 _a_mr_format_name = 'the ' + mrFormatName
 
                 ref_code = getOneLetterCodeSequence(self.__polySeqModel[0]['comp_id'])
                 test_code = getOneLetterCodeSequence(self.__polySeqPrmTop[0]['comp_id'])
 
-                if abs(len(ref_code) - len(test_code)) < 20 and ref_code > 40:
+                hint = ''
+                if abs(len(ref_code) - len(test_code)) < 20 and len(ref_code) > 40:
                     hint = f"For example, coordinates ({self.__polySeqModel[0]['auth_chain_id']}): {ref_code} vs topology: {test_code}. "
 
                 self.__f.append(f"[Sequence mismatch] Polymer sequence between the coordinate and {_a_mr_format_name} data does not match. {hint}"
                                 "Please verify the two sequences and re-upload the correct file(s) if required.")
 
             assi_ref_chain_ids = {}
             proc_test_chain_ids = []
             atom_nums = []
             delete_atom_nums = []
 
             def update_atom_num(seq_align, orphan):
                 ref_chain_id = seq_align['ref_chain_id']
                 test_chain_id = seq_align['test_chain_id']
 
+                if ref_chain_id in assi_ref_chain_ids or test_chain_id in proc_test_chain_ids:
+                    return
+
                 ps_cif = next(ps for ps in self.__polySeqModel if ps['auth_chain_id'] == ref_chain_id)
 
                 if ref_chain_id not in assi_ref_chain_ids:
                     assi_ref_chain_ids[ref_chain_id] = seq_align['length'] - seq_align['matched'] - seq_align['conflict']
                 else:
                     assi_ref_chain_ids[ref_chain_id] -= seq_align['matched'] + seq_align['conflict']
                 proc_test_chain_ids.append(test_chain_id)
@@ -627,15 +632,15 @@
                         test_seq_id = atomNum['seq_id']
 
                         if first_seq_id is None:
                             first_seq_id = test_seq_id
 
                         if test_seq_id in seq_align['test_seq_id']:
                             idx = seq_align['test_seq_id'].index(test_seq_id)
-                            if idx < len(seq_align['ref_auth_seq_id']):
+                            if 'ref_auth_seq_id' in seq_align and idx < len(seq_align['ref_auth_seq_id']):
                                 ref_seq_id = seq_align['ref_auth_seq_id'][idx]
                             elif offset is not None:
                                 ref_seq_id = test_seq_id + offset
                             else:
                                 continue
                         elif offset is not None:
                             ref_seq_id = test_seq_id + offset
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/AmberPTReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/AmberPTReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,18 @@
         finally:
             if isFilePath and ifh is not None:
                 ifh.close()
 
 
 if __name__ == "__main__":
     reader = AmberPTReader(True)
+    reader.parse('../../tests-nmr/mock-data-daother-8685/FANA3_0M_ZDNAminwat.prmtop',
+                 '../../tests-nmr/mock-data-daother-8685/D_800590_model_P1.cif.V4')
+
+    reader = AmberPTReader(True)
     reader.parse('../../tests-nmr/mock-data-remediation/7b72/ds.prmtop',
                  '../../tests-nmr/mock-data-remediation/7b72/7b72.cif')
 
     reader = AmberPTReader(True)
     reader.parse('../../tests-nmr/mock-data-daother-7690/D_1300028390_mr-upload_P1.dat.V1',
                  '../../tests-nmr/mock-data-daother-7690/D_1300028390_model-annotate_P1.cif.V2')
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from BiosymMRLexer.g4 by ANTLR 4.12.0
+# Generated from BiosymMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -181,13 +181,13 @@
                   "SIMPLE_NAME", "Ordinal", "SPACE", "ENCLOSE_COMMENT", 
                   "SECTION_COMMENT", "LINE_COMMENT" ]
 
     grammarFileName = "BiosymMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from BiosymMRParser.g4 by ANTLR 4.12.0
+# Generated from BiosymMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -119,15 +119,15 @@
     SPACE=10
     ENCLOSE_COMMENT=11
     SECTION_COMMENT=12
     LINE_COMMENT=13
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Biosym_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/BiosymMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/BiosymMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CharmmMRLexer.g4 by ANTLR 4.12.0
+# Generated from CharmmMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -1288,13 +1288,13 @@
                   "Any_name", "SPACE_CM", "RETURN_CM", "Abs", "Attr_properties", 
                   "Comparison_ops", "SPACE_AP" ]
 
     grammarFileName = "CharmmMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CharmmMRParser.g4 by ANTLR 4.12.0
+# Generated from CharmmMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -680,15 +680,15 @@
     Abs=177
     Attr_properties=178
     Comparison_ops=179
     SPACE_AP=180
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Charmm_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CharmmMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CharmmMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CnsMRLexer.g4 by ANTLR 4.12.0
+# Generated from CnsMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -2237,13 +2237,13 @@
                   "Symbol_name_CF", "Simple_name_CF", "SPACE_CF", "COMMENT_CF", 
                   "Simple_name_LL", "SPACE_LL" ]
 
     grammarFileName = "CnsMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CnsMRParser.g4 by ANTLR 4.12.0
+# Generated from CnsMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -1305,15 +1305,15 @@
     SPACE_CF=251
     COMMENT_CF=252
     Simple_name_LL=253
     SPACE_LL=254
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Cns_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CnsMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CnsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRLexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CyanaMRLexer.g4 by ANTLR 4.12.0
+# Generated from CyanaMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -507,13 +507,13 @@
                   "Integer_MP", "Simple_name_MP", "Equ_op_MP", "SPACE_MP", 
                   "RETURN_MP", "LINE_COMMENT_MP" ]
 
     grammarFileName = "CyanaMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from CyanaMRParser.g4 by ANTLR 4.12.0
+# Generated from CyanaMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -408,15 +408,15 @@
     Equ_op_MP=54
     SPACE_MP=55
     RETURN_MP=56
     LINE_COMMENT_MP=57
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Cyana_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/CyanaMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/CyanaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from DynamoMRLexer.g4 by ANTLR 4.12.0
+# Generated from DynamoMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -799,13 +799,13 @@
                   "Class", "SPACE_VA", "RETURN_VA", "LINE_COMMENT_VA", "Format_code", 
                   "SPACE_FO", "RETURN_FO", "LINE_COMMENT_FO" ]
 
     grammarFileName = "DynamoMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from DynamoMRParser.g4 by ANTLR 4.12.0
+# Generated from DynamoMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -643,15 +643,15 @@
     Format_code=122
     SPACE_FO=123
     RETURN_FO=124
     LINE_COMMENT_FO=125
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Dynamo_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/DynamoMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/DynamoMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from GromacsMRLexer.g4 by ANTLR 4.12.0
+# Generated from GromacsMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -239,13 +239,13 @@
                   "ATM_TYPE_CHAR", "SIMPLE_NAME", "SPACE", "ENCLOSE_COMMENT", 
                   "SECTION_COMMENT", "LINE_COMMENT" ]
 
     grammarFileName = "GromacsMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from GromacsMRParser.g4 by ANTLR 4.12.0
+# Generated from GromacsMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -125,15 +125,15 @@
     SPACE=16
     ENCLOSE_COMMENT=17
     SECTION_COMMENT=18
     LINE_COMMENT=19
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Gromacs_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from GromacsPTLexer.g4 by ANTLR 4.12.0
+# Generated from GromacsPTLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -420,13 +420,13 @@
                   "SECTION_COMMENT", "LINE_COMMENT", "R_brkt_AA", "SECTION_COMMENT_AA", 
                   "LINE_COMMENT_AA", "Simple_name_AA", "SPACE_AA", "RETURN_AA" ]
 
     grammarFileName = "GromacsPTLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from GromacsPTParser.g4 by ANTLR 4.12.0
+# Generated from GromacsPTParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -389,15 +389,15 @@
     LINE_COMMENT_AA=42
     Simple_name_AA=43
     SPACE_AA=44
     RETURN_AA=45
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Gromacs_ptContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTParserListener.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,18 +223,19 @@
                 if compId not in monDict3 and self.__mrAtomNameMapping is not None and atomName[0] in protonBeginCode:
                     _, compId, _atomName = retrieveAtomIdentFromMRMap(self.__mrAtomNameMapping, _seqId, compId, atomName)
                     if _atomName != atomName:
                         atomName = _atomName
                         retrievedAtomNumList.append(atomNum)
                 overrun = False
                 # the second condition indicates metal ions
-                if terminus[atomNum - 2]\
+                if (terminus[atomNum - 2] and not prevCompId.endswith('5'))\
                    or (prevCompId is not None and prevCompId.endswith('3') and compId.endswith('5')
                        and not any(t for t in canceledTermNum if t - 10 < atomNum < t + 10))\
-                   or (compId == atomName and compId.title() in NAMES_ELEMENT)\
+                   or (compId == atomName and compId.split('+')[0].title() in NAMES_ELEMENT)\
+                   or (compId == atomName and compId.split('-')[0].title() in NAMES_ELEMENT)\
                    or (len(prevAtomName) > 0 and prevAtomName[0] not in NON_METAL_ELEMENTS and prevSeqId != _seqId):
 
                     if len(self.__polySeqPrmTop) > 0 and len(seqIdList) > 1 and prevAtomName.endswith('T'):
                         seqIdList.pop()
                         compIdList.pop()
                         overrun = True
 
@@ -537,29 +538,33 @@
             if len(self.__seqAlign) == 0:
                 mrFormatName = getRestraintFormatName(self.__file_type)
                 _a_mr_format_name = 'the ' + mrFormatName
 
                 ref_code = getOneLetterCodeSequence(self.__polySeqModel[0]['comp_id'])
                 test_code = getOneLetterCodeSequence(self.__polySeqPrmTop[0]['comp_id'])
 
-                if abs(len(ref_code) - len(test_code)) < 20 and ref_code > 40:
+                hint = ''
+                if abs(len(ref_code) - len(test_code)) < 20 and len(ref_code) > 40:
                     hint = f"For example, coordinates ({self.__polySeqModel[0]['auth_chain_id']}): {ref_code} vs topology: {test_code}. "
 
                 self.__f.append(f"[Sequence mismatch] Polymer sequence between the coordinate and {_a_mr_format_name} data does not match. {hint}"
                                 "Please verify the two sequences and re-upload the correct file(s) if required.")
 
             assi_ref_chain_ids = {}
             proc_test_chain_ids = []
             atom_nums = []
             delete_atom_nums = []
 
             def update_atom_num(seq_align, orphan):
                 ref_chain_id = seq_align['ref_chain_id']
                 test_chain_id = seq_align['test_chain_id']
 
+                if ref_chain_id in assi_ref_chain_ids or test_chain_id in proc_test_chain_ids:
+                    return
+
                 ps_cif = next(ps for ps in self.__polySeqModel if ps['auth_chain_id'] == ref_chain_id)
 
                 if ref_chain_id not in assi_ref_chain_ids:
                     assi_ref_chain_ids[ref_chain_id] = seq_align['length'] - seq_align['matched'] - seq_align['conflict']
                 else:
                     assi_ref_chain_ids[ref_chain_id] -= seq_align['matched'] + seq_align['conflict']
                 proc_test_chain_ids.append(test_chain_id)
@@ -575,15 +580,15 @@
                         test_seq_id = atomNum['seq_id']
 
                         if first_seq_id is None:
                             first_seq_id = test_seq_id
 
                         if test_seq_id in seq_align['test_seq_id']:
                             idx = seq_align['test_seq_id'].index(test_seq_id)
-                            if idx < len(seq_align['ref_auth_seq_id']):
+                            if 'ref_auth_seq_id' in seq_align and idx < len(seq_align['ref_auth_seq_id']):
                                 ref_seq_id = seq_align['ref_auth_seq_id'][idx]
                             elif offset is not None:
                                 ref_seq_id = test_seq_id + offset
                             else:
                                 continue
                         elif offset is not None:
                             ref_seq_id = test_seq_id + offset
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/GromacsPTReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/GromacsPTReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRLexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from IsdMRLexer.g4 by ANTLR 4.12.0
+# Generated from IsdMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -169,13 +169,13 @@
                   "NAME_CHAR", "ATM_NAME_CHAR", "ATM_TYPE_CHAR", "SIMPLE_NAME", 
                   "SPACE", "ENCLOSE_COMMENT", "SECTION_COMMENT", "LINE_COMMENT" ]
 
     grammarFileName = "IsdMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from IsdMRParser.g4 by ANTLR 4.12.0
+# Generated from IsdMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -52,15 +52,15 @@
     SPACE=8
     ENCLOSE_COMMENT=9
     SECTION_COMMENT=10
     LINE_COMMENT=11
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Isd_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/IsdMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/IsdMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/LexerErrorListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/LexerErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserErrorListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/ParserErrorListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/ParserListenerUtil.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/ParserListenerUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from RosettaMRLexer.g4 by ANTLR 4.12.0
+# Generated from RosettaMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -514,13 +514,13 @@
                   "Atom_pair_selection", "Atom_selection", "Any_name", "SPACE_CM", 
                   "RETURN_CM" ]
 
     grammarFileName = "RosettaMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from RosettaMRParser.g4 by ANTLR 4.12.0
+# Generated from RosettaMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -343,15 +343,15 @@
     Atom_selection=61
     Any_name=62
     SPACE_CM=63
     RETURN_CM=64
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Rosetta_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/RosettaMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/RosettaMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from SybylMRLexer.g4 by ANTLR 4.12.0
+# Generated from SybylMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -180,13 +180,13 @@
                   "ATM_TYPE_CHAR", "SIMPLE_NAME", "SPACE", "ENCLOSE_COMMENT", 
                   "SECTION_COMMENT", "LINE_COMMENT" ]
 
     grammarFileName = "SybylMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from SybylMRParser.g4 by ANTLR 4.12.0
+# Generated from SybylMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -61,15 +61,15 @@
     SPACE=11
     ENCLOSE_COMMENT=12
     SECTION_COMMENT=13
     LINE_COMMENT=14
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Sybyl_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/SybylMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/SybylMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRLexer.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from XplorMRLexer.g4 by ANTLR 4.12.0
+# Generated from XplorMRLexer.g4 by ANTLR 4.13.0
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
@@ -2462,13 +2462,13 @@
                   "Symbol_name_CF", "Simple_name_CF", "SPACE_CF", "COMMENT_CF", 
                   "Simple_name_LL", "SPACE_LL" ]
 
     grammarFileName = "XplorMRLexer.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParser.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated from XplorMRParser.g4 by ANTLR 4.12.0
+# Generated from XplorMRParser.g4 by ANTLR 4.13.0
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
@@ -1974,15 +1974,15 @@
     SPACE_CF=299
     COMMENT_CF=300
     Simple_name_LL=301
     SPACE_LL=302
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
 
     class Xplor_nih_mrContext(ParserRuleContext):
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRParserListener.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRParserListener.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/mr/XplorMRReader.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/mr/XplorMRReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb/utils/nmr/rci/RCI.py` & `wwpdb.utils.nmr-0.29/wwpdb/utils/nmr/rci/RCI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/PKG-INFO` & `wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.nmr
-Version: 0.28.dev1
+Version: 0.29
 Summary: wwPDB NMR utilities
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_nmr
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.nmr-0.28.dev1/wwpdb.utils.nmr.egg-info/SOURCES.txt` & `wwpdb.utils.nmr-0.29/wwpdb.utils.nmr.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -95,9 +95,13 @@
 wwpdb/utils/nmr/mr/SybylMRParserListener.py
 wwpdb/utils/nmr/mr/SybylMRReader.py
 wwpdb/utils/nmr/mr/XplorMRLexer.py
 wwpdb/utils/nmr/mr/XplorMRParser.py
 wwpdb/utils/nmr/mr/XplorMRParserListener.py
 wwpdb/utils/nmr/mr/XplorMRReader.py
 wwpdb/utils/nmr/mr/__init__.py
+wwpdb/utils/nmr/nmr-star_schema/category_order.pkl
+wwpdb/utils/nmr/nmr-star_schema/data_types.pkl
+wwpdb/utils/nmr/nmr-star_schema/schema.pkl
+wwpdb/utils/nmr/nmr-star_schema/schema_order.pkl
 wwpdb/utils/nmr/rci/RCI.py
 wwpdb/utils/nmr/rci/__init__.py
```

