# Comparing `tmp/openjij-0.7.3.tar.gz` & `tmp/openjij-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjij-0.7.3.tar", last modified: Fri Jun 16 07:14:32 2023, max compression
+gzip compressed data, was "openjij-0.7.4.tar", last modified: Fri Jul 28 04:08:04 2023, max compression
```

## Comparing `openjij-0.7.3.tar` & `openjij-0.7.4.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-16 07:14:14.000000 openjij-0.7.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 07:14:14.000000 openjij-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 07:14:14.000000 openjij-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-16 07:14:14.000000 openjij-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-16 07:14:32.988612 openjij-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-16 07:14:14.000000 openjij-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/FindGcov.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/FindLcov.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/Findcodecov.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/GenerateDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/PythonAutoDetectOSX.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 07:14:14.000000 openjij-0.7.3/cmake/llvm-cov-wrapper
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-16 07:14:14.000000 openjij-0.7.3/doc-requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/external/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 07:14:14.000000 openjij-0.7.3/external/cimod.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-16 07:14:14.000000 openjij-0.7.3/external/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-16 07:14:14.000000 openjij-0.7.3/external/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 07:14:14.000000 openjij-0.7.3/external/json.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 07:14:14.000000 openjij-0.7.3/external/pybind11-json.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-16 07:14:14.000000 openjij-0.7.3/include/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.968611 openjij-0.7.3/include/openjij/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/include/openjij/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/algorithm/algorithm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/algorithm/all.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/include/openjij/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/binary_polynomial_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/chimera.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/converter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/csr_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/ising_polynomial_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.972611 openjij-0.7.3/include/openjij/graph/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/json/parse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/graph/square.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/result/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/result/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/result/get_solution.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/sampler/sa_sampler.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/system/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/binary_polynomial_sa_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/classical_ising.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/classical_ising_polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/continuous_time_ising.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/system/gpu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/kernel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/gpu/chimera_gpu_classical.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/gpu/chimera_gpu_transverse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/ising_polynomial_sa_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23994 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/k_local_polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/sa_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/system/transverse_ising.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.976611 openjij-0.7.3/include/openjij/updater/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/continuous_time_swendsen_wang.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/k_local.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/single_spin_flip.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/updater/swendsen_wang.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/include/openjij/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/create_geometric_progression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/disable_eigen_warning.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/eigen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/include/openjij/utility/fmath/
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/fmath/fmath.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/include/openjij/utility/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/gpu/cublas.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/gpu/handle_error.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/gpu/memory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/index_type.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/insert_or_assign.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/memory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/pairhash.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/random.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/schedule_list.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/thres_hold.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-16 07:14:14.000000 openjij-0.7.3/include/openjij/utility/union_find.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/openjij/
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/compile_config.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/declare.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/openjij/model/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/model/chimera_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/model/king_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.984611 openjij-0.7.3/openjij/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/base_sa_sample_hubo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.984611 openjij-0.7.3/openjij/sampler/chimera_gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/chimera_gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/chimera_gpu/base_gpu_chimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/csqa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    24475 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/sa_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/sampler/sqa_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.984611 openjij-0.7.3/openjij/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/cxx_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/res_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/utils/time_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-16 07:14:14.000000 openjij-0.7.3/openjij/variable_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.980611 openjij-0.7.3/openjij.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:14:32.000000 openjij-0.7.3/openjij.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-16 07:14:14.000000 openjij-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-16 07:14:32.988612 openjij-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 07:14:14.000000 openjij-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.984611 openjij-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.984611 openjij-0.7.3/tests/cxxtest/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/cxxtest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/tests/cxxtest/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/graph/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/graph/polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/graph/quadratic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    36692 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/polynomial_test.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/tests/cxxtest/result/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/result/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/result/result.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/tests/cxxtest/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/k_local.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/quadraitc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/tests/cxxtest/system/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/classical_ising.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/system/k_local.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/testcase.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:14:32.988612 openjij-0.7.3/tests/cxxtest/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/utility/all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/utility/eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/utility/gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/cxxtest/utility/union_find.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_cxx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    59737 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_hubo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_sqa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-16 07:14:14.000000 openjij-0.7.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.500226 openjij-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-28 04:07:46.000000 openjij-0.7.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 04:07:46.000000 openjij-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 04:07:46.000000 openjij-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-28 04:07:46.000000 openjij-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-28 04:08:04.500226 openjij-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-28 04:07:46.000000 openjij-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.468226 openjij-0.7.4/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/FindGcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/FindLcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/Findcodecov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/GenerateDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/PythonAutoDetectOSX.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-28 04:07:46.000000 openjij-0.7.4/cmake/llvm-cov-wrapper
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 04:07:46.000000 openjij-0.7.4/doc-requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.468226 openjij-0.7.4/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 04:07:46.000000 openjij-0.7.4/external/cimod.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-28 04:07:46.000000 openjij-0.7.4/external/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-28 04:07:46.000000 openjij-0.7.4/external/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 04:07:46.000000 openjij-0.7.4/external/json.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-28 04:07:46.000000 openjij-0.7.4/external/pybind11-json.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.468226 openjij-0.7.4/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-28 04:07:46.000000 openjij-0.7.4/include/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.460226 openjij-0.7.4/include/openjij/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.472226 openjij-0.7.4/include/openjij/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/algorithm/algorithm.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/algorithm/all.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.472226 openjij-0.7.4/include/openjij/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/binary_polynomial_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/chimera.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/converter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/csr_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/ising_polynomial_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.476226 openjij-0.7.4/include/openjij/graph/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/json/parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/graph/square.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.476226 openjij-0.7.4/include/openjij/result/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/result/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/result/get_solution.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.476226 openjij-0.7.4/include/openjij/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/sampler/sa_sampler.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.480226 openjij-0.7.4/include/openjij/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/binary_polynomial_sa_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/classical_ising.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/classical_ising_polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/continuous_time_ising.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.480226 openjij-0.7.4/include/openjij/system/gpu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.480226 openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/kernel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/gpu/chimera_gpu_classical.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/gpu/chimera_gpu_transverse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/ising_polynomial_sa_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23994 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/k_local_polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/sa_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/system/transverse_ising.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.480226 openjij-0.7.4/include/openjij/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18946 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/continuous_time_swendsen_wang.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/k_local.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/single_spin_flip.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/updater/swendsen_wang.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.484226 openjij-0.7.4/include/openjij/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/create_geometric_progression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/disable_eigen_warning.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/eigen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.484226 openjij-0.7.4/include/openjij/utility/fmath/
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/fmath/fmath.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.488226 openjij-0.7.4/include/openjij/utility/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/gpu/cublas.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/gpu/handle_error.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/gpu/memory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/index_type.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/insert_or_assign.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/memory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/pairhash.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/random.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/schedule_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/thres_hold.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 04:07:46.000000 openjij-0.7.4/include/openjij/utility/union_find.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.488226 openjij-0.7.4/openjij/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/compile_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/declare.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.492226 openjij-0.7.4/openjij/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/model/chimera_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/model/king_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.492226 openjij-0.7.4/openjij/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/base_sa_sample_hubo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.492226 openjij-0.7.4/openjij/sampler/chimera_gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/chimera_gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/csqa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24475 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/sa_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/sampler/sqa_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/openjij/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/cxx_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/res_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/utils/time_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 04:07:46.000000 openjij-0.7.4/openjij/variable_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.492226 openjij-0.7.4/openjij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 04:08:04.000000 openjij-0.7.4/openjij.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-28 04:07:46.000000 openjij-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-28 04:08:04.500226 openjij-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-28 04:07:46.000000 openjij-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/tests/cxxtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/cxxtest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/tests/cxxtest/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/graph/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/graph/polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/graph/quadratic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36692 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/polynomial_test.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/tests/cxxtest/result/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/result/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/result/result.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.496226 openjij-0.7.4/tests/cxxtest/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/k_local.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/quadraitc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.500226 openjij-0.7.4/tests/cxxtest/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/classical_ising.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/system/k_local.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/testcase.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:08:04.500226 openjij-0.7.4/tests/cxxtest/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/utility/all.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/utility/eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/utility/gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/cxxtest/utility/union_find.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27147 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_cxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59737 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_hubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_sqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-28 04:07:46.000000 openjij-0.7.4/tests/test_utils.py
```

### Comparing `openjij-0.7.3/CMakeLists.txt` & `openjij-0.7.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/LICENSE` & `openjij-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/MANIFEST.in` & `openjij-0.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/PKG-INFO` & `openjij-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: openjij
-Version: 0.7.3
+Version: 0.7.4
 Summary: Framework for the Ising model and QUBO.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@openjij.org
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/OpenJij
 Project-URL: Documentation, https://openjij.github.io/OpenJij
 Project-URL: Reference, https://ref.openjij.org/index.html
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenJij : Framework for the Ising model and QUBO.
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/openjij.svg)](https://pypi.python.org/pypi/openjij/)
```

### Comparing `openjij-0.7.3/README.md` & `openjij-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/FindGcov.cmake` & `openjij-0.7.4/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/FindLcov.cmake` & `openjij-0.7.4/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/Findcodecov.cmake` & `openjij-0.7.4/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/GenerateDocs.cmake` & `openjij-0.7.4/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/PythonAutoDetectOSX.cmake` & `openjij-0.7.4/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/cmake/llvm-cov-wrapper` & `openjij-0.7.4/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/doc-requirements.in` & `openjij-0.7.4/doc-requirements.in`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/external/cimod.cmake` & `openjij-0.7.4/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/external/eigen.cmake` & `openjij-0.7.4/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/external/googletest.cmake` & `openjij-0.7.4/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/external/json.cmake` & `openjij-0.7.4/external/json.cmake`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/CMakeLists.txt` & `openjij-0.7.4/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/algorithm/algorithm.hpp` & `openjij-0.7.4/include/openjij/algorithm/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/algorithm/all.hpp` & `openjij-0.7.4/include/openjij/algorithm/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/all.hpp` & `openjij-0.7.4/include/openjij/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/binary_polynomial_model.hpp` & `openjij-0.7.4/include/openjij/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/chimera.hpp` & `openjij-0.7.4/include/openjij/graph/chimera.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/converter.hpp` & `openjij-0.7.4/include/openjij/graph/converter.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/csr_sparse.hpp` & `openjij-0.7.4/include/openjij/graph/csr_sparse.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/dense.hpp` & `openjij-0.7.4/include/openjij/graph/dense.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/graph.hpp` & `openjij-0.7.4/include/openjij/graph/graph.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/ising_polynomial_model.hpp` & `openjij-0.7.4/include/openjij/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/json/parse.hpp` & `openjij-0.7.4/include/openjij/graph/json/parse.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/polynomial.hpp` & `openjij-0.7.4/include/openjij/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/sparse.hpp` & `openjij-0.7.4/include/openjij/graph/sparse.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/graph/square.hpp` & `openjij-0.7.4/include/openjij/graph/square.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/result/all.hpp` & `openjij-0.7.4/include/openjij/result/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/result/get_solution.hpp` & `openjij-0.7.4/include/openjij/result/get_solution.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/sampler/sa_sampler.hpp` & `openjij-0.7.4/include/openjij/sampler/sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/CMakeLists.txt` & `openjij-0.7.4/include/openjij/system/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/all.hpp` & `openjij-0.7.4/include/openjij/system/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/binary_polynomial_sa_system.hpp` & `openjij-0.7.4/include/openjij/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/classical_ising.hpp` & `openjij-0.7.4/include/openjij/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/classical_ising_polynomial.hpp` & `openjij-0.7.4/include/openjij/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/continuous_time_ising.hpp` & `openjij-0.7.4/include/openjij/system/continuous_time_ising.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/index.hpp` & `openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/index.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/kernel.cu` & `openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/kernel.cu`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/gpu/chimera_cuda/kernel.hpp` & `openjij-0.7.4/include/openjij/system/gpu/chimera_cuda/kernel.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/gpu/chimera_gpu_classical.hpp` & `openjij-0.7.4/include/openjij/system/gpu/chimera_gpu_classical.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/gpu/chimera_gpu_transverse.hpp` & `openjij-0.7.4/include/openjij/system/gpu/chimera_gpu_transverse.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/ising_polynomial_sa_system.hpp` & `openjij-0.7.4/include/openjij/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/k_local_polynomial.hpp` & `openjij-0.7.4/include/openjij/system/k_local_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/sa_system.hpp` & `openjij-0.7.4/include/openjij/system/sa_system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/system.hpp` & `openjij-0.7.4/include/openjij/system/system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/system/transverse_ising.hpp` & `openjij-0.7.4/include/openjij/system/transverse_ising.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/all.hpp` & `openjij-0.7.4/include/openjij/updater/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/continuous_time_swendsen_wang.hpp` & `openjij-0.7.4/include/openjij/updater/continuous_time_swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/gpu.hpp` & `openjij-0.7.4/include/openjij/updater/gpu.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/k_local.hpp` & `openjij-0.7.4/include/openjij/updater/k_local.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/single_spin_flip.hpp` & `openjij-0.7.4/include/openjij/updater/single_spin_flip.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/updater/swendsen_wang.hpp` & `openjij-0.7.4/include/openjij/updater/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/create_geometric_progression.hpp` & `openjij-0.7.4/include/openjij/utility/create_geometric_progression.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/disable_eigen_warning.hpp` & `openjij-0.7.4/include/openjij/utility/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/eigen.hpp` & `openjij-0.7.4/include/openjij/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/fmath/fmath.hpp` & `openjij-0.7.4/include/openjij/utility/fmath/fmath.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/gpu/cublas.hpp` & `openjij-0.7.4/include/openjij/utility/gpu/cublas.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/gpu/handle_error.hpp` & `openjij-0.7.4/include/openjij/utility/gpu/handle_error.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/gpu/memory.hpp` & `openjij-0.7.4/include/openjij/utility/gpu/memory.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/index_type.hpp` & `openjij-0.7.4/include/openjij/utility/index_type.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/insert_or_assign.hpp` & `openjij-0.7.4/include/openjij/utility/insert_or_assign.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/memory.hpp` & `openjij-0.7.4/include/openjij/utility/memory.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/pairhash.hpp` & `openjij-0.7.4/include/openjij/utility/pairhash.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/random.hpp` & `openjij-0.7.4/include/openjij/utility/random.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/schedule_list.hpp` & `openjij-0.7.4/include/openjij/utility/schedule_list.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/thres_hold.hpp` & `openjij-0.7.4/include/openjij/utility/thres_hold.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/type_traits.hpp` & `openjij-0.7.4/include/openjij/utility/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/include/openjij/utility/union_find.hpp` & `openjij-0.7.4/include/openjij/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/CMakeLists.txt` & `openjij-0.7.4/openjij/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/__init__.py` & `openjij-0.7.4/openjij/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/compile_config.hpp` & `openjij-0.7.4/openjij/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/declare.hpp` & `openjij-0.7.4/openjij/declare.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/main.cpp` & `openjij-0.7.4/openjij/main.cpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/model/__init__.py` & `openjij-0.7.4/openjij/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/model/chimera_model.py` & `openjij-0.7.4/openjij/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/model/king_graph.py` & `openjij-0.7.4/openjij/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/model/model.py` & `openjij-0.7.4/openjij/model/model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/base_sa_sample_hubo.py` & `openjij-0.7.4/openjij/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/chimera_gpu/base_gpu_chimera.py` & `openjij-0.7.4/openjij/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/chimera_gpu/gpu_sa_sampler.py` & `openjij-0.7.4/openjij/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py` & `openjij-0.7.4/openjij/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/csqa_sampler.py` & `openjij-0.7.4/openjij/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/response.py` & `openjij-0.7.4/openjij/sampler/response.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/sa_sampler.py` & `openjij-0.7.4/openjij/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/sampler.py` & `openjij-0.7.4/openjij/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/sampler/sqa_sampler.py` & `openjij-0.7.4/openjij/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/__init__.py` & `openjij-0.7.4/openjij/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/benchmark.py` & `openjij-0.7.4/openjij/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/cxx_cast.py` & `openjij-0.7.4/openjij/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/decorator.py` & `openjij-0.7.4/openjij/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/graph_utils.py` & `openjij-0.7.4/openjij/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/utils/res_convertor.py` & `openjij-0.7.4/openjij/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij/variable_type.py` & `openjij-0.7.4/openjij/variable_type.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/openjij.egg-info/PKG-INFO` & `openjij-0.7.4/openjij.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: openjij
-Version: 0.7.3
+Version: 0.7.4
 Summary: Framework for the Ising model and QUBO.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@openjij.org
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/OpenJij
 Project-URL: Documentation, https://openjij.github.io/OpenJij
 Project-URL: Reference, https://ref.openjij.org/index.html
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenJij : Framework for the Ising model and QUBO.
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/openjij.svg)](https://pypi.python.org/pypi/openjij/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/openjij.svg)](https://pypi.python.org/pypi/openjij/)
```

### Comparing `openjij-0.7.3/openjij.egg-info/SOURCES.txt` & `openjij-0.7.4/openjij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/pyproject.toml` & `openjij-0.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 ]
 reportImportCycles = 'warning'
 reportUnusedImport = 'warning'
 reportUnusedVariable =  'warning'
 reportDuplicateImport = 'warning'
 
 [tool.cibuildwheel]
-skip = ["cp36*", "cp311*", "*musllinux_x86_64", "*musllinux_aarch64", "pp*"]
+skip = ["cp36*", "cp37*", "cp311*", "*musllinux_x86_64", "*musllinux_aarch64", "pp*"]
 build-verbosity = 1
 dependency-versions = "latest"
 
 [tool.cibuildwheel.linux]
 archs = ["x86_64", "aarch64"]
 build-frontend = "build"
 #environment = "-CFLAGS='-march=haswell' -CXXFLAGS='-march=haswell' -FFLAGS='-march=haswell'"
```

### Comparing `openjij-0.7.3/setup.cfg` & `openjij-0.7.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 long_description_content_type = text/markdown
 license_files = LICENSE
 license = Apache License 2.0
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Intended Audience :: Science/Research
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
@@ -31,15 +30,15 @@
 	Operating System :: MacOS
 project_urls = 
 	Source=https://github.com/OpenJij/OpenJij
 	Documentation=https://openjij.github.io/OpenJij
 	Reference=https://ref.openjij.org/index.html
 
 [options]
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
 	numpy >=1.17.3, < 1.25.0
 	dimod < 0.13.0
 	scipy >= 1.7.3, < 1.11.0
 	requests >= 2.28.0, < 2.29.0
 	jij-cimod >= 1.4.42, < 1.5.0
 	typing-extensions >= 4.2.0
```

### Comparing `openjij-0.7.3/setup.py` & `openjij-0.7.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 try:
     from skbuild import setup
 except ImportError:
     from setuptools import setup
 
 setup_requires = [
     "numpy",
-    "pybind11 >=2.10.0, < 2.11.0",
+    "pybind11",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
 if any(arg in sys.argv for arg in ("pytest", "test")):
     setup_requires.append("pytest-runner")
```

### Comparing `openjij-0.7.3/tests/CMakeLists.txt` & `openjij-0.7.4/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/cxxtest.cpp` & `openjij-0.7.4/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/graph/all.hpp` & `openjij-0.7.4/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/graph/binary_polynomial_model.hpp` & `openjij-0.7.4/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/graph/ising_polynomial_model.hpp` & `openjij-0.7.4/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/graph/polynomial.hpp` & `openjij-0.7.4/tests/cxxtest/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/graph/quadratic.hpp` & `openjij-0.7.4/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/polynomial_test.hpp` & `openjij-0.7.4/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/result/all.hpp` & `openjij-0.7.4/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/result/result.hpp` & `openjij-0.7.4/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/all.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/gpu.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/k_local.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/polynomial.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/quadraitc.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/sampler/swendsen_wang.hpp` & `openjij-0.7.4/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/all.hpp` & `openjij-0.7.4/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `openjij-0.7.4/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/classical_ising.hpp` & `openjij-0.7.4/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/classical_ising_polynomial.hpp` & `openjij-0.7.4/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `openjij-0.7.4/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/system/k_local.hpp` & `openjij-0.7.4/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/testcase.hpp` & `openjij-0.7.4/tests/cxxtest/testcase.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/utility/all.hpp` & `openjij-0.7.4/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/utility/eigen.hpp` & `openjij-0.7.4/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/utility/gpu.hpp` & `openjij-0.7.4/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/cxxtest/utility/union_find.hpp` & `openjij-0.7.4/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_cxx.py` & `openjij-0.7.4/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_gpu.py` & `openjij-0.7.4/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_hubo.py` & `openjij-0.7.4/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_model.py` & `openjij-0.7.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_sampler.py` & `openjij-0.7.4/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_sqa.py` & `openjij-0.7.4/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `openjij-0.7.3/tests/test_utils.py` & `openjij-0.7.4/tests/test_utils.py`

 * *Files identical despite different names*

