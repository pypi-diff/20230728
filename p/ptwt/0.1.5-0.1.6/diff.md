# Comparing `tmp/ptwt-0.1.5.tar.gz` & `tmp/ptwt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptwt-0.1.5.tar", last modified: Tue Apr 25 08:28:29 2023, max compression
+gzip compressed data, was "ptwt-0.1.6.tar", last modified: Fri Jul 28 19:31:44 2023, max compression
```

## Comparing `ptwt-0.1.5.tar` & `ptwt-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.288498 ptwt-0.1.5/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    14013 2022-06-08 12:13:31.000000 ptwt-0.1.5/LICENSE
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8791 2023-04-25 08:28:29.288498 ptwt-0.1.5/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7653 2023-04-25 08:12:55.000000 ptwt-0.1.5/README.rst
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1350 2023-04-25 08:28:29.288498 ptwt-0.1.5/setup.cfg
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2022-06-08 12:13:31.000000 ptwt-0.1.5/setup.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/ptwt/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      603 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/__init__.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1989 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/_util.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    11257 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/continuous_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    11636 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     9066 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform_2.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     9342 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform_3.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    22734 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    32359 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform_2.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    16716 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform_3.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    21343 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/packets.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    13612 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/separable_conv_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    20237 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/sparse_math.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      986 2023-04-25 08:20:47.000000 ptwt-0.1.5/src/ptwt/version.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    10275 2022-06-08 12:13:31.000000 ptwt-0.1.5/src/ptwt/wavelets_learnable.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/ptwt.egg-info/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8791 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      875 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/SOURCES.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/dependency_links.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)       63 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/requires.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        5 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/top_level.txt
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/tests/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8187 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_convolution_fwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     2637 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_convolution_fwt_3.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     3961 2022-10-24 11:21:37.000000 ptwt-0.1.5/tests/test_cwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     6477 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_jit.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7206 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8091 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt_2.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     3090 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt_3.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    11918 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_packets.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     5702 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_separable_conv_fwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    10862 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_sparse_math.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1048 2022-06-08 12:13:31.000000 ptwt-0.1.5/tests/test_util.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1316 2022-06-08 12:13:31.000000 ptwt-0.1.5/tests/test_wavelet.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-07-28 19:31:44.653421 ptwt-0.1.6/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    14013 2021-10-14 22:41:05.000000 ptwt-0.1.6/LICENSE
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9027 2023-07-28 19:31:44.653421 ptwt-0.1.6/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     7855 2023-07-28 19:30:57.000000 ptwt-0.1.6/README.rst
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1384 2023-07-28 19:31:44.653421 ptwt-0.1.6/setup.cfg
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2021-12-03 11:23:43.000000 ptwt-0.1.6/setup.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-07-28 19:31:44.649422 ptwt-0.1.6/src/
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-07-28 19:31:44.649422 ptwt-0.1.6/src/ptwt/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      603 2023-07-28 18:34:35.000000 ptwt-0.1.6/src/ptwt/__init__.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1830 2023-07-28 19:08:19.000000 ptwt-0.1.6/src/ptwt/_stationary_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3966 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/_util.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11256 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/continuous_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    13735 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/conv_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11980 2023-07-28 19:06:55.000000 ptwt-0.1.6/src/ptwt/conv_transform_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9691 2023-07-28 19:24:43.000000 ptwt-0.1.6/src/ptwt/conv_transform_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    23726 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/matmul_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    33097 2023-07-28 19:06:53.000000 ptwt-0.1.6/src/ptwt/matmul_transform_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    16716 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/matmul_transform_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    21534 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/packets.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11930 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/separable_conv_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    20246 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/sparse_math.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      989 2023-07-28 19:25:59.000000 ptwt-0.1.6/src/ptwt/version.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    10309 2023-07-28 18:54:30.000000 ptwt-0.1.6/src/ptwt/wavelets_learnable.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-07-28 19:31:44.649422 ptwt-0.1.6/src/ptwt.egg-info/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9027 2023-07-28 19:31:44.000000 ptwt-0.1.6/src/ptwt.egg-info/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      927 2023-07-28 19:31:44.000000 ptwt-0.1.6/src/ptwt.egg-info/SOURCES.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2023-07-28 19:31:44.000000 ptwt-0.1.6/src/ptwt.egg-info/dependency_links.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)       63 2023-07-28 19:31:44.000000 ptwt-0.1.6/src/ptwt.egg-info/requires.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        5 2023-07-28 19:31:44.000000 ptwt-0.1.6/src/ptwt.egg-info/top_level.txt
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-07-28 19:31:44.653421 ptwt-0.1.6/tests/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9662 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_convolution_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     2661 2023-07-28 19:24:28.000000 ptwt-0.1.6/tests/test_convolution_fwt_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3961 2022-10-26 20:00:30.000000 ptwt-0.1.6/tests/test_cwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     6481 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_jit.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8196 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_matrix_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8893 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_matrix_fwt_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3090 2023-05-02 20:00:25.000000 ptwt-0.1.6/tests/test_matrix_fwt_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11849 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_packets.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     4639 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_separable_conv_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    10862 2023-07-28 18:34:35.000000 ptwt-0.1.6/tests/test_sparse_math.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      818 2023-07-28 19:08:31.000000 ptwt-0.1.6/tests/test_swt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     2534 2023-07-28 18:54:30.000000 ptwt-0.1.6/tests/test_util.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1316 2022-04-01 17:54:07.000000 ptwt-0.1.6/tests/test_wavelet.py
```

### Comparing `ptwt-0.1.5/LICENSE` & `ptwt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.5/PKG-INFO` & `ptwt-0.1.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,9 @@
-Metadata-Version: 2.1
-Name: ptwt
-Version: 0.1.5
-Summary: Differentiable and gpu enabled fast wavelet transforms in PyTorch
-Home-page: https://github.com/v0lta/PyTorch-Wavelet-Toolbox
-Download-URL: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
-Author: Moritz Wolter
-Author-email: moritz@wolter.tech
-Maintainer: Moritz Wolter
-Maintainer-email: moritz@wolter.tech
-License: EUPL-1.2
-Project-URL: Bug Tracker, https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
-Project-URL: Source Code, https://github.com/v0lta/PyTorch-Wavelet-Toolbox
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ********************************
-Pytorch Wavelet Toolbox (`ptwt`)
+Pytorch Wavelet Toolbox (`ptwt`) 
 ********************************
 
 .. image:: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml/badge.svg 
     :target: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml
     :alt: GitHub Actions
 
 .. image:: https://readthedocs.org/projects/pytorch-wavelet-toolbox/badge/?version=latest
@@ -52,30 +26,28 @@
     :target: https://github.com/psf/black
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
-
-
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
 - ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
 - ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
 - 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
 - ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_. In addition to boundary wavelets, we provide GPU and gradient support via a PyTorch backend.
 Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
@@ -112,23 +84,23 @@
   # invert the fwt.
   print(ptwt.waverec(ptwt.wavedec(data_torch, wavelet, mode='zero'),
                      wavelet))
 
 
 The functions ``wavedec`` and ``waverec`` compute the 1d-fwt and its inverse.
 Internally both rely on ``conv1d``, and its transposed counterpart ``conv_transpose1d``
-from the ``torch.nn.functional`` module. This toolbox supports discrete wavelets
-see also ``pywt.wavelist(kind='discrete')``. I have tested
-Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, which are usually a good starting point. 
+from the ``torch.nn.functional`` module. This toolbox also supports discrete wavelets
+see ``pywt.wavelist(kind='discrete')``. I have tested
+Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, are usually a good starting point. 
 
 **Two-dimensional transform**
 
 Analog to the 1d-case ``wavedec2`` and ``waverec2`` rely on 
 ``conv2d``, and its transposed counterpart ``conv_transpose2d``.
-To test an example run:
+To test an example, run:
 
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
@@ -138,14 +110,18 @@
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
 
+**Speed tests**
+
+Speed tests comparing our tools to related libraries are `available <https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/speed_tests/>`_.
+
 
 **Boundary Wavelets with Sparse-Matrices**
 
 In addition to convolution and padding approaches,
 sparse-matrix-based code with boundary wavelet support is available.
 In contrast to padding, boundary wavelets do not add extra pixels at 
 the edges.
@@ -205,29 +181,29 @@
 
 
 to run all existing tests.
 
 Citation
 """"""""
 
