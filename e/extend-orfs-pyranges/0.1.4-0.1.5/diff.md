# Comparing `tmp/extend_orfs_pyranges-0.1.4.tar.gz` & `tmp/extend_orfs_pyranges-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend_orfs_pyranges-0.1.4.tar", last modified: Wed Jul 26 14:29:52 2023, max compression
+gzip compressed data, was "extend_orfs_pyranges-0.1.5.tar", last modified: Fri Jul 28 14:00:24 2023, max compression
```

## Comparing `extend_orfs_pyranges-0.1.4.tar` & `extend_orfs_pyranges-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 14:29:21.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    23390 2023-07-26 13:18:05.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    25675 2023-07-26 14:27:22.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      458 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.5/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.5/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.5/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-28 13:56:32.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    25878 2023-07-28 13:56:21.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges/extend_orfs_pyranges.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 14:00:24.954932 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-28 14:00:24.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      405 2023-07-28 14:00:24.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-28 14:00:24.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-28 14:00:24.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-28 14:00:24.000000 extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/top_level.txt
```

### Comparing `extend_orfs_pyranges-0.1.4/PKG-INFO` & `extend_orfs_pyranges-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend_orfs_pyranges
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extend_orfs_pyranges-0.1.4/setup.cfg` & `extend_orfs_pyranges-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py` & `extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges/extend_orfs_pyranges.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #!/usr/bin/env python 
 
 # Imports 
 import pyranges as pr
-import pyranges.out as out ########################################################################################### I DID NOT FIND ANY OTHER WAY TO DO THIS
+import pyranges.out as out ########################################################################################### So far I did not find any other way to do this
 import csv 
 from pyfaidx import Fasta
 import pandas as pd
 import copy
 from easyterm import *
 
-# Definitions
+# Definitions #
+
 def extend_orfs(p = None, as_df = False, fasta_path = None, cds_id = None, 
                 starts = ['ATG'], stops = ['TAG', 'TGA', 'TAA'], 
                 default_full = False, direction = ['up', 'down'], 
-                chunk_size = 900, o = None): 
+                chunk_size = 900, o = None):
 
     """Extends PyRanges intervals to their next Start codon upstream 
        and/or to their next Stop codon downstream.
       
        Parameters
        ----------
 
        p : a PyRanges instance containing the intervals to be extended. 
 
        as_df : Wether provided input and desired output is a DataFrame
 
        fasta_path : location of the Fasta file from which the sequences
-           for the extensions.
+           for the extensions will be retrieved.
 
        cds_id : column on the PyRanges instance used to group rows as 
            transcripts. Default None.
 
        starts : list containing the nucleotide pattern to look for upstream.
            Default ['ATG']
 
@@ -39,15 +40,16 @@
 
        default_full : returns the whole sequence if the desired pattern is not
            found. Default False.
 
        direction : whether the extension should be upstream ('up'), downstream
            ('down') or both. Default ['up', 'down']
 
-       chunk_size : the size to be extended on each direction. Default 900.
+       chunk_size : the amount of nucleotides to be extended on each iteration. 
+           Default 900.
     """
 
     # Sanity Checks
     assert p is not None, "Please, provide the path to a Pyranges instance."
 
     assert fasta_path is not None, "Please, provide the path to a Fasta file."
 
@@ -55,21 +57,21 @@
         p_df = p.df
     else:
         p_df = p
 
     l_patterns = [starts, stops] #List of Patterns
     for pattern in l_patterns:
        msg = "Please, ensure all patterns have a length of 3 nt."
-       assert set([len(i) for i in pattern]) == {3},msg
-       
+       assert set([len(i) for i in pattern]) == {3},msg       
+
 
     # So all subsequent steps can be done with group_by:
     if cds_id is None: 
         cds_id = 'Custom_ID'
