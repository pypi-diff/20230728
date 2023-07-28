# Comparing `tmp/rastermap-0.9.1.tar.gz` & `tmp/rastermap-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastermap-0.9.1.tar", last modified: Wed Jul 26 11:51:09 2023, max compression
+gzip compressed data, was "rastermap-0.9.2.tar", last modified: Fri Jul 28 18:48:46 2023, max compression
```

## Comparing `rastermap-0.9.1.tar` & `rastermap-0.9.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.039098 rastermap-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.027097 rastermap-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.031097 rastermap-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-26 11:50:54.000000 rastermap-0.9.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 11:50:54.000000 rastermap-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:50:54.000000 rastermap-0.9.1/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 11:50:54.000000 rastermap-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-26 11:51:09.039098 rastermap-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-07-26 11:50:54.000000 rastermap-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-26 11:50:54.000000 rastermap-0.9.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.031097 rastermap-0.9.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_largescale.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_singleneurons.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_widefield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_zebrafish.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig5.py
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/other_upsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/qrdqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/splitting.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/guiparts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:51:09.039098 rastermap-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-26 11:50:54.000000 rastermap-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.039098 rastermap-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 11:50:54.000000 rastermap-0.9.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-26 11:50:54.000000 rastermap-0.9.1/tests/test_rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 11:50:54.000000 rastermap-0.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.102566 rastermap-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.106566 rastermap-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 18:48:33.000000 rastermap-0.9.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 18:48:33.000000 rastermap-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 18:48:33.000000 rastermap-0.9.2/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-28 18:48:33.000000 rastermap-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-07-28 18:48:46.114566 rastermap-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-07-28 18:48:33.000000 rastermap-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-28 18:48:33.000000 rastermap-0.9.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 18:48:33.000000 rastermap-0.9.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.106566 rastermap-0.9.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_largescale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_singleneurons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_widefield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/rastermap_zebrafish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-07-28 18:48:33.000000 rastermap-0.9.2/notebooks/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.110566 rastermap-0.9.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-28 18:48:33.000000 rastermap-0.9.2/paper/splitting.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.110566 rastermap-0.9.2/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28224 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-28 18:48:33.000000 rastermap-0.9.2/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 18:48:46.000000 rastermap-0.9.2/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:48:46.114566 rastermap-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-28 18:48:33.000000 rastermap-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:48:46.114566 rastermap-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-28 18:48:33.000000 rastermap-0.9.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 18:48:33.000000 rastermap-0.9.2/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 18:48:33.000000 rastermap-0.9.2/tox.ini
```

### Comparing `rastermap-0.9.1/.gitignore` & `rastermap-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/LICENSE` & `rastermap-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/PKG-INFO` & `rastermap-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.1
+Version: 0.9.2
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -26,24 +26,26 @@
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovry algorithm for neural data. The algorithm was written by 
 Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
 
-Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab:
+Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
+**all demo data available [here](https://osf.io/xn4cm/)**
+
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
-<img src="https://www.suite2p.org/static/images/example_sorting_spont.png" width="600" alt="random sorting and rastermap sorting of spontaneous activity"/>
+<img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
 <img src="https://www.suite2p.org/static/images/rastermap_zebrafish.PNG" width="800" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
 
 # Installation
 
@@ -84,27 +86,27 @@
 
 If you have an older `rastermap` environment you can remove it with `conda env remove -n rastermap` before creating a new one.
 
 Note you will always have to run **conda activate rastermap** before you run rastermap. If you want to run jupyter notebooks in this environment, then also `pip install notebook`.
 
 ### Dependencies
 
-This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt5**, **PyQt5.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt5**, then make an Anaconda environment and try to install within it with `pip install PyQt5` or `conda install pyqt`.
+This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt6**, **PyQt6.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt6**, then make an Anaconda environment and try to install within it `conda install pyqt`. On **Ubuntu** you may need to `sudo apt-get install libegl1` to support PyQt6. Alternatively, you can use PyQt5 by running `pip uninstall PyQt6` and `pip install PyQt5`. If you already have a PyQt version installed, Rastermap will not install a new one.
 
 # Using rastermap
 
 ## GUI
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file. Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 ## In a notebook
@@ -240,16 +242,16 @@
 plt.scatter(xpos, ypos, cmap="gist_rainbow", c=y, s=1)
 ```
 
 Here is the list of all variables assigned from `fit`:
 
 * **embedding** : array, shape (n_samples, 1)
             embedding of each neuron / voxel
-* **isort** : sorting along first dimension of input matrix
-            use this to get neuron / voxel sorting
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
 * **igood** : array, shape (n_samples, 1)
     neurons/voxels which had non-zero activity and were used for sorting
 * **Usv** : array, shape (n_samples, n_PCs) 
     singular vectors U times singular values sv
 * **Vsv** : array, shape (n_features, n_PCs)
     singular vectors U times singular values sv
 * **U_nodes** : array, shape (n_clusters, n_PCs) 
@@ -263,13 +265,27 @@
 * **embedding_clust** : array, shape (n_samples, 1)
     assignment of each neuron/voxel to each cluster (before upsampling)
 * **X** : array, shape (n_samples, n_features)
     normalized data stored (if keep_norm_X is True)
 * **X_embedding** : array, shape (n_samples//bin_size, n_features)
     normalized data binned across samples (if compute_X_embedding is True)
 
+The output from the GUI and the command line is a file that ends with `_embedding.npy`. This file contains:
+* **filename**: str,
+    path to file that rastermap was run on
+* **save_path**: str,
+    folder with filename
+* **embedding** : array, shape (n_samples, 1)
+            embedding of each neuron / voxel
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
+* **user_clusters**: list, 
+    list of user drawn clusters in GUI
+* **ops**: dict,
+    dictionary of options used to run rastermap
+
 
 # License
 
 Copyright (C) 2023 Howard Hughes Medical Institute Janelia Research Campus, the labs of Carsen Stringer and Marius Pachitariu.
 
 **This code is licensed under GPL v3 (no redistribution without credit, and no redistribution in private repos, see the [license](LICENSE) for more details).**
```

### Comparing `rastermap-0.9.1/README.md` & `rastermap-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovry algorithm for neural data. The algorithm was written by 
 Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
 
-Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab:
+Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
+**all demo data available [here](https://osf.io/xn4cm/)**
+
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
-<img src="https://www.suite2p.org/static/images/example_sorting_spont.png" width="600" alt="random sorting and rastermap sorting of spontaneous activity"/>
+<img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
 <img src="https://www.suite2p.org/static/images/rastermap_zebrafish.PNG" width="800" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
 
 # Installation
 
@@ -70,27 +72,27 @@
 
 If you have an older `rastermap` environment you can remove it with `conda env remove -n rastermap` before creating a new one.
 
 Note you will always have to run **conda activate rastermap** before you run rastermap. If you want to run jupyter notebooks in this environment, then also `pip install notebook`.
 
 ### Dependencies
 
-This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt5**, **PyQt5.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt5**, then make an Anaconda environment and try to install within it with `pip install PyQt5` or `conda install pyqt`.
+This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt6**, **PyQt6.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt6**, then make an Anaconda environment and try to install within it `conda install pyqt`. On **Ubuntu** you may need to `sudo apt-get install libegl1` to support PyQt6. Alternatively, you can use PyQt5 by running `pip uninstall PyQt6` and `pip install PyQt5`. If you already have a PyQt version installed, Rastermap will not install a new one.
 
 # Using rastermap
 
 ## GUI
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file. Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 ## In a notebook
@@ -226,16 +228,16 @@
 plt.scatter(xpos, ypos, cmap="gist_rainbow", c=y, s=1)
 ```
 
 Here is the list of all variables assigned from `fit`:
 
 * **embedding** : array, shape (n_samples, 1)
             embedding of each neuron / voxel
-* **isort** : sorting along first dimension of input matrix
-            use this to get neuron / voxel sorting
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
 * **igood** : array, shape (n_samples, 1)
     neurons/voxels which had non-zero activity and were used for sorting
 * **Usv** : array, shape (n_samples, n_PCs) 
     singular vectors U times singular values sv
 * **Vsv** : array, shape (n_features, n_PCs)
     singular vectors U times singular values sv
 * **U_nodes** : array, shape (n_clusters, n_PCs) 
@@ -249,13 +251,27 @@
 * **embedding_clust** : array, shape (n_samples, 1)
     assignment of each neuron/voxel to each cluster (before upsampling)
 * **X** : array, shape (n_samples, n_features)
     normalized data stored (if keep_norm_X is True)
 * **X_embedding** : array, shape (n_samples//bin_size, n_features)
     normalized data binned across samples (if compute_X_embedding is True)
 
+The output from the GUI and the command line is a file that ends with `_embedding.npy`. This file contains:
+* **filename**: str,
+    path to file that rastermap was run on
+* **save_path**: str,
+    folder with filename
+* **embedding** : array, shape (n_samples, 1)
+            embedding of each neuron / voxel
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
+* **user_clusters**: list, 
+    list of user drawn clusters in GUI
+* **ops**: dict,
+    dictionary of options used to run rastermap
+
 
 # License
 
 Copyright (C) 2023 Howard Hughes Medical Institute Janelia Research Campus, the labs of Carsen Stringer and Marius Pachitariu.
 
-**This code is licensed under GPL v3 (no redistribution without credit, and no redistribution in private repos, see the [license](LICENSE) for more details).**
+**This code is licensed under GPL v3 (no redistribution without credit, and no redistribution in private repos, see the [license](LICENSE) for more details).**
```

### Comparing `rastermap-0.9.1/conftest.py` & `rastermap-0.9.2/conftest.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/notebooks/rastermap_largescale.ipynb` & `rastermap-0.9.2/notebooks/rastermap_largescale.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/notebooks/rastermap_singleneurons.ipynb` & `rastermap-0.9.2/notebooks/rastermap_singleneurons.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/notebooks/rastermap_widefield.ipynb` & `rastermap-0.9.2/notebooks/rastermap_widefield.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/notebooks/rastermap_zebrafish.ipynb` & `rastermap-0.9.2/notebooks/rastermap_zebrafish.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/notebooks/tutorial.ipynb` & `rastermap-0.9.2/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig1.ipynb` & `rastermap-0.9.2/paper/fig1.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig1.py` & `rastermap-0.9.2/paper/fig1.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig2.ipynb` & `rastermap-0.9.2/paper/fig2.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig2.py` & `rastermap-0.9.2/paper/fig2.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 def suppfig_random(root, save_figure=True):
     d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
     sn = d["sn"]
     sn_rand = d["sn_rand"]
     run = d["run"]
     itest = d["itest"]
 
-    fig = plt.figure(figsize=(14*0.75,8*0.75))
+    fig = plt.figure(figsize=(14,8))
 
     grid = plt.GridSpec(1,2, figure=fig, left=0.02, right=0.99, top=0.9, bottom=0.13, 
                         wspace = 0.15, hspace = 0.3)
     il = 0
 
     titles = ["random sorting", 
             "Rastermap sorting"]
```

### Comparing `rastermap-0.9.1/paper/fig3.ipynb` & `rastermap-0.9.2/paper/fig3.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig3.py` & `rastermap-0.9.2/paper/fig3.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig4.ipynb` & `rastermap-0.9.2/paper/fig4.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig4.py` & `rastermap-0.9.2/paper/fig4.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig5.ipynb` & `rastermap-0.9.2/paper/fig5.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig5.py` & `rastermap-0.9.2/paper/fig5.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig_splitting.py` & `rastermap-0.9.2/paper/fig_splitting.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/fig_utils.py` & `rastermap-0.9.2/paper/fig_utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/loaders.py` & `rastermap-0.9.2/paper/loaders.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/metrics.py` & `rastermap-0.9.2/paper/metrics.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/other_upsampling.py` & `rastermap-0.9.2/paper/other_upsampling.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/qrdqn.py` & `rastermap-0.9.2/paper/qrdqn.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/simulations.py` & `rastermap-0.9.2/paper/simulations.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/paper/splitting.ipynb` & `rastermap-0.9.2/paper/splitting.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/__main__.py` & `rastermap-0.9.2/rastermap/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                         help="processed data file 'embedding.npy'")
     parser.add_argument("--ops", default=[], type=str, help="options file 'ops.npy'")
     parser.add_argument("--iscell", default=[], type=str,
                         help="which cells to select for processing")
     args = parser.parse_args()
 
     if len(args.ops) > 0 and len(args.S) > 0:
-        X, Usv, Vsv = load_activity(args.S)
+        X, Usv, Vsv, xy = load_activity(args.S)
         ops = np.load(args.ops, allow_pickle=True).item()
         if len(args.iscell) > 0:
             iscell = np.load(args.iscell)
             if iscell.ndim > 1:
                 iscell = iscell[:, 0].astype("bool")
             else:
                 iscell = iscell.astype("bool")
@@ -58,22 +58,20 @@
                 train_time = np.zeros(X.shape[1], "bool")
                 train_time[np.arange(ops["start_time"], ops["end_time"]).astype(int)] = 1
                 X = X[:, train_time]
 
         model.fit(data=X, Usv=Usv, Vsv=Vsv)
 
         proc = {
-            "embedding": model.embedding,
+            "filename": args.S,
+            "save_path": os.path.split(args.S)[0],
             "isort": model.isort,
-            "Usv": model.Usv,
-            "Vsv": model.Vsv,
-            "sv": model.sv,
+            "embedding": model.embedding,
+            "user_clusters": None,
             "ops": ops,
-            "filename": args.S,
-            "train_time": train_time
         }
         basename, fname = os.path.split(args.S)
         fname = os.path.splitext(fname)[0]
         try:
             np.save(os.path.join(basename, f"{fname}_embedding.npy"), proc)
         except Exception as e:
             print("ERROR: no permission to write to data folder")
```

### Comparing `rastermap-0.9.1/rastermap/cluster.py` & `rastermap-0.9.2/rastermap/cluster.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/gui/colormaps.py` & `rastermap-0.9.2/rastermap/gui/colormaps.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/gui/gui.py` & `rastermap-0.9.2/rastermap/gui/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
 import sys, os
 import numpy as np
 import pyqtgraph as pg
-from PyQt5 import QtGui, QtCore
-from PyQt5 import QtWidgets as QtW
-from PyQt5.QtCore import QEvent
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QButtonGroup, QRadioButton, QStatusBar
+from qtpy import QtGui, QtCore
+from qtpy import QtWidgets as QtW
+from qtpy.QtCore import QEvent
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QButtonGroup, QRadioButton, QStatusBar
 from scipy.stats import zscore
 # patch for Qt 5.15 on macos >= 12
 os.environ["USE_MAC_SLIDER_PATCH"] = "1"
 from superqt import QRangeSlider  # noqa
 
 Horizontal = QtCore.Qt.Orientation.Horizontal
 Vertical = QtCore.Qt.Orientation.Vertical
@@ -141,15 +141,15 @@
         self.smooth.setFixedWidth(45)
         self.smooth.setAlignment(QtCore.Qt.AlignRight)
         self.smooth.returnPressed.connect(self.plot_activity)
 
         # Add slider for saturation
         self.sat = [30., 70.]
         self.sat_slider = QRangeSlider(Horizontal)
-        self.sat_slider.setRange(0., 200.)
+        self.sat_slider.setRange(0., 100.)
         self.sat_slider.setTickPosition(QtW.QSlider.TickPosition.TicksAbove)
         self.sat_slider.valueChanged.connect(self.sat_changed)
         self.sat_slider.setValue((self.sat[0], self.sat[1]))
         self.sat_slider.setFixedWidth(130)
         sat_label = QLabel("Saturation")
         sat_label.setStyleSheet("color: white;")
 
@@ -225,15 +225,14 @@
     def sat_changed(self):
         self.sat = self.sat_slider.value()
         self.img.setLevels([self.sat[0] / 100., self.sat[1] / 100.])
         self.imgROI.setLevels([self.sat[0] / 100., self.sat[1] / 100.])
         self.show()
 
     def reset(self):
-        self.run_embedding_button.setEnabled(False)
         self.p1.clear()
         self.p2.clear()
         self.p3.clear()
         self.p4.clear()
         self.p5.clear()
 
     def reset_variables(self):
@@ -286,19 +285,26 @@
         if event.mimeData().hasUrls():
             event.accept()
         else:
             event.ignore()
 
     def dropEvent(self, event):
         files = [u.toLocalFile() for u in event.mimeData().urls()]
-        ext = os.path.splitext(files[0])[-1]
-        if ext == ".npy" or ext == ".mat":
-            io.load_mat(self, name=files[0])
+        file = files[0]
+        file0, ext = os.path.splitext(file)
+        proc_file = file0 + "_embedding.npy"
+        if ext == ".npy" or ext == ".mat" or ext==".npz" or ext==".nwb":
+            if file[-14:] == "_embedding.npy":
+                io.load_proc(self, name=files[0])
+            elif os.path.exists(proc_file):
+                io.load_proc(self, name=proc_file)
+            else:
+                io.load_mat(self, name=files[0])
         else:
-            print("ERROR: must drag and drop *.npy or *.mat files")
+            print("ERROR: must drag and drop *.npy, *.npz, *.nwb or *.mat files")
 
     def plane_window(self):
         self.PlaneWindow = views.PlaneWindow(self)
         self.PlaneWindow.show()
 
     def update_status_bar(self, message, update_progress=False):
         if update_progress:
@@ -447,31 +453,33 @@
                 self.sp_smoothed = np.reshape(self.sp[self.sorting][:nn * N],
                                               (nn, N, -1)).mean(axis=1)
             else:
                 Usv_ds = np.reshape(self.Usv[self.sorting][:nn * N],
                                               (nn, N, -1)).mean(axis=1)
                 self.sp_smoothed = (Usv_ds / self.sv) @ self.Vsv.T
             self.sp_smoothed = zscore(self.sp_smoothed, axis=1)
-            self.sp_smoothed = np.maximum(-4, np.minimum(8, self.sp_smoothed)) + 4
-            self.sp_smoothed /= 12
+            self.sp_smoothed = np.maximum(-2, np.minimum(5, self.sp_smoothed)) + 2
+            self.sp_smoothed /= 7
         else:
-            self.sp_smoothed = self.sp.copy()
+            self.sp_smoothed = self.sp[self.sorting].copy()
         self.nsmooth = self.sp_smoothed.shape[0]
         yr0 = min(4, self.nsmooth // 4)
         ym = self.nsmooth // 2
         self.selected = slice(ym - yr0, ym + yr0)
         if len(self.cluster_rois) > 0:
             for i in range(len(self.cluster_rois)):
                 self.p2.removeItem(self.cluster_rois[i])
         self.cluster_rois, self.cluster_slices = [], []
         if self.user_clusters is None:
             self.add_cluster()
         self.get_behav_corr() if self.behav_data else None
         if self.neuron_pos is not None or self.behav_data is not None:
             self.update_scatter(init=True)
+        elif self.neuron_pos is None and self.scatter_comboBox.currentIndex()==0:
+            self.p5.clear()
         self.p2.show()
         self.p3.show()
 
     def add_cluster(self):
         roi_id = len(self.cluster_rois)
         self.cluster_rois.append(
             guiparts.ClusterROI(self, color=self.colors[roi_id],
@@ -547,15 +555,14 @@
     def update_scatter(self, init=False, roi_id=None):
         if init:
             self.p5.setLabel("left", "")
             self.p5.setLabel("bottom", "")
             self.p5.invertY(False)
         request = self.scatter_comboBox.currentIndex()
         if request > 0:
-
             self.plot_behav_corr(roi_id=roi_id, init=init)
         else:
             self.plot_neuron_pos(roi_id=roi_id, init=init)
 
     def get_behav_corr(self):
         beh = self.behav_data
         self.behav_corr_all = (self.sp_smoothed @ beh.T) / self.n_time
@@ -587,42 +594,47 @@
             if init:
                 self.p5.setLabel("left", "y position")
                 self.p5.setLabel("bottom", "x position")
         else:
             self.update_status_bar("ERROR: please upload neuron position data")
 
     def plot_scatter(self, x, y, roi_id=None, iplane=0):
+        subsample = max(1, int(len(x)/5000))
+        n_pts = len(x) // subsample
+        marker_size = int(3 * max(1, 800 / n_pts))
         if self.all_neurons_checkBox.isChecked() and roi_id is None:
             colors = colormaps.gist_ncar[np.linspace(
                 0, 254, len(x)).astype("int")][self.sorting]
-            brushes = [pg.mkBrush(color=c) for c in colors]
-            self.scatter_plots[iplane][0].setData(x, y, symbol="o", size=3,
+            brushes = [pg.mkBrush(color=c) for c in colors[::subsample]]
+            self.scatter_plots[iplane][0].setData(x[::subsample], y[::subsample], 
+                                                  symbol="o", size=marker_size,
                                                   brush=brushes,
                                                   hoverable=True)
             for i in range(1, nclust_max + 1):
                 self.scatter_plots[iplane][i].setData([], [])
         else:
             if roi_id is None:
                 self.scatter_plots[iplane][0].setData(
-                    x, y, symbol="o", size=3,
+                    x, y, symbol="o", size=marker_size,
                     brush=pg.mkBrush(color=(180, 180, 180)),
                     hoverable=True)
                 for roi_id in range(nclust_max):
                     if roi_id < len(self.cluster_rois):
                         selected = self.neurons_selected(self.cluster_slices[roi_id])
                         self.scatter_plots[iplane][roi_id + 1].setData(
-                            x[selected], y[selected], symbol="o", size=3,
+                            x[selected][::subsample], y[selected][::subsample], 
+                            symbol="o", size=marker_size,
                             brush=pg.mkBrush(color=self.colors[roi_id][:3]),
                             hoverable=True)
                     else:
                         self.scatter_plots[iplane][roi_id + 1].setData([], [])
             else:
                 selected = self.neurons_selected(self.cluster_slices[roi_id])
                 self.scatter_plots[iplane][roi_id + 1].setData(
-                    x[selected], y[selected], symbol="o", size=3,
+                    x[selected], y[selected], symbol="o", size=marker_size,
                     brush=pg.mkBrush(color=self.colors[roi_id][:3]), hoverable=True)
 
 
 def run(filename=None, proc=False):
     # Always start by initializing Qt (only once per application)
     app = QApplication(sys.argv)
     icon_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "logo.png")
```

### Comparing `rastermap-0.9.1/rastermap/gui/guiparts.py` & `rastermap-0.9.2/rastermap/gui/guiparts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
-from PyQt5 import QtGui, QtCore, QtWidgets
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QStyle, QStyleOptionSlider
+from qtpy import QtGui, QtCore, QtWidgets
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QStyle, QStyleOptionSlider
 import pyqtgraph as pg
 from pyqtgraph import functions as fn
 from pyqtgraph import Point
 import numpy as np
 
 
 class TimeROI(pg.LinearRegionItem):
```

### Comparing `rastermap-0.9.1/rastermap/gui/io.py` & `rastermap-0.9.2/rastermap/gui/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
 import os
 import numpy as np
-from PyQt5 import QtGui, QtCore, QtWidgets
-from PyQt5.QtWidgets import QFileDialog, QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox
+from qtpy import QtGui, QtCore, QtWidgets
+from qtpy.QtWidgets import QFileDialog, QInputDialog, QMainWindow, QApplication, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox
 import pyqtgraph as pg
 from scipy.stats import zscore
 import scipy.io as sio
 from . import guiparts
 from ..io import _load_iscell, _load_stat, load_activity
 
-def _load_activity_gui(parent, X, Usv, Vsv):
-        
+def _load_activity_gui(parent, X, Usv, Vsv, xy):
+    igood = None
     if X is not None:
         parent.update_status_bar(
             f"activity loaded: {X.shape[0]} samples by {X.shape[1]} timepoints")
         parent.update_status_bar(f"z-scoring activity matrix")
         parent.sp = zscore(X, axis=1)
         _load_iscell_stat(parent)
         del X
     elif Usv is not None:
         Usv = Usv.astype("float32")
         Vsv = Vsv.astype("float32")
         parent.sp = None
         parent.Usv = Usv 
         parent.Vsv = Vsv
         parent.sv = (Vsv**2).sum(axis=0)**0.5
+        igood = np.logical_and(~np.isnan(Usv[...,0]), 
+                                Usv.std(axis=-1) > 0)
         if parent.Usv.ndim==3:
-            igood = ~np.isnan(Usv[:,:,0])
             xy = np.array(np.nonzero(igood)).T
             parent.Usv = parent.Usv[xy[:,0], xy[:,1]]
             parent.neuron_pos = xy
             parent.update_status_bar(
                 f"using voxel positions for xy")
+        elif parent.Usv.ndim==2:
+            parent.Usv = parent.Usv[igood]
+            
         parent.update_status_bar(
             f"PCs of activity loaded: {Usv.shape[0]} samples by {Vsv.shape[0]} timepoints")
         
     else:
         raise ValueError("file missing keys / data")
 
+    parent.neuron_pos = xy if igood is None else xy[igood]
+
     parent.n_samples = (parent.sp.shape[0] if parent.sp is not None 
                         else parent.Usv.shape[0])
     parent.n_time = (parent.sp.shape[1] if parent.sp is not None 
                         else parent.Vsv.shape[0])
     parent.embedding = np.arange(0, parent.n_samples).astype(np.int64)[:, np.newaxis]
     parent.sorting = np.arange(0, parent.n_samples).astype(np.int64)
     _load_sp(parent)
@@ -51,31 +57,44 @@
 
 def load_mat(parent, name=None):
     """ load data matrix of neurons by time (*.npy or *.mat)
     
     Note: can only load mat files containing one key assigned to data matrix
     
     """
-    try:
-        if name is None:
-            name = QFileDialog.getOpenFileName(parent, "Open *.npy or *.mat",
-                                               filter="*.npy *.npz *.mat")
-            parent.fname = name[0]
-            parent.filebase = name[0]
-        else:
-            parent.fname = name
-            parent.filebase = name
-        
-        X, Usv, Vsv = load_activity(parent.fname)
-        _load_activity_gui(parent, X, Usv, Vsv)
-        
-    except Exception as e:
-        print(e)
-        X = None
-        return
+    if name is None:
+        name = QFileDialog.getOpenFileName(parent, "Open *.npy, *.npz, *.nwb or *.mat",
+                                            filter="*.npy *.npz *.mat *.nwb")
+        parent.fname = name[0]
+    else:
+        parent.fname = name
+    
+    X, Usv, Vsv, xy = load_activity(parent.fname)
+    _load_activity_gui(parent, X, Usv, Vsv, xy)
+
+#def load_dandiset(parent, name=None):
+#    try:
+#        import fsspec
+#        import dandi
+#        import pynwb
+#        import aiohttp
+#    except:
+#        raise ImportError("fsspec, dandi, pynwb, and/or aiohttp not installed, please 'pip install fsspec dandi pynwb aiohttp'")
+#    if name is None:
+#        name, ok = QInputDialog().getText(parent, "QInputDialog().getText()",
+#                                     "Dandiset ID:", QLineEdit.Normal)
+#        if not (name and ok):
+#            raise ValueError("not input by user")
+#    
+#    fs = fsspec.filesystem("http")
+
+    #X, Usv, Vsv, xy = load_activity(parent.fname)
+    #_load_activity_gui(parent, X, Usv, Vsv, xy)
+
+
 
 def _load_sp(parent):
     if parent.n_samples < 100:
         smooth = 1
     elif parent.n_samples < 1000:
         smooth = 5
     else:
@@ -344,38 +363,35 @@
             parent.fname = os.path.join(foldername, filename)
         else:
             print(f"ERROR: {parent.proc['filename']} not found")
             return
 
         isort = parent.proc["isort"]
         y = parent.proc["embedding"]
-        Usv = parent.proc["Usv"]
-        Vsv = parent.proc["Vsv"]
-        sv = parent.proc["sv"]
         ops = parent.proc["ops"]
         user_clusters = parent.proc.get("user_clusters", None)
         
-        X, Usv, Vsv = load_activity(parent.fname)
-        _load_activity_gui(parent, X, Usv, Vsv)
+        X, Usv, Vsv, xy = load_activity(parent.fname)
+        _load_activity_gui(parent, X, Usv, Vsv, xy)
         
     except Exception as e:
         raise e
 
     parent.startROI = False
     parent.posROI = np.zeros((2, 2))
 
     if user_clusters is not None:
         parent.smooth_bin = user_clusters[0]["binsize"]
         parent.smooth.setText(str(int(parent.smooth_bin)))
 
+    print(f"using sorting from {name}")
     parent.embedding = y
     parent.sorting = isort
     parent.Usv = Usv #if parent.Usv is None else parent.Usv
     parent.Vsv = Vsv #if parent.Vsv is None else parent.Vsv
-    parent.sv = sv #if parent.sv is None else parent.sv
     parent.ops = ops
     parent.user_clusters = user_clusters
 
     print(f"loaded:  {parent.proc['filename']}")
     _load_iscell_stat(parent)
     _load_sp(parent)
 
@@ -392,15 +408,15 @@
     try:
         if parent.embedding is not None:
             if parent.save_path is None:
                 folderName = QFileDialog.getExistingDirectory(
                     parent, "Choose save folder")
                 parent.save_path = folderName
             if parent.save_path:
-                filename = parent.fname.split("/")[-1]
+                filename = os.path.split(parent.fname)[-1]
                 filename, ext = os.path.splitext(filename)
                 savename = os.path.join(parent.save_path,
                                         ("%s_embedding.npy" % filename))
                 # save user clusters
                 if len(parent.cluster_slices) > 0:
                     user_clusters = []
                     for roi_id, cs in enumerate(parent.cluster_slices):
@@ -415,15 +431,14 @@
                 # Rastermap embedding parameters
                 ops = parent.ops
                 proc = {
                     "filename": parent.fname,
                     "save_path": parent.save_path,
                     "isort": parent.sorting,
                     "embedding": parent.embedding,
-                    "Usv": parent.U,
                     "user_clusters": user_clusters,
                     "ops": ops
                 }
 
                 np.save(savename, proc, allow_pickle=True)
                 print(f"processed file saved: {savename}")
         else:
```

### Comparing `rastermap-0.9.1/rastermap/gui/menus.py` & `rastermap-0.9.2/rastermap/gui/menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
-from PyQt5 import QtGui, QtCore, QtWidgets
-from PyQt5.QtWidgets import QAction
+from qtpy import QtGui, QtCore, QtWidgets
+from qtpy.QtWidgets import QAction
 import pyqtgraph as pg
 import numpy as np
 from . import io, run, gui, views
 
 
 # ------ MENU BAR -----------------
 def mainmenu(parent):
```

### Comparing `rastermap-0.9.1/rastermap/gui/run.py` & `rastermap-0.9.2/rastermap/gui/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
 import numpy as np
-import os
-from PyQt5 import QtGui, QtCore
-from PyQt5.QtWidgets import QMainWindow, QApplication, QSizePolicy, QDialog, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QButtonGroup, QRadioButton, QStatusBar, QTextEdit
+import os, sys
+from qtpy import QtGui, QtCore
+from qtpy.QtWidgets import QMainWindow, QApplication, QSizePolicy, QDialog, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QButtonGroup, QRadioButton, QStatusBar, QTextEdit
 from . import io
 
 
 ### custom QDialog which allows user to fill in ops and run rastermap
 class RunWindow(QDialog):
 
     def __init__(self, parent=None):
@@ -25,15 +25,15 @@
         )
         from rastermap import default_settings, settings_info, Rastermap
         # default ops
         self.ops = default_settings()
         info = settings_info()
         keys = [
             "n_clusters", "n_PCs", "time_lag_window", "locality", "grid_upsample",
-            "time_bin", "n_splits", "run_scaled_kmeans"
+            "time_bin", "n_splits"
         ]
         tooltips = [info[key] for key in keys]
         bigfont = QtGui.QFont("Arial", 10, QtGui.QFont.Bold)
         l = 0
         self.keylist = []
         self.editlist = []
         k = 0
@@ -59,42 +59,48 @@
         #self.runButton.setEnabled(False)
         self.textEdit = QTextEdit()
         self.textEdit.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.layout.addWidget(self.textEdit, 20, 0, 30, 14)
         self.process = QtCore.QProcess(self)
         self.process.readyReadStandardOutput.connect(self.stdout_write)
         self.process.readyReadStandardError.connect(self.stderr_write)
-        # disable the button when running the s2p process
+        # disable the button when running the rastermap process
         self.process.started.connect(self.started)
         self.process.finished.connect(lambda: self.finished(parent))
+        self.process.errorOccurred.connect(self.errored)
         # stop process
         self.stopButton = QPushButton("STOP")
         self.stopButton.setEnabled(False)
         self.layout.addWidget(self.stopButton, 19, 1, 1, 1)
         self.stopButton.clicked.connect(self.stop)
 
         self.show()
 
     def run_RMAP(self, parent):
-        del parent.sp
         self.finish = True
         self.error = False
         self.save_text()
-        np.save("rmap_ops.npy", self.ops)
+        ops_path = os.path.join(os.getcwd(), "rmap_ops.npy")
+        np.save(ops_path, self.ops)
         print("Running rastermap with command:")
-        cmd = f"python -u -W ignore -m rastermap --ops rmap_ops.npy --S {parent.filebase} "
+        cmd = f"-u -W ignore -m rastermap --ops {ops_path} --S {parent.fname}"
         if parent.file_iscell is not None:
             cmd += f"--iscell {parent.file_iscell}"
-        print(cmd)
-        self.process.start(cmd)
+        print("python " + cmd)
+        self.process.start(sys.executable, cmd.split(" "))
 
     def stop(self):
         self.finish = False
         self.process.kill()
 
+    def errored(self, error):
+        print("ERROR")
+        process = self.process
+        print("error: ", error, "-", " ".join([process.program()] + process.arguments()))
+
     def started(self):
         self.runButton.setEnabled(False)
         self.stopButton.setEnabled(True)
 
     def finished(self, parent):
         self.runButton.setEnabled(True)
         self.stopButton.setEnabled(False)
```

### Comparing `rastermap-0.9.1/rastermap/gui/views.py` & `rastermap-0.9.2/rastermap/gui/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
-from PyQt5 import QtGui, QtCore, QtWidgets
-from PyQt5.QtWidgets import QMainWindow, QApplication, QDialog, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QStyle, QStyleOptionSlider
+from qtpy import QtGui, QtCore, QtWidgets
+from qtpy.QtWidgets import QMainWindow, QApplication, QDialog, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QStyle, QStyleOptionSlider
 import pyqtgraph as pg
 from pyqtgraph import functions as fn
 from pyqtgraph import Point
 import numpy as np
 
 from . import colormaps
```

### Comparing `rastermap-0.9.1/rastermap/rastermap.py` & `rastermap-0.9.2/rastermap/rastermap.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         X : array, shape (n_samples, n_features)
             normalized data stored (if keep_norm_X is True)
         X_embedding : array, shape (n_samples//bin_size, n_features)
             normalized data binned across samples (if compute_X_embedding is True)
 
         """
         t0 = time.time()
-
+        self.n_clusters = None if self.n_clusters==0 else self.n_clusters
         
         # normalize data
         igood = ~np.isnan(data[:,0]) if data is not None else ~np.isnan(Usv[:,0])
         stdx = None
         normed = False
         if data is not None:
             if self.normalize:
```

### Comparing `rastermap-0.9.1/rastermap/sort.py` & `rastermap-0.9.2/rastermap/sort.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/svd.py` & `rastermap-0.9.2/rastermap/svd.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/upsample.py` & `rastermap-0.9.2/rastermap/upsample.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.1/rastermap/utils.py` & `rastermap-0.9.2/rastermap/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,24 +95,23 @@
         shutil.move(f.name, dst)
     finally:
         f.close()
         if os.path.exists(f.name):
             os.remove(f.name)
 
 def download_data(data_type="hippocampus"):
-    #url = f"http://www.suite2p.org/static/test_data/{data_type}_data.npz"
     if data_type=="widefield":
-        url = "https://osf.io/5d8q7"
+        url = "https://osf.io/5d8q7/download"
     elif data_type=="spont2":
-        url = "https://osf.io/8xg7n"
+        url = "https://osf.io/8xg7n/download"
     elif data_type=="hippocampus":
-        url = "https://osf.io/szmw6"
+        url = "https://osf.io/szmw6/download"
     elif data_type=="fish":
-        url = "https://osf.io/2w8pa"
+        url = "https://osf.io/2w8pa/download"
     ddir = Path.home().joinpath('.rastermap')
     ddir.mkdir(exist_ok=True)
     data_dir = ddir.joinpath('data')
     data_dir.mkdir(exist_ok=True)
     data_file = str(data_dir.joinpath(f"{data_type}_data.npz"))
     if not os.path.exists(data_file):
         download_url_to_file(url, data_file)
-    return data_file
+    return data_file
```

### Comparing `rastermap-0.9.1/rastermap.egg-info/PKG-INFO` & `rastermap-0.9.2/rastermap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.1
+Version: 0.9.2
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -26,24 +26,26 @@
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovry algorithm for neural data. The algorithm was written by 
 Carsen Stringer and Marius Pachitariu. To learn about Rastermap, read the [paper]() or watch the [talk](). For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation).
 
-Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab:
+Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
 * [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
 
+**all demo data available [here](https://osf.io/xn4cm/)**
+
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
-<img src="https://www.suite2p.org/static/images/example_sorting_spont.png" width="600" alt="random sorting and rastermap sorting of spontaneous activity"/>
+<img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
 Here is what the output looks like for a recording of wholebrain neural activity in a larval zebrafish from Chen, Mu, Hu, Kuan et al 2018 (dataset [here](https://figshare.com/articles/Whole-brain_light-sheet_imaging_data/7272617/1)). The plot on the left shows the sorted activity, and the right plot is the 2D positions of the neurons in the tissue, divided into 18 clusters according to their 1D position in the Rastermap embedding:
 
 <img src="https://www.suite2p.org/static/images/rastermap_zebrafish.PNG" width="800" alt="wholebrain neural activity from a zebrafish sorted by rastermap"/>
 
 # Installation
 
@@ -84,27 +86,27 @@
 
 If you have an older `rastermap` environment you can remove it with `conda env remove -n rastermap` before creating a new one.
 
 Note you will always have to run **conda activate rastermap** before you run rastermap. If you want to run jupyter notebooks in this environment, then also `pip install notebook`.
 
 ### Dependencies
 
-This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt5**, **PyQt5.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt5**, then make an Anaconda environment and try to install within it with `pip install PyQt5` or `conda install pyqt`.
+This package relies on the awesomeness of **numpy**, **scipy**, **numba**, **scikit-learn**, **PyQt6**, **PyQt6.sip** and **pyqtgraph**. You can pip install or conda install all of these packages. If having issues with **PyQt6**, then make an Anaconda environment and try to install within it `conda install pyqt`. On **Ubuntu** you may need to `sudo apt-get install libegl1` to support PyQt6. Alternatively, you can use PyQt5 by running `pip uninstall PyQt6` and `pip install PyQt5`. If you already have a PyQt version installed, Rastermap will not install a new one.
 
 # Using rastermap
 
 ## GUI
 
 The quickest way to start is to open the GUI from a command line terminal. You might need to open an anaconda prompt if you did not add anaconda to the path. Then run:
 
 ~~~sh
 python -m rastermap
 ~~~
 
-To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file. Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
+To start using the GUI, save your data into an npy file that is just a matrix that is neurons x timepoints. Then "File > Load data matrix" and choose this file (or drag and drop your file). Next click "Run > Run rastermap" and click run. See the parameters section to learn about the parameters.
 
 The GUI will start with a highlighted region that you can drag to visualize the average activity of neurons in a given part of the plot. To draw more regions, you right-click to start a region, then right-click to end it. The neurons' activity traces then show up on the botton of the GUI, and if the neuron positions are loaded, you will see them colored by the region color. You can delete a region by holding CTRL and clicking on it. You can save the ROIs you've drawn with the "Save > Save processed data" button. They will save along with the embedding so you can reload the file with the "Load processed data" option.
 
 NOTE: If you are using suite2p "spks.npy", then the GUI will automatically use the "iscell.npy" file in the same folder to subsample your recording with the chosen neurons, and will automatically load 
 the neuron positions from the "stat.npy" file.
 
 ## In a notebook
@@ -240,16 +242,16 @@
 plt.scatter(xpos, ypos, cmap="gist_rainbow", c=y, s=1)
 ```
 
 Here is the list of all variables assigned from `fit`:
 
 * **embedding** : array, shape (n_samples, 1)
             embedding of each neuron / voxel
-* **isort** : sorting along first dimension of input matrix
-            use this to get neuron / voxel sorting
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
 * **igood** : array, shape (n_samples, 1)
     neurons/voxels which had non-zero activity and were used for sorting
 * **Usv** : array, shape (n_samples, n_PCs) 
     singular vectors U times singular values sv
 * **Vsv** : array, shape (n_features, n_PCs)
     singular vectors U times singular values sv
 * **U_nodes** : array, shape (n_clusters, n_PCs) 
@@ -263,13 +265,27 @@
 * **embedding_clust** : array, shape (n_samples, 1)
     assignment of each neuron/voxel to each cluster (before upsampling)
 * **X** : array, shape (n_samples, n_features)
     normalized data stored (if keep_norm_X is True)
 * **X_embedding** : array, shape (n_samples//bin_size, n_features)
     normalized data binned across samples (if compute_X_embedding is True)
 
+The output from the GUI and the command line is a file that ends with `_embedding.npy`. This file contains:
+* **filename**: str,
+    path to file that rastermap was run on
+* **save_path**: str,
+    folder with filename
+* **embedding** : array, shape (n_samples, 1)
+            embedding of each neuron / voxel
+* **isort** : array, shape (n_samples,)
+    sorting along first dimension of input matrix - use this to get neuron / voxel sorting
+* **user_clusters**: list, 
+    list of user drawn clusters in GUI
+* **ops**: dict,
+    dictionary of options used to run rastermap
+
 
 # License
 
 Copyright (C) 2023 Howard Hughes Medical Institute Janelia Research Campus, the labs of Carsen Stringer and Marius Pachitariu.
 
 **This code is licensed under GPL v3 (no redistribution without credit, and no redistribution in private repos, see the [license](LICENSE) for more details).**
```

### Comparing `rastermap-0.9.1/rastermap.egg-info/SOURCES.txt` & `rastermap-0.9.2/rastermap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .style.yapf
 LICENSE
 README.md
+codecov.yml
 conftest.py
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
 notebooks/rastermap_largescale.ipynb
 notebooks/rastermap_singleneurons.ipynb
 notebooks/rastermap_widefield.ipynb
```

### Comparing `rastermap-0.9.1/tox.ini` & `rastermap-0.9.2/tox.ini`

 * *Files identical despite different names*

