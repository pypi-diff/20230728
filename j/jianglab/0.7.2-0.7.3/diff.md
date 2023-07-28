# Comparing `tmp/jianglab-0.7.2.tar.gz` & `tmp/jianglab-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.2.tar", last modified: Fri Jul 28 00:10:55 2023, max compression
+gzip compressed data, was "jianglab-0.7.3.tar", last modified: Fri Jul 28 00:13:06 2023, max compression
```

## Comparing `jianglab-0.7.2.tar` & `jianglab-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:10:55.336378 jianglab-0.7.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:10:55.336018 jianglab-0.7.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:10:55.332111 jianglab-0.7.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    48865 2023-07-28 00:09:07.000000 jianglab-0.7.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:10:55.335361 jianglab-0.7.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:10:55.000000 jianglab-0.7.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-28 00:10:55.000000 jianglab-0.7.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-28 00:10:55.000000 jianglab-0.7.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      158 2023-07-28 00:10:55.000000 jianglab-0.7.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-28 00:10:55.000000 jianglab-0.7.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-28 00:10:55.336513 jianglab-0.7.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1141 2023-07-27 23:58:55.000000 jianglab-0.7.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.458008 jianglab-0.7.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:13:06.457648 jianglab-0.7.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.453956 jianglab-0.7.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    48868 2023-07-28 00:12:46.000000 jianglab-0.7.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-28 00:13:06.456848 jianglab-0.7.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      158 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-28 00:13:06.000000 jianglab-0.7.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-28 00:13:06.458137 jianglab-0.7.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1141 2023-07-28 00:12:53.000000 jianglab-0.7.3/setup.py
```

### Comparing `jianglab-0.7.2/PKG-INFO` & `jianglab-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.2
+Version: 0.7.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.2/README.md` & `jianglab-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.2/jianglab/common_functions.py` & `jianglab-0.7.3/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,15 +1152,15 @@
 
 
 
 def plot_elbow_figure(data, max_cluster_num = 11):
     clusters = []
 
     for i in range(1, max_cluster_num):
-        km = KMeans(n_clusters=i).fit(X)
+        km = KMeans(n_clusters=i).fit(data)
         clusters.append(km.inertia_)
         
     fig, ax = plt.subplots(figsize=(12, 8))
     sns.lineplot(x=list(range(1, max_cluster_num)), y=clusters, ax=ax)
     ax.set_title('Searching for Elbow')
     ax.set_xlabel('Clusters')
     ax.set_ylabel('Inertia')
```

### Comparing `jianglab-0.7.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.3/jianglab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.2
+Version: 0.7.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.2/setup.py` & `jianglab-0.7.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.2',
+    version='0.7.3',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