-        p_df[cds_id] = [i for i in range(len(p))] #Generates a New Column
+        p_df[cds_id] = [str(i) for i in range(len(p))] #Generates a New Column
 
 
     # Show a warning if some transcript lengths are not divisible by 3:
     p_df['length'] = p_df['End'] - p_df['Start'] 
 
     module_3 = p_df.groupby(by = cds_id)\
                        .apply(lambda x: sum(x['length']) % 3)
@@ -83,160 +85,174 @@
 
     p_df.drop(labels=['length'], inplace=True, axis=1) # Drop unnecessary column                                           
 
 
     # Load Sequence Data from a Fasta file
     fs = Fasta(fasta_path) #pyfaidx_fasta object, fasta sequences
 
+
     # Prepare Dictionary to Clip Out Bound Intervals afterwards
     #Dictionary of Chromosome lengths
     d_c = {k: len(fs[k]) for k in p.Chromosome.drop_duplicates()} 
 
+
     # This change is done to reduce artificially the number of chromosomes
     # so the subsequent steps are performed faster
     p_df["True_Chromosome"] = p_df["Chromosome"]
     p_df["Chromosome"] = [1 for i in range(len(p_df))]
     p_df["Initial_Start"] = p_df["Start"]
     p_df["Initial_End"] = p_df["End"]
      
     p = pr.PyRanges(p_df) 
-    
+
+    assert p.stranded , "ERROR the PyRanges must be stranded! Ensure that the strand column exists and all values are + or -"
+
     ######################  Extend Sequence Upstream ###########################
 
     if 'up' in direction or 'up' == direction:
 
        # The steps followed are:
                                # 1/ Extension
                                # 2/ Select Subsequence
                                # 3/ Adjust Subsequence to Chromosome Boundaries
+                               # 4/ Retrieve Subsequence from the fasta file
+                               # 5/ Parse Subsequence for the desired patterns
 
         # 1/ Extension
         pup_i = p.extend({"5":chunk_size}, group_by=cds_id) #Initial pup 
         pup_df = pd.DataFrame() # Empty Dataframe
         ic = 0 #Iteration Counter
 
+        # Set initial values for the search parameters
+        pup_i.up_start_pos = -1 # A sort of NA that does not modify  
+                                   # the column datatype
+        pup_i.Iteration_of_up_start_pos = ic
+        pup_i.Upstream_Stop_Codon_Found = False
+        
+        # Effective_Extension_Length of up_start_pos
+        pup_i.EEL_of_up_start_pos = -1
+
         while len(pup_i) > 0: #Iterate until it is empty
 
             # 2/ Select Subsequence
             # Only one row per cds_id. 
             # Without strand=True does not work for - Stand
             pup_i = pup_i.subsequence(0,chunk_size,by=cds_id,strand=True) ###################################### At some point, change this for spliced_subsequence
 
             # 3/ Adjust Subsequence to Chromosome Boundaries
             # Clip Out of Bounds Intervals
-            pup_i_df = mod_genome_bounds(pup_i, d_c) 
+            pup_i_df = mod_genome_bounds(pup_i, d_c)
 
             # As we keep those that are clipped, there may be effective extensions
             # smaller than chunk_size; we need to know the Effective_Extension_Length
             pup_i_df['Effective_Extension_Length'] = pup_i_df['End'] - pup_i_df['Start']
 
-            # Obtain the sequence corresponding to the extension
-            seqs = pup_i_df.apply(lambda x: mod_get_sequence(x, pyfaidx_fasta=fs), axis=1) 
-            ext5 = pd.DataFrame(pup_i_df[cds_id]) 
+            # 4/ Retrieve Subsequence from the fasta file
+            seqs = pup_i_df.apply(lambda x: mod_get_sequence(x, 
+                                            pyfaidx_fasta=fs), axis=1) 
+            ext5 = pup_i_df[[cds_id, 'Effective_Extension_Length',
+                                     'up_start_pos',
+                                     'Iteration_of_up_start_pos', 
+                                     'Upstream_Stop_Codon_Found',
+                                     'EEL_of_up_start_pos']].copy() 
             ext5['Sequence'] = seqs
 
