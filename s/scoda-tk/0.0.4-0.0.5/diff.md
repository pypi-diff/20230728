# Comparing `tmp/scoda-tk-0.0.4.tar.gz` & `tmp/scoda-tk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.0.4.tar", last modified: Wed Jul 26 16:20:03 2023, max compression
+gzip compressed data, was "scoda-tk-0.0.5.tar", last modified: Fri Jul 28 08:50:08 2023, max compression
```

## Comparing `scoda-tk-0.0.4.tar` & `scoda-tk-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:20:03.940050 scoda-tk-0.0.4/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.4/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 16:20:03.940050 scoda-tk-0.0.4/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-26 16:19:47.000000 scoda-tk-0.0.4/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-26 16:20:03.940050 scoda-tk-0.0.4/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:20:03.876052 scoda-tk-0.0.4/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:20:03.880052 scoda-tk-0.0.4/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:20:03.924051 scoda-tk-0.0.4/src/scoda/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.4/src/scoda/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 15:27:40.000000 scoda-tk-0.0.4/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.4/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.4/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    51630 2023-07-26 16:19:37.000000 scoda-tk-0.0.4/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:20:03.940050 scoda-tk-0.0.4/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-26 16:20:03.000000 scoda-tk-0.0.4/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-28 08:50:08.142763 scoda-tk-0.0.5/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.5/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-28 08:50:08.142763 scoda-tk-0.0.5/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-28 08:48:44.000000 scoda-tk-0.0.5/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-28 08:50:08.142763 scoda-tk-0.0.5/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-28 08:50:07.414779 scoda-tk-0.0.5/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-28 08:50:07.462778 scoda-tk-0.0.5/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-28 08:50:07.982766 scoda-tk-0.0.5/src/scoda/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.5/src/scoda/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 17:14:30.000000 scoda-tk-0.0.5/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.5/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37051 2023-07-28 08:48:50.000000 scoda-tk-0.0.5/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.5/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    51630 2023-07-26 16:19:37.000000 scoda-tk-0.0.5/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-28 08:50:08.138763 scoda-tk-0.0.5/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-28 08:50:07.000000 scoda-tk-0.0.5/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.0.4/LICENSE` & `scoda-tk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/PKG-INFO` & `scoda-tk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.4/pyproject.toml` & `scoda-tk-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.0.4"
+version = "0.0.5"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.0.4/src/scoda/cpdb.py` & `scoda-tk-0.0.5/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/data/GTmap_hg19.csv` & `scoda-tk-0.0.5/src/scoda/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/data/GTmap_hg38.csv` & `scoda-tk-0.0.5/src/scoda/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/data/GTmap_mm10.csv` & `scoda-tk-0.0.5/src/scoda/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/deg.py` & `scoda-tk-0.0.5/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/deiso.py` & `scoda-tk-0.0.5/src/scoda/deiso.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/gsea.py` & `scoda-tk-0.0.5/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/hicat.py` & `scoda-tk-0.0.5/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/icnv.py` & `scoda-tk-0.0.5/src/scoda/icnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -923,16 +923,16 @@
                         window_size=100, n_jobs = n_cores)
 
         if pca_umap:
             print('PCA .. ', end = '')
             cnv.tl.pca(adata, svd_solver='arpack', n_comps = N_pca) 
             print('Finding neighbors .. ', end = '')
             cnv.pp.neighbors(adata, key_added = 'cnv_neighbors', n_neighbors=n_neighbors, n_pcs=N_pca)
-            print('Clustering .. ', end = '')
-            cnv.tl.leiden(adata, neighbors_key='cnv_neighbors', key_added=cluster_key, resolution = resolution)
+            # print('Clustering .. ', end = '')
+            # cnv.tl.leiden(adata, neighbors_key='cnv_neighbors', key_added=cluster_key, resolution = resolution)
             print('UMAP .. ', end = '')
             cnv.tl.umap(adata)
             
         print('Scoring .. ', end = '')
         cnv.tl.cnv_score(adata, groupby = cluster_key, key_added = 'cnv_score')
         print('done.')
 
@@ -967,27 +967,28 @@
     from sknetwork.clustering import Louvain
 except ImportError:
     print('WARNING: sknetwork not installed. Will used GMM for clustering.')
     CLUSTERING_AGO = 'gmm'
     SKNETWORK = False
 
     