-If you use this work in a scientific context please cite:
+If you use this work in a scientific context, please cite the following:
 
 .. code-block::
 
   @phdthesis{handle:20.500.11811/9245,
     urn: https://nbn-resolving.org/urn:nbn:de:hbz:5-63361,
     author = {{Moritz Wolter}},
     title = {Frequency Domain Methods in Recurrent Neural Networks for Sequential Data Processing},
     school = {Rheinische Friedrich-Wilhelms-Universität Bonn},
     year = 2021,
     month = jul,
     url = {https://hdl.handle.net/20.500.11811/9245}
   }
 
-If you use the boundary wavelet support please additionally cite:
+If you use the boundary wavelet support, please additionally cite:
 
 .. code-block::
 
   @thesis{Blanke2021,
     author = {Felix Blanke},
     title = {{Randbehandlung bei Wavelets für Faltungsnetzwerke}},
     type = {Bachelor's Thesis},
```

### Comparing `ptwt-0.1.5/README.rst` & `ptwt-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,35 @@
+Metadata-Version: 2.1
+Name: ptwt
+Version: 0.1.6
+Summary: Differentiable and gpu enabled fast wavelet transforms in PyTorch
+Home-page: https://github.com/v0lta/PyTorch-Wavelet-Toolbox
+Download-URL: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
+Author: Moritz Wolter and Felix Blanke
+Author-email: moritz@wolter.tech
+Maintainer: Moritz Wolter and Felix Blanke
+Maintainer-email: moritz@wolter.tech
+License: EUPL-1.2
+Project-URL: Bug Tracker, https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
+Project-URL: Source Code, https://github.com/v0lta/PyTorch-Wavelet-Toolbox
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ********************************
-Pytorch Wavelet Toolbox (`ptwt`)
+Pytorch Wavelet Toolbox (`ptwt`) 
 ********************************
 
 .. image:: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml/badge.svg 
     :target: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml
     :alt: GitHub Actions
 
 .. image:: https://readthedocs.org/projects/pytorch-wavelet-toolbox/badge/?version=latest
@@ -26,30 +52,28 @@
     :target: https://github.com/psf/black
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
-
-
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
 - ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
 - ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
 - 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
 - ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_. In addition to boundary wavelets, we provide GPU and gradient support via a PyTorch backend.
 Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
@@ -86,23 +110,23 @@
   # invert the fwt.
   print(ptwt.waverec(ptwt.wavedec(data_torch, wavelet, mode='zero'),
                      wavelet))
 
 
 The functions ``wavedec`` and ``waverec`` compute the 1d-fwt and its inverse.
 Internally both rely on ``conv1d``, and its transposed counterpart ``conv_transpose1d``
-from the ``torch.nn.functional`` module. This toolbox supports discrete wavelets
-see also ``pywt.wavelist(kind='discrete')``. I have tested
-Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, which are usually a good starting point. 
+from the ``torch.nn.functional`` module. This toolbox also supports discrete wavelets
+see ``pywt.wavelist(kind='discrete')``. I have tested
+Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, are usually a good starting point. 
 
 **Two-dimensional transform**
 
 Analog to the 1d-case ``wavedec2`` and ``waverec2`` rely on 
 ``conv2d``, and its transposed counterpart ``conv_transpose2d``.
-To test an example run:
+To test an example, run:
 
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
@@ -112,14 +136,18 @@
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
 
+**Speed tests**
+
+Speed tests comparing our tools to related libraries are `available <https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/speed_tests/>`_.
+
 
 **Boundary Wavelets with Sparse-Matrices**
 
 In addition to convolution and padding approaches,
 sparse-matrix-based code with boundary wavelet support is available.
 In contrast to padding, boundary wavelets do not add extra pixels at 
 the edges.
@@ -179,29 +207,29 @@
 
 
 to run all existing tests.
 
 Citation
 """"""""
 
-If you use this work in a scientific context please cite:
+If you use this work in a scientific context, please cite the following:
 
 .. code-block::
 
   @phdthesis{handle:20.500.11811/9245,
     urn: https://nbn-resolving.org/urn:nbn:de:hbz:5-63361,
     author = {{Moritz Wolter}},
     title = {Frequency Domain Methods in Recurrent Neural Networks for Sequential Data Processing},
     school = {Rheinische Friedrich-Wilhelms-Universität Bonn},
     year = 2021,
     month = jul,
     url = {https://hdl.handle.net/20.500.11811/9245}
   }
 
-If you use the boundary wavelet support please additionally cite:
+If you use the boundary wavelet support, please additionally cite:
 
 .. code-block::
 
   @thesis{Blanke2021,
     author = {Felix Blanke},
     title = {{Randbehandlung bei Wavelets für Faltungsnetzwerke}},
     type = {Bachelor's Thesis},
```

### Comparing `ptwt-0.1.5/setup.cfg` & `ptwt-0.1.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = ptwt
-version = 0.1.5
+version = 0.1.6
 description = Differentiable and gpu enabled fast wavelet transforms in PyTorch
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 download_url = https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
 project_urls = 
 	Bug Tracker = https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
 	Source Code = https://github.com/v0lta/PyTorch-Wavelet-Toolbox
-author = Moritz Wolter
+author = Moritz Wolter and Felix Blanke
 author_email = moritz@wolter.tech
-maintainer = Moritz Wolter
+maintainer = Moritz Wolter and Felix Blanke
 maintainer_email = moritz@wolter.tech
 license = EUPL-1.2
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 	Development Status :: 4 - Beta
 	Environment :: Console
```

### Comparing `ptwt-0.1.5/src/ptwt/__init__.py` & `ptwt-0.1.6/src/ptwt/__init__.py`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.5/src/ptwt/continuous_transform.py` & `ptwt-0.1.6/src/ptwt/continuous_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def cwt(
     data: torch.Tensor,
     scales: Union[np.ndarray, torch.Tensor],  # type: ignore
     wavelet: Union[ContinuousWavelet, str],
     sampling_period: float = 1.0,
 ) -> Tuple[torch.Tensor, np.ndarray]:  # type: ignore
-    """Compute the single dimensional continuous wavelet transform.
+    """Compute the single-dimensional continuous wavelet transform.
 
     This function is a PyTorch port of pywt.cwt as found at:
     https://github.com/PyWavelets/pywt/blob/master/pywt/_cwt.py
 
     Args:
         data (torch.Tensor): The input tensor of shape [batch_size, time].
         scales (torch.Tensor or np.array):
@@ -162,15 +162,15 @@
 
     Ported from:
     https://github.com/PyWavelets/pywt/blob/cef09e7f419aaf4c39b9f778bdc2d54b32fd7337/pywt/_functions.py#L60
 
 
     Parameters
     ----------
-    wavelet : Wavelet instance or str
+    wavelet: Wavelet instance or str
         Wavelet to integrate.  If a string, should be the name of a wavelet.
     precision : int, optional
         Precision that will be used for wavelet function
         approximation computed with the wavefun(level=precision)
         Wavelet's method (default: 8).
     Returns
     -------
```

### Comparing `ptwt-0.1.5/src/ptwt/conv_transform.py` & `ptwt-0.1.6/src/ptwt/conv_transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 """
 # Created by moritz wolter, 14.04.20
 from typing import List, Optional, Sequence, Tuple, Union
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported
+from ._util import (
+    Wavelet,
+    _as_wavelet,
+    _fold_channels,
+    _get_len,
+    _is_dtype_supported,
+    _pad_symmetric,
+    _unfold_channels,
+)
 
 
 def _create_tensor(
     filter: Sequence[float], flip: bool, device: torch.device, dtype: torch.dtype
 ) -> torch.Tensor:
     if flip:
         if isinstance(filter, torch.Tensor):
@@ -22,15 +30,15 @@
     else:
         if isinstance(filter, torch.Tensor):
             return filter.unsqueeze(0).to(device=device, dtype=dtype)
         else:
             return torch.tensor(filter, device=device, dtype=dtype).unsqueeze(0)
 
 
-def get_filter_tensors(
+def _get_filter_tensors(
     wavelet: Union[Wavelet, str],
     flip: bool,
     device: Union[torch.device, str],
     dtype: torch.dtype = torch.float32,
 ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
     """Convert input wavelet to filter tensors.
 
@@ -112,33 +120,37 @@
         pt_mode = "replicate"
     elif pywt_mode == "zero":
         pt_mode = "constant"
     elif pywt_mode == "reflect":
         pt_mode = pywt_mode
     elif pywt_mode == "periodic":
         pt_mode = "circular"
+    elif pywt_mode == "symmetric":
+        # pytorch does not support symmetric mode,
+        # we have our own implementation.
+        pt_mode = pywt_mode
     else:
         raise ValueError("Padding mode not supported.")
     return pt_mode
 
 
 def _fwt_pad(
     data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str = "reflect"
 ) -> torch.Tensor:
     """Pad the input signal to make the fwt matrix work.
 
     The padding assumes a future step will transform the last axis.
 
     Args:
-        data (torch.Tensor): Input data [batch_size, 1, time]
+        data (torch.Tensor): Input data ``[batch_size, 1, time]``
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         mode (str): The desired way to pad. The following methods are supported::
 
-                "reflect", "zero", "constant", "periodic".
+                "reflect", "zero", "constant", "periodic", "symmetric".
 
             Refection padding mirrors samples along the border.
             Zero padding pads zeros.
             Constant padding replicates border values.
             Periodic padding cyclically repeats samples.
             This function defaults to reflect.
 
@@ -147,15 +159,18 @@
 
     """
     wavelet = _as_wavelet(wavelet)
     # convert pywt to pytorch convention.
     mode = _translate_boundary_strings(mode)
 
     padr, padl = _get_pad(data.shape[-1], _get_len(wavelet))
-    data_pad = torch.nn.functional.pad(data, [padl, padr], mode=mode)
+    if mode == "symmetric":
+        data_pad = _pad_symmetric(data, [(padl, padr)])
+    else:
+        data_pad = torch.nn.functional.pad(data, [padl, padr], mode=mode)
     return data_pad
 
 
 def _flatten_2d_coeff_lst(
     coeff_lst_2d: List[
         Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
     ],
@@ -192,40 +207,78 @@
     pred_size = res_ll_size - (pad_start + pad_end)
     next_size = coeff_size
     if next_size == pred_size:
         pass
     elif next_size == pred_size - 1:
         pad_end += 1
     else:
-        raise AssertionError("padding error, please open an issue on github")
+        raise AssertionError(
+            "padding error, please check if dec and rec wavelets are identical."
+        )
     return pad_end, pad_start
 
 
+def _wavedec_fold_channels_1d(data: torch.Tensor) -> Tuple[torch.Tensor, List[int]]:
+    data = data.unsqueeze(-2)
+    ds = data.shape
+    data = _fold_channels(data)
+    return data, list(ds)
+
+
+def _wavedec_unfold_channels_1d_list(
+    result_list: List[torch.Tensor], ds: List[int]
+) -> List[torch.Tensor]:
+    unfold_res = []
+    for res_coeff in result_list:
+        unfold_res.append(
+            _unfold_channels(res_coeff.unsqueeze(1), list(ds)).squeeze(-2)
+        )
+    return unfold_res
+
+
+def _waverec_fold_channels_1d_list(
+    coeff_list: List[torch.Tensor],
+) -> Tuple[List[torch.Tensor], List[int]]:
+    folded = []
+    ds = coeff_list[0].unsqueeze(-2).shape
+    for to_fold_coeff in coeff_list:
+        folded.append(_fold_channels(to_fold_coeff.unsqueeze(-2)).squeeze(-2))
+    return folded, list(ds)
+
+
 def wavedec(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
     mode: str = "reflect",
     level: Optional[int] = None,
 ) -> List[torch.Tensor]:
     """Compute the analysis (forward) 1d fast wavelet transform.
 
     Args:
-        data (torch.Tensor): Input time series of shape [batch_size, 1, time]
-                             1d inputs are interpreted as [time],
-                             2d inputs are interpreted as [batch_size, time].
+        data (torch.Tensor): The input time series,
+                             1d inputs are interpreted as ``[time]``,
+                             2d inputs as ``[batch_size, time]``,
+                             and 3d inputs as ``[batch_size, channels, time]``.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
             Please consider the output from ``pywt.wavelist(kind='discrete')``
             for possible choices.
         mode (str): The desired padding mode. Padding extends the signal along
             the edges. Supported methods are::
 
-                "reflect", "zero", "constant", "periodic".
+                "reflect", "zero", "constant", "periodic", "symmetric".
 
             Defaults to "reflect".
+
+            Symmetric padding mirrors samples along the border.
+            Refection padding reflects samples along the border.
+            Zero padding pads zeros.
+            Constant padding replicates border values.
+            Periodic padding cyclically repeats samples.
+
         level (int): The scale level to be computed.
                                Defaults to None.
 
     Returns:
         list: A list::
 
             [cA_n, cD_n, cD_n-1, …, cD2, cD1]
@@ -242,44 +295,53 @@
         >>> import numpy as np
         >>> # generate an input of even length.
         >>> data = np.array([0, 1, 2, 3, 4, 5, 5, 4, 3, 2, 1, 0])
         >>> data_torch = torch.from_numpy(data.astype(np.float32))
         >>> # compute the forward fwt coefficients
         >>> ptwt.wavedec(data_torch, pywt.Wavelet('haar'),
         >>>              mode='zero', level=2)
-
     """
+    fold = False
     if data.dim() == 1:
         # assume time series
         data = data.unsqueeze(0).unsqueeze(0)
     elif data.dim() == 2:
         # assume batched time series
         data = data.unsqueeze(1)
+    elif data.dim() == 3:
+        # assume batch, channels, time -> fold channels
+        fold = True
+        data, ds = _wavedec_fold_channels_1d(data)
 
     if not _is_dtype_supported(data.dtype):
         raise ValueError(f"Input dtype {data.dtype} not supported")
 
-    dec_lo, dec_hi, _, _ = get_filter_tensors(
+    dec_lo, dec_hi, _, _ = _get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
     filt_len = dec_lo.shape[-1]
     filt = torch.stack([dec_lo, dec_hi], 0)
 
     if level is None:
         level = pywt.dwt_max_level(data.shape[-1], filt_len)
 
-    result_lst = []
+    result_list = []
     res_lo = data
     for _ in range(level):
         res_lo = _fwt_pad(res_lo, wavelet, mode=mode)
         res = torch.nn.functional.conv1d(res_lo, filt, stride=2)
         res_lo, res_hi = torch.split(res, 1, 1)
-        result_lst.append(res_hi.squeeze(1))
-    result_lst.append(res_lo.squeeze(1))
-    return result_lst[::-1]
+        result_list.append(res_hi.squeeze(1))
+    result_list.append(res_lo.squeeze(1))
+
+    # unfold if necessary
+    if fold:
+        result_list = _wavedec_unfold_channels_1d_list(result_list, ds)
+
+    return result_list[::-1]
 
 
 def waverec(coeffs: List[torch.Tensor], wavelet: Union[Wavelet, str]) -> torch.Tensor:
     """Reconstruct a signal from wavelet coefficients.
 
     Args:
         coeffs (list): The wavelet coefficient list produced by wavedec.
@@ -313,15 +375,21 @@
 
     for coeff in coeffs[1:]:
         if torch_device != coeff.device:
             raise ValueError("coefficients must be on the same device")
         elif torch_dtype != coeff.dtype:
             raise ValueError("coefficients must have the same dtype")
 
-    _, _, rec_lo, rec_hi = get_filter_tensors(
+    # fold channels, if necessary.
+    fold = False
+    if coeffs[0].dim() == 3:
+        fold = True
+        coeffs, ds = _waverec_fold_channels_1d_list(coeffs)
+
+    _, _, rec_lo, rec_hi = _get_filter_tensors(
         wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
     filt = torch.stack([rec_lo, rec_hi], 0)
 
     res_lo = coeffs[0]
     for c_pos, res_hi in enumerate(coeffs[1:]):
@@ -335,8 +403,12 @@
             padr, padl = _adjust_padding_at_reconstruction(
                 res_lo.shape[-1], coeffs[c_pos + 2].shape[-1], padr, padl
             )
         if padl > 0:
             res_lo = res_lo[..., padl:]
         if padr > 0:
             res_lo = res_lo[..., :-padr]
+
+    if fold:
+        res_lo = _unfold_channels(res_lo.unsqueeze(-2), list(ds)).squeeze(-2)
+
     return res_lo
```

### Comparing `ptwt-0.1.5/src/ptwt/conv_transform_2.py` & `ptwt-0.1.6/src/ptwt/conv_transform_3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,287 @@
-"""This module implements two-dimensional padded wavelet transforms.
+"""Code for three dimensional padded transforms.
 
-The implementation relies on torch.nn.functional.conv2d and
-torch.nn.functional.conv_transpose2d under the hood.
+The functions here are based on torch.nn.functional.conv3d and it's transpose.
 """
 
-
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Sequence, Union, cast
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported, _outer
+from ._util import (
+    Wavelet,
+    _as_wavelet,
+    _get_len,
+    _is_dtype_supported,
+    _outer,
+    _pad_symmetric,
+)
 from .conv_transform import (
     _adjust_padding_at_reconstruction,
+    _get_filter_tensors,
     _get_pad,
     _translate_boundary_strings,
-    get_filter_tensors,
 )
 
 
-def construct_2d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
-    """Construct two-dimensional filters using outer products.
+def _construct_3d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
+    """Construct three-dimensional filters using outer products.
 
     Args:
         lo (torch.Tensor): Low-pass input filter.
         hi (torch.Tensor): High-pass input filter
 
     Returns:
-        torch.Tensor: Stacked 2d-filters of dimension
+        torch.Tensor: Stacked 3d filters of dimension::
 
-        [filt_no, 1, height, width].
+        [8, 1, length, height, width].
 
         The four filters are ordered ll, lh, hl, hh.
 
     """
-    ll = _outer(lo, lo)
-    lh = _outer(hi, lo)
-    hl = _outer(lo, hi)
-    hh = _outer(hi, hi)
-    filt = torch.stack([ll, lh, hl, hh], 0)
+    dim_size = lo.shape[-1]
+    size = [dim_size] * 3
+    lll = _outer(lo, _outer(lo, lo)).reshape(size)
+    llh = _outer(lo, _outer(lo, hi)).reshape(size)
+    lhl = _outer(lo, _outer(hi, lo)).reshape(size)
+    lhh = _outer(lo, _outer(hi, hi)).reshape(size)
+    hll = _outer(hi, _outer(lo, lo)).reshape(size)
+    hlh = _outer(hi, _outer(lo, hi)).reshape(size)
+    hhl = _outer(hi, _outer(hi, lo)).reshape(size)
+    hhh = _outer(hi, _outer(hi, hi)).reshape(size)
+    filt = torch.stack([lll, llh, lhl, lhh, hll, hlh, hhl, hhh], 0)
     filt = filt.unsqueeze(1)
     return filt
 
 
-def _fwt_pad2(
-    data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str = "reflect"
+def _fwt_pad3(
+    data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str
 ) -> torch.Tensor:
-    """Pad data for the 2d FWT.
+    """Pad data for the 3d-FWT.
 
-    This function pads along the last two axes.
+    This function pads the last three axes.
 
     Args:
         data (torch.Tensor): Input data with 4 dimensions.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
-        mode (str): The padding mode.
-            Supported modes are::
-
-                "reflect", "zero", "constant", "periodic".
+        mode (str): The padding mode. Supported modes are::
 
-            "reflect" is the default mode.
+            "reflect", "zero", "constant", "periodic", "symmetric".
 
     Returns:
         The padded output tensor.
 
     """
     mode = _translate_boundary_strings(mode)
 
     wavelet = _as_wavelet(wavelet)
-    padb, padt = _get_pad(data.shape[-2], _get_len(wavelet))
-    padr, padl = _get_pad(data.shape[-1], _get_len(wavelet))
-    data_pad = torch.nn.functional.pad(data, [padl, padr, padt, padb], mode=mode)
+    pad_back, pad_front = _get_pad(data.shape[-3], _get_len(wavelet))
+    pad_bottom, pad_top = _get_pad(data.shape[-2], _get_len(wavelet))
+    pad_right, pad_left = _get_pad(data.shape[-1], _get_len(wavelet))
+    if mode == "symmetric":
+        data_pad = _pad_symmetric(
+            data, [(pad_front, pad_back), (pad_top, pad_bottom), (pad_left, pad_right)]
+        )
+    else:
+        data_pad = torch.nn.functional.pad(
+            data,
+            [pad_left, pad_right, pad_top, pad_bottom, pad_front, pad_back],
+            mode=mode,
+        )
     return data_pad
 
 
-def wavedec2(
+def wavedec3(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
-    mode: str = "reflect",
+    mode: str = "zero",
     level: Optional[int] = None,
-) -> List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]:
-    """Non separated two-dimensional wavelet transform.
+) -> List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
+    """Compute a three-dimensional wavelet transform.
 
     Args:
-        data (torch.Tensor): The input data tensor with up to three dimensions.
-            2d inputs are interpreted as [height, width],
-            3d inputs are interpreted as [batch_size, height, width].
-        wavelet (Wavelet or str): A pywt wavelet compatible object or
-            the name of a pywt wavelet. Refer to the output of
-            ``pywt.wavelist(kind="discrete")`` for a list of possible choices.
-        mode (str): The padding mode. Options are::
-
-                "reflect", "zero", "constant", "periodic".
-
-            This function defaults to "reflect".
-        level (int): The number of desired scales.
-            Defaults to None.
+        data (torch.Tensor): The input data of shape
+            [batch_size, length, height, width]
+        wavelet (Union[Wavelet, str]): The wavelet to transform with.
+            ``pywt.wavelist(kind='discrete')`` lists possible choices.
+        mode (str): The padding mode. Possible options are::
+
+                "reflect", "zero", "constant", "periodic", "symmetric".
+
+            Defaults to "zero".
+        level (Optional[int]): The maximum decomposition level.
+            This argument defaults to None.
 
     Returns:
-        list: A list containing the wavelet coefficients.
-        The coefficients are in pywt order. That is::
+        list: A list with the lll coefficients and dictionaries
+        with the filter order strings::
 
-            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
+            ("aad", "ada", "add", "daa", "dad", "dda", "ddd")
 
-        A denotes approximation, H horizontal, V vertical
-        and D diagonal coefficients.
+        as keys. With a for the low pass or approximation filter and
+        d for the high-pass or detail filter.
 
     Raises:
-        ValueError: If the dimensionality or the dtype of the input data tensor
-            is unsupported.
+        ValueError: If the input has fewer than three dimensions or
+            if the dtype is not supported.
 
     Example:
-        >>> import torch
-        >>> import ptwt, pywt
-        >>> import numpy as np
-        >>> from scipy import datasets
-        >>> face = np.transpose(datasets.face(),
-        >>>                     [2, 0, 1]).astype(np.float64)
-        >>> pytorch_face = torch.tensor(face)
-        >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
-        >>>                              level=2, mode="zero")
+        >>> import ptwt, torch
+        >>> data = torch.randn(5, 16, 16, 16)
+        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
 
     """
-    if data.dim() == 2:
-        data = data.unsqueeze(0).unsqueeze(0)
+    if data.dim() < 3:
+        raise ValueError("Three dimensional inputs required for 3d wavedec.")
     elif data.dim() == 3:
-        # add a channel dimension for torch.
-        data = data.unsqueeze(1)
-    elif data.dim() == 4:
-        raise ValueError(
-            "Wavedec2 does not support four input dimensions. \
-             Optionally-batched two-dimensional inputs work."
-        )
-    elif data.dim() == 1:
-        raise ValueError("Wavedec2 needs more than one input dimension to work.")
+        # add batch dim.
+        data = data.unsqueeze(0)
 
     if not _is_dtype_supported(data.dtype):
         raise ValueError(f"Input dtype {data.dtype} not supported")
 
     wavelet = _as_wavelet(wavelet)
-    dec_lo, dec_hi, _, _ = get_filter_tensors(
+    dec_lo, dec_hi, _, _ = _get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
-    dec_filt = construct_2d_filt(lo=dec_lo, hi=dec_hi)
+    dec_filt = _construct_3d_filt(lo=dec_lo, hi=dec_hi)
 
     if level is None:
-        level = pywt.dwtn_max_level([data.shape[-1], data.shape[-2]], wavelet)
+        level = pywt.dwtn_max_level(
+            [data.shape[-1], data.shape[-2], data.shape[-3]], wavelet
+        )
 
-    result_lst: List[
-        Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
-    ] = []
-    res_ll = data
+    result_lst: List[Union[torch.Tensor, Dict[str, torch.Tensor]]] = []
+    res_lll = data
     for _ in range(level):
-        res_ll = _fwt_pad2(res_ll, wavelet, mode=mode)
-        res = torch.nn.functional.conv2d(res_ll, dec_filt, stride=2)
-        res_ll, res_lh, res_hl, res_hh = torch.split(res, 1, 1)
-        to_append = (res_lh.squeeze(1), res_hl.squeeze(1), res_hh.squeeze(1))
-        result_lst.append(to_append)
-    result_lst.append(res_ll.squeeze(1))
+        res_lll = _fwt_pad3(res_lll.unsqueeze(1), wavelet, mode=mode)
+        res = torch.nn.functional.conv3d(res_lll, dec_filt, stride=2)
+        res_lll, res_llh, res_lhl, res_lhh, res_hll, res_hlh, res_hhl, res_hhh = [
+            sr.squeeze(1) for sr in torch.split(res, 1, 1)
+        ]
+        result_lst.append(
+            {
+                "aad": res_llh,
+                "ada": res_lhl,
+                "add": res_lhh,
+                "daa": res_hll,
+                "dad": res_hlh,
+                "dda": res_hhl,
+                "ddd": res_hhh,
+            }
+        )
+    result_lst.append(res_lll)
     return result_lst[::-1]
 
 
-def waverec2(
-    coeffs: List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
+def waverec3(
+    coeffs: Sequence[Union[torch.Tensor, Dict[str, torch.Tensor]]],
     wavelet: Union[Wavelet, str],
 ) -> torch.Tensor:
     """Reconstruct a signal from wavelet coefficients.
 
     Args:
-        coeffs (list): The wavelet coefficient list produced by wavedec2.
-            The coefficients must be in pywt order. That is::
-
-            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
-
-            A denotes approximation, H horizontal, V vertical,
-            and D diagonal coefficients.
+        coeffs (list): The wavelet coefficient list produced by wavedec3.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
 
     Returns:
-        torch.Tensor: The reconstructed signal of shape [batch, height, width].
+        torch.Tensor: The reconstructed four-dimensional signal of shape
+        [batch, depth, height, width].
 
     Raises:
-        ValueError: If `coeffs` is not in a shape as returned from `wavedec2` or
+        ValueError: If coeffs is not in a shape as returned from wavedec3 or
             if the dtype is not supported.
 
     Example:
-        >>> import ptwt, pywt, torch
-        >>> import numpy as np
-        >>> from scipy import datasets
-        >>> face = np.transpose(datasets.face(),
-        >>>                     [2, 0, 1]).astype(np.float64)
-        >>> pytorch_face = torch.tensor(face)
-        >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
-        >>>                              level=2, mode="constant")
-        >>> reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
+        >>> import ptwt, torch
+        >>> data = torch.randn(5, 16, 16, 16)
+        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
+        >>> reconstruction = ptwt.waverec3(transformed, "haar")
 
     """
     wavelet = _as_wavelet(wavelet)
-
-    res_ll = coeffs[0]
-    if not isinstance(res_ll, torch.Tensor):
+    # the Union[tensor, dict] idea is coming from pywt. We don't change it here.
+    res_lll = coeffs[0]
+    if not isinstance(res_lll, torch.Tensor):
         raise ValueError(
             "First element of coeffs must be the approximation coefficient tensor."
         )
 
-    torch_device = res_ll.device
-    torch_dtype = res_ll.dtype
+    torch_device = res_lll.device
+    torch_dtype = res_lll.dtype
 
     if not _is_dtype_supported(torch_dtype):
-        raise ValueError(f"Input dtype {torch_dtype} not supported")
+        if not _is_dtype_supported(torch_dtype):
+            raise ValueError(f"Input dtype {torch_dtype} not supported")
 
-    _, _, rec_lo, rec_hi = get_filter_tensors(
+    _, _, rec_lo, rec_hi = _get_filter_tensors(
         wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
-    rec_filt = construct_2d_filt(lo=rec_lo, hi=rec_hi)
+    rec_filt = _construct_3d_filt(lo=rec_lo, hi=rec_hi)
 
-    for c_pos, coeff_tuple in enumerate(coeffs[1:]):
-        if not isinstance(coeff_tuple, tuple) or len(coeff_tuple) != 3:
+    coeff_dicts = cast(Sequence[Dict[str, torch.Tensor]], coeffs[1:])
+    for c_pos, coeff_dict in enumerate(coeff_dicts):
+        if not isinstance(coeff_dict, dict) or len(coeff_dict) != 7:
             raise ValueError(
-                f"Unexpected detail coefficient type: {type(coeff_tuple)}. Detail "
-                "coefficients must be a 3-tuple of tensors as returned by "
-                "wavedec2."
+                f"Unexpected detail coefficient type: {type(coeff_dict)}. Detail "
+                "coefficients must be a dict containing 7 tensors as returned by "
+                "wavedec3."
             )
-
-        curr_shape = res_ll.shape
-        for coeff in coeff_tuple:
+        for coeff in coeff_dict.values():
             if torch_device != coeff.device:
                 raise ValueError("coefficients must be on the same device")
             elif torch_dtype != coeff.dtype:
                 raise ValueError("coefficients must have the same dtype")
-            elif coeff.shape != curr_shape:
+            elif res_lll.shape != coeff.shape:
                 raise ValueError(
                     "All coefficients on each level must have the same shape"
                 )
-
-        res_lh, res_hl, res_hh = coeff_tuple
-
-        res_ll = torch.stack([res_ll, res_lh, res_hl, res_hh], 1)
-        res_ll = torch.nn.functional.conv_transpose2d(
-            res_ll, rec_filt, stride=2
-        ).squeeze(1)
+        res_lll = torch.stack(
+            [
+                res_lll,
+                coeff_dict["aad"],
+                coeff_dict["ada"],
+                coeff_dict["add"],
+                coeff_dict["daa"],
+                coeff_dict["dad"],
+                coeff_dict["dda"],
+                coeff_dict["ddd"],
+            ],
+            1,
+        )
+        res_lll = torch.nn.functional.conv_transpose3d(res_lll, rec_filt, stride=2)
+        res_lll = res_lll.squeeze(1)
 
         # remove the padding
+        padfr = (2 * filt_len - 3) // 2
+        padba = (2 * filt_len - 3) // 2
         padl = (2 * filt_len - 3) // 2
         padr = (2 * filt_len - 3) // 2
         padt = (2 * filt_len - 3) // 2
         padb = (2 * filt_len - 3) // 2
-        if c_pos < len(coeffs) - 2:
+        if c_pos + 1 < len(coeff_dicts):
             padr, padl = _adjust_padding_at_reconstruction(
-                res_ll.shape[-1], coeffs[c_pos + 2][0].shape[-1], padr, padl
+                res_lll.shape[-1], coeff_dicts[c_pos + 1]["aad"].shape[-1], padr, padl
             )
             padb, padt = _adjust_padding_at_reconstruction(
-                res_ll.shape[-2], coeffs[c_pos + 2][0].shape[-2], padb, padt
+                res_lll.shape[-2], coeff_dicts[c_pos + 1]["aad"].shape[-2], padb, padt
+            )
+            padba, padfr = _adjust_padding_at_reconstruction(
+                res_lll.shape[-3], coeff_dicts[c_pos + 1]["aad"].shape[-3], padba, padfr
             )
-
         if padt > 0:
-            res_ll = res_ll[..., padt:, :]
+            res_lll = res_lll[..., padt:, :]
         if padb > 0:
-            res_ll = res_ll[..., :-padb, :]
+            res_lll = res_lll[..., :-padb, :]
         if padl > 0:
-            res_ll = res_ll[..., padl:]
+            res_lll = res_lll[..., padl:]
         if padr > 0:
-            res_ll = res_ll[..., :-padr]
-    return res_ll
+            res_lll = res_lll[..., :-padr]
+        if padfr > 0:
+            res_lll = res_lll[..., padfr:, :, :]
+        if padba > 0:
+            res_lll = res_lll[..., :-padba, :, :]
+    return res_lll
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ptwt-0.1.5/src/ptwt/conv_transform_3.py` & `ptwt-0.1.6/src/ptwt/conv_transform_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,269 +1,354 @@
-"""Code for three dimensional padded transforms.
+"""This module implements two-dimensional padded wavelet transforms.
 
-The functions here are based on torch.nn.functional.conv3d and it's transpose.
+The implementation relies on torch.nn.functional.conv2d and
+torch.nn.functional.conv_transpose2d under the hood.
 """
 
-from typing import Dict, List, Optional, Sequence, Union, cast
+
+from typing import Any, List, Optional, Tuple, Union
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported, _outer
+from ._util import (
+    Wavelet,
+    _as_wavelet,
+    _fold_channels,
+    _get_len,
+    _is_dtype_supported,
+    _outer,
+    _pad_symmetric,
+    _unfold_channels,
+)
 from .conv_transform import (
     _adjust_padding_at_reconstruction,
+    _get_filter_tensors,
     _get_pad,
     _translate_boundary_strings,
-    get_filter_tensors,
 )
 
 
-def _construct_3d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
-    """Construct three dimensional filters using outer products.
+def _construct_2d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
+    """Construct two-dimensional filters using outer products.
 
     Args:
         lo (torch.Tensor): Low-pass input filter.
         hi (torch.Tensor): High-pass input filter
 
     Returns:
-        torch.Tensor: Stacked 3d filters of dimension::
+        torch.Tensor: Stacked 2d-filters of dimension
 
-        [8, 1, length, height, width].
+        [filt_no, 1, height, width].
 
         The four filters are ordered ll, lh, hl, hh.
 
     """
-    dim_size = lo.shape[-1]
-    size = [dim_size] * 3
-    lll = _outer(lo, _outer(lo, lo)).reshape(size)
-    llh = _outer(lo, _outer(lo, hi)).reshape(size)
-    lhl = _outer(lo, _outer(hi, lo)).reshape(size)
-    lhh = _outer(lo, _outer(hi, hi)).reshape(size)
-    hll = _outer(hi, _outer(lo, lo)).reshape(size)
-    hlh = _outer(hi, _outer(lo, hi)).reshape(size)
-    hhl = _outer(hi, _outer(hi, lo)).reshape(size)
-    hhh = _outer(hi, _outer(hi, hi)).reshape(size)
-    filt = torch.stack([lll, llh, lhl, lhh, hll, hlh, hhl, hhh], 0)
+    ll = _outer(lo, lo)
+    lh = _outer(hi, lo)
+    hl = _outer(lo, hi)
+    hh = _outer(hi, hi)
+    filt = torch.stack([ll, lh, hl, hh], 0)
     filt = filt.unsqueeze(1)
     return filt
 
 
-def _fwt_pad3(
-    data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str
+def _fwt_pad2(
+    data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str = "reflect"
 ) -> torch.Tensor:
-    """Pad data for the 3d-FWT.
+    """Pad data for the 2d FWT.
 
-    This function pads the last three axes.
+    This function pads along the last two axes.
 
     Args:
         data (torch.Tensor): Input data with 4 dimensions.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
-        mode (str): The padding mode. Supported modes are "zero".
+        mode (str): The padding mode.
+            Supported modes are::
+
+                "reflect", "zero", "constant", "periodic", "symmetric".
+
+            "reflect" is the default mode.
 
     Returns:
         The padded output tensor.
 
     """
     mode = _translate_boundary_strings(mode)
-
     wavelet = _as_wavelet(wavelet)
-    pad_back, pad_front = _get_pad(data.shape[-3], _get_len(wavelet))
-    pad_bottom, pad_top = _get_pad(data.shape[-2], _get_len(wavelet))
-    pad_right, pad_left = _get_pad(data.shape[-1], _get_len(wavelet))
-    data_pad = torch.nn.functional.pad(
-        data, [pad_left, pad_right, pad_top, pad_bottom, pad_front, pad_back], mode=mode
-    )
+    padb, padt = _get_pad(data.shape[-2], _get_len(wavelet))
+    padr, padl = _get_pad(data.shape[-1], _get_len(wavelet))
+    if mode == "symmetric":
+        data_pad = _pad_symmetric(data, [(padt, padb), (padl, padr)])
+    else:
+        data_pad = torch.nn.functional.pad(data, [padl, padr, padt, padb], mode=mode)
     return data_pad
 
 
-def wavedec3(
+def _wavedec2d_unfold_channels_2d_list(
+    result_list: List[
+        Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
+    ],
+    ds: List[int],
+) -> List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]:
+    # unfolds the wavedec2d result lists, restoring the channel dimension.
+    unfold_res: List[
+        Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
+    ] = []
+    for cres in result_list:
+        if isinstance(cres, torch.Tensor):
+            unfold_res.append(_unfold_channels(cres, list(ds)))
+        else:
+            unfold_res.append(
+                (
+                    _unfold_channels(cres[0], list(ds)),
+                    _unfold_channels(cres[1], list(ds)),
+                    _unfold_channels(cres[2], list(ds)),
+                )
+            )
+    return unfold_res
+
+
+def _waverec2d_fold_channels_2d_list(
+    coeffs: List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
+) -> Tuple[
+    List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
+    List[int],
+]:
+    # fold the input coefficients for processing conv2d_transpose.
+    fold_coeffs: List[
+        Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
+    ] = []
+    ds = list(_check_if_tensor(coeffs[0]).shape)
+    for coeff in coeffs:
+        if isinstance(coeff, torch.Tensor):
+            fold_coeffs.append(_fold_channels(coeff))
+        else:
+            fold_coeffs.append(
+                (
+                    _fold_channels(coeff[0]),
+                    _fold_channels(coeff[1]),
+                    _fold_channels(coeff[2]),
+                )
+            )
+    return fold_coeffs, ds
+
+
+def wavedec2(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
-    mode: str = "zero",
+    mode: str = "reflect",
     level: Optional[int] = None,
-) -> List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
-    """Compute a three-dimensional wavelet transform.
+) -> List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]:
+    """Non-separated two-dimensional wavelet transform. Only the last two axes change.
 
     Args:
-        data (torch.Tensor): The input data of shape
-            [batch_size, length, height, width]
-        wavelet (Union[Wavelet, str]): The wavelet to transform with.
-            ``pywt.wavelist(kind='discrete')`` lists possible choices.
-        mode (str): The padding mode. Possible options are
-            "zero", "constant" or "periodic".
-            Defaults to "zero".
-        level (Optional[int]): The maximum decomposition level.
-            This argument defaults to None.
+        data (torch.Tensor): The input data tensor with up to three dimensions.
+            2d inputs are interpreted as ``[height, width]``,
+            3d inputs are interpreted as ``[batch_size, height, width]``.
+            4d inputs are interpreted as ``[batch_size, channels, height, width]``.
+        wavelet (Wavelet or str): A pywt wavelet compatible object or
+            the name of a pywt wavelet. Refer to the output of
+            ``pywt.wavelist(kind="discrete")`` for a list of possible choices.
+        mode (str): The padding mode. Options are::
+
+                "reflect", "zero", "constant", "periodic", "symmetric".
+
+            This function defaults to "reflect".
+        level (int): The number of desired scales.
+            Defaults to None.
 
     Returns:
-        list: A list with the lll coefficients and dictionaries
-        with the filter order strings::
+        list: A list containing the wavelet coefficients.
+        The coefficients are in pywt order. That is::
 
-        ("aad", "ada", "add", "daa", "dad", "dda", "ddd")
+            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
 
-        as keys. With a for the low pass or approximation filter and
-        d for the high-pass or detail filter.
+        A denotes approximation, H horizontal, V vertical
+        and D diagonal coefficients.
 
     Raises:
-        ValueError: If the input has fewer than three dimensions or
-            if the dtype is not supported.
+        ValueError: If the dimensionality or the dtype of the input data tensor
+            is unsupported.
 
     Example:
-        >>> import ptwt, torch
-        >>> data = torch.randn(5, 16, 16, 16)
-        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
+        >>> import torch
+        >>> import ptwt, pywt
+        >>> import numpy as np
+        >>> from scipy import datasets
+        >>> face = np.transpose(datasets.face(),
+        >>>                     [2, 0, 1]).astype(np.float64)
+        >>> pytorch_face = torch.tensor(face)
+        >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
+        >>>                              level=2, mode="zero")
 
     """
-    if data.dim() < 3:
-        raise ValueError("Three dimensional inputs required for 3d wavedec.")
+    fold = False
+    if data.dim() == 2:
+        data = data.unsqueeze(0).unsqueeze(0)
     elif data.dim() == 3:
-        # add batch dim.
-        data = data.unsqueeze(0)
+        # add a channel dimension for torch.
+        data = data.unsqueeze(1)
+    elif data.dim() == 4:
+        # avoid the channel sum, fold the channels into batches.
+        fold = True
+        ds = data.shape
+        data = _fold_channels(data).unsqueeze(1)
+    elif data.dim() == 1:
+        raise ValueError("Wavedec2 needs more than one input dimension to work.")
+    else:
+        raise ValueError(
+            "Wavedec2 does not support four input dimensions. \
+             Optionally-batched two-dimensional inputs work."
+        )
 
     if not _is_dtype_supported(data.dtype):
         raise ValueError(f"Input dtype {data.dtype} not supported")
 
     wavelet = _as_wavelet(wavelet)
-    dec_lo, dec_hi, _, _ = get_filter_tensors(
+    dec_lo, dec_hi, _, _ = _get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
-    dec_filt = _construct_3d_filt(lo=dec_lo, hi=dec_hi)
+    dec_filt = _construct_2d_filt(lo=dec_lo, hi=dec_hi)
 
     if level is None:
-        level = pywt.dwtn_max_level(
-            [data.shape[-1], data.shape[-2], data.shape[-3]], wavelet
-        )
+        level = pywt.dwtn_max_level([data.shape[-1], data.shape[-2]], wavelet)
 
-    result_lst: List[Union[torch.Tensor, Dict[str, torch.Tensor]]] = []
-    res_lll = data
+    result_lst: List[
+        Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
+    ] = []
+    res_ll = data
     for _ in range(level):
-        res_lll = _fwt_pad3(res_lll.unsqueeze(1), wavelet, mode=mode)
-        res = torch.nn.functional.conv3d(res_lll, dec_filt, stride=2)
-        res_lll, res_llh, res_lhl, res_lhh, res_hll, res_hlh, res_hhl, res_hhh = [
-            sr.squeeze(1) for sr in torch.split(res, 1, 1)
-        ]
-        result_lst.append(
-            {
-                "aad": res_llh,
-                "ada": res_lhl,
-                "add": res_lhh,
-                "daa": res_hll,
-                "dad": res_hlh,
-                "dda": res_hhl,
-                "ddd": res_hhh,
-            }
-        )
-    result_lst.append(res_lll)
+        res_ll = _fwt_pad2(res_ll, wavelet, mode=mode)
+        res = torch.nn.functional.conv2d(res_ll, dec_filt, stride=2)
+        res_ll, res_lh, res_hl, res_hh = torch.split(res, 1, 1)
+        to_append = (res_lh.squeeze(1), res_hl.squeeze(1), res_hh.squeeze(1))
+        result_lst.append(to_append)
+    result_lst.append(res_ll.squeeze(1))
+
+    if fold:
+        result_lst = _wavedec2d_unfold_channels_2d_list(result_lst, list(ds))
+
     return result_lst[::-1]
 
 
-def waverec3(
-    coeffs: Sequence[Union[torch.Tensor, Dict[str, torch.Tensor]]],
+def _check_if_tensor(to_check: Any) -> torch.Tensor:
+    # Ensuring the first list elements are tensors makes mypy happy :-).
+    if not isinstance(to_check, torch.Tensor):
+        raise ValueError(
+            "First element of coeffs must be the approximation coefficient tensor."
+        )
+    else:
+        return to_check
+
+
+def waverec2(
+    coeffs: List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
     wavelet: Union[Wavelet, str],
 ) -> torch.Tensor:
     """Reconstruct a signal from wavelet coefficients.
 
     Args:
-        coeffs (list): The wavelet coefficient list produced by wavedec3.
+        coeffs (list): The wavelet coefficient list produced by wavedec2.
+            The coefficients must be in pywt order. That is::
+
+            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
+
+            A denotes approximation, H horizontal, V vertical,
+            and D diagonal coefficients.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
 
     Returns:
-        torch.Tensor: The reconstructed four-dimensional signal of shape
-        [batch, depth, height, width].
+        torch.Tensor: The reconstructed signal of shape ``[batch, height, width]`` or
+            ``[batch, channel, height, width]`` depending on the input to `wavedec2`.
 
     Raises:
-        ValueError: If `coeffs` is not in a shape as returned from `wavedec3` or
+        ValueError: If coeffs is not in a shape as returned from wavedec2 or
             if the dtype is not supported.
 
     Example:
-        >>> import ptwt, torch
-        >>> data = torch.randn(5, 16, 16, 16)
-        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
-        >>> reconstruction = ptwt.waverec3(transformed, "haar")
+        >>> import ptwt, pywt, torch
+        >>> import numpy as np
+        >>> from scipy import datasets
+        >>> face = np.transpose(datasets.face(),
+        >>>                     [2, 0, 1]).astype(np.float64)
+        >>> pytorch_face = torch.tensor(face)
+        >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
+        >>>                              level=2, mode="constant")
+        >>> reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
 
     """
     wavelet = _as_wavelet(wavelet)
-    # the Union[tensor, dict] idea is coming from pywt. We don't change it here.
-    res_lll = coeffs[0]
-    if not isinstance(res_lll, torch.Tensor):
-        raise ValueError(
-            "First element of coeffs must be the approximation coefficient tensor."
-        )
 
-    torch_device = res_lll.device
-    torch_dtype = res_lll.dtype
+    res_ll = _check_if_tensor(coeffs[0])
+    torch_device = res_ll.device
+    torch_dtype = res_ll.dtype
+
+    fold = False
+    if res_ll.dim() == 4:
+        # avoid the channel sum, fold the channels into batches.
+        fold = True
+        coeffs, ds = _waverec2d_fold_channels_2d_list(coeffs)
+        res_ll = _check_if_tensor(coeffs[0])
 
     if not _is_dtype_supported(torch_dtype):
-        if not _is_dtype_supported(torch_dtype):
-            raise ValueError(f"Input dtype {torch_dtype} not supported")
+        raise ValueError(f"Input dtype {torch_dtype} not supported")
 
-    _, _, rec_lo, rec_hi = get_filter_tensors(
+    _, _, rec_lo, rec_hi = _get_filter_tensors(
         wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
-    rec_filt = _construct_3d_filt(lo=rec_lo, hi=rec_hi)
+    rec_filt = _construct_2d_filt(lo=rec_lo, hi=rec_hi)
 
-    coeff_dicts = cast(Sequence[Dict[str, torch.Tensor]], coeffs[1:])
-    for c_pos, coeff_dict in enumerate(coeff_dicts):
-        if not isinstance(coeff_dict, dict) or len(coeff_dict) != 7:
+    for c_pos, coeff_tuple in enumerate(coeffs[1:]):
+        if not isinstance(coeff_tuple, tuple) or len(coeff_tuple) != 3:
             raise ValueError(
-                f"Unexpected detail coefficient type: {type(coeff_dict)}. Detail "
-                "coefficients must be a dict containing 7 tensors as returned by "
-                "wavedec3."
+                f"Unexpected detail coefficient type: {type(coeff_tuple)}. Detail "
+                "coefficients must be a 3-tuple of tensors as returned by "
+                "wavedec2."
             )
-        for coeff in coeff_dict.values():
+
+        curr_shape = res_ll.shape
+        for coeff in coeff_tuple:
             if torch_device != coeff.device:
                 raise ValueError("coefficients must be on the same device")
             elif torch_dtype != coeff.dtype:
                 raise ValueError("coefficients must have the same dtype")
-            elif res_lll.shape != coeff.shape:
+            elif coeff.shape != curr_shape:
                 raise ValueError(
                     "All coefficients on each level must have the same shape"
                 )
-        res_lll = torch.stack(
-            [
-                res_lll,
-                coeff_dict["aad"],
-                coeff_dict["ada"],
-                coeff_dict["add"],
-                coeff_dict["daa"],
-                coeff_dict["dad"],
-                coeff_dict["dda"],
-                coeff_dict["ddd"],
-            ],
-            1,
-        )
-        res_lll = torch.nn.functional.conv_transpose3d(res_lll, rec_filt, stride=2)
-        res_lll = res_lll.squeeze(1)
+
+        res_lh, res_hl, res_hh = coeff_tuple
+        res_ll = torch.stack([res_ll, res_lh, res_hl, res_hh], 1)
+        res_ll = torch.nn.functional.conv_transpose2d(
+            res_ll, rec_filt, stride=2
+        ).squeeze(1)
 
         # remove the padding
-        padfr = (2 * filt_len - 3) // 2
-        padba = (2 * filt_len - 3) // 2
         padl = (2 * filt_len - 3) // 2
         padr = (2 * filt_len - 3) // 2
         padt = (2 * filt_len - 3) // 2
         padb = (2 * filt_len - 3) // 2
-        if c_pos + 1 < len(coeff_dicts):
+        if c_pos < len(coeffs) - 2:
             padr, padl = _adjust_padding_at_reconstruction(
-                res_lll.shape[-1], coeff_dicts[c_pos + 1]["aad"].shape[-1], padr, padl
+                res_ll.shape[-1], coeffs[c_pos + 2][0].shape[-1], padr, padl
             )
             padb, padt = _adjust_padding_at_reconstruction(
-                res_lll.shape[-2], coeff_dicts[c_pos + 1]["aad"].shape[-2], padb, padt
-            )
-            padba, padfr = _adjust_padding_at_reconstruction(
-                res_lll.shape[-3], coeff_dicts[c_pos + 1]["aad"].shape[-3], padba, padfr
+                res_ll.shape[-2], coeffs[c_pos + 2][0].shape[-2], padb, padt
             )
+
         if padt > 0:
-            res_lll = res_lll[..., padt:, :]
+            res_ll = res_ll[..., padt:, :]
         if padb > 0:
-            res_lll = res_lll[..., :-padb, :]
+            res_ll = res_ll[..., :-padb, :]
         if padl > 0:
-            res_lll = res_lll[..., padl:]
+            res_ll = res_ll[..., padl:]
         if padr > 0:
-            res_lll = res_lll[..., :-padr]
-        if padfr > 0:
-            res_lll = res_lll[..., padfr:, :, :]
-        if padba > 0:
-            res_lll = res_lll[..., :-padba, :, :]
-    return res_lll
+            res_ll = res_ll[..., :-padr]
+
+    if fold:
+        res_ll = _unfold_channels(res_ll, list(ds))
+
+    return res_ll
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ptwt-0.1.5/src/ptwt/matmul_transform.py` & `ptwt-0.1.6/src/ptwt/matmul_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Implement matrix based fwt and ifwt.
+"""Implement matrix-based fwt and ifwt.
 
 This module uses boundary filters instead of padding.
 
 The implementation is based on the description
 in Strang Nguyen (p. 32), as well as the description
 of boundary filters in "Ripples in Mathematics" section 10.3 .
 """
@@ -14,16 +14,22 @@
 import torch
 
 from ._util import (
     Wavelet,
     _as_wavelet,
     _is_boundary_mode_supported,
     _is_dtype_supported,
+    _unfold_channels,
+)
+from .conv_transform import (
+    _get_filter_tensors,
+    _wavedec_fold_channels_1d,
+    _wavedec_unfold_channels_1d_list,
+    _waverec_fold_channels_1d_list,
 )
-from .conv_transform import get_filter_tensors
 from .sparse_math import (
     _orth_by_gram_schmidt,
     _orth_by_qr,
     cat_sparse_identity_matrix,
     construct_strided_conv_matrix,
 )
 
@@ -33,30 +39,30 @@
     length: int,
     device: Union[torch.device, str] = "cpu",
     dtype: torch.dtype = torch.float64,
 ) -> torch.Tensor:
     """Construct a raw analysis matrix.
 
     The resulting matrix will only be orthogonal in the Haar case,
-    in most cases you will want to use construct_boundary_a instead.
+    in most cases, you will want to use construct_boundary_a instead.
 
     Args:
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
-        length (int): The length of the input signal to transfrom.
+        length (int): The length of the input signal to transform.
         device (torch.device or str, optional): Where to create the matrix.
             Choose a torch device or device name. Defaults to "cpu".
         dtype (optional): The desired torch datatype. Choose torch.float32
             or torch.float64. Defaults to torch.float64.
 
     Returns:
         torch.Tensor: The sparse raw analysis matrix.
     """
     wavelet = _as_wavelet(wavelet)
-    dec_lo, dec_hi, _, _ = get_filter_tensors(
+    dec_lo, dec_hi, _, _ = _get_filter_tensors(
         wavelet, flip=False, device=device, dtype=dtype
     )
     analysis_lo = construct_strided_conv_matrix(
         dec_lo.squeeze(), length, 2, "sameshift"
     )
     analysis_hi = construct_strided_conv_matrix(
         dec_hi.squeeze(), length, 2, "sameshift"
@@ -75,25 +81,25 @@
 
     The construced matrix is NOT necessary orthogonal.
     In most cases construct_boundary_s should be used instead.
 
     Args:
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
-        length (int): The lenght of the originally transformed signal.
+        length (int): The length of the originally transformed signal.
         device (torch.device, optional): Choose cuda or cpu.
             Defaults to torch.device("cpu").
         dtype ([type], optional): The desired data type. Choose torch.float32
             or torch.float64. Defaults to torch.float64.
 
     Returns:
         torch.Tensor: The raw sparse synthesis matrix.
     """
     wavelet = _as_wavelet(wavelet)
-    _, _, rec_lo, rec_hi = get_filter_tensors(
+    _, _, rec_lo, rec_hi = _get_filter_tensors(
         wavelet, flip=True, device=device, dtype=dtype
     )
     synthesis_lo = construct_strided_conv_matrix(
         rec_lo.squeeze(), length, 2, "sameshift"
     )
     synthesis_hi = construct_strided_conv_matrix(
         rec_hi.squeeze(), length, 2, "sameshift"
@@ -146,16 +152,16 @@
     return matrix
 
 
 class MatrixWavedec(object):
     """Compute the sparse matrix fast wavelet transform.
 
     Intermediate scale results must be divisible
-    by two. A working third level transform
-    could use and input length of 128.
+    by two. A working third-level transform
+    could use an input length of 128.
     This would lead to intermediate resolutions
     of 64 and 32. All are divisible by two.
 
     Example:
         >>> import ptwt, torch, pywt
         >>> import numpy as np
         >>> # generate an input of even length.
@@ -184,15 +190,15 @@
                 Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's dense qr
                 implementation, it is fast but memory hungry. The 'gramschmidt'
                 option is sparse, memory efficient, and slow. Choose 'gramschmidt' if
                 'qr' runs out of memory. Defaults to 'qr'.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
-            ValueError: If the wavelet filters have different lenghts.
+            ValueError: If the wavelet filters have different lengths.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.level = level
         self.boundary = boundary
 
         self.input_length: Optional[int] = None
         self.fwt_matrix_list: List[torch.Tensor] = []
@@ -210,16 +216,16 @@
     def sparse_fwt_operator(self) -> torch.Tensor:
         """Return the sparse transformation operator.
 
         If the input signal at all levels is divisible by two,
         the whole operation is padding-free and can be expressed
         as a single matrix multiply.
 
-        With the operator torch.sparse.mm(sparse_fwt_operator, data.T)
-        to computes a batched fwt.
+        The operation torch.sparse.mm(sparse_fwt_operator, data.T)
+        computes a batched fwt.
 
         This property exists to make the operator matrix transparent.
         Calling the object will handle odd-length inputs properly.
 
         Returns:
             torch.Tensor: The sparse operator matrix.
 
@@ -291,35 +297,43 @@
             curr_length = curr_length // 2
 
         self.size_list.append(curr_length)
 
     def __call__(self, input_signal: torch.Tensor) -> List[torch.Tensor]:
         """Compute the matrix fwt for the given input signal.
 
-        Matrix fwt are used to avoid padding.
+        Matrix FWTs are used to avoid padding.
 
         Args:
-            input_signal (torch.Tensor): Batched input data [batch_size, time],
-                should be of even length. 1d inputs are interpreted as [time].
+            input_signal (torch.Tensor): Batched input data ``[batch_size, time]``,
+                should be of even length. 1d inputs are interpreted as ``[time]``.
+                3d inputs are treated as ``[batch, channels, time]``.
+                This transform only affects the last axis.
 
         Returns:
             List[torch.Tensor]: A list with the coefficients for each scale.
 
         Raises:
             ValueError: If the decomposition level is not a positive integer
                 or if the input signal has not the expected shape.
         """
+        fold = False
         if input_signal.dim() == 1:
             # assume time series
             input_signal = input_signal.unsqueeze(0)
-        elif input_signal.dim() != 2:
+        elif input_signal.dim() == 3:
+            # assume batch, channels, time -> fold channels
+            fold = True
+            input_signal, ds = _wavedec_fold_channels_1d(input_signal)
+            input_signal = input_signal.squeeze(1)
+        elif input_signal.dim() > 3:
             raise ValueError(
                 f"Invalid input tensor shape {input_signal.size()}. "
                 "The input signal is expected to be of the form "
-                "[batch_size, length]."
+                "[batch_size, (channels), length]."
             )
 
         if not _is_dtype_supported(input_signal.dtype):
             raise ValueError(f"Input dtype {input_signal.dtype} not supported")
 
         if input_signal.shape[-1] % 2 != 0:
             # odd length input
@@ -352,15 +366,21 @@
                 # fix odd coefficients lengths for the conv matrix to work.
                 lo = torch.nn.functional.pad(lo.T.unsqueeze(1), [0, 1]).squeeze(1).T
             coefficients = torch.sparse.mm(fwt_matrix, lo)
             lo, hi = torch.split(coefficients, coefficients.shape[0] // 2, dim=0)
             split_list.append(hi)
         split_list.append(lo)
         # undo the transpose we used to handle the batch dimension.
-        return [s.T for s in split_list[::-1]]
+        result_list = [s.T for s in split_list[::-1]]
+
+        # unfold if necessary
+        if fold:
+            result_list = _wavedec_unfold_channels_1d_list(result_list, ds)
+
+        return result_list
 
 
 def construct_boundary_a(
     wavelet: Union[Wavelet, str],
     length: int,
     device: Union[torch.device, str] = "cpu",
     boundary: str = "qr",
@@ -414,15 +434,15 @@
     wavelet = _as_wavelet(wavelet)
     s_full = _construct_s(wavelet, length, dtype=dtype, device=device)
     s_orth = orthogonalize(s_full.transpose(1, 0), wavelet.rec_len, method=boundary)
     return s_orth.transpose(1, 0)
 
 
 class MatrixWaverec(object):
-    """Matrix based inverse fast wavelet transform.
+    """Matrix-based inverse fast wavelet transform.
 
     Example:
         >>> import ptwt, torch, pywt
         >>> import numpy as np
         >>> # generate an input of even length.
         >>> data = np.array([0, 1, 2, 3, 4, 5, 5, 4, 3, 2, 1, 0])
         >>> data_torch = torch.from_numpy(data.astype(np.float32))
@@ -435,28 +455,28 @@
     """
 
     def __init__(
         self,
         wavelet: Union[Wavelet, str],
         boundary: str = "qr",
     ) -> None:
-        """Create the inverse matrix based fast wavelet transformation.
+        """Create the inverse matrix-based fast wavelet transformation.
 
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             boundary (str): The method used for boundary filter treatment.
                 Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's dense qr
                 implementation, it is fast but memory hungry. The 'gramschmidt' option
                 is sparse, memory efficient, and slow. Choose 'gramschmidt' if 'qr' runs
                 out of memory. Defaults to 'qr'.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
-            ValueError: If the wavelet filters have different lenghts.
+            ValueError: If the wavelet filters have different lengths.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.boundary = boundary
 
         self.ifwt_matrix_list: List[torch.Tensor] = []
         self.level: Optional[int] = None
         self.input_length: Optional[int] = None
@@ -474,17 +494,17 @@
 
         If the input signal at all levels is divisible by two,
         the whole operation is padding-free and can be expressed
         as a single matrix multiply.
 
         Having concatenated the analysis coefficients,
         torch.sparse.mm(sparse_ifwt_operator, coefficients.T)
-        to computes a batched ifwt.
+        to computes a batched iFWT.
 
-        This functionality is manly here to make the operator-matrix
+        This functionality is mainly here to make the operator-matrix
         transparent. Calling the object handles padding for odd inputs.
 
         Returns:
             torch.Tensor: The sparse operator matrix.
 
         Raises:
             NotImplementedError: if padding had to be used in the creation of the
@@ -563,14 +583,19 @@
             torch.Tensor: The input signal reconstruction.
 
         Raises:
             ValueError: If the decomposition level is not a positive integer or if the
                 coefficients are not in the shape as it is returned from a
                 `MatrixWavedec` object.
         """
+        fold = False
+        if coefficients[0].dim() == 3:
+            fold = True
+            coefficients, ds = _waverec_fold_channels_1d_list(coefficients)
+
         level = len(coefficients) - 1
         input_length = coefficients[-1].shape[-1] * 2
 
         re_build = False
         if self.level != level or self.input_length != input_length:
             self.level = level
             self.input_length = input_length
@@ -611,8 +636,13 @@
                 if next_len != pred_len:
                     lo = lo[:-1, :]
                     pred_len = lo.shape[0]
                     assert (
                         pred_len == next_len
                     ), "padding error, please open an issue on github"
 
-        return lo.T
+        res_lo = lo.T
+
+        if fold:
+            res_lo = _unfold_channels(res_lo.unsqueeze(-2), list(ds)).squeeze(-2)
+
+        return res_lo
```

### Comparing `ptwt-0.1.5/src/ptwt/matmul_transform_2.py` & `ptwt-0.1.6/src/ptwt/matmul_transform_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-"""Two dimensional matrix based fast wavelet transform implementations.
+"""Two-dimensional matrix based fast wavelet transform implementations.
 
 This module uses boundary filters to minimize padding.
 """
 # Written by moritz ( @ wolter.tech ) in 2021
 import sys
 from typing import List, Optional, Tuple, Union, cast
 
 import numpy as np
 import torch
 
 from ._util import (
     Wavelet,
     _as_wavelet,
+    _fold_channels,
     _is_boundary_mode_supported,
     _is_dtype_supported,
+    _unfold_channels,
+)
+from .conv_transform import _get_filter_tensors
+from .conv_transform_2 import (
+    _check_if_tensor,
+    _wavedec2d_unfold_channels_2d_list,
+    _waverec2d_fold_channels_2d_list,
+    _construct_2d_filt,
 )
-from .conv_transform import get_filter_tensors
-from .conv_transform_2 import construct_2d_filt
 from .matmul_transform import construct_boundary_a, construct_boundary_s, orthogonalize
 from .sparse_math import (
     batch_mm,
     cat_sparse_identity_matrix,
     construct_strided_conv2d_matrix,
 )
 
@@ -29,42 +36,42 @@
     wavelet: Union[Wavelet, str],
     height: int,
     width: int,
     device: Union[torch.device, str],
     dtype: torch.dtype = torch.float64,
     mode: str = "sameshift",
 ) -> torch.Tensor:
-    """Construct a raw two dimensional analysis wavelet transformation matrix.
+    """Construct a raw two-dimensional analysis wavelet transformation matrix.
 
     Args:
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         height (int): The height of the input image.
         width (int): The width of the input image.
         device (torch.device or str): Where to place the matrix.
-        dtype (torch.dtype, optional): Desired matrix data-type.
+        dtype (torch.dtype, optional): Desired matrix data type.
             Defaults to torch.float64.
         mode (str): The convolution type.
             Options are 'full', 'valid', 'same' and 'sameshift'.
             Defaults to 'sameshift'.
 
     Returns:
         torch.Tensor: A sparse fwt analysis matrix.
             The matrices are ordered a,h,v,d or
             ll, lh, hl, hh.
 
     Note:
-        The construced matrix is NOT necessary orthogonal.
-        In most cases construct_boundary_a2d should be used instead.
+        The constructed matrix is NOT necessarily orthogonal.
+        In most cases, construct_boundary_a2d should be used instead.
 
     """
-    dec_lo, dec_hi, _, _ = get_filter_tensors(
+    dec_lo, dec_hi, _, _ = _get_filter_tensors(
         wavelet, flip=False, device=device, dtype=dtype
     )
-    dec_filt = construct_2d_filt(lo=dec_lo, hi=dec_hi)
+    dec_filt = _construct_2d_filt(lo=dec_lo, hi=dec_hi)
     ll, lh, hl, hh = dec_filt.squeeze(1)
     analysis_ll = construct_strided_conv2d_matrix(ll, height, width, mode=mode)
     analysis_lh = construct_strided_conv2d_matrix(lh, height, width, mode=mode)
     analysis_hl = construct_strided_conv2d_matrix(hl, height, width, mode=mode)
     analysis_hh = construct_strided_conv2d_matrix(hh, height, width, mode=mode)
     analysis = torch.cat([analysis_ll, analysis_lh, analysis_hl, analysis_hh], 0)
     return analysis
@@ -77,40 +84,40 @@
     device: Union[torch.device, str],
     dtype: torch.dtype = torch.float64,
     mode: str = "sameshift",
 ) -> torch.Tensor:
     """Construct a raw fast wavelet transformation synthesis matrix.
 
     Note:
-        The construced matrix is NOT necessary orthogonal.
-        In most cases construct_boundary_s2d should be used instead.
+        The constructed matrix is NOT necessarily orthogonal.
+        In most cases, construct_boundary_s2d should be used instead.
 
     Args:
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         height (int): The height of the input image, which was originally
             transformed.
         width (int): The width of the input image, which was originally
             transformed.
-        device ([type]): Where to place the synthesis matrix,
-            usually cpu or gpu.
-        dtype ([type], optional): The data-type the matrix should have.
+        device (torch.device): Where to place the synthesis matrix,
+            usually CPU or GPU.
+        dtype (torch.dtype, optional): The data type the matrix should have.
             Defaults to torch.float64.
         mode (str): The convolution type.
             Options are 'full', 'valid', 'same' and 'sameshift'.
             Defaults to 'sameshift'.
 
     Returns:
         [torch.Tensor]: The generated fast wavelet synthesis matrix.
     """
     wavelet = _as_wavelet(wavelet)
-    _, _, rec_lo, rec_hi = get_filter_tensors(
+    _, _, rec_lo, rec_hi = _get_filter_tensors(
         wavelet, flip=True, device=device, dtype=dtype
     )
-    dec_filt = construct_2d_filt(lo=rec_lo, hi=rec_hi)
+    dec_filt = _construct_2d_filt(lo=rec_lo, hi=rec_hi)
     ll, lh, hl, hh = dec_filt.squeeze(1)
     synthesis_ll = construct_strided_conv2d_matrix(ll, height, width, mode=mode)
     synthesis_lh = construct_strided_conv2d_matrix(lh, height, width, mode=mode)
     synthesis_hl = construct_strided_conv2d_matrix(hl, height, width, mode=mode)
     synthesis_hh = construct_strided_conv2d_matrix(hh, height, width, mode=mode)
     synthesis = torch.cat(
         [synthesis_ll, synthesis_lh, synthesis_hl, synthesis_hh], 0
@@ -141,15 +148,15 @@
             Should be divisible by two.
         width (int): The width of the input matrix.
             Should be divisible by two.
         device (torch.device): Where to place the matrix. Either on
             the CPU or GPU.
         boundary (str): The method to use for matrix orthogonalization.
             Choose "qr" or "gramschmidt". Defaults to "qr".
-        dtype (torch.dtype, optional): The desired data-type for the matrix.
+        dtype (torch.dtype, optional): The desired data type for the matrix.
             Defaults to torch.float64.
 
     Returns:
         torch.Tensor: A sparse fwt matrix, with orthogonalized boundary
             wavelets.
     """
     wavelet = _as_wavelet(wavelet)
@@ -172,15 +179,15 @@
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         height (int): The original height of the input matrix.
         width (int): The width of the original input matrix.
         device (torch.device): Choose CPU or GPU.
         boundary (str): The method to use for matrix orthogonalization.
             Choose qr or gramschmidt. Defaults to qr.
-        dtype (torch.dtype, optional): The data-type of the
+        dtype (torch.dtype, optional): The data type of the
             sparse matrix, choose float32 or 64.
             Defaults to torch.float64.
 
     Returns:
         torch.Tensor: The synthesis matrix, used to compute the
             inverse fast wavelet transform.
     """
@@ -202,29 +209,29 @@
         pad_tuple = (True, pad_tuple[1])
     return height, width, pad_tuple
 
 
 class MatrixWavedec2(object):
     """Experimental sparse matrix 2d wavelet transform.
 
-        For a completely pad free transform,
+        For a completely pad-free transform,
         input images are expected to be divisible by two.
         For multiscale transforms all intermediate
         scale dimensions should be divisible
         by two, i.e. 128, 128 -> 64, 64 -> 32, 32 would work
         well for a level three transform.
         In this case multiplication with the `sparse_fwt_operator`
         property is equivalent.
 
     Note:
         Constructing the sparse fwt-matrix is expensive.
-        For longer wavelets, high level transforms, and large
+        For longer wavelets, high-level transforms, and large
         input images this may take a while.
         The matrix is therefore constructed only once.
-        In the non separable case, it can be accessed via
+        In the non-separable case, it can be accessed via
         the sparse_fwt_operator property.
 
     Example:
         >>> import ptwt, torch, pywt
         >>> import numpy as np
         >>> from scipy import datasets
         >>> face = datasets.face()[:256, :256, :].astype(np.float32)
@@ -246,29 +253,29 @@
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             level (int, optional): The level up to which to compute the fwt. If None,
                 the maximum level based on the signal length is chosen. Defaults to
                 None.
             boundary (str): The method used for boundary filter treatment.
-                Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's
+                Choose 'qr' or 'gramschmidt'. 'qr' relies on Pytorch's
                 dense qr implementation, it is fast but memory hungry.
                 The 'gramschmidt' option is sparse, memory efficient,
                 and slow.
                 Choose 'gramschmidt' if 'qr' runs out of memory.
                 Defaults to 'qr'.
             separable (bool): If this flag is set, a separable transformation
                 is used, i.e. a 1d transformation along each axis.
                 Matrix construction is significantly faster for separable
                 transformations since only a small constant-size part of the
                 matrices must be orthogonalized. Defaults to True.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
-            ValueError: If the wavelet filters have different lenghts.
+            ValueError: If the wavelet filters have different lengths.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.level = level
         self.boundary = boundary
         self.separable = separable
         self.input_signal_shape: Optional[Tuple[int, int]] = None
         self.fwt_matrix_list: List[
@@ -340,15 +347,15 @@
             if current_height < filt_len or current_width < filt_len:
                 # we have reached the max decomposition depth.
                 sys.stderr.write(
                     f"Warning: The selected number of decomposition levels {self.level}"
                     f" is too large for the given input shape {self.input_signal_shape}"
                     f". At level {curr_level}, at least one of the current signal "
                     f"height and width ({current_height}, {current_width}) is smaller "
-                    f"than the filter length {filt_len}. Therefore, the transformation "
+                    f"then the filter length {filt_len}. Therefore, the transformation "
                     f"is only computed up to the decomposition level {curr_level-1}.\n"
                 )
                 break
             # the conv matrices require even length inputs.
             current_height, current_width, pad_tuple = _matrix_pad_2(
                 current_height, current_width
             )
@@ -394,42 +401,47 @@
         """Compute the fwt for the given input signal.
 
         The fwt matrix is set up during the first call
         and stored for future use.
 
         Args:
             input_signal (torch.Tensor): An input signal of shape
-                [batch_size, height, width].
-                2d inputs are interpreted as [height, width].
-                Inputs of the form [batch_size, 1, height, width] are squeezed.
+                ``[batch_size, height, width]``.
+                2d inputs are interpreted as ``[height, width]``.
+                4d inputs as ``[batch_size, channels, height, width]``.
+                This transform affects the last two dimensions.
 
         Returns:
-            (list): The resulting coefficients per level stored in
+            (list): The resulting coefficients per level are stored in
             a pywt style list. The list is ordered as::
 
                 (ll, (lh, hl, hh), ...)
 
-            with 'l' for low-pass and 'h' for high pass filters.
+            with 'l' for low-pass and 'h' for high-pass filters.
 
         Raises:
             ValueError: If the decomposition level is not a positive integer
                 or if the input signal has not the expected shape.
         """
+        fold = False
         if input_signal.dim() == 2:
             # add batch dim to unbatched input
             input_signal = input_signal.unsqueeze(0)
-        elif input_signal.dim() == 4 and input_signal.size(1) == 1:
+        elif input_signal.dim() == 4:
             # we assume the shape [batch_size, color_channels, height, width]
-            # and squeeze the single color channel
-            input_signal = input_signal.squeeze(1)
+            # and fold the color channel
+            fold = True
+            ds = input_signal.shape
+            input_signal = _fold_channels(input_signal)
         elif input_signal.dim() != 3:
             raise ValueError(
                 f"Invalid input tensor shape {input_signal.size()}. "
                 "The input signal is expected to be of the form "
-                "[batch_size, height, width]."
+                "[batch_size, height, width] or "
+                "[batch_size, channels, height, width]."
             )
 
         batch_size, height, width = input_signal.shape
 
         if not _is_dtype_supported(input_signal.dtype):
             raise ValueError(f"Input dtype {input_signal.dtype} not supported")
 
@@ -522,14 +534,18 @@
                     ),
                 )
                 split_list.append(reshaped)
                 ll = four_split[0]
             split_list.append(
                 ll.T.reshape(batch_size, size[1] // 2, size[0] // 2).transpose(2, 1)
             )
+
+        if fold:
+            split_list = _wavedec2d_unfold_channels_2d_list(split_list, list(ds))
+
         return split_list[::-1]
 
 
 class MatrixWaverec2(object):
     """Synthesis or inverse matrix based-wavelet transformation object.
 
     Example:
@@ -546,34 +562,34 @@
 
     def __init__(
         self,
         wavelet: Union[Wavelet, str],
         boundary: str = "qr",
         separable: bool = True,
     ):
-        """Create the inverse matrix based fast wavelet transformation.
+        """Create the inverse matrix-based fast wavelet transformation.
 
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             boundary (str): The method used for boundary filter treatment.
                 Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's dense qr
                 implementation, it is fast but memory hungry. The 'gramschmidt' option
                 is sparse, memory efficient, and slow. Choose 'gramschmidt' if 'qr' runs
                 out of memory. Defaults to 'qr'.
             separable (bool): If this flag is set, a separable transformation
                 is used, i.e. a 1d transformation along each axis. This is significantly
                 faster than a non-separable transformation since only a small constant-
                 size part of the matrices must be orthogonalized.
-                For invertability the analysis and synthesis values must be identical!
+                For invertibility, the analysis and synthesis values must be identical!
                 Defaults to True.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
-            ValueError: If the wavelet filters have different lenghts.
+            ValueError: If the wavelet filters have different lengths.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.boundary = boundary
         self.separable = separable
 
         self.ifwt_matrix_list: List[
             Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]
@@ -590,15 +606,15 @@
             raise ValueError("All filters must have the same length")
 
     @property
     def sparse_ifwt_operator(self) -> torch.Tensor:
         """Compute the ifwt operator matrix for pad-free cases.
 
         Returns:
-            torch.Tensor: The sparse 2d-ifwt operator matrix.
+            torch.Tensor: The sparse 2d ifwt operator matrix.
 
         Raises:
             NotImplementedError: if a separable transformation was used or if padding
                 had to be used in the creation of the transformation matrices.
             ValueError: If no level transformation matrices are stored (most likely
                 since the object was not called yet).
         """
@@ -643,15 +659,15 @@
         for curr_level in range(1, self.level + 1):
             if current_height < filt_len or current_width < filt_len:
                 sys.stderr.write(
                     f"Warning: The selected number of decomposition levels {self.level}"
                     f" is too large for the given input shape {self.input_signal_shape}"
                     f". At level {curr_level}, at least one of the current signal "
                     f"height and width ({current_height}, {current_width}) is smaller "
-                    f"than the filter length {filt_len}. Therefore, the transformation "
+                    f"then the filter length {filt_len}. Therefore, the transformation "
                     f"is only computed up to the decomposition level {curr_level-1}.\n"
                 )
                 break
             current_height, current_width, pad_tuple = _matrix_pad_2(
                 current_height, current_width
             )
             if any(pad_tuple):
@@ -697,21 +713,31 @@
 
         Args:
             coefficients (list): The coefficient list as returned
                 by the `MatrixWavedec2`-Object.
 
         Returns:
             torch.Tensor: The original signal reconstruction of
-                shape [batch_size, height, width].
+                shape ``[batch_size, height, width]`` or
+                ``[batch_size, channels, height, width]``
+                depending on the input to the forward transform.
 
         Raises:
             ValueError: If the decomposition level is not a positive integer or if the
                 coefficients are not in the shape as it is returned from a
                 `MatrixWavedec2` object.
         """
+        ll = _check_if_tensor(coefficients[0])
+        fold = False
+        if ll.dim() == 4:
+            # fold all channels into the batches.
+            fold = True
+            coefficients, ds = _waverec2d_fold_channels_2d_list(coefficients)
+            ll = _check_if_tensor(coefficients[0])
+
         level = len(coefficients) - 1
         height, width = tuple(c * 2 for c in coefficients[-1][0].shape[-2:])
 
         re_build = False
         if (
             self.input_signal_shape is None
             or self.input_signal_shape[0] != height
@@ -720,20 +746,14 @@
             self.input_signal_shape = height, width
             re_build = True
 
         if self.level != level:
             self.level = level
             re_build = True
 
-        ll = coefficients[0]
-        if not isinstance(ll, torch.Tensor):
-            raise ValueError(
-                "First element of coeffs must be the approximation coefficient tensor."
-            )
-
         batch_size = ll.shape[0]
         torch_device = ll.device
         torch_dtype = ll.dtype
 
         if not _is_dtype_supported(torch_dtype):
             raise ValueError(f"Input dtype {torch_dtype} not supported")
 
@@ -801,8 +821,11 @@
                 next_len = list(coefficients[c_pos + 2][0].shape[-2:])
                 if pred_len != next_len:
                     if pred_len[0] != next_len[0]:
                         ll = ll[:, :-1, :]
                     if pred_len[1] != next_len[1]:
                         ll = ll[:, :, :-1]
 
+        if fold:
+            ll = _unfold_channels(ll, list(ds))
+
         return ll
```

### Comparing `ptwt-0.1.5/src/ptwt/matmul_transform_3.py` & `ptwt-0.1.6/src/ptwt/matmul_transform_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 # we have reached the max decomposition depth.
                 sys.stderr.write(
                     f"Warning: The selected number of decomposition levels {self.level}"
                     f" is too large for the given input shape {self.input_signal_shape}"
                     f". At level {curr_level}, at least one of the current signal "
                     f"depth, height, and width ({current_depth}, {current_height},"
                     f"{current_width}) is smaller "
-                    f"than the filter length {filt_len}. Therefore, the transformation "
+                    f"then the filter length {filt_len}. Therefore, the transformation "
                     f"is only computed up to the decomposition level {curr_level-1}.\n"
                 )
                 break
             # the conv matrices require even length inputs.
             current_depth, current_height, current_width, pad_tuple = _matrix_pad_3(
                 depth=current_depth, height=current_height, width=current_width
             )
@@ -145,15 +145,15 @@
         """Compute a separable 3d-boundary wavelet transform.
 
         Args:
             input_signal (torch.Tensor): An input signal of shape
                 [batch_size, depth, height, width].
 
         Raises:
-            ValueError: If the input dimensions dont work.
+            ValueError: If the input dimensions don't work.
 
         Returns:
             List[Union[torch.Tensor, TypedDict[str, torch.Tensor]]]:
                 A list with the approximation coefficients,
                 and a coefficient dict for each scale.
         """
         if input_signal.dim() == 3:
@@ -255,15 +255,15 @@
     ):
         """Compute a three-dimensional separable boundary wavelet synthesis transform.
 
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             boundary (str): The method used for boundary filter treatment.
-                Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's dense qr
+                Choose 'qr' or 'gramschmidt'. 'qr' relies on Pytorch's dense qr
                 implementation, it is fast but memory hungry. The 'gramschmidt' option
                 is sparse, memory efficient, and slow. Choose 'gramschmidt' if 'qr' runs
                 out of memory. Defaults to 'qr'.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
             ValueError: If the wavelet filters have different lengths.
@@ -350,15 +350,15 @@
             else:
                 return cat_tensor
         return self._cat_coeff_recursive(done_dict)
 
     def __call__(
         self, coefficients: List[Union[torch.Tensor, Dict[str, torch.Tensor]]]
     ) -> torch.Tensor:
-        """Reconstruct a batched 3d-signal from it's coefficients.
+        """Reconstruct a batched 3d-signal from its coefficients.
 
         Args:
             coefficients (List[Union[torch.Tensor, Dict[str, torch.Tensor]]]):
                 The output from MatrixWavedec3.
 
         Returns:
             torch.Tensor: A reconstruction of the original signal.
```

### Comparing `ptwt-0.1.5/src/ptwt/packets.py` & `ptwt-0.1.6/src/ptwt/packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,31 +38,32 @@
     """
     n = np.array(range(int(np.power(2.0, level))))
     freqs = (fs / 2.0) * (n / (np.power(2.0, level)))
     return list(freqs)
 
 
 class WaveletPacket(BaseDict):
-    """One dimensional wavelet packets."""
+    """Implements a single-dimensional wavelet packets analysis transform."""
 
     def __init__(
         self,
         data: Optional[torch.Tensor],
         wavelet: Union[Wavelet, str],
         mode: str = "reflect",
         boundary_orthogonalization: str = "qr",
         maxlevel: Optional[int] = None,
     ) -> None:
         """Create a wavelet packet decomposition object.
 
         The decompositions will rely on padded fast wavelet transforms.
 
         Args:
-            data (torch.Tensor, optional): The input data array of shape [time]
-                or [batch_size, time]. If None, the object is initialized without
+            data (torch.Tensor, optional): The input data array of shape ``[time]``,
+                ``[batch_size, time]`` or ``[batch_size, channels, time]``.
+                If None, the object is initialized without
                 performing a decomposition.
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             mode (str): The desired padding method. If you select 'boundary',
                 the sparse matrix backend will be used. Defaults to 'reflect'.
             boundary_orthogonalization (str): The orthogonalization method
                 to use. Only used if `mode` equals 'boundary'. Choose from
@@ -120,20 +121,20 @@
         self.maxlevel = maxlevel
         self._recursive_dwt(data, level=0, path="")
         return self
 
     def reconstruct(self) -> "WaveletPacket":
         """Recursively reconstruct the input starting from the leaf nodes.
 
-        Reconstruction replaces the input-data originally assigned to this object.
+        Reconstruction replaces the input data originally assigned to this object.
 
         Note:
-           Only changes to leaf node data impacts the results,
+           Only changes to leaf node data impact the results,
            since changes in all other nodes will be replaced with
-           a reconstruction from the leafs.
+           a reconstruction from the leaves.
 
         Example:
             >>> import numpy as np
             >>> import ptwt, torch
             >>> signal = np.random.randn(1, 16)
             >>> ptwp = ptwt.WaveletPacket(torch.from_numpy(signal), "haar",
             >>>     mode="boundary", maxlevel=2)
@@ -181,15 +182,15 @@
                     self.wavelet, boundary=self.boundary
                 )
             return self._matrix_waverec_dict[length]
         else:
             return partial(waverec, wavelet=self.wavelet)
 
     def get_level(self, level: int) -> List[str]:
-        """Return the graycode ordered paths to the filter tree nodes.
+        """Return the graycode-ordered paths to the filter tree nodes.
 
         Args:
             level (int): The depth of the tree.
 
         Returns:
             list: A list with the paths to each node.
         """
@@ -216,15 +217,15 @@
             self._recursive_dwt(res_lo, level + 1, path + "a")
             self._recursive_dwt(res_hi, level + 1, path + "d")
 
     def __getitem__(self, key: str) -> torch.Tensor:
         """Access the coefficients in the wavelet packets tree.
 
         Args:
-            key (str): The key of the accessed coefficents. The string may only consist
+            key (str): The key of the accessed coefficients. The string may only consist
                 of the following chars: 'a', 'd'.
 
         Returns:
             torch.Tensor: The accessed wavelet packet coefficients.
 
         Raises:
             ValueError: If the wavelet packet tree is not initialized.
@@ -241,15 +242,15 @@
                 "cannot be accessed! This wavelet packet tree is initialized with "
                 f"maximum level {self.maxlevel}."
             )
         return super().__getitem__(key)
 
 
 class WaveletPacket2D(BaseDict):
-    """Two dimensional wavelet packets.
+    """Two-dimensional wavelet packets.
 
     Example code illustrating the use of this class is available at:
     https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/deepfake_analysis
     """
 
     def __init__(
         self,
@@ -260,16 +261,18 @@
         separable: bool = False,
         maxlevel: Optional[int] = None,
     ) -> None:
         """Create a 2D-Wavelet packet tree.
 
         Args:
             data (torch.tensor, optional): The input data tensor
-                of shape [batch_size, height, width].  If None, the object
-                is initialized without performing a decomposition.
+                of shape ``[batch_size, height, width]`` or
+                ``[batch_size, channels, height, width]``.
+                If None, the object is initialized without performing
+                a decomposition.
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             mode (str): A string indicating the desired padding mode.
                 If you select 'boundary', the sparse matrix backend is used.
                 Defaults to 'reflect'
             boundary_orthogonalization (str): The orthogonalization method
                 to use in the sparse matrix backend. Only used if `mode`
@@ -320,17 +323,17 @@
         self._recursive_dwt2d(data, level=0, path="")
         return self
 
     def reconstruct(self) -> "WaveletPacket2D":
         """Recursively reconstruct the input starting from the leaf nodes.
 
         Note:
-           Only changes to leaf node data impacts the results,
+           Only changes to leaf node data impact the results,
            since changes in all other nodes will be replaced with
-           a reconstruction from the leafs.
+           a reconstruction from the leaves.
         """
         if self.maxlevel is None:
             self.maxlevel = pywt.dwt_max_level(
                 min(self[""].shape[-2:]), self.wavelet.dec_len
             )
 
         for level in reversed(range(self.maxlevel)):
@@ -342,20 +345,20 @@
                 rec = self._get_waverec(data_a.shape[-2:])(
                     [data_a, (data_h, data_v, data_d)]
                 )
                 if level > 0:
                     if rec.shape[-1] != self[node].shape[-1]:
                         assert (
                             rec.shape[-1] == self[node].shape[-1] + 1
-                        ), "padding error, please open an issue on github"
+                        ), "padding error, please open an issue on GitHub"
                         rec = rec[..., :-1]
                     if rec.shape[-2] != self[node].shape[-2]:
                         assert (
                             rec.shape[-2] == self[node].shape[-2] + 1
-                        ), "padding error, please open an issue on github"
+                        ), "padding error, please open an issue on GitHub"
                         rec = rec[..., :-1, :]
                 self[node] = rec
         return self
 
     def get_natural_order(self, level: int) -> List[str]:
         """Get the natural ordering for a given decomposition level.
 
@@ -469,15 +472,16 @@
             self._recursive_dwt2d(result_v, level + 1, path + "v")
             self._recursive_dwt2d(result_d, level + 1, path + "d")
 
     def __getitem__(self, key: str) -> torch.Tensor:
         """Access the coefficients in the wavelet packets tree.
 
         Args:
-            key (str): The key of the accessed coefficents. The string may only consist
+            key (str): The key of the accessed coefficients.
+                The string may only consist
                 of the following chars: 'a', 'h', 'v', 'd'.
 
         Returns:
             torch.Tensor: The accessed wavelet packet coefficients.
 
         Raises:
             ValueError: If the wavelet packet tree is not initialized.
```

### Comparing `ptwt-0.1.5/src/ptwt/separable_conv_transform.py` & `ptwt-0.1.6/src/ptwt/separable_conv_transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""Implement separable convolution based transforms.
+"""Implement separable convolution-based transforms.
 
 Under the hood code in this module transforms all dimensions
 individually using torch.nn.functional.conv1d and it's
 transpose.
 """
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pywt
 import torch
 
-from ._util import _as_wavelet
+from ._util import _as_wavelet, _fold_channels, _unfold_channels
 from .conv_transform import wavedec, waverec
 
 
 def _separable_conv_dwtn_(
     rec_dict: Dict[str, torch.Tensor],
     input: torch.Tensor,
     wavelet: Union[str, pywt.Wavelet],
     mode: str = "reflect",
     key: str = "",
 ) -> None:
-    """Compute a single level separable fast wavelet transform.
+    """Compute a single-level separable fast wavelet transform.
 
     All but the first axes are transformed.
 
     Args:
         input (torch.Tensor): Tensor of shape [batch, data_1, ... data_n].
         wavelet (Union[str, pywt.Wavelet]): The Wavelet to work with.
         mode (str): The padding mode. The following methods are supported::
@@ -150,98 +150,53 @@
         wavelet (Union[str, pywt.Wavelet]):
             The wavelet used by `_separable_conv_wavedecn`.
 
     Returns:
         torch.Tensor: The reconstruction of the original signal.
 
     Raises:
-        ValueError: If the coeff_list is no not structured as expected.
+        ValueError: If the coeff_list is not structured as expected.
     """
     if not isinstance(coeff_list[0], torch.Tensor):
         raise ValueError("approximation tensor must be first in coefficient list.")
     if not all(map(lambda x: isinstance(x, dict), coeff_list[1:])):
         raise ValueError("All entries after approximation tensor must be dicts.")
 
     approx: torch.Tensor = coeff_list[0]
     for level_dict in coeff_list[1:]:
         keys = list(level_dict.keys())  # type: ignore
         level_dict["a" * max(map(len, keys))] = approx  # type: ignore
         approx = _separable_conv_idwtn(level_dict, wavelet)  # type: ignore
     return approx
 
 
-def _fswavedec(
-    input: torch.Tensor,
-    wavelet: Union[str, pywt.Wavelet],
-    mode: str = "reflect",
-    level: Optional[int] = None,
-) -> List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
-    """Compute a fully separable 1D-padded analysis wavelet transform.
-
-       This function is private. Results are the identical to wavedec.
-       Use wavedec instead.
-
-    Args:
-        input (torch.Tensor): An input signal of shape [batch, length].
-        wavelet (Wavelet or str): A pywt wavelet compatible object or
-            the name of a pywt wavelet. Refer to the output of
-            ``pywt.wavelist(kind="discrete")`` for a list of possible choices.
-        mode (str): The padding mode. Options are::
-
-                "reflect", "zero", "constant", "periodic".
-
-            This function defaults to "reflect".
-        level (int): The number of desired scales.
-            Defaults to None.
-
-
-    Raises:
-        ValueError: If the input is not a batched 1d-signal.
-
-    Returns:
-        List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
-            The transformed signal.
-
-    Example:
-        >>> import torch
-        >>> import ptwt
-        >>> data = torch.randn(5,10)
-        >>> coeff = ptwt.fswavedec(data, "haar", level=2)
-
-    """
-    if len(input.shape) == 1:
-        input = input.unsqueeze(0)
-    if len(input.shape) != 2:
-        raise ValueError("Batched 1d inputs required for a 1d transform.")
-    return _separable_conv_wavedecn(input, wavelet, mode, level)
-
-
 def fswavedec2(
     input: torch.Tensor,
     wavelet: Union[str, pywt.Wavelet],
     mode: str = "reflect",
     level: Optional[int] = None,
 ) -> List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
     """Compute a fully separable 2D-padded analysis wavelet transform.
 
     Args:
-        input (torch.Tensor): An input signal of shape [batch, height, width].
+        input (torch.Tensor): An input signal of shape ``[batch, height, width]``
+            or ``[batch, channels, height, width]``.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet. Refer to the output of
             ``pywt.wavelist(kind="discrete")`` for a list of possible choices.
         mode (str): The padding mode. Options are::
 
                 "reflect", "zero", "constant", "periodic".
 
             This function defaults to "reflect".
         level (int): The number of desired scales.
             Defaults to None.
 
     Raises:
-        ValueError: If the input is not a batched 2d-signal.
+        ValueError: If the input is not a batched 2D signal.
 
     Returns:
         List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
         A list with the lll coefficients and dictionaries
         with the filter order strings::
 
         ("ad", "da", "dd")
@@ -253,19 +208,38 @@
     Example:
         >>> import torch
         >>> import ptwt
         >>> data = torch.randn(5, 10, 10)
         >>> coeff = ptwt.fswavedec2(data, "haar", level=2)
 
     """
+    fold = False
     if len(input.shape) == 2:
         input = input.unsqueeze(0)
-    if len(input.shape) != 3:
+    elif input.dim() == 4:
+        # fold channels into batches.
+        fold = True
+        ds = list(input.shape)
+        input = _fold_channels(input)
+    elif len(input.shape) != 3:
         raise ValueError("Batched 2d inputs required for a 2d transform.")
-    return _separable_conv_wavedecn(input, wavelet, mode, level)
+    res = _separable_conv_wavedecn(input, wavelet, mode, level)
+
+    if fold:
+        unfold: List[Union[torch.Tensor, Dict[str, torch.Tensor]]] = []
+        for resel in res:
+            if isinstance(resel, torch.Tensor):
+                unfold.append(_unfold_channels(resel, ds))
+            else:
+                unfold.append(
+                    {key: _unfold_channels(value, ds) for key, value in resel.items()}
+                )
+        res = unfold
+
+    return res
 
 
 def fswavedec3(
     input: torch.Tensor,
     wavelet: Union[str, pywt.Wavelet],
     mode: str = "reflect",
     level: Optional[int] = None,
@@ -282,15 +256,15 @@
                 "reflect", "zero", "constant", "periodic".
 
             This function defaults to "reflect".
         level (int): The number of desired scales.
             Defaults to None.
 
     Raises:
-        ValueError: If the input is not a batched 3d-signal.
+        ValueError: If the input is not a batched 3D signal.
 
     Returns:
         List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
         A list with the lll coefficients and dictionaries
         with the filter order strings::
 
         ("aad", "ada", "add", "daa", "dad", "dda", "ddd")
@@ -308,40 +282,14 @@
         input = input.unsqueeze(0)
     if len(input.shape) != 4:
         raise ValueError("Batched 3d inputs required for a 3d transform.")
 
     return _separable_conv_wavedecn(input, wavelet, mode, level)
 
 
-def _fswaverec(
-    coeff_list: List[Union[torch.Tensor, Dict[str, torch.Tensor]]],
-    wavelet: Union[str, pywt.Wavelet],
-) -> torch.Tensor:
-    """Compute a fully separable 1D-padded synthesis wavelet transform.
-
-    Args:
-        coeff_list (List[Union[torch.Tensor, Dict[str, torch.Tensor]]]):
-            The wavelet coefficients as computed by `fswavedec`.
-        wavelet (Union[str, pywt.Wavelet]): The wavelet to use for the
-            synthesis transform.
-
-    Returns:
-        torch.Tensor: A reconstruction of the signal encoded in the
-            wavelet coefficients.
-
-    Example:
-        >>> import torch
-        >>> import ptwt
-        >>> data = torch.randn(5,10)
-        >>> coeff = ptwt.fswavedec(data, "haar", level=2)
-        >>> rec = ptwt.fswaverec(coeff, "haar")
-    """
-    return _separable_conv_waverecn(coeff_list, wavelet)
-
-
 def fswaverec2(
     coeff_list: List[Union[torch.Tensor, Dict[str, torch.Tensor]]],
     wavelet: Union[str, pywt.Wavelet],
 ) -> torch.Tensor:
     """Compute a fully separable 2D-padded synthesis wavelet transform.
 
     Args:
```

### Comparing `ptwt-0.1.5/src/ptwt/sparse_math.py` & `ptwt-0.1.6/src/ptwt/sparse_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         sparse_tensor_a.to_dense(), sparse_tensor_b.to_dense()
     ).to_sparse()
 
 
 def sparse_kron(
     sparse_tensor_a: torch.Tensor, sparse_tensor_b: torch.Tensor
 ) -> torch.Tensor:
-    """Compute a sparse kronecker product.
+    """Compute a sparse Kronecker product.
 
     As defined at:
     https://en.wikipedia.org/wiki/Kronecker_product
     Adapted from:
     https://github.com/scipy/scipy/blob/v1.7.1/scipy/sparse/construct.py#L274-L357
 
     Args:
@@ -103,16 +103,16 @@
     Returns:
         torch.Tensor: Square [input, eye] matrix
             of size [new_length, new_length]
     """
     # assert square matrix.
     assert (
         sparse_matrix.shape[0] == sparse_matrix.shape[1]
-    ), "Matrices must be square. Odd inputs can cause to non-square matrices."
-    assert new_length > sparse_matrix.shape[0], "cant add negatively many entries."
+    ), "Matrices must be square. Odd inputs can cause non-square matrices."
+    assert new_length > sparse_matrix.shape[0], "can't add negatively many entries."
     x = torch.arange(
         sparse_matrix.shape[0],
         new_length,
         dtype=sparse_matrix.dtype,
         device=sparse_matrix.device,
     )
     y = torch.arange(
@@ -134,28 +134,29 @@
     )
     return new_matrix
 
 
 def sparse_diag(
     diagonal: torch.Tensor, col_offset: int, rows: int, cols: int
 ) -> torch.Tensor:
-    """Create a rows-by-cols sparse diagnoal-matrix.
+    """Create a rows-by-cols sparse diagonal-matrix.
 
-    The matrix is construced by taking the columns of Bin and
-    placing them along the diagonal specified by col_offset.
+    The matrix is constructed by taking the columns of the
+    input and placing them along the diagonal
+    specified by col_offset.
 
     Args:
         diagonal (torch.Tensor): The values for the diagonal.
         col_offset (int): Move the diagonal to the right by
             offset columns.
         rows (int): The number of rows in the final matrix.
         cols (int): The number of columns in the final matrix.
 
     Returns:
-        torch.Tensor: A sparse matrix with a shifted diaginal.
+        torch.Tensor: A sparse matrix with a shifted diagonal.
 
     """
     diag_indices = torch.stack(
         [
             torch.arange(len(diagonal), device=diagonal.device),
             torch.arange(len(diagonal), device=diagonal.device),
         ]
@@ -189,26 +190,26 @@
     matrix: torch.Tensor, row_index: int, row: torch.Tensor
 ) -> torch.Tensor:
     """Replace a row within a sparse [rows, cols] matrix.
 
     I.e. matrix[row_no, :] = row.
 
     Args:
-        matrix (torch.Tensor): A sparse two dimensional matrix.
+        matrix (torch.Tensor): A sparse two-dimensional matrix.
         row_index (int): The row to replace.
         row (torch.Tensor): The row to insert into the sparse matrix.
 
     Returns:
         torch.Tensor: A sparse matrix, with the new row inserted at
         row_index.
     """
     matrix = matrix.coalesce()
     assert (
         matrix.shape[-1] == row.shape[-1]
-    ), "matrix and replacement-row must share the same column number."
+    ), "matrix and replacement row must share the same column number."
 
     # delete existing indices we dont want
     diag_indices = torch.arange(matrix.shape[0])
     diag = torch.ones_like(diag_indices)
     diag[row_index] = 0
     removal_matrix = torch.sparse_coo_tensor(
         torch.stack([diag_indices] * 2, 0),
@@ -231,15 +232,15 @@
 
 
 def _orth_by_qr(
     matrix: torch.Tensor, rows_to_orthogonalize: torch.Tensor
 ) -> torch.Tensor:
     """Orthogonalize a wavelet matrix through qr decomposition.
 
-    A dense qr-decomposition is used for gpu-efficiency reasons.
+    A dense qr-decomposition is used for GPU-efficiency reasons.
     If memory becomes a constraint choose _orth_by_gram_schmidt
     instead, which is implemented using only sparse function calls.
 
     Args:
         matrix (torch.Tensor): The matrix to orthogonalize.
         rows_to_orthogonalize (torch.Tensor): The matrix rows, which need work.
 
@@ -334,17 +335,17 @@
 
     Full, valid and same, padding are supported.
     For reference see:
     https://github.com/RoyiAvital/StackExchangeCodes/blob/\
     master/StackOverflow/Q2080835/CreateConvMtxSparse.m
 
     Args:
-        filter (torch.tensor): The 1d-filter to convolve with.
+        filter (torch.tensor): The 1D-filter to convolve with.
         input_rows (int): The number of columns in the input.
-        mode (str): String indetifier for the desired padding.
+        mode (str): String identifier for the desired padding.
             Choose 'full', 'valid' or 'same'.
             Defaults to valid.
 
     Returns:
         torch.Tensor: The sparse convolution tensor.
 
     Raises:
@@ -493,15 +494,15 @@
     input_columns: int,
     stride: int = 2,
     mode: str = "full",
 ) -> torch.Tensor:
     """Create a strided sparse two dimensional convolution matrix.
 
     Args:
-        filter (torch.Tensor): The two dimensional convolution filter.
+        filter (torch.Tensor): The two-dimensional convolution filter.
         input_rows (int): The number of rows in the 2d-input matrix.
         input_columns (int): The number of columns in the 2d- input matrix.
         stride (int): The stride between the filter positions.
             Defaults to 2.
         mode (str): The convolution type.
             Options are 'full', 'valid', 'same' and 'sameshift'.
             Defaults to 'full'. Sameshift starts at 1 instead of 0.
```

### Comparing `ptwt-0.1.5/src/ptwt/version.py` & `ptwt-0.1.6/src/ptwt/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 import os
 from subprocess import CalledProcessError, check_output  # noqa: S404
 
 __all__ = [
     "VERSION",
     "get_version",
-    "get_git_hash",
+    "_get_git_hash",
 ]
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 
 
-def get_git_hash() -> str:
+def _get_git_hash() -> str:
     """Get the :mod:`ptwt` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
                 ["git", "rev-parse", "HEAD"],
                 cwd=os.path.dirname(__file__),
                 stderr=devnull,
@@ -30,12 +30,12 @@
             return "UNHASHED"
         else:
             return ret.strip().decode("utf-8")[:8]
 
 
 def get_version(with_git_hash: bool = False) -> str:
     """Get the :mod:`ptwt` version string, including a git hash."""
-    return f"{VERSION}-{get_git_hash()}" if with_git_hash else VERSION
+    return f"{VERSION}-{_get_git_hash()}" if with_git_hash else VERSION
 
 
 if __name__ == "__main__":
     print(get_version(with_git_hash=True))
```

### Comparing `ptwt-0.1.5/src/ptwt/wavelets_learnable.py` & `ptwt-0.1.6/src/ptwt/wavelets_learnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import torch
 
 
 class WaveletFilter(ABC):
     """Interface for learnable wavelets.
 
-    Each wavelet has a filter bank a loss function
-    and comes with functionality the test the perfect
+    Each wavelet has a filter bank loss function
+    and comes with functionality that tests the perfect
     reconstruction and anti-aliasing conditions.
     """
 
     @property
     @abstractmethod
     def filter_bank(
         self,
@@ -48,15 +48,15 @@
 
         See: Strang+Nguyen 105: F0(z) = H1(-z); F1(z) = -H0(-z)
         Alternating sign convention from 0 to N see Strang overview
         on the back of the cover.
 
         Returns:
             list: The numerical value of the alias cancellation loss,
-                  as well both loss components for analysis.
+                  as well as both loss components for analysis.
 
         """
         dec_lo, dec_hi, rec_lo, rec_hi = self.filter_bank
         m1 = torch.tensor([-1], device=dec_lo.device, dtype=dec_lo.dtype)
         length = dec_lo.shape[0]
         mask = torch.tensor(
             [torch.pow(m1, n) for n in range(length)][::-1],
@@ -83,15 +83,15 @@
 
         Implementation of the ac-loss as described
         on page 104 of Strang+Nguyen.
         F0(z)H0(-z) + F1(z)H1(-z) = 0
 
         Returns:
             list: The numerical value of the alias cancellation loss,
-                  as well both loss components for analysis.
+                  as well as both loss components for analysis.
 
         """
         dec_lo, dec_hi, rec_lo, rec_hi = self.filter_bank
         m1 = torch.tensor([-1], device=dec_lo.device, dtype=dec_lo.dtype)
         length = dec_lo.shape[0]
         mask = torch.tensor(
             [torch.pow(m1, n) for n in range(length)][::-1],
@@ -119,30 +119,30 @@
         return torch.sum(errs), p_test, zeros
 
     def perfect_reconstruction_loss(
         self,
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """Return the perfect reconstruction loss.
 
-        Strang 107: Assuming alias cancellation holds:
-        P(z) = F(z)H(z)
-        Product filter P(z) + P(-z) = 2.
-        However since alias cancellation is implemented as soft constraint:
-        P_0 + P_1 = 2
-        Somehow numpy and torch implement convolution differently.
-        For some reason the machine learning people call cross-correlation
-        convolution.
-        https://discuss.pytorch.org/t/numpy-convolve-and-conv1d-in-pytorch/12172
-        Therefore for true convolution one element needs to be flipped.
-
         Returns:
             list: The numerical value of the alias cancellation loss,
                   as well as both intermediate values for analysis.
 
         """
+        # Strang 107: Assuming alias cancellation holds:
+        # P(z) = F(z)H(z)
+        # Product filter P(z) + P(-z) = 2.
+        # However, since alias cancellation is implemented as a soft constraint:
+        # P_0 + P_1 = 2
+        # Somehow NumPy and PyTorch implement convolution differently.
+        # For some reason, the machine learning people call cross-correlation
+        # convolution.
+        # https://discuss.pytorch.org/t/numpy-convolve-and-conv1d-in-pytorch/12172
+        # Therefore for true convolution, one element needs to be flipped.
+
         dec_lo, dec_hi, rec_lo, rec_hi = self.filter_bank
         # polynomial multiplication is convolution, compute p(z):
         pad = dec_lo.shape[0] - 1
         p_lo = torch.nn.functional.conv1d(
             dec_lo.unsqueeze(0).unsqueeze(0),
             torch.flip(rec_lo, [-1]).unsqueeze(0).unsqueeze(0),
             padding=pad,
@@ -278,15 +278,15 @@
         err = res - test
         return torch.sum(err * err)
 
     def filt_bank_orthogonality_loss(self) -> torch.Tensor:
         """Return a Jensen+Harbo inspired soft orthogonality loss.
 
         On Page 79 of the Book Ripples in Mathematics
-        by Jensen la Cour-Harbo the constraint
+        by Jensen la Cour-Harbo, the constraint
         g0[k] = h0[-k] and g1[k] = h1[-k] for orthogonal filters
         is presented. A measurement is implemented below.
 
         Returns:
             torch.Tensor: A tensor with the orthogonality constraint value.
         """
         eq0 = self.dec_lo - self.rec_lo.flip(-1)
```

### Comparing `ptwt-0.1.5/src/ptwt.egg-info/PKG-INFO` & `ptwt-0.1.6/src/ptwt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ptwt
-Version: 0.1.5
+Version: 0.1.6
 Summary: Differentiable and gpu enabled fast wavelet transforms in PyTorch
 Home-page: https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 Download-URL: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
-Author: Moritz Wolter
+Author: Moritz Wolter and Felix Blanke
 Author-email: moritz@wolter.tech
-Maintainer: Moritz Wolter
+Maintainer: Moritz Wolter and Felix Blanke
 Maintainer-email: moritz@wolter.tech
 License: EUPL-1.2
 Project-URL: Bug Tracker, https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
 Project-URL: Source Code, https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ********************************
-Pytorch Wavelet Toolbox (`ptwt`)
+Pytorch Wavelet Toolbox (`ptwt`) 
 ********************************
 
 .. image:: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml/badge.svg 
     :target: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/actions/workflows/tests.yml
     :alt: GitHub Actions
 
 .. image:: https://readthedocs.org/projects/pytorch-wavelet-toolbox/badge/?version=latest
@@ -52,30 +52,28 @@
     :target: https://github.com/psf/black
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
-
-
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
 - ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
 - ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
 - 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
 - ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_. In addition to boundary wavelets, we provide GPU and gradient support via a PyTorch backend.
 Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
@@ -112,23 +110,23 @@
   # invert the fwt.
   print(ptwt.waverec(ptwt.wavedec(data_torch, wavelet, mode='zero'),
                      wavelet))
 
 
 The functions ``wavedec`` and ``waverec`` compute the 1d-fwt and its inverse.
 Internally both rely on ``conv1d``, and its transposed counterpart ``conv_transpose1d``
-from the ``torch.nn.functional`` module. This toolbox supports discrete wavelets
-see also ``pywt.wavelist(kind='discrete')``. I have tested
-Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, which are usually a good starting point. 
+from the ``torch.nn.functional`` module. This toolbox also supports discrete wavelets
+see ``pywt.wavelist(kind='discrete')``. I have tested
+Daubechies-Wavelets ``db-x`` and symlets ``sym-x``, are usually a good starting point. 
 
 **Two-dimensional transform**
 
 Analog to the 1d-case ``wavedec2`` and ``waverec2`` rely on 
 ``conv2d``, and its transposed counterpart ``conv_transpose2d``.
-To test an example run:
+To test an example, run:
 
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
@@ -138,14 +136,18 @@
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
 
+**Speed tests**
+
+Speed tests comparing our tools to related libraries are `available <https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/speed_tests/>`_.
+
 
 **Boundary Wavelets with Sparse-Matrices**
 
 In addition to convolution and padding approaches,
 sparse-matrix-based code with boundary wavelet support is available.
 In contrast to padding, boundary wavelets do not add extra pixels at 
 the edges.
@@ -205,29 +207,29 @@
 
 
 to run all existing tests.
 
 Citation
 """"""""
 
-If you use this work in a scientific context please cite:
+If you use this work in a scientific context, please cite the following:
 
 .. code-block::
 
   @phdthesis{handle:20.500.11811/9245,
     urn: https://nbn-resolving.org/urn:nbn:de:hbz:5-63361,
     author = {{Moritz Wolter}},
     title = {Frequency Domain Methods in Recurrent Neural Networks for Sequential Data Processing},
     school = {Rheinische Friedrich-Wilhelms-Universität Bonn},
     year = 2021,
     month = jul,
     url = {https://hdl.handle.net/20.500.11811/9245}
   }
 
-If you use the boundary wavelet support please additionally cite:
+If you use the boundary wavelet support, please additionally cite:
 
 .. code-block::
 
   @thesis{Blanke2021,
     author = {Felix Blanke},
     title = {{Randbehandlung bei Wavelets für Faltungsnetzwerke}},
     type = {Bachelor's Thesis},
```

### Comparing `ptwt-0.1.5/src/ptwt.egg-info/SOURCES.txt` & `ptwt-0.1.6/src/ptwt.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 src/ptwt/__init__.py
+src/ptwt/_stationary_transform.py
 src/ptwt/_util.py
 src/ptwt/continuous_transform.py
 src/ptwt/conv_transform.py
 src/ptwt/conv_transform_2.py
 src/ptwt/conv_transform_3.py
 src/ptwt/matmul_transform.py
 src/ptwt/matmul_transform_2.py
@@ -27,9 +28,10 @@
 tests/test_jit.py
 tests/test_matrix_fwt.py
 tests/test_matrix_fwt_2.py
 tests/test_matrix_fwt_3.py
 tests/test_packets.py
 tests/test_separable_conv_fwt.py
 tests/test_sparse_math.py
+tests/test_swt.py
 tests/test_util.py
 tests/test_wavelet.py
```

### Comparing `ptwt-0.1.5/tests/test_convolution_fwt.py` & `ptwt-0.1.6/tests/test_convolution_fwt.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 from tests._mackey_glass import MackeyGenerator
 
 
 @pytest.mark.parametrize("wavelet_string", ["db1", "db2", "db3", "db4", "db5", "sym5"])
 @pytest.mark.parametrize("level", [1, 2, None])
 @pytest.mark.parametrize("length", [64, 65])
 @pytest.mark.parametrize("batch_size", [1, 3])
-@pytest.mark.parametrize("mode", ["reflect", "zero", "constant", "periodic"])
+@pytest.mark.parametrize(
+    "mode", ["reflect", "zero", "constant", "periodic", "symmetric"]
+)
 @pytest.mark.parametrize("dtype", [torch.float32, torch.float64])
-def test_conv_fwt(wavelet_string, level, mode, length, batch_size, dtype):
+def test_conv_fwt1d(wavelet_string, level, mode, length, batch_size, dtype):
     """Test multiple convolution fwt, for various levels and padding options."""
     generator = MackeyGenerator(
         batch_size=batch_size, tmax=length, delta_t=1, device="cpu"
     )
-
     mackey_data_1 = torch.squeeze(generator(), -1).type(dtype)
     wavelet = pywt.Wavelet(wavelet_string)
     ptcoeff = wavedec(mackey_data_1, wavelet, level=level, mode=mode)
     cptcoeff = torch.cat(ptcoeff, -1)
     py_list = []
     for b_el in range(batch_size):
         py_list.append(
@@ -48,14 +49,31 @@
     assert np.allclose(
         cptcoeff.numpy(), py_coeff, atol=np.finfo(py_coeff.dtype).resolution
     )
     res = waverec(ptcoeff, wavelet)
     assert np.allclose(mackey_data_1.numpy(), res.numpy()[:, : mackey_data_1.shape[-1]])
 
 
+@pytest.mark.parametrize("size", [[5, 10, 64], [1, 1, 32]])
+@pytest.mark.parametrize("wavelet", ["haar", "db2"])
+def test_conv_fwt1d_channel(size, wavelet):
+    """Test channel dimension support."""
+    data = torch.randn(*size).type(torch.float64)
+    ptwt_coeff = wavedec(data, wavelet)
+    pywt_coeff = pywt.wavedec(data.numpy(), wavelet, mode="reflect")
+    assert all(
+        [
+            np.allclose(ptwtc.numpy(), pywtc)
+            for ptwtc, pywtc in zip(ptwt_coeff, pywt_coeff)
+        ]
+    )
+    rec = waverec(ptwt_coeff, wavelet)
+    assert np.allclose(data.numpy(), rec.numpy())
+
+
 def test_ripples_haar_lvl3():
     """Compute example from page 7 of Ripples in Mathematics, Jensen, la Cour-Harbo."""
 
     class _MyHaarFilterBank(object):
         @property
         def filter_bank(self):
             """Unscaled Haar wavelet filters."""
@@ -154,15 +172,17 @@
 
 @pytest.mark.slow
 @pytest.mark.parametrize(
     "wavelet_str", ["haar", "db2", "db3", "db4", "sym4", "rbio2.4", "coif3", "bior2.2"]
 )
 @pytest.mark.parametrize("level", [1, 2, None])
 @pytest.mark.parametrize("size", [(32, 32), (32, 64), (64, 32), (31, 31)])
-@pytest.mark.parametrize("mode", ["reflect", "zero", "constant", "periodic"])
+@pytest.mark.parametrize(
+    "mode", ["reflect", "zero", "constant", "periodic", "symmetric"]
+)
 def test_2d_wavedec_rec(wavelet_str, level, size, mode):
     """Ensure pywt.wavedec2 and ptwt.wavedec2 produce the same coefficients.
 
     wavedec2 and waverec2 must invert each other.
     """
     face = np.transpose(
         datasets.face()[256 : (512 + size[0]), 256 : (512 + size[1])], [2, 0, 1]
@@ -184,26 +204,50 @@
     flat_coeff_list_ptwt = torch.cat(_flatten_2d_coeff_lst(coeff2d), -1)
     assert np.allclose(flat_coeff_list_pywt, flat_coeff_list_ptwt.numpy())
     rec = waverec2(coeff2d, wavelet)
     rec = rec.numpy().squeeze()
     assert np.allclose(face, rec[:, : face.shape[1], : face.shape[2]])
 
 
+@pytest.mark.parametrize(
+    "size", [(50, 20, 128, 128), (49, 21, 128, 128), (4, 5, 64, 64)]
+)
+@pytest.mark.parametrize("level", [1, 3, None])
+@pytest.mark.parametrize("wavelet", ["haar", "db2", "sym3"])
+def test_input_4d(size, level, wavelet):
+    """Test the error for 4d inputs to wavedec2."""
+    data = torch.randn(*size).type(torch.float64)
+
+    pt_res = wavedec2(data, wavelet=wavelet, level=level, mode="reflect")
+    pywt_res = pywt.wavedec2(data.numpy(), wavelet=wavelet, level=level, mode="reflect")
+    rec = waverec2(pt_res, wavelet)
+
+    # test coefficients
+    for ptwtcs, pywtcs in zip(pt_res, pywt_res):
+        if isinstance(ptwtcs, tuple):
+            assert all(
+                (
+                    np.allclose(ptwtc.numpy(), pywtc)
+                    for ptwtc, pywtc in zip(ptwtcs, pywtcs)
+                )
+            )
+        else:
+            assert np.allclose(ptwtcs, pywtcs)
+
+    # test reconstruction.
+    assert np.allclose(
+        data.numpy(), rec.numpy()[..., : data.shape[-2], : data.shape[-1]]
+    )
+
+
 @pytest.mark.parametrize("padding_str", ["invalid_padding_name"])
 def test_incorrect_padding(padding_str):
     """Test expected errors for an invalid padding name."""
     with pytest.raises(ValueError):
         _ = _translate_boundary_strings(padding_str)
 
 
-def test_input_4d_dimension_error():
-    """Test the error for 4d inputs to wavedec2."""
-    with pytest.raises(ValueError):
-        data = torch.randn(50, 20, 128, 128)
-        wavedec2(data, "haar", 4)
-
-
 def test_input_1d_dimension_error():
     """Test the error for 1d inputs to wavedec2."""
     with pytest.raises(ValueError):
         data = torch.randn(50)
         wavedec2(data, "haar", 4)
```

### Comparing `ptwt-0.1.5/tests/test_convolution_fwt_3.py` & `ptwt-0.1.6/tests/test_convolution_fwt_3.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         (3, 31, 31, 31),
         (3, 32, 32, 32),
         (3, 31, 32, 33),
     ],
 )
 @pytest.mark.parametrize("wavelet", ["haar", "db2", "db4"])
 @pytest.mark.parametrize("level", [1, 2, None])
-@pytest.mark.parametrize("mode", ["zero", "constant", "periodic"])
+@pytest.mark.parametrize("mode", ["reflect", "zero", "constant", "periodic", "symmetric"])
 def test_waverec3(shape: list, wavelet: str, level: int, mode: str) -> None:
     """Ensure the 3d analysis transform is invertible."""
     data = np.random.randn(*shape)
     data = torch.from_numpy(data)
     ptwc = ptwt.wavedec3(data, wavelet, level=level, mode=mode)
     batch_list = []
     for batch_no in range(data.shape[0]):
```

### Comparing `ptwt-0.1.5/tests/test_cwt.py` & `ptwt-0.1.6/tests/test_cwt.py`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.5/tests/test_jit.py` & `ptwt-0.1.6/tests/test_jit.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pytest
 import pywt
 import torch
 from scipy import signal
 
 import src.ptwt as ptwt
-from ptwt.continuous_transform import _ShannonWavelet
+from src.ptwt.continuous_transform import _ShannonWavelet
 from tests._mackey_glass import MackeyGenerator
 
 
 class WaveletTuple(NamedTuple):
     """Replaces namedtuple("Wavelet", ("dec_lo", "dec_hi", "rec_lo", "rec_hi"))."""
 
     dec_lo: torch.Tensor
@@ -146,20 +146,20 @@
     wavelet = pywt.Wavelet("db4")
     coeff = _to_jit_wavedec_3(data, wavelet)
     rec = _to_jit_waverec_3(coeff, wavelet)
     assert np.allclose(rec.squeeze(1).numpy(), data.numpy())
 
     wavelet = _set_up_wavelet_tuple(wavelet, dtype=torch.float64)
     with pytest.warns(Warning):
-        jit_wavedec2 = torch.jit.trace(
+        jit_wavedec3 = torch.jit.trace(
             _to_jit_wavedec_3,
             (data, wavelet),
             strict=False,
         )
-        jit_ptcoeff = jit_wavedec2(data, wavelet)
+        jit_ptcoeff = jit_wavedec3(data, wavelet)
         # unstack the lists.
         jit_waverec = torch.jit.trace(_to_jit_waverec_3, (jit_ptcoeff, wavelet))
         rec = jit_waverec(jit_ptcoeff, wavelet)
     assert np.allclose(rec.squeeze(1).numpy(), data.numpy(), atol=1e-7)
 
 
 def _to_jit_cwt(sig):
```

### Comparing `ptwt-0.1.5/tests/test_matrix_fwt.py` & `ptwt-0.1.6/tests/test_matrix_fwt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test the fwt and ifwt matrices."""
 # Written by moritz ( @ wolter.tech ) in 2021
+from typing import List
+
 import numpy as np
 import pytest
 import pywt
 import torch
 
 from src.ptwt.matmul_transform import (
     MatrixWavedec,
@@ -60,20 +62,20 @@
     reconstructed_data = matrix_waverec(coeffs_matfwt)
     assert np.allclose(pt_data.cpu().numpy(), reconstructed_data.cpu().numpy())
 
 
 @pytest.mark.slow
 @pytest.mark.parametrize("level", [1, 2, 3, 4, None])
 @pytest.mark.parametrize("wavelet", ["db2", "db3", "db4", "sym5"])
-def test_fwt_ifwt_mackey(level: int, wavelet: str) -> None:
+@pytest.mark.parametrize("size", [[2, 256], [2, 3, 256], [1, 1, 128]])
+def test_1d_matrix_fwt_ifwt(level: int, wavelet: str, size: List[int]) -> None:
     """Test multiple wavelets and levels for a long signal."""
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     wavelet = pywt.Wavelet(wavelet)
-    generator = MackeyGenerator(batch_size=2, tmax=512, delta_t=1, device=device)
-    pt_data = torch.squeeze(generator()).type(torch.float64)
+    pt_data = torch.randn(*size, device=device).type(torch.float64)
     matrix_wavedec = MatrixWavedec(wavelet, level)
     coeffs_mat_max = matrix_wavedec(pt_data)
     matrix_waverec = MatrixWaverec(wavelet)
     reconstructed_data = matrix_waverec(coeffs_mat_max)
     assert np.allclose(reconstructed_data.cpu().numpy(), pt_data.cpu().numpy())
 
 
@@ -175,7 +177,35 @@
                 test_mat = torch.sparse.mm(
                     matrix_waverec.sparse_ifwt_operator,
                     matrix_wavedec.sparse_fwt_operator,
                 )
                 assert np.allclose(
                     test_mat.to_dense().numpy(), np.eye(test_mat.shape[0])
                 )
+
+
+def test_4d_input_to_1d_transform_dimension_error():
+    """Test the error for 1d inputs to the MatrixWavedec __call__."""
+    with pytest.raises(ValueError):
+        data = torch.randn(50, 50, 50, 50)
+        matrix_wavedec_1d = MatrixWavedec("haar", 4)
+        matrix_wavedec_1d(data)
+
+
+@pytest.mark.parametrize("size", [[2, 3, 32], [5, 32], [32], [1, 1, 64]])
+def test_matrix1d_batch_channel(size):
+    """Test if batch and channel support works as expected."""
+    data = torch.randn(*size).type(torch.float64)
+    matrix_wavedec_1d = MatrixWavedec("haar", 3)
+    ptwt_coeff = matrix_wavedec_1d(data)
+    pywt_coeff = pywt.wavedec(data.numpy(), "haar", level=3)
+
+    test = [
+        np.allclose(ptwtcs.numpy(), pywtcs)
+        for ptwtcs, pywtcs in zip(ptwt_coeff, pywt_coeff)
+    ]
+    assert all(test)
+
+    matrix_waverec_2d = MatrixWaverec("haar")
+    rec = matrix_waverec_2d(ptwt_coeff)
+
+    assert np.allclose(data.numpy(), rec.numpy())
```

### Comparing `ptwt-0.1.5/tests/test_matrix_fwt_2.py` & `ptwt-0.1.6/tests/test_matrix_fwt_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test code for the boundary wavelets."""
+"""Test code for the 2d boundary wavelets."""
 # Created by moritz ( wolter@cs.uni-bonn.de ), 08.09.21
 import numpy as np
 import pytest
 import pywt
 import scipy.signal
 import torch
 
@@ -182,14 +182,34 @@
         [
             np.allclose(pywt_test, ptwt_test.numpy())
             for pywt_test, ptwt_test in zip(pywtres, ptwtres)
         ]
     )
 
 
+@pytest.mark.parametrize("size", [[3, 2, 32, 32], [4, 32, 32], [1, 1, 32, 32]])
+def test_batch_channel_2d_haar(size):
+    """Test matrix fwt-2d leading channel and batch dimension code."""
+    signal = torch.randn(*size).type(torch.float64)
+    ptwt_coeff = MatrixWavedec2("haar", 2, separable=False)(signal)
+    pywt_coeff = pywt.wavedec2(signal, "haar", level=2)
+
+    for ptwtc, pywtc in zip(ptwt_coeff, pywt_coeff):
+        if isinstance(ptwtc, torch.Tensor):
+            assert np.allclose(ptwtc.numpy(), pywtc)
+        else:
+            test = [
+                np.allclose(ptwtcel, pywtcel) for ptwtcel, pywtcel in zip(ptwtc, pywtc)
+            ]
+            assert all(test)
+
+    rec = MatrixWaverec2("haar", separable=False)(ptwt_coeff)
+    assert np.allclose(rec.numpy(), signal.numpy())
+
+
 @pytest.mark.parametrize("operator", [MatrixWavedec2, MatrixWavedec])
 def test_empty_operators(operator) -> None:
     """Check if the error is thrown properly if no matrix was ever built."""
     if operator is MatrixWavedec2:
         matrixfwt = operator("haar", separable=False)
     else:
         matrixfwt = operator("haar")
```

### Comparing `ptwt-0.1.5/tests/test_matrix_fwt_3.py` & `ptwt-0.1.6/tests/test_matrix_fwt_3.py`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.5/tests/test_packets.py` & `ptwt-0.1.6/tests/test_packets.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,37 +287,36 @@
 
     with pytest.raises(KeyError):
         twp["a" * 100]
 
 
 @pytest.mark.parametrize("level", [1, 2, 3])
 @pytest.mark.parametrize("base_key", ["a", "d"])
-@pytest.mark.parametrize("length", [63, 64, 128])
-@pytest.mark.parametrize("batch_size", [1, 2])
+@pytest.mark.parametrize("shape", [[1, 63], [3, 2, 64], [128]])
 @pytest.mark.parametrize("wavelet", ["db1", "db2", "sym4"])
-def test_inverse_packet_1d(level, base_key, length, batch_size, wavelet):
+def test_inverse_packet_1d(level, base_key, shape, wavelet):
     """Test the 1d reconstruction code."""
-    signal = np.random.randn(batch_size, length)
+    signal = np.random.randn(*shape)
     mode = "reflect"
     wp = pywt.WaveletPacket(signal, wavelet, mode=mode, maxlevel=level)
     ptwp = WaveletPacket(torch.from_numpy(signal), wavelet, mode=mode, maxlevel=level)
     wp[base_key * level].data *= 0
     ptwp[base_key * level].data *= 0
     wp.reconstruct(update=True)
     ptwp.reconstruct()
-    assert np.allclose(wp[""].data, ptwp[""].numpy()[:, :length])
+    assert np.allclose(wp[""].data, ptwp[""].numpy()[..., : shape[-1]])
 
 
 @pytest.mark.parametrize("level", [1, 3])
 @pytest.mark.parametrize("base_key", ["a", "h", "d"])
-@pytest.mark.parametrize("size", [(1, 32, 32), (2, 31, 64)])
+@pytest.mark.parametrize("size", [(1, 32, 32), (2, 1, 31, 64)])
 @pytest.mark.parametrize("wavelet", ["db1", "db2", "sym4"])
 def test_inverse_packet_2d(level, base_key, size, wavelet):
     """Test the 2d reconstruction code."""
-    signal = np.random.randn(size[0], size[1], size[2])
+    signal = np.random.randn(*size)
     mode = "reflect"
     wp = pywt.WaveletPacket2D(signal, wavelet, mode=mode, maxlevel=level)
     ptwp = WaveletPacket2D(torch.from_numpy(signal), wavelet, mode=mode, maxlevel=level)
     wp[base_key * level].data *= 0
     ptwp[base_key * level].data *= 0
     wp.reconstruct(update=True)
     ptwp.reconstruct()
```

### Comparing `ptwt-0.1.5/tests/test_separable_conv_fwt.py` & `ptwt-0.1.6/tests/test_separable_conv_fwt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Separable transform test code."""
 
 import numpy as np
 import pytest
 import pywt
 import torch
 
-from src.ptwt.conv_transform import wavedec
 from src.ptwt.matmul_transform_2 import MatrixWavedec2
 from src.ptwt.matmul_transform_3 import MatrixWavedec3
 from src.ptwt.separable_conv_transform import (
-    _fswavedec,
-    _fswaverec,
     _separable_conv_wavedecn,
     _separable_conv_waverecn,
     fswavedec2,
     fswavedec3,
     fswaverec2,
     fswaverec3,
 )
@@ -59,24 +56,14 @@
         ]
     )
 
     rec = _separable_conv_waverecn(ptwt_res, "haar")
     assert np.allclose(rec.numpy(), data)
 
 
-@pytest.mark.parametrize("shape", [(5, 64), (5, 65), (5, 29)])
-@pytest.mark.parametrize("wavelet", ["haar", "db3", "sym5"])
-def test_example_fs1d(shape, wavelet):
-    """Test 1d fully separable padding."""
-    data = torch.randn(*shape).type(torch.float64)
-    coeff = _fswavedec(data, wavelet, level=2)
-    rec = _fswaverec(coeff, wavelet)
-    assert np.allclose(data.numpy(), rec[: shape[0], : shape[1]].numpy())
-
-
 @pytest.mark.parametrize("shape", [(5, 64, 64), (5, 65, 65), (5, 29, 29)])
 @pytest.mark.parametrize("wavelet", ["haar", "db3", "sym5"])
 def test_example_fs2d(shape, wavelet):
     """Test 2d fully separable padding."""
     data = torch.randn(*shape).type(torch.float64)
     coeff = fswavedec2(data, wavelet, level=2)
     rec = fswaverec2(coeff, wavelet)
@@ -89,35 +76,20 @@
     """Test 3d fully separable padding."""
     data = torch.randn(*shape).type(torch.float64)
     coeff = fswavedec3(data, wavelet, level=2)
     rec = fswaverec3(coeff, wavelet)
     assert np.allclose(data.numpy(), rec[[slice(0, s) for s in shape]].numpy())
 
 
-@pytest.mark.parametrize("shape", [(5, 64), (5, 65), (5, 29)])
-@pytest.mark.parametrize("wavelet", ["haar", "db3", "sym5"])
-def test_conv_convsep1d(shape, wavelet):
-    """Test 1d fully separable padding."""
-    data = torch.randn(*shape).type(torch.float64)
-    coeff = _fswavedec(data, wavelet, level=2)
-    coeff2 = wavedec(data, wavelet, level=2)
-    assert np.allclose(coeff[0].numpy(), coeff2[0].numpy())
-    assert all(
-        np.allclose(c["d"].numpy(), c2.numpy()) for c, c2 in zip(coeff[1:], coeff2[1:])
-    )
-    rec = _fswaverec(coeff, wavelet)
-    assert np.allclose(data.numpy(), rec[: shape[0], : shape[1]].numpy())
-
-
 # test separable conv and mamul consistency for the Haar case.
 @pytest.mark.slow
 @pytest.mark.parametrize("level", [1, 2, 3, None])
-def test_conv_mm_2d(level):
+@pytest.mark.parametrize("shape", [[5, 128, 128], [3, 2, 64, 64], [1, 1, 64, 64]])
+def test_conv_mm_2d(level, shape):
     """Compare mm and conv fully separable results."""
-    shape = (5, 128, 128)
     data = torch.randn(*shape).type(torch.float64)
     fs_conv_coeff = fswavedec2(data, "haar", level=level)
     fs_mm_coeff = MatrixWavedec2("haar", level, separable=True)(data)
     # compare coefficients
     assert len(fs_conv_coeff) == len(fs_mm_coeff)
     for c_conv, c_mm in zip(fs_conv_coeff, fs_mm_coeff):
         if isinstance(c_conv, torch.Tensor):
```

### Comparing `ptwt-0.1.5/tests/test_sparse_math.py` & `ptwt-0.1.6/tests/test_sparse_math.py`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.5/tests/test_wavelet.py` & `ptwt-0.1.6/tests/test_wavelet.py`

 * *Files identical despite different names*