-            # Get Index of Leftmost Start Codon (Downstream of Rightmost Stop Codon)
-            ext5["up_start_pos"] = ext5.Sequence.apply(lambda x: find_upstream_patterns(x, starts, stops)) 
-            ext5.drop(columns='Sequence',inplace=True) # Not to burden pup_i_df with Sequence 
+            # 5/ Parse Subsequence for the desired patterns
+            ext5 = ext5.groupby(cds_id, group_keys=False).apply(lambda x: 
+                                   find_upstream_patterns(x, starts, stops, ic))
+
+            ext5.drop(columns='Sequence',inplace=True)
+            pup_i_df.drop(columns=['up_start_pos',  'Iteration_of_up_start_pos',
+                                   'Upstream_Stop_Codon_Found', 
+                                    'EEL_of_up_start_pos',
+                                    'Effective_Extension_Length'], inplace=True)                                    
             pup_i_df = pd.merge(pup_i_df, ext5, on=cds_id) 
 
-            # Identify those rows that require further iteration:
-            # - They do not have the pattern (x['up_start_pos'] == -1)
-            # - Not yet at the chromsome edge (x['Effective_Extension_Length'] == chunk_size)
-            pup_i_df["Further_Iteration"] = pup_i_df.apply(lambda x: True if ((x['up_start_pos'] == -1) and 
-                                                           (x['Effective_Extension_Length'] == chunk_size)) else False, axis=1) 
-
-            # Compute Final Upstream Extension Size
-            # Extension_Size_Upstream = Effective_Extension_Length - up_start_pos + chunk_size * ic
-            # The last component is added so we can keep track on the number 
-            # of iterations
-            # If there is a -1 do not extend it (Extension_Size_Upstream = 0)
-            # unless default_full is requested
-
-            if default_full is True:
-                pup_i_df["Extension_Size_Upstream"] = pup_i_df.apply(lambda x: int(filler(x, 'up', d_c, chunk_size, ic)),axis=1)                                    
-            else:
-                pup_i_df["Extension_Size_Upstream"] = pup_i_df.apply(lambda x: 0 if (x['up_start_pos'] == -1) 
-                                                                     else x['Effective_Extension_Length'] - x['up_start_pos'] 
-                                                                     + chunk_size * ic, axis=1)
+            # Identify those transcripts that require further iteration
+            pup_i_df = pup_i_df.groupby(cds_id, 
+                               group_keys=False).apply(lambda x: 
+                               upstream_further_iteration_sorter(x, chunk_size)) 
+
+            # Compute Final UPTREAM Extension Size
+            pup_i_df = pup_i_df.groupby(cds_id, group_keys=False).apply(
+                lambda x: upstream_filler(x, default_full, d_c, chunk_size, ic)) 
 
             # Concatenate to pup_df those fulfilling the conditons 
             # and keep iterating with the rest 
-            ok_pup = pup_i_df[~pup_i_df["Further_Iteration"]] 
+            ok_pup = pup_i_df[~pup_i_df["Further_Iteration"]]
             ok_pup = ok_pup.drop(columns=['Effective_Extension_Length',
                                           'up_start_pos','Further_Iteration'])
             pup_df = pd.concat([pup_df, ok_pup])
-            pup_i_df = pup_i_df[pup_i_df["Further_Iteration"]]
+            pup_i_df = pup_i_df[pup_i_df["Further_Iteration"]] 
+            pup_i_df.reset_index(drop=True, inplace=True)
             pup_i_df = pup_i_df.drop(columns=['Effective_Extension_Length', 
-                                              'up_start_pos',
                                               'Extension_Size_Upstream',
                                               'Further_Iteration'])
 
             # 1/ Extension 
             pup_i = pr.PyRanges(pup_i_df) #So it is a PyRanges instance again
             pup_i = pup_i.extend({"5":chunk_size}, group_by=cds_id) 
             ic += 1 #Update Iteration Counter 
             
     else: # No extension upstream (i.e. the extension is 0)
         pup_df = p.df[cds_id].drop_duplicates().to_frame() 