-def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10):
+def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
+                   mode='distance', n_cores = 4):
     
     if clust_algo[:2] == 'gm':
         gmm = mixture.GaussianMixture(n_components = int(N_clusters), random_state = 0)
         cluster_label = gmm.fit_predict(np.array(X_pca))
         return cluster_label, gmm
     elif clust_algo[:2] == 'km':
         km = cluster.KMeans(n_clusters = int(N_clusters), random_state = 0)
         km.fit(X_pca)
         cluster_label = km.labels_
         return cluster_label, km
     else:
-        adj = kneighbors_graph(X_pca, int(N_neighbors), mode='connectivity', include_self=True)
+        adj = kneighbors_graph(X_pca, int(N_neighbors), mode=mode, include_self=True, n_jobs = n_cores)
         louvain = Louvain(resolution = resolution)
         if hasattr(louvain, 'fit_predict'):
             cluster_label = louvain.fit_predict(adj)        
         else:
             cluster_label = louvain.fit_transform(adj)        
         return cluster_label, louvain
     '''
@@ -999,44 +1000,56 @@
     '''
 
 def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                        dec_margin = 0.05, n_neighbors = 10, gcm = 0.05,
-                       plot_stat = False, use_ref = True, 
+                       plot_stat = False, use_ref = True, n_cores = 4,
                        suffix = '', Data = None):
     
     score_key = 'tumor_score' + suffix
     cluster_key = 'cnv_cluster' 
     ## Get X_pca for ref_type cells
 
     start_time = time.time()
+    start_time_a = start_time
     print('Running iCNV addon .. ', end = '', flush = True)
     
     if isinstance(X_cnv, pd.DataFrame):
         df = pd.DataFrame(index = X_cnv.index.values)
     else:
         df = pd.DataFrame()
         X_cnv = pd.DataFrame(X_cnv)
     
     N_components_pca = 15
     pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
 
     if not pca: 
         X_pca = pca_obj.fit_transform(X_cnv)
+        
+        etime = round(time.time() - start_time) 
+        print('P(%i) .. ' % etime, end = '', flush = True)
+        start_time = time.time()
+           
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
-    if clust:      
+    if clust is not None:      
         y_clust = list(clust)
+        cobj = None
     else:
         y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
-                                resolution = Clustering_resolution, N_neighbors = n_neighbors)
+                                       resolution = Clustering_resolution, N_neighbors = n_neighbors, 
+                                       n_cores = n_cores)
         
+        etime = round(time.time() - start_time) 
+        print('C(%i) .. ' % etime, end = '', flush = True)
+        start_time = time.time()
+    
     cnv_clust_lst = list(set(y_clust))
     df[cluster_key] = y_clust
         
     if use_ref:
         cnv_clust_lst.sort()
         b_inc = []
         for idx in cnv_clust_lst:
@@ -1062,18 +1075,14 @@
             df['tumor_cluster'+ suffix] = ''
             return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
         X_pca_sel = X_pca[b,:]
     else:
         X_pca_sel = X_pca
 
-
-    etime = round(time.time() - start_time) 
-    # print('C(%i).' % etime, end = '', flush = True)
-
     ## Get GMM model parameters
     gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
     gmm.fit(X_pca_sel)
     y_conf_gmm = -gmm.score_samples(X_pca)
     #'''
     y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
 
@@ -1083,26 +1092,26 @@
     ymax = yc[odr[n]]
     b = y_conf > ymax
     y_conf[b] = ymax
 
     df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))
 
     etime = round(time.time() - start_time) 
-    print('G(%i)' % etime, end = '', flush = True)
+    print('G(%i) .. ' % etime, end = '', flush = True)
+    start_time = time.time()
     
     ## Replace GMM scores with their cluster mean
     if ref_ind is not None:
         dft, params = get_cnv_threshold_useref( df, ref_ind, 
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
     else:
         dft, params = get_cnv_threshold_bimodal( df, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
                                         th_min = th_min, refp_min = refp_min, ucr = dec_margin,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
     
-    etime = round(time.time() - start_time) 
-    print(' .. done (%i) ' % etime) #, end = '', flush = True)
+    etime = round(time.time() - start_time_a) 
+    print('done (%i) ' % etime) #, end = '', flush = True)
     
-    return df, params
-
+    return df, params, cobj
```

### Comparing `scoda-tk-0.0.4/src/scoda/misc.py` & `scoda-tk-0.0.5/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda/viz.py` & `scoda-tk-0.0.5/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.4/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.0.5/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.4/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.0.5/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