-        pup_df['Extension_Size_Upstream'] =  [0 for i in range(len(pup_df))]
+        pup_df['Extension_Size_Upstream'] = [0 for i in range(len(pup_df))]
         
+
     ######################  Extend Sequence Downstream #########################
 
     if 'down' in direction or 'down' == direction:
 
         #The steps followed are:
                                # 1/ Extension
                                # 2/ Select Subsequence
                                # 3/ Adjust Subsequence to Chromosome Boundaries
+                               # 4/ Retrieve Subsequence from the fasta file
+                               # 5/ Parse Subsequence for the desired patterns
 
         # 1/ Extension
         pdp_i = p.extend({"3":chunk_size}, group_by=cds_id) #Initial pdp 
         pdp_df = pd.DataFrame() # Empty Dataframe
         ic = 0 #Iteration Counter
 
         while len(pdp_i) > 0: #Iterate until it is empty
-#        for i in range(1):
 
             # 2/ Select Subsequence
             # From -chunk_size nt before the end, up to the end. 
             # Without strand=True does not work for - Stand
             pdp_i = pdp_i.subsequence(-chunk_size,by=cds_id,strand=True) ###################################### At some point, change this for spliced_subsequence
 
             # 3/ Adjust Subsequence to Chromosome Boundaries
             # Clip Out of Bounds Intervals
-            # clip=True because we want to keep those elements 
-            # that have one end within the chromosome
             pdp_i_df = mod_genome_bounds(pdp_i, d_c) 
 
             #ext3 is a dataframe with ID and Sequence that must be merged to pup 
-#            pdp_i_df = pdp_i.df
             seqs = pdp_i_df.apply(lambda x: mod_get_sequence(x, pyfaidx_fasta=fs), axis=1)
             ext3 = pd.DataFrame(pdp_i_df[cds_id])
             ext3['Sequence'] = seqs
             
             # Get Index of Leftmost Stop Codon 
             ext3["down_stop_pos"] = ext3.Sequence.apply(lambda x: find_downstream_patterns(x, stops)) 
-            ext3 = ext3.drop(columns='Sequence') #Not to burden pdp_i with Sequence
+            ext3 = ext3.drop(columns='Sequence')
             pdp_i_df = pd.merge(pdp_i_df, ext3, on=cds_id)
         
-            # Identify those rows that require further iteration
+            # Identify those transcripts that require further iteration
             #These are those that have not found a pattern x['down_stop_pos'] == -1
             #And have not reached yet the chromsome edge (x['End'] - x['Start'] == chunk_size)
             pdp_i_df["Further_Iteration"] = pdp_i_df.apply(lambda x: True if ((x['down_stop_pos'] == -1) and 
                                                            (x['End'] - x['Start'] == chunk_size)) else False, axis=1) 
             # Compute Final DOWNSTREAM Extension Size
             # Extension_Size_Downstream = down_stop_pos + chunk_size * ic
             # The last component is added so we can keep track of the number
             # of iterations
             # If there is a -1 do not extend it (Extension_Size_Downstream = 0)
             # unless default_full is requested
 
             if default_full is True: 
-                pdp_i_df["Extension_Size_Downstream"] = pdp_i_df.apply(lambda x: int(filler(x, 'down', d_c, chunk_size, ic)),axis=1)  
+                pdp_i_df["Extension_Size_Downstream"] = pdp_i_df.apply(lambda x: int(downstream_filler(x, d_c, chunk_size, ic)),axis=1)  
 
             else:
                 pdp_i_df["Extension_Size_Downstream"] = pdp_i_df.apply(lambda x: 0 
                                                                        if (x['down_stop_pos'] == -1) else 
                                                                        x['down_stop_pos'] + chunk_size * ic,axis=1)    
 
             # To ensure there are no negative values      
@@ -262,24 +278,25 @@
         pdp_df = p.df[cds_id].drop_duplicates().to_frame()
         pdp_df['Extension_Size_Downstream'] = [0 for i in range(len(pdp_df))]
 
     ########################  Merge Both Extensions ############################
 
     p_df = p.df
 
-    # Remove Unnecessary Columns
+    # Drop Unnecessary Columns
     pup_df = pup_df.drop(columns=[i for i in list(pup_df.columns) if i != cds_id 
                                   and i != 'Extension_Size_Upstream']) 
     pdp_df = pdp_df.drop(columns=[i for i in list(pdp_df.columns) if i != cds_id
                                   and i != 'Extension_Size_Downstream']) 
 
     # Merge Extension Columns into the main Dataframe
     p_df = pd.merge(p_df, pup_df, on=cds_id)
     p_df = pd.merge(p_df, pdp_df, on=cds_id)
 
+    p_df.Strand=p_df.Strand.cat.remove_unused_categories() #debug MM 28/07/2023
     p = pr.PyRanges(p_df)
 
     p = mod_extend(p, group_by=cds_id)
 
     p_df = p.df
 
     p_df['Chromosome'] = p_df['True_Chromosome']
@@ -288,178 +305,249 @@
     if 'Custom_ID' in p_df:
         p_df.drop(labels=['Custom_ID'], inplace=True, axis=1)
 
     p_df.drop(labels=['Extension_Size_Upstream','Extension_Size_Downstream', 
                       'True_Chromosome', 'Initial_Start', 'Initial_End'], 
                       inplace=True, axis=1) 
 
+    # Output
     if o is not None:
         mod_to_gff3(p_df, path=o)
 
     if as_df is False:
         return pr.PyRanges(p_df)
     else:        
         return p_df
 
-def mod_genome_bounds(gr, chromsizes):
 
+def mod_genome_bounds(gr, chromsizes):
     """Modified version of Pyranges genomicfeatures.genome_bounds
     """
 
     gr = gr.df # apply for pyranges was problematic
 
     return gr.apply(lambda x: _outside_bounds_j(x, chromsizes),axis=1)
 
-def _outside_bounds_j(series, chromsizes):
 
+def _outside_bounds_j(series, chromsizes):
     """Modified version of Pyranges genomicfeatures._outside_bounds
        so it works with pandas DFs
     """
 
     size = int(chromsizes[series['True_Chromosome']])
 
     if series['End'] > size:
         series['End'] = size
 
     if series['Start'] < 0:
         series['Start'] = 0
  
     return series
 
-def mod_get_sequence(gr, path=None, pyfaidx_fasta=None):
 
+def mod_get_sequence(gr, path=None, pyfaidx_fasta=None):
     """Modified version of Pyranges get_fasta.get_sequence
        so it works with pandas DFs
     """
 
     if pyfaidx_fasta is None:
         if path is None:
             raise Exception('ERROR get_sequence : you must provide a fasta path'
                             ' or pyfaidx_fasta object')
         pyfaidx_fasta = pyfaidx.Fasta(path, read_ahead=int(1e5))
 
     seqs = []
     if gr['Strand'] is not None:  # if it is stranded
         _fasta = pyfaidx_fasta[gr['True_Chromosome']]
         if gr['Strand']=='-':
-            seqs.append( (-_fasta[gr['Start']:gr['End']]).seq ) # reverse complement
+            # Reverse complement
+            seqs.append( (-_fasta[gr['Start']:gr['End']]).seq )
         else:
              seqs.append( (_fasta[gr['Start']:gr['End']]).seq ) 
 
     else: # if it is not stranded
         _fasta = pyfaidx_fasta[gr['True_Chromosome']] 
         seqs.append( (_fasta[gr['Start']:gr['End']]).seq )   
 
     return pd.concat([pd.Series(s) for s in seqs]).reset_index(drop=True)
 
-def find_upstream_patterns(seq, starts, stops):
 
+def find_upstream_patterns(df, starts, stops, ic):                                                
     """Find Stop and Start Codons in ext5
     Output is the leftmost start codon downstream of the rightmost stop codon
-    Iterate backwards modifying t_i with the position of each start codon 
-    encountered. As one iterates backwards, when one finds the first stop codon 
-    it is sure it is the rightmost, so the last start codon encountered must be 
-    the leftmost to the right of that stop codon.
+    Iterate backwards modifying df["up_start_pos"] with the position of 
+    each subsequent start codon encountered. As one iterates backwards, when one
+    finds the first stop codon it is sure it is the rightmost, so the last start
+    codon encountered must be the leftmost to the right of that stop codon.
     If a stop codon is found before encountering any start codon, it returns
     the position of the stop codon.
-    If default_full is True, returns full sequence if pattern is not found.
+    'Iteration_of_up_start_pos' and 'EEL_of_up_start_pos' are used to keep track
+    of the leftmost Start Codon position through different iterations.
     """
 
-    start_i = -1 #Start Index
+    seq = df['Sequence'].values[0] 
 
-    for i in range(len(seq),0,-3): #-3 so iteration goes backwards 3 nt
+    # Effective_Extension_Length
+    eel = int(df['Effective_Extension_Length'].values)
+                                       
+    for i in range(len(seq),0,-3): #-3 so iteration goes backwards 3 nt 
         if seq[i-3:i] in starts: 
-            start_i = i - 3 #So extension includes the Start Codon
-
-        elif seq[i-3:i] in stops and start_i != -1:  
-            return start_i # A stop codon has been found. 
-                           # Return the last start position stored
-                           # before the stop codon
+            df["up_start_pos"] = i - 3 #So extension includes the Start Codon
+            df["Iteration_of_up_start_pos"] = ic
+            df["EEL_of_up_start_pos"] = eel
+
+        elif seq[i-3:i] in stops and df["up_start_pos"].values[0] != -1: 
+            df["Upstream_Stop_Codon_Found"] = True
+
+            return df # A stop codon has been found. 
+                      # Return the last start position stored
+                      # before the stop codon
 
         elif seq[i-3:i] in stops:
-            return i - 3 # A stop was found before any start codon. 
-                              # Return stop position
+            df["Upstream_Stop_Codon_Found"] = True
+            df["up_start_pos"] = i - 3 #So extension includes the Stop Codon
+            df["Iteration_of_up_start_pos"] = ic
+            df["EEL_of_up_start_pos"] = eel
 
-    return start_i #No match found. -1 so the resulting column can be numerical 
-              #It is a sort of NA that does not modify the column datatype
+            return df # A stop was found before any start codon. 
+                      # Return stop position
 
-def find_downstream_patterns(seq, stops):
+    return df 
+              
+
+def upstream_further_iteration_sorter(df, chunk_size): 
+    """Determines which transcripts have fulfilled the conditions and which ones
+       should be kept for the next iteration.
+       Keep iterating if no Stop codon has been found (even if a Start codon has
+       been found) and there is still room to iterate (eel == chunk_size).
+    """
+
+    # Effective_Extension_Length
+    eel = int(df['Effective_Extension_Length'].values)
+
+    # Upstream Stop Codon Found
+    uscf = bool(df['Upstream_Stop_Codon_Found'].values)
+
+    if uscf is False and eel == chunk_size: 
+        df["Further_Iteration"] = True
+
+    else:
+        df["Further_Iteration"] = False
+
+    return df
+
+
+def upstream_filler(df, default_full, dictionary, chunk_size, ic):
+    """
+    Compute the amount of nucleotides to extend upstream.
+    If a Start pattern and/or Stop pattern have been found, the extension is:
+
+             extension = chunk_size * iusp + eel_usp - usp
 
+    chunk_size * iusp recapitulate the extensions performed when the pattern was
+    found.
+    eel_usp is the largest extension possible when the pattern was found.
+    usp corrects the extension to the position where the pattern was found.
+    If no pattern is found and default_full is True, extend as much as possible
+    up to the edge of the chromosome.
+    If no pattern is found and default_full is False, no extension is performed.
+    """
+    # MM # input is a DataFrame
+    
+    # Upstream Start Position
+    usp = int(df['up_start_pos'].values)
+
+    # Effective_Extension_Length of Upstream Start Position
+    eel_usp = int(df['EEL_of_up_start_pos'].values)
+
+    # Iteration of Upstream Start Position
+    iusp = int(df['Iteration_of_up_start_pos'].values)
+
+    # Upstream Stop Codon Found
+    uscf = bool(df['Upstream_Stop_Codon_Found'].values)
+
+    strand = df['Strand'].values[0]
+
+    if usp != -1 or uscf is True:
+        extension = chunk_size * iusp + eel_usp - usp 
+
+    elif default_full is True:
+
+        if strand == '+':
+            extension = df['Initial_Start'] # Extension to the edge
+            extension = extension - extension % 3 # Extension corrected
+
+        elif strand == '-':
+            extension = dictionary[df['True_Chromosome'].values[0]] - df['Initial_End']
+            extension = extension - extension % 3
+
+    else:
+        extension = 0
+
+    df["Extension_Size_Upstream"] = extension
+
+    return df 
+
+
+def find_downstream_patterns(seq, stops):
     """Find leftmost stop codon in ext3.
        If default_full is True, returns full sequence if pattern is not found.
     """
     stop_i = -1 #Stop Index
 
     for i in range(0,len(seq),3): 
         if seq[i:i+3] in stops:
             stop_i = i + 3 #So extension includes the stop codon
             return stop_i
 
     return stop_i #No match found. -1 so the resulting column can be numerical 
               #It is a sort of NA that does not modify the column datatype
 
-def filler(p, stream, dictionary, chunk_size, ic): 
 
+def downstream_filler(df, dictionary, chunk_size, ic): 
     """
     If no pattern has been found for a given range (i.e. pattern_position == -1)
     returns the Extension corresponding to the Full Sequence or the longest one
     possible multiple of 3.
     If a pattern has been found, return the corresponding extension.
     """
+    # MM # input is a SERIES
 
-    if stream == 'up':
-        if p['up_start_pos'] == -1: 
-            if p['Strand'] == '+':
-                extension = p['Initial_Start'] # Extension to the edge
-                return extension - extension % 3 # Extension corrected
-
-            elif p['Strand'] == '-':
-                extension = dictionary[p['True_Chromosome']] - p['Initial_End']
-                return extension - extension % 3
-
-        else:
-           return ( p['Effective_Extension_Length'] - 
-                    p['up_start_pos'] + chunk_size * ic )
+    
+    if df['down_stop_pos'] == -1:
+        if df['Strand'] == '+': 
+            extension = dictionary[df['True_Chromosome']] - df['Initial_End']
+            return extension - extension % 3
+
+        elif df['Strand'] == '-':
+            extension = df['Initial_Start']
+            return extension - extension % 3 
 
-    elif stream == 'down':
-        if p['down_stop_pos'] == -1:
-            if p['Strand'] == '+': 
-                extension = dictionary[p['True_Chromosome']] - p['Initial_End']
-                return extension - extension % 3
-
-            elif p['Strand'] == '-':
-                 extension = p['Initial_Start']
-                 return extension - extension % 3 
+    else:
+        return ( df['down_stop_pos'] + chunk_size * ic )
 
-        else:
-            return ( p['down_stop_pos'] + chunk_size * ic )
 
 def mod_extend(p, group_by):
-
     """Modified version of PyRanges extend()
     The modifications allow for a specific 'chunk' extension for each group.
     """
 
-    try: 
-        kwargs = pr.pyranges_main.fill_kwargs({"strand": p.stranded})        
-    except:
-        # backwards compatibility: a submodule in pyranges changed its name
-        kwargs = pr.pyranges.fill_kwargs({"strand": p.stranded})
-        
+    kwargs = pr.pyranges_main.fill_kwargs({"strand": p.stranded})
           
     kwargs['group_by']=group_by
     prg = pr.PyRanges(
-                      pr.multithreaded.pyrange_apply_single(_extend_grp_j, p, **kwargs))            
+                      pr.multithreaded.pyrange_apply_single(_extend_grp_j, p, **kwargs))  
 
     return prg
 
-def _extend_grp_j(df, **kwargs):
 
+def _extend_grp_j(df, **kwargs):
     """Modified version of Pyranges multithreaded._extend_grp
     """
+
     df = df.copy()
     dtype = df.Start.dtype
     strand = df.Strand.iloc[0]    
     by = kwargs["group_by"]
     g=df.groupby(by)
  
     # So it only extends the first and last exons of each transcript:
@@ -474,17 +562,16 @@
          df.loc[minstarts_pos, "Start"] -= df.loc[minstarts_pos, "Extension_Size_Downstream"]
 
     df = df.astype({"Start": dtype, "End": dtype})
     assert (df.Start < df.End).all(), "Some intervals are negative or zero length after applying extend!"
 
     return df
 
-#def mod_to_gff3(df, path=None, compression="infer", map_cols=None):
-def mod_to_gff3(df, path=None, compression="infer"):
 
+def mod_to_gff3(df, path=None, compression="infer"):
     """Modified version of pyranges.out._to_gff3
        so it works with pandas DFs
     """
     
     mapping=out._gff3_columns.copy()
 
     df = out._gff3(df, mapping)
@@ -496,15 +583,16 @@
               header=False,
               compression=compression,
               mode=mode,
               sep="\t",
               quoting=csv.QUOTE_NONE)
     mode = "a"
 	
-#Execution 
+
+# Execution #
 
 if __name__ == "__main__": 
 
     def_opt={'p':'',
              'as_df':False,
              'clean_p':False, 
              'fasta_path':'',
@@ -535,31 +623,32 @@
                    no output file will be generated.
                 -h OR -help OR --help print this help and exit""" 
 
     opt=command_line_options(def_opt, help_msg)
 
     printerr('Current options are:',how='reverse,green')
     printerr(opt, how='yellow') 
-    if opt['clean_p']:
-        daf = pr.read_gff3(opt['p'], as_df=True) #gff3 to Dataframe
+ 
+    daf = pr.read_gff3(opt['p'], as_df=True) #gff3 to Dataframe
+    print('\nThis is the input in DataFrame format:\n',daf)
 
+    if opt['clean_p']:
         # Clean the DF
-        print('\nThis is the initial dataframe:\n',daf)
         daf = daf[['Chromosome', 'Start', 'End', 'Strand', 'ID', 'Parent', 
                'Feature']][daf.Feature=='CDS']
-        daf['Strand'] = daf['Strand'].astype("string") #So the Pyragnes object is correctly labelled as stranded
-
-    else:
-        pyr = opt['p'] ############################################################################################################################# THINK ABOUT THIS
+        
+# So the Pyragnes object is correctly labelled as stranded
+        daf['Strand'] = daf['Strand'].astype("string") 
+        print('\nThis is the input DataFrame cleaned:\n',daf)
 
     output = extend_orfs(p=daf, as_df=opt['as_df'] if opt['as_df'] else None, 
                          fasta_path=opt['fasta_path'],
                          cds_id=opt['cds_id'] if opt['cds_id'] else None,
                          starts=opt['starts'], stops=opt['stops'], 
                          default_full=opt['default_full'], 
                          direction=opt['direction'],
                          chunk_size=opt['chunk_size'],
                          o=opt['o'] if opt['o'] else None)
 
-    print('\nThis is the output:\n',output)
+    print('\nThis is the output in DataFrame format:\n',output)
```

### Comparing `extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/PKG-INFO` & `extend_orfs_pyranges-0.1.5/src/extend_orfs_pyranges.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend-orfs-pyranges
-Version: 0.1.4
+Version: 0.1.5
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

